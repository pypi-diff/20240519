# Comparing `tmp/image2gcode-2.9.8.tar.gz` & `tmp/image2gcode-2.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "image2gcode-2.9.8.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "image2gcode-2.9.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `image2gcode-2.9.8.tar` & `image2gcode-2.9.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1085 2023-09-11 14:46:10.617779 image2gcode-2.9.8/LICENSE
--rw-r--r--   0        0        0    11919 2024-01-08 18:58:00.075902 image2gcode-2.9.8/README.md
--rw-r--r--   0        0        0       70 2024-01-08 19:03:51.602610 image2gcode-2.9.8/image2gcode/__init__.py
--rw-r--r--   0        0        0    10063 2024-01-08 19:04:13.873033 image2gcode-2.9.8/image2gcode/__main__.py
--rw-r--r--   0        0        0     3250 2024-01-08 19:05:03.763980 image2gcode-2.9.8/image2gcode/boundingbox.py
--rw-r--r--   0        0        0    13069 2024-01-08 19:05:36.884608 image2gcode-2.9.8/image2gcode/image2gcode.py
--rw-r--r--   0        0        0    14270 2023-09-20 13:06:13.800653 image2gcode-2.9.8/image2gcode/imagegen.py
--rw-r--r--   0        0        0    13043 2023-12-02 13:37:41.739883 image2gcode-2.9.8/image2gcode/newimage2gcode.py
--rw-r--r--   0        0        0      711 2023-12-02 14:55:05.587169 image2gcode-2.9.8/pyproject.toml
--rw-r--r--   0        0        0    12468 1970-01-01 00:00:00.000000 image2gcode-2.9.8/PKG-INFO
+-rw-r--r--   0        0        0     1085 2023-09-11 14:46:10.617779 image2gcode-2.9.9/LICENSE
+-rw-r--r--   0        0        0    11922 2024-02-17 16:13:15.918873 image2gcode-2.9.9/README.md
+-rw-r--r--   0        0        0       70 2024-02-17 16:12:49.288226 image2gcode-2.9.9/image2gcode/__init__.py
+-rw-r--r--   0        0        0    10063 2024-01-08 19:04:13.873033 image2gcode-2.9.9/image2gcode/__main__.py
+-rw-r--r--   0        0        0     3250 2024-01-08 19:05:03.763980 image2gcode-2.9.9/image2gcode/boundingbox.py
+-rw-r--r--   0        0        0    13069 2024-01-08 19:05:36.884608 image2gcode-2.9.9/image2gcode/image2gcode.py
+-rw-r--r--   0        0        0    14270 2023-09-20 13:06:13.800653 image2gcode-2.9.9/image2gcode/imagegen.py
+-rw-r--r--   0        0        0    13043 2023-12-02 13:37:41.739883 image2gcode-2.9.9/image2gcode/newimage2gcode.py
+-rw-r--r--   0        0        0      711 2023-12-02 14:55:05.587169 image2gcode-2.9.9/pyproject.toml
+-rw-r--r--   0        0        0    12471 1970-01-01 00:00:00.000000 image2gcode-2.9.9/PKG-INFO
```

### Comparing `image2gcode-2.9.8/LICENSE` & `image2gcode-2.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `image2gcode-2.9.8/README.md` & `image2gcode-2.9.9/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 For example if your machines laser width is 0.08mm I would recomment using a pixel size of 0.1mm; an engraving of 50x65 mm^2 (*width*x*height*) will need the source image resolution to be 500x650 pixels (*width*x*height*) in this case.
 It is also possible to set the DPI of an image to be exported from Inkscape (for example) and so get the right resolution for your laser machine. In this case the image to be exported should have a DPI setting of 254 (one inch is 25.4mm/0.1 = 254), note the image size when you do the export, because that will be exacly what you get on the laser machine!
 
 If this is too cumbersome, use option --size (release 2.5.0 or above), also for conveniance, to get the origin at the center, set --center. Note that --size will make a conversion of the source image.
 
 Some people noticed incorrect low burn levels at the edges of objects within an image, this can be remedied by using option '--overscan <nbr of pixels>'. This makes sure the laser head will continue for a few pixels on a line after the last non empty pixel, or start the head a few pixels before the first non empty pixel is written on a line.
 
-It is possible to calibrate your laser machine now: option ```--genimages pixel-width pixel-height write``` generates a set calibration files that can be used as input for ```image2gcode``` to experiment with settings like ```--pixelsize```, ```--speed and ```--maxpower``` to get the right setup! For example use ```image2gcode --showimage --genimages 200 200 0``` to generate test images of 200 by 200 pixels that show up in the viewer (but are not written to the file system). See chapter *calibrate* below.
+It is possible to calibrate your laser machine now: option ```--genimages pixel-width pixel-height write``` generates a set calibration files that can be used as input for ```image2gcode``` to experiment with settings like ```--pixelsize```, ```--speed``` and ```--maxpower``` to get the right setup! For example use ```image2gcode --showimage --genimages 200 200 0``` to generate test images of 200 by 200 pixels that show up in the viewer (but are not written to the file system). See chapter *calibrate* below.
 
 Please consider supporting me, so I can make this application better and add new functionality to it: <http://paypal.me/johannesnoordanus/5,00>
 
 To summarize:
 
 Optimized gcode
 - draw pixels in one go until change of power
