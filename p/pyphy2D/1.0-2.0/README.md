# Comparing `tmp/pyphy2D-1.0.tar.gz` & `tmp/pyphy2D-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyphy2D-1.0.tar", last modified: Sat May 18 12:08:02 2024, max compression
+gzip compressed data, was "pyphy2D-2.0.tar", last modified: Sun May 19 17:37:19 2024, max compression
```

## Comparing `pyphy2D-1.0.tar` & `pyphy2D-2.0.tar`

### file list

```diff
@@ -1,25 +1,27 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 12:08:02.072235 pyphy2D-1.0/
--rw-rw-rw-   0        0        0     1088 2024-05-18 09:18:42.000000 pyphy2D-1.0/LICENSE
--rw-rw-rw-   0        0        0     1562 2024-05-18 12:08:02.067248 pyphy2D-1.0/PKG-INFO
--rw-rw-rw-   0        0        0     1143 2024-05-18 12:07:38.000000 pyphy2D-1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 12:08:02.045227 pyphy2D-1.0/pyphy/
--rw-rw-rw-   0        0        0      173 2024-05-18 12:07:25.000000 pyphy2D-1.0/pyphy/__init__.py
--rw-rw-rw-   0        0        0     7430 2024-05-18 12:07:25.000000 pyphy2D-1.0/pyphy/body.py
--rw-rw-rw-   0        0        0      225 2024-05-18 12:07:25.000000 pyphy2D-1.0/pyphy/boundingbox.py
--rw-rw-rw-   0        0        0      452 2024-05-18 12:07:25.000000 pyphy2D-1.0/pyphy/collision_manifold.py
--rw-rw-rw-   0        0        0    10138 2024-05-18 12:07:25.000000 pyphy2D-1.0/pyphy/collisions.py
--rw-rw-rw-   0        0        0     1174 2024-05-14 20:33:36.000000 pyphy2D-1.0/pyphy/pygame_integration.py
--rw-rw-rw-   0        0        0     1388 2024-05-18 12:07:25.000000 pyphy2D-1.0/pyphy/pyphymath.py
--rw-rw-rw-   0        0        0     1370 2024-05-18 12:07:25.000000 pyphy2D-1.0/pyphy/sample.py
--rw-rw-rw-   0        0        0      311 2024-05-18 12:07:25.000000 pyphy2D-1.0/pyphy/transform.py
--rw-rw-rw-   0        0        0     2874 2024-05-13 15:57:53.000000 pyphy2D-1.0/pyphy/vector2.py
--rw-rw-rw-   0        0        0     9970 2024-05-18 12:07:25.000000 pyphy2D-1.0/pyphy/world.py
-drwxrwxrwx   0        0        0        0 2024-05-18 12:08:02.064230 pyphy2D-1.0/pyphy2D.egg-info/
--rw-rw-rw-   0        0        0     1562 2024-05-18 12:08:01.000000 pyphy2D-1.0/pyphy2D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      410 2024-05-18 12:08:01.000000 pyphy2D-1.0/pyphy2D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 12:08:01.000000 pyphy2D-1.0/pyphy2D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-18 12:08:01.000000 pyphy2D-1.0/pyphy2D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2024-05-18 12:08:01.000000 pyphy2D-1.0/pyphy2D.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      101 2024-05-18 10:35:03.000000 pyphy2D-1.0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-18 12:08:02.073233 pyphy2D-1.0/setup.cfg
--rw-rw-rw-   0        0        0      590 2024-05-18 12:07:14.000000 pyphy2D-1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:37:19.187569 pyphy2D-2.0/
+-rw-rw-rw-   0        0        0     1088 2024-05-18 09:18:42.000000 pyphy2D-2.0/LICENSE
+-rw-rw-rw-   0        0        0     1956 2024-05-19 17:37:19.172580 pyphy2D-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1537 2024-05-19 17:25:56.000000 pyphy2D-2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 17:37:19.137563 pyphy2D-2.0/pyphy/
+-rw-rw-rw-   0        0        0      585 2024-05-19 17:20:10.000000 pyphy2D-2.0/pyphy/__init__.py
+-rw-rw-rw-   0        0        0     6090 2024-05-19 17:20:18.000000 pyphy2D-2.0/pyphy/body.py
+-rw-rw-rw-   0        0        0      225 2024-05-19 17:20:22.000000 pyphy2D-2.0/pyphy/boundingbox.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:37:19.143566 pyphy2D-2.0/pyphy/c_src_files/
+-rw-rw-rw-   0        0        0   516863 2024-05-19 17:35:51.000000 pyphy2D-2.0/pyphy/c_src_files/collisions_c.c
+-rw-rw-rw-   0        0        0   357469 2024-05-19 17:35:51.000000 pyphy2D-2.0/pyphy/c_src_files/resolveCollisions_c.c
+-rw-rw-rw-   0        0        0      452 2024-05-19 17:20:30.000000 pyphy2D-2.0/pyphy/collision_manifold.py
+-rw-rw-rw-   0        0        0     1174 2024-05-14 20:33:36.000000 pyphy2D-2.0/pyphy/pygame_integration.py
+-rw-rw-rw-   0        0        0     1388 2024-05-19 17:20:40.000000 pyphy2D-2.0/pyphy/pyphymath.py
+-rw-rw-rw-   0        0        0     1352 2024-05-19 12:43:10.000000 pyphy2D-2.0/pyphy/sample.py
+-rw-rw-rw-   0        0        0      311 2024-05-19 17:20:48.000000 pyphy2D-2.0/pyphy/transform.py
+-rw-rw-rw-   0        0        0     2979 2024-05-19 16:40:00.000000 pyphy2D-2.0/pyphy/vector2.py
+-rw-rw-rw-   0        0        0     5588 2024-05-19 17:21:00.000000 pyphy2D-2.0/pyphy/world.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:37:19.168580 pyphy2D-2.0/pyphy2D.egg-info/
+-rw-rw-rw-   0        0        0     1956 2024-05-19 17:37:18.000000 pyphy2D-2.0/pyphy2D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      463 2024-05-19 17:37:19.000000 pyphy2D-2.0/pyphy2D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 17:37:18.000000 pyphy2D-2.0/pyphy2D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-19 17:37:18.000000 pyphy2D-2.0/pyphy2D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       39 2024-05-19 17:37:18.000000 pyphy2D-2.0/pyphy2D.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      101 2024-05-18 10:35:03.000000 pyphy2D-2.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 17:37:19.188583 pyphy2D-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      945 2024-05-19 17:34:54.000000 pyphy2D-2.0/setup.py
```

### Comparing `pyphy2D-1.0/LICENSE` & `pyphy2D-2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyphy2D-1.0/PKG-INFO` & `pyphy2D-2.0/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,71 +1,59 @@
-Metadata-Version: 2.1
-Name: pyphy2D
-Version: 1.0
-Summary: A 2D Rigid Body Physics Engine.
-Author: Krishiv Goel
-Author-email: KrishivGoelXD@gmail.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: pygame
-
 # PyPhy2D
 
 ## Description
