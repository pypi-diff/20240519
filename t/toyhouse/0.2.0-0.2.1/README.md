# Comparing `tmp/toyhouse-0.2.0.tar.gz` & `tmp/toyhouse-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "toyhouse-0.2.0.tar", last modified: Sat Nov 18 03:45:06 2023, max compression
+gzip compressed data, was "toyhouse-0.2.1.tar", last modified: Sun May 19 03:19:17 2024, max compression
```

## Comparing `toyhouse-0.2.0.tar` & `toyhouse-0.2.1.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-11-18 03:45:06.881726 toyhouse-0.2.0/
--rw-rw-rw-   0        0        0    35802 2023-10-22 07:09:23.000000 toyhouse-0.2.0/LICENSE
--rw-rw-rw-   0        0        0     7319 2023-11-18 03:45:06.879777 toyhouse-0.2.0/PKG-INFO
--rw-rw-rw-   0        0        0     6694 2023-11-18 03:28:27.000000 toyhouse-0.2.0/README.md
--rw-rw-rw-   0        0        0      754 2023-11-18 03:10:20.000000 toyhouse-0.2.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-11-18 03:45:06.882330 toyhouse-0.2.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-11-18 03:45:06.818893 toyhouse-0.2.0/src/
-drwxrwxrwx   0        0        0        0 2023-11-18 03:45:06.844823 toyhouse-0.2.0/src/toyhouse/
--rw-rw-rw-   0        0        0      129 2023-11-02 23:55:46.000000 toyhouse-0.2.0/src/toyhouse/__init__.py
--rw-rw-rw-   0        0        0     3944 2023-11-15 00:53:43.000000 toyhouse-0.2.0/src/toyhouse/character.py
--rw-rw-rw-   0        0        0     1988 2023-11-18 02:56:46.000000 toyhouse-0.2.0/src/toyhouse/session.py
-drwxrwxrwx   0        0        0        0 2023-11-18 03:45:06.875740 toyhouse-0.2.0/src/toyhouse/tests/
--rw-rw-rw-   0        0        0      495 2023-11-18 03:18:14.000000 toyhouse-0.2.0/src/toyhouse/tests/import.py
--rw-rw-rw-   0        0        0        0 2023-11-03 00:09:54.000000 toyhouse-0.2.0/src/toyhouse/tests/local.py
--rw-rw-rw-   0        0        0     6803 2023-11-18 03:26:44.000000 toyhouse-0.2.0/src/toyhouse/user.py
--rw-rw-rw-   0        0        0     3905 2023-11-18 03:03:30.000000 toyhouse-0.2.0/src/toyhouse/utilities.py
-drwxrwxrwx   0        0        0        0 2023-11-18 03:45:06.872656 toyhouse-0.2.0/src/toyhouse.egg-info/
--rw-rw-rw-   0        0        0     7319 2023-11-18 03:45:06.000000 toyhouse-0.2.0/src/toyhouse.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      355 2023-11-18 03:45:06.000000 toyhouse-0.2.0/src/toyhouse.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-11-18 03:45:06.000000 toyhouse-0.2.0/src/toyhouse.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-11-18 03:45:06.000000 toyhouse-0.2.0/src/toyhouse.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 03:19:17.210546 toyhouse-0.2.1/
+-rw-rw-rw-   0        0        0    35802 2023-10-22 07:09:23.000000 toyhouse-0.2.1/LICENSE
+-rw-rw-rw-   0        0        0     8065 2024-05-19 03:19:17.208547 toyhouse-0.2.1/PKG-INFO
+-rw-rw-rw-   0        0        0     7368 2024-05-06 08:50:42.000000 toyhouse-0.2.1/README.md
+-rw-rw-rw-   0        0        0      773 2024-05-19 03:19:08.000000 toyhouse-0.2.1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 03:19:17.210546 toyhouse-0.2.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-19 03:19:17.134320 toyhouse-0.2.1/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 03:19:17.168956 toyhouse-0.2.1/src/toyhouse/
+-rw-rw-rw-   0        0        0      157 2023-12-11 07:48:37.000000 toyhouse-0.2.1/src/toyhouse/__init__.py
+-rw-rw-rw-   0        0        0     3944 2023-11-15 00:53:43.000000 toyhouse-0.2.1/src/toyhouse/character.py
+-rw-rw-rw-   0        0        0     1600 2024-05-06 08:37:22.000000 toyhouse-0.2.1/src/toyhouse/forum.py
+-rw-rw-rw-   0        0        0     1988 2023-11-18 02:56:46.000000 toyhouse-0.2.1/src/toyhouse/session.py
+drwxrwxrwx   0        0        0        0 2024-05-19 03:19:17.203587 toyhouse-0.2.1/src/toyhouse/tests/
+-rw-rw-rw-   0        0        0      804 2024-03-17 06:29:30.000000 toyhouse-0.2.1/src/toyhouse/tests/import.py
+-rw-rw-rw-   0        0        0      165 2024-05-06 08:17:11.000000 toyhouse-0.2.1/src/toyhouse/tests/local.py
+-rw-rw-rw-   0        0        0     6803 2023-11-18 03:26:44.000000 toyhouse-0.2.1/src/toyhouse/user.py
+-rw-rw-rw-   0        0        0     3895 2023-12-27 09:30:02.000000 toyhouse-0.2.1/src/toyhouse/utilities.py
+drwxrwxrwx   0        0        0        0 2024-05-19 03:19:17.206684 toyhouse-0.2.1/src/toyhouse.egg-info/
+-rw-rw-rw-   0        0        0     8065 2024-05-19 03:19:17.000000 toyhouse-0.2.1/src/toyhouse.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      412 2024-05-19 03:19:17.000000 toyhouse-0.2.1/src/toyhouse.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 03:19:17.000000 toyhouse-0.2.1/src/toyhouse.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       40 2024-05-19 03:19:17.000000 toyhouse-0.2.1/src/toyhouse.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2024-05-19 03:19:17.000000 toyhouse-0.2.1/src/toyhouse.egg-info/top_level.txt
```

### Comparing `toyhouse-0.2.0/LICENSE` & `toyhouse-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `toyhouse-0.2.0/PKG-INFO` & `toyhouse-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: toyhouse
-Version: 0.2.0
+Version: 0.2.1
 Summary: An unofficial Python API for the site Toyhou.se
 Author-email: Annabel Quach <annabelquach13@gmail.com>
 Project-URL: Homepage, https://github.com/phthallo/toyhouse-data
 Project-URL: Bug Tracker, https://github.com/phthallo/toyhouse-data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: beautifulsoup4>=4.12.2
+Requires-Dist: requests>=2.31.0
 
 # Toyhouse Data
-[work in progress] A Toyhouse service to retrieve data about your (and other people's) OCs, as well as your (and other people's) profiles. 
+[work in progress] An API wrapper for the site Toyhou.se to retrieve data about user profiles, character profiles, forum posts and more.
 
 This is very much a niche project (lol) but I'm hoping it'll serve some use to anyone curious!
 
 ## Prerequisites
 - [Python3](https://www.python.org/downloads/)
 - [Requests](https://pypi.org/project/requests/)
 - [BeautifulSoup4](https://pypi.org/project/beautifulsoup4/)
 
 ## Installation
 You can now use [pip](https://pip.pypa.io/en/stable/) to install this project! Simply run:
 
 ```
