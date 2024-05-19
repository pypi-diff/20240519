# Comparing `tmp/gym_simplegrid-1.0.5.tar.gz` & `tmp/gym_simplegrid-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gym_simplegrid-1.0.5.tar", last modified: Wed Aug 23 13:00:50 2023, max compression
+gzip compressed data, was "gym_simplegrid-1.0.6.tar", last modified: Sun May 19 11:46:48 2024, max compression
```

## Comparing `gym_simplegrid-1.0.5.tar` & `gym_simplegrid-1.0.6.tar`

### file list

```diff
@@ -1,20 +1,18 @@
-drwxr-xr-x   0 leodamato   (501) staff       (20)        0 2023-08-23 13:00:50.049311 gym_simplegrid-1.0.5/
--rw-r--r--   0 leodamato   (501) staff       (20)    11355 2022-04-12 14:25:12.000000 gym_simplegrid-1.0.5/LICENSE
--rw-r--r--   0 leodamato   (501) staff       (20)     5784 2023-08-23 13:00:50.049034 gym_simplegrid-1.0.5/PKG-INFO
--rw-rw-r--   0 leodamato   (501) staff       (20)     5226 2023-08-23 12:59:26.000000 gym_simplegrid-1.0.5/README.md
-drwxr-xr-x   0 leodamato   (501) staff       (20)        0 2023-08-23 13:00:50.044952 gym_simplegrid-1.0.5/gym_simplegrid/
--rw-r--r--   0 leodamato   (501) staff       (20)      478 2023-08-17 01:06:06.000000 gym_simplegrid-1.0.5/gym_simplegrid/__init__.py
-drwxr-xr-x   0 leodamato   (501) staff       (20)        0 2023-08-23 13:00:50.048237 gym_simplegrid-1.0.5/gym_simplegrid/envs/
--rw-rw-r--   0 leodamato   (501) staff       (20)       58 2023-08-14 11:27:43.000000 gym_simplegrid-1.0.5/gym_simplegrid/envs/__init__.py
--rw-r--r--   0 leodamato   (501) staff       (20)    16240 2023-08-23 12:38:19.000000 gym_simplegrid-1.0.5/gym_simplegrid/envs/simple_grid.py
--rw-r--r--   0 leodamato   (501) staff       (20)     7367 2023-08-14 12:45:45.000000 gym_simplegrid-1.0.5/gym_simplegrid/rendering.py
--rw-r--r--   0 leodamato   (501) staff       (20)     2295 2023-08-23 08:49:23.000000 gym_simplegrid-1.0.5/gym_simplegrid/window.py
-drwxr-xr-x   0 leodamato   (501) staff       (20)        0 2023-08-23 13:00:50.047233 gym_simplegrid-1.0.5/gym_simplegrid.egg-info/
--rw-r--r--   0 leodamato   (501) staff       (20)     5784 2023-08-23 13:00:49.000000 gym_simplegrid-1.0.5/gym_simplegrid.egg-info/PKG-INFO
--rw-r--r--   0 leodamato   (501) staff       (20)      377 2023-08-23 13:00:49.000000 gym_simplegrid-1.0.5/gym_simplegrid.egg-info/SOURCES.txt
--rw-r--r--   0 leodamato   (501) staff       (20)        1 2023-08-23 13:00:49.000000 gym_simplegrid-1.0.5/gym_simplegrid.egg-info/dependency_links.txt
--rw-r--r--   0 leodamato   (501) staff       (20)       21 2023-08-23 13:00:49.000000 gym_simplegrid-1.0.5/gym_simplegrid.egg-info/requires.txt
--rw-r--r--   0 leodamato   (501) staff       (20)       15 2023-08-23 13:00:49.000000 gym_simplegrid-1.0.5/gym_simplegrid.egg-info/top_level.txt
--rw-r--r--   0 leodamato   (501) staff       (20)       84 2022-04-14 11:44:55.000000 gym_simplegrid-1.0.5/pyproject.toml
--rw-r--r--   0 leodamato   (501) staff       (20)       38 2023-08-23 13:00:50.049414 gym_simplegrid-1.0.5/setup.cfg
--rw-r--r--   0 leodamato   (501) staff       (20)      816 2023-08-23 13:00:37.000000 gym_simplegrid-1.0.5/setup.py
+drwxr-xr-x   0 leodamato   (501) staff       (20)        0 2024-05-19 11:46:48.525585 gym_simplegrid-1.0.6/
+-rw-r--r--   0 leodamato   (501) staff       (20)    11355 2022-04-12 14:25:12.000000 gym_simplegrid-1.0.6/LICENSE
+-rw-r--r--   0 leodamato   (501) staff       (20)     5788 2024-05-19 11:46:48.524984 gym_simplegrid-1.0.6/PKG-INFO
+-rw-r--r--   0 leodamato   (501) staff       (20)     5216 2024-05-19 11:40:31.000000 gym_simplegrid-1.0.6/README.md
+drwxr-xr-x   0 leodamato   (501) staff       (20)        0 2024-05-19 11:46:48.516519 gym_simplegrid-1.0.6/gym_simplegrid/
+-rw-r--r--   0 leodamato   (501) staff       (20)      478 2023-08-23 13:45:24.000000 gym_simplegrid-1.0.6/gym_simplegrid/__init__.py
+drwxr-xr-x   0 leodamato   (501) staff       (20)        0 2024-05-19 11:46:48.523178 gym_simplegrid-1.0.6/gym_simplegrid/envs/
+-rw-r--r--   0 leodamato   (501) staff       (20)       58 2023-08-23 13:45:24.000000 gym_simplegrid-1.0.6/gym_simplegrid/envs/__init__.py
+-rw-r--r--   0 leodamato   (501) staff       (20)    14481 2024-05-19 11:17:12.000000 gym_simplegrid-1.0.6/gym_simplegrid/envs/simple_grid.py
+drwxr-xr-x   0 leodamato   (501) staff       (20)        0 2024-05-19 11:46:48.524348 gym_simplegrid-1.0.6/gym_simplegrid.egg-info/
+-rw-r--r--   0 leodamato   (501) staff       (20)     5788 2024-05-19 11:46:48.000000 gym_simplegrid-1.0.6/gym_simplegrid.egg-info/PKG-INFO
+-rw-r--r--   0 leodamato   (501) staff       (20)      324 2024-05-19 11:46:48.000000 gym_simplegrid-1.0.6/gym_simplegrid.egg-info/SOURCES.txt
+-rw-r--r--   0 leodamato   (501) staff       (20)        1 2024-05-19 11:46:48.000000 gym_simplegrid-1.0.6/gym_simplegrid.egg-info/dependency_links.txt
+-rw-r--r--   0 leodamato   (501) staff       (20)       21 2024-05-19 11:46:48.000000 gym_simplegrid-1.0.6/gym_simplegrid.egg-info/requires.txt
+-rw-r--r--   0 leodamato   (501) staff       (20)       15 2024-05-19 11:46:48.000000 gym_simplegrid-1.0.6/gym_simplegrid.egg-info/top_level.txt
+-rw-r--r--   0 leodamato   (501) staff       (20)       84 2022-04-14 11:44:55.000000 gym_simplegrid-1.0.6/pyproject.toml
+-rw-r--r--   0 leodamato   (501) staff       (20)       38 2024-05-19 11:46:48.525770 gym_simplegrid-1.0.6/setup.cfg
+-rw-r--r--   0 leodamato   (501) staff       (20)      816 2024-05-19 10:24:50.000000 gym_simplegrid-1.0.6/setup.py
```

### Comparing `gym_simplegrid-1.0.5/LICENSE` & `gym_simplegrid-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gym_simplegrid-1.0.5/PKG-INFO` & `gym_simplegrid-1.0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: gym_simplegrid
-Version: 1.0.5
+Version: 1.0.6
 Summary: Simple Gridworld Environment for Gymnasium
 Home-page: https://github.com/damat-le/gym-simplegrid
 Author: Leo D'Amato
 Author-email: leo.damato.dev@gmail.com