```

### Comparing `image2gcode-2.9.8/image2gcode/__main__.py` & `image2gcode-2.9.9/image2gcode/__main__.py`

 * *Files identical despite different names*

### Comparing `image2gcode-2.9.8/image2gcode/boundingbox.py` & `image2gcode-2.9.9/image2gcode/boundingbox.py`

 * *Files identical despite different names*

### Comparing `image2gcode-2.9.8/image2gcode/image2gcode.py` & `image2gcode-2.9.9/image2gcode/image2gcode.py`

 * *Files identical despite different names*

### Comparing `image2gcode-2.9.8/image2gcode/imagegen.py` & `image2gcode-2.9.9/image2gcode/imagegen.py`

 * *Files identical despite different names*

### Comparing `image2gcode-2.9.8/image2gcode/newimage2gcode.py` & `image2gcode-2.9.9/image2gcode/newimage2gcode.py`

 * *Files identical despite different names*

### Comparing `image2gcode-2.9.8/pyproject.toml` & `image2gcode-2.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `image2gcode-2.9.8/PKG-INFO` & `image2gcode-2.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: image2gcode
-Version: 2.9.8
+Version: 2.9.9
 Summary: image2gcode: convert an image to gcode.
 Keywords: engraving,laser,image,laser engraving,PWM,gcode
 Author-email: Johannes Noordanus <mailjohannes.mailnoordanus@gmail.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Requires-Dist: gcode2image >= 2.3.1
@@ -31,15 +31,15 @@
 For example if your machines laser width is 0.08mm I would recomment using a pixel size of 0.1mm; an engraving of 50x65 mm^2 (*width*x*height*) will need the source image resolution to be 500x650 pixels (*width*x*height*) in this case.
 It is also possible to set the DPI of an image to be exported from Inkscape (for example) and so get the right resolution for your laser machine. In this case the image to be exported should have a DPI setting of 254 (one inch is 25.4mm/0.1 = 254), note the image size when you do the export, because that will be exacly what you get on the laser machine!
 
 If this is too cumbersome, use option --size (release 2.5.0 or above), also for conveniance, to get the origin at the center, set --center. Note that --size will make a conversion of the source image.
 
 Some people noticed incorrect low burn levels at the edges of objects within an image, this can be remedied by using option '--overscan <nbr of pixels>'. This makes sure the laser head will continue for a few pixels on a line after the last non empty pixel, or start the head a few pixels before the first non empty pixel is written on a line.
 
-It is possible to calibrate your laser machine now: option ```--genimages pixel-width pixel-height write``` generates a set calibration files that can be used as input for ```image2gcode``` to experiment with settings like ```--pixelsize```, ```--speed and ```--maxpower``` to get the right setup! For example use ```image2gcode --showimage --genimages 200 200 0``` to generate test images of 200 by 200 pixels that show up in the viewer (but are not written to the file system). See chapter *calibrate* below.
+It is possible to calibrate your laser machine now: option ```--genimages pixel-width pixel-height write``` generates a set calibration files that can be used as input for ```image2gcode``` to experiment with settings like ```--pixelsize```, ```--speed``` and ```--maxpower``` to get the right setup! For example use ```image2gcode --showimage --genimages 200 200 0``` to generate test images of 200 by 200 pixels that show up in the viewer (but are not written to the file system). See chapter *calibrate* below.
 
 Please consider supporting me, so I can make this application better and add new functionality to it: <http://paypal.me/johannesnoordanus/5,00>
 
 To summarize:
 
 Optimized gcode
 - draw pixels in one go until change of power
```

