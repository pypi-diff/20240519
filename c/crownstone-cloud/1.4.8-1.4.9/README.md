# Comparing `tmp/crownstone-cloud-1.4.8.tar.gz` & `tmp/crownstone-cloud-1.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crownstone-cloud-1.4.8.tar", last modified: Mon Sep 20 15:17:16 2021, max compression
+gzip compressed data, was "dist/crownstone-cloud-1.4.9.tar", last modified: Wed Nov 10 07:43:16 2021, max compression
```

## Comparing `crownstone-cloud-1.4.8.tar` & `crownstone-cloud-1.4.9.tar`

### file list

```diff
@@ -1,42 +1,41 @@
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2021-09-20 15:17:16.647768 crownstone-cloud-1.4.8/
--rw-r--r--   0 alex       (501) staff       (20)     1080 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/LICENSE.md
--rw-r--r--   0 alex       (501) staff       (20)       24 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/MANIFEST.in
--rw-r--r--   0 alex       (501) staff       (20)    12514 2021-09-20 15:17:16.647312 crownstone-cloud-1.4.8/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)    12118 2021-09-20 15:13:49.000000 crownstone-cloud-1.4.8/README.md
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2021-09-20 15:17:16.637805 crownstone-cloud-1.4.8/crownstone_cloud/
--rw-r--r--   0 alex       (501) staff       (20)      224 2021-09-20 15:13:49.000000 crownstone-cloud-1.4.8/crownstone_cloud/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     4826 2021-09-20 15:13:49.000000 crownstone-cloud-1.4.8/crownstone_cloud/cloud.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2021-09-20 15:17:16.641818 crownstone-cloud-1.4.8/crownstone_cloud/cloud_models/
--rw-r--r--   0 alex       (501) staff       (20)       61 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/crownstone_cloud/cloud_models/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     7309 2021-09-20 15:13:49.000000 crownstone-cloud-1.4.8/crownstone_cloud/cloud_models/crownstones.py
--rw-r--r--   0 alex       (501) staff       (20)     3815 2021-09-20 15:13:49.000000 crownstone-cloud-1.4.8/crownstone_cloud/cloud_models/locations.py
--rw-r--r--   0 alex       (501) staff       (20)     4608 2021-09-20 15:13:49.000000 crownstone-cloud-1.4.8/crownstone_cloud/cloud_models/spheres.py
--rw-r--r--   0 alex       (501) staff       (20)     3746 2021-09-20 15:13:49.000000 crownstone-cloud-1.4.8/crownstone_cloud/cloud_models/users.py
--rw-r--r--   0 alex       (501) staff       (20)      347 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/crownstone_cloud/const.py
--rw-r--r--   0 alex       (501) staff       (20)     1318 2021-09-20 15:13:49.000000 crownstone-cloud-1.4.8/crownstone_cloud/exceptions.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2021-09-20 15:17:16.643480 crownstone-cloud-1.4.8/crownstone_cloud/helpers/
--rw-r--r--   0 alex       (501) staff       (20)       56 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/crownstone_cloud/helpers/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      844 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/crownstone_cloud/helpers/aiohttp_client.py
--rw-r--r--   0 alex       (501) staff       (20)      570 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/crownstone_cloud/helpers/conversion.py
--rw-r--r--   0 alex       (501) staff       (20)     5995 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/crownstone_cloud/helpers/requests.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2021-09-20 15:17:16.644276 crownstone-cloud-1.4.8/crownstone_cloud/util/
--rw-r--r--   0 alex       (501) staff       (20)       53 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/crownstone_cloud/util/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)      348 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/crownstone_cloud/util/runners.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2021-09-20 15:17:16.639785 crownstone-cloud-1.4.8/crownstone_cloud.egg-info/
--rw-r--r--   0 alex       (501) staff       (20)    12514 2021-09-20 15:17:16.000000 crownstone-cloud-1.4.8/crownstone_cloud.egg-info/PKG-INFO
--rw-r--r--   0 alex       (501) staff       (20)     1049 2021-09-20 15:17:16.000000 crownstone-cloud-1.4.8/crownstone_cloud.egg-info/SOURCES.txt
--rw-r--r--   0 alex       (501) staff       (20)        1 2021-09-20 15:17:16.000000 crownstone-cloud-1.4.8/crownstone_cloud.egg-info/dependency_links.txt
--rw-r--r--   0 alex       (501) staff       (20)       57 2021-09-20 15:17:16.000000 crownstone-cloud-1.4.8/crownstone_cloud.egg-info/requires.txt
--rw-r--r--   0 alex       (501) staff       (20)       23 2021-09-20 15:17:16.000000 crownstone-cloud-1.4.8/crownstone_cloud.egg-info/top_level.txt
--rw-r--r--   0 alex       (501) staff       (20)       56 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/requirements.txt
--rw-r--r--   0 alex       (501) staff       (20)       38 2021-09-20 15:17:16.647890 crownstone-cloud-1.4.8/setup.cfg
--rw-r--r--   0 alex       (501) staff       (20)      698 2021-09-20 15:13:49.000000 crownstone-cloud-1.4.8/setup.py
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2021-09-20 15:17:16.635038 crownstone-cloud-1.4.8/tests/
-drwxr-xr-x   0 alex       (501) staff       (20)        0 2021-09-20 15:17:16.646732 crownstone-cloud-1.4.8/tests/mocked_replies/
--rw-r--r--   0 alex       (501) staff       (20)        0 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/tests/mocked_replies/__init__.py
--rw-r--r--   0 alex       (501) staff       (20)     5207 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/tests/mocked_replies/crownstone_data.py
--rw-r--r--   0 alex       (501) staff       (20)      573 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/tests/mocked_replies/errors.py
--rw-r--r--   0 alex       (501) staff       (20)     1785 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/tests/mocked_replies/location_data.py
--rw-r--r--   0 alex       (501) staff       (20)      141 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/tests/mocked_replies/login_data.py
--rw-r--r--   0 alex       (501) staff       (20)     2514 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/tests/mocked_replies/sphere_data.py
--rw-r--r--   0 alex       (501) staff       (20)     1375 2021-08-18 08:31:46.000000 crownstone-cloud-1.4.8/tests/mocked_replies/user_data.py
+drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2021-11-10 07:43:16.000000 crownstone-cloud-1.4.9/
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)    12118 2021-10-25 08:43:07.000000 crownstone-cloud-1.4.9/README.md
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)       20 2021-11-10 07:38:28.000000 crownstone-cloud-1.4.9/requirements.txt
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)    15468 2021-11-10 07:43:16.000000 crownstone-cloud-1.4.9/PKG-INFO
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)       38 2021-11-10 07:43:16.000000 crownstone-cloud-1.4.9/setup.cfg
+drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2021-11-10 07:43:16.000000 crownstone-cloud-1.4.9/crownstone_cloud.egg-info/
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)       23 2021-11-10 07:43:15.000000 crownstone-cloud-1.4.9/crownstone_cloud.egg-info/top_level.txt
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)    15468 2021-11-10 07:43:15.000000 crownstone-cloud-1.4.9/crownstone_cloud.egg-info/PKG-INFO
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     1038 2021-11-10 07:43:15.000000 crownstone-cloud-1.4.9/crownstone_cloud.egg-info/SOURCES.txt
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)       21 2021-11-10 07:43:15.000000 crownstone-cloud-1.4.9/crownstone_cloud.egg-info/requires.txt
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)        1 2021-11-10 07:43:15.000000 crownstone-cloud-1.4.9/crownstone_cloud.egg-info/dependency_links.txt
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)      698 2021-11-10 07:43:05.000000 crownstone-cloud-1.4.9/setup.py
+drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2021-11-10 07:43:16.000000 crownstone-cloud-1.4.9/tests/
+drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2021-11-10 07:43:16.000000 crownstone-cloud-1.4.9/tests/mocked_replies/
+-rw-r--r--   0 vliedel   (1000) vliedel   (1000)      573 2020-10-15 10:59:14.000000 crownstone-cloud-1.4.9/tests/mocked_replies/errors.py
+-rw-r--r--   0 vliedel   (1000) vliedel   (1000)      141 2020-10-15 10:59:14.000000 crownstone-cloud-1.4.9/tests/mocked_replies/login_data.py
+-rw-r--r--   0 vliedel   (1000) vliedel   (1000)     1375 2020-10-15 10:59:14.000000 crownstone-cloud-1.4.9/tests/mocked_replies/user_data.py
+-rw-r--r--   0 vliedel   (1000) vliedel   (1000)        0 2020-10-15 10:59:14.000000 crownstone-cloud-1.4.9/tests/mocked_replies/__init__.py
+-rw-r--r--   0 vliedel   (1000) vliedel   (1000)     1785 2020-10-15 10:59:14.000000 crownstone-cloud-1.4.9/tests/mocked_replies/location_data.py
+-rw-r--r--   0 vliedel   (1000) vliedel   (1000)     5207 2020-11-02 13:45:14.000000 crownstone-cloud-1.4.9/tests/mocked_replies/crownstone_data.py
+-rw-r--r--   0 vliedel   (1000) vliedel   (1000)     2514 2020-10-15 10:59:14.000000 crownstone-cloud-1.4.9/tests/mocked_replies/sphere_data.py
+-rw-r--r--   0 vliedel   (1000) vliedel   (1000)       24 2020-10-15 10:59:14.000000 crownstone-cloud-1.4.9/MANIFEST.in
+drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2021-11-10 07:43:16.000000 crownstone-cloud-1.4.9/crownstone_cloud/
+drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2021-11-10 07:43:16.000000 crownstone-cloud-1.4.9/crownstone_cloud/helpers/
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)      844 2021-08-10 09:22:33.000000 crownstone-cloud-1.4.9/crownstone_cloud/helpers/aiohttp_client.py
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)      570 2021-10-25 08:43:07.000000 crownstone-cloud-1.4.9/crownstone_cloud/helpers/conversion.py
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     5995 2021-10-25 08:43:07.000000 crownstone-cloud-1.4.9/crownstone_cloud/helpers/requests.py
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)       56 2021-08-10 09:22:33.000000 crownstone-cloud-1.4.9/crownstone_cloud/helpers/__init__.py
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     4826 2021-10-25 08:43:07.000000 crownstone-cloud-1.4.9/crownstone_cloud/cloud.py
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)      347 2021-08-10 09:22:33.000000 crownstone-cloud-1.4.9/crownstone_cloud/const.py
+drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2021-11-10 07:43:16.000000 crownstone-cloud-1.4.9/crownstone_cloud/cloud_models/
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     4608 2021-10-25 08:43:07.000000 crownstone-cloud-1.4.9/crownstone_cloud/cloud_models/spheres.py
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     3746 2021-10-25 08:43:07.000000 crownstone-cloud-1.4.9/crownstone_cloud/cloud_models/users.py
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)       61 2021-08-10 09:22:33.000000 crownstone-cloud-1.4.9/crownstone_cloud/cloud_models/__init__.py
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     7309 2021-10-25 08:43:07.000000 crownstone-cloud-1.4.9/crownstone_cloud/cloud_models/crownstones.py
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     3815 2021-10-25 08:43:07.000000 crownstone-cloud-1.4.9/crownstone_cloud/cloud_models/locations.py
+drwxrwxr-x   0 vliedel   (1000) vliedel   (1000)        0 2021-11-10 07:43:16.000000 crownstone-cloud-1.4.9/crownstone_cloud/util/
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)      348 2021-08-10 09:22:33.000000 crownstone-cloud-1.4.9/crownstone_cloud/util/runners.py
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)       53 2021-08-10 09:22:33.000000 crownstone-cloud-1.4.9/crownstone_cloud/util/__init__.py
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)     1318 2021-10-25 08:43:07.000000 crownstone-cloud-1.4.9/crownstone_cloud/exceptions.py
+-rw-rw-r--   0 vliedel   (1000) vliedel   (1000)      224 2021-11-10 07:43:05.000000 crownstone-cloud-1.4.9/crownstone_cloud/__init__.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `crownstone-cloud-1.4.8/PKG-INFO` & `crownstone-cloud-1.4.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: crownstone-cloud
-Version: 1.4.8
-Summary: UNKNOWN
-Home-page: https://github.com/crownstone/crownstone-lib-python-cloud
-Author: Crownstone B.V.
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 # crownstone-lib-python-cloud
 
 Asynchronous Python library to get data from the cloud, and switch Crownstones.
 
 ## Functionality
 
 * Async: using asyncio and aiohttp, optimized for speed.
@@ -379,9 +365,7 @@
 $ coverage html
 ```
 To view your html file directly on Linux:
 ```console
 $ ./htmlcov/index.html
 ```
 On Windows simply navigate to the htmlcov folder inside the project folder, and double-click index.html. It will be executed in your selected browser.
