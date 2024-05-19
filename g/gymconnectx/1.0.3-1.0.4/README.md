# Comparing `tmp/gymconnectx-1.0.3.tar.gz` & `tmp/gymconnectx-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gymconnectx-1.0.3.tar", last modified: Fri May 17 23:59:22 2024, max compression
+gzip compressed data, was "gymconnectx-1.0.4.tar", last modified: Sun May 19 07:50:51 2024, max compression
```

## Comparing `gymconnectx-1.0.3.tar` & `gymconnectx-1.0.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:59:22.603245 gymconnectx-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-17 23:59:18.000000 gymconnectx-1.0.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-17 23:59:22.603245 gymconnectx-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4885 2024-05-17 23:59:18.000000 gymconnectx-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:59:22.599244 gymconnectx-1.0.3/gymconnectx/
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-17 23:59:18.000000 gymconnectx-1.0.3/gymconnectx/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:59:22.603245 gymconnectx-1.0.3/gymconnectx/envs/
--rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-17 23:59:18.000000 gymconnectx-1.0.3/gymconnectx/envs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    26694 2024-05-17 23:59:18.000000 gymconnectx-1.0.3/gymconnectx/envs/gymconnectxenv.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-17 23:59:22.603245 gymconnectx-1.0.3/gymconnectx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6856 2024-05-17 23:59:22.000000 gymconnectx-1.0.3/gymconnectx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-17 23:59:22.000000 gymconnectx-1.0.3/gymconnectx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-17 23:59:22.000000 gymconnectx-1.0.3/gymconnectx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-17 23:59:22.000000 gymconnectx-1.0.3/gymconnectx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-17 23:59:22.000000 gymconnectx-1.0.3/gymconnectx.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-17 23:59:18.000000 gymconnectx-1.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-17 23:59:22.603245 gymconnectx-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-17 23:59:18.000000 gymconnectx-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:50:51.594297 gymconnectx-1.0.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1073 2024-05-19 07:50:47.000000 gymconnectx-1.0.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-19 07:50:51.594297 gymconnectx-1.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4895 2024-05-19 07:50:47.000000 gymconnectx-1.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:50:51.594297 gymconnectx-1.0.4/gymconnectx/
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-05-19 07:50:47.000000 gymconnectx-1.0.4/gymconnectx/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:50:51.594297 gymconnectx-1.0.4/gymconnectx/envs/
+-rw-r--r--   0 runner    (1001) docker     (127)      118 2024-05-19 07:50:47.000000 gymconnectx-1.0.4/gymconnectx/envs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26410 2024-05-19 07:50:47.000000 gymconnectx-1.0.4/gymconnectx/envs/gymconnectxenv.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 07:50:51.594297 gymconnectx-1.0.4/gymconnectx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6888 2024-05-19 07:50:51.000000 gymconnectx-1.0.4/gymconnectx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      306 2024-05-19 07:50:51.000000 gymconnectx-1.0.4/gymconnectx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 07:50:51.000000 gymconnectx-1.0.4/gymconnectx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-05-19 07:50:51.000000 gymconnectx-1.0.4/gymconnectx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-19 07:50:51.000000 gymconnectx-1.0.4/gymconnectx.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 07:50:47.000000 gymconnectx-1.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 07:50:51.594297 gymconnectx-1.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      745 2024-05-19 07:50:47.000000 gymconnectx-1.0.4/setup.py
```

### Comparing `gymconnectx-1.0.3/LICENSE.md` & `gymconnectx-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `gymconnectx-1.0.3/PKG-INFO` & `gymconnectx-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gymconnectx
-Version: 1.0.3
+Version: 1.0.4
 Summary: An OpenAI Gym Environment Connect X Game with GUI. ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N.
 Home-page: https://github.com/fauzisho/GymConnectX
 Author: Fauzi Sholichin
 License: MIT License
         
         Copyright (c) 2024 AI Trafic Project
         
@@ -22,15 +22,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/fauzisho/GymConnectX
-Keywords: tictactoe,gym,pygame
+Keywords: connect4,gym,pygame,reinforcement learning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: gym
@@ -151,9 +151,9 @@
 - **height** (int): The height of the game board, measured in number of rows. Default is `7`.
 - **reward_winner** (float): The reward given to the winner at the end of the game. Default is `1`.
 - **reward_loser** (float): The penalty (or negative reward) given to the loser at the end of the game. Default is `-1`.
 - **living_reward** (float): A reward given at each step of the game, applicable to all ongoing games. Default is `0`.
 - **max_steps** (int): The maximum number of steps the game can take before it ends. Default is `100`.
 - **delay** (int): Time delay (in milliseconds) between moves, primarily used for GUI purposes. Default is `100`.
 - **square_size** (int): Size of the squares in the GUI. Default is `100`.
-- **avatar_player_1** (string): Base64 format avatar image for player 1. This is used in the GUI.
-- **avatar_player_2** (string): Base64 format avatar image for player 2. This is used in the GUI.
+- **avatar_player_1** (string): Base64/path format avatar image for player 1. This is used in the GUI.
+- **avatar_player_2** (string): Base64/path format avatar image for player 2. This is used in the GUI.
```

### Comparing `gymconnectx-1.0.3/README.md` & `gymconnectx-1.0.4/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -113,9 +113,9 @@
 - **height** (int): The height of the game board, measured in number of rows. Default is `7`.
 - **reward_winner** (float): The reward given to the winner at the end of the game. Default is `1`.
 - **reward_loser** (float): The penalty (or negative reward) given to the loser at the end of the game. Default is `-1`.
 - **living_reward** (float): A reward given at each step of the game, applicable to all ongoing games. Default is `0`.
 - **max_steps** (int): The maximum number of steps the game can take before it ends. Default is `100`.
 - **delay** (int): Time delay (in milliseconds) between moves, primarily used for GUI purposes. Default is `100`.
 - **square_size** (int): Size of the squares in the GUI. Default is `100`.
