# Comparing `tmp/parliamentarch-0.2.tar.gz` & `tmp/parliamentarch-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "parliamentarch-0.2.tar", last modified: Thu May  2 20:38:22 2024, max compression
+gzip compressed data, was "parliamentarch-1.0.tar", last modified: Sun May 19 16:24:27 2024, max compression
```

## Comparing `parliamentarch-0.2.tar` & `parliamentarch-1.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:38:22.186259 parliamentarch-0.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:38:22.182259 parliamentarch-0.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:38:22.182259 parliamentarch-0.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-02 20:38:17.000000 parliamentarch-0.2/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-02 20:38:17.000000 parliamentarch-0.2/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-02 20:38:17.000000 parliamentarch-0.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-02 20:38:17.000000 parliamentarch-0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12498 2024-05-02 20:38:17.000000 parliamentarch-0.2/LISEZMOI.rst
--rw-r--r--   0 runner    (1001) docker     (127)    13883 2024-05-02 20:38:22.186259 parliamentarch-0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11861 2024-05-02 20:38:17.000000 parliamentarch-0.2/README.rst
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-02 20:38:17.000000 parliamentarch-0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-02 20:38:22.186259 parliamentarch-0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:38:22.182259 parliamentarch-0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:38:22.186259 parliamentarch-0.2/src/ParliamentArch.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13883 2024-05-02 20:38:22.000000 parliamentarch-0.2/src/ParliamentArch.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-02 20:38:22.000000 parliamentarch-0.2/src/ParliamentArch.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-02 20:38:22.000000 parliamentarch-0.2/src/ParliamentArch.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-02 20:38:22.000000 parliamentarch-0.2/src/ParliamentArch.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-02 20:38:22.186259 parliamentarch-0.2/src/parliamentarch/
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-02 20:38:17.000000 parliamentarch-0.2/src/parliamentarch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2255 2024-05-02 20:38:17.000000 parliamentarch-0.2/src/parliamentarch/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2034 2024-05-02 20:38:17.000000 parliamentarch-0.2/src/parliamentarch/_util.py
--rw-r--r--   0 runner    (1001) docker     (127)     8732 2024-05-02 20:38:17.000000 parliamentarch-0.2/src/parliamentarch/geometry.py
--rw-r--r--   0 runner    (1001) docker     (127)     6095 2024-05-02 20:38:17.000000 parliamentarch-0.2/src/parliamentarch/svg.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:24:27.438959 parliamentarch-1.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:24:27.434960 parliamentarch-1.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:24:27.438959 parliamentarch-1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1229 2024-05-19 16:24:20.000000 parliamentarch-1.0/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-19 16:24:20.000000 parliamentarch-1.0/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 16:24:20.000000 parliamentarch-1.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     1499 2024-05-19 16:24:20.000000 parliamentarch-1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12947 2024-05-19 16:24:20.000000 parliamentarch-1.0/LISEZMOI.rst
+-rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-05-19 16:24:27.438959 parliamentarch-1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12321 2024-05-19 16:24:20.000000 parliamentarch-1.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-19 16:24:20.000000 parliamentarch-1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 16:24:27.438959 parliamentarch-1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:24:27.434960 parliamentarch-1.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:24:27.438959 parliamentarch-1.0/src/ParliamentArch.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14343 2024-05-19 16:24:27.000000 parliamentarch-1.0/src/ParliamentArch.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-05-19 16:24:27.000000 parliamentarch-1.0/src/ParliamentArch.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 16:24:27.000000 parliamentarch-1.0/src/ParliamentArch.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-19 16:24:27.000000 parliamentarch-1.0/src/ParliamentArch.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 16:24:27.438959 parliamentarch-1.0/src/parliamentarch/
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-19 16:24:20.000000 parliamentarch-1.0/src/parliamentarch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-19 16:24:20.000000 parliamentarch-1.0/src/parliamentarch/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-19 16:24:20.000000 parliamentarch-1.0/src/parliamentarch/_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8869 2024-05-19 16:24:20.000000 parliamentarch-1.0/src/parliamentarch/geometry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6347 2024-05-19 16:24:20.000000 parliamentarch-1.0/src/parliamentarch/svg.py
```

### Comparing `parliamentarch-0.2/.github/workflows/python-package.yml` & `parliamentarch-1.0/.github/workflows/python-package.yml`

 * *Files identical despite different names*

### Comparing `parliamentarch-0.2/.github/workflows/python-publish.yml` & `parliamentarch-1.0/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `parliamentarch-0.2/LICENSE` & `parliamentarch-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `parliamentarch-0.2/LISEZMOI.rst` & `parliamentarch-1.0/LISEZMOI.rst`

 * *Files 3% similar despite different names*

```diff
@@ -23,15 +23,15 @@
   supérieur droit du rectangle sont vides).
 - Les sièges sont placés en rangées, tel que :
   - Les rangées sont des arcs de cercle, concentriques avec les arcs de cercle
     formant l'hémicycle.
   - La différence entre les rayons de deux rangées consécutives est une
     constante appelée "épaisseur de rangée".
   - Les sièges sont des cercles (ou des disques) de rayon égal. Ce rayon divisé