-pip install toyhouse
+py -m pip install toyhouse
 ```
 
 This project can be found [here](https://pypi.org/project/toyhouse/), albeit slightly out of date.
 
 > [!IMPORTANT]
 > I cannot guarantee that this service works on profiles with extreme custom CSS, legacy layouts or profile warnings! If you want to use this, please manually visit `https://toyhou.se/~account/display` and turn off all three settings under 'Profile Browsing'. In the meantime, I will be attempting to fix that.
 
@@ -48,28 +50,30 @@
 import toyhouse
 session = toyhouse.Session("<username>", "<password>", "file_path")
 session.auth()
 # alternatively
 session = toyhouse.GuestSession("<file_path>")
 ```
 
+## Examples
+If you don't care about the docs and just want to know how you can use this, see the [Snippets page](/snippets.md).
 
 ## Functions
 ### Session
 ```python
 session = toyhouse.Session("<username>", "<password>")
 session.auth()
 ```
 Starts a new logged-in Session using the credentials above, letting you access information on the Toyhouse website. 
 
 
 ```python
 session = toyhouse.GuestSession()
 ```
-Starts a new Guest Session. No authentication is required.
+Starts a new Guest Session. No authentication is required, but you will be limited to only publicly viewable data. 
 
 ---
 
 ### User
 ```python
 user_info = toyhouse.User(session, "<username>")
 ```
@@ -112,15 +116,15 @@
 ```
 Retrieves the specified user's **profile picture**, and if `download=True`, **downloads the image** at the file path mentioned under [Usage](#usage). If `download=False`, it returns the URL at which you can access the profile picture.
 
 #### designs
 ```python
 user_info.designs
 ```