-
 PyPhy2D is a 2D Rigid Body Physics Engine designed to simulate physical interactions of objects in a two-dimensional space. It is easy to integrate and can be used for games, simulations, and educational purposes.
 
-## License
+## Whats New In PyPhy2D Version 2.0?
+PyPhy2D now comes with the simplicity of python and the blazing speeds of C.
+With the help of the cython engine PyPhy2D can now use C for heavy computations for a smoother operation.
+Through benchmarks PyPhy2D 2.0 comes out to be 10-20x faster than version 1.0.
 
+## License
 This project is licensed under the MIT License.
 
 ## Installation
-
 Before installing PyPhy2D, ensure you have PyGame installed:
 
 ```sh
 pip install pygame
 
 ```
 or
-
 ```sh
 pip install pygame-ce
 
 ```
 
 ## Example Project
-
 ```python
 from pyphy import World, Body, Vector2
 import pygame
 import sys
 
 WIDTH, HEIGHT = 900, 900
 WINDOW = pygame.display.set_mode((WIDTH, HEIGHT))
 
-space = World(window=WINDOW, gravity=(0, 9.8))
+physicsAccuracy = 1 # precision of the engine (directly hits the performance)
+
+space = World(window=WINDOW, gravity=(0, 9.8), physicsAccuracy)
 
 clock = pygame.time.Clock()
 FPS = 60
 
 testBody = Body.CreateCircleBody(radius=25, center=Vector2(100, 100), density=1.2, restitution=0.8, static=False)
 space.AddBody(testBody)
 
 while True:
-    dt = clock.tick(60) / 1000
+    dt = clock.tick(FPS) / 1000
 
     space.step(dt)
 
     WINDOW.fill((0, 0, 0))
     space.Render()
 
     pygame.display.update()
 
     for event in pygame.event.get():
         if event.type == pygame.QUIT:
             sys.exit()
-```
+```
```