-    par l'épaisseur de rangée donne le "ratio de rayon de siège".
+    par la moitié de l'épaisseur de rangée donne le "ratio de rayon de siège".
   - Le centre d'un siège est placé sur l'arc de la rangée dont il fait partie.
   - Dans une rangée donnée, la distance entre deux sièges voisins est constante.
   - La rangée la plus intérieure est l'arc de cercle le plus petit ayant servi à
     définir l'hémicycle.
   - Le rayon de la rangée la plus extérieure est égal au rayon du cercle
     extérieur moins la moitié de l'épaisseur de rangée, de manière à ce qu'aucun
     siège ne puisse mordre l'arc de cercle extérieur.
@@ -56,16 +56,16 @@
 
 Comme sous-entendu plus haut, plusieurs paramètres peuvent être ajustés pour
 changer la forme de l'hémicycle.
 
 - L'angle sur lequel s'étend l'hémicycle peut être réduit en-dessous de 180°
   (les valeurs plus grandes ne sont pas supportées). Cependant, le cas où
   l'angle est suffisament aigü pour empêcher une rangée de contenir un seul
-  siège n'est pas supporté, et pourra causer des erreurs dans des versions
-  futures.
+  siège n'est pas supporté, peut donner des résultats incorrects, et pourra
+  causer des erreurs dans des versions futures.
 - Le nombre de rangées peut être augmenté par rapport au minimum nécessaire pour
   contenir le nombre de sièges donné.
 - Le ratio de rayon de siège peut être ajusté entre 0 et 1, avec les sièges
   touchant leurs voisins latéraux avec une valeur de 1.
 - Tant que le nombre de sièges n'est pas le nombre maximum que le nombre de
   rangées peut contenir, différentes stratégies peuvent être suivies pour les
   répartir entre les rangées.
@@ -78,32 +78,39 @@
 ``SeatData``
 
 Cette classe est définie et expliquée dans le sous-module SVG ci-dessous, mais
 il est exposé au sein du module principal.
 
 ``write_svg_from_attribution(file, attrib, **kwargs)``
 
-Cette fonction écrit un fichier SVG représentant un hémicycle dans le fichier
-fourni. Les paramètres sont les suivants :
+Cette fonction écrit un fichier SVG représentant un hémicycle. Les paramètres
+sont les suivants :
 
-- ``file: io.TextIOBase`` : un fichier ouvert en mode texte.
+- ``file: str|io.TextIOBase`` : un fichier ouvert en mode texte, ou le chemin
+  vers le fichier sur lequel écrire. Si un chemin est fourni, le fichier sera
+  créé si il n'existe pas, et sera écrasé sinon.
 - ``attrib: dict[SeatData, int]`` : un dictionnaire d'objets SeatData
   s'appliquant à un ensemble de sièges présents dans l'hémicycle, vers le nombre
   de sièges auxquels l'objet s'applique. Typiquement, chaque objet correspond à
   un parti ou un groupe. L'ordre des clés a un sens, et les éléments seront
   disposés de gauche à droite dans l'hémicycle.
 - ``**kwargs`` : tous les paramètres optionnels acceptés par
   ``parliamentarch.geometry.get_seats_centers`` ou par
   ``parliamentarch.svg.write_svg`` peuvent être passés à cette fonction.
 
-``get_svg_from_attribution(attrib, **kwargs)``
+``get_svg_from_attribution(attrib, **kwargs) -> str``
 
 Au lieu d'écrire dans un fichier, cette fonction renvoie le contenu au format
 SVG dans une chaîne de caractères. Les autres paramètres sont identiques.
 
+Interface en ligne de commande
+------------------------------
+
+Voir ``py -m parliamentarch -h`` pour la liste des paramètres.
+
 Contenu du sous-module geometry
 -------------------------------
 
 Ces éléments se trouvent dans le sous-module ``parliamentarch.geometry``.
 
 ``get_nrows_from_nseats(nseats: int, span_angle: float = 180.) -> int``
 
@@ -168,15 +175,15 @@
 triée de gauche à droite.
 
 Contenu du sous-module SVG
 --------------------------
 
 Ces éléments se trouvent dans le sous-module ``parliamentarch.svg``.
 
-``SeatData(data, color, border_size, border_color)``
+``SeatData(data, color, border_size=0, border_color="#000")``
 
 Une classe informant la représentation d'un siège ou d'un groupe de sièges.
 
 - ``data: str`` : métadonnées à propos du groupe de sièges, qui finira dans le
   fichier SVG. Typiquement le nom du parti ou de l'élu.
 - ``color: Color`` : la couleur de remplissage du cercle représentant le siège.
   Accepte divers formats de données : une string "#RGB", "#RRGGBB", "#RGBA" ou
@@ -185,18 +192,20 @@
   de couleurs CSS sont aussi acceptés.
 - ``border_size: float`` : la taille de la bordure du cercle représentant le
   siège. (à documenter avec plus de détails)
 - ``border_color: Color`` : la couleur de la bordure.
 
 ``write_svg(file, seat_centers, seat_actual_radius, *, canvas_size=175, margins=5., write_number_of_seats=True, font_size_factor=...)``
 
-Cette fonction écrit un fichier SVG représentant un hémicycle dans le fichier
-fourni. Les paramètres sont les suivants :
+Cette fonction écrit un fichier SVG représentant un hémicycle. Les paramètres
+sont les suivants :
 