-
-
```

### Comparing `crownstone-cloud-1.4.8/README.md` & `crownstone-cloud-1.4.9/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,371 +1,384 @@
-# crownstone-lib-python-cloud
-
-Asynchronous Python library to get data from the cloud, and switch Crownstones.
-
-## Functionality
-
-* Async: using asyncio and aiohttp, optimized for speed.
-* Easy to use: sync all your Crownstone Cloud data with just one command!
-* Structurally sound: find your data with ease!
-* Complete: set the switch state and brightness of your Crownstones remotely!
-* Flexible: Login and get the data for multiple accounts at once!
-
-## Requirements
-
-* Python 3.8 or higher
-* Aiohttp 3.7.4
-
-## Standard installation
-
-cd to the project folder and run:
-```console
-$ python setup.py install
-```
-
-## Install in a virtual environment
-
-To install the library execute the following command:
-```console
-$ python -m venv venv
-```
-Activate your venv using:
-```console
-$ source venv/bin/activate
-```
-Once activated, the venv is used to executed python files, and libraries will be installed in the venv.<br>
-To install this library, cd to the project folder and run:
-```console
-$ python setup.py install
-```
-
-## Getting started
-
-### Examples
-
-#### Async example
-
-```python
-from crownstone_cloud import CrownstoneCloud, create_clientsession
-import logging
-import asyncio
-
-# Enable logging.
-logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.DEBUG)
-
-
-async def main():
-    # Every instance creates it's own websession for easy accessibility, however using 1 websession is recommended.
-    # Create your websession like so:
-    websession = create_clientsession()
-    # Initialize cloud.
-    cloud_user_1 = CrownstoneCloud('email_user_1', 'password_user_1', websession)
-    # Login to the Crownstone Cloud and synchronize all cloud data.
-    await cloud_user_1.async_initialize()
-
-    # Get a crownstone by name that can dim, and put it on 20% brightness for user 1
-    crownstone_lamp = cloud_user_1.get_crownstone('Lamp')
-    await crownstone_lamp.async_set_brightness(20)
-
-    # Login & synchronize data for an other account.
-    cloud_user_2 = CrownstoneCloud('email_user_2', 'password_user_2', websession)
-    await cloud_user_2.async_initialize()
-
-    # Get a crownstone by name and turn it on for user 2.
-    crownstone_tv = cloud_user_2.get_crownstone('TV')
-    await crownstone_tv.async_turn_on()
-
-    # If you want to update specific data you can get the cloud data object for your user.
-    # This object has all the cloud data for your user saved in it, which was synced with async_initialize()
-    # Parts of the data can also be synced individually without touching the other data.
-    # To sync all data at once, use async_synchronize() instead.
-    my_sphere = cloud_user_1.cloud_data.find("my_sphere_name")
-    # request to sync only the locations with the cloud
-    await my_sphere.locations.async_update_location_data()
-    # get the keys for this sphere so you can use them with the Crownstone BLE python library
-    sphere_keys = await my_sphere.async_get_keys()
-
-    # Close the aiohttp clientsession after we are done.
-    await websession.close()
-
-asyncio.run(main())
-```
-
-#### Sync example
-
-```python
-from crownstone_cloud import CrownstoneCloud, run_async
-import logging
-
-# Enable logging.
-logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.DEBUG)
-
-# Initialize cloud.
-cloud = CrownstoneCloud('email', 'password')
-# Use 'run_async' to run async functions in sync context.
-# Login & synchronize all cloud data.
-run_async(cloud.async_initialize())
-
-# Get a crownstone by name and turn it on.
-crownstone_coffee_machine = cloud.get_crownstone('Coffee machine')
-run_async(crownstone_coffee_machine.async_turn_on())
-
-# Close the session after we are done.
-run_async(cloud.async_close_session())
-```
-
-### Initialization
-
-The Crownstone cloud is initialized with the email and password of a user:
-```python
-cloud = CrownstoneCloud('email', 'password')
-```
-If you do not yet have a Crownstone account, go to [My Crownstone](https://my.crownstone.rocks) to set one up.
-The email and password are used to re-login after an access token has expired.
-
-You can log into multiple accounts by creating more CrownstoneCloud objects. When doing so, it is recommended to use
-only 1 websession for all your requests. Create a websession and append it as parameter to all your CrownstoneCloud
-objects. Take a look at the async example above.
-```python
-cloud = CrownstoneCloud('email', 'password', websession)
-```
-To log in and get all your Crownstone from the cloud:
-```python
-await cloud.async_initialize()
-```
-
-## Data structure
-
-The cloud can be displayed with the following structure:
-* User
-    * Keys
-    * Spheres
-        * Locations
-        * Crownstones
-        * Users
-        
-
-### User
-
-The user is the to whom the data belongs.<br> 
-The user is the one that logs in using email and password.<br>
-By getting a user specific access token after login, the data for that specific user can be requested.
-
-### Keys
-
-The keys are user specific.<br> 
-They are required to connect to the crownstone bluetooth mesh.<br>
-The most common used keys are the sphere keys. They are located within each individual sphere.<br>
-
-### Spheres
-
-Spheres are the main data entry. They have rooms (locations), Crownstones and users in them.<br>
-Example spheres:
-* House
-* Office
-* Apartment
-
-A Sphere has the following fields in the cloud lib:
-* crownstones: Crownstones
-* locations: Locations
-* users: Users
-* keys: Dict (optional, default = None)
-* name: String
-* cloud_id: String
-* unique_id: String
-* present_people: List
-
-### Locations
-
-Locations are the rooms in your house or other building.<br>
-For example for a house: 
-* Living room
-* Bedroom
-* Garage
-* Bathroom
-
-A Location has the following fields in the cloud lib:
-* present_people: List
-* name: String
-* cloud_id: String
-* unique_id: String
-
-### Crownstones
-
-Crownstones are smart plugs that can make every device that isn't smart, way smarter!<br>
-Crownstones are located within a sphere.<br>
-Example names of Crownstones:
-* Lamp
-* Charger
-* Television
-
-A Crownstone has the following fields in the cloud lib:
-* abilities: Dict
-* state: Int (0..100)
-* name: String
-* unique_id: String
-* cloud_id: String
-* type: String
-* sw_version: String
-
-### Users
-
-Users are people who have access to a sphere.<br>
-A user can have 3 roles:
-* Admin
-* Member
-* Guest
-
-A User has the following fields in the cloud lib:
-* role: String
-* first_name: String
-* last_name: String
-* email: String
-* cloud_id: String
-* email_verified: Bool
-
-## Function list
-
-### Cloud
-
-#### async_initialize()
-> Login and sync all data for the user from the cloud.
-
-#### async_synchronize()
-> Synchronize all data for a user. Use case is to update the local data with new data from the cloud.
-> This function is already called in `async_initialize()`.
-
-#### get_crownstone(crownstone_name: String, sphere_id: String = None) -> Crownstone
-> Get a Crownstone object by name for a user. Raises CrownstoneNotFoundError if it doesn't exist.
-> You can optionally provide a sphere id to match where the Crownstone should be found.
-
-#### get_crownstone_by_id(crownstone_id: String, sphere_id: String = None) -> Crownstone
-> Get a Crownstone object by it's id for a user. Raises CrownstoneNotFoundError if it doesn't exist.
-> You can optionally provide a sphere id to match where the Crownstone should be found.
-
-#### get_crownstone_by_uid(crownstone_uid: int, sphere_id: String = None) -> Crownstone
-> Get a Crownstone object by it's uid for a user. Raises CrownstoneNotFoundError if it doesn't exist.
-> You can optionally provide a sphere id to match where the Crownstone should be found.
-
-#### async_close_session()
-> Async function. This will close the websession in requestHandler to cleanup nicely after the program has finished.
-
-### Spheres
-
-#### async_update_sphere_data()
-> Async function. Sync the Spheres with the cloud. Calling the function again after init will update the current data.
-
-#### find(sphere_name: String) -> Sphere
-> Returns a sphere object if one exists by that name.
-
-#### find_by_id(sphere_id: String) -> Sphere
-> Return a sphere object if one exists by that id.
-
-### Sphere
-
-#### async_update_sphere_presence()
-> Async function. Sync the presence of users in the sphere with the cloud.
-
-#### async_get_keys() -> Dict
-> Async function. Returns a dict with the keys of this sphere. 
-> The keys can be used for BLE connectivity with the Crownstones.
-
-### Crownstones
-
-#### async_update_crownstone_data()
-> Async function. Sync the Crownstones with the cloud for a sphere. 
-> Calling the function again after init will update the current data.
-
-#### find(crownstone_name: String) -> Crownstone
-> Return a Crownstone object if one exists by that name.
-
-#### find_by_id(crownstone_id: String) -> Crownstone
-> Return a Crownstone object if one exists by that id.
-
-### Crownstone
-
-#### async_turn_on()
-> Async function. Send a command to turn a Crownstone on. 
-> To make this work make sure to be in the selected sphere and have Bluetooth enabled on your phone.
-
-#### async_turn_off()
-> Async function. Send a command to turn a Crownstone off. 
-> To make this work make sure to be in the selected sphere and have Bluetooth enabled on your phone.
-
-#### async_set_brightness(value: Integer)
-> Async function. Send a command to set a Crownstone to a given brightness level. 
-> To make this work make sure to be in the selected sphere and have Bluetooth enabled on your phone.
-> The value parameter should be between 0 and 100.
-
-### Locations
-
-#### async_update_location_data()
-> Async function. Sync the Locations with the cloud for a sphere. Calling the function again after init will update the current data.
-
-#### async_update_location_presence()
-> Async function. Sync the presence with the cloud. This will replace the current presence with the new presence.
-
-#### find(location_name: String) -> Location
-> Return a location object if one exists by that name.
-
-#### find_by_id(location_id: String) -> Location
-> Return a location object if one exists by that id.
-
-### Users
-
-#### async_update_user_data()
-> Async function. Sync the Users with the cloud for a sphere. Calling the function again after init will update the current data.
-
-#### find_by_first_name(first_name: String) -> List
-> Returns a list of all users with that first name, as duplicate first names can exist.
-
-#### find_by_last_name(last_name: String) -> List
-> Return a list of all users with that last name, as duplicate last names can exist.
-
-#### find_by_id(user_id: String) -> Location
-> Return a location object if one exists by that id.
-
-## Async vs sync
-The lib can be used synchronously and asynchronously.<br>
-The disadvantage of sync context is that all functions are blocking. 
-The program will simply wait until a function is complete. In async context, functions (coroutines) can yield control,
-which means that functions can be "paused" while they are waiting for external data to come in, like data from a server.
-Other functions can then be executed in the meantime. This way the program is always busy.<br>
-
-All async functions in the library API functions in this library have the prefix **async_**
-Async functions need to be awaited:
-```Python
-await cloud.async_close_session()
-```
-All the async functions mentioned above can also be used synchronously.<br>
-Use the `run_async()` function like so:
-```Python
-from crownstone_cloud import run_async
-
-run_async(cloud.async_close_session())
-```
-Make sure to see the examples above!
-
-## Testing
-
-To run the tests using tox install tox first by running:
-```console
-$ pip install tox
-```
-To execute the tests cd to the project folder and run:
-```console
-$ tox
-```
-To see which parts of the code are covered by the tests, a coverage report is generated after the tests have been successful.<br>
-To see the coverage report run:
-```console
-$ coverage report
-```
-If you like to get a better overview of the test you can generate a HTML file like so:
-```console
-$ coverage html
-```
-To view your html file directly on Linux:
-```console
-$ ./htmlcov/index.html
-```
-On Windows simply navigate to the htmlcov folder inside the project folder, and double-click index.html. It will be executed in your selected browser.
+Metadata-Version: 2.1
+Name: crownstone-cloud
+Version: 1.4.9
+Summary: UNKNOWN
+Home-page: https://github.com/crownstone/crownstone-lib-python-cloud
+Author: Crownstone B.V.
+License: UNKNOWN
+Description: # crownstone-lib-python-cloud
+        
+        Asynchronous Python library to get data from the cloud, and switch Crownstones.
+        
+        ## Functionality
+        
+        * Async: using asyncio and aiohttp, optimized for speed.
+        * Easy to use: sync all your Crownstone Cloud data with just one command!
+        * Structurally sound: find your data with ease!
+        * Complete: set the switch state and brightness of your Crownstones remotely!
+        * Flexible: Login and get the data for multiple accounts at once!
+        
+        ## Requirements
+        
+        * Python 3.8 or higher
+        * Aiohttp 3.7.4
+        
+        ## Standard installation
+        
+        cd to the project folder and run:
+        ```console
+        $ python setup.py install
+        ```
+        
+        ## Install in a virtual environment
+        
+        To install the library execute the following command:
+        ```console
+        $ python -m venv venv
+        ```
+        Activate your venv using:
+        ```console
+        $ source venv/bin/activate
+        ```
+        Once activated, the venv is used to executed python files, and libraries will be installed in the venv.<br>
+        To install this library, cd to the project folder and run:
+        ```console
+        $ python setup.py install
+        ```
+        
+        ## Getting started
+        
+        ### Examples
+        
+        #### Async example
+        
+        ```python
+        from crownstone_cloud import CrownstoneCloud, create_clientsession
+        import logging
+        import asyncio
+        
+        # Enable logging.
+        logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.DEBUG)
+        
+        
+        async def main():
+            # Every instance creates it's own websession for easy accessibility, however using 1 websession is recommended.
+            # Create your websession like so:
+            websession = create_clientsession()
+            # Initialize cloud.
+            cloud_user_1 = CrownstoneCloud('email_user_1', 'password_user_1', websession)
+            # Login to the Crownstone Cloud and synchronize all cloud data.
+            await cloud_user_1.async_initialize()
+        
+            # Get a crownstone by name that can dim, and put it on 20% brightness for user 1
+            crownstone_lamp = cloud_user_1.get_crownstone('Lamp')
+            await crownstone_lamp.async_set_brightness(20)
+        
+            # Login & synchronize data for an other account.
+            cloud_user_2 = CrownstoneCloud('email_user_2', 'password_user_2', websession)
+            await cloud_user_2.async_initialize()
+        
+            # Get a crownstone by name and turn it on for user 2.
+            crownstone_tv = cloud_user_2.get_crownstone('TV')
+            await crownstone_tv.async_turn_on()
+        
+            # If you want to update specific data you can get the cloud data object for your user.
+            # This object has all the cloud data for your user saved in it, which was synced with async_initialize()
+            # Parts of the data can also be synced individually without touching the other data.
+            # To sync all data at once, use async_synchronize() instead.
+            my_sphere = cloud_user_1.cloud_data.find("my_sphere_name")
+            # request to sync only the locations with the cloud
+            await my_sphere.locations.async_update_location_data()
+            # get the keys for this sphere so you can use them with the Crownstone BLE python library
+            sphere_keys = await my_sphere.async_get_keys()
+        
+            # Close the aiohttp clientsession after we are done.
+            await websession.close()
+        
+        asyncio.run(main())
+        ```
+        
+        #### Sync example
+        
+        ```python
+        from crownstone_cloud import CrownstoneCloud, run_async
+        import logging
+        
+        # Enable logging.
+        logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.DEBUG)
+        
+        # Initialize cloud.
+        cloud = CrownstoneCloud('email', 'password')
+        # Use 'run_async' to run async functions in sync context.
+        # Login & synchronize all cloud data.
+        run_async(cloud.async_initialize())
+        
+        # Get a crownstone by name and turn it on.
+        crownstone_coffee_machine = cloud.get_crownstone('Coffee machine')
+        run_async(crownstone_coffee_machine.async_turn_on())
+        
+        # Close the session after we are done.
+        run_async(cloud.async_close_session())
+        ```
+        
+        ### Initialization
+        
+        The Crownstone cloud is initialized with the email and password of a user:
+        ```python
+        cloud = CrownstoneCloud('email', 'password')
+        ```
+        If you do not yet have a Crownstone account, go to [My Crownstone](https://my.crownstone.rocks) to set one up.
+        The email and password are used to re-login after an access token has expired.
+        
+        You can log into multiple accounts by creating more CrownstoneCloud objects. When doing so, it is recommended to use
+        only 1 websession for all your requests. Create a websession and append it as parameter to all your CrownstoneCloud
+        objects. Take a look at the async example above.
+        ```python
+        cloud = CrownstoneCloud('email', 'password', websession)
+        ```
+        To log in and get all your Crownstone from the cloud:
+        ```python
+        await cloud.async_initialize()
+        ```
+        
+        ## Data structure
+        
+        The cloud can be displayed with the following structure:
+        * User
+            * Keys
+            * Spheres
+                * Locations
+                * Crownstones
+                * Users
+                
+        
+        ### User
+        
+        The user is the to whom the data belongs.<br> 
+        The user is the one that logs in using email and password.<br>
+        By getting a user specific access token after login, the data for that specific user can be requested.
+        
+        ### Keys
+        
+        The keys are user specific.<br> 
+        They are required to connect to the crownstone bluetooth mesh.<br>
+        The most common used keys are the sphere keys. They are located within each individual sphere.<br>
+        
+        ### Spheres
+        
+        Spheres are the main data entry. They have rooms (locations), Crownstones and users in them.<br>
+        Example spheres:
+        * House
+        * Office
+        * Apartment
+        
+        A Sphere has the following fields in the cloud lib:
+        * crownstones: Crownstones
+        * locations: Locations
+        * users: Users
+        * keys: Dict (optional, default = None)
+        * name: String
+        * cloud_id: String
+        * unique_id: String
+        * present_people: List
+        
+        ### Locations
+        
+        Locations are the rooms in your house or other building.<br>
+        For example for a house: 
+        * Living room
+        * Bedroom
+        * Garage
+        * Bathroom
+        
+        A Location has the following fields in the cloud lib:
+        * present_people: List
+        * name: String
+        * cloud_id: String
+        * unique_id: String
+        
+        ### Crownstones
+        
+        Crownstones are smart plugs that can make every device that isn't smart, way smarter!<br>
+        Crownstones are located within a sphere.<br>
+        Example names of Crownstones:
+        * Lamp
+        * Charger
+        * Television
+        
+        A Crownstone has the following fields in the cloud lib:
+        * abilities: Dict
+        * state: Int (0..100)
+        * name: String
+        * unique_id: String
+        * cloud_id: String
+        * type: String
+        * sw_version: String
+        
+        ### Users
+        
+        Users are people who have access to a sphere.<br>
+        A user can have 3 roles:
+        * Admin
+        * Member
+        * Guest
+        
+        A User has the following fields in the cloud lib:
+        * role: String
+        * first_name: String
+        * last_name: String
+        * email: String
+        * cloud_id: String
+        * email_verified: Bool
+        
+        ## Function list
+        
+        ### Cloud
+        
+        #### async_initialize()
+        > Login and sync all data for the user from the cloud.
+        
+        #### async_synchronize()
+        > Synchronize all data for a user. Use case is to update the local data with new data from the cloud.
+        > This function is already called in `async_initialize()`.
+        
+        #### get_crownstone(crownstone_name: String, sphere_id: String = None) -> Crownstone
+        > Get a Crownstone object by name for a user. Raises CrownstoneNotFoundError if it doesn't exist.
+        > You can optionally provide a sphere id to match where the Crownstone should be found.
+        
+        #### get_crownstone_by_id(crownstone_id: String, sphere_id: String = None) -> Crownstone
+        > Get a Crownstone object by it's id for a user. Raises CrownstoneNotFoundError if it doesn't exist.
+        > You can optionally provide a sphere id to match where the Crownstone should be found.
+        
+        #### get_crownstone_by_uid(crownstone_uid: int, sphere_id: String = None) -> Crownstone
+        > Get a Crownstone object by it's uid for a user. Raises CrownstoneNotFoundError if it doesn't exist.
+        > You can optionally provide a sphere id to match where the Crownstone should be found.
+        
+        #### async_close_session()
+        > Async function. This will close the websession in requestHandler to cleanup nicely after the program has finished.
+        
+        ### Spheres
+        
+        #### async_update_sphere_data()
+        > Async function. Sync the Spheres with the cloud. Calling the function again after init will update the current data.
+        
+        #### find(sphere_name: String) -> Sphere
+        > Returns a sphere object if one exists by that name.
+        
+        #### find_by_id(sphere_id: String) -> Sphere
+        > Return a sphere object if one exists by that id.
+        
+        ### Sphere
+        
+        #### async_update_sphere_presence()
+        > Async function. Sync the presence of users in the sphere with the cloud.
+        
+        #### async_get_keys() -> Dict
+        > Async function. Returns a dict with the keys of this sphere. 
+        > The keys can be used for BLE connectivity with the Crownstones.
+        
+        ### Crownstones
+        
+        #### async_update_crownstone_data()
+        > Async function. Sync the Crownstones with the cloud for a sphere. 
+        > Calling the function again after init will update the current data.
+        
+        #### find(crownstone_name: String) -> Crownstone
+        > Return a Crownstone object if one exists by that name.
+        
+        #### find_by_id(crownstone_id: String) -> Crownstone
+        > Return a Crownstone object if one exists by that id.
+        
+        ### Crownstone
+        
+        #### async_turn_on()
+        > Async function. Send a command to turn a Crownstone on. 
+        > To make this work make sure to be in the selected sphere and have Bluetooth enabled on your phone.
+        
+        #### async_turn_off()
+        > Async function. Send a command to turn a Crownstone off. 
+        > To make this work make sure to be in the selected sphere and have Bluetooth enabled on your phone.
+        
+        #### async_set_brightness(value: Integer)
+        > Async function. Send a command to set a Crownstone to a given brightness level. 
+        > To make this work make sure to be in the selected sphere and have Bluetooth enabled on your phone.
+        > The value parameter should be between 0 and 100.
+        
+        ### Locations
+        
+        #### async_update_location_data()
+        > Async function. Sync the Locations with the cloud for a sphere. Calling the function again after init will update the current data.
+        
+        #### async_update_location_presence()
+        > Async function. Sync the presence with the cloud. This will replace the current presence with the new presence.
+        
+        #### find(location_name: String) -> Location
+        > Return a location object if one exists by that name.
+        
+        #### find_by_id(location_id: String) -> Location
+        > Return a location object if one exists by that id.
+        
+        ### Users
+        
+        #### async_update_user_data()
+        > Async function. Sync the Users with the cloud for a sphere. Calling the function again after init will update the current data.
+        
+        #### find_by_first_name(first_name: String) -> List
+        > Returns a list of all users with that first name, as duplicate first names can exist.
+        
+        #### find_by_last_name(last_name: String) -> List
+        > Return a list of all users with that last name, as duplicate last names can exist.
+        
+        #### find_by_id(user_id: String) -> Location
+        > Return a location object if one exists by that id.
+        
+        ## Async vs sync
+        The lib can be used synchronously and asynchronously.<br>
+        The disadvantage of sync context is that all functions are blocking. 
+        The program will simply wait until a function is complete. In async context, functions (coroutines) can yield control,
+        which means that functions can be "paused" while they are waiting for external data to come in, like data from a server.
+        Other functions can then be executed in the meantime. This way the program is always busy.<br>
+        
+        All async functions in the library API functions in this library have the prefix **async_**
+        Async functions need to be awaited:
+        ```Python
+        await cloud.async_close_session()
+        ```
+        All the async functions mentioned above can also be used synchronously.<br>
+        Use the `run_async()` function like so:
+        ```Python
+        from crownstone_cloud import run_async
+        
+        run_async(cloud.async_close_session())
+        ```
+        Make sure to see the examples above!
+        
+        ## Testing
+        
+        To run the tests using tox install tox first by running:
+        ```console
+        $ pip install tox
+        ```
+        To execute the tests cd to the project folder and run:
+        ```console
+        $ tox
+        ```
+        To see which parts of the code are covered by the tests, a coverage report is generated after the tests have been successful.<br>
+        To see the coverage report run:
+        ```console
+        $ coverage report
+        ```
+        If you like to get a better overview of the test you can generate a HTML file like so:
+        ```console
+        $ coverage html
+        ```
+        To view your html file directly on Linux:
+        ```console
+        $ ./htmlcov/index.html
+        ```
+        On Windows simply navigate to the htmlcov folder inside the project folder, and double-click index.html. It will be executed in your selected browser.
+        
+Platform: UNKNOWN
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
```

### Comparing `crownstone-cloud-1.4.8/crownstone_cloud/cloud.py` & `crownstone-cloud-1.4.9/crownstone_cloud/cloud.py`

 * *Files identical despite different names*

### Comparing `crownstone-cloud-1.4.8/crownstone_cloud/cloud_models/crownstones.py` & `crownstone-cloud-1.4.9/crownstone_cloud/cloud_models/crownstones.py`

 * *Files identical despite different names*

### Comparing `crownstone-cloud-1.4.8/crownstone_cloud/cloud_models/locations.py` & `crownstone-cloud-1.4.9/crownstone_cloud/cloud_models/locations.py`

 * *Files identical despite different names*

### Comparing `crownstone-cloud-1.4.8/crownstone_cloud/cloud_models/spheres.py` & `crownstone-cloud-1.4.9/crownstone_cloud/cloud_models/spheres.py`

 * *Files identical despite different names*

### Comparing `crownstone-cloud-1.4.8/crownstone_cloud/cloud_models/users.py` & `crownstone-cloud-1.4.9/crownstone_cloud/cloud_models/users.py`

 * *Files identical despite different names*

### Comparing `crownstone-cloud-1.4.8/crownstone_cloud/exceptions.py` & `crownstone-cloud-1.4.9/crownstone_cloud/exceptions.py`

 * *Files identical despite different names*

### Comparing `crownstone-cloud-1.4.8/crownstone_cloud/helpers/aiohttp_client.py` & `crownstone-cloud-1.4.9/crownstone_cloud/helpers/aiohttp_client.py`

 * *Files identical despite different names*

### Comparing `crownstone-cloud-1.4.8/crownstone_cloud/helpers/conversion.py` & `crownstone-cloud-1.4.9/crownstone_cloud/helpers/conversion.py`

 * *Files identical despite different names*

### Comparing `crownstone-cloud-1.4.8/crownstone_cloud/helpers/requests.py` & `crownstone-cloud-1.4.9/crownstone_cloud/helpers/requests.py`

 * *Files identical despite different names*

### Comparing `crownstone-cloud-1.4.8/crownstone_cloud.egg-info/PKG-INFO` & `crownstone-cloud-1.4.9/crownstone_cloud.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,387 +1,384 @@
 Metadata-Version: 2.1
 Name: crownstone-cloud
-Version: 1.4.8
+Version: 1.4.9
 Summary: UNKNOWN
 Home-page: https://github.com/crownstone/crownstone-lib-python-cloud
 Author: Crownstone B.V.
 License: UNKNOWN
+Description: # crownstone-lib-python-cloud
+        
+        Asynchronous Python library to get data from the cloud, and switch Crownstones.
+        
+        ## Functionality
+        
+        * Async: using asyncio and aiohttp, optimized for speed.
+        * Easy to use: sync all your Crownstone Cloud data with just one command!
+        * Structurally sound: find your data with ease!
+        * Complete: set the switch state and brightness of your Crownstones remotely!
+        * Flexible: Login and get the data for multiple accounts at once!
+        
+        ## Requirements
+        
+        * Python 3.8 or higher
+        * Aiohttp 3.7.4
+        
+        ## Standard installation
+        
+        cd to the project folder and run:
+        ```console
+        $ python setup.py install
+        ```
+        
+        ## Install in a virtual environment
+        
+        To install the library execute the following command:
+        ```console
+        $ python -m venv venv
+        ```
+        Activate your venv using:
+        ```console
+        $ source venv/bin/activate
+        ```
+        Once activated, the venv is used to executed python files, and libraries will be installed in the venv.<br>
+        To install this library, cd to the project folder and run:
+        ```console
+        $ python setup.py install
+        ```
+        
+        ## Getting started
+        
+        ### Examples
+        
+        #### Async example
+        
+        ```python
+        from crownstone_cloud import CrownstoneCloud, create_clientsession
+        import logging
+        import asyncio
+        
+        # Enable logging.
+        logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.DEBUG)
+        
+        
+        async def main():
+            # Every instance creates it's own websession for easy accessibility, however using 1 websession is recommended.
+            # Create your websession like so:
+            websession = create_clientsession()
+            # Initialize cloud.
+            cloud_user_1 = CrownstoneCloud('email_user_1', 'password_user_1', websession)
+            # Login to the Crownstone Cloud and synchronize all cloud data.
+            await cloud_user_1.async_initialize()
+        
+            # Get a crownstone by name that can dim, and put it on 20% brightness for user 1
+            crownstone_lamp = cloud_user_1.get_crownstone('Lamp')
+            await crownstone_lamp.async_set_brightness(20)
+        
+            # Login & synchronize data for an other account.
+            cloud_user_2 = CrownstoneCloud('email_user_2', 'password_user_2', websession)
+            await cloud_user_2.async_initialize()
+        
+            # Get a crownstone by name and turn it on for user 2.
+            crownstone_tv = cloud_user_2.get_crownstone('TV')
+            await crownstone_tv.async_turn_on()
+        
+            # If you want to update specific data you can get the cloud data object for your user.
+            # This object has all the cloud data for your user saved in it, which was synced with async_initialize()
+            # Parts of the data can also be synced individually without touching the other data.
+            # To sync all data at once, use async_synchronize() instead.
+            my_sphere = cloud_user_1.cloud_data.find("my_sphere_name")
+            # request to sync only the locations with the cloud
+            await my_sphere.locations.async_update_location_data()
+            # get the keys for this sphere so you can use them with the Crownstone BLE python library
+            sphere_keys = await my_sphere.async_get_keys()
+        
+            # Close the aiohttp clientsession after we are done.
+            await websession.close()
+        
+        asyncio.run(main())
+        ```
+        
+        #### Sync example
+        
+        ```python
+        from crownstone_cloud import CrownstoneCloud, run_async
+        import logging
+        
+        # Enable logging.
+        logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.DEBUG)
+        
+        # Initialize cloud.
+        cloud = CrownstoneCloud('email', 'password')
+        # Use 'run_async' to run async functions in sync context.
+        # Login & synchronize all cloud data.
+        run_async(cloud.async_initialize())
+        
+        # Get a crownstone by name and turn it on.
+        crownstone_coffee_machine = cloud.get_crownstone('Coffee machine')
+        run_async(crownstone_coffee_machine.async_turn_on())
+        
+        # Close the session after we are done.
+        run_async(cloud.async_close_session())
+        ```
+        
+        ### Initialization
+        
+        The Crownstone cloud is initialized with the email and password of a user:
+        ```python
+        cloud = CrownstoneCloud('email', 'password')
+        ```
+        If you do not yet have a Crownstone account, go to [My Crownstone](https://my.crownstone.rocks) to set one up.
+        The email and password are used to re-login after an access token has expired.
+        
+        You can log into multiple accounts by creating more CrownstoneCloud objects. When doing so, it is recommended to use
+        only 1 websession for all your requests. Create a websession and append it as parameter to all your CrownstoneCloud
+        objects. Take a look at the async example above.
+        ```python
+        cloud = CrownstoneCloud('email', 'password', websession)
+        ```
+        To log in and get all your Crownstone from the cloud:
+        ```python
+        await cloud.async_initialize()
+        ```
+        
+        ## Data structure
+        
+        The cloud can be displayed with the following structure:
+        * User
+            * Keys
+            * Spheres
+                * Locations
+                * Crownstones
+                * Users
+                
+        
+        ### User
+        
+        The user is the to whom the data belongs.<br> 
+        The user is the one that logs in using email and password.<br>
+        By getting a user specific access token after login, the data for that specific user can be requested.
+        
+        ### Keys
+        
+        The keys are user specific.<br> 
+        They are required to connect to the crownstone bluetooth mesh.<br>
+        The most common used keys are the sphere keys. They are located within each individual sphere.<br>
+        
+        ### Spheres
+        
+        Spheres are the main data entry. They have rooms (locations), Crownstones and users in them.<br>
+        Example spheres:
+        * House
+        * Office
+        * Apartment
+        
+        A Sphere has the following fields in the cloud lib:
+        * crownstones: Crownstones
+        * locations: Locations
+        * users: Users
+        * keys: Dict (optional, default = None)
+        * name: String
+        * cloud_id: String
+        * unique_id: String
+        * present_people: List
+        
+        ### Locations
+        
+        Locations are the rooms in your house or other building.<br>
+        For example for a house: 
+        * Living room
+        * Bedroom
+        * Garage
+        * Bathroom
+        
+        A Location has the following fields in the cloud lib:
+        * present_people: List
+        * name: String
+        * cloud_id: String
+        * unique_id: String
+        
+        ### Crownstones
+        
+        Crownstones are smart plugs that can make every device that isn't smart, way smarter!<br>
+        Crownstones are located within a sphere.<br>
+        Example names of Crownstones:
+        * Lamp
+        * Charger
+        * Television
+        
+        A Crownstone has the following fields in the cloud lib:
+        * abilities: Dict
+        * state: Int (0..100)
+        * name: String
+        * unique_id: String
+        * cloud_id: String
+        * type: String
+        * sw_version: String
+        
+        ### Users
+        
+        Users are people who have access to a sphere.<br>
+        A user can have 3 roles:
+        * Admin
+        * Member
+        * Guest
+        
+        A User has the following fields in the cloud lib:
+        * role: String
+        * first_name: String
+        * last_name: String
+        * email: String
+        * cloud_id: String
+        * email_verified: Bool
+        
+        ## Function list
+        
+        ### Cloud
+        
+        #### async_initialize()
+        > Login and sync all data for the user from the cloud.
+        
+        #### async_synchronize()
+        > Synchronize all data for a user. Use case is to update the local data with new data from the cloud.
+        > This function is already called in `async_initialize()`.
+        
+        #### get_crownstone(crownstone_name: String, sphere_id: String = None) -> Crownstone
+        > Get a Crownstone object by name for a user. Raises CrownstoneNotFoundError if it doesn't exist.
+        > You can optionally provide a sphere id to match where the Crownstone should be found.
+        
+        #### get_crownstone_by_id(crownstone_id: String, sphere_id: String = None) -> Crownstone
+        > Get a Crownstone object by it's id for a user. Raises CrownstoneNotFoundError if it doesn't exist.
+        > You can optionally provide a sphere id to match where the Crownstone should be found.
+        
+        #### get_crownstone_by_uid(crownstone_uid: int, sphere_id: String = None) -> Crownstone
+        > Get a Crownstone object by it's uid for a user. Raises CrownstoneNotFoundError if it doesn't exist.
+        > You can optionally provide a sphere id to match where the Crownstone should be found.
+        
+        #### async_close_session()
+        > Async function. This will close the websession in requestHandler to cleanup nicely after the program has finished.
+        
+        ### Spheres
+        
+        #### async_update_sphere_data()
+        > Async function. Sync the Spheres with the cloud. Calling the function again after init will update the current data.
+        
+        #### find(sphere_name: String) -> Sphere
+        > Returns a sphere object if one exists by that name.
+        
+        #### find_by_id(sphere_id: String) -> Sphere
+        > Return a sphere object if one exists by that id.
+        
+        ### Sphere
+        
+        #### async_update_sphere_presence()
+        > Async function. Sync the presence of users in the sphere with the cloud.
+        
+        #### async_get_keys() -> Dict
+        > Async function. Returns a dict with the keys of this sphere. 
+        > The keys can be used for BLE connectivity with the Crownstones.
+        
+        ### Crownstones
+        
+        #### async_update_crownstone_data()
+        > Async function. Sync the Crownstones with the cloud for a sphere. 
+        > Calling the function again after init will update the current data.
+        
+        #### find(crownstone_name: String) -> Crownstone
+        > Return a Crownstone object if one exists by that name.
+        
+        #### find_by_id(crownstone_id: String) -> Crownstone
+        > Return a Crownstone object if one exists by that id.
+        
+        ### Crownstone
+        
+        #### async_turn_on()
+        > Async function. Send a command to turn a Crownstone on. 
+        > To make this work make sure to be in the selected sphere and have Bluetooth enabled on your phone.
+        
+        #### async_turn_off()
+        > Async function. Send a command to turn a Crownstone off. 
+        > To make this work make sure to be in the selected sphere and have Bluetooth enabled on your phone.
+        
+        #### async_set_brightness(value: Integer)
+        > Async function. Send a command to set a Crownstone to a given brightness level. 
+        > To make this work make sure to be in the selected sphere and have Bluetooth enabled on your phone.
+        > The value parameter should be between 0 and 100.
+        
+        ### Locations
+        
+        #### async_update_location_data()
+        > Async function. Sync the Locations with the cloud for a sphere. Calling the function again after init will update the current data.
+        
+        #### async_update_location_presence()
+        > Async function. Sync the presence with the cloud. This will replace the current presence with the new presence.
+        
+        #### find(location_name: String) -> Location
+        > Return a location object if one exists by that name.
+        
+        #### find_by_id(location_id: String) -> Location
+        > Return a location object if one exists by that id.
+        
+        ### Users
+        
+        #### async_update_user_data()
+        > Async function. Sync the Users with the cloud for a sphere. Calling the function again after init will update the current data.
+        
+        #### find_by_first_name(first_name: String) -> List
+        > Returns a list of all users with that first name, as duplicate first names can exist.
+        
+        #### find_by_last_name(last_name: String) -> List
+        > Return a list of all users with that last name, as duplicate last names can exist.
+        
+        #### find_by_id(user_id: String) -> Location
+        > Return a location object if one exists by that id.
+        
+        ## Async vs sync
+        The lib can be used synchronously and asynchronously.<br>
+        The disadvantage of sync context is that all functions are blocking. 
+        The program will simply wait until a function is complete. In async context, functions (coroutines) can yield control,
+        which means that functions can be "paused" while they are waiting for external data to come in, like data from a server.
+        Other functions can then be executed in the meantime. This way the program is always busy.<br>
+        
+        All async functions in the library API functions in this library have the prefix **async_**
+        Async functions need to be awaited:
+        ```Python
+        await cloud.async_close_session()
+        ```
+        All the async functions mentioned above can also be used synchronously.<br>
+        Use the `run_async()` function like so:
+        ```Python
+        from crownstone_cloud import run_async
+        
+        run_async(cloud.async_close_session())
+        ```
+        Make sure to see the examples above!
+        
+        ## Testing
+        
+        To run the tests using tox install tox first by running:
+        ```console
+        $ pip install tox
+        ```
+        To execute the tests cd to the project folder and run:
+        ```console
+        $ tox
+        ```
+        To see which parts of the code are covered by the tests, a coverage report is generated after the tests have been successful.<br>
+        To see the coverage report run:
+        ```console
+        $ coverage report
+        ```
+        If you like to get a better overview of the test you can generate a HTML file like so:
+        ```console
+        $ coverage html
+        ```
+        To view your html file directly on Linux:
+        ```console
+        $ ./htmlcov/index.html
+        ```
+        On Windows simply navigate to the htmlcov folder inside the project folder, and double-click index.html. It will be executed in your selected browser.
+        
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
-# crownstone-lib-python-cloud
-
-Asynchronous Python library to get data from the cloud, and switch Crownstones.
-
-## Functionality
-
-* Async: using asyncio and aiohttp, optimized for speed.
-* Easy to use: sync all your Crownstone Cloud data with just one command!
-* Structurally sound: find your data with ease!
-* Complete: set the switch state and brightness of your Crownstones remotely!
-* Flexible: Login and get the data for multiple accounts at once!
-
-## Requirements
-
-* Python 3.8 or higher
-* Aiohttp 3.7.4
-
-## Standard installation
-
-cd to the project folder and run:
-```console
-$ python setup.py install
-```
-
-## Install in a virtual environment
-
-To install the library execute the following command:
-```console
-$ python -m venv venv
-```
-Activate your venv using:
-```console
-$ source venv/bin/activate
-```
-Once activated, the venv is used to executed python files, and libraries will be installed in the venv.<br>
-To install this library, cd to the project folder and run:
-```console
-$ python setup.py install
-```
-
-## Getting started
-
-### Examples
-
-#### Async example
-
-```python
-from crownstone_cloud import CrownstoneCloud, create_clientsession
-import logging
-import asyncio
-
-# Enable logging.
-logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.DEBUG)
-
-
-async def main():
-    # Every instance creates it's own websession for easy accessibility, however using 1 websession is recommended.
-    # Create your websession like so:
-    websession = create_clientsession()
-    # Initialize cloud.
-    cloud_user_1 = CrownstoneCloud('email_user_1', 'password_user_1', websession)
-    # Login to the Crownstone Cloud and synchronize all cloud data.
-    await cloud_user_1.async_initialize()
-
-    # Get a crownstone by name that can dim, and put it on 20% brightness for user 1
-    crownstone_lamp = cloud_user_1.get_crownstone('Lamp')
-    await crownstone_lamp.async_set_brightness(20)
-
-    # Login & synchronize data for an other account.
-    cloud_user_2 = CrownstoneCloud('email_user_2', 'password_user_2', websession)
-    await cloud_user_2.async_initialize()
-
-    # Get a crownstone by name and turn it on for user 2.
-    crownstone_tv = cloud_user_2.get_crownstone('TV')
-    await crownstone_tv.async_turn_on()
-
-    # If you want to update specific data you can get the cloud data object for your user.
-    # This object has all the cloud data for your user saved in it, which was synced with async_initialize()
-    # Parts of the data can also be synced individually without touching the other data.
-    # To sync all data at once, use async_synchronize() instead.
-    my_sphere = cloud_user_1.cloud_data.find("my_sphere_name")
-    # request to sync only the locations with the cloud
-    await my_sphere.locations.async_update_location_data()
-    # get the keys for this sphere so you can use them with the Crownstone BLE python library
-    sphere_keys = await my_sphere.async_get_keys()
-
-    # Close the aiohttp clientsession after we are done.
-    await websession.close()
-
-asyncio.run(main())
-```
-
-#### Sync example
-
-```python
-from crownstone_cloud import CrownstoneCloud, run_async
-import logging
-
-# Enable logging.
-logging.basicConfig(format='%(levelname)s:%(message)s', level=logging.DEBUG)
-
-# Initialize cloud.
-cloud = CrownstoneCloud('email', 'password')
-# Use 'run_async' to run async functions in sync context.
-# Login & synchronize all cloud data.
-run_async(cloud.async_initialize())
-
-# Get a crownstone by name and turn it on.
-crownstone_coffee_machine = cloud.get_crownstone('Coffee machine')
-run_async(crownstone_coffee_machine.async_turn_on())
-
-# Close the session after we are done.
-run_async(cloud.async_close_session())
-```
-
-### Initialization
-
-The Crownstone cloud is initialized with the email and password of a user:
-```python
-cloud = CrownstoneCloud('email', 'password')
-```
-If you do not yet have a Crownstone account, go to [My Crownstone](https://my.crownstone.rocks) to set one up.
-The email and password are used to re-login after an access token has expired.
-
-You can log into multiple accounts by creating more CrownstoneCloud objects. When doing so, it is recommended to use
-only 1 websession for all your requests. Create a websession and append it as parameter to all your CrownstoneCloud
-objects. Take a look at the async example above.
-```python
-cloud = CrownstoneCloud('email', 'password', websession)
-```
-To log in and get all your Crownstone from the cloud:
-```python
-await cloud.async_initialize()
-```
-
-## Data structure
-
-The cloud can be displayed with the following structure:
-* User
-    * Keys
-    * Spheres
-        * Locations
-        * Crownstones
-        * Users
-        
-
-### User
-
-The user is the to whom the data belongs.<br> 
-The user is the one that logs in using email and password.<br>
-By getting a user specific access token after login, the data for that specific user can be requested.
-
-### Keys
-
-The keys are user specific.<br> 
-They are required to connect to the crownstone bluetooth mesh.<br>
-The most common used keys are the sphere keys. They are located within each individual sphere.<br>
-
-### Spheres
-
-Spheres are the main data entry. They have rooms (locations), Crownstones and users in them.<br>
-Example spheres:
-* House
-* Office
-* Apartment
-
-A Sphere has the following fields in the cloud lib:
-* crownstones: Crownstones
-* locations: Locations
-* users: Users
-* keys: Dict (optional, default = None)
-* name: String
-* cloud_id: String
-* unique_id: String
-* present_people: List
-
-### Locations
-
-Locations are the rooms in your house or other building.<br>
-For example for a house: 
-* Living room
-* Bedroom
-* Garage
-* Bathroom
-
-A Location has the following fields in the cloud lib:
-* present_people: List
-* name: String
-* cloud_id: String
-* unique_id: String
-
-### Crownstones
-
-Crownstones are smart plugs that can make every device that isn't smart, way smarter!<br>
-Crownstones are located within a sphere.<br>
-Example names of Crownstones:
-* Lamp
-* Charger
-* Television
-
-A Crownstone has the following fields in the cloud lib:
-* abilities: Dict
-* state: Int (0..100)
-* name: String
-* unique_id: String
-* cloud_id: String
-* type: String
-* sw_version: String
-
-### Users
-
-Users are people who have access to a sphere.<br>
-A user can have 3 roles:
-* Admin
-* Member
-* Guest
-
-A User has the following fields in the cloud lib:
-* role: String
-* first_name: String
-* last_name: String
-* email: String
-* cloud_id: String
-* email_verified: Bool
-
-## Function list
-
-### Cloud
-
-#### async_initialize()
-> Login and sync all data for the user from the cloud.
-
-#### async_synchronize()
-> Synchronize all data for a user. Use case is to update the local data with new data from the cloud.
-> This function is already called in `async_initialize()`.
-
-#### get_crownstone(crownstone_name: String, sphere_id: String = None) -> Crownstone
-> Get a Crownstone object by name for a user. Raises CrownstoneNotFoundError if it doesn't exist.
-> You can optionally provide a sphere id to match where the Crownstone should be found.
-
-#### get_crownstone_by_id(crownstone_id: String, sphere_id: String = None) -> Crownstone
-> Get a Crownstone object by it's id for a user. Raises CrownstoneNotFoundError if it doesn't exist.
-> You can optionally provide a sphere id to match where the Crownstone should be found.
-
-#### get_crownstone_by_uid(crownstone_uid: int, sphere_id: String = None) -> Crownstone
-> Get a Crownstone object by it's uid for a user. Raises CrownstoneNotFoundError if it doesn't exist.
-> You can optionally provide a sphere id to match where the Crownstone should be found.
-
-#### async_close_session()
-> Async function. This will close the websession in requestHandler to cleanup nicely after the program has finished.
-
-### Spheres
-
-#### async_update_sphere_data()
-> Async function. Sync the Spheres with the cloud. Calling the function again after init will update the current data.
-
-#### find(sphere_name: String) -> Sphere
-> Returns a sphere object if one exists by that name.
-
-#### find_by_id(sphere_id: String) -> Sphere
-> Return a sphere object if one exists by that id.
-
-### Sphere
-
-#### async_update_sphere_presence()
-> Async function. Sync the presence of users in the sphere with the cloud.
-
-#### async_get_keys() -> Dict
-> Async function. Returns a dict with the keys of this sphere. 
-> The keys can be used for BLE connectivity with the Crownstones.
-
-### Crownstones
-
-#### async_update_crownstone_data()
-> Async function. Sync the Crownstones with the cloud for a sphere. 
-> Calling the function again after init will update the current data.
-
-#### find(crownstone_name: String) -> Crownstone
-> Return a Crownstone object if one exists by that name.
-
-#### find_by_id(crownstone_id: String) -> Crownstone
-> Return a Crownstone object if one exists by that id.
-
-### Crownstone
-
-#### async_turn_on()
-> Async function. Send a command to turn a Crownstone on. 
-> To make this work make sure to be in the selected sphere and have Bluetooth enabled on your phone.
-
-#### async_turn_off()
-> Async function. Send a command to turn a Crownstone off. 
-> To make this work make sure to be in the selected sphere and have Bluetooth enabled on your phone.
-
-#### async_set_brightness(value: Integer)
-> Async function. Send a command to set a Crownstone to a given brightness level. 
-> To make this work make sure to be in the selected sphere and have Bluetooth enabled on your phone.
-> The value parameter should be between 0 and 100.
-
-### Locations
-
-#### async_update_location_data()
-> Async function. Sync the Locations with the cloud for a sphere. Calling the function again after init will update the current data.
-
-#### async_update_location_presence()
-> Async function. Sync the presence with the cloud. This will replace the current presence with the new presence.
-
-#### find(location_name: String) -> Location
-> Return a location object if one exists by that name.
-
-#### find_by_id(location_id: String) -> Location
-> Return a location object if one exists by that id.
-
-### Users
-
-#### async_update_user_data()
-> Async function. Sync the Users with the cloud for a sphere. Calling the function again after init will update the current data.
-
-#### find_by_first_name(first_name: String) -> List
-> Returns a list of all users with that first name, as duplicate first names can exist.
-
-#### find_by_last_name(last_name: String) -> List
-> Return a list of all users with that last name, as duplicate last names can exist.
-
-#### find_by_id(user_id: String) -> Location
-> Return a location object if one exists by that id.
-
-## Async vs sync
-The lib can be used synchronously and asynchronously.<br>
-The disadvantage of sync context is that all functions are blocking. 
-The program will simply wait until a function is complete. In async context, functions (coroutines) can yield control,
-which means that functions can be "paused" while they are waiting for external data to come in, like data from a server.
-Other functions can then be executed in the meantime. This way the program is always busy.<br>
-
-All async functions in the library API functions in this library have the prefix **async_**
-Async functions need to be awaited:
-```Python
-await cloud.async_close_session()
-```
-All the async functions mentioned above can also be used synchronously.<br>
-Use the `run_async()` function like so:
-```Python
-from crownstone_cloud import run_async
-
-run_async(cloud.async_close_session())
-```
-Make sure to see the examples above!
-
-## Testing
-
-To run the tests using tox install tox first by running:
-```console
-$ pip install tox
-```
-To execute the tests cd to the project folder and run:
-```console
-$ tox
-```
-To see which parts of the code are covered by the tests, a coverage report is generated after the tests have been successful.<br>
-To see the coverage report run:
-```console
-$ coverage report
-```
-If you like to get a better overview of the test you can generate a HTML file like so:
-```console
-$ coverage html
-```
-To view your html file directly on Linux:
-```console
-$ ./htmlcov/index.html
-```
-On Windows simply navigate to the htmlcov folder inside the project folder, and double-click index.html. It will be executed in your selected browser.
-
-
```

### Comparing `crownstone-cloud-1.4.8/crownstone_cloud.egg-info/SOURCES.txt` & `crownstone-cloud-1.4.9/crownstone_cloud.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-LICENSE.md
 MANIFEST.in
 README.md
 requirements.txt
 setup.py
 crownstone_cloud/__init__.py
 crownstone_cloud/cloud.py
 crownstone_cloud/const.py
```

### Comparing `crownstone-cloud-1.4.8/setup.py` & `crownstone-cloud-1.4.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='crownstone-cloud',
-    version="1.4.8",
+    version="1.4.9",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/crownstone/crownstone-lib-python-cloud',
     author='Crownstone B.V.',
     packages=find_packages(exclude=['examples', 'tests']),
     install_requires=list(package.strip() for package in open('requirements.txt')),
     classifiers=[
```

### Comparing `crownstone-cloud-1.4.8/tests/mocked_replies/crownstone_data.py` & `crownstone-cloud-1.4.9/tests/mocked_replies/crownstone_data.py`

 * *Files identical despite different names*

### Comparing `crownstone-cloud-1.4.8/tests/mocked_replies/errors.py` & `crownstone-cloud-1.4.9/tests/mocked_replies/errors.py`

 * *Files identical despite different names*

### Comparing `crownstone-cloud-1.4.8/tests/mocked_replies/location_data.py` & `crownstone-cloud-1.4.9/tests/mocked_replies/location_data.py`

 * *Files identical despite different names*

### Comparing `crownstone-cloud-1.4.8/tests/mocked_replies/sphere_data.py` & `crownstone-cloud-1.4.9/tests/mocked_replies/sphere_data.py`

 * *Files identical despite different names*

### Comparing `crownstone-cloud-1.4.8/tests/mocked_replies/user_data.py` & `crownstone-cloud-1.4.9/tests/mocked_replies/user_data.py`

 * *Files identical despite different names*