### Comparing `pyphy2D-1.0/pyphy/body.py` & `pyphy2D-2.0/pyphy/body.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from pyphy.pygame_integration import PyphyPygame
 from pyphy.transform import Transform
 from pyphy.boundingbox import AABB
 from pyphy.vector2 import Vector2
 from pyphy.pyphymath import math
+import body_c
 
 class Body:
     CIRCLE = 0
     BOX = 1
     POLYGON = 2
 
     def __init__(self, pos: Vector2, mass: float, density: float, restitution: float, area: float, shape, radius: float, width: float, height: float, static: bool, vertices=None) -> None:
@@ -27,15 +28,15 @@
         self.isStatic = static
 
         if self.shape != Body.CIRCLE:
             self.vertices = vertices or self.__createBoxVertices__(width, height)
         else:
             self.vertices = None
 
-        self.Inertia = self.CalculateRotationalInertia()
+        self.Inertia, self.shape = body_c.CalculateRotationalInertia(self.shape, self.mass, self.radius, self.width, self.height, self.vertices, self.density)
         self.InvInertia = 0 if self.isStatic else (1 / self.Inertia)
 
         self.StaticFriction = 0.6
         self.DynamicFriction = 0.4
 
         self.force = Vector2.zero()
 
@@ -69,42 +70,14 @@
         return [
             Vector2(-width/2, height/2),
             Vector2(width/2, height/2),
             Vector2(width/2, -height/2),
             Vector2(-width/2, -height/2)
         ]
     
-    @staticmethod
-    def __calculatePolygonArea__(vertices: list[Vector2]) -> float:
-        n = len(vertices)
-        area = 0.0
-        for i in range(n):
-            j = (i + 1) % n
-            area += vertices[i].x * vertices[j].y
-            area -= vertices[j].x * vertices[i].y
-        area = abs(area) / 2.0
-        return area
-    
-    def CalculateRotationalInertia(self) -> float:
-        if self.shape == Body.CIRCLE:
-            return self.mass * self.radius ** 2 / 2
-
-        elif self.shape == Body.BOX:
-            return self.mass / 12 * (self.width ** 2 + self.height ** 2)
-        
-        elif self.shape == Body.POLYGON:
-            inertia = 0.0
-            for i in range(len(self.vertices)):
-                j = (i + 1) % len(self.vertices)
-                cross = self.vertices[i].cross(self.vertices[j])
-                dot = self.vertices[i].dot(self.vertices[i] + self.vertices[j])
-                inertia += (cross * dot)
-            self.shape = Body.BOX
-            return (self.density / 6.0) * abs(inertia)
-    
     def getAABB(self) -> AABB:
         if not self.aabbUpdateRequired:
             return self.aabb
 
         minX = float('inf')
         minY = float('inf')
         maxX = float('-inf')
@@ -164,33 +137,25 @@
 
     def Rotate(self, angle: float) -> None:
         self.angle += angle
         self.angle %= 360
         self.transformedVerticesUpdateRequired = True
         self.aabbUpdateRequired = True
 
-    @staticmethod
-    def __scale_and_transform_vertices__(vertices: list[Vector2], width: float, height: float, position: Vector2) -> list[Vector2]:
-        scaled_vertices = []
-        for vertex in vertices:
-            scaled_vertex = Vector2(vertex.x * width, -vertex.y * height)
-            scaled_vertices.append(scaled_vertex)
-        return scaled_vertices
-
     @classmethod
     def CreateCircleBody(cls, radius: float, center: Vector2, density: float, restitution: float, static: bool) -> "Body":
         area = 3.14 * radius ** 2
         mass = area * density
         return cls(center, mass, density, math.clamp(restitution, 0, 1), area, Body.CIRCLE, radius, 0, 0, static)
 
     @classmethod
     def CreateBoxBody(cls, width: float, height: float, pos: Vector2, density: float, restitution: float, static: bool) -> "Body":
         area = width * height
         mass = area * density
         return cls(pos, mass, density, math.clamp(restitution, 0, 1), area, Body.BOX, 0, width, height, static)
     
     @classmethod
     def CreatePolygon(cls, vertices: list[Vector2], width: float, height: float, pos: Vector2, density: float, restitution: float, static: bool) -> "Body":
