# Comparing `tmp/my_road-2.0.2.tar.gz` & `tmp/my_road-2.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "my_road-2.0.2.tar", last modified: Sat May 18 23:09:08 2024, max compression
+gzip compressed data, was "my_road-2.0.3.tar", last modified: Sat May 18 23:17:09 2024, max compression
```

## Comparing `my_road-2.0.2.tar` & `my_road-2.0.3.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxrwx   0        0        0        0 2024-05-18 23:09:08.353833 my_road-2.0.2/
--rw-rw-rw-   0        0        0     1088 2024-05-18 21:54:26.000000 my_road-2.0.2/LICENSE
--rw-rw-rw-   0        0        0    26064 2024-05-18 23:09:08.353833 my_road-2.0.2/PKG-INFO
--rw-rw-rw-   0        0        0    25849 2024-05-18 23:09:05.000000 my_road-2.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-18 23:09:08.352833 my_road-2.0.2/my_road.egg-info/
--rw-rw-rw-   0        0        0    26064 2024-05-18 23:09:08.000000 my_road-2.0.2/my_road.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      161 2024-05-18 23:09:08.000000 my_road-2.0.2/my_road.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-18 23:09:08.000000 my_road-2.0.2/my_road.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-05-18 23:09:08.000000 my_road-2.0.2/my_road.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      629 2024-05-18 23:08:38.000000 my_road-2.0.2/my_road.py
--rw-rw-rw-   0        0        0       42 2024-05-18 23:09:08.354833 my_road-2.0.2/setup.cfg
--rw-rw-rw-   0        0        0      356 2024-05-18 23:09:05.000000 my_road-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-18 23:17:09.341906 my_road-2.0.3/
+-rw-rw-rw-   0        0        0     1088 2024-05-18 21:54:26.000000 my_road-2.0.3/LICENSE
+-rw-rw-rw-   0        0        0    26195 2024-05-18 23:17:09.341906 my_road-2.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0    25980 2024-05-18 23:16:31.000000 my_road-2.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-18 23:17:09.340906 my_road-2.0.3/my_road.egg-info/
+-rw-rw-rw-   0        0        0    26195 2024-05-18 23:17:09.000000 my_road-2.0.3/my_road.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      161 2024-05-18 23:17:09.000000 my_road-2.0.3/my_road.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 23:17:09.000000 my_road-2.0.3/my_road.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-05-18 23:17:09.000000 my_road-2.0.3/my_road.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      652 2024-05-18 23:16:31.000000 my_road-2.0.3/my_road.py
+-rw-rw-rw-   0        0        0       42 2024-05-18 23:17:09.342905 my_road-2.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      356 2024-05-18 23:17:01.000000 my_road-2.0.3/setup.py
```

### Comparing `my_road-2.0.2/LICENSE` & `my_road-2.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `my_road-2.0.2/PKG-INFO` & `my_road-2.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: my_road
-Version: 2.0.2
+Version: 2.0.3
 Summary: long Road or not????
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Смотри на дорогу
 
 ## Использование
 
+`road('число циклов' 'скорость')`
+
+Eсли не менять скорость то она равна 0.025
+
 ```
 from my_road import my_road
 
 road(1) #От числа зависит длина дороги
 
 # Вывод
 .                                                                                                .                                                                                                .
```

### Comparing `my_road-2.0.2/README.md` & `my_road-2.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Смотри на дорогу
 
 ## Использование
 
+`road('число циклов' 'скорость')`
+
+Eсли не менять скорость то она равна 0.025
+
 ```
 from my_road import my_road
 
 road(1) #От числа зависит длина дороги
 
 # Вывод
 .                                                                                                .                                                                                                .
```

### Comparing `my_road-2.0.2/my_road.egg-info/PKG-INFO` & `my_road-2.0.3/my_road.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 Metadata-Version: 2.1
 Name: my_road
-Version: 2.0.2
+Version: 2.0.3
 Summary: long Road or not????
 Author: k0ng999
 Author-email: baydar_14@mail.ru
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Смотри на дорогу
 
 ## Использование
 
+`road('число циклов' 'скорость')`
+
+Eсли не менять скорость то она равна 0.025
+
 ```
 from my_road import my_road
 
 road(1) #От числа зависит длина дороги
 
 # Вывод
 .                                                                                                .                                                                                                .
```

### Comparing `my_road-2.0.2/my_road.py` & `my_road-2.0.3/my_road.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 __all__ = ['my_road']
 
 import time
 
 
-def cycle():
+def cycle(speed=0.025):
     string = '.'
     a = 0
     b = True
     while b:
         if a <= 15:
             for i in range(1, 65 + 1):
                 print(f'{string * i:97}.{string * i:>97}')
                 a += 1
-                time.sleep(0.025)
+                time.sleep(speed)
                 if a == 65:
                     for i in range(65, 0, -1):
                         print(f"{string * i:97}.{string * i:>97}")
-                        time.sleep(0.025)
+                        time.sleep(speed)
                         if i == 1:
                             b = False
 
 
-def my_road(num):
+def my_road(num, speed):
     for i in range(1, num + 1):
-        cycle()
+        cycle(speed)
```