-- ``file: io.TextIOBase`` : un fichier ouvert en mode texte.
+- ``file: str|io.TextIOBase`` : un fichier ouvert en mode texte, ou le chemin
+  vers le fichier sur lequel écrire. Si un chemin est fourni, le fichier sera
+  créé si il n'existe pas, et sera écrasé sinon.
 - ``seat_centers: dict[tuple[float, float], SeatData]`` : un dictionnaire des
   coordonnées (x, y) des centres des sièges vers des objets SeatData.
 - ``seat_actual_radius: float`` : le rayon des sièges, tel que renvoyé par
   ``get_seats_centers``.
 - ``canvas_size: float`` : la hauteur du rectangle 2:1 dans lequel l'hémicycle
   est inscrit.
 - ``margins: float|tuple[float, float]|tuple[float, float, float, float]`` : les
```

### Comparing `parliamentarch-0.2/PKG-INFO` & `parliamentarch-1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParliamentArch
-Version: 0.2
+Version: 1.0
 Summary: Generation of arch-styled parliamentary arches
 Author: Gouvernathor
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Gouvernathor
         
         Redistribution and use in source and binary forms, with or without
@@ -60,16 +60,16 @@
   top right corners of the rectangle are empty).
 - The seats will placed in rows, such that:
   - The rows are semicircular arcs concentric to the inner and outer arcs.
 
   - The difference between the radii of two consecutive rows is a constant
     called the "row thickness" (radii is the plural of radius).
 
-  - The seat are circles (or disk) of equal radius. That radius divided by the
-    row thickness makes the "seat radius factor".
+  - The seat are circles (or disks) of equal radius. That radius divided by half
+    of the row thickness makes the "seat radius factor".
 
   - The center of a seat is on the arc of that seat's row.
   - In a given row, the distance between two neighboring seats is a constant.
   - The innermost row's arc is the inner arc.
   - The radius of the outermost row's arc is equal to the radius of the outer
     arc minus half of the row thickness, such that no seat may overlap the
     outer arc.
@@ -93,16 +93,16 @@
 ---------------
 
 As hinted above, there are several parameters that can be tweaked to change the
 layout of the hemicycle. Among them:
 
 - The span angle of the hemicycle can be set to a value lower than 180° (higher
   values are not supported). However, values so low as to prevent some row from
-  containing even ones seat are not supported, and may raise errors in future
-  versions.
+  containing even one seat are not supported, will yield incorrect results, and
+  may raise errors in future versions.
 - The number of rows can be set higher than the minimum required to hold the
   provided number of seats.
 - The seat radius factor can be changed between 0 and 1, with the seats touching
   their lateral neighbors when the factor is 1.
 - As long as the number of seats is not the maximum number the number of rows
   can hold, different strategies can be chosen to distribute the seats.
 
@@ -114,32 +114,39 @@
 ``SeatData``
 
 This class is defined and explained in the SVG submodule below, but it is
 exposed as part of the main module.
 
 ``write_svg_from_attribution(file, attrib, **kwargs)``
 
-This function writes an SVG file representing a hemicycle to the given file-like
-object. The parameters are as follows:
+This function writes an SVG file representing a hemicycle. The parameters are as
+follows:
 
-- ``file: io.TextIOBase``: a file-like object open in text mode.
+- ``file: str|io.TextIOBase``: a file-like object open in text mode, or the path
+  to the file to write on. If a path is provided, the file will be created if it
+  doesn't exist, and otherwise overwritten.
 - ``attrib: dict[SeatData, int]``: a mapping from a SeatData object applying to
   a number of seats in the resulting hemicycle, to the number of seats each
   object applies to. Typically, each SeatData object corresponds to a group or
   party. The ordering of the keys matter, and the elements will be arranged from
   left to right in the hemicycle.
 - ``**kwargs``: all optional keyword parameters taken by
   ``parliamentarch.geometry.get_seats_centers`` or by
   ``parliamentarch.svg.write_svg`` can be passed to this function.
 
-``get_svg_from_attribution(attrib, **kwargs)``
+``get_svg_from_attribution(attrib, **kwargs) -> str``
 
 Instead of writing it to a file, this function returns the SVG content as a
 string. The parameters are otherwise the same.
 
+Command-line interface
+----------------------
+
+See ``py -m parliamentarch -h`` for the accepted parameters.
+
 Geometry submodule contents
 ---------------------------
 
 These are found in the ``parliamentarch.geometry`` submodule.
 
 ``get_nrows_from_nseats(nseats: int, span_angle: float = 180.) -> int``
 
@@ -206,15 +213,15 @@
 arranged from left to right.
 
 SVG submodule content
 ---------------------
 
 These are found in the ``parliamentarch.svg`` submodule.
 
-``SeatData(data, color, border_size, border_color)``
+``SeatData(data, color, border_size=0, border_color="#000")``
 
 A class representing how to display a given seat or set of seats.
 
 - ``data: str``: metadata about the group of seats, which will end up in the
   SVG file. Typically the name of the party or of the member.
 - ``color: Color``: the color with which to fill the seat circles. This may take
   any number of formats: a "#RGB", "#RRGGBB", "#RGBA" or "#RRGGBBAA" string, a