-- **avatar_player_1** (string): Base64 format avatar image for player 1. This is used in the GUI.
-- **avatar_player_2** (string): Base64 format avatar image for player 2. This is used in the GUI.
+- **avatar_player_1** (string): Base64/path format avatar image for player 1. This is used in the GUI.
+- **avatar_player_2** (string): Base64/path format avatar image for player 2. This is used in the GUI.
```

### Comparing `gymconnectx-1.0.3/gymconnectx/__init__.py` & `gymconnectx-1.0.4/gymconnectx/__init__.py`

 * *Files identical despite different names*

### Comparing `gymconnectx-1.0.3/gymconnectx/envs/gymconnectxenv.py` & `gymconnectx-1.0.4/gymconnectx/envs/gymconnectxenv.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 import os
 import re
 import urllib
+import urllib.request
 from typing import List
 import io
 import gym
 from gym.spaces import Box, Discrete, Tuple
-import base64
+import imgBase64
 import pygame
 import sys
 import numpy as np
 
 
 class PyGameRenderEnv:
     def __init__(self, game_env, square_size, avatar_player_1=None, avatar_player_2=None):
@@ -61,24 +62,18 @@
         """Check if the string is a file path. This is usually the fallback option."""
         return os.path.isfile(string)
 
     def load_image_from_path(self, path):
         """Loads an image from a local file path and resizes it."""
         return self.process_image(pygame.image.load(path))
 
-    def load_image_from_url(self, url):
-        """Loads an image from a URL and resizes it."""
-        with urllib.request.urlopen(url) as response:
-            image_data = response.read()
-        return self.process_image(pygame.image.load(io.BytesIO(image_data)))
-
     def load_avatar(self, avatar_string):
         """Determines the type of the avatar input and loads the image accordingly."""
-        if self.is_url(avatar_string):
-            return self.load_image_from_url(avatar_string)
+        if avatar_string is None:
+            return None
         elif self.is_base64(avatar_string):
             return self.load_image_from_base64(avatar_string)
         elif avatar_string is not None:
             return self.load_image_from_path(avatar_string)
         return None
 
     def load_image_from_base64(self, base64_string):
```

### Comparing `gymconnectx-1.0.3/gymconnectx.egg-info/PKG-INFO` & `gymconnectx-1.0.4/gymconnectx.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gymconnectx
-Version: 1.0.3
+Version: 1.0.4
 Summary: An OpenAI Gym Environment Connect X Game with GUI. ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N.
 Home-page: https://github.com/fauzisho/GymConnectX
 Author: Fauzi Sholichin
 License: MIT License
         
         Copyright (c) 2024 AI Trafic Project
         
@@ -22,15 +22,15 @@
         IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
         FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
         AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
         LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
         OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
         SOFTWARE.
 Project-URL: Homepage, https://github.com/fauzisho/GymConnectX
-Keywords: tictactoe,gym,pygame
+Keywords: connect4,gym,pygame,reinforcement learning
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 Requires-Dist: gym
@@ -151,9 +151,9 @@
 - **height** (int): The height of the game board, measured in number of rows. Default is `7`.
 - **reward_winner** (float): The reward given to the winner at the end of the game. Default is `1`.
 - **reward_loser** (float): The penalty (or negative reward) given to the loser at the end of the game. Default is `-1`.
 - **living_reward** (float): A reward given at each step of the game, applicable to all ongoing games. Default is `0`.
 - **max_steps** (int): The maximum number of steps the game can take before it ends. Default is `100`.
 - **delay** (int): Time delay (in milliseconds) between moves, primarily used for GUI purposes. Default is `100`.
 - **square_size** (int): Size of the squares in the GUI. Default is `100`.
-- **avatar_player_1** (string): Base64 format avatar image for player 1. This is used in the GUI.
-- **avatar_player_2** (string): Base64 format avatar image for player 2. This is used in the GUI.
+- **avatar_player_1** (string): Base64/path format avatar image for player 1. This is used in the GUI.
+- **avatar_player_2** (string): Base64/path format avatar image for player 2. This is used in the GUI.
```

### Comparing `gymconnectx-1.0.3/pyproject.toml` & `gymconnectx-1.0.4/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "gymconnectx"
-version = "1.0.3"
+version = "1.0.4"
 description = "An OpenAI Gym Environment Connect X Game with GUI. ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N."
 readme = "README.md"
 authors = [{ name = "Fauzi Sholichin" }]
 license = { file = "LICENSE.md" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
     "Programming Language :: Python :: 3",
 ]
-keywords = ["tictactoe", "gym", "pygame"]
+keywords = ["connect4", "gym", "pygame", "reinforcement learning"]
 dependencies = ["gym", "pygame"]
 requires-python = ">=3.9"
 
 [project.urls]
 Homepage = "https://github.com/fauzisho/GymConnectX"
```

### Comparing `gymconnectx-1.0.3/setup.py` & `gymconnectx-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='gymconnectx',
-    version='1.0.3',
+    version='1.0.4',
     description='ConnectX is a game for two players that is based on the well-known Connect 4. The goal is to place X coins in a row, column, or diagonal on a board with dimensions M by N.',
     url='https://github.com/fauzisho/GymConnectX',
     author='Fauzi Sholichin',
     license='MIT License',
     packages=find_packages(),
     install_requires=['gym', 'pygame', 'numpy'],
     classifiers=[
```