-        transformed_vertices = cls.__scale_and_transform_vertices__(vertices, width, height, pos)
-        area = cls.__calculatePolygonArea__(transformed_vertices)
+        transformed_vertices = body_c.scale_and_transform_vertices(vertices, width, height)
+        area = body_c.calculatePolygonArea(transformed_vertices)
         mass = area * density
         return cls(pos, mass, density, math.clamp(restitution, 0, 1), area, Body.POLYGON, 0, width, height, static, transformed_vertices)
```

### Comparing `pyphy2D-1.0/pyphy/pygame_integration.py` & `pyphy2D-2.0/pyphy/pygame_integration.py`

 * *Files identical despite different names*

### Comparing `pyphy2D-1.0/pyphy/pyphymath.py` & `pyphy2D-2.0/pyphy/pyphymath.py`

 * *Files identical despite different names*

### Comparing `pyphy2D-1.0/pyphy/sample.py` & `pyphy2D-2.0/pyphy/sample.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from pyphy.vector2 import Vector2
-from pyphy.world import World
-from pyphy.body import Body
+from vector2 import Vector2
+from world import World
+from body import Body
 import pygame as pg
 
 pg.init()
 
 WIDTH, HEIGHT = 1280, 720
 WINDOW = pg.display.set_mode((WIDTH, HEIGHT))
 pg.display.set_caption('Dummy File')
```

### Comparing `pyphy2D-1.0/pyphy/vector2.py` & `pyphy2D-2.0/pyphy/vector2.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,14 +21,18 @@
     def to_tuple(self) -> tuple[float, float]:
         return (self.x, self.y)
     
     @property
     def magnitude(self) -> float:
         return (self.x**2 + self.y**2)**0.5
     
+    @property
+    def perpendicular(self) -> "Vector2":
+        return Vector2(-self.y, self.x)
+    
     @classmethod
     def from_tuple(cls, tup) -> "Vector2":
         if not isinstance(tup, tuple):
             raise TypeError(f'Invalid Input {type(tup)}')
         return Vector2(*tup)
 
     @classmethod
```

### Comparing `pyphy2D-1.0/pyphy2D.egg-info/PKG-INFO` & `pyphy2D-2.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,66 +1,68 @@
 Metadata-Version: 2.1
 Name: pyphy2D
-Version: 1.0
+Version: 2.0
 Summary: A 2D Rigid Body Physics Engine.
 Author: Krishiv Goel
 Author-email: KrishivGoelXD@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pygame
 
 # PyPhy2D
 
 ## Description
-
 PyPhy2D is a 2D Rigid Body Physics Engine designed to simulate physical interactions of objects in a two-dimensional space. It is easy to integrate and can be used for games, simulations, and educational purposes.
 
-## License
+## Whats New In PyPhy2D Version 2.0?
+PyPhy2D now comes with the simplicity of python and the blazing speeds of C.
+With the help of the cython engine PyPhy2D can now use C for heavy computations for a smoother operation.
+Through benchmarks PyPhy2D 2.0 comes out to be 10-20x faster than version 1.0.
 
+## License
 This project is licensed under the MIT License.
 
 ## Installation
-
 Before installing PyPhy2D, ensure you have PyGame installed:
 
 ```sh
 pip install pygame
 
 ```
 or
-
 ```sh
 pip install pygame-ce
 
 ```
 
 ## Example Project
-
 ```python
 from pyphy import World, Body, Vector2
 import pygame
 import sys
 
 WIDTH, HEIGHT = 900, 900
 WINDOW = pygame.display.set_mode((WIDTH, HEIGHT))
 
-space = World(window=WINDOW, gravity=(0, 9.8))
+physicsAccuracy = 1 # precision of the engine (directly hits the performance)
+
+space = World(window=WINDOW, gravity=(0, 9.8), physicsAccuracy)
 
 clock = pygame.time.Clock()
 FPS = 60
 
 testBody = Body.CreateCircleBody(radius=25, center=Vector2(100, 100), density=1.2, restitution=0.8, static=False)
 space.AddBody(testBody)
 
 while True:
-    dt = clock.tick(60) / 1000
+    dt = clock.tick(FPS) / 1000
 
     space.step(dt)
 
     WINDOW.fill((0, 0, 0))
     space.Render()
 
     pygame.display.update()
```