@@ -222,18 +229,20 @@
   ints between 0 and 255. CSS color names are also supported.
 - ``border_size: float``: the size of the border around the seat circle. (to be
   documented at greater length)
 - ``border_color: Color``: the color of the border.
 
 ``write_svg(file, seat_centers, seat_actual_radius, *, canvas_size=175, margins=5., write_number_of_seats=True, font_size_factor=...)``
 
-This function writes an SVG file representing a hemicycle to the given file-like
-object. The parameters are as follows:
+This function writes an SVG file representing a hemicycle. The parameters are as
+follows:
 
-- ``file: io.TextIOBase``: a file-like object open in text mode.
+- ``file: str|io.TextIOBase``: a file-like object open in text mode, or the path
+  to the file to write on. If a path is provided, the file will be created if it
+  doesn't exist, and otherwise overwritten.
 - ``seat_centers: dict[tuple[float, float], SeatData]``: a mapping from the
   (x, y) coordinates of each seat's center to a SeatData object.
 - ``seat_actual_radius: float``: as output by ``get_seats_centers``.
 - ``canvas_size: float``: the height of the 2:1 rectangle in which the hemicycle
   will be drawn.
 - ``margins: float|tuple[float, float]|tuple[float, float, float, float]``:
   the margins around that rectangle. If four values are given, they are the
@@ -284,7 +293,8 @@
 - Allow SeatData to take some <a> element properties (like href), and if so use <a> instead of <g>
 - Allow SeatData to contain more creative SVG content like gradients
   - Maybe give it a .wrap method that wraps the circles in a g or a, and make it subclassable ?
   - Maybe just give a style method ?
 - Add tests
 - Add the option to force all rows to contain an even number of seats
 - Add a simpler way to input parameters in CLI
+  - Maybe by allowing the use of the standard input to pass JSON content ?
```

### Comparing `parliamentarch-0.2/README.rst` & `parliamentarch-1.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -21,16 +21,16 @@
   top right corners of the rectangle are empty).
 - The seats will placed in rows, such that:
   - The rows are semicircular arcs concentric to the inner and outer arcs.
 
   - The difference between the radii of two consecutive rows is a constant
     called the "row thickness" (radii is the plural of radius).
 
-  - The seat are circles (or disk) of equal radius. That radius divided by the
-    row thickness makes the "seat radius factor".
+  - The seat are circles (or disks) of equal radius. That radius divided by half
+    of the row thickness makes the "seat radius factor".
 
   - The center of a seat is on the arc of that seat's row.
   - In a given row, the distance between two neighboring seats is a constant.
   - The innermost row's arc is the inner arc.
   - The radius of the outermost row's arc is equal to the radius of the outer
     arc minus half of the row thickness, such that no seat may overlap the
     outer arc.
@@ -54,16 +54,16 @@
 ---------------
 
 As hinted above, there are several parameters that can be tweaked to change the
 layout of the hemicycle. Among them:
 
 - The span angle of the hemicycle can be set to a value lower than 180° (higher
   values are not supported). However, values so low as to prevent some row from
-  containing even ones seat are not supported, and may raise errors in future
-  versions.
+  containing even one seat are not supported, will yield incorrect results, and
+  may raise errors in future versions.
 - The number of rows can be set higher than the minimum required to hold the
   provided number of seats.
 - The seat radius factor can be changed between 0 and 1, with the seats touching
   their lateral neighbors when the factor is 1.
 - As long as the number of seats is not the maximum number the number of rows
   can hold, different strategies can be chosen to distribute the seats.
 
@@ -75,32 +75,39 @@
 ``SeatData``
 
 This class is defined and explained in the SVG submodule below, but it is
 exposed as part of the main module.
 
 ``write_svg_from_attribution(file, attrib, **kwargs)``
 
-This function writes an SVG file representing a hemicycle to the given file-like
-object. The parameters are as follows:
+This function writes an SVG file representing a hemicycle. The parameters are as
+follows:
 
-- ``file: io.TextIOBase``: a file-like object open in text mode.
+- ``file: str|io.TextIOBase``: a file-like object open in text mode, or the path
+  to the file to write on. If a path is provided, the file will be created if it
+  doesn't exist, and otherwise overwritten.
 - ``attrib: dict[SeatData, int]``: a mapping from a SeatData object applying to
   a number of seats in the resulting hemicycle, to the number of seats each
   object applies to. Typically, each SeatData object corresponds to a group or
   party. The ordering of the keys matter, and the elements will be arranged from
   left to right in the hemicycle.
 - ``**kwargs``: all optional keyword parameters taken by
   ``parliamentarch.geometry.get_seats_centers`` or by
   ``parliamentarch.svg.write_svg`` can be passed to this function.
 
-``get_svg_from_attribution(attrib, **kwargs)``
+``get_svg_from_attribution(attrib, **kwargs) -> str``
 
 Instead of writing it to a file, this function returns the SVG content as a
 string. The parameters are otherwise the same.
 
+Command-line interface
+----------------------
+
+See ``py -m parliamentarch -h`` for the accepted parameters.
+
 Geometry submodule contents
 ---------------------------
 
 These are found in the ``parliamentarch.geometry`` submodule.
 
 ``get_nrows_from_nseats(nseats: int, span_angle: float = 180.) -> int``
 