-License: UNKNOWN
 Keywords: reinforcement learning,environment,gridworld,agent,rl,openaigym,openai-gym,gym,gymnasium,farama-foundation
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: gymnasium
+Requires-Dist: matplotlib
 
-# Simple Gridworld Environment for OpenAI Gym
+# Simple Gridworld Gymnasium Environment
 
-SimpleGrid is a super simple gridworld environment for [Gymnasium](https://gymnasium.farama.org/). It is easy to use and customise and it is intended to offer an environment for quickly testing and prototyping different RL algorithms.
+SimpleGrid is a super simple grid environment for [Gymnasium](https://gymnasium.farama.org/). It is easy to use and customise and it is intended to offer an environment for quickly testing and prototyping different RL algorithms.
 
 It is also efficient, lightweight and has few dependencies (gymnasium, numpy, matplotlib). 
 
 ![](img/simplegrid.gif)
 
 SimpleGrid involves navigating a grid from a Start (red tile) to a Goal (green tile) state without colliding with any Wall (black tiles) by walking over the Empty (white tiles) cells. The yellow circle denotes the agent's current position. 
 
@@ -173,14 +173,12 @@
         return 0.0
 ```
 
 It is possible to subclass the `SimpleGridEnv` class  and to override this method to define custom rewards.
 
 ## Notes on rendering
 
-The default frame rate is 5 FPS. It is possible to change it through the `metadata` dictionary. 
+The default frame rate is 8 FPS. It is possible to change it through the `metadata` dictionary. 
 
 To properly render the environment, remember that the point (x,y) in the desc matrix corresponds to the point (y,x) in the rendered matrix.
 This is because the rendering code works in terms of width and height while the computation in the environment is done using x and y coordinates.
 You don't have to worry about this unless you play with the environment's internals.
-
-
```

### Comparing `gym_simplegrid-1.0.5/README.md` & `gym_simplegrid-1.0.6/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-# Simple Gridworld Environment for OpenAI Gym
+# Simple Gridworld Gymnasium Environment
 
-SimpleGrid is a super simple gridworld environment for [Gymnasium](https://gymnasium.farama.org/). It is easy to use and customise and it is intended to offer an environment for quickly testing and prototyping different RL algorithms.
+SimpleGrid is a super simple grid environment for [Gymnasium](https://gymnasium.farama.org/). It is easy to use and customise and it is intended to offer an environment for quickly testing and prototyping different RL algorithms.
 
 It is also efficient, lightweight and has few dependencies (gymnasium, numpy, matplotlib). 
 
 ![](img/simplegrid.gif)
 
 SimpleGrid involves navigating a grid from a Start (red tile) to a Goal (green tile) state without colliding with any Wall (black tiles) by walking over the Empty (white tiles) cells. The yellow circle denotes the agent's current position. 
 
@@ -157,12 +157,12 @@
         return 0.0
 ```
 
 It is possible to subclass the `SimpleGridEnv` class  and to override this method to define custom rewards.
 
 ## Notes on rendering
 
-The default frame rate is 5 FPS. It is possible to change it through the `metadata` dictionary. 
+The default frame rate is 8 FPS. It is possible to change it through the `metadata` dictionary. 
 
 To properly render the environment, remember that the point (x,y) in the desc matrix corresponds to the point (y,x) in the rendered matrix.
 This is because the rendering code works in terms of width and height while the computation in the environment is done using x and y coordinates.
 You don't have to worry about this unless you play with the environment's internals.
```

### Comparing `gym_simplegrid-1.0.5/gym_simplegrid/envs/simple_grid.py` & `gym_simplegrid-1.0.6/gym_simplegrid/envs/simple_grid.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from __future__ import annotations
 import logging
 import numpy as np
-import gym_simplegrid.rendering as r
-from gym_simplegrid.window import Window
 from gymnasium import spaces, Env
+import matplotlib.pyplot as plt
+import matplotlib as mpl
+import sys
 
 MAPS = {
     "4x4": ["0000", "0101", "0001", "1000"],
     "8x8": [
         "00000000",
         "00000000",
         "00010000",
@@ -31,15 +32,15 @@
      "0001", 
      "1000"]
 
     Assume the environment is a grid of size (nrow, ncol). A state s of the environment is an elemente of gym.spaces.Discete(nrow*ncol), i.e. an integer between 0 and nrow * ncol - 1. Assume nrow=ncol=5 and s=10, to compute the (x,y) coordinates of s on the grid the following formula are used: x = s // ncol  and y = s % ncol.
      
     The user can also decide the starting and goal positions of the agent. This can be done by through the `options` dictionary in the `reset` method. The user can specify the starting and goal positions by adding the key-value pairs(`starts_xy`, v1) and `goals_xy`, v2), where v1 and v2 are both of type int (s) or tuple (x,y) and represent the agent starting and goal positions respectively. 
     """
-    metadata = {"render_modes": ["human", "rgb_array"], 'render_fps': 5}
+    metadata = {"render_modes": ["human", "rgb_array", "ansi"], 'render_fps': 8}
     FREE: int = 0
     OBSTACLE: int = 1
     MOVES: dict[int,tuple] = {
         0: (-1, 0), #UP
         1: (1, 0),  #DOWN
         2: (0, -1), #LEFT
         3: (0, 1)   #RIGHT
@@ -69,20 +70,18 @@
         self.obstacles = self.parse_obstacle_map(obstacle_map) #walls
         self.nrow, self.ncol = self.obstacles.shape
 
         self.action_space = spaces.Discrete(len(self.MOVES))
         self.observation_space = spaces.Discrete(n=self.nrow*self.ncol)
 
         # Rendering configuration
+        self.fig = None
+
         self.render_mode = render_mode
-        self.window = None
-        self.agent_color = 'yellow'
-        self.tile_cache = {}
         self.fps = self.metadata['render_fps']
-        #self.frames = []
 
     def reset(
             self, 
             seed: int | None = None, 
             options: dict = dict()
         ) -> tuple:
         """
@@ -103,28 +102,31 @@
         self.start_xy = self.parse_state_option('start_loc', options)
         self.goal_xy = self.parse_state_option('goal_loc', options)
 
         # initialise internal vars
         self.agent_xy = self.start_xy
         self.reward = self.get_reward(*self.agent_xy)
         self.done = self.on_goal()
+        self.agent_action = None
+        self.n_iter = 0
 
         # Check integrity
         self.integrity_checks()
 
         #if self.render_mode == "human":
         self.render()
 
         return self.get_obs(), self.get_info()
     
     def step(self, action: int):
         """
         Take a step in the environment.
         """
         #assert action in self.action_space
+        self.agent_action = action
 
         # Get the current position of the agent
         row, col = self.agent_xy
         dx, dy = self.MOVES[action]
 
         # Compute the target position of the agent
         target_row = row + dx
@@ -134,14 +136,16 @@
         self.reward = self.get_reward(target_row, target_col)
         
         # Check if the move is valid
         if self.is_in_bounds(target_row, target_col) and self.is_free(target_row, target_col):
             self.agent_xy = (target_row, target_col)
             self.done = self.on_goal()
 
+        self.n_iter += 1
+
         # if self.render_mode == "human":
         self.render()
 
         return self.get_obs(), self.reward, self.done, False, self.get_info()
     
     def parse_obstacle_map(self, obstacle_map) -> np.ndarray:
         """
@@ -253,197 +257,143 @@
         else:
             return 0.0
 
     def get_obs(self) -> int:
         return self.to_s(*self.agent_xy)
     
     def get_info(self) -> dict:
-        return {'agent_xy': self.agent_xy}
-
-    def close(self):
-        """
-        Close the environment.
-        """
-        if self.window:
-            self.window.close()
-        return None
+        return {
+            'agent_xy': self.agent_xy,
+            'n_iter': self.n_iter,
+        }
 
     def render(self):
         """
         Render the environment.
         """
-        if self.render_mode == "human":
-            img = self.render_frame()
-            if not self.window:
-                self.window = Window()
-                self.window.show(block=False)
-            caption = ''
-            self.window.show_img(img, caption, self.fps)
+        if self.render_mode is None:
             return None
+        
+        elif self.render_mode == "ansi":
+            s = f"{self.n_iter},{self.agent_xy[0]},{self.agent_xy[1]},{self.reward},{self.done},{self.agent_action}\n"
+            #print(s)
+            return s
+
         elif self.render_mode == "rgb_array":
-            return self.render_frame()
-        # elif mode == "rgb_array_list":
-        #     img = self.render_frame(caption=caption)
-        #     self.frames.append(img)
-        #     return self.frames
+            self.render_frame()
+            self.fig.canvas.draw()
+            img = np.array(self.fig.canvas.renderer.buffer_rgba())
+            return img
+    
+        elif self.render_mode == "human":
+            self.render_frame()
+            plt.pause(1/self.fps)
+            return None
+        
         else:
             raise ValueError(f"Unsupported rendering mode {self.render_mode}")
+
+    def render_frame(self):
+        if self.fig is None:
+            self.render_initial_frame()
+            self.fig.canvas.mpl_connect('close_event', self.close)
+        else:
+            self.update_agent_patch()
+        self.ax.set_title(f"Step: {self.n_iter}, Reward: {self.reward}")
     
-    def render_frame(self, tile_size=r.TILE_PIXELS, highlight_mask=None):
+    def create_agent_patch(self):
         """
-        @NOTE: Once again, if agent position is (x,y) then, to properly 
-        render it, we have to pass (y,x) to the grid.render method.
+        Create a Circle patch for the agent.
 
-        tile_size: tile size in pixels
+        @NOTE: If agent position is (x,y) then, to properly render it, we have to pass (y,x) as center to the Circle patch.
         """
-        width = self.ncol
-        height = self.nrow
-
-        if highlight_mask is None:
-            highlight_mask = np.zeros(shape=(width, height), dtype=bool)
-
-        # Compute the total grid size
-        width_px = width * tile_size
-        height_px = height * tile_size
-
-        img = np.zeros(shape=(height_px, width_px, 3), dtype=np.uint8)
-
-        # Render grid with obstacles
-        for x in range(self.nrow):
-            for y in range(self.ncol):
-                if self.obstacles[x,y] == self.OBSTACLE:
-                    cell = r.Wall(color='black')
-                else:
-                    cell = None
-
-                img = self.update_cell_in_frame(img, x, y, cell, tile_size)
-
-        # Render start
-        x, y = self.start_xy
-        cell = r.ColoredTile(color="red")
-        img = self.update_cell_in_frame(img, x, y, cell, tile_size)
-
-        # Render goal
-        x, y = self.goal_xy
-        cell = r.ColoredTile(color="green")
-        img = self.update_cell_in_frame(img, x, y, cell, tile_size)
+        return mpl.patches.Circle(
+            (self.agent_xy[1]+.5, self.agent_xy[0]+.5), 
+            0.3, 
+            facecolor='orange', 
+            fill=True, 
+            edgecolor='black', 
+            linewidth=1.5,
+            zorder=100,
+        )
 
-        # Render agent
-        x, y = self.agent_xy
-        cell = r.Agent(color=self.agent_color)
-        img = self.update_cell_in_frame(img, x, y, cell, tile_size)
-
-        return img
-        
-    def render_cell(
-        self,
-        obj: r.WorldObj,
-        highlight=False,
-        tile_size=r.TILE_PIXELS,
-        subdivs=3
-    ):
+    def update_agent_patch(self):
         """
-        Render a tile and cache the result
+        @NOTE: If agent position is (x,y) then, to properly 
+        render it, we have to pass (y,x) as center to the Circle patch.
         """
+        self.agent_patch.center = (self.agent_xy[1]+.5, self.agent_xy[0]+.5)
+        return None
+    
+    def render_initial_frame(self):
+        """
+        Render the initial frame.
 
-        # Hash map lookup key for the cache
-        if not isinstance(obj, r.Agent):
-            key = (None, highlight, tile_size)
-            key = obj.encode() + key if obj else key
-
-            if key in self.tile_cache:
-                return self.tile_cache[key]
-
-        img = np.zeros(shape=(tile_size * subdivs, tile_size * subdivs, 3), dtype=np.uint8) + 255
-
-        if obj != None:
-            obj.render(img)
-
-        # Highlight the cell if needed
-        if highlight:
-            r.highlight_img(img)
-
-        # Draw the grid lines (top and left edges)
-        r.fill_coords(img, r.point_in_rect(0, 0.031, 0, 1), (170, 170, 170))
-        r.fill_coords(img, r.point_in_rect(0, 1, 0, 0.031), (170, 170, 170))
-
-        # Downsample the image to perform supersampling/anti-aliasing
-        img = r.downsample(img, subdivs)
-
-        # Cache the rendered tile
-        if not isinstance(obj, r.Agent):
-            self.tile_cache[key] = img
+        @NOTE: 0: free cell (white), 1: obstacle (black), 2: start (red), 3: goal (green)
+        """
+        data = self.obstacles.copy()
+        data[self.start_xy] = 2
+        data[self.goal_xy] = 3
+
+        colors = ['white', 'black', 'red', 'green']
+        bounds=[i-0.1 for i in [0, 1, 2, 3, 4]]
+
+        # create discrete colormap
+        cmap = mpl.colors.ListedColormap(colors)
+        norm = mpl.colors.BoundaryNorm(bounds, cmap.N)
+
+        plt.ion()
+        fig, ax = plt.subplots()
+        self.fig = fig
+        self.ax = ax
+
+        #ax.grid(axis='both', color='#D3D3D3', linewidth=2) 
+        ax.grid(axis='both', color='k', linewidth=1.3) 
+        ax.set_xticks(np.arange(0, data.shape[1], 1))  # correct grid sizes
+        ax.set_yticks(np.arange(0, data.shape[0], 1))
+        ax.tick_params(
+            bottom=False, 
+            top=False, 
+            left=False, 
+            right=False, 
+            labelbottom=False, 
+            labelleft=False
+        ) 
+
+        # draw the grid
+        ax.imshow(
+            data, 
+            cmap=cmap, 
+            norm=norm,
+            extent=[0, data.shape[1], data.shape[0], 0],
+            interpolation='none'
+        )
+
+        # Create white holes on start and goal positions
+        for pos in [self.start_xy, self.goal_xy]:
+            wp = self.create_white_patch(*pos)
+            ax.add_patch(wp)
+
+        # Create agent patch in start position
+        self.agent_patch = self.create_agent_patch()
+        ax.add_patch(self.agent_patch)
 
-        return img
+        return None
 
-    def update_cell_in_frame(self, img, x, y, cell, tile_size):
+    def create_white_patch(self, x, y):
         """
-        Parameters
-        ----------
-        img : np.ndarray
-            Image to update.
-        x : int
-            x-coordinate of the cell to update.
-        y : int
-            y-coordinate of the cell to update.
-        cell : r.WorldObj
-            New cell to render.
-        tile_size : int
-            Size of the cell in pixels.
-        """
-        tile_img = self.render_cell(cell, tile_size=tile_size)
-        height_min = x * tile_size
-        height_max = (x+1) * tile_size
-        width_min = y * tile_size
-        width_max = (y+1) * tile_size
-        img[height_min:height_max, width_min:width_max, :] = tile_img
-        return img
-
-    def encode(self, vis_mask=None):
-        """
-        Produce a compact numpy encoding of the grid
-        """
-    #     width = self.ncol
-    #     height = self.nrow
-
-    #     if vis_mask is None:
-    #         vis_mask = np.ones((width, height), dtype=bool)
-
-    #     array = np.zeros((width, height, 3), dtype='uint8')
-
-    #     for i in range(width):
-    #         for j in range(height):
-    #             if vis_mask[i, j]:
-    #                 v = self.get(i, j)
-
-    #                 if v is None:
-    #                     array[i, j, 0] = r.OBJECT_TO_IDX['empty']
-    #                     array[i, j, 1] = 0
-    #                     array[i, j, 2] = 0
-
-    #                 else:
-    #                     array[i, j, :] = v.encode()
-
-    #     return array
-        pass
-
-    @staticmethod
-    def decode(array):
-        """
-        Decode an array grid encoding back into a grid
-        """
-
-    #     width, height, channels = array.shape
-    #     assert channels == 3
-
-    #     vis_mask = np.ones(shape=(width, height), dtype=bool)
-
-    #     grid = SimpleGrid(width, height)
-    #     for i in range(width):
-    #         for j in range(height):
-    #             type_idx, color_idx, state = array[i, j]
-    #             v = WorldObj.decode(type_idx, color_idx, state)
-    #             grid.set(i, j, v)
-    #             vis_mask[i, j] = (type_idx != OBJECT_TO_IDX['unseen'])
+        Render a white patch in the given position.
+        """
+        return mpl.patches.Circle(
+            (y+.5, x+.5), 
+            0.4, 
+            color='white', 
+            fill=True, 
+            zorder=99,
+        )
 
-    #     return grid, vis_mask
-        pass
+    def close(self, *args):
+        """
+        Close the environment.
+        """
+        plt.close(self.fig)
+        sys.exit()
```

### Comparing `gym_simplegrid-1.0.5/gym_simplegrid.egg-info/PKG-INFO` & `gym_simplegrid-1.0.6/gym_simplegrid.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
-Name: gym-simplegrid
-Version: 1.0.5
+Name: gym_simplegrid
+Version: 1.0.6
 Summary: Simple Gridworld Environment for Gymnasium
 Home-page: https://github.com/damat-le/gym-simplegrid
 Author: Leo D'Amato
 Author-email: leo.damato.dev@gmail.com
-License: UNKNOWN
 Keywords: reinforcement learning,environment,gridworld,agent,rl,openaigym,openai-gym,gym,gymnasium,farama-foundation
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: gymnasium
+Requires-Dist: matplotlib
 
-# Simple Gridworld Environment for OpenAI Gym
+# Simple Gridworld Gymnasium Environment
 
-SimpleGrid is a super simple gridworld environment for [Gymnasium](https://gymnasium.farama.org/). It is easy to use and customise and it is intended to offer an environment for quickly testing and prototyping different RL algorithms.
+SimpleGrid is a super simple grid environment for [Gymnasium](https://gymnasium.farama.org/). It is easy to use and customise and it is intended to offer an environment for quickly testing and prototyping different RL algorithms.
 
 It is also efficient, lightweight and has few dependencies (gymnasium, numpy, matplotlib). 
 
 ![](img/simplegrid.gif)
 
 SimpleGrid involves navigating a grid from a Start (red tile) to a Goal (green tile) state without colliding with any Wall (black tiles) by walking over the Empty (white tiles) cells. The yellow circle denotes the agent's current position. 
 
@@ -173,14 +173,12 @@
         return 0.0
 ```
 
 It is possible to subclass the `SimpleGridEnv` class  and to override this method to define custom rewards.
 
 ## Notes on rendering
 
-The default frame rate is 5 FPS. It is possible to change it through the `metadata` dictionary. 
+The default frame rate is 8 FPS. It is possible to change it through the `metadata` dictionary. 
 
 To properly render the environment, remember that the point (x,y) in the desc matrix corresponds to the point (y,x) in the rendered matrix.
 This is because the rendering code works in terms of width and height while the computation in the environment is done using x and y coordinates.
 You don't have to worry about this unless you play with the environment's internals.
-
-
```

### Comparing `gym_simplegrid-1.0.5/setup.py` & `gym_simplegrid-1.0.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='gym_simplegrid',
-    version='1.0.5',
+    version='1.0.6',
     keywords='reinforcement learning, environment, gridworld, agent, rl, openaigym, openai-gym, gym, gymnasium, farama-foundation',
     url='https://github.com/damat-le/gym-simplegrid',
     description='Simple Gridworld Environment for Gymnasium',
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=['gym_simplegrid', 'gym_simplegrid.envs'],
     install_requires=[
```