-Outputs a **list of tuples** in format `(<char_name>, <char_id>, <char_url>, <char_loc>)` for all characters that the user is credited as a designer of. This format is the same as [chars()](#chars) except with `<char_loc` returning the URL + page number that the character is on.
+Outputs a **list of tuples** in format `(<char_name>, <char_id>, <char_url>, <char_loc>)` for all characters that the user is credited as a designer of. This format is the same as [chars()](#chars) except with `<char_loc>` returning the URL + page number that the character is on.
 
 
 #### favs
 ```python
 user_info.favs
 ```
 Outputs a **list of tuples** in format `(<char_name>, <char_id>, <char_url>, <char_loc>)` for all **characters that the user has favourited**. 
@@ -155,14 +159,30 @@
 char_info.favs
 # Returns 
 ['i_favourited_this_character', 'i_did_too', 'i_did_as_well']
 ```
 Outputs a **list** of all accounts that have the **character favourited**.
 
 ---
+
+### Forum
+
+```python
+forum_info = toyhouse.Forum(session, forumboardid)
+```
+Creates a new Forum object, letting you retrieve information about Forum boards and their posts. 
+
+#### threads
+```python
+forum_info.threads
+```
+
+Outputs a **list of tuples** in format `[(thread_title, thread_author, thread_creation_date)]` for the threads on the first page of a specific forum board. There is currently no distinguishing between pinned threads and standard threads. 
+
+---
 ## To-Do List
 
 - [ ] Retrieve character stats (~~favourites/favourite amount~~ - comments/comment amount - ~~ownership log~~)
 
 - [X] Add Guest Session
 
 - [ ] Find a profile which has multiple designers listed
```

### Comparing `toyhouse-0.2.0/README.md` & `toyhouse-0.2.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 # Toyhouse Data
-[work in progress] A Toyhouse service to retrieve data about your (and other people's) OCs, as well as your (and other people's) profiles. 
+[work in progress] An API wrapper for the site Toyhou.se to retrieve data about user profiles, character profiles, forum posts and more.
 
 This is very much a niche project (lol) but I'm hoping it'll serve some use to anyone curious!
 
 ## Prerequisites
 - [Python3](https://www.python.org/downloads/)
 - [Requests](https://pypi.org/project/requests/)
 - [BeautifulSoup4](https://pypi.org/project/beautifulsoup4/)
 
 ## Installation
 You can now use [pip](https://pip.pypa.io/en/stable/) to install this project! Simply run:
 
 ```
-pip install toyhouse
+py -m pip install toyhouse
 ```
 
 This project can be found [here](https://pypi.org/project/toyhouse/), albeit slightly out of date.
 
 > [!IMPORTANT]
 > I cannot guarantee that this service works on profiles with extreme custom CSS, legacy layouts or profile warnings! If you want to use this, please manually visit `https://toyhou.se/~account/display` and turn off all three settings under 'Profile Browsing'. In the meantime, I will be attempting to fix that.
 
@@ -33,28 +33,30 @@
 import toyhouse
 session = toyhouse.Session("<username>", "<password>", "file_path")
 session.auth()
 # alternatively
 session = toyhouse.GuestSession("<file_path>")
 ```
 
+## Examples
+If you don't care about the docs and just want to know how you can use this, see the [Snippets page](/snippets.md).
 
 ## Functions
 ### Session
 ```python
 session = toyhouse.Session("<username>", "<password>")
 session.auth()
 ```
 Starts a new logged-in Session using the credentials above, letting you access information on the Toyhouse website. 
 
 
 ```python
 session = toyhouse.GuestSession()
 ```
-Starts a new Guest Session. No authentication is required.
+Starts a new Guest Session. No authentication is required, but you will be limited to only publicly viewable data. 
 
 ---
 
 ### User
 ```python
 user_info = toyhouse.User(session, "<username>")
 ```
@@ -97,15 +99,15 @@
 ```
 Retrieves the specified user's **profile picture**, and if `download=True`, **downloads the image** at the file path mentioned under [Usage](#usage). If `download=False`, it returns the URL at which you can access the profile picture.
 
 #### designs
 ```python
 user_info.designs
 ```
-Outputs a **list of tuples** in format `(<char_name>, <char_id>, <char_url>, <char_loc>)` for all characters that the user is credited as a designer of. This format is the same as [chars()](#chars) except with `<char_loc` returning the URL + page number that the character is on.
+Outputs a **list of tuples** in format `(<char_name>, <char_id>, <char_url>, <char_loc>)` for all characters that the user is credited as a designer of. This format is the same as [chars()](#chars) except with `<char_loc>` returning the URL + page number that the character is on.
 
 
 #### favs
 ```python
 user_info.favs
 ```
 Outputs a **list of tuples** in format `(<char_name>, <char_id>, <char_url>, <char_loc>)` for all **characters that the user has favourited**. 
@@ -140,14 +142,30 @@
 char_info.favs
 # Returns 
 ['i_favourited_this_character', 'i_did_too', 'i_did_as_well']
 ```
 Outputs a **list** of all accounts that have the **character favourited**.
 
 ---
+
+### Forum
+
+```python
+forum_info = toyhouse.Forum(session, forumboardid)
+```
+Creates a new Forum object, letting you retrieve information about Forum boards and their posts. 
+
+#### threads
+```python
+forum_info.threads
+```
+
+Outputs a **list of tuples** in format `[(thread_title, thread_author, thread_creation_date)]` for the threads on the first page of a specific forum board. There is currently no distinguishing between pinned threads and standard threads. 
+
+---
 ## To-Do List
 
 - [ ] Retrieve character stats (~~favourites/favourite amount~~ - comments/comment amount - ~~ownership log~~)
 
 - [X] Add Guest Session
 
 - [ ] Find a profile which has multiple designers listed
```

### Comparing `toyhouse-0.2.0/pyproject.toml` & `toyhouse-0.2.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 [build-system]
 requires = [
-"setuptools>=61.0", 
-"beautifulsoup4>=4.12.2",
-"requests>=2.31.0"
+"setuptools>=61.0"
 ]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "toyhouse"
-version = "0.2.0"
+version = "0.2.1"
+dependencies = [
+"beautifulsoup4>=4.12.2",
+"requests>=2.31.0"
+]
 authors = [
   { name="Annabel Quach", email="annabelquach13@gmail.com" },
 ]
 description = "An unofficial Python API for the site Toyhou.se"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `toyhouse-0.2.0/src/toyhouse/character.py` & `toyhouse-0.2.1/src/toyhouse/character.py`

 * *Files identical despite different names*

### Comparing `toyhouse-0.2.0/src/toyhouse/session.py` & `toyhouse-0.2.1/src/toyhouse/session.py`

 * *Files identical despite different names*

### Comparing `toyhouse-0.2.0/src/toyhouse/user.py` & `toyhouse-0.2.1/src/toyhouse/user.py`

 * *Files identical despite different names*

### Comparing `toyhouse-0.2.0/src/toyhouse/utilities.py` & `toyhouse-0.2.1/src/toyhouse/utilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     else: 
         retrieve_attributes = retrieve_lxml.find(tag, class_attr)
     return retrieve_attributes
 
 
 
 # Some illegal characters are present in the character's name (as in they are illegal in URLs). If they're kept in, it will break that link.
-def strip_illegal(phrase):
+def sanitise(phrase):
     for character in phrase: 
         if character in """\/:*?"<>|() """:
             phrase = phrase.replace(character,"-")
         elif character not in string.ascii_letters and character not in string.digits:
             phrase = phrase.replace(character, "")
     phrase = re.sub('\-\-+', '-', phrase)
     return phrase.lower()
@@ -40,15 +40,15 @@
         max_pages = 1
     for i in range(1, int(max_pages)+1):
         retrieve_characters = scrape(session, f"{url}?page={i}","a", {"class": "btn btn-sm btn-primary character-name-badge"})
         for character in retrieve_characters:
             output.append(
                 ((character.text).strip(), 
                     int((character.get('href')[1:]).split('.',1)[0]),
-                    f"https://toyhou.se/{int((character.get('href')[1:]).split('.',1)[0])}." + strip_illegal((character.text).strip()),
+                    f"https://toyhou.se/{int((character.get('href')[1:]).split('.',1)[0])}." + sanitise((character.text).strip()),
                     f"{url}?page={i}"
                     ))
     return output 
 
 def create_path(username, file_path):
     if username in file_path:
         return file_path
```

### Comparing `toyhouse-0.2.0/src/toyhouse.egg-info/PKG-INFO` & `toyhouse-0.2.1/src/toyhouse.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,37 +1,39 @@
 Metadata-Version: 2.1
 Name: toyhouse
-Version: 0.2.0
+Version: 0.2.1
 Summary: An unofficial Python API for the site Toyhou.se
 Author-email: Annabel Quach <annabelquach13@gmail.com>
 Project-URL: Homepage, https://github.com/phthallo/toyhouse-data
 Project-URL: Bug Tracker, https://github.com/phthallo/toyhouse-data/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Classifier: Development Status :: 2 - Pre-Alpha
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: beautifulsoup4>=4.12.2
+Requires-Dist: requests>=2.31.0
 
 # Toyhouse Data
-[work in progress] A Toyhouse service to retrieve data about your (and other people's) OCs, as well as your (and other people's) profiles. 
+[work in progress] An API wrapper for the site Toyhou.se to retrieve data about user profiles, character profiles, forum posts and more.
 
 This is very much a niche project (lol) but I'm hoping it'll serve some use to anyone curious!
 
 ## Prerequisites
 - [Python3](https://www.python.org/downloads/)
 - [Requests](https://pypi.org/project/requests/)
 - [BeautifulSoup4](https://pypi.org/project/beautifulsoup4/)
 
 ## Installation
 You can now use [pip](https://pip.pypa.io/en/stable/) to install this project! Simply run:
 
 ```
-pip install toyhouse
+py -m pip install toyhouse
 ```
 
 This project can be found [here](https://pypi.org/project/toyhouse/), albeit slightly out of date.
 
 > [!IMPORTANT]
 > I cannot guarantee that this service works on profiles with extreme custom CSS, legacy layouts or profile warnings! If you want to use this, please manually visit `https://toyhou.se/~account/display` and turn off all three settings under 'Profile Browsing'. In the meantime, I will be attempting to fix that.
 
@@ -48,28 +50,30 @@
 import toyhouse
 session = toyhouse.Session("<username>", "<password>", "file_path")
 session.auth()
 # alternatively
 session = toyhouse.GuestSession("<file_path>")
 ```
 
+## Examples
+If you don't care about the docs and just want to know how you can use this, see the [Snippets page](/snippets.md).
 
 ## Functions
 ### Session
 ```python
 session = toyhouse.Session("<username>", "<password>")
 session.auth()
 ```
 Starts a new logged-in Session using the credentials above, letting you access information on the Toyhouse website. 
 
 
 ```python
 session = toyhouse.GuestSession()
 ```
-Starts a new Guest Session. No authentication is required.
+Starts a new Guest Session. No authentication is required, but you will be limited to only publicly viewable data. 
 
 ---
 
 ### User
 ```python
 user_info = toyhouse.User(session, "<username>")
 ```
@@ -112,15 +116,15 @@
 ```
 Retrieves the specified user's **profile picture**, and if `download=True`, **downloads the image** at the file path mentioned under [Usage](#usage). If `download=False`, it returns the URL at which you can access the profile picture.
 
 #### designs
 ```python
 user_info.designs
 ```
-Outputs a **list of tuples** in format `(<char_name>, <char_id>, <char_url>, <char_loc>)` for all characters that the user is credited as a designer of. This format is the same as [chars()](#chars) except with `<char_loc` returning the URL + page number that the character is on.
+Outputs a **list of tuples** in format `(<char_name>, <char_id>, <char_url>, <char_loc>)` for all characters that the user is credited as a designer of. This format is the same as [chars()](#chars) except with `<char_loc>` returning the URL + page number that the character is on.
 
 
 #### favs
 ```python
 user_info.favs
 ```
 Outputs a **list of tuples** in format `(<char_name>, <char_id>, <char_url>, <char_loc>)` for all **characters that the user has favourited**. 
@@ -155,14 +159,30 @@
 char_info.favs
 # Returns 
 ['i_favourited_this_character', 'i_did_too', 'i_did_as_well']
 ```
 Outputs a **list** of all accounts that have the **character favourited**.
 
 ---
+
+### Forum
+
+```python
+forum_info = toyhouse.Forum(session, forumboardid)
+```
+Creates a new Forum object, letting you retrieve information about Forum boards and their posts. 
+
+#### threads
+```python
+forum_info.threads
+```
+
+Outputs a **list of tuples** in format `[(thread_title, thread_author, thread_creation_date)]` for the threads on the first page of a specific forum board. There is currently no distinguishing between pinned threads and standard threads. 
+
+---
 ## To-Do List
 
 - [ ] Retrieve character stats (~~favourites/favourite amount~~ - comments/comment amount - ~~ownership log~~)
 
 - [X] Add Guest Session
 
 - [ ] Find a profile which has multiple designers listed
```