@@ -167,15 +174,15 @@
 arranged from left to right.
 
 SVG submodule content
 ---------------------
 
 These are found in the ``parliamentarch.svg`` submodule.
 
-``SeatData(data, color, border_size, border_color)``
+``SeatData(data, color, border_size=0, border_color="#000")``
 
 A class representing how to display a given seat or set of seats.
 
 - ``data: str``: metadata about the group of seats, which will end up in the
   SVG file. Typically the name of the party or of the member.
 - ``color: Color``: the color with which to fill the seat circles. This may take
   any number of formats: a "#RGB", "#RRGGBB", "#RGBA" or "#RRGGBBAA" string, a
@@ -183,18 +190,20 @@
   ints between 0 and 255. CSS color names are also supported.
 - ``border_size: float``: the size of the border around the seat circle. (to be
   documented at greater length)
 - ``border_color: Color``: the color of the border.
 
 ``write_svg(file, seat_centers, seat_actual_radius, *, canvas_size=175, margins=5., write_number_of_seats=True, font_size_factor=...)``
 
-This function writes an SVG file representing a hemicycle to the given file-like
-object. The parameters are as follows:
+This function writes an SVG file representing a hemicycle. The parameters are as
+follows:
 
-- ``file: io.TextIOBase``: a file-like object open in text mode.
+- ``file: str|io.TextIOBase``: a file-like object open in text mode, or the path
+  to the file to write on. If a path is provided, the file will be created if it
+  doesn't exist, and otherwise overwritten.
 - ``seat_centers: dict[tuple[float, float], SeatData]``: a mapping from the
   (x, y) coordinates of each seat's center to a SeatData object.
 - ``seat_actual_radius: float``: as output by ``get_seats_centers``.
 - ``canvas_size: float``: the height of the 2:1 rectangle in which the hemicycle
   will be drawn.
 - ``margins: float|tuple[float, float]|tuple[float, float, float, float]``:
   the margins around that rectangle. If four values are given, they are the
@@ -245,7 +254,8 @@
 - Allow SeatData to take some <a> element properties (like href), and if so use <a> instead of <g>
 - Allow SeatData to contain more creative SVG content like gradients
   - Maybe give it a .wrap method that wraps the circles in a g or a, and make it subclassable ?
   - Maybe just give a style method ?
 - Add tests
 - Add the option to force all rows to contain an even number of seats
 - Add a simpler way to input parameters in CLI
+  - Maybe by allowing the use of the standard input to pass JSON content ?
```

### Comparing `parliamentarch-0.2/src/ParliamentArch.egg-info/PKG-INFO` & `parliamentarch-1.0/src/ParliamentArch.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ParliamentArch
-Version: 0.2
+Version: 1.0
 Summary: Generation of arch-styled parliamentary arches
 Author: Gouvernathor
 License: BSD 3-Clause License
         
         Copyright (c) 2024, Gouvernathor
         
         Redistribution and use in source and binary forms, with or without
@@ -60,16 +60,16 @@
   top right corners of the rectangle are empty).
 - The seats will placed in rows, such that:
   - The rows are semicircular arcs concentric to the inner and outer arcs.
 
   - The difference between the radii of two consecutive rows is a constant
     called the "row thickness" (radii is the plural of radius).
 
-  - The seat are circles (or disk) of equal radius. That radius divided by the
-    row thickness makes the "seat radius factor".
+  - The seat are circles (or disks) of equal radius. That radius divided by half
+    of the row thickness makes the "seat radius factor".
 
   - The center of a seat is on the arc of that seat's row.
   - In a given row, the distance between two neighboring seats is a constant.
   - The innermost row's arc is the inner arc.
   - The radius of the outermost row's arc is equal to the radius of the outer
     arc minus half of the row thickness, such that no seat may overlap the
     outer arc.
@@ -93,16 +93,16 @@
 ---------------
 
 As hinted above, there are several parameters that can be tweaked to change the
 layout of the hemicycle. Among them:
 
 - The span angle of the hemicycle can be set to a value lower than 180° (higher
   values are not supported). However, values so low as to prevent some row from
-  containing even ones seat are not supported, and may raise errors in future
-  versions.
+  containing even one seat are not supported, will yield incorrect results, and
+  may raise errors in future versions.
 - The number of rows can be set higher than the minimum required to hold the
   provided number of seats.
 - The seat radius factor can be changed between 0 and 1, with the seats touching
   their lateral neighbors when the factor is 1.
 - As long as the number of seats is not the maximum number the number of rows
   can hold, different strategies can be chosen to distribute the seats.
 
@@ -114,32 +114,39 @@
 ``SeatData``
 
 This class is defined and explained in the SVG submodule below, but it is
 exposed as part of the main module.
 
 ``write_svg_from_attribution(file, attrib, **kwargs)``
 
-This function writes an SVG file representing a hemicycle to the given file-like
-object. The parameters are as follows:
+This function writes an SVG file representing a hemicycle. The parameters are as
+follows:
 
-- ``file: io.TextIOBase``: a file-like object open in text mode.
+- ``file: str|io.TextIOBase``: a file-like object open in text mode, or the path
+  to the file to write on. If a path is provided, the file will be created if it
+  doesn't exist, and otherwise overwritten.
 - ``attrib: dict[SeatData, int]``: a mapping from a SeatData object applying to
   a number of seats in the resulting hemicycle, to the number of seats each
   object applies to. Typically, each SeatData object corresponds to a group or
   party. The ordering of the keys matter, and the elements will be arranged from
   left to right in the hemicycle.
 - ``**kwargs``: all optional keyword parameters taken by
   ``parliamentarch.geometry.get_seats_centers`` or by
   ``parliamentarch.svg.write_svg`` can be passed to this function.
 
-``get_svg_from_attribution(attrib, **kwargs)``
+``get_svg_from_attribution(attrib, **kwargs) -> str``
 
 Instead of writing it to a file, this function returns the SVG content as a
 string. The parameters are otherwise the same.
 
+Command-line interface
+----------------------
+
+See ``py -m parliamentarch -h`` for the accepted parameters.
+
 Geometry submodule contents
 ---------------------------
 
 These are found in the ``parliamentarch.geometry`` submodule.
 
 ``get_nrows_from_nseats(nseats: int, span_angle: float = 180.) -> int``
 
@@ -206,15 +213,15 @@
 arranged from left to right.
 
 SVG submodule content
 ---------------------
 
 These are found in the ``parliamentarch.svg`` submodule.
 
-``SeatData(data, color, border_size, border_color)``
+``SeatData(data, color, border_size=0, border_color="#000")``
 
 A class representing how to display a given seat or set of seats.
 
 - ``data: str``: metadata about the group of seats, which will end up in the
   SVG file. Typically the name of the party or of the member.
 - ``color: Color``: the color with which to fill the seat circles. This may take
   any number of formats: a "#RGB", "#RRGGBB", "#RGBA" or "#RRGGBBAA" string, a
@@ -222,18 +229,20 @@
   ints between 0 and 255. CSS color names are also supported.
 - ``border_size: float``: the size of the border around the seat circle. (to be
   documented at greater length)
 - ``border_color: Color``: the color of the border.
 
 ``write_svg(file, seat_centers, seat_actual_radius, *, canvas_size=175, margins=5., write_number_of_seats=True, font_size_factor=...)``
 
-This function writes an SVG file representing a hemicycle to the given file-like
-object. The parameters are as follows:
+This function writes an SVG file representing a hemicycle. The parameters are as
+follows:
 
-- ``file: io.TextIOBase``: a file-like object open in text mode.
+- ``file: str|io.TextIOBase``: a file-like object open in text mode, or the path
+  to the file to write on. If a path is provided, the file will be created if it
+  doesn't exist, and otherwise overwritten.
 - ``seat_centers: dict[tuple[float, float], SeatData]``: a mapping from the
   (x, y) coordinates of each seat's center to a SeatData object.
 - ``seat_actual_radius: float``: as output by ``get_seats_centers``.
 - ``canvas_size: float``: the height of the 2:1 rectangle in which the hemicycle
   will be drawn.
 - ``margins: float|tuple[float, float]|tuple[float, float, float, float]``:
   the margins around that rectangle. If four values are given, they are the
@@ -284,7 +293,8 @@
 - Allow SeatData to take some <a> element properties (like href), and if so use <a> instead of <g>
 - Allow SeatData to contain more creative SVG content like gradients
   - Maybe give it a .wrap method that wraps the circles in a g or a, and make it subclassable ?
   - Maybe just give a style method ?
 - Add tests
 - Add the option to force all rows to contain an even number of seats
 - Add a simpler way to input parameters in CLI
+  - Maybe by allowing the use of the standard input to pass JSON content ?
```

### Comparing `parliamentarch-0.2/src/parliamentarch/__init__.py` & `parliamentarch-1.0/src/parliamentarch/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 from inspect import signature
 from io import TextIOBase
 
 from .geometry import get_seats_centers
-from .svg import SeatData, dispatch_seats, write_grouped_svg
-from ._util import filter_kwargs, get_from_write
+from .svg import SeatData, dispatch_seats, get_grouped_svg
+from ._util import filter_kwargs, write_from_get
 
 __all__ = ("get_svg_from_attribution", "write_svg_from_attribution", "SeatData")
 
 _GET_SEATS_CENTERS_PARAM_NAMES = {k for k, p in signature(get_seats_centers).parameters.items() if p.kind==p.KEYWORD_ONLY}
-_WRITE_GROUPED_SVG_PARAM_NAMES = {k for k, p in signature(write_grouped_svg).parameters.items() if p.kind==p.KEYWORD_ONLY}
+_WRITE_GROUPED_SVG_PARAM_NAMES = {k for k, p in signature(get_grouped_svg).parameters.items() if p.kind==p.KEYWORD_ONLY}
 
-def write_svg_from_attribution(file: TextIOBase, attrib: dict[SeatData, int], **kwargs) -> None:
+def get_svg_from_attribution(attrib: dict[SeatData, int], **kwargs) -> str:
     nseats = sum(attrib.values())
     get_seats_centers_kwargs, write_grouped_svg_kwargs, kwargs = filter_kwargs(_GET_SEATS_CENTERS_PARAM_NAMES, _WRITE_GROUPED_SVG_PARAM_NAMES, **kwargs)
 
     if kwargs:
         raise TypeError("Unknown parameters : " + ", ".join(kwargs))
 
     results = get_seats_centers(nseats, **get_seats_centers_kwargs)
     seat_centers_by_group = dispatch_seats(attrib, sorted(results, key=results.__getitem__, reverse=True))
-    write_grouped_svg(file, seat_centers_by_group, results.seat_actual_radius, **write_grouped_svg_kwargs)
+    return get_grouped_svg(seat_centers_by_group, results.seat_actual_radius, **write_grouped_svg_kwargs)
 
-get_svg_from_attribution = get_from_write(write_svg_from_attribution)
+write_svg_from_attribution = write_from_get(get_svg_from_attribution)
```

### Comparing `parliamentarch-0.2/src/parliamentarch/__main__.py` & `parliamentarch-1.0/src/parliamentarch/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,53 +12,55 @@
         prog="ParliamentArch",
         description="Generate arch-like parliament diagrams.",
     )
 
     # input filename (json)
     parser.add_argument("input",
         type=argparse.FileType("rb"),
-        help="""A readable JSON file containing the named parameters to use when
-        creating the diagram. The parameters are as the get_svg_from_attribution
-        function takes them, except that the "attrib" parameter should be a
-        sequence of dicts (JSON objects) with key/value pairs being parameters
-        to SeatData, and the optional nseats (defaulting to 1) being the number
-        of seats of that party.""",
+        help="""A readable JSON file containing one object whose members are the
+        named parameters to use when creating the diagram. The parameters are as
+        the get_svg_from_attribution function takes them, except for the
+        "attrib" parameter. It should instead be a sequence of JSON objects with
+        members being parameters to SeatData, and an optional "nseats" member
+        (defaulting to 1) being the number of seats for that party.""",
     )
     # each possible parameter separately ?
     # TODO do this programmatically using inspect
     # only require input if not all required are passed specifically
 
     # output filename
-    parser.add_argument("--output",
+    parser.add_argument("-o", "--output",
         type=argparse.FileType("w+"), # TODO check : write mode, clobber if exists, create if not
         help="""The file in which to write the SVG diagram. If not passed, the
         SVG code will be printed in the standard output.""",
         # TODO: make sure that this argument is optional and defaults to None
     )
-    # whether to print the resulting file's content (when the output file is not given)
+    # whether to print the resulting file's content (regardless of the output file being given)
     parser.add_argument("-p", "--print",
         action="store_true",
         help="""Pass this to print the SVG code in the standard output even when
         an output file is passed.""",
     )
     # if both are given, do both
-    # if none are given, only print
+    # if none are given, raise
 
 
     args = parser.parse_args()
 
+    if not (args.output or args.print):
+        parser.error("At least one of --output or --print must be passed.")
+
     with args.input as f:
         kwparams = json.load(f)
     kwparams["attrib"] = {SeatData(**d): n for d in kwparams["attrib"] if (n := d.pop("nseats", 1))}
 
     result = get_svg_from_attribution(**kwparams)
 
-    file_output = args.output is not None
-    if file_output:
+    if args.output is not None:
         with args.output as f:
             f.write(result)
-    if args.print or not file_output:
+    if args.print:
         print(result)
 
 
 if __name__ == "__main__":
     sys.exit(main())
```

### Comparing `parliamentarch-0.2/src/parliamentarch/geometry.py` & `parliamentarch-1.0/src/parliamentarch/geometry.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,14 +85,18 @@
     """
 
     OUTER_PRIORITY = enum.auto(), """
     Fills up the rows as much as possible, starting with the outermost ones.
     """
 
 class _SeatsCenterContainer(dict[tuple[float, float], float], UnPicklable):
+    """
+    Stores the coordinates of each seat as keys, the counterclockwise angle as values,
+    and other data as attributes.
+    """
     seat_radius_factor: float
     nrows: int
 
     @property
     def row_thickness(self):
         return _get_row_thickness(self.nrows)
     @property
```

### Comparing `parliamentarch-0.2/src/parliamentarch/svg.py` & `parliamentarch-1.0/src/parliamentarch/svg.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from collections.abc import Iterable
 from functools import cached_property
 from io import TextIOBase
 import re
+import warnings
 
-from ._util import Color, UnPicklable, get_from_write
+from ._util import Color, UnPicklable, write_from_get
 
 __all__ = ("SeatData", "dispatch_seats", "write_svg", "write_grouped_svg", "get_svg", "get_grouped_svg")
 
 class SeatData(UnPicklable):
     """Put this somewhere else"""
     id: int|None = None
     data: str
@@ -47,87 +48,92 @@
     to the number of seats each group has,
     and an iterable of seats in a given order,
     returns a dict associating each group to a list of seats.
     (Typically S is a tuple of x/y coordinates.)
     The length of the iterable should be the sum of the values in the dict.
     Typically the groups are ordered from the left to the right,
     and the seats are ordered from the left to the right.
+    If too few seats are passed, an exception is raised.
+    If too many seats are passed, a warning is emitted.
     """
     its = iter(seats)
     rv = {}
     for group, nseats in group_seats.items():
         rv[group] = [next(its) for _ in range(nseats)]
+    if tuple(its):
+        warnings.warn("Too many seats were passed to dispatch_seats.")
     return rv
 
 
-def write_svg(
-        file: TextIOBase,
+def get_svg(
         seat_centers: dict[tuple[float, float], SeatData],
         *args, **kwargs,
-        ) -> None:
+        ) -> str:
     seat_centers_by_group = {}
     for seat, group in seat_centers.items():
         seat_centers_by_group.setdefault(group, []).append(seat)
-    write_grouped_svg(file, seat_centers_by_group, *args, **kwargs)
+    return get_grouped_svg(seat_centers_by_group, *args, **kwargs)
 
-def write_grouped_svg(
-        file: TextIOBase,
+def get_grouped_svg(
         seat_centers_by_group: dict[SeatData, list[tuple[float, float]]],
         seat_actual_radius: float, *,
         canvas_size: float = 175,
         margins: float|tuple[float, float]|tuple[float, float, float, float] = 5.,
         write_number_of_seats: bool = True,
         font_size_factor: float = 36/175,
-        ) -> None:
+        ) -> str:
     """
     The margins is either a single value for all four sides,
     or a (horizontal, vertical) tuple,
     or a (left, top, right, bottom) tuple.
 
     canvas_size is the height and half of the width
     of the canvas 2:1 rectangle to which to add the margins.
     """
+    buffer = []
 
     if isinstance(margins, (int, float)):
         margins = (margins, margins, margins, margins)
     elif len(margins) == 2:
         margins = margins + margins
     left_margin, top_margin, right_margin, bottom_margin = margins
 
-    _write_svg_header(file,
+    _append_svg_header(buffer,
         width=left_margin+2*canvas_size+right_margin,
         height=top_margin+canvas_size+bottom_margin)
     if write_number_of_seats:
         font_size = round(font_size_factor * canvas_size)
-        _write_svg_number_of_seats(file, sum(map(len, seat_centers_by_group.values())),
-            x=left_margin+canvas_size, y=top_margin+canvas_size, font_size=font_size)
-    _write_grouped_svg_seats(file, seat_centers_by_group, seat_actual_radius,
+        _append_svg_number_of_seats(buffer, sum(map(len, seat_centers_by_group.values())),
+            x=left_margin+canvas_size, y=top_margin+(canvas_size*170/175), font_size=font_size)
+    _append_grouped_svg_seats(buffer, seat_centers_by_group, seat_actual_radius,
         canvas_size=canvas_size, left_margin=left_margin, top_margin=top_margin)
-    _write_svg_footer(file)
+    _append_svg_footer(buffer)
+
+    return "".join(buffer)
 
-def _write_svg_header(file: TextIOBase, width: float, height: float) -> None:
-    file.write(f"""\
+def _append_svg_header(buffer: list[str], width: float, height: float) -> None:
+    buffer.append(f"""\
 <?xml version="1.0" encoding="UTF-8" standalone="no"?>
 <svg xmlns:svg="http://www.w3.org/2000/svg"
      xmlns="http://www.w3.org/2000/svg" version="1.1"
      width="{width}" height="{height}">
     <!-- Created with parliamentarch (https://github.com/Gouvernathor/parliamentarch/) -->""")
 
-def _write_svg_number_of_seats(
-        file: TextIOBase,
+def _append_svg_number_of_seats(
+        buffer: list[str],
         nseats: int,
         x: float, y: float,
         font_size: int,
         ) -> None:
-    file.write(f"""
+    buffer.append(f"""
     <text x="{x}" y="{y}"
           style="font-size:{font_size}px;font-weight:bold;text-align:center;text-anchor:middle;font-family:sans-serif">{nseats}</text>""")
 
-def _write_grouped_svg_seats(
-        file: TextIOBase,
+def _append_grouped_svg_seats(
+        buffer: list[str],
         seat_centers_by_group: dict[SeatData, list[tuple[float, float]]],
         seat_actual_radius: float,
         canvas_size: float,
         left_margin: float,
         top_margin: float,
         ) -> None:
 
@@ -145,30 +151,30 @@
         group_color = group.color
         if isinstance(group_color, Color):
             group_color = group_color.hexcode
         group_border_color = group.border_color
         if isinstance(group_border_color, Color):
             group_border_color = group_border_color.hexcode
 
-        file.write(f"""
+        buffer.append(f"""
     <g style="fill:{group_color}; stroke-width:{group_border_width:.2f}; stroke:{group_border_color}"
        id="{block_id}">
         <title>{group.data}</title>""")
 
         for x, y in seat_centers:
             actual_x = left_margin + canvas_size * x
             actual_y = top_margin + canvas_size * (1 - y)
             actual_radius = seat_actual_radius * canvas_size - group_border_width/2
-            file.write(f"""
+            buffer.append(f"""
         <circle cx="{actual_x:.2f}" cy="{actual_y:.2f}" r="{actual_radius:.2f}"/>""")
 
-        file.write("""
+        buffer.append("""
     </g>""")
 
-def _write_svg_footer(file: TextIOBase) -> None:
-    file.write("""
+def _append_svg_footer(buffer: list[str]) -> None:
+    buffer.append("""
 </svg>
 """)
 
 
-get_svg = get_from_write(write_svg)
-get_grouped_svg = get_from_write(write_grouped_svg)
+write_svg = write_from_get(get_svg)
+write_grouped_svg = write_from_get(get_grouped_svg)
```

