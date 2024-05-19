# Comparing `tmp/patched_yolo_infer-1.1.2.tar.gz` & `tmp/patched_yolo_infer-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patched_yolo_infer-1.1.2.tar", last modified: Fri Mar 29 08:34:55 2024, max compression
+gzip compressed data, was "patched_yolo_infer-1.1.3.tar", last modified: Sun May 19 17:44:33 2024, max compression
```

## Comparing `patched_yolo_infer-1.1.2.tar` & `patched_yolo_infer-1.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-03-29 08:34:55.884494 patched_yolo_infer-1.1.2/
--rw-rw-rw-   0        0        0    35184 2024-03-29 07:50:02.000000 patched_yolo_infer-1.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0    10207 2024-03-29 08:34:55.884494 patched_yolo_infer-1.1.2/PKG-INFO
--rw-rw-rw-   0        0        0    10542 2024-03-29 08:09:41.000000 patched_yolo_infer-1.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-03-29 08:34:55.856797 patched_yolo_infer-1.1.2/patched_yolo_infer/
--rw-rw-rw-   0        0        0      262 2024-03-14 20:52:00.000000 patched_yolo_infer-1.1.2/patched_yolo_infer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 08:34:55.879444 patched_yolo_infer-1.1.2/patched_yolo_infer/elements/
--rw-rw-rw-   0        0        0     5431 2024-03-20 21:30:32.000000 patched_yolo_infer-1.1.2/patched_yolo_infer/elements/CropElement.py
--rw-rw-rw-   0        0        0        0 2024-03-14 21:13:30.000000 patched_yolo_infer-1.1.2/patched_yolo_infer/elements/__init__.py
--rw-rw-rw-   0        0        0    15961 2024-03-21 08:29:19.000000 patched_yolo_infer-1.1.2/patched_yolo_infer/functions_extra.py
-drwxrwxrwx   0        0        0        0 2024-03-29 08:34:55.879444 patched_yolo_infer-1.1.2/patched_yolo_infer/nodes/
--rw-rw-rw-   0        0        0    12807 2024-03-29 08:17:13.000000 patched_yolo_infer-1.1.2/patched_yolo_infer/nodes/CombineDetections.py
--rw-rw-rw-   0        0        0     8337 2024-03-17 20:48:48.000000 patched_yolo_infer-1.1.2/patched_yolo_infer/nodes/MakeCropsDetectThem.py
--rw-rw-rw-   0        0        0        0 2024-03-14 21:13:13.000000 patched_yolo_infer-1.1.2/patched_yolo_infer/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-29 08:34:55.879444 patched_yolo_infer-1.1.2/patched_yolo_infer.egg-info/
--rw-rw-rw-   0        0        0    10207 2024-03-29 08:34:55.000000 patched_yolo_infer-1.1.2/patched_yolo_infer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2024-03-29 08:34:55.000000 patched_yolo_infer-1.1.2/patched_yolo_infer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-29 08:34:55.000000 patched_yolo_infer-1.1.2/patched_yolo_infer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-03-29 08:34:55.000000 patched_yolo_infer-1.1.2/patched_yolo_infer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-03-29 08:34:55.000000 patched_yolo_infer-1.1.2/patched_yolo_infer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-03-29 08:34:55.885611 patched_yolo_infer-1.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1695 2024-03-29 08:33:07.000000 patched_yolo_infer-1.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:44:33.910807 patched_yolo_infer-1.1.3/
+-rw-rw-rw-   0        0        0    35184 2024-03-29 07:50:02.000000 patched_yolo_infer-1.1.3/LICENSE.txt
+-rw-rw-rw-   0        0        0    12908 2024-05-19 17:44:33.910807 patched_yolo_infer-1.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0    13286 2024-05-19 17:40:50.000000 patched_yolo_infer-1.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 17:44:33.893389 patched_yolo_infer-1.1.3/patched_yolo_infer/
+-rw-rw-rw-   0        0        0      262 2024-03-14 20:52:00.000000 patched_yolo_infer-1.1.3/patched_yolo_infer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:44:33.902874 patched_yolo_infer-1.1.3/patched_yolo_infer/elements/
+-rw-rw-rw-   0        0        0     6841 2024-05-19 16:18:07.000000 patched_yolo_infer-1.1.3/patched_yolo_infer/elements/CropElement.py
+-rw-rw-rw-   0        0        0        0 2024-03-14 21:13:30.000000 patched_yolo_infer-1.1.3/patched_yolo_infer/elements/__init__.py
+-rw-rw-rw-   0        0        0    16850 2024-05-19 14:49:58.000000 patched_yolo_infer-1.1.3/patched_yolo_infer/functions_extra.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:44:33.909833 patched_yolo_infer-1.1.3/patched_yolo_infer/nodes/
+-rw-rw-rw-   0        0        0    13486 2024-05-19 07:54:44.000000 patched_yolo_infer-1.1.3/patched_yolo_infer/nodes/CombineDetections.py
+-rw-rw-rw-   0        0        0     8716 2024-05-19 16:09:46.000000 patched_yolo_infer-1.1.3/patched_yolo_infer/nodes/MakeCropsDetectThem.py
+-rw-rw-rw-   0        0        0        0 2024-03-14 21:13:13.000000 patched_yolo_infer-1.1.3/patched_yolo_infer/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:44:33.902874 patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/
+-rw-rw-rw-   0        0        0    12908 2024-05-19 17:44:33.000000 patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2024-05-19 17:44:33.000000 patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 17:44:33.000000 patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-19 17:44:33.000000 patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-19 17:44:33.000000 patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 17:44:33.912316 patched_yolo_infer-1.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1695 2024-05-19 17:43:52.000000 patched_yolo_infer-1.1.3/setup.py
```

### Comparing `patched_yolo_infer-1.1.2/LICENSE.txt` & `patched_yolo_infer-1.1.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `patched_yolo_infer-1.1.2/PKG-INFO` & `patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: patched_yolo_infer
-Version: 1.1.2
+Name: patched-yolo-infer
+Version: 1.1.3
 Summary: YOLO-Patch-Based-Inference for detection/segmentation of small objects in images.
 Home-page: https://github.com/Koldim2001/YOLO-Patch-Based-Inference
 Author: Koldim2001
 License: AGPL-3.0 license
 Keywords: python,yolov8,yolov9,rtdetr,sam,object detection,instance segmentation,patch-based inference,small object detection,yolov8-seg,image patching,yolo visualization,slice-based inference,slicing inference,inference visualization,patchify,ultralytics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -46,28 +46,29 @@
 
 __Check this Colab examples:__
                          
 YOLO-Patch-Based-Inference Example - [Open in Colab](https://colab.research.google.com/drive/1FUao91GyB-ojGRN_okUxYyfagTT9tdsP?usp=sharing)
 
 Example of using various functions for visualizing basic YOLOv8/v9 inference results and handling overlapping crops - [Open in Colab](https://colab.research.google.com/drive/1eM4o1e0AUQrS1mLDpcgK9HKInWEvnaMn?usp=sharing)
 
+
 ## Usage
 
 ### 1. Patch-Based-Inference
-To carry out patch-based inference of YOLO models using our library, you need to follow a sequential procedure. First, you create an instance of the MakeCropsDetectThem class, providing all desired parameters related to YOLO inference and the patch segmentation principle.<br/> Subsequently, you pass the obtained object of this class to CombineDetections, which facilitates the consolidation of all predictions from each overlapping crop, followed by intelligent suppression of duplicates. <br/>Upon completion, you receive the result, from which you can extract the desired outcome of frame processing.
+To carry out patch-based inference of YOLO models using our library, you need to follow a sequential procedure. First, you create an instance of the `MakeCropsDetectThem` class, providing all desired parameters related to YOLO inference and the patch segmentation principle.<br/> Subsequently, you pass the obtained object of this class to `CombineDetections`, which facilitates the consolidation of all predictions from each overlapping crop, followed by intelligent suppression of duplicates. <br/>Upon completion, you receive the result, from which you can extract the desired outcome of frame processing.
 
 The output obtained from the process includes several attributes that can be leveraged for further analysis or visualization:
 
 1. img: This attribute contains the original image on which the inference was performed. It provides context for the detected objects.
 
 2. confidences: This attribute holds the confidence scores associated with each detected object. These scores indicate the model's confidence level in the accuracy of its predictions.
 
 3. boxes: These bounding boxes are represented as a list of lists, where each list contains four values: [x_min, y_min, x_max, y_max]. These values correspond to the coordinates of the top-left and bottom-right corners of each bounding box.
 
-4. masks: If available, this attribute provides segmentation masks corresponding to the detected objects. These masks can be used to precisely delineate object boundaries.
+4. polygons: If available, this attribute provides a list containing NumPy arrays of polygon coordinates that represent segmentation masks corresponding to the detected objects. These polygons can be utilized to accurately outline the boundaries of each object.
 
 5. classes_ids: This attribute contains the class IDs assigned to each detected object. These IDs correspond to specific object classes defined during the model training phase.
 
 6. classes_names: These are the human-readable names corresponding to the class IDs. They provide semantic labels for the detected objects, making the results easier to interpret.
 
 ```python
 import cv2
@@ -91,15 +92,15 @@
 )
 result = CombineDetections(element_crops, nms_threshold=0.25, match_metric='IOS')  
 
 # Final Results:
 img=result.image
 confidences=result.filtered_confidences
 boxes=result.filtered_boxes
-masks=result.filtered_masks
+polygons=result.filtered_polygons
 classes_ids=result.filtered_classes_id
 classes_names=result.filtered_classes_names
 ```
 
 #### Explanation of possible input arguments:
 
 **MakeCropsDetectThem**
@@ -115,33 +116,38 @@
 - **segment** (*bool*): Whether to perform segmentation (YOLOv8-seg).
 - **shape_x** (*int*): Size of the crop in the x-coordinate.
 - **shape_y** (*int*): Size of the crop in the y-coordinate.
 - **overlap_x** (*float*): Percentage of overlap along the x-axis.
 - **overlap_y** (*float*): Percentage of overlap along the y-axis.
 - **show_crops** (*bool*): Whether to visualize the cropping.
 - **resize_initial_size** (*bool*): Whether to resize the results to the original image size (ps: slow operation).
+- **memory_optimize** (*bool*): Memory optimization option for segmentation (less accurate results when enabled).
 
 **CombineDetections**
 Class implementing combining masks/boxes from multiple crops + NMS (Non-Maximum Suppression).\
 **Args:**
 - **element_crops** (*MakeCropsDetectThem*): Object containing crop information.
 - **nms_threshold** (*float*): IoU/IoS threshold for non-maximum suppression.
 - **match_metric** (*str*): Matching metric, either 'IOU' or 'IOS'.
-- **intelligent_sorter** (*bool*): Enable sorting by area and rounded confidence parameter. If False, sorting will be done only by confidence (usual nms). (Dafault is True)
+- **intelligent_sorter** (*bool*): Enable sorting by area and rounded confidence parameter. 
+            If False, sorting will be done only by confidence (usual nms). (Dafault is True)
+
+
 
 ---
 ### 2. Custom inference visualization:
 Visualizes custom results of object detection or segmentation on an image.
 
 **Args:**
 - **img** (*numpy.ndarray*): The input image in BGR format.
 - **boxes** (*list*): A list of bounding boxes in the format [x_min, y_min, x_max, y_max].
 - **classes_ids** (*list*): A list of class IDs for each detection.
 - **confidences** (*list*): A list of confidence scores corresponding to each bounding box. Default is an empty list.
 - **classes_names** (*list*): A list of class names corresponding to the class IDs. Default is an empty list.
+- **polygons** (*list*): A list containing NumPy arrays of polygon coordinates that represent segmentation masks.
 - **masks** (*list*): A list of masks. Default is an empty list.
 - **segment** (*bool*): Whether to perform instance segmentation. Default is False.
 - **show_boxes** (*bool*): Whether to show bounding boxes. Default is True.
 - **show_class** (*bool*): Whether to show class labels. Default is True.
 - **fill_mask** (*bool*): Whether to fill the segmented regions with color. Default is False.
 - **alpha** (*float*): The transparency of filled masks. Default is 0.3.
 - **color_class_background** (*tuple*): The background BGR color for class labels. Default is (0, 0, 255) (red).
@@ -151,28 +157,61 @@
 - **font_scale** (*float*): The scale factor for font size. Default is 1.5.
 - **delta_colors** (*int*): The random seed offset for color variation. Default is seed=0.
 - **dpi** (*int*): Final visualization size (plot is bigger when dpi is higher). Default is 150.
 - **random_object_colors** (*bool*): If true, colors for each object are selected randomly. Default is False.
 - **show_confidences** (*bool*): If true and show_class=True, confidences near class are visualized. Default is False.
 - **axis_off** (*bool*): If true, axis is turned off in the final visualization. Default is True.
 - **show_classes_list** (*list*): If empty, visualize all classes. Otherwise, visualize only classes in the list.
-- **return_image_array** (*bool*): If True, the function returns the image (BGR np.array) instead of displaying it. Default is False.
+- **return_image_array** (*bool*): If True, the function returns the image (BGR np.array) instead of displaying it. 
+                                   Default is False.
 
 
 Example of using:
 ```python
 from patched_yolo_infer import visualize_results
 
 # Assuming result is an instance of the CombineDetections class
 result = CombineDetections(...) 
 
 # Visualizing the results using the visualize_results function
 visualize_results(
     img=result.image,
     confidences=result.filtered_confidences,
     boxes=result.filtered_boxes,
-    masks=result.filtered_masks,
+    polygons=result.filtered_polygons,
     classes_ids=result.filtered_classes_id,
     classes_names=result.filtered_classes_names,
     segment=False,
 )
+```
+
+---
+
+## __HOW TO IMPROVE THE QUALITY OF THE ALGORITHM FOR THE TASK OF INSTANCE SEGMENTATION:__
+
+In this approach, all operations under the hood are performed on binary masks of recognized objects. Storing these masks consumes a lot of memory, so this method requires more RAM and slightly more processing time. However, the accuracy of recognition significantly improves, which is especially noticeable in cases where there are many objects of different sizes and they are densely packed. Therefore, we recommend using this approach in production if accuracy is important and not speed, and if your computational resources allow storing hundreds of binary masks in RAM.
+
+The difference in the approach to using the function lies in specifying the parameter ```memory_optimize=False``` in the ```MakeCropsDetectThem``` class.
+In such a case, the informative values after processing will be the following:
+
+1. img: This attribute contains the original image on which the inference was performed. It provides context for the detected objects.
+
+2. confidences: This attribute holds the confidence scores associated with each detected object. These scores indicate the model's confidence level in the accuracy of its predictions.
+
+3. boxes: These bounding boxes are represented as a list of lists, where each list contains four values: [x_min, y_min, x_max, y_max]. These values correspond to the coordinates of the top-left and bottom-right corners of each bounding box.
+
+4. masks: This attribute provides segmentation binary masks corresponding to the detected objects. These masks can be used to precisely delineate object boundaries.
+
+5. classes_ids: This attribute contains the class IDs assigned to each detected object. These IDs correspond to specific object classes defined during the model training phase.
+
+6. classes_names: These are the human-readable names corresponding to the class IDs. They provide semantic labels for the detected objects, making the results easier to interpret.
+
+
+Here's how you can obtain them:
+```python
+img=result.image
+confidences=result.filtered_confidences
+boxes=result.filtered_boxes
+masks=result.filtered_masks
+classes_ids=result.filtered_classes_id
+classes_names=result.filtered_classes_names
 ```
```

### Comparing `patched_yolo_infer-1.1.2/README.md` & `patched_yolo_infer-1.1.3/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -23,637 +23,809 @@
 00000160: 0d0a 2a2a 4d6f 6465 6c20 5375 7070 6f72  ..**Model Suppor
 00000170: 742a 2a3a 2054 6865 206c 6962 7261 7279  t**: The library
 00000180: 206f 6666 6572 7320 7375 7070 6f72 7420   offers support 
 00000190: 666f 7220 6d75 6c74 6970 6c65 2075 6c74  for multiple ult
 000001a0: 7261 6c79 7469 6373 2064 6565 7020 6c65  ralytics deep le
 000001b0: 6172 6e69 6e67 206d 6f64 656c 732c 2073  arning models, s
 000001c0: 7563 6820 6173 2059 4f4c 4f76 382c 2059  uch as YOLOv8, Y
-000001d0: 4f4c 4f76 392c 2053 414d 2c20 616e 6420  OLOv9, SAM, and 
-000001e0: 5254 4445 5452 2e20 5573 6572 7320 6361  RTDETR. Users ca
-000001f0: 6e20 7365 6c65 6374 2066 726f 6d20 7072  n select from pr
-00000200: 652d 7472 6169 6e65 6420 6f70 7469 6f6e  e-trained option
-00000210: 7320 6f72 2075 7469 6c69 7a65 2063 7573  s or utilize cus
-00000220: 746f 6d2d 7472 6169 6e65 6420 6d6f 6465  tom-trained mode
-00000230: 6c73 2074 6f20 6265 7374 206d 6565 7420  ls to best meet 
-00000240: 7468 6569 7220 7461 736b 2072 6571 7569  their task requi
-00000250: 7265 6d65 6e74 732e 0d0a 0d0a 2323 2049  rements.....## I
-00000260: 6e73 7461 6c6c 6174 696f 6e0d 0a59 6f75  nstallation..You
-00000270: 2063 616e 2069 6e73 7461 6c6c 2074 6865   can install the
-00000280: 206c 6962 7261 7279 2076 6961 2070 6970   library via pip
-00000290: 3a0d 0a0d 0a60 6060 6261 7368 0d0a 7069  :....```bash..pi
-000002a0: 7020 696e 7374 616c 6c20 7061 7463 6865  p install patche
-000002b0: 645f 796f 6c6f 5f69 6e66 6572 0d0a 6060  d_yolo_infer..``
-000002c0: 600d 0a0d 0a5b 215b 5079 5049 2056 6572  `....[![PyPI Ver
-000002d0: 7369 6f6e 5d28 6874 7470 733a 2f2f 696d  sion](https://im
-000002e0: 672e 7368 6965 6c64 732e 696f 2f70 7970  g.shields.io/pyp
-000002f0: 692f 762f 7061 7463 6865 642d 796f 6c6f  i/v/patched-yolo
-00000300: 2d69 6e66 6572 2e73 7667 295d 2868 7474  -infer.svg)](htt
-00000310: 7073 3a2f 2f70 7970 692e 6f72 672f 7072  ps://pypi.org/pr
-00000320: 6f6a 6563 742f 7061 7463 6865 642d 796f  oject/patched-yo
-00000330: 6c6f 2d69 6e66 6572 2f29 202d 2043 6c69  lo-infer/) - Cli
-00000340: 636b 2068 6572 6520 746f 2076 6973 6974  ck here to visit
-00000350: 2074 6865 2050 7950 4920 7061 6765 2066   the PyPI page f
-00000360: 6f72 2060 7061 7463 6865 642d 796f 6c6f  or `patched-yolo
-00000370: 2d69 6e66 6572 602c 2077 6865 7265 2079  -infer`, where y
-00000380: 6f75 2063 616e 2066 696e 6420 6d6f 7265  ou can find more
-00000390: 2069 6e66 6f72 6d61 7469 6f6e 2061 6e64   information and
-000003a0: 2064 6f63 756d 656e 7461 7469 6f6e 2e0d   documentation..
-000003b0: 0a0d 0a4e 6f74 653a 2049 6620 4355 4441  ...Note: If CUDA
-000003c0: 2073 7570 706f 7274 2069 7320 6176 6169   support is avai
-000003d0: 6c61 626c 652c 2069 7427 7320 7265 636f  lable, it's reco
-000003e0: 6d6d 656e 6465 6420 746f 2070 7265 2d69  mmended to pre-i
-000003f0: 6e73 7461 6c6c 2050 7954 6f72 6368 2077  nstall PyTorch w
-00000400: 6974 6820 4355 4441 2073 7570 706f 7274  ith CUDA support
-00000410: 2062 6566 6f72 6520 696e 7374 616c 6c69   before installi
-00000420: 6e67 2074 6865 206c 6962 7261 7279 2e20  ng the library. 
-00000430: 4f74 6865 7277 6973 652c 2074 6865 2043  Otherwise, the C
-00000440: 5055 2076 6572 7369 6f6e 2077 696c 6c20  PU version will 
-00000450: 6265 2069 6e73 7461 6c6c 6564 2062 7920  be installed by 
-00000460: 6465 6661 756c 742e 0d0a 0d0a 2d2d 2d0d  default.....---.
-00000470: 0a0d 0a3c 2f64 6574 6169 6c73 3e0d 0a0d  ...</details>...
-00000480: 0a23 2320 4e6f 7465 626f 6f6b 730d 0a0d  .## Notebooks...
-00000490: 0a49 6e74 6572 6163 7469 7665 206e 6f74  .Interactive not
-000004a0: 6562 6f6f 6b73 2061 7265 2070 726f 7669  ebooks are provi
-000004b0: 6465 6420 746f 2073 686f 7763 6173 6520  ded to showcase 
-000004c0: 7468 6520 6675 6e63 7469 6f6e 616c 6974  the functionalit
-000004d0: 7920 6f66 2074 6865 206c 6962 7261 7279  y of the library
-000004e0: 2e20 5468 6573 6520 6e6f 7465 626f 6f6b  . These notebook
-000004f0: 7320 636f 7665 7220 6261 7463 682d 696e  s cover batch-in
-00000500: 6665 7265 6e63 6520 7072 6f63 6564 7572  ference procedur
-00000510: 6573 2066 6f72 2064 6574 6563 7469 6f6e  es for detection
-00000520: 2c20 696e 7374 616e 6365 2073 6567 6d65  , instance segme
-00000530: 6e74 6174 696f 6e2c 2069 6e66 6572 656e  ntation, inferen
-00000540: 6365 2063 7573 746f 6d20 7669 7375 616c  ce custom visual
-00000550: 697a 6174 696f 6e2c 2061 6e64 206d 6f72  ization, and mor
-00000560: 652e 2045 6163 6820 6e6f 7465 626f 6f6b  e. Each notebook
-00000570: 2069 7320 7061 6972 6564 2077 6974 6820   is paired with 
-00000580: 6120 7475 746f 7269 616c 206f 6e20 596f  a tutorial on Yo
-00000590: 7554 7562 652c 206d 616b 696e 6720 6974  uTube, making it
-000005a0: 2065 6173 7920 746f 206c 6561 726e 2061   easy to learn a
-000005b0: 6e64 2069 6d70 6c65 6d65 6e74 2066 6561  nd implement fea
-000005c0: 7475 7265 732e 0d0a 0d0a 0d0a 7c20 2a2a  tures.......| **
-000005d0: 546f 7069 632a 2a20 7c20 2a2a 4e6f 7465  Topic** | **Note
-000005e0: 626f 6f6b 2a2a 207c 202a 2a59 6f75 5475  book** | **YouTu
-000005f0: 6265 2a2a 207c 0d0a 7c20 2d2d 2d2d 2d20  be** |..| ----- 
-00000600: 7c20 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d  | -------- | ---
-00000610: 2d2d 2d2d 207c 0d0a 7c20 5b50 6174 6368  ---- |..| [Patch
-00000620: 2d42 6173 6564 2d49 6e66 6572 656e 6365  -Based-Inference
-00000630: 2045 7861 6d70 6c65 5d28 6874 7470 733a   Example](https:
-00000640: 2f2f 6e62 7669 6577 6572 2e6f 7267 2f67  //nbviewer.org/g
-00000650: 6974 6875 622f 4b6f 6c64 696d 3230 3031  ithub/Koldim2001
-00000660: 2f59 4f4c 4f2d 5061 7463 682d 4261 7365  /YOLO-Patch-Base
-00000670: 642d 496e 6665 7265 6e63 652f 626c 6f62  d-Inference/blob
-00000680: 2f6d 6169 6e2f 6578 616d 706c 6573 2f65  /main/examples/e
-00000690: 7861 6d70 6c65 5f70 6174 6368 5f62 6173  xample_patch_bas
-000006a0: 6564 5f69 6e66 6572 656e 6365 2e69 7079  ed_inference.ipy
-000006b0: 6e62 2920 7c20 5b21 5b4f 7065 6e20 496e  nb) | [![Open In
-000006c0: 2043 6f6c 6162 5d28 6874 7470 733a 2f2f   Colab](https://
-000006d0: 636f 6c61 622e 7265 7365 6172 6368 2e67  colab.research.g
-000006e0: 6f6f 676c 652e 636f 6d2f 6173 7365 7473  oogle.com/assets
-000006f0: 2f63 6f6c 6162 2d62 6164 6765 2e73 7667  /colab-badge.svg
-00000700: 295d 2868 7474 7073 3a2f 2f63 6f6c 6162  )](https://colab
-00000710: 2e72 6573 6561 7263 682e 676f 6f67 6c65  .research.google
-00000720: 2e63 6f6d 2f64 7269 7665 2f31 4655 616f  .com/drive/1FUao
-00000730: 3931 4779 422d 6f6a 4752 4e5f 6f6b 5578  91GyB-ojGRN_okUx
-00000740: 5979 6661 6754 5439 7464 7350 3f75 7370  YyfagTT9tdsP?usp
-00000750: 3d73 6861 7269 6e67 2920 7c20 3c70 2061  =sharing) | <p a
-00000760: 6c69 676e 3d22 6365 6e74 6572 223e 3c61  lign="center"><a
-00000770: 2068 7265 663d 2268 7474 7073 3a2f 2f79   href="https://y
-00000780: 6f75 7475 2e62 652f 4966 624e 4f4c 524f  outu.be/IfbNOLRO
-00000790: 796d 3422 3e3c 696d 6720 7769 6474 683d  ym4"><img width=
-000007a0: 3330 2520 7372 633d 2268 7474 7073 3a2f  30% src="https:/
-000007b0: 2f72 6177 2e67 6974 6875 6275 7365 7263  /raw.githubuserc
-000007c0: 6f6e 7465 6e74 2e63 6f6d 2f75 6c74 7261  ontent.com/ultra
-000007d0: 6c79 7469 6373 2f61 7373 6574 732f 6d61  lytics/assets/ma
-000007e0: 696e 2f73 6f63 6961 6c2f 6c6f 676f 2d73  in/social/logo-s
-000007f0: 6f63 6961 6c2d 796f 7574 7562 652d 7265  ocial-youtube-re
-00000800: 6374 2e70 6e67 2220 616c 743d 2259 6f75  ct.png" alt="You
-00000810: 7475 6265 2056 6964 656f 223e 3c2f 613e  tube Video"></a>
-00000820: 3c2f 703e 207c 0d0a 7c20 5b45 7861 6d70  </p> |..| [Examp
-00000830: 6c65 206f 6620 7574 696c 697a 696e 6720  le of utilizing 
-00000840: 6120 6675 6e63 7469 6f6e 2074 6f20 7669  a function to vi
-00000850: 7375 616c 697a 6520 6261 7369 6320 556c  sualize basic Ul
-00000860: 7472 616c 7974 6963 7320 6d6f 6465 6c20  tralytics model 
-00000870: 696e 6665 7265 6e63 6520 7265 7375 6c74  inference result
-00000880: 7320 616e 6420 6d61 6e61 6769 6e67 206f  s and managing o
-00000890: 7665 726c 6170 7069 6e67 2069 6d61 6765  verlapping image
-000008a0: 2063 726f 7073 5d28 6874 7470 733a 2f2f   crops](https://
-000008b0: 6e62 7669 6577 6572 2e6f 7267 2f67 6974  nbviewer.org/git
-000008c0: 6875 622f 4b6f 6c64 696d 3230 3031 2f59  hub/Koldim2001/Y
-000008d0: 4f4c 4f2d 5061 7463 682d 4261 7365 642d  OLO-Patch-Based-
-000008e0: 496e 6665 7265 6e63 652f 626c 6f62 2f6d  Inference/blob/m
-000008f0: 6169 6e2f 6578 616d 706c 6573 2f65 7861  ain/examples/exa
-00000900: 6d70 6c65 5f65 7874 7261 5f66 756e 6374  mple_extra_funct
-00000910: 696f 6e73 2e69 7079 6e62 2920 7c20 5b21  ions.ipynb) | [!
-00000920: 5b4f 7065 6e20 496e 2043 6f6c 6162 5d28  [Open In Colab](
-00000930: 6874 7470 733a 2f2f 636f 6c61 622e 7265  https://colab.re
-00000940: 7365 6172 6368 2e67 6f6f 676c 652e 636f  search.google.co
-00000950: 6d2f 6173 7365 7473 2f63 6f6c 6162 2d62  m/assets/colab-b
-00000960: 6164 6765 2e73 7667 295d 2868 7474 7073  adge.svg)](https
-00000970: 3a2f 2f63 6f6c 6162 2e72 6573 6561 7263  ://colab.researc
-00000980: 682e 676f 6f67 6c65 2e63 6f6d 2f64 7269  h.google.com/dri
-00000990: 7665 2f31 654d 346f 3165 3041 5551 7253  ve/1eM4o1e0AUQrS
-000009a0: 316d 4c44 7063 674b 3948 4b49 6e57 4576  1mLDpcgK9HKInWEv
-000009b0: 6e61 4d6e 3f75 7370 3d73 6861 7269 6e67  naMn?usp=sharing
-000009c0: 2920 7c20 3c70 2061 6c69 676e 3d22 6365  ) | <p align="ce
-000009d0: 6e74 6572 223e 3c61 2068 7265 663d 2268  nter"><a href="h
-000009e0: 7474 7073 3a2f 2f79 6f75 7475 2e62 652f  ttps://youtu.be/
-000009f0: 6e42 5175 5761 3633 3138 3822 3e3c 696d  nBQuWa63188"><im
-00000a00: 6720 7769 6474 683d 3330 2520 7372 633d  g width=30% src=
-00000a10: 2268 7474 7073 3a2f 2f72 6177 2e67 6974  "https://raw.git
-00000a20: 6875 6275 7365 7263 6f6e 7465 6e74 2e63  hubusercontent.c
-00000a30: 6f6d 2f75 6c74 7261 6c79 7469 6373 2f61  om/ultralytics/a
-00000a40: 7373 6574 732f 6d61 696e 2f73 6f63 6961  ssets/main/socia
-00000a50: 6c2f 6c6f 676f 2d73 6f63 6961 6c2d 796f  l/logo-social-yo
-00000a60: 7574 7562 652d 7265 6374 2e70 6e67 2220  utube-rect.png" 
-00000a70: 616c 743d 2259 6f75 7475 6265 2056 6964  alt="Youtube Vid
-00000a80: 656f 223e 3c2f 613e 3c2f 703e 207c 0d0a  eo"></a></p> |..
-00000a90: 0d0a 0d0a 466f 7220 5275 7373 6961 6e20  ....For Russian 
-00000aa0: 7573 6572 732c 2074 6865 7265 2069 7320  users, there is 
-00000ab0: 6120 6465 7461 696c 6564 2076 6964 656f  a detailed video
-00000ac0: 2070 7265 7365 6e74 6174 696f 6e20 6f66   presentation of
-00000ad0: 2074 6869 7320 7072 6f6a 6563 742e 2059   this project. Y
-00000ae0: 6f75 5475 6265 2076 6964 656f 2069 6e20  ouTube video in 
-00000af0: 5275 7373 6961 6e20 6973 2061 7661 696c  Russian is avail
-00000b00: 6162 6c65 2061 7420 7468 6973 205b 5f5f  able at this [__
-00000b10: 6c69 6e6b 5f5f 5d28 6874 7470 733a 2f2f  link__](https://
-00000b20: 796f 7574 752e 6265 2f69 6863 6836 7049  youtu.be/ihch6pI
-00000b30: 5a74 5167 292e 0d0a 0d0a 2d2d 2d0d 0a23  ZtQg).....---..#
-00000b40: 2320 4578 616d 706c 6573 3a0d 0a0d 0a23  # Examples:....#
-00000b50: 2323 2320 4465 7465 6374 696f 6e20 6578  ### Detection ex
-00000b60: 616d 706c 653a 0d0a 3c69 6d67 2073 7263  ample:..<img src
-00000b70: 3d22 7265 6164 6d65 5f63 6f6e 7465 6e74  ="readme_content
-00000b80: 2f67 6574 6563 7469 6f6e 2e67 6966 2220  /getection.gif" 
-00000b90: 616c 743d 2244 6574 6563 7469 6f6e 2220  alt="Detection" 
-00000ba0: 7769 6474 683d 2238 3030 223e 0d0a 0d0a  width="800">....
-00000bb0: 2323 2323 2049 6e73 7461 6e63 6520 5365  #### Instance Se
-00000bc0: 676d 656e 7461 7469 6f6e 2065 7861 6d70  gmentation examp
-00000bd0: 6c65 2031 3a0d 0a3c 696d 6720 7372 633d  le 1:..<img src=
-00000be0: 2272 6561 646d 655f 636f 6e74 656e 742f  "readme_content/
-00000bf0: 7365 676d 656e 745f 312e 6769 6622 2061  segment_1.gif" a
-00000c00: 6c74 3d22 5365 676d 656e 7461 7469 6f6e  lt="Segmentation
-00000c10: 2220 7769 6474 683d 2238 3030 223e 0d0a  " width="800">..
-00000c20: 0d0a 2323 2323 2049 6e73 7461 6e63 6520  ..#### Instance 
-00000c30: 5365 676d 656e 7461 7469 6f6e 2065 7861  Segmentation exa
-00000c40: 6d70 6c65 2032 3a0d 0a3c 696d 6720 7372  mple 2:..<img sr
-00000c50: 633d 2272 6561 646d 655f 636f 6e74 656e  c="readme_conten
-00000c60: 742f 7365 676d 656e 745f 322e 6769 6622  t/segment_2.gif"
-00000c70: 2061 6c74 3d22 5365 676d 656e 7461 7469   alt="Segmentati
-00000c80: 6f6e 2220 7769 6474 683d 2238 3030 223e  on" width="800">
-00000c90: 0d0a 0d0a 2d2d 2d0d 0a23 2320 5573 6167  ....---..## Usag
-00000ca0: 650d 0a0d 0a23 2323 2031 2e20 5061 7463  e....### 1. Patc
-00000cb0: 682d 4261 7365 642d 496e 6665 7265 6e63  h-Based-Inferenc
-00000cc0: 650d 0a54 6f20 6361 7272 7920 6f75 7420  e..To carry out 
-00000cd0: 7061 7463 682d 6261 7365 6420 696e 6665  patch-based infe
-00000ce0: 7265 6e63 6520 6f66 2059 4f4c 4f20 6d6f  rence of YOLO mo
-00000cf0: 6465 6c73 2075 7369 6e67 206f 7572 206c  dels using our l
-00000d00: 6962 7261 7279 2c20 796f 7520 6e65 6564  ibrary, you need
-00000d10: 2074 6f20 666f 6c6c 6f77 2061 2073 6571   to follow a seq
-00000d20: 7565 6e74 6961 6c20 7072 6f63 6564 7572  uential procedur
-00000d30: 652e 2046 6972 7374 2c20 796f 7520 6372  e. First, you cr
-00000d40: 6561 7465 2061 6e20 696e 7374 616e 6365  eate an instance
-00000d50: 206f 6620 7468 6520 4d61 6b65 4372 6f70   of the MakeCrop
-00000d60: 7344 6574 6563 7454 6865 6d20 636c 6173  sDetectThem clas
-00000d70: 732c 2070 726f 7669 6469 6e67 2061 6c6c  s, providing all
-00000d80: 2064 6573 6972 6564 2070 6172 616d 6574   desired paramet
-00000d90: 6572 7320 7265 6c61 7465 6420 746f 2059  ers related to Y
-00000da0: 4f4c 4f20 696e 6665 7265 6e63 6520 616e  OLO inference an
-00000db0: 6420 7468 6520 7061 7463 6820 7365 676d  d the patch segm
-00000dc0: 656e 7461 7469 6f6e 2070 7269 6e63 6970  entation princip
-00000dd0: 6c65 2e3c 6272 2f3e 2053 7562 7365 7175  le.<br/> Subsequ
-00000de0: 656e 746c 792c 2079 6f75 2070 6173 7320  ently, you pass 
-00000df0: 7468 6520 6f62 7461 696e 6564 206f 626a  the obtained obj
-00000e00: 6563 7420 6f66 2074 6869 7320 636c 6173  ect of this clas
-00000e10: 7320 746f 2043 6f6d 6269 6e65 4465 7465  s to CombineDete
-00000e20: 6374 696f 6e73 2c20 7768 6963 6820 6661  ctions, which fa
-00000e30: 6369 6c69 7461 7465 7320 7468 6520 636f  cilitates the co
-00000e40: 6e73 6f6c 6964 6174 696f 6e20 6f66 2061  nsolidation of a
-00000e50: 6c6c 2070 7265 6469 6374 696f 6e73 2066  ll predictions f
-00000e60: 726f 6d20 6561 6368 206f 7665 726c 6170  rom each overlap
-00000e70: 7069 6e67 2063 726f 702c 2066 6f6c 6c6f  ping crop, follo
-00000e80: 7765 6420 6279 2069 6e74 656c 6c69 6765  wed by intellige
-00000e90: 6e74 2073 7570 7072 6573 7369 6f6e 206f  nt suppression o
-00000ea0: 6620 6475 706c 6963 6174 6573 2e20 3c62  f duplicates. <b
-00000eb0: 722f 3e55 706f 6e20 636f 6d70 6c65 7469  r/>Upon completi
-00000ec0: 6f6e 2c20 796f 7520 7265 6365 6976 6520  on, you receive 
-00000ed0: 7468 6520 7265 7375 6c74 2c20 6672 6f6d  the result, from
-00000ee0: 2077 6869 6368 2079 6f75 2063 616e 2065   which you can e
-00000ef0: 7874 7261 6374 2074 6865 2064 6573 6972  xtract the desir
-00000f00: 6564 206f 7574 636f 6d65 206f 6620 6672  ed outcome of fr
-00000f10: 616d 6520 7072 6f63 6573 7369 6e67 2e0d  ame processing..
-00000f20: 0a0d 0a54 6865 206f 7574 7075 7420 6f62  ...The output ob
-00000f30: 7461 696e 6564 2066 726f 6d20 7468 6520  tained from the 
-00000f40: 7072 6f63 6573 7320 696e 636c 7564 6573  process includes
-00000f50: 2073 6576 6572 616c 2061 7474 7269 6275   several attribu
-00000f60: 7465 7320 7468 6174 2063 616e 2062 6520  tes that can be 
-00000f70: 6c65 7665 7261 6765 6420 666f 7220 6675  leveraged for fu
-00000f80: 7274 6865 7220 616e 616c 7973 6973 206f  rther analysis o
-00000f90: 7220 7669 7375 616c 697a 6174 696f 6e3a  r visualization:
-00000fa0: 0d0a 0d0a 312e 2069 6d67 3a20 5468 6973  ....1. img: This
-00000fb0: 2061 7474 7269 6275 7465 2063 6f6e 7461   attribute conta
-00000fc0: 696e 7320 7468 6520 6f72 6967 696e 616c  ins the original
-00000fd0: 2069 6d61 6765 206f 6e20 7768 6963 6820   image on which 
-00000fe0: 7468 6520 696e 6665 7265 6e63 6520 7761  the inference wa
-00000ff0: 7320 7065 7266 6f72 6d65 642e 2049 7420  s performed. It 
-00001000: 7072 6f76 6964 6573 2063 6f6e 7465 7874  provides context
-00001010: 2066 6f72 2074 6865 2064 6574 6563 7465   for the detecte
-00001020: 6420 6f62 6a65 6374 732e 0d0a 0d0a 322e  d objects.....2.
-00001030: 2063 6f6e 6669 6465 6e63 6573 3a20 5468   confidences: Th
-00001040: 6973 2061 7474 7269 6275 7465 2068 6f6c  is attribute hol
-00001050: 6473 2074 6865 2063 6f6e 6669 6465 6e63  ds the confidenc
-00001060: 6520 7363 6f72 6573 2061 7373 6f63 6961  e scores associa
-00001070: 7465 6420 7769 7468 2065 6163 6820 6465  ted with each de
-00001080: 7465 6374 6564 206f 626a 6563 742e 2054  tected object. T
-00001090: 6865 7365 2073 636f 7265 7320 696e 6469  hese scores indi
-000010a0: 6361 7465 2074 6865 206d 6f64 656c 2773  cate the model's
-000010b0: 2063 6f6e 6669 6465 6e63 6520 6c65 7665   confidence leve
-000010c0: 6c20 696e 2074 6865 2061 6363 7572 6163  l in the accurac
-000010d0: 7920 6f66 2069 7473 2070 7265 6469 6374  y of its predict
-000010e0: 696f 6e73 2e0d 0a0d 0a33 2e20 626f 7865  ions.....3. boxe
-000010f0: 733a 2054 6865 7365 2062 6f75 6e64 696e  s: These boundin
-00001100: 6720 626f 7865 7320 6172 6520 7265 7072  g boxes are repr
-00001110: 6573 656e 7465 6420 6173 2061 206c 6973  esented as a lis
-00001120: 7420 6f66 206c 6973 7473 2c20 7768 6572  t of lists, wher
-00001130: 6520 6561 6368 206c 6973 7420 636f 6e74  e each list cont
-00001140: 6169 6e73 2066 6f75 7220 7661 6c75 6573  ains four values
-00001150: 3a20 5b78 5f6d 696e 2c20 795f 6d69 6e2c  : [x_min, y_min,
-00001160: 2078 5f6d 6178 2c20 795f 6d61 785d 2e20   x_max, y_max]. 
-00001170: 5468 6573 6520 7661 6c75 6573 2063 6f72  These values cor
-00001180: 7265 7370 6f6e 6420 746f 2074 6865 2063  respond to the c
-00001190: 6f6f 7264 696e 6174 6573 206f 6620 7468  oordinates of th
-000011a0: 6520 746f 702d 6c65 6674 2061 6e64 2062  e top-left and b
-000011b0: 6f74 746f 6d2d 7269 6768 7420 636f 726e  ottom-right corn
-000011c0: 6572 7320 6f66 2065 6163 6820 626f 756e  ers of each boun
-000011d0: 6469 6e67 2062 6f78 2e0d 0a0d 0a34 2e20  ding box.....4. 
-000011e0: 6d61 736b 733a 2049 6620 6176 6169 6c61  masks: If availa
-000011f0: 626c 652c 2074 6869 7320 6174 7472 6962  ble, this attrib
-00001200: 7574 6520 7072 6f76 6964 6573 2073 6567  ute provides seg
-00001210: 6d65 6e74 6174 696f 6e20 6d61 736b 7320  mentation masks 
-00001220: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
-00001230: 2074 6865 2064 6574 6563 7465 6420 6f62   the detected ob
-00001240: 6a65 6374 732e 2054 6865 7365 206d 6173  jects. These mas
-00001250: 6b73 2063 616e 2062 6520 7573 6564 2074  ks can be used t
-00001260: 6f20 7072 6563 6973 656c 7920 6465 6c69  o precisely deli
-00001270: 6e65 6174 6520 6f62 6a65 6374 2062 6f75  neate object bou
-00001280: 6e64 6172 6965 732e 0d0a 0d0a 352e 2063  ndaries.....5. c
-00001290: 6c61 7373 6573 5f69 6473 3a20 5468 6973  lasses_ids: This
-000012a0: 2061 7474 7269 6275 7465 2063 6f6e 7461   attribute conta
-000012b0: 696e 7320 7468 6520 636c 6173 7320 4944  ins the class ID
-000012c0: 7320 6173 7369 676e 6564 2074 6f20 6561  s assigned to ea
-000012d0: 6368 2064 6574 6563 7465 6420 6f62 6a65  ch detected obje
-000012e0: 6374 2e20 5468 6573 6520 4944 7320 636f  ct. These IDs co
-000012f0: 7272 6573 706f 6e64 2074 6f20 7370 6563  rrespond to spec
-00001300: 6966 6963 206f 626a 6563 7420 636c 6173  ific object clas
-00001310: 7365 7320 6465 6669 6e65 6420 6475 7269  ses defined duri
-00001320: 6e67 2074 6865 206d 6f64 656c 2074 7261  ng the model tra
-00001330: 696e 696e 6720 7068 6173 652e 0d0a 0d0a  ining phase.....
-00001340: 362e 2063 6c61 7373 6573 5f6e 616d 6573  6. classes_names
-00001350: 3a20 5468 6573 6520 6172 6520 7468 6520  : These are the 
-00001360: 6875 6d61 6e2d 7265 6164 6162 6c65 206e  human-readable n
-00001370: 616d 6573 2063 6f72 7265 7370 6f6e 6469  ames correspondi
-00001380: 6e67 2074 6f20 7468 6520 636c 6173 7320  ng to the class 
-00001390: 4944 732e 2054 6865 7920 7072 6f76 6964  IDs. They provid
-000013a0: 6520 7365 6d61 6e74 6963 206c 6162 656c  e semantic label
-000013b0: 7320 666f 7220 7468 6520 6465 7465 6374  s for the detect
-000013c0: 6564 206f 626a 6563 7473 2c20 6d61 6b69  ed objects, maki
-000013d0: 6e67 2074 6865 2072 6573 756c 7473 2065  ng the results e
-000013e0: 6173 6965 7220 746f 2069 6e74 6572 7072  asier to interpr
-000013f0: 6574 2e0d 0a0d 0a60 6060 7079 7468 6f6e  et.....```python
-00001400: 0d0a 696d 706f 7274 2063 7632 0d0a 6672  ..import cv2..fr
-00001410: 6f6d 2070 6174 6368 6564 5f79 6f6c 6f5f  om patched_yolo_
-00001420: 696e 6665 7220 696d 706f 7274 204d 616b  infer import Mak
-00001430: 6543 726f 7073 4465 7465 6374 5468 656d  eCropsDetectThem
-00001440: 2c20 436f 6d62 696e 6544 6574 6563 7469  , CombineDetecti
-00001450: 6f6e 730d 0a0d 0a23 204c 6f61 6420 7468  ons....# Load th
-00001460: 6520 696d 6167 6520 0d0a 696d 675f 7061  e image ..img_pa
-00001470: 7468 203d 2027 7465 7374 5f69 6d61 6765  th = 'test_image
-00001480: 2e6a 7067 270d 0a69 6d67 203d 2063 7632  .jpg'..img = cv2
-00001490: 2e69 6d72 6561 6428 696d 675f 7061 7468  .imread(img_path
-000014a0: 290d 0a0d 0a65 6c65 6d65 6e74 5f63 726f  )....element_cro
-000014b0: 7073 203d 204d 616b 6543 726f 7073 4465  ps = MakeCropsDe
-000014c0: 7465 6374 5468 656d 280d 0a20 2020 2069  tectThem(..    i
-000014d0: 6d61 6765 3d69 6d67 2c0d 0a20 2020 206d  mage=img,..    m
-000014e0: 6f64 656c 5f70 6174 683d 2279 6f6c 6f76  odel_path="yolov
-000014f0: 386d 2e70 7422 2c0d 0a20 2020 2073 6567  8m.pt",..    seg
-00001500: 6d65 6e74 3d46 616c 7365 2c0d 0a20 2020  ment=False,..   
-00001510: 2073 6861 7065 5f78 3d36 3430 2c0d 0a20   shape_x=640,.. 
-00001520: 2020 2073 6861 7065 5f79 3d36 3430 2c0d     shape_y=640,.
-00001530: 0a20 2020 206f 7665 726c 6170 5f78 3d35  .    overlap_x=5
-00001540: 302c 0d0a 2020 2020 6f76 6572 6c61 705f  0,..    overlap_
-00001550: 793d 3530 2c0d 0a20 2020 2063 6f6e 663d  y=50,..    conf=
-00001560: 302e 352c 0d0a 2020 2020 696f 753d 302e  0.5,..    iou=0.
-00001570: 372c 0d0a 2020 2020 7265 7369 7a65 5f69  7,..    resize_i
-00001580: 6e69 7469 616c 5f73 697a 653d 5472 7565  nitial_size=True
-00001590: 2c0d 0a29 0d0a 7265 7375 6c74 203d 2043  ,..)..result = C
-000015a0: 6f6d 6269 6e65 4465 7465 6374 696f 6e73  ombineDetections
-000015b0: 2865 6c65 6d65 6e74 5f63 726f 7073 2c20  (element_crops, 
-000015c0: 6e6d 735f 7468 7265 7368 6f6c 643d 302e  nms_threshold=0.
-000015d0: 3235 2c20 6d61 7463 685f 6d65 7472 6963  25, match_metric
-000015e0: 3d27 494f 5327 2920 200d 0a0d 0a23 2046  ='IOS')  ....# F
-000015f0: 696e 616c 2052 6573 756c 7473 3a0d 0a69  inal Results:..i
-00001600: 6d67 3d72 6573 756c 742e 696d 6167 650d  mg=result.image.
-00001610: 0a63 6f6e 6669 6465 6e63 6573 3d72 6573  .confidences=res
-00001620: 756c 742e 6669 6c74 6572 6564 5f63 6f6e  ult.filtered_con
-00001630: 6669 6465 6e63 6573 0d0a 626f 7865 733d  fidences..boxes=
-00001640: 7265 7375 6c74 2e66 696c 7465 7265 645f  result.filtered_
-00001650: 626f 7865 730d 0a6d 6173 6b73 3d72 6573  boxes..masks=res
-00001660: 756c 742e 6669 6c74 6572 6564 5f6d 6173  ult.filtered_mas
-00001670: 6b73 0d0a 636c 6173 7365 735f 6964 733d  ks..classes_ids=
-00001680: 7265 7375 6c74 2e66 696c 7465 7265 645f  result.filtered_
-00001690: 636c 6173 7365 735f 6964 0d0a 636c 6173  classes_id..clas
-000016a0: 7365 735f 6e61 6d65 733d 7265 7375 6c74  ses_names=result
-000016b0: 2e66 696c 7465 7265 645f 636c 6173 7365  .filtered_classe
-000016c0: 735f 6e61 6d65 730d 0a60 6060 0d0a 0d0a  s_names..```....
-000016d0: 2323 2323 2045 7870 6c61 6e61 7469 6f6e  #### Explanation
-000016e0: 206f 6620 706f 7373 6962 6c65 2069 6e70   of possible inp
-000016f0: 7574 2061 7267 756d 656e 7473 3a0d 0a0d  ut arguments:...
-00001700: 0a2a 2a4d 616b 6543 726f 7073 4465 7465  .**MakeCropsDete
-00001710: 6374 5468 656d 2a2a 0d0a 436c 6173 7320  ctThem**..Class 
-00001720: 696d 706c 656d 656e 7469 6e67 2063 726f  implementing cro
-00001730: 7070 696e 6720 616e 6420 7061 7373 696e  pping and passin
-00001740: 6720 6372 6f70 7320 7468 726f 7567 6820  g crops through 
-00001750: 6120 6e65 7572 616c 206e 6574 776f 726b  a neural network
-00001760: 2066 6f72 2064 6574 6563 7469 6f6e 2f73   for detection/s
-00001770: 6567 6d65 6e74 6174 696f 6e2e 5c0d 0a2a  egmentation.\..*
-00001780: 2a41 7267 733a 2a2a 0d0a 2d20 2a2a 696d  *Args:**..- **im
-00001790: 6167 652a 2a20 282a 6e70 2e6e 6461 7272  age** (*np.ndarr
-000017a0: 6179 2a29 3a20 496e 7075 7420 696d 6167  ay*): Input imag
-000017b0: 6520 4247 522e 0d0a 2d20 2a2a 6d6f 6465  e BGR...- **mode
-000017c0: 6c5f 7061 7468 2a2a 2028 2a73 7472 2a29  l_path** (*str*)
-000017d0: 3a20 5061 7468 2074 6f20 7468 6520 594f  : Path to the YO
-000017e0: 4c4f 206d 6f64 656c 2e0d 0a2d 202a 2a6d  LO model...- **m
-000017f0: 6f64 656c 2a2a 2028 2a75 6c74 7261 6c79  odel** (*ultraly
-00001800: 7469 6373 206d 6f64 656c 2a29 2050 7265  tics model*) Pre
-00001810: 2d69 6e69 7469 616c 697a 6564 206d 6f64  -initialized mod
-00001820: 656c 206f 626a 6563 742e 2049 6620 7072  el object. If pr
-00001830: 6f76 6964 6564 2c20 7468 6520 6d6f 6465  ovided, the mode
-00001840: 6c20 7769 6c6c 2062 6520 7573 6564 2064  l will be used d
-00001850: 6972 6563 746c 7920 696e 7374 6561 6420  irectly instead 
-00001860: 6f66 206c 6f61 6469 6e67 2066 726f 6d20  of loading from 
-00001870: 6d6f 6465 6c5f 7061 7468 2e0d 0a2d 202a  model_path...- *
-00001880: 2a69 6d67 737a 2a2a 2028 2a69 6e74 2a29  *imgsz** (*int*)
-00001890: 3a20 5369 7a65 206f 6620 7468 6520 696e  : Size of the in
-000018a0: 7075 7420 696d 6167 6520 666f 7220 696e  put image for in
-000018b0: 6665 7265 6e63 6520 594f 4c4f 2e0d 0a2d  ference YOLO...-
-000018c0: 202a 2a63 6f6e 662a 2a20 282a 666c 6f61   **conf** (*floa
-000018d0: 742a 293a 2043 6f6e 6669 6465 6e63 6520  t*): Confidence 
-000018e0: 7468 7265 7368 6f6c 6420 666f 7220 6465  threshold for de
-000018f0: 7465 6374 696f 6e73 2059 4f4c 4f2e 0d0a  tections YOLO...
-00001900: 2d20 2a2a 696f 752a 2a20 282a 666c 6f61  - **iou** (*floa
-00001910: 742a 293a 2049 6f55 2074 6872 6573 686f  t*): IoU thresho
-00001920: 6c64 2066 6f72 206e 6f6e 2d6d 6178 696d  ld for non-maxim
-00001930: 756d 2073 7570 7072 6573 7369 6f6e 2059  um suppression Y
-00001940: 4f4c 4f76 3820 6f66 2073 696e 676c 6520  OLOv8 of single 
-00001950: 6372 6f70 2e0d 0a2d 202a 2a63 6c61 7373  crop...- **class
-00001960: 6573 5f6c 6973 742a 2a20 282a 4c69 7374  es_list** (*List
-00001970: 5b69 6e74 5d20 6f72 204e 6f6e 652a 293a  [int] or None*):
-00001980: 204c 6973 7420 6f66 2063 6c61 7373 6573   List of classes
-00001990: 2074 6f20 6669 6c74 6572 2064 6574 6563   to filter detec
-000019a0: 7469 6f6e 732e 2049 6620 4e6f 6e65 2c20  tions. If None, 
-000019b0: 616c 6c20 636c 6173 7365 7320 6172 6520  all classes are 
-000019c0: 636f 6e73 6964 6572 6564 2e20 4465 6661  considered. Defa
-000019d0: 756c 7473 2074 6f20 4e6f 6e65 2e0d 0a2d  ults to None...-
-000019e0: 202a 2a73 6567 6d65 6e74 2a2a 2028 2a62   **segment** (*b
-000019f0: 6f6f 6c2a 293a 2057 6865 7468 6572 2074  ool*): Whether t
-00001a00: 6f20 7065 7266 6f72 6d20 7365 676d 656e  o perform segmen
-00001a10: 7461 7469 6f6e 2028 594f 4c4f 7638 2d73  tation (YOLOv8-s
-00001a20: 6567 292e 0d0a 2d20 2a2a 7368 6170 655f  eg)...- **shape_
-00001a30: 782a 2a20 282a 696e 742a 293a 2053 697a  x** (*int*): Siz
-00001a40: 6520 6f66 2074 6865 2063 726f 7020 696e  e of the crop in
-00001a50: 2074 6865 2078 2d63 6f6f 7264 696e 6174   the x-coordinat
-00001a60: 652e 0d0a 2d20 2a2a 7368 6170 655f 792a  e...- **shape_y*
-00001a70: 2a20 282a 696e 742a 293a 2053 697a 6520  * (*int*): Size 
-00001a80: 6f66 2074 6865 2063 726f 7020 696e 2074  of the crop in t
-00001a90: 6865 2079 2d63 6f6f 7264 696e 6174 652e  he y-coordinate.
-00001aa0: 0d0a 2d20 2a2a 6f76 6572 6c61 705f 782a  ..- **overlap_x*
-00001ab0: 2a20 282a 666c 6f61 742a 293a 2050 6572  * (*float*): Per
-00001ac0: 6365 6e74 6167 6520 6f66 206f 7665 726c  centage of overl
-00001ad0: 6170 2061 6c6f 6e67 2074 6865 2078 2d61  ap along the x-a
-00001ae0: 7869 732e 0d0a 2d20 2a2a 6f76 6572 6c61  xis...- **overla
-00001af0: 705f 792a 2a20 282a 666c 6f61 742a 293a  p_y** (*float*):
-00001b00: 2050 6572 6365 6e74 6167 6520 6f66 206f   Percentage of o
-00001b10: 7665 726c 6170 2061 6c6f 6e67 2074 6865  verlap along the
-00001b20: 2079 2d61 7869 732e 0d0a 2d20 2a2a 7368   y-axis...- **sh
-00001b30: 6f77 5f63 726f 7073 2a2a 2028 2a62 6f6f  ow_crops** (*boo
-00001b40: 6c2a 293a 2057 6865 7468 6572 2074 6f20  l*): Whether to 
-00001b50: 7669 7375 616c 697a 6520 7468 6520 6372  visualize the cr
-00001b60: 6f70 7069 6e67 2e0d 0a2d 202a 2a72 6573  opping...- **res
-00001b70: 697a 655f 696e 6974 6961 6c5f 7369 7a65  ize_initial_size
-00001b80: 2a2a 2028 2a62 6f6f 6c2a 293a 2057 6865  ** (*bool*): Whe
-00001b90: 7468 6572 2074 6f20 7265 7369 7a65 2074  ther to resize t
-00001ba0: 6865 2072 6573 756c 7473 2074 6f20 7468  he results to th
-00001bb0: 6520 6f72 6967 696e 616c 2069 6d61 6765  e original image
-00001bc0: 2073 697a 6520 2870 733a 2073 6c6f 7720   size (ps: slow 
-00001bd0: 6f70 6572 6174 696f 6e29 2e0d 0a0d 0a2a  operation).....*
-00001be0: 2a43 6f6d 6269 6e65 4465 7465 6374 696f  *CombineDetectio
-00001bf0: 6e73 2a2a 0d0a 436c 6173 7320 696d 706c  ns**..Class impl
-00001c00: 656d 656e 7469 6e67 2063 6f6d 6269 6e69  ementing combini
-00001c10: 6e67 206d 6173 6b73 2f62 6f78 6573 2066  ng masks/boxes f
-00001c20: 726f 6d20 6d75 6c74 6970 6c65 2063 726f  rom multiple cro
-00001c30: 7073 202b 204e 4d53 2028 4e6f 6e2d 4d61  ps + NMS (Non-Ma
-00001c40: 7869 6d75 6d20 5375 7070 7265 7373 696f  ximum Suppressio
-00001c50: 6e29 2e5c 0d0a 2a2a 4172 6773 3a2a 2a0d  n).\..**Args:**.
-00001c60: 0a2d 202a 2a65 6c65 6d65 6e74 5f63 726f  .- **element_cro
-00001c70: 7073 2a2a 2028 2a4d 616b 6543 726f 7073  ps** (*MakeCrops
-00001c80: 4465 7465 6374 5468 656d 2a29 3a20 4f62  DetectThem*): Ob
-00001c90: 6a65 6374 2063 6f6e 7461 696e 696e 6720  ject containing 
-00001ca0: 6372 6f70 2069 6e66 6f72 6d61 7469 6f6e  crop information
-00001cb0: 2e0d 0a2d 202a 2a6e 6d73 5f74 6872 6573  ...- **nms_thres
-00001cc0: 686f 6c64 2a2a 2028 2a66 6c6f 6174 2a29  hold** (*float*)
-00001cd0: 3a20 496f 552f 496f 5320 7468 7265 7368  : IoU/IoS thresh
-00001ce0: 6f6c 6420 666f 7220 6e6f 6e2d 6d61 7869  old for non-maxi
-00001cf0: 6d75 6d20 7375 7070 7265 7373 696f 6e2e  mum suppression.
-00001d00: 0d0a 2d20 2a2a 6d61 7463 685f 6d65 7472  ..- **match_metr
-00001d10: 6963 2a2a 2028 2a73 7472 2a29 3a20 4d61  ic** (*str*): Ma
-00001d20: 7463 6869 6e67 206d 6574 7269 632c 2065  tching metric, e
-00001d30: 6974 6865 7220 2749 4f55 2720 6f72 2027  ither 'IOU' or '
-00001d40: 494f 5327 2e0d 0a2d 202a 2a69 6e74 656c  IOS'...- **intel
-00001d50: 6c69 6765 6e74 5f73 6f72 7465 722a 2a20  ligent_sorter** 
-00001d60: 282a 626f 6f6c 2a29 3a20 456e 6162 6c65  (*bool*): Enable
-00001d70: 2073 6f72 7469 6e67 2062 7920 6172 6561   sorting by area
-00001d80: 2061 6e64 2072 6f75 6e64 6564 2063 6f6e   and rounded con
-00001d90: 6669 6465 6e63 6520 7061 7261 6d65 7465  fidence paramete
-00001da0: 722e 200d 0a20 2020 2020 2020 2020 2020  r. ..           
-00001db0: 2049 6620 4661 6c73 652c 2073 6f72 7469   If False, sorti
-00001dc0: 6e67 2077 696c 6c20 6265 2064 6f6e 6520  ng will be done 
-00001dd0: 6f6e 6c79 2062 7920 636f 6e66 6964 656e  only by confiden
-00001de0: 6365 2028 7573 7561 6c20 6e6d 7329 2e20  ce (usual nms). 
-00001df0: 2844 6166 6175 6c74 2069 7320 5472 7565  (Dafault is True
-00001e00: 290d 0a0d 0a0d 0a0d 0a2d 2d2d 0d0a 2323  )........---..##
-00001e10: 2320 322e 2043 7573 746f 6d20 696e 6665  # 2. Custom infe
-00001e20: 7265 6e63 6520 7669 7375 616c 697a 6174  rence visualizat
-00001e30: 696f 6e3a 0d0a 5669 7375 616c 697a 6573  ion:..Visualizes
-00001e40: 2063 7573 746f 6d20 7265 7375 6c74 7320   custom results 
-00001e50: 6f66 206f 626a 6563 7420 6465 7465 6374  of object detect
-00001e60: 696f 6e20 6f72 2073 6567 6d65 6e74 6174  ion or segmentat
-00001e70: 696f 6e20 6f6e 2061 6e20 696d 6167 652e  ion on an image.
-00001e80: 0d0a 0d0a 2a2a 4172 6773 3a2a 2a0d 0a2d  ....**Args:**..-
-00001e90: 202a 2a69 6d67 2a2a 2028 2a6e 756d 7079   **img** (*numpy
-00001ea0: 2e6e 6461 7272 6179 2a29 3a20 5468 6520  .ndarray*): The 
-00001eb0: 696e 7075 7420 696d 6167 6520 696e 2042  input image in B
-00001ec0: 4752 2066 6f72 6d61 742e 0d0a 2d20 2a2a  GR format...- **
-00001ed0: 626f 7865 732a 2a20 282a 6c69 7374 2a29  boxes** (*list*)
-00001ee0: 3a20 4120 6c69 7374 206f 6620 626f 756e  : A list of boun
-00001ef0: 6469 6e67 2062 6f78 6573 2069 6e20 7468  ding boxes in th
-00001f00: 6520 666f 726d 6174 205b 785f 6d69 6e2c  e format [x_min,
-00001f10: 2079 5f6d 696e 2c20 785f 6d61 782c 2079   y_min, x_max, y
-00001f20: 5f6d 6178 5d2e 0d0a 2d20 2a2a 636c 6173  _max]...- **clas
-00001f30: 7365 735f 6964 732a 2a20 282a 6c69 7374  ses_ids** (*list
-00001f40: 2a29 3a20 4120 6c69 7374 206f 6620 636c  *): A list of cl
-00001f50: 6173 7320 4944 7320 666f 7220 6561 6368  ass IDs for each
-00001f60: 2064 6574 6563 7469 6f6e 2e0d 0a2d 202a   detection...- *
-00001f70: 2a63 6f6e 6669 6465 6e63 6573 2a2a 2028  *confidences** (
-00001f80: 2a6c 6973 742a 293a 2041 206c 6973 7420  *list*): A list 
-00001f90: 6f66 2063 6f6e 6669 6465 6e63 6520 7363  of confidence sc
-00001fa0: 6f72 6573 2063 6f72 7265 7370 6f6e 6469  ores correspondi
-00001fb0: 6e67 2074 6f20 6561 6368 2062 6f75 6e64  ng to each bound
-00001fc0: 696e 6720 626f 782e 2044 6566 6175 6c74  ing box. Default
-00001fd0: 2069 7320 616e 2065 6d70 7479 206c 6973   is an empty lis
-00001fe0: 742e 0d0a 2d20 2a2a 636c 6173 7365 735f  t...- **classes_
-00001ff0: 6e61 6d65 732a 2a20 282a 6c69 7374 2a29  names** (*list*)
-00002000: 3a20 4120 6c69 7374 206f 6620 636c 6173  : A list of clas
-00002010: 7320 6e61 6d65 7320 636f 7272 6573 706f  s names correspo
-00002020: 6e64 696e 6720 746f 2074 6865 2063 6c61  nding to the cla
-00002030: 7373 2049 4473 2e20 4465 6661 756c 7420  ss IDs. Default 
-00002040: 6973 2061 6e20 656d 7074 7920 6c69 7374  is an empty list
-00002050: 2e0d 0a2d 202a 2a6d 6173 6b73 2a2a 2028  ...- **masks** (
-00002060: 2a6c 6973 742a 293a 2041 206c 6973 7420  *list*): A list 
-00002070: 6f66 206d 6173 6b73 2e20 4465 6661 756c  of masks. Defaul
-00002080: 7420 6973 2061 6e20 656d 7074 7920 6c69  t is an empty li
-00002090: 7374 2e0d 0a2d 202a 2a73 6567 6d65 6e74  st...- **segment
+000001d0: 4f4c 4f76 382d 7365 672c 2059 4f4c 4f76  OLOv8-seg, YOLOv
+000001e0: 392c 2059 4f4c 4f76 392d 7365 672c 2046  9, YOLOv9-seg, F
+000001f0: 6173 7453 414d 2c20 616e 6420 5254 4445  astSAM, and RTDE
+00000200: 5452 2e20 5573 6572 7320 6361 6e20 7365  TR. Users can se
+00000210: 6c65 6374 2066 726f 6d20 7072 652d 7472  lect from pre-tr
+00000220: 6169 6e65 6420 6f70 7469 6f6e 7320 6f72  ained options or
+00000230: 2075 7469 6c69 7a65 2063 7573 746f 6d2d   utilize custom-
+00000240: 7472 6169 6e65 6420 6d6f 6465 6c73 2074  trained models t
+00000250: 6f20 6265 7374 206d 6565 7420 7468 6569  o best meet thei
+00000260: 7220 7461 736b 2072 6571 7569 7265 6d65  r task requireme
+00000270: 6e74 732e 0d0a 0d0a 2323 2049 6e73 7461  nts.....## Insta
+00000280: 6c6c 6174 696f 6e0d 0a59 6f75 2063 616e  llation..You can
+00000290: 2069 6e73 7461 6c6c 2074 6865 206c 6962   install the lib
+000002a0: 7261 7279 2076 6961 2070 6970 3a0d 0a0d  rary via pip:...
+000002b0: 0a60 6060 6261 7368 0d0a 7069 7020 696e  .```bash..pip in
+000002c0: 7374 616c 6c20 7061 7463 6865 645f 796f  stall patched_yo
+000002d0: 6c6f 5f69 6e66 6572 0d0a 6060 600d 0a0d  lo_infer..```...
+000002e0: 0a5b 215b 5079 5049 2056 6572 7369 6f6e  .[![PyPI Version
+000002f0: 5d28 6874 7470 733a 2f2f 696d 672e 7368  ](https://img.sh
+00000300: 6965 6c64 732e 696f 2f70 7970 692f 762f  ields.io/pypi/v/
+00000310: 7061 7463 6865 642d 796f 6c6f 2d69 6e66  patched-yolo-inf
+00000320: 6572 2e73 7667 295d 2868 7474 7073 3a2f  er.svg)](https:/
+00000330: 2f70 7970 692e 6f72 672f 7072 6f6a 6563  /pypi.org/projec
+00000340: 742f 7061 7463 6865 642d 796f 6c6f 2d69  t/patched-yolo-i
+00000350: 6e66 6572 2f29 202d 2043 6c69 636b 2068  nfer/) - Click h
+00000360: 6572 6520 746f 2076 6973 6974 2074 6865  ere to visit the
+00000370: 2050 7950 4920 7061 6765 2066 6f72 2060   PyPI page for `
+00000380: 7061 7463 6865 642d 796f 6c6f 2d69 6e66  patched-yolo-inf
+00000390: 6572 602c 2077 6865 7265 2079 6f75 2063  er`, where you c
+000003a0: 616e 2066 696e 6420 6d6f 7265 2069 6e66  an find more inf
+000003b0: 6f72 6d61 7469 6f6e 2061 6e64 2064 6f63  ormation and doc
+000003c0: 756d 656e 7461 7469 6f6e 2e0d 0a0d 0a4e  umentation.....N
+000003d0: 6f74 653a 2049 6620 4355 4441 2073 7570  ote: If CUDA sup
+000003e0: 706f 7274 2069 7320 6176 6169 6c61 626c  port is availabl
+000003f0: 652c 2069 7427 7320 7265 636f 6d6d 656e  e, it's recommen
+00000400: 6465 6420 746f 2070 7265 2d69 6e73 7461  ded to pre-insta
+00000410: 6c6c 2050 7954 6f72 6368 2077 6974 6820  ll PyTorch with 
+00000420: 4355 4441 2073 7570 706f 7274 2062 6566  CUDA support bef
+00000430: 6f72 6520 696e 7374 616c 6c69 6e67 2074  ore installing t
+00000440: 6865 206c 6962 7261 7279 2e20 4f74 6865  he library. Othe
+00000450: 7277 6973 652c 2074 6865 2043 5055 2076  rwise, the CPU v
+00000460: 6572 7369 6f6e 2077 696c 6c20 6265 2069  ersion will be i
+00000470: 6e73 7461 6c6c 6564 2062 7920 6465 6661  nstalled by defa
+00000480: 756c 742e 0d0a 0d0a 2d2d 2d0d 0a0d 0a3c  ult.....---....<
+00000490: 2f64 6574 6169 6c73 3e0d 0a0d 0a23 2320  /details>....## 
+000004a0: 4e6f 7465 626f 6f6b 730d 0a0d 0a49 6e74  Notebooks....Int
+000004b0: 6572 6163 7469 7665 206e 6f74 6562 6f6f  eractive noteboo
+000004c0: 6b73 2061 7265 2070 726f 7669 6465 6420  ks are provided 
+000004d0: 746f 2073 686f 7763 6173 6520 7468 6520  to showcase the 
+000004e0: 6675 6e63 7469 6f6e 616c 6974 7920 6f66  functionality of
+000004f0: 2074 6865 206c 6962 7261 7279 2e20 5468   the library. Th
+00000500: 6573 6520 6e6f 7465 626f 6f6b 7320 636f  ese notebooks co
+00000510: 7665 7220 6261 7463 682d 696e 6665 7265  ver batch-infere
+00000520: 6e63 6520 7072 6f63 6564 7572 6573 2066  nce procedures f
+00000530: 6f72 2064 6574 6563 7469 6f6e 2c20 696e  or detection, in
+00000540: 7374 616e 6365 2073 6567 6d65 6e74 6174  stance segmentat
+00000550: 696f 6e2c 2069 6e66 6572 656e 6365 2063  ion, inference c
+00000560: 7573 746f 6d20 7669 7375 616c 697a 6174  ustom visualizat
+00000570: 696f 6e2c 2061 6e64 206d 6f72 652e 2045  ion, and more. E
+00000580: 6163 6820 6e6f 7465 626f 6f6b 2069 7320  ach notebook is 
+00000590: 7061 6972 6564 2077 6974 6820 6120 7475  paired with a tu
+000005a0: 746f 7269 616c 206f 6e20 596f 7554 7562  torial on YouTub
+000005b0: 652c 206d 616b 696e 6720 6974 2065 6173  e, making it eas
+000005c0: 7920 746f 206c 6561 726e 2061 6e64 2069  y to learn and i
+000005d0: 6d70 6c65 6d65 6e74 2066 6561 7475 7265  mplement feature
+000005e0: 732e 0d0a 0d0a 0d0a 0d0a 7c20 2a2a 546f  s.........| **To
+000005f0: 7069 632a 2a20 7c20 2a2a 4e6f 7465 626f  pic** | **Notebo
+00000600: 6f6b 2a2a 207c 202a 2a59 6f75 5475 6265  ok** | **YouTube
+00000610: 2a2a 207c 0d0a 7c20 2d2d 2d2d 2d20 7c20  ** |..| ----- | 
+00000620: 2d2d 2d2d 2d2d 2d2d 207c 202d 2d2d 2d2d  -------- | -----
+00000630: 2d2d 207c 0d0a 7c20 5b50 6174 6368 2d42  -- |..| [Patch-B
+00000640: 6173 6564 2d49 6e66 6572 656e 6365 2045  ased-Inference E
+00000650: 7861 6d70 6c65 5d5b 6e62 5f65 7861 6d70  xample][nb_examp
+00000660: 6c65 315d 207c 205b 215b 4f70 656e 2049  le1] | [![Open I
+00000670: 6e20 436f 6c61 625d 5b63 6f6c 6162 5f62  n Colab][colab_b
+00000680: 6164 6765 5d5d 5b63 6f6c 6162 5f65 7831  adge]][colab_ex1
+00000690: 5d20 7c3c 6469 7620 616c 6967 6e3d 2263  ] |<div align="c
+000006a0: 656e 7465 7222 3e5b 3c69 6d67 2077 6964  enter">[<img wid
+000006b0: 7468 3d33 3025 2061 6c74 3d22 596f 7574  th=30% alt="Yout
+000006c0: 7562 6520 5669 6465 6f22 2073 7263 3d68  ube Video" src=h
+000006d0: 7474 7073 3a2f 2f72 6177 2e67 6974 6875  ttps://raw.githu
+000006e0: 6275 7365 7263 6f6e 7465 6e74 2e63 6f6d  busercontent.com
+000006f0: 2f75 6c74 7261 6c79 7469 6373 2f61 7373  /ultralytics/ass
+00000700: 6574 732f 6d61 696e 2f73 6f63 6961 6c2f  ets/main/social/
+00000710: 6c6f 676f 2d73 6f63 6961 6c2d 796f 7574  logo-social-yout
+00000720: 7562 652d 7265 6374 2e70 6e67 3e5d 5b79  ube-rect.png>][y
+00000730: 745f 6c69 6e6b 315d 207c 0d0a 7c20 5b45  t_link1] |..| [E
+00000740: 7861 6d70 6c65 206f 6620 7574 696c 697a  xample of utiliz
+00000750: 696e 6720 6120 6675 6e63 7469 6f6e 2074  ing a function t
+00000760: 6f20 7669 7375 616c 697a 6520 6261 7369  o visualize basi
+00000770: 6320 556c 7472 616c 7974 6963 7320 6d6f  c Ultralytics mo
+00000780: 6465 6c20 696e 6665 7265 6e63 6520 7265  del inference re
+00000790: 7375 6c74 7320 616e 6420 6d61 6e61 6769  sults and managi
+000007a0: 6e67 206f 7665 726c 6170 7069 6e67 2069  ng overlapping i
+000007b0: 6d61 6765 2063 726f 7073 5d5b 6e62 5f65  mage crops][nb_e
+000007c0: 7861 6d70 6c65 325d 207c 205b 215b 4f70  xample2] | [![Op
+000007d0: 656e 2049 6e20 436f 6c61 625d 5b63 6f6c  en In Colab][col
+000007e0: 6162 5f62 6164 6765 5d5d 5b63 6f6c 6162  ab_badge]][colab
+000007f0: 5f65 7832 5d20 7c20 3c64 6976 2061 6c69  _ex2] | <div ali
+00000800: 676e 3d22 6365 6e74 6572 223e 5b3c 696d  gn="center">[<im
+00000810: 6720 7769 6474 683d 3330 2520 616c 743d  g width=30% alt=
+00000820: 2259 6f75 7475 6265 2056 6964 656f 2220  "Youtube Video" 
+00000830: 7372 633d 6874 7470 733a 2f2f 7261 772e  src=https://raw.
+00000840: 6769 7468 7562 7573 6572 636f 6e74 656e  githubuserconten
+00000850: 742e 636f 6d2f 756c 7472 616c 7974 6963  t.com/ultralytic
+00000860: 732f 6173 7365 7473 2f6d 6169 6e2f 736f  s/assets/main/so
+00000870: 6369 616c 2f6c 6f67 6f2d 736f 6369 616c  cial/logo-social
+00000880: 2d79 6f75 7475 6265 2d72 6563 742e 706e  -youtube-rect.pn
+00000890: 673e 5d5b 7974 5f6c 696e 6b32 5d20 7c0d  g>][yt_link2] |.
+000008a0: 0a0d 0a0d 0a46 6f72 2052 7573 7369 616e  .....For Russian
+000008b0: 2075 7365 7273 2c20 7468 6572 6520 6973   users, there is
+000008c0: 2061 2064 6574 6169 6c65 6420 7669 6465   a detailed vide
+000008d0: 6f20 7072 6573 656e 7461 7469 6f6e 206f  o presentation o
+000008e0: 6620 7468 6973 2070 726f 6a65 6374 2e20  f this project. 
+000008f0: 596f 7554 7562 6520 7669 6465 6f20 696e  YouTube video in
+00000900: 2052 7573 7369 616e 2069 7320 6176 6169   Russian is avai
+00000910: 6c61 626c 6520 6174 2074 6869 7320 5b5f  lable at this [_
+00000920: 5f6c 696e 6b5f 5f5d 2868 7474 7073 3a2f  _link__](https:/
+00000930: 2f79 6f75 7475 2e62 652f 6968 6368 3670  /youtu.be/ihch6p
+00000940: 495a 7451 6729 2e0d 0a0d 0a2d 2d2d 0d0a  IZtQg).....---..
+00000950: 2323 2045 7861 6d70 6c65 733a 0d0a 0d0a  ## Examples:....
+00000960: 2323 2323 2044 6574 6563 7469 6f6e 2065  #### Detection e
+00000970: 7861 6d70 6c65 3a0d 0a3c 696d 6720 7372  xample:..<img sr
+00000980: 633d 2272 6561 646d 655f 636f 6e74 656e  c="readme_conten
+00000990: 742f 6765 7465 6374 696f 6e2e 6769 6622  t/getection.gif"
+000009a0: 2061 6c74 3d22 4465 7465 6374 696f 6e22   alt="Detection"
+000009b0: 2077 6964 7468 3d22 3830 3022 3e0d 0a0d   width="800">...
+000009c0: 0a23 2323 2320 496e 7374 616e 6365 2053  .#### Instance S
+000009d0: 6567 6d65 6e74 6174 696f 6e20 6578 616d  egmentation exam
+000009e0: 706c 6520 313a 0d0a 3c69 6d67 2073 7263  ple 1:..<img src
+000009f0: 3d22 7265 6164 6d65 5f63 6f6e 7465 6e74  ="readme_content
+00000a00: 2f73 6567 6d65 6e74 5f31 2e67 6966 2220  /segment_1.gif" 
+00000a10: 616c 743d 2253 6567 6d65 6e74 6174 696f  alt="Segmentatio
+00000a20: 6e22 2077 6964 7468 3d22 3830 3022 3e0d  n" width="800">.
+00000a30: 0a0d 0a23 2323 2320 496e 7374 616e 6365  ...#### Instance
+00000a40: 2053 6567 6d65 6e74 6174 696f 6e20 6578   Segmentation ex
+00000a50: 616d 706c 6520 323a 0d0a 3c69 6d67 2073  ample 2:..<img s
+00000a60: 7263 3d22 7265 6164 6d65 5f63 6f6e 7465  rc="readme_conte
+00000a70: 6e74 2f73 6567 6d65 6e74 5f32 2e67 6966  nt/segment_2.gif
+00000a80: 2220 616c 743d 2253 6567 6d65 6e74 6174  " alt="Segmentat
+00000a90: 696f 6e22 2077 6964 7468 3d22 3830 3022  ion" width="800"
+00000aa0: 3e0d 0a0d 0a2d 2d2d 0d0a 2323 2055 7361  >....---..## Usa
+00000ab0: 6765 0d0a 0d0a 2323 2320 312e 2050 6174  ge....### 1. Pat
+00000ac0: 6368 2d42 6173 6564 2d49 6e66 6572 656e  ch-Based-Inferen
+00000ad0: 6365 0d0a 546f 2063 6172 7279 206f 7574  ce..To carry out
+00000ae0: 2070 6174 6368 2d62 6173 6564 2069 6e66   patch-based inf
+00000af0: 6572 656e 6365 206f 6620 594f 4c4f 206d  erence of YOLO m
+00000b00: 6f64 656c 7320 7573 696e 6720 6f75 7220  odels using our 
+00000b10: 6c69 6272 6172 792c 2079 6f75 206e 6565  library, you nee
+00000b20: 6420 746f 2066 6f6c 6c6f 7720 6120 7365  d to follow a se
+00000b30: 7175 656e 7469 616c 2070 726f 6365 6475  quential procedu
+00000b40: 7265 2e20 4669 7273 742c 2079 6f75 2063  re. First, you c
+00000b50: 7265 6174 6520 616e 2069 6e73 7461 6e63  reate an instanc
+00000b60: 6520 6f66 2074 6865 2060 4d61 6b65 4372  e of the `MakeCr
+00000b70: 6f70 7344 6574 6563 7454 6865 6d60 2063  opsDetectThem` c
+00000b80: 6c61 7373 2c20 7072 6f76 6964 696e 6720  lass, providing 
+00000b90: 616c 6c20 6465 7369 7265 6420 7061 7261  all desired para
+00000ba0: 6d65 7465 7273 2072 656c 6174 6564 2074  meters related t
+00000bb0: 6f20 594f 4c4f 2069 6e66 6572 656e 6365  o YOLO inference
+00000bc0: 2061 6e64 2074 6865 2070 6174 6368 2073   and the patch s
+00000bd0: 6567 6d65 6e74 6174 696f 6e20 7072 696e  egmentation prin
+00000be0: 6369 706c 652e 3c62 722f 3e20 5375 6273  ciple.<br/> Subs
+00000bf0: 6571 7565 6e74 6c79 2c20 796f 7520 7061  equently, you pa
+00000c00: 7373 2074 6865 206f 6274 6169 6e65 6420  ss the obtained 
+00000c10: 6f62 6a65 6374 206f 6620 7468 6973 2063  object of this c
+00000c20: 6c61 7373 2074 6f20 6043 6f6d 6269 6e65  lass to `Combine
+00000c30: 4465 7465 6374 696f 6e73 602c 2077 6869  Detections`, whi
+00000c40: 6368 2066 6163 696c 6974 6174 6573 2074  ch facilitates t
+00000c50: 6865 2063 6f6e 736f 6c69 6461 7469 6f6e  he consolidation
+00000c60: 206f 6620 616c 6c20 7072 6564 6963 7469   of all predicti
+00000c70: 6f6e 7320 6672 6f6d 2065 6163 6820 6f76  ons from each ov
+00000c80: 6572 6c61 7070 696e 6720 6372 6f70 2c20  erlapping crop, 
+00000c90: 666f 6c6c 6f77 6564 2062 7920 696e 7465  followed by inte
+00000ca0: 6c6c 6967 656e 7420 7375 7070 7265 7373  lligent suppress
+00000cb0: 696f 6e20 6f66 2064 7570 6c69 6361 7465  ion of duplicate
+00000cc0: 732e 203c 6272 2f3e 5570 6f6e 2063 6f6d  s. <br/>Upon com
+00000cd0: 706c 6574 696f 6e2c 2079 6f75 2072 6563  pletion, you rec
+00000ce0: 6569 7665 2074 6865 2072 6573 756c 742c  eive the result,
+00000cf0: 2066 726f 6d20 7768 6963 6820 796f 7520   from which you 
+00000d00: 6361 6e20 6578 7472 6163 7420 7468 6520  can extract the 
+00000d10: 6465 7369 7265 6420 6f75 7463 6f6d 6520  desired outcome 
+00000d20: 6f66 2066 7261 6d65 2070 726f 6365 7373  of frame process
+00000d30: 696e 672e 0d0a 0d0a 5468 6520 6f75 7470  ing.....The outp
+00000d40: 7574 206f 6274 6169 6e65 6420 6672 6f6d  ut obtained from
+00000d50: 2074 6865 2070 726f 6365 7373 2069 6e63   the process inc
+00000d60: 6c75 6465 7320 7365 7665 7261 6c20 6174  ludes several at
+00000d70: 7472 6962 7574 6573 2074 6861 7420 6361  tributes that ca
+00000d80: 6e20 6265 206c 6576 6572 6167 6564 2066  n be leveraged f
+00000d90: 6f72 2066 7572 7468 6572 2061 6e61 6c79  or further analy
+00000da0: 7369 7320 6f72 2076 6973 7561 6c69 7a61  sis or visualiza
+00000db0: 7469 6f6e 3a0d 0a0d 0a31 2e20 696d 673a  tion:....1. img:
+00000dc0: 2054 6869 7320 6174 7472 6962 7574 6520   This attribute 
+00000dd0: 636f 6e74 6169 6e73 2074 6865 206f 7269  contains the ori
+00000de0: 6769 6e61 6c20 696d 6167 6520 6f6e 2077  ginal image on w
+00000df0: 6869 6368 2074 6865 2069 6e66 6572 656e  hich the inferen
+00000e00: 6365 2077 6173 2070 6572 666f 726d 6564  ce was performed
+00000e10: 2e20 4974 2070 726f 7669 6465 7320 636f  . It provides co
+00000e20: 6e74 6578 7420 666f 7220 7468 6520 6465  ntext for the de
+00000e30: 7465 6374 6564 206f 626a 6563 7473 2e0d  tected objects..
+00000e40: 0a0d 0a32 2e20 636f 6e66 6964 656e 6365  ...2. confidence
+00000e50: 733a 2054 6869 7320 6174 7472 6962 7574  s: This attribut
+00000e60: 6520 686f 6c64 7320 7468 6520 636f 6e66  e holds the conf
+00000e70: 6964 656e 6365 2073 636f 7265 7320 6173  idence scores as
+00000e80: 736f 6369 6174 6564 2077 6974 6820 6561  sociated with ea
+00000e90: 6368 2064 6574 6563 7465 6420 6f62 6a65  ch detected obje
+00000ea0: 6374 2e20 5468 6573 6520 7363 6f72 6573  ct. These scores
+00000eb0: 2069 6e64 6963 6174 6520 7468 6520 6d6f   indicate the mo
+00000ec0: 6465 6c27 7320 636f 6e66 6964 656e 6365  del's confidence
+00000ed0: 206c 6576 656c 2069 6e20 7468 6520 6163   level in the ac
+00000ee0: 6375 7261 6379 206f 6620 6974 7320 7072  curacy of its pr
+00000ef0: 6564 6963 7469 6f6e 732e 0d0a 0d0a 332e  edictions.....3.
+00000f00: 2062 6f78 6573 3a20 5468 6573 6520 626f   boxes: These bo
+00000f10: 756e 6469 6e67 2062 6f78 6573 2061 7265  unding boxes are
+00000f20: 2072 6570 7265 7365 6e74 6564 2061 7320   represented as 
+00000f30: 6120 6c69 7374 206f 6620 6c69 7374 732c  a list of lists,
+00000f40: 2077 6865 7265 2065 6163 6820 6c69 7374   where each list
+00000f50: 2063 6f6e 7461 696e 7320 666f 7572 2076   contains four v
+00000f60: 616c 7565 733a 205b 785f 6d69 6e2c 2079  alues: [x_min, y
+00000f70: 5f6d 696e 2c20 785f 6d61 782c 2079 5f6d  _min, x_max, y_m
+00000f80: 6178 5d2e 2054 6865 7365 2076 616c 7565  ax]. These value
+00000f90: 7320 636f 7272 6573 706f 6e64 2074 6f20  s correspond to 
+00000fa0: 7468 6520 636f 6f72 6469 6e61 7465 7320  the coordinates 
+00000fb0: 6f66 2074 6865 2074 6f70 2d6c 6566 7420  of the top-left 
+00000fc0: 616e 6420 626f 7474 6f6d 2d72 6967 6874  and bottom-right
+00000fd0: 2063 6f72 6e65 7273 206f 6620 6561 6368   corners of each
+00000fe0: 2062 6f75 6e64 696e 6720 626f 782e 0d0a   bounding box...
+00000ff0: 0d0a 342e 2070 6f6c 7967 6f6e 733a 2049  ..4. polygons: I
+00001000: 6620 6176 6169 6c61 626c 652c 2074 6869  f available, thi
+00001010: 7320 6174 7472 6962 7574 6520 7072 6f76  s attribute prov
+00001020: 6964 6573 2061 206c 6973 7420 636f 6e74  ides a list cont
+00001030: 6169 6e69 6e67 204e 756d 5079 2061 7272  aining NumPy arr
+00001040: 6179 7320 6f66 2070 6f6c 7967 6f6e 2063  ays of polygon c
+00001050: 6f6f 7264 696e 6174 6573 2074 6861 7420  oordinates that 
+00001060: 7265 7072 6573 656e 7420 7365 676d 656e  represent segmen
+00001070: 7461 7469 6f6e 206d 6173 6b73 2063 6f72  tation masks cor
+00001080: 7265 7370 6f6e 6469 6e67 2074 6f20 7468  responding to th
+00001090: 6520 6465 7465 6374 6564 206f 626a 6563  e detected objec
+000010a0: 7473 2e20 5468 6573 6520 706f 6c79 676f  ts. These polygo
+000010b0: 6e73 2063 616e 2062 6520 7574 696c 697a  ns can be utiliz
+000010c0: 6564 2074 6f20 6163 6375 7261 7465 6c79  ed to accurately
+000010d0: 206f 7574 6c69 6e65 2074 6865 2062 6f75   outline the bou
+000010e0: 6e64 6172 6965 7320 6f66 2065 6163 6820  ndaries of each 
+000010f0: 6f62 6a65 6374 2e0d 0a0d 0a35 2e20 636c  object.....5. cl
+00001100: 6173 7365 735f 6964 733a 2054 6869 7320  asses_ids: This 
+00001110: 6174 7472 6962 7574 6520 636f 6e74 6169  attribute contai
+00001120: 6e73 2074 6865 2063 6c61 7373 2049 4473  ns the class IDs
+00001130: 2061 7373 6967 6e65 6420 746f 2065 6163   assigned to eac
+00001140: 6820 6465 7465 6374 6564 206f 626a 6563  h detected objec
+00001150: 742e 2054 6865 7365 2049 4473 2063 6f72  t. These IDs cor
+00001160: 7265 7370 6f6e 6420 746f 2073 7065 6369  respond to speci
+00001170: 6669 6320 6f62 6a65 6374 2063 6c61 7373  fic object class
+00001180: 6573 2064 6566 696e 6564 2064 7572 696e  es defined durin
+00001190: 6720 7468 6520 6d6f 6465 6c20 7472 6169  g the model trai
+000011a0: 6e69 6e67 2070 6861 7365 2e0d 0a0d 0a36  ning phase.....6
+000011b0: 2e20 636c 6173 7365 735f 6e61 6d65 733a  . classes_names:
+000011c0: 2054 6865 7365 2061 7265 2074 6865 2068   These are the h
+000011d0: 756d 616e 2d72 6561 6461 626c 6520 6e61  uman-readable na
+000011e0: 6d65 7320 636f 7272 6573 706f 6e64 696e  mes correspondin
+000011f0: 6720 746f 2074 6865 2063 6c61 7373 2049  g to the class I
+00001200: 4473 2e20 5468 6579 2070 726f 7669 6465  Ds. They provide
+00001210: 2073 656d 616e 7469 6320 6c61 6265 6c73   semantic labels
+00001220: 2066 6f72 2074 6865 2064 6574 6563 7465   for the detecte
+00001230: 6420 6f62 6a65 6374 732c 206d 616b 696e  d objects, makin
+00001240: 6720 7468 6520 7265 7375 6c74 7320 6561  g the results ea
+00001250: 7369 6572 2074 6f20 696e 7465 7270 7265  sier to interpre
+00001260: 742e 0d0a 0d0a 6060 6070 7974 686f 6e0d  t.....```python.
+00001270: 0a69 6d70 6f72 7420 6376 320d 0a66 726f  .import cv2..fro
+00001280: 6d20 7061 7463 6865 645f 796f 6c6f 5f69  m patched_yolo_i
+00001290: 6e66 6572 2069 6d70 6f72 7420 4d61 6b65  nfer import Make
+000012a0: 4372 6f70 7344 6574 6563 7454 6865 6d2c  CropsDetectThem,
+000012b0: 2043 6f6d 6269 6e65 4465 7465 6374 696f   CombineDetectio
+000012c0: 6e73 0d0a 0d0a 2320 4c6f 6164 2074 6865  ns....# Load the
+000012d0: 2069 6d61 6765 200d 0a69 6d67 5f70 6174   image ..img_pat
+000012e0: 6820 3d20 2774 6573 745f 696d 6167 652e  h = 'test_image.
+000012f0: 6a70 6727 0d0a 696d 6720 3d20 6376 322e  jpg'..img = cv2.
+00001300: 696d 7265 6164 2869 6d67 5f70 6174 6829  imread(img_path)
+00001310: 0d0a 0d0a 656c 656d 656e 745f 6372 6f70  ....element_crop
+00001320: 7320 3d20 4d61 6b65 4372 6f70 7344 6574  s = MakeCropsDet
+00001330: 6563 7454 6865 6d28 0d0a 2020 2020 696d  ectThem(..    im
+00001340: 6167 653d 696d 672c 0d0a 2020 2020 6d6f  age=img,..    mo
+00001350: 6465 6c5f 7061 7468 3d22 796f 6c6f 7638  del_path="yolov8
+00001360: 6d2e 7074 222c 0d0a 2020 2020 7365 676d  m.pt",..    segm
+00001370: 656e 743d 4661 6c73 652c 0d0a 2020 2020  ent=False,..    
+00001380: 7368 6170 655f 783d 3634 302c 0d0a 2020  shape_x=640,..  
+00001390: 2020 7368 6170 655f 793d 3634 302c 0d0a    shape_y=640,..
+000013a0: 2020 2020 6f76 6572 6c61 705f 783d 3530      overlap_x=50
+000013b0: 2c0d 0a20 2020 206f 7665 726c 6170 5f79  ,..    overlap_y
+000013c0: 3d35 302c 0d0a 2020 2020 636f 6e66 3d30  =50,..    conf=0
+000013d0: 2e35 2c0d 0a20 2020 2069 6f75 3d30 2e37  .5,..    iou=0.7
+000013e0: 2c0d 0a20 2020 2072 6573 697a 655f 696e  ,..    resize_in
+000013f0: 6974 6961 6c5f 7369 7a65 3d54 7275 652c  itial_size=True,
+00001400: 0d0a 290d 0a72 6573 756c 7420 3d20 436f  ..)..result = Co
+00001410: 6d62 696e 6544 6574 6563 7469 6f6e 7328  mbineDetections(
+00001420: 656c 656d 656e 745f 6372 6f70 732c 206e  element_crops, n
+00001430: 6d73 5f74 6872 6573 686f 6c64 3d30 2e32  ms_threshold=0.2
+00001440: 352c 206d 6174 6368 5f6d 6574 7269 633d  5, match_metric=
+00001450: 2749 4f53 2729 2020 0d0a 0d0a 2320 4669  'IOS')  ....# Fi
+00001460: 6e61 6c20 5265 7375 6c74 733a 0d0a 696d  nal Results:..im
+00001470: 673d 7265 7375 6c74 2e69 6d61 6765 0d0a  g=result.image..
+00001480: 636f 6e66 6964 656e 6365 733d 7265 7375  confidences=resu
+00001490: 6c74 2e66 696c 7465 7265 645f 636f 6e66  lt.filtered_conf
+000014a0: 6964 656e 6365 730d 0a62 6f78 6573 3d72  idences..boxes=r
+000014b0: 6573 756c 742e 6669 6c74 6572 6564 5f62  esult.filtered_b
+000014c0: 6f78 6573 0d0a 706f 6c79 676f 6e73 3d72  oxes..polygons=r
+000014d0: 6573 756c 742e 6669 6c74 6572 6564 5f70  esult.filtered_p
+000014e0: 6f6c 7967 6f6e 730d 0a63 6c61 7373 6573  olygons..classes
+000014f0: 5f69 6473 3d72 6573 756c 742e 6669 6c74  _ids=result.filt
+00001500: 6572 6564 5f63 6c61 7373 6573 5f69 640d  ered_classes_id.
+00001510: 0a63 6c61 7373 6573 5f6e 616d 6573 3d72  .classes_names=r
+00001520: 6573 756c 742e 6669 6c74 6572 6564 5f63  esult.filtered_c
+00001530: 6c61 7373 6573 5f6e 616d 6573 0d0a 6060  lasses_names..``
+00001540: 600d 0a0d 0a23 2323 2320 4578 706c 616e  `....#### Explan
+00001550: 6174 696f 6e20 6f66 2070 6f73 7369 626c  ation of possibl
+00001560: 6520 696e 7075 7420 6172 6775 6d65 6e74  e input argument
+00001570: 733a 0d0a 0d0a 2a2a 4d61 6b65 4372 6f70  s:....**MakeCrop
+00001580: 7344 6574 6563 7454 6865 6d2a 2a0d 0a43  sDetectThem**..C
+00001590: 6c61 7373 2069 6d70 6c65 6d65 6e74 696e  lass implementin
+000015a0: 6720 6372 6f70 7069 6e67 2061 6e64 2070  g cropping and p
+000015b0: 6173 7369 6e67 2063 726f 7073 2074 6872  assing crops thr
+000015c0: 6f75 6768 2061 206e 6575 7261 6c20 6e65  ough a neural ne
+000015d0: 7477 6f72 6b20 666f 7220 6465 7465 6374  twork for detect
+000015e0: 696f 6e2f 7365 676d 656e 7461 7469 6f6e  ion/segmentation
+000015f0: 2e5c 0d0a 2a2a 4172 6773 3a2a 2a0d 0a2d  .\..**Args:**..-
+00001600: 202a 2a69 6d61 6765 2a2a 2028 2a6e 702e   **image** (*np.
+00001610: 6e64 6172 7261 792a 293a 2049 6e70 7574  ndarray*): Input
+00001620: 2069 6d61 6765 2042 4752 2e0d 0a2d 202a   image BGR...- *
+00001630: 2a6d 6f64 656c 5f70 6174 682a 2a20 282a  *model_path** (*
+00001640: 7374 722a 293a 2050 6174 6820 746f 2074  str*): Path to t
+00001650: 6865 2059 4f4c 4f20 6d6f 6465 6c2e 0d0a  he YOLO model...
+00001660: 2d20 2a2a 6d6f 6465 6c2a 2a20 282a 756c  - **model** (*ul
+00001670: 7472 616c 7974 6963 7320 6d6f 6465 6c2a  tralytics model*
+00001680: 2920 5072 652d 696e 6974 6961 6c69 7a65  ) Pre-initialize
+00001690: 6420 6d6f 6465 6c20 6f62 6a65 6374 2e20  d model object. 
+000016a0: 4966 2070 726f 7669 6465 642c 2074 6865  If provided, the
+000016b0: 206d 6f64 656c 2077 696c 6c20 6265 2075   model will be u
+000016c0: 7365 6420 6469 7265 6374 6c79 2069 6e73  sed directly ins
+000016d0: 7465 6164 206f 6620 6c6f 6164 696e 6720  tead of loading 
+000016e0: 6672 6f6d 206d 6f64 656c 5f70 6174 682e  from model_path.
+000016f0: 0d0a 2d20 2a2a 696d 6773 7a2a 2a20 282a  ..- **imgsz** (*
+00001700: 696e 742a 293a 2053 697a 6520 6f66 2074  int*): Size of t
+00001710: 6865 2069 6e70 7574 2069 6d61 6765 2066  he input image f
+00001720: 6f72 2069 6e66 6572 656e 6365 2059 4f4c  or inference YOL
+00001730: 4f2e 0d0a 2d20 2a2a 636f 6e66 2a2a 2028  O...- **conf** (
+00001740: 2a66 6c6f 6174 2a29 3a20 436f 6e66 6964  *float*): Confid
+00001750: 656e 6365 2074 6872 6573 686f 6c64 2066  ence threshold f
+00001760: 6f72 2064 6574 6563 7469 6f6e 7320 594f  or detections YO
+00001770: 4c4f 2e0d 0a2d 202a 2a69 6f75 2a2a 2028  LO...- **iou** (
+00001780: 2a66 6c6f 6174 2a29 3a20 496f 5520 7468  *float*): IoU th
+00001790: 7265 7368 6f6c 6420 666f 7220 6e6f 6e2d  reshold for non-
+000017a0: 6d61 7869 6d75 6d20 7375 7070 7265 7373  maximum suppress
+000017b0: 696f 6e20 594f 4c4f 7638 206f 6620 7369  ion YOLOv8 of si
+000017c0: 6e67 6c65 2063 726f 702e 0d0a 2d20 2a2a  ngle crop...- **
+000017d0: 636c 6173 7365 735f 6c69 7374 2a2a 2028  classes_list** (
+000017e0: 2a4c 6973 745b 696e 745d 206f 7220 4e6f  *List[int] or No
+000017f0: 6e65 2a29 3a20 4c69 7374 206f 6620 636c  ne*): List of cl
+00001800: 6173 7365 7320 746f 2066 696c 7465 7220  asses to filter 
+00001810: 6465 7465 6374 696f 6e73 2e20 4966 204e  detections. If N
+00001820: 6f6e 652c 2061 6c6c 2063 6c61 7373 6573  one, all classes
+00001830: 2061 7265 2063 6f6e 7369 6465 7265 642e   are considered.
+00001840: 2044 6566 6175 6c74 7320 746f 204e 6f6e   Defaults to Non
+00001850: 652e 0d0a 2d20 2a2a 7365 676d 656e 742a  e...- **segment*
+00001860: 2a20 282a 626f 6f6c 2a29 3a20 5768 6574  * (*bool*): Whet
+00001870: 6865 7220 746f 2070 6572 666f 726d 2073  her to perform s
+00001880: 6567 6d65 6e74 6174 696f 6e20 2859 4f4c  egmentation (YOL
+00001890: 4f76 382d 7365 6729 2e0d 0a2d 202a 2a73  Ov8-seg)...- **s
+000018a0: 6861 7065 5f78 2a2a 2028 2a69 6e74 2a29  hape_x** (*int*)
+000018b0: 3a20 5369 7a65 206f 6620 7468 6520 6372  : Size of the cr
+000018c0: 6f70 2069 6e20 7468 6520 782d 636f 6f72  op in the x-coor
+000018d0: 6469 6e61 7465 2e0d 0a2d 202a 2a73 6861  dinate...- **sha
+000018e0: 7065 5f79 2a2a 2028 2a69 6e74 2a29 3a20  pe_y** (*int*): 
+000018f0: 5369 7a65 206f 6620 7468 6520 6372 6f70  Size of the crop
+00001900: 2069 6e20 7468 6520 792d 636f 6f72 6469   in the y-coordi
+00001910: 6e61 7465 2e0d 0a2d 202a 2a6f 7665 726c  nate...- **overl
+00001920: 6170 5f78 2a2a 2028 2a66 6c6f 6174 2a29  ap_x** (*float*)
+00001930: 3a20 5065 7263 656e 7461 6765 206f 6620  : Percentage of 
+00001940: 6f76 6572 6c61 7020 616c 6f6e 6720 7468  overlap along th
+00001950: 6520 782d 6178 6973 2e0d 0a2d 202a 2a6f  e x-axis...- **o
+00001960: 7665 726c 6170 5f79 2a2a 2028 2a66 6c6f  verlap_y** (*flo
+00001970: 6174 2a29 3a20 5065 7263 656e 7461 6765  at*): Percentage
+00001980: 206f 6620 6f76 6572 6c61 7020 616c 6f6e   of overlap alon
+00001990: 6720 7468 6520 792d 6178 6973 2e0d 0a2d  g the y-axis...-
+000019a0: 202a 2a73 686f 775f 6372 6f70 732a 2a20   **show_crops** 
+000019b0: 282a 626f 6f6c 2a29 3a20 5768 6574 6865  (*bool*): Whethe
+000019c0: 7220 746f 2076 6973 7561 6c69 7a65 2074  r to visualize t
+000019d0: 6865 2063 726f 7070 696e 672e 0d0a 2d20  he cropping...- 
+000019e0: 2a2a 7265 7369 7a65 5f69 6e69 7469 616c  **resize_initial
+000019f0: 5f73 697a 652a 2a20 282a 626f 6f6c 2a29  _size** (*bool*)
+00001a00: 3a20 5768 6574 6865 7220 746f 2072 6573  : Whether to res
+00001a10: 697a 6520 7468 6520 7265 7375 6c74 7320  ize the results 
+00001a20: 746f 2074 6865 206f 7269 6769 6e61 6c20  to the original 
+00001a30: 696d 6167 6520 7369 7a65 2028 7073 3a20  image size (ps: 
+00001a40: 736c 6f77 206f 7065 7261 7469 6f6e 292e  slow operation).
+00001a50: 0d0a 2d20 2a2a 6d65 6d6f 7279 5f6f 7074  ..- **memory_opt
+00001a60: 696d 697a 652a 2a20 282a 626f 6f6c 2a29  imize** (*bool*)
+00001a70: 3a20 4d65 6d6f 7279 206f 7074 696d 697a  : Memory optimiz
+00001a80: 6174 696f 6e20 6f70 7469 6f6e 2066 6f72  ation option for
+00001a90: 2073 6567 6d65 6e74 6174 696f 6e20 286c   segmentation (l
+00001aa0: 6573 7320 6163 6375 7261 7465 2072 6573  ess accurate res
+00001ab0: 756c 7473 2077 6865 6e20 656e 6162 6c65  ults when enable
+00001ac0: 6429 2e0d 0a0d 0a2a 2a43 6f6d 6269 6e65  d).....**Combine
+00001ad0: 4465 7465 6374 696f 6e73 2a2a 0d0a 436c  Detections**..Cl
+00001ae0: 6173 7320 696d 706c 656d 656e 7469 6e67  ass implementing
+00001af0: 2063 6f6d 6269 6e69 6e67 206d 6173 6b73   combining masks
+00001b00: 2f62 6f78 6573 2066 726f 6d20 6d75 6c74  /boxes from mult
+00001b10: 6970 6c65 2063 726f 7073 202b 204e 4d53  iple crops + NMS
+00001b20: 2028 4e6f 6e2d 4d61 7869 6d75 6d20 5375   (Non-Maximum Su
+00001b30: 7070 7265 7373 696f 6e29 2e5c 0d0a 2a2a  ppression).\..**
+00001b40: 4172 6773 3a2a 2a0d 0a2d 202a 2a65 6c65  Args:**..- **ele
+00001b50: 6d65 6e74 5f63 726f 7073 2a2a 2028 2a4d  ment_crops** (*M
+00001b60: 616b 6543 726f 7073 4465 7465 6374 5468  akeCropsDetectTh
+00001b70: 656d 2a29 3a20 4f62 6a65 6374 2063 6f6e  em*): Object con
+00001b80: 7461 696e 696e 6720 6372 6f70 2069 6e66  taining crop inf
+00001b90: 6f72 6d61 7469 6f6e 2e0d 0a2d 202a 2a6e  ormation...- **n
+00001ba0: 6d73 5f74 6872 6573 686f 6c64 2a2a 2028  ms_threshold** (
+00001bb0: 2a66 6c6f 6174 2a29 3a20 496f 552f 496f  *float*): IoU/Io
+00001bc0: 5320 7468 7265 7368 6f6c 6420 666f 7220  S threshold for 
+00001bd0: 6e6f 6e2d 6d61 7869 6d75 6d20 7375 7070  non-maximum supp
+00001be0: 7265 7373 696f 6e2e 0d0a 2d20 2a2a 6d61  ression...- **ma
+00001bf0: 7463 685f 6d65 7472 6963 2a2a 2028 2a73  tch_metric** (*s
+00001c00: 7472 2a29 3a20 4d61 7463 6869 6e67 206d  tr*): Matching m
+00001c10: 6574 7269 632c 2065 6974 6865 7220 2749  etric, either 'I
+00001c20: 4f55 2720 6f72 2027 494f 5327 2e0d 0a2d  OU' or 'IOS'...-
+00001c30: 202a 2a69 6e74 656c 6c69 6765 6e74 5f73   **intelligent_s
+00001c40: 6f72 7465 722a 2a20 282a 626f 6f6c 2a29  orter** (*bool*)
+00001c50: 3a20 456e 6162 6c65 2073 6f72 7469 6e67  : Enable sorting
+00001c60: 2062 7920 6172 6561 2061 6e64 2072 6f75   by area and rou
+00001c70: 6e64 6564 2063 6f6e 6669 6465 6e63 6520  nded confidence 
+00001c80: 7061 7261 6d65 7465 722e 200d 0a20 2020  parameter. ..   
+00001c90: 2020 2020 2020 2020 2049 6620 4661 6c73           If Fals
+00001ca0: 652c 2073 6f72 7469 6e67 2077 696c 6c20  e, sorting will 
+00001cb0: 6265 2064 6f6e 6520 6f6e 6c79 2062 7920  be done only by 
+00001cc0: 636f 6e66 6964 656e 6365 2028 7573 7561  confidence (usua
+00001cd0: 6c20 6e6d 7329 2e20 2844 6166 6175 6c74  l nms). (Dafault
+00001ce0: 2069 7320 5472 7565 290d 0a0d 0a0d 0a0d   is True).......
+00001cf0: 0a2d 2d2d 0d0a 2323 2320 322e 2043 7573  .---..### 2. Cus
+00001d00: 746f 6d20 696e 6665 7265 6e63 6520 7669  tom inference vi
+00001d10: 7375 616c 697a 6174 696f 6e3a 0d0a 5669  sualization:..Vi
+00001d20: 7375 616c 697a 6573 2063 7573 746f 6d20  sualizes custom 
+00001d30: 7265 7375 6c74 7320 6f66 206f 626a 6563  results of objec
+00001d40: 7420 6465 7465 6374 696f 6e20 6f72 2073  t detection or s
+00001d50: 6567 6d65 6e74 6174 696f 6e20 6f6e 2061  egmentation on a
+00001d60: 6e20 696d 6167 652e 0d0a 0d0a 2a2a 4172  n image.....**Ar
+00001d70: 6773 3a2a 2a0d 0a2d 202a 2a69 6d67 2a2a  gs:**..- **img**
+00001d80: 2028 2a6e 756d 7079 2e6e 6461 7272 6179   (*numpy.ndarray
+00001d90: 2a29 3a20 5468 6520 696e 7075 7420 696d  *): The input im
+00001da0: 6167 6520 696e 2042 4752 2066 6f72 6d61  age in BGR forma
+00001db0: 742e 0d0a 2d20 2a2a 626f 7865 732a 2a20  t...- **boxes** 
+00001dc0: 282a 6c69 7374 2a29 3a20 4120 6c69 7374  (*list*): A list
+00001dd0: 206f 6620 626f 756e 6469 6e67 2062 6f78   of bounding box
+00001de0: 6573 2069 6e20 7468 6520 666f 726d 6174  es in the format
+00001df0: 205b 785f 6d69 6e2c 2079 5f6d 696e 2c20   [x_min, y_min, 
+00001e00: 785f 6d61 782c 2079 5f6d 6178 5d2e 0d0a  x_max, y_max]...
+00001e10: 2d20 2a2a 636c 6173 7365 735f 6964 732a  - **classes_ids*
+00001e20: 2a20 282a 6c69 7374 2a29 3a20 4120 6c69  * (*list*): A li
+00001e30: 7374 206f 6620 636c 6173 7320 4944 7320  st of class IDs 
+00001e40: 666f 7220 6561 6368 2064 6574 6563 7469  for each detecti
+00001e50: 6f6e 2e0d 0a2d 202a 2a63 6f6e 6669 6465  on...- **confide
+00001e60: 6e63 6573 2a2a 2028 2a6c 6973 742a 293a  nces** (*list*):
+00001e70: 2041 206c 6973 7420 6f66 2063 6f6e 6669   A list of confi
+00001e80: 6465 6e63 6520 7363 6f72 6573 2063 6f72  dence scores cor
+00001e90: 7265 7370 6f6e 6469 6e67 2074 6f20 6561  responding to ea
+00001ea0: 6368 2062 6f75 6e64 696e 6720 626f 782e  ch bounding box.
+00001eb0: 2044 6566 6175 6c74 2069 7320 616e 2065   Default is an e
+00001ec0: 6d70 7479 206c 6973 742e 0d0a 2d20 2a2a  mpty list...- **
+00001ed0: 636c 6173 7365 735f 6e61 6d65 732a 2a20  classes_names** 
+00001ee0: 282a 6c69 7374 2a29 3a20 4120 6c69 7374  (*list*): A list
+00001ef0: 206f 6620 636c 6173 7320 6e61 6d65 7320   of class names 
+00001f00: 636f 7272 6573 706f 6e64 696e 6720 746f  corresponding to
+00001f10: 2074 6865 2063 6c61 7373 2049 4473 2e20   the class IDs. 
+00001f20: 4465 6661 756c 7420 6973 2061 6e20 656d  Default is an em
+00001f30: 7074 7920 6c69 7374 2e0d 0a2d 202a 2a70  pty list...- **p
+00001f40: 6f6c 7967 6f6e 732a 2a20 282a 6c69 7374  olygons** (*list
+00001f50: 2a29 3a20 4120 6c69 7374 2063 6f6e 7461  *): A list conta
+00001f60: 696e 696e 6720 4e75 6d50 7920 6172 7261  ining NumPy arra
+00001f70: 7973 206f 6620 706f 6c79 676f 6e20 636f  ys of polygon co
+00001f80: 6f72 6469 6e61 7465 7320 7468 6174 2072  ordinates that r
+00001f90: 6570 7265 7365 6e74 2073 6567 6d65 6e74  epresent segment
+00001fa0: 6174 696f 6e20 6d61 736b 732e 0d0a 2d20  ation masks...- 
+00001fb0: 2a2a 6d61 736b 732a 2a20 282a 6c69 7374  **masks** (*list
+00001fc0: 2a29 3a20 4120 6c69 7374 206f 6620 6d61  *): A list of ma
+00001fd0: 736b 732e 2044 6566 6175 6c74 2069 7320  sks. Default is 
+00001fe0: 616e 2065 6d70 7479 206c 6973 742e 0d0a  an empty list...
+00001ff0: 2d20 2a2a 7365 676d 656e 742a 2a20 282a  - **segment** (*
+00002000: 626f 6f6c 2a29 3a20 5768 6574 6865 7220  bool*): Whether 
+00002010: 746f 2070 6572 666f 726d 2069 6e73 7461  to perform insta
+00002020: 6e63 6520 7365 676d 656e 7461 7469 6f6e  nce segmentation
+00002030: 2e20 4465 6661 756c 7420 6973 2046 616c  . Default is Fal
+00002040: 7365 2e0d 0a2d 202a 2a73 686f 775f 626f  se...- **show_bo
+00002050: 7865 732a 2a20 282a 626f 6f6c 2a29 3a20  xes** (*bool*): 
+00002060: 5768 6574 6865 7220 746f 2073 686f 7720  Whether to show 
+00002070: 626f 756e 6469 6e67 2062 6f78 6573 2e20  bounding boxes. 
+00002080: 4465 6661 756c 7420 6973 2054 7275 652e  Default is True.
+00002090: 0d0a 2d20 2a2a 7368 6f77 5f63 6c61 7373  ..- **show_class
 000020a0: 2a2a 2028 2a62 6f6f 6c2a 293a 2057 6865  ** (*bool*): Whe
-000020b0: 7468 6572 2074 6f20 7065 7266 6f72 6d20  ther to perform 
-000020c0: 696e 7374 616e 6365 2073 6567 6d65 6e74  instance segment
-000020d0: 6174 696f 6e2e 2044 6566 6175 6c74 2069  ation. Default i
-000020e0: 7320 4661 6c73 652e 0d0a 2d20 2a2a 7368  s False...- **sh
-000020f0: 6f77 5f62 6f78 6573 2a2a 2028 2a62 6f6f  ow_boxes** (*boo
-00002100: 6c2a 293a 2057 6865 7468 6572 2074 6f20  l*): Whether to 
-00002110: 7368 6f77 2062 6f75 6e64 696e 6720 626f  show bounding bo
-00002120: 7865 732e 2044 6566 6175 6c74 2069 7320  xes. Default is 
-00002130: 5472 7565 2e0d 0a2d 202a 2a73 686f 775f  True...- **show_
-00002140: 636c 6173 732a 2a20 282a 626f 6f6c 2a29  class** (*bool*)
-00002150: 3a20 5768 6574 6865 7220 746f 2073 686f  : Whether to sho
-00002160: 7720 636c 6173 7320 6c61 6265 6c73 2e20  w class labels. 
-00002170: 4465 6661 756c 7420 6973 2054 7275 652e  Default is True.
-00002180: 0d0a 2d20 2a2a 6669 6c6c 5f6d 6173 6b2a  ..- **fill_mask*
-00002190: 2a20 282a 626f 6f6c 2a29 3a20 5768 6574  * (*bool*): Whet
-000021a0: 6865 7220 746f 2066 696c 6c20 7468 6520  her to fill the 
-000021b0: 7365 676d 656e 7465 6420 7265 6769 6f6e  segmented region
-000021c0: 7320 7769 7468 2063 6f6c 6f72 2e20 4465  s with color. De
-000021d0: 6661 756c 7420 6973 2046 616c 7365 2e0d  fault is False..
-000021e0: 0a2d 202a 2a61 6c70 6861 2a2a 2028 2a66  .- **alpha** (*f
-000021f0: 6c6f 6174 2a29 3a20 5468 6520 7472 616e  loat*): The tran
-00002200: 7370 6172 656e 6379 206f 6620 6669 6c6c  sparency of fill
-00002210: 6564 206d 6173 6b73 2e20 4465 6661 756c  ed masks. Defaul
-00002220: 7420 6973 2030 2e33 2e0d 0a2d 202a 2a63  t is 0.3...- **c
-00002230: 6f6c 6f72 5f63 6c61 7373 5f62 6163 6b67  olor_class_backg
-00002240: 726f 756e 642a 2a20 282a 7475 706c 652a  round** (*tuple*
-00002250: 293a 2054 6865 2062 6163 6b67 726f 756e  ): The backgroun
-00002260: 6420 4247 5220 636f 6c6f 7220 666f 7220  d BGR color for 
-00002270: 636c 6173 7320 6c61 6265 6c73 2e20 4465  class labels. De
-00002280: 6661 756c 7420 6973 2028 302c 2030 2c20  fault is (0, 0, 
-00002290: 3235 3529 2028 7265 6429 2e0d 0a2d 202a  255) (red)...- *
-000022a0: 2a63 6f6c 6f72 5f63 6c61 7373 5f74 6578  *color_class_tex
-000022b0: 742a 2a20 282a 7475 706c 652a 293a 2054  t** (*tuple*): T
-000022c0: 6865 2074 6578 7420 636f 6c6f 7220 666f  he text color fo
-000022d0: 7220 636c 6173 7320 6c61 6265 6c73 2e20  r class labels. 
-000022e0: 4465 6661 756c 7420 6973 2028 3235 352c  Default is (255,
-000022f0: 2032 3535 2c20 3235 3529 2028 7768 6974   255, 255) (whit
-00002300: 6529 2e0d 0a2d 202a 2a74 6869 636b 6e65  e)...- **thickne
-00002310: 7373 2a2a 2028 2a69 6e74 2a29 3a20 5468  ss** (*int*): Th
-00002320: 6520 7468 6963 6b6e 6573 7320 6f66 2062  e thickness of b
-00002330: 6f75 6e64 696e 6720 626f 7820 616e 6420  ounding box and 
-00002340: 7465 7874 2e20 4465 6661 756c 7420 6973  text. Default is
-00002350: 2034 2e0d 0a2d 202a 2a66 6f6e 742a 2a3a   4...- **font**:
-00002360: 2054 6865 2066 6f6e 7420 7479 7065 2066   The font type f
-00002370: 6f72 2063 6c61 7373 206c 6162 656c 732e  or class labels.
-00002380: 2044 6566 6175 6c74 2069 7320 6376 322e   Default is cv2.
-00002390: 464f 4e54 5f48 4552 5348 4559 5f53 494d  FONT_HERSHEY_SIM
-000023a0: 504c 4558 2e0d 0a2d 202a 2a66 6f6e 745f  PLEX...- **font_
-000023b0: 7363 616c 652a 2a20 282a 666c 6f61 742a  scale** (*float*
-000023c0: 293a 2054 6865 2073 6361 6c65 2066 6163  ): The scale fac
-000023d0: 746f 7220 666f 7220 666f 6e74 2073 697a  tor for font siz
-000023e0: 652e 2044 6566 6175 6c74 2069 7320 312e  e. Default is 1.
-000023f0: 352e 0d0a 2d20 2a2a 6465 6c74 615f 636f  5...- **delta_co
-00002400: 6c6f 7273 2a2a 2028 2a69 6e74 2a29 3a20  lors** (*int*): 
-00002410: 5468 6520 7261 6e64 6f6d 2073 6565 6420  The random seed 
-00002420: 6f66 6673 6574 2066 6f72 2063 6f6c 6f72  offset for color
-00002430: 2076 6172 6961 7469 6f6e 2e20 4465 6661   variation. Defa
-00002440: 756c 7420 6973 2073 6565 643d 302e 0d0a  ult is seed=0...
-00002450: 2d20 2a2a 6470 692a 2a20 282a 696e 742a  - **dpi** (*int*
-00002460: 293a 2046 696e 616c 2076 6973 7561 6c69  ): Final visuali
-00002470: 7a61 7469 6f6e 2073 697a 6520 2870 6c6f  zation size (plo
-00002480: 7420 6973 2062 6967 6765 7220 7768 656e  t is bigger when
-00002490: 2064 7069 2069 7320 6869 6768 6572 292e   dpi is higher).
-000024a0: 2044 6566 6175 6c74 2069 7320 3135 302e   Default is 150.
-000024b0: 0d0a 2d20 2a2a 7261 6e64 6f6d 5f6f 626a  ..- **random_obj
-000024c0: 6563 745f 636f 6c6f 7273 2a2a 2028 2a62  ect_colors** (*b
-000024d0: 6f6f 6c2a 293a 2049 6620 7472 7565 2c20  ool*): If true, 
-000024e0: 636f 6c6f 7273 2066 6f72 2065 6163 6820  colors for each 
-000024f0: 6f62 6a65 6374 2061 7265 2073 656c 6563  object are selec
-00002500: 7465 6420 7261 6e64 6f6d 6c79 2e20 4465  ted randomly. De
-00002510: 6661 756c 7420 6973 2046 616c 7365 2e0d  fault is False..
-00002520: 0a2d 202a 2a73 686f 775f 636f 6e66 6964  .- **show_confid
-00002530: 656e 6365 732a 2a20 282a 626f 6f6c 2a29  ences** (*bool*)
-00002540: 3a20 4966 2074 7275 6520 616e 6420 7368  : If true and sh
-00002550: 6f77 5f63 6c61 7373 3d54 7275 652c 2063  ow_class=True, c
-00002560: 6f6e 6669 6465 6e63 6573 206e 6561 7220  onfidences near 
-00002570: 636c 6173 7320 6172 6520 7669 7375 616c  class are visual
-00002580: 697a 6564 2e20 4465 6661 756c 7420 6973  ized. Default is
-00002590: 2046 616c 7365 2e0d 0a2d 202a 2a61 7869   False...- **axi
-000025a0: 735f 6f66 662a 2a20 282a 626f 6f6c 2a29  s_off** (*bool*)
-000025b0: 3a20 4966 2074 7275 652c 2061 7869 7320  : If true, axis 
-000025c0: 6973 2074 7572 6e65 6420 6f66 6620 696e  is turned off in
-000025d0: 2074 6865 2066 696e 616c 2076 6973 7561   the final visua
-000025e0: 6c69 7a61 7469 6f6e 2e20 4465 6661 756c  lization. Defaul
-000025f0: 7420 6973 2054 7275 652e 0d0a 2d20 2a2a  t is True...- **
-00002600: 7368 6f77 5f63 6c61 7373 6573 5f6c 6973  show_classes_lis
-00002610: 742a 2a20 282a 6c69 7374 2a29 3a20 4966  t** (*list*): If
-00002620: 2065 6d70 7479 2c20 7669 7375 616c 697a   empty, visualiz
-00002630: 6520 616c 6c20 636c 6173 7365 732e 204f  e all classes. O
-00002640: 7468 6572 7769 7365 2c20 7669 7375 616c  therwise, visual
-00002650: 697a 6520 6f6e 6c79 2063 6c61 7373 6573  ize only classes
-00002660: 2069 6e20 7468 6520 6c69 7374 2e0d 0a2d   in the list...-
-00002670: 202a 2a72 6574 7572 6e5f 696d 6167 655f   **return_image_
-00002680: 6172 7261 792a 2a20 282a 626f 6f6c 2a29  array** (*bool*)
-00002690: 3a20 4966 2054 7275 652c 2074 6865 2066  : If True, the f
-000026a0: 756e 6374 696f 6e20 7265 7475 726e 7320  unction returns 
-000026b0: 7468 6520 696d 6167 6520 2842 4752 206e  the image (BGR n
-000026c0: 702e 6172 7261 7929 2069 6e73 7465 6164  p.array) instead
-000026d0: 206f 6620 6469 7370 6c61 7969 6e67 2069   of displaying i
-000026e0: 742e 200d 0a20 2020 2020 2020 2020 2020  t. ..           
-000026f0: 2020 2020 2020 2020 2020 2020 2020 2020                  
-00002700: 2020 2020 2020 2020 4465 6661 756c 7420          Default 
-00002710: 6973 2046 616c 7365 2e0d 0a0d 0a0d 0a45  is False.......E
-00002720: 7861 6d70 6c65 206f 6620 7573 696e 673a  xample of using:
-00002730: 0d0a 6060 6070 7974 686f 6e0d 0a66 726f  ..```python..fro
-00002740: 6d20 7061 7463 6865 645f 796f 6c6f 5f69  m patched_yolo_i
-00002750: 6e66 6572 2069 6d70 6f72 7420 7669 7375  nfer import visu
-00002760: 616c 697a 655f 7265 7375 6c74 730d 0a0d  alize_results...
-00002770: 0a23 2041 7373 756d 696e 6720 7265 7375  .# Assuming resu
-00002780: 6c74 2069 7320 616e 2069 6e73 7461 6e63  lt is an instanc
-00002790: 6520 6f66 2074 6865 2043 6f6d 6269 6e65  e of the Combine
-000027a0: 4465 7465 6374 696f 6e73 2063 6c61 7373  Detections class
-000027b0: 0d0a 7265 7375 6c74 203d 2043 6f6d 6269  ..result = Combi
-000027c0: 6e65 4465 7465 6374 696f 6e73 282e 2e2e  neDetections(...
-000027d0: 2920 0d0a 0d0a 2320 5669 7375 616c 697a  ) ....# Visualiz
-000027e0: 696e 6720 7468 6520 7265 7375 6c74 7320  ing the results 
-000027f0: 7573 696e 6720 7468 6520 7669 7375 616c  using the visual
-00002800: 697a 655f 7265 7375 6c74 7320 6675 6e63  ize_results func
-00002810: 7469 6f6e 0d0a 7669 7375 616c 697a 655f  tion..visualize_
-00002820: 7265 7375 6c74 7328 0d0a 2020 2020 696d  results(..    im
-00002830: 673d 7265 7375 6c74 2e69 6d61 6765 2c0d  g=result.image,.
-00002840: 0a20 2020 2063 6f6e 6669 6465 6e63 6573  .    confidences
-00002850: 3d72 6573 756c 742e 6669 6c74 6572 6564  =result.filtered
-00002860: 5f63 6f6e 6669 6465 6e63 6573 2c0d 0a20  _confidences,.. 
-00002870: 2020 2062 6f78 6573 3d72 6573 756c 742e     boxes=result.
-00002880: 6669 6c74 6572 6564 5f62 6f78 6573 2c0d  filtered_boxes,.
-00002890: 0a20 2020 206d 6173 6b73 3d72 6573 756c  .    masks=resul
-000028a0: 742e 6669 6c74 6572 6564 5f6d 6173 6b73  t.filtered_masks
-000028b0: 2c0d 0a20 2020 2063 6c61 7373 6573 5f69  ,..    classes_i
-000028c0: 6473 3d72 6573 756c 742e 6669 6c74 6572  ds=result.filter
-000028d0: 6564 5f63 6c61 7373 6573 5f69 642c 0d0a  ed_classes_id,..
-000028e0: 2020 2020 636c 6173 7365 735f 6e61 6d65      classes_name
-000028f0: 733d 7265 7375 6c74 2e66 696c 7465 7265  s=result.filtere
-00002900: 645f 636c 6173 7365 735f 6e61 6d65 732c  d_classes_names,
-00002910: 0d0a 2020 2020 7365 676d 656e 743d 4661  ..    segment=Fa
-00002920: 6c73 652c 0d0a 290d 0a60 6060 0d0a       lse,..)..```..
+000020b0: 7468 6572 2074 6f20 7368 6f77 2063 6c61  ther to show cla
+000020c0: 7373 206c 6162 656c 732e 2044 6566 6175  ss labels. Defau
+000020d0: 6c74 2069 7320 5472 7565 2e0d 0a2d 202a  lt is True...- *
+000020e0: 2a66 696c 6c5f 6d61 736b 2a2a 2028 2a62  *fill_mask** (*b
+000020f0: 6f6f 6c2a 293a 2057 6865 7468 6572 2074  ool*): Whether t
+00002100: 6f20 6669 6c6c 2074 6865 2073 6567 6d65  o fill the segme
+00002110: 6e74 6564 2072 6567 696f 6e73 2077 6974  nted regions wit
+00002120: 6820 636f 6c6f 722e 2044 6566 6175 6c74  h color. Default
+00002130: 2069 7320 4661 6c73 652e 0d0a 2d20 2a2a   is False...- **
+00002140: 616c 7068 612a 2a20 282a 666c 6f61 742a  alpha** (*float*
+00002150: 293a 2054 6865 2074 7261 6e73 7061 7265  ): The transpare
+00002160: 6e63 7920 6f66 2066 696c 6c65 6420 6d61  ncy of filled ma
+00002170: 736b 732e 2044 6566 6175 6c74 2069 7320  sks. Default is 
+00002180: 302e 332e 0d0a 2d20 2a2a 636f 6c6f 725f  0.3...- **color_
+00002190: 636c 6173 735f 6261 636b 6772 6f75 6e64  class_background
+000021a0: 2a2a 2028 2a74 7570 6c65 2a29 3a20 5468  ** (*tuple*): Th
+000021b0: 6520 6261 636b 6772 6f75 6e64 2042 4752  e background BGR
+000021c0: 2063 6f6c 6f72 2066 6f72 2063 6c61 7373   color for class
+000021d0: 206c 6162 656c 732e 2044 6566 6175 6c74   labels. Default
+000021e0: 2069 7320 2830 2c20 302c 2032 3535 2920   is (0, 0, 255) 
+000021f0: 2872 6564 292e 0d0a 2d20 2a2a 636f 6c6f  (red)...- **colo
+00002200: 725f 636c 6173 735f 7465 7874 2a2a 2028  r_class_text** (
+00002210: 2a74 7570 6c65 2a29 3a20 5468 6520 7465  *tuple*): The te
+00002220: 7874 2063 6f6c 6f72 2066 6f72 2063 6c61  xt color for cla
+00002230: 7373 206c 6162 656c 732e 2044 6566 6175  ss labels. Defau
+00002240: 6c74 2069 7320 2832 3535 2c20 3235 352c  lt is (255, 255,
+00002250: 2032 3535 2920 2877 6869 7465 292e 0d0a   255) (white)...
+00002260: 2d20 2a2a 7468 6963 6b6e 6573 732a 2a20  - **thickness** 
+00002270: 282a 696e 742a 293a 2054 6865 2074 6869  (*int*): The thi
+00002280: 636b 6e65 7373 206f 6620 626f 756e 6469  ckness of boundi
+00002290: 6e67 2062 6f78 2061 6e64 2074 6578 742e  ng box and text.
+000022a0: 2044 6566 6175 6c74 2069 7320 342e 0d0a   Default is 4...
+000022b0: 2d20 2a2a 666f 6e74 2a2a 3a20 5468 6520  - **font**: The 
+000022c0: 666f 6e74 2074 7970 6520 666f 7220 636c  font type for cl
+000022d0: 6173 7320 6c61 6265 6c73 2e20 4465 6661  ass labels. Defa
+000022e0: 756c 7420 6973 2063 7632 2e46 4f4e 545f  ult is cv2.FONT_
+000022f0: 4845 5253 4845 595f 5349 4d50 4c45 582e  HERSHEY_SIMPLEX.
+00002300: 0d0a 2d20 2a2a 666f 6e74 5f73 6361 6c65  ..- **font_scale
+00002310: 2a2a 2028 2a66 6c6f 6174 2a29 3a20 5468  ** (*float*): Th
+00002320: 6520 7363 616c 6520 6661 6374 6f72 2066  e scale factor f
+00002330: 6f72 2066 6f6e 7420 7369 7a65 2e20 4465  or font size. De
+00002340: 6661 756c 7420 6973 2031 2e35 2e0d 0a2d  fault is 1.5...-
+00002350: 202a 2a64 656c 7461 5f63 6f6c 6f72 732a   **delta_colors*
+00002360: 2a20 282a 696e 742a 293a 2054 6865 2072  * (*int*): The r
+00002370: 616e 646f 6d20 7365 6564 206f 6666 7365  andom seed offse
+00002380: 7420 666f 7220 636f 6c6f 7220 7661 7269  t for color vari
+00002390: 6174 696f 6e2e 2044 6566 6175 6c74 2069  ation. Default i
+000023a0: 7320 7365 6564 3d30 2e0d 0a2d 202a 2a64  s seed=0...- **d
+000023b0: 7069 2a2a 2028 2a69 6e74 2a29 3a20 4669  pi** (*int*): Fi
+000023c0: 6e61 6c20 7669 7375 616c 697a 6174 696f  nal visualizatio
+000023d0: 6e20 7369 7a65 2028 706c 6f74 2069 7320  n size (plot is 
+000023e0: 6269 6767 6572 2077 6865 6e20 6470 6920  bigger when dpi 
+000023f0: 6973 2068 6967 6865 7229 2e20 4465 6661  is higher). Defa
+00002400: 756c 7420 6973 2031 3530 2e0d 0a2d 202a  ult is 150...- *
+00002410: 2a72 616e 646f 6d5f 6f62 6a65 6374 5f63  *random_object_c
+00002420: 6f6c 6f72 732a 2a20 282a 626f 6f6c 2a29  olors** (*bool*)
+00002430: 3a20 4966 2074 7275 652c 2063 6f6c 6f72  : If true, color
+00002440: 7320 666f 7220 6561 6368 206f 626a 6563  s for each objec
+00002450: 7420 6172 6520 7365 6c65 6374 6564 2072  t are selected r
+00002460: 616e 646f 6d6c 792e 2044 6566 6175 6c74  andomly. Default
+00002470: 2069 7320 4661 6c73 652e 0d0a 2d20 2a2a   is False...- **
+00002480: 7368 6f77 5f63 6f6e 6669 6465 6e63 6573  show_confidences
+00002490: 2a2a 2028 2a62 6f6f 6c2a 293a 2049 6620  ** (*bool*): If 
+000024a0: 7472 7565 2061 6e64 2073 686f 775f 636c  true and show_cl
+000024b0: 6173 733d 5472 7565 2c20 636f 6e66 6964  ass=True, confid
+000024c0: 656e 6365 7320 6e65 6172 2063 6c61 7373  ences near class
+000024d0: 2061 7265 2076 6973 7561 6c69 7a65 642e   are visualized.
+000024e0: 2044 6566 6175 6c74 2069 7320 4661 6c73   Default is Fals
+000024f0: 652e 0d0a 2d20 2a2a 6178 6973 5f6f 6666  e...- **axis_off
+00002500: 2a2a 2028 2a62 6f6f 6c2a 293a 2049 6620  ** (*bool*): If 
+00002510: 7472 7565 2c20 6178 6973 2069 7320 7475  true, axis is tu
+00002520: 726e 6564 206f 6666 2069 6e20 7468 6520  rned off in the 
+00002530: 6669 6e61 6c20 7669 7375 616c 697a 6174  final visualizat
+00002540: 696f 6e2e 2044 6566 6175 6c74 2069 7320  ion. Default is 
+00002550: 5472 7565 2e0d 0a2d 202a 2a73 686f 775f  True...- **show_
+00002560: 636c 6173 7365 735f 6c69 7374 2a2a 2028  classes_list** (
+00002570: 2a6c 6973 742a 293a 2049 6620 656d 7074  *list*): If empt
+00002580: 792c 2076 6973 7561 6c69 7a65 2061 6c6c  y, visualize all
+00002590: 2063 6c61 7373 6573 2e20 4f74 6865 7277   classes. Otherw
+000025a0: 6973 652c 2076 6973 7561 6c69 7a65 206f  ise, visualize o
+000025b0: 6e6c 7920 636c 6173 7365 7320 696e 2074  nly classes in t
+000025c0: 6865 206c 6973 742e 0d0a 2d20 2a2a 7265  he list...- **re
+000025d0: 7475 726e 5f69 6d61 6765 5f61 7272 6179  turn_image_array
+000025e0: 2a2a 2028 2a62 6f6f 6c2a 293a 2049 6620  ** (*bool*): If 
+000025f0: 5472 7565 2c20 7468 6520 6675 6e63 7469  True, the functi
+00002600: 6f6e 2072 6574 7572 6e73 2074 6865 2069  on returns the i
+00002610: 6d61 6765 2028 4247 5220 6e70 2e61 7272  mage (BGR np.arr
+00002620: 6179 2920 696e 7374 6561 6420 6f66 2064  ay) instead of d
+00002630: 6973 706c 6179 696e 6720 6974 2e20 0d0a  isplaying it. ..
+00002640: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002650: 2020 2020 2020 2020 2020 2020 2020 2020                  
+00002660: 2020 2044 6566 6175 6c74 2069 7320 4661     Default is Fa
+00002670: 6c73 652e 0d0a 0d0a 0d0a 4578 616d 706c  lse.......Exampl
+00002680: 6520 6f66 2075 7369 6e67 3a0d 0a60 6060  e of using:..```
+00002690: 7079 7468 6f6e 0d0a 6672 6f6d 2070 6174  python..from pat
+000026a0: 6368 6564 5f79 6f6c 6f5f 696e 6665 7220  ched_yolo_infer 
+000026b0: 696d 706f 7274 2076 6973 7561 6c69 7a65  import visualize
+000026c0: 5f72 6573 756c 7473 0d0a 0d0a 2320 4173  _results....# As
+000026d0: 7375 6d69 6e67 2072 6573 756c 7420 6973  suming result is
+000026e0: 2061 6e20 696e 7374 616e 6365 206f 6620   an instance of 
+000026f0: 7468 6520 436f 6d62 696e 6544 6574 6563  the CombineDetec
+00002700: 7469 6f6e 7320 636c 6173 730d 0a72 6573  tions class..res
+00002710: 756c 7420 3d20 436f 6d62 696e 6544 6574  ult = CombineDet
+00002720: 6563 7469 6f6e 7328 2e2e 2e29 200d 0a0d  ections(...) ...
+00002730: 0a23 2056 6973 7561 6c69 7a69 6e67 2074  .# Visualizing t
+00002740: 6865 2072 6573 756c 7473 2075 7369 6e67  he results using
+00002750: 2074 6865 2076 6973 7561 6c69 7a65 5f72   the visualize_r
+00002760: 6573 756c 7473 2066 756e 6374 696f 6e0d  esults function.
+00002770: 0a76 6973 7561 6c69 7a65 5f72 6573 756c  .visualize_resul
+00002780: 7473 280d 0a20 2020 2069 6d67 3d72 6573  ts(..    img=res
+00002790: 756c 742e 696d 6167 652c 0d0a 2020 2020  ult.image,..    
+000027a0: 636f 6e66 6964 656e 6365 733d 7265 7375  confidences=resu
+000027b0: 6c74 2e66 696c 7465 7265 645f 636f 6e66  lt.filtered_conf
+000027c0: 6964 656e 6365 732c 0d0a 2020 2020 626f  idences,..    bo
+000027d0: 7865 733d 7265 7375 6c74 2e66 696c 7465  xes=result.filte
+000027e0: 7265 645f 626f 7865 732c 0d0a 2020 2020  red_boxes,..    
+000027f0: 706f 6c79 676f 6e73 3d72 6573 756c 742e  polygons=result.
+00002800: 6669 6c74 6572 6564 5f70 6f6c 7967 6f6e  filtered_polygon
+00002810: 732c 0d0a 2020 2020 636c 6173 7365 735f  s,..    classes_
+00002820: 6964 733d 7265 7375 6c74 2e66 696c 7465  ids=result.filte
+00002830: 7265 645f 636c 6173 7365 735f 6964 2c0d  red_classes_id,.
+00002840: 0a20 2020 2063 6c61 7373 6573 5f6e 616d  .    classes_nam
+00002850: 6573 3d72 6573 756c 742e 6669 6c74 6572  es=result.filter
+00002860: 6564 5f63 6c61 7373 6573 5f6e 616d 6573  ed_classes_names
+00002870: 2c0d 0a20 2020 2073 6567 6d65 6e74 3d46  ,..    segment=F
+00002880: 616c 7365 2c0d 0a29 0d0a 6060 600d 0a0d  alse,..)..```...
+00002890: 0a2d 2d2d 0d0a 2d2d 2d0d 0a0d 0a23 2320  .---..---....## 
+000028a0: 5f5f 484f 5720 544f 2049 4d50 524f 5645  __HOW TO IMPROVE
+000028b0: 2054 4845 2051 5541 4c49 5459 204f 4620   THE QUALITY OF 
+000028c0: 5448 4520 414c 474f 5249 5448 4d20 464f  THE ALGORITHM FO
+000028d0: 5220 5448 4520 5441 534b 204f 4620 494e  R THE TASK OF IN
+000028e0: 5354 414e 4345 2053 4547 4d45 4e54 4154  STANCE SEGMENTAT
+000028f0: 494f 4e3a 5f5f 0d0a 0d0a 496e 2074 6869  ION:__....In thi
+00002900: 7320 6170 7072 6f61 6368 2c20 616c 6c20  s approach, all 
+00002910: 6f70 6572 6174 696f 6e73 2075 6e64 6572  operations under
+00002920: 2074 6865 2068 6f6f 6420 6172 6520 7065   the hood are pe
+00002930: 7266 6f72 6d65 6420 6f6e 2062 696e 6172  rformed on binar
+00002940: 7920 6d61 736b 7320 6f66 2072 6563 6f67  y masks of recog
+00002950: 6e69 7a65 6420 6f62 6a65 6374 732e 2053  nized objects. S
+00002960: 746f 7269 6e67 2074 6865 7365 206d 6173  toring these mas
+00002970: 6b73 2063 6f6e 7375 6d65 7320 6120 6c6f  ks consumes a lo
+00002980: 7420 6f66 206d 656d 6f72 792c 2073 6f20  t of memory, so 
+00002990: 7468 6973 206d 6574 686f 6420 7265 7175  this method requ
+000029a0: 6972 6573 206d 6f72 6520 5241 4d20 616e  ires more RAM an
+000029b0: 6420 736c 6967 6874 6c79 206d 6f72 6520  d slightly more 
+000029c0: 7072 6f63 6573 7369 6e67 2074 696d 652e  processing time.
+000029d0: 2048 6f77 6576 6572 2c20 7468 6520 6163   However, the ac
+000029e0: 6375 7261 6379 206f 6620 7265 636f 676e  curacy of recogn
+000029f0: 6974 696f 6e20 7369 676e 6966 6963 616e  ition significan
+00002a00: 746c 7920 696d 7072 6f76 6573 2c20 7768  tly improves, wh
+00002a10: 6963 6820 6973 2065 7370 6563 6961 6c6c  ich is especiall
+00002a20: 7920 6e6f 7469 6365 6162 6c65 2069 6e20  y noticeable in 
+00002a30: 6361 7365 7320 7768 6572 6520 7468 6572  cases where ther
+00002a40: 6520 6172 6520 6d61 6e79 206f 626a 6563  e are many objec
+00002a50: 7473 206f 6620 6469 6666 6572 656e 7420  ts of different 
+00002a60: 7369 7a65 7320 616e 6420 7468 6579 2061  sizes and they a
+00002a70: 7265 2064 656e 7365 6c79 2070 6163 6b65  re densely packe
+00002a80: 642e 2054 6865 7265 666f 7265 2c20 7765  d. Therefore, we
+00002a90: 2072 6563 6f6d 6d65 6e64 2075 7369 6e67   recommend using
+00002aa0: 2074 6869 7320 6170 7072 6f61 6368 2069   this approach i
+00002ab0: 6e20 7072 6f64 7563 7469 6f6e 2069 6620  n production if 
+00002ac0: 6163 6375 7261 6379 2069 7320 696d 706f  accuracy is impo
+00002ad0: 7274 616e 7420 616e 6420 6e6f 7420 7370  rtant and not sp
+00002ae0: 6565 642c 2061 6e64 2069 6620 796f 7572  eed, and if your
+00002af0: 2063 6f6d 7075 7461 7469 6f6e 616c 2072   computational r
+00002b00: 6573 6f75 7263 6573 2061 6c6c 6f77 2073  esources allow s
+00002b10: 746f 7269 6e67 2068 756e 6472 6564 7320  toring hundreds 
+00002b20: 6f66 2062 696e 6172 7920 6d61 736b 7320  of binary masks 
+00002b30: 696e 2052 414d 2e0d 0a0d 0a54 6865 2064  in RAM.....The d
+00002b40: 6966 6665 7265 6e63 6520 696e 2074 6865  ifference in the
+00002b50: 2061 7070 726f 6163 6820 746f 2075 7369   approach to usi
+00002b60: 6e67 2074 6865 2066 756e 6374 696f 6e20  ng the function 
+00002b70: 6c69 6573 2069 6e20 7370 6563 6966 7969  lies in specifyi
+00002b80: 6e67 2074 6865 2070 6172 616d 6574 6572  ng the parameter
+00002b90: 2060 6060 6d65 6d6f 7279 5f6f 7074 696d   ```memory_optim
+00002ba0: 697a 653d 4661 6c73 6560 6060 2069 6e20  ize=False``` in 
+00002bb0: 7468 6520 6060 604d 616b 6543 726f 7073  the ```MakeCrops
+00002bc0: 4465 7465 6374 5468 656d 6060 6020 636c  DetectThem``` cl
+00002bd0: 6173 732e 0d0a 496e 2073 7563 6820 6120  ass...In such a 
+00002be0: 6361 7365 2c20 7468 6520 696e 666f 726d  case, the inform
+00002bf0: 6174 6976 6520 7661 6c75 6573 2061 6674  ative values aft
+00002c00: 6572 2070 726f 6365 7373 696e 6720 7769  er processing wi
+00002c10: 6c6c 2062 6520 7468 6520 666f 6c6c 6f77  ll be the follow
+00002c20: 696e 673a 0d0a 0d0a 312e 2069 6d67 3a20  ing:....1. img: 
+00002c30: 5468 6973 2061 7474 7269 6275 7465 2063  This attribute c
+00002c40: 6f6e 7461 696e 7320 7468 6520 6f72 6967  ontains the orig
+00002c50: 696e 616c 2069 6d61 6765 206f 6e20 7768  inal image on wh
+00002c60: 6963 6820 7468 6520 696e 6665 7265 6e63  ich the inferenc
+00002c70: 6520 7761 7320 7065 7266 6f72 6d65 642e  e was performed.
+00002c80: 2049 7420 7072 6f76 6964 6573 2063 6f6e   It provides con
+00002c90: 7465 7874 2066 6f72 2074 6865 2064 6574  text for the det
+00002ca0: 6563 7465 6420 6f62 6a65 6374 732e 0d0a  ected objects...
+00002cb0: 0d0a 322e 2063 6f6e 6669 6465 6e63 6573  ..2. confidences
+00002cc0: 3a20 5468 6973 2061 7474 7269 6275 7465  : This attribute
+00002cd0: 2068 6f6c 6473 2074 6865 2063 6f6e 6669   holds the confi
+00002ce0: 6465 6e63 6520 7363 6f72 6573 2061 7373  dence scores ass
+00002cf0: 6f63 6961 7465 6420 7769 7468 2065 6163  ociated with eac
+00002d00: 6820 6465 7465 6374 6564 206f 626a 6563  h detected objec
+00002d10: 742e 2054 6865 7365 2073 636f 7265 7320  t. These scores 
+00002d20: 696e 6469 6361 7465 2074 6865 206d 6f64  indicate the mod
+00002d30: 656c 2773 2063 6f6e 6669 6465 6e63 6520  el's confidence 
+00002d40: 6c65 7665 6c20 696e 2074 6865 2061 6363  level in the acc
+00002d50: 7572 6163 7920 6f66 2069 7473 2070 7265  uracy of its pre
+00002d60: 6469 6374 696f 6e73 2e0d 0a0d 0a33 2e20  dictions.....3. 
+00002d70: 626f 7865 733a 2054 6865 7365 2062 6f75  boxes: These bou
+00002d80: 6e64 696e 6720 626f 7865 7320 6172 6520  nding boxes are 
+00002d90: 7265 7072 6573 656e 7465 6420 6173 2061  represented as a
+00002da0: 206c 6973 7420 6f66 206c 6973 7473 2c20   list of lists, 
+00002db0: 7768 6572 6520 6561 6368 206c 6973 7420  where each list 
+00002dc0: 636f 6e74 6169 6e73 2066 6f75 7220 7661  contains four va
+00002dd0: 6c75 6573 3a20 5b78 5f6d 696e 2c20 795f  lues: [x_min, y_
+00002de0: 6d69 6e2c 2078 5f6d 6178 2c20 795f 6d61  min, x_max, y_ma
+00002df0: 785d 2e20 5468 6573 6520 7661 6c75 6573  x]. These values
+00002e00: 2063 6f72 7265 7370 6f6e 6420 746f 2074   correspond to t
+00002e10: 6865 2063 6f6f 7264 696e 6174 6573 206f  he coordinates o
+00002e20: 6620 7468 6520 746f 702d 6c65 6674 2061  f the top-left a
+00002e30: 6e64 2062 6f74 746f 6d2d 7269 6768 7420  nd bottom-right 
+00002e40: 636f 726e 6572 7320 6f66 2065 6163 6820  corners of each 
+00002e50: 626f 756e 6469 6e67 2062 6f78 2e0d 0a0d  bounding box....
+00002e60: 0a34 2e20 6d61 736b 733a 2054 6869 7320  .4. masks: This 
+00002e70: 6174 7472 6962 7574 6520 7072 6f76 6964  attribute provid
+00002e80: 6573 2073 6567 6d65 6e74 6174 696f 6e20  es segmentation 
+00002e90: 6269 6e61 7279 206d 6173 6b73 2063 6f72  binary masks cor
+00002ea0: 7265 7370 6f6e 6469 6e67 2074 6f20 7468  responding to th
+00002eb0: 6520 6465 7465 6374 6564 206f 626a 6563  e detected objec
+00002ec0: 7473 2e20 5468 6573 6520 6d61 736b 7320  ts. These masks 
+00002ed0: 6361 6e20 6265 2075 7365 6420 746f 2070  can be used to p
+00002ee0: 7265 6369 7365 6c79 2064 656c 696e 6561  recisely delinea
+00002ef0: 7465 206f 626a 6563 7420 626f 756e 6461  te object bounda
+00002f00: 7269 6573 2e0d 0a0d 0a35 2e20 636c 6173  ries.....5. clas
+00002f10: 7365 735f 6964 733a 2054 6869 7320 6174  ses_ids: This at
+00002f20: 7472 6962 7574 6520 636f 6e74 6169 6e73  tribute contains
+00002f30: 2074 6865 2063 6c61 7373 2049 4473 2061   the class IDs a
+00002f40: 7373 6967 6e65 6420 746f 2065 6163 6820  ssigned to each 
+00002f50: 6465 7465 6374 6564 206f 626a 6563 742e  detected object.
+00002f60: 2054 6865 7365 2049 4473 2063 6f72 7265   These IDs corre
+00002f70: 7370 6f6e 6420 746f 2073 7065 6369 6669  spond to specifi
+00002f80: 6320 6f62 6a65 6374 2063 6c61 7373 6573  c object classes
+00002f90: 2064 6566 696e 6564 2064 7572 696e 6720   defined during 
+00002fa0: 7468 6520 6d6f 6465 6c20 7472 6169 6e69  the model traini
+00002fb0: 6e67 2070 6861 7365 2e0d 0a0d 0a36 2e20  ng phase.....6. 
+00002fc0: 636c 6173 7365 735f 6e61 6d65 733a 2054  classes_names: T
+00002fd0: 6865 7365 2061 7265 2074 6865 2068 756d  hese are the hum
+00002fe0: 616e 2d72 6561 6461 626c 6520 6e61 6d65  an-readable name
+00002ff0: 7320 636f 7272 6573 706f 6e64 696e 6720  s corresponding 
+00003000: 746f 2074 6865 2063 6c61 7373 2049 4473  to the class IDs
+00003010: 2e20 5468 6579 2070 726f 7669 6465 2073  . They provide s
+00003020: 656d 616e 7469 6320 6c61 6265 6c73 2066  emantic labels f
+00003030: 6f72 2074 6865 2064 6574 6563 7465 6420  or the detected 
+00003040: 6f62 6a65 6374 732c 206d 616b 696e 6720  objects, making 
+00003050: 7468 6520 7265 7375 6c74 7320 6561 7369  the results easi
+00003060: 6572 2074 6f20 696e 7465 7270 7265 742e  er to interpret.
+00003070: 0d0a 0d0a 0d0a 4865 7265 2773 2068 6f77  ......Here's how
+00003080: 2079 6f75 2063 616e 206f 6274 6169 6e20   you can obtain 
+00003090: 7468 656d 3a0d 0a60 6060 7079 7468 6f6e  them:..```python
+000030a0: 0d0a 696d 673d 7265 7375 6c74 2e69 6d61  ..img=result.ima
+000030b0: 6765 0d0a 636f 6e66 6964 656e 6365 733d  ge..confidences=
+000030c0: 7265 7375 6c74 2e66 696c 7465 7265 645f  result.filtered_
+000030d0: 636f 6e66 6964 656e 6365 730d 0a62 6f78  confidences..box
+000030e0: 6573 3d72 6573 756c 742e 6669 6c74 6572  es=result.filter
+000030f0: 6564 5f62 6f78 6573 0d0a 6d61 736b 733d  ed_boxes..masks=
+00003100: 7265 7375 6c74 2e66 696c 7465 7265 645f  result.filtered_
+00003110: 6d61 736b 730d 0a63 6c61 7373 6573 5f69  masks..classes_i
+00003120: 6473 3d72 6573 756c 742e 6669 6c74 6572  ds=result.filter
+00003130: 6564 5f63 6c61 7373 6573 5f69 640d 0a63  ed_classes_id..c
+00003140: 6c61 7373 6573 5f6e 616d 6573 3d72 6573  lasses_names=res
+00003150: 756c 742e 6669 6c74 6572 6564 5f63 6c61  ult.filtered_cla
+00003160: 7373 6573 5f6e 616d 6573 0d0a 6060 600d  sses_names..```.
+00003170: 0a0d 0a0d 0a5b 6e62 5f65 7861 6d70 6c65  .....[nb_example
+00003180: 315d 3a20 6874 7470 733a 2f2f 6e62 7669  1]: https://nbvi
+00003190: 6577 6572 2e6f 7267 2f67 6974 6875 622f  ewer.org/github/
+000031a0: 4b6f 6c64 696d 3230 3031 2f59 4f4c 4f2d  Koldim2001/YOLO-
+000031b0: 5061 7463 682d 4261 7365 642d 496e 6665  Patch-Based-Infe
+000031c0: 7265 6e63 652f 626c 6f62 2f6d 6169 6e2f  rence/blob/main/
+000031d0: 6578 616d 706c 6573 2f65 7861 6d70 6c65  examples/example
+000031e0: 5f70 6174 6368 5f62 6173 6564 5f69 6e66  _patch_based_inf
+000031f0: 6572 656e 6365 2e69 7079 6e62 0d0a 5b63  erence.ipynb..[c
+00003200: 6f6c 6162 5f62 6164 6765 5d3a 2068 7474  olab_badge]: htt
+00003210: 7073 3a2f 2f63 6f6c 6162 2e72 6573 6561  ps://colab.resea
+00003220: 7263 682e 676f 6f67 6c65 2e63 6f6d 2f61  rch.google.com/a
+00003230: 7373 6574 732f 636f 6c61 622d 6261 6467  ssets/colab-badg
+00003240: 652e 7376 670d 0a5b 636f 6c61 625f 6578  e.svg..[colab_ex
+00003250: 315d 3a20 6874 7470 733a 2f2f 636f 6c61  1]: https://cola
+00003260: 622e 7265 7365 6172 6368 2e67 6f6f 676c  b.research.googl
+00003270: 652e 636f 6d2f 6472 6976 652f 3146 5561  e.com/drive/1FUa
+00003280: 6f39 3147 7942 2d6f 6a47 524e 5f6f 6b55  o91GyB-ojGRN_okU
+00003290: 7859 7966 6167 5454 3974 6473 503f 7573  xYyfagTT9tdsP?us
+000032a0: 703d 7368 6172 696e 670d 0a5b 7974 5f6c  p=sharing..[yt_l
+000032b0: 696e 6b31 5d3a 2068 7474 7073 3a2f 2f79  ink1]: https://y
+000032c0: 6f75 7475 2e62 652f 4966 624e 4f4c 524f  outu.be/IfbNOLRO
+000032d0: 796d 340d 0a5b 6e62 5f65 7861 6d70 6c65  ym4..[nb_example
+000032e0: 325d 3a20 6874 7470 733a 2f2f 6e62 7669  2]: https://nbvi
+000032f0: 6577 6572 2e6f 7267 2f67 6974 6875 622f  ewer.org/github/
+00003300: 4b6f 6c64 696d 3230 3031 2f59 4f4c 4f2d  Koldim2001/YOLO-
+00003310: 5061 7463 682d 4261 7365 642d 496e 6665  Patch-Based-Infe
+00003320: 7265 6e63 652f 626c 6f62 2f6d 6169 6e2f  rence/blob/main/
+00003330: 6578 616d 706c 6573 2f65 7861 6d70 6c65  examples/example
+00003340: 5f65 7874 7261 5f66 756e 6374 696f 6e73  _extra_functions
+00003350: 2e69 7079 6e62 0d0a 5b63 6f6c 6162 5f65  .ipynb..[colab_e
+00003360: 7832 5d3a 2068 7474 7073 3a2f 2f63 6f6c  x2]: https://col
+00003370: 6162 2e72 6573 6561 7263 682e 676f 6f67  ab.research.goog
+00003380: 6c65 2e63 6f6d 2f64 7269 7665 2f31 654d  le.com/drive/1eM
+00003390: 346f 3165 3041 5551 7253 316d 4c44 7063  4o1e0AUQrS1mLDpc
+000033a0: 674b 3948 4b49 6e57 4576 6e61 4d6e 3f75  gK9HKInWEvnaMn?u
+000033b0: 7370 3d73 6861 7269 6e67 0d0a 5b79 745f  sp=sharing..[yt_
+000033c0: 6c69 6e6b 325d 3a20 6874 7470 733a 2f2f  link2]: https://
+000033d0: 796f 7574 752e 6265 2f6e 4251 7557 6136  youtu.be/nBQuWa6
+000033e0: 3331 3838 0d0a                           3188..
```

### Comparing `patched_yolo_infer-1.1.2/patched_yolo_infer/elements/CropElement.py` & `patched_yolo_infer-1.1.3/patched_yolo_infer/elements/CropElement.py`

 * *Files 14% similar despite different names*

```diff
@@ -21,46 +21,54 @@
         self.y_start = y_start  # Coordinate of the top-left corner Y
 
         # YOLO output results:
         self.detected_conf = None  # List of confidence scores of detected objects
         self.detected_cls = None  # List of classes of detected objects
         self.detected_xyxy = None  # List of lists containing xyxy box coordinates
         self.detected_masks = None # List of np arrays containing masks in case of yolo-seg
+        self.polygons = None # List of polygons points in case of using memory optimaze
         
         # Refined coordinates according to crop position information
         self.detected_xyxy_real = None  # List of lists containing xyxy box coordinates in values from source_image_resized or source_image
         self.detected_masks_real = None # List of np arrays containing masks in case of yolo-seg with the size of source_image_resized or source_image
+        self.detected_polygons_real = None # List of polygons points in case of using memory optimaze in values from source_image_resized or source_image
 
-    def calculate_inference(self, model, imgsz=640, conf=0.35, iou=0.7, segment=False, classes_list=None):
-        # Perform inference
+    def calculate_inference(self, model, imgsz=640, conf=0.35, iou=0.7, segment=False, classes_list=None, memory_optimize=False):
 
+        # Perform inference
         predictions = model.predict(self.crop, imgsz=imgsz, conf=conf, iou=iou, classes=classes_list, verbose=False)
 
         pred = predictions[0]
 
         # Get the bounding boxes and convert them to a list of lists
         self.detected_xyxy = pred.boxes.xyxy.cpu().int().tolist()
 
         # Get the classes and convert them to a list
         self.detected_cls = pred.boxes.cls.cpu().int().tolist()
 
         # Get the mask confidence scores
         self.detected_conf = pred.boxes.conf.cpu().numpy()
 
         if segment and len(self.detected_cls) != 0:
-            # Get the masks
-            self.detected_masks = pred.masks.data.cpu().numpy()
+            if memory_optimize:
+                # Get the polygons
+                self.polygons = [mask.astype(np.uint16) for mask in pred.masks.xy]
+            else:
+                # Get the masks
+                self.detected_masks = pred.masks.data.cpu().numpy()
+            
 
     def calculate_real_values(self):
         # Calculate real values of bboxes and masks in source_image_resized
         x_start_global = self.x_start  # Global X coordinate of the crop
         y_start_global = self.y_start  # Global Y coordinate of the crop
 
         self.detected_xyxy_real = []  # List of lists with xyxy box coordinates in the values ​​of the source_image_resized
         self.detected_masks_real = []  # List of np arrays with masks in case of yolo-seg sized as source_image_resized
+        self.detected_polygons_real = [] # List of polygons in case of yolo-seg sized as source_image_resized
 
         for bbox in self.detected_xyxy:
             # Calculate real box coordinates based on the position information of the crop
             x_min, y_min, x_max, y_max = bbox
             x_min_real = x_min + x_start_global
             y_min_real = y_min + y_start_global
             x_max_real = x_max + x_start_global
@@ -77,18 +85,26 @@
                 # Place the mask in the correct position on the black image
                 black_image[y_start_global:y_start_global+self.crop.shape[0],
                             x_start_global:x_start_global+self.crop.shape[1]] = mask_resized
 
                 # Append the masked image to the list of detected_masks_real
                 self.detected_masks_real.append(black_image)
 
+        if self.polygons is not None:
+            # Adjust the mask coordinates
+            for mask in self.polygons:
+                mask[:, 0] += x_start_global  # Add x_start_global to all x coordinates
+                mask[:, 1] += y_start_global  # Add y_start_global to all y coordinates
+                self.detected_polygons_real.append(mask.astype(np.uint16))
+        
     def resize_results(self):
         # from source_image_resized to source_image sizes transformation
         resized_xyxy = []
         resized_masks = []
+        resized_polygons = []
 
         for bbox in self.detected_xyxy_real:
             # Resize bbox coordinates
             x_min, y_min, x_max, y_max = bbox
             x_min_resized = int(x_min * (self.source_image.shape[1] / self.source_image_resized.shape[1]))
             y_min_resized = int(y_min * (self.source_image.shape[0] / self.source_image_resized.shape[0]))
             x_max_resized = int(x_max * (self.source_image.shape[1] / self.source_image_resized.shape[1]))
@@ -97,9 +113,16 @@
 
         for mask in self.detected_masks_real:
             # Resize mask
             mask_resized = cv2.resize(mask, (self.source_image.shape[1], self.source_image.shape[0]),
                                     interpolation=cv2.INTER_NEAREST)
             resized_masks.append(mask_resized)
 
+
+        for polygon in self.detected_polygons_real:
+            polygon[:, 0] = (polygon[:, 0] * (self.source_image.shape[1] / self.source_image_resized.shape[1])).astype(np.uint16)
+            polygon[:, 1] = (polygon[:, 1] * (self.source_image.shape[0] / self.source_image_resized.shape[0])).astype(np.uint16)
+            resized_polygons.append(polygon)
+
         self.detected_xyxy_real = resized_xyxy
         self.detected_masks_real = resized_masks
+        self.detected_polygons_real = resized_polygons
```

### Comparing `patched_yolo_infer-1.1.2/patched_yolo_infer/functions_extra.py` & `patched_yolo_infer-1.1.3/patched_yolo_infer/functions_extra.py`

 * *Files 5% similar despite different names*

```diff
@@ -260,14 +260,15 @@
 def visualize_results(
     img,
     boxes,
     classes_ids,
     confidences=[],
     classes_names=[], 
     masks=[],
+    polygons=[],
     segment=False,
     show_boxes=True,
     show_class=True,
     fill_mask=False,
     alpha=0.3,
     color_class_background=(0, 0, 255),
     color_class_text=(255, 255, 255),
@@ -338,31 +339,46 @@
             # Assign color according to class
             random.seed(int(classes_ids[i] + delta_colors))
             color = (random.randint(0, 255), random.randint(0, 255), random.randint(0, 255))
 
         box = boxes[i]
         x_min, y_min, x_max, y_max = box
 
-        if segment:
+        if segment and len(masks) > 0:
             mask = masks[i]
             # Resize mask to the size of the original image using nearest neighbor interpolation
             mask_resized = cv2.resize(
                 np.array(mask), (img.shape[1], img.shape[0]), interpolation=cv2.INTER_NEAREST
             )
             # Add label to the mask
             mask_contours, _ = cv2.findContours(
                 mask_resized.astype(np.uint8), cv2.RETR_EXTERNAL, cv2.CHAIN_APPROX_SIMPLE
             )
             
             if fill_mask:
-                color_mask = np.zeros_like(img)
-                color_mask[mask_resized > 0] = color
-                labeled_image = cv2.addWeighted(labeled_image, 1, color_mask, alpha, 0)
+                if alpha == 1:
+                    cv2.fillPoly(labeled_image, pts=mask_contours, color=color)
+                else:
+                    color_mask = np.zeros_like(img)
+                    color_mask[mask_resized > 0] = color
+                    labeled_image = cv2.addWeighted(labeled_image, 1, color_mask, alpha, 0)
 
             cv2.drawContours(labeled_image, mask_contours, -1, color, thickness)
+        
+        elif segment and len(polygons) > 0:
+            if len(polygons[i]) > 0:
+                points = np.array(polygons[i].reshape((-1, 1, 2)), dtype=np.int32)
+                cv2.drawContours(labeled_image, [points], -1, color, thickness)
+                if fill_mask:
+                    if alpha == 1:
+                        cv2.fillPoly(labeled_image, pts=[points], color=color)
+                    else:
+                        mask_from_poly = np.zeros_like(img)
+                        color_mask_from_poly = cv2.fillPoly(mask_from_poly, pts=[points], color=color)
+                        labeled_image = cv2.addWeighted(labeled_image, 1, color_mask_from_poly, alpha, 0)
 
         # Write class label
         if show_boxes:
             cv2.rectangle(labeled_image, (x_min, y_min), (x_max, y_max), color, thickness)
 
         if show_class:
             if show_confidences:
```

### Comparing `patched_yolo_infer-1.1.2/patched_yolo_infer/nodes/CombineDetections.py` & `patched_yolo_infer-1.1.3/patched_yolo_infer/nodes/CombineDetections.py`

 * *Files 3% similar despite different names*

```diff
@@ -21,22 +21,24 @@
         image (np.ndarray): Source image in BGR.
         nms_threshold (float): IOU/IOS threshold for non-maximum suppression.
         match_metric (str): Matching metric (IOU/IOS).
         intelligent_sorter (bool): Flag indicating whether sorting by area and confidence parameter is enabled.
         detected_conf_list_full (list): List of detected confidences.
         detected_xyxy_list_full (list): List of detected bounding boxes.
         detected_masks_list_full (list): List of detected masks.
+        detected_polygons_list_full (list): List of detected polygons when memory optimization is enabled.
         detected_cls_id_list_full (list): List of detected class IDs.
         detected_cls_names_list_full (list): List of detected class names.
         filtered_indices (list): List of indices after non-maximum suppression.
         filtered_confidences (list): List of confidences after non-maximum suppression.
         filtered_boxes (list): List of bounding boxes after non-maximum suppression.
         filtered_classes_id (list): List of class IDs after non-maximum suppression.
         filtered_classes_names (list): List of class names after non-maximum suppression.
         filtered_masks (list): List of filtered (after nms) masks if segmentation is enabled.
+        filtered_polygons (list): List of filtered (after nms) polygons if segmentation and memory optimization are enabled.
     """
 
     def __init__(
         self,
         element_crops: MakeCropsDetectThem,
         nms_threshold=0.3,
         match_metric='IOS',
@@ -55,15 +57,16 @@
         self.intelligent_sorter = intelligent_sorter # enable sorting by area and confidence parameter
 
         # combinate detections of all patches
         (
             self.detected_conf_list_full,
             self.detected_xyxy_list_full,
             self.detected_masks_list_full,
-            self.detected_cls_id_list_full
+            self.detected_cls_id_list_full,
+            self.detected_polygons_list_full
         ) = self.combinate_detections(crops=self.crops)
 
         self.detected_cls_names_list_full = [
             self.class_names[value] for value in self.detected_cls_id_list_full
         ]  # make str list
 
         # Invoke the NMS for segmentation masks method for filtering predictions
@@ -89,18 +92,23 @@
 
         # Apply filtering (nms output indeces) to the prediction lists
         self.filtered_confidences = [self.detected_conf_list_full[i] for i in self.filtered_indices]
         self.filtered_boxes = [self.detected_xyxy_list_full[i] for i in self.filtered_indices]
         self.filtered_classes_id = [self.detected_cls_id_list_full[i] for i in self.filtered_indices]
         self.filtered_classes_names = [self.detected_cls_names_list_full[i] for i in self.filtered_indices]
 
-        if element_crops.segment:
+        if element_crops.segment and not element_crops.memory_optimize:
             self.filtered_masks = [self.detected_masks_list_full[i] for i in self.filtered_indices]
         else:
             self.filtered_masks = []
+        
+        if element_crops.segment and element_crops.memory_optimize:
+            self.filtered_polygons = [self.detected_polygons_list_full[i] for i in self.filtered_indices]
+        else:
+            self.filtered_polygons = []
 
     def combinate_detections(self, crops):
         """
         Combine detections from multiple crop elements.
 
         Args:
             crops (list): List of CropElement objects.
@@ -109,22 +117,24 @@
             tuple: Tuple containing lists of detected confidences, bounding boxes,
                 masks, and class IDs.
         """
         detected_conf = []
         detected_xyxy = []
         detected_masks = []
         detected_cls = []
+        detected_polygons = []
 
         for crop in crops:
             detected_conf.extend(crop.detected_conf)
             detected_xyxy.extend(crop.detected_xyxy_real)
             detected_masks.extend(crop.detected_masks_real)
             detected_cls.extend(crop.detected_cls)
+            detected_polygons.extend(crop.detected_polygons_real)
 
-        return detected_conf, detected_xyxy, detected_masks, detected_cls
+        return detected_conf, detected_xyxy, detected_masks, detected_cls, detected_polygons
 
     @staticmethod
     def intersect_over_union(mask, masks_list):
         """
         Compute Intersection over Union (IoU) scores for a given mask against a list of masks.
 
         Args:
```

### Comparing `patched_yolo_infer-1.1.2/patched_yolo_infer/nodes/MakeCropsDetectThem.py` & `patched_yolo_infer-1.1.3/patched_yolo_infer/nodes/MakeCropsDetectThem.py`

 * *Files 8% similar despite different names*

```diff
@@ -25,14 +25,15 @@
         overlap_x (int): Percentage of overlap along the x-axis.
         overlap_y (int): Percentage of overlap along the y-axis.
         show_crops (bool): Whether to visualize the cropping.
         resize_initial_size (bool): Whether to resize the results to the original 
                                     image size (ps: slow operation).
         model: Pre-initialized model object. If provided, the model will be used directly 
                    instead of loading from model_path.
+        memory_optimize (bool): Memory optimization option for segmentation (less accurate results)
 
     Attributes:
         model: YOLOv8 model loaded from the specified path.
         image (np.ndarray): Input image BGR.
         imgsz (int): Size of the input image for inference.
         conf (float): Confidence threshold for detections.
         iou (float): IoU threshold for non-maximum suppression.
@@ -44,14 +45,15 @@
         overlap_x (int): Percentage of overlap along the x-axis.
         overlap_y (int): Percentage of overlap along the y-axis.
         crops (list): List to store the CropElement objects.
         show_crops (bool): Whether to visualize the cropping.
         resize_initial_size (bool): Whether to resize the results to the original  
                                     image size (ps: slow operation).
         class_names_dict (dict): Dictionary containing class names of the YOLO model.
+        memory_optimize (bool): Memory optimization option for segmentation (less accurate results)
     """
 
     def __init__(
         self,
         image: np.ndarray,
         model_path="yolov8m.pt",
         imgsz=640,
@@ -62,14 +64,15 @@
         shape_x=700,
         shape_y=700,
         overlap_x=25,
         overlap_y=25,
         show_crops=False,
         resize_initial_size=False,
         model=None,
+        memory_optimize=True
     ) -> None:
         if model is None:
             self.model = YOLO(model_path)  # Load the model from the specified path
         else:
             self.model = model
         self.image = image  # Input image
         self.imgsz = imgsz  # Size of the input image for inference
@@ -80,14 +83,15 @@
         self.shape_x = shape_x  # Size of the crop in the x-coordinate
         self.shape_y = shape_y  # Size of the crop in the y-coordinate
         self.overlap_x = overlap_x  # Percentage of overlap along the x-axis
         self.overlap_y = overlap_y  # Percentage of overlap along the y-axis
         self.crops = []  # List to store the CropElement objects
         self.show_crops = show_crops  # Whether to visualize the cropping
         self.resize_initial_size = resize_initial_size  # slow operation !
+        self.memory_optimize = memory_optimize # memory opimization option for segmentation
         self.class_names_dict = self.model.names
 
         self.crops = self.get_crops_xy(
             self.image,
             shape_x=self.shape_x,
             shape_y=self.shape_y,
             overlap_x=self.overlap_x,
@@ -191,11 +195,12 @@
             crop.calculate_inference(
                 self.model,
                 imgsz=self.imgsz,
                 conf=self.conf,
                 iou=self.iou,
                 segment=self.segment,
                 classes_list=self.classes_list,
+                memory_optimize=self.memory_optimize
             )
             crop.calculate_real_values()
             if self.resize_initial_size:
                 crop.resize_results()
```

### Comparing `patched_yolo_infer-1.1.2/patched_yolo_infer.egg-info/PKG-INFO` & `patched_yolo_infer-1.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: patched-yolo-infer
-Version: 1.1.2
+Name: patched_yolo_infer
+Version: 1.1.3
 Summary: YOLO-Patch-Based-Inference for detection/segmentation of small objects in images.
 Home-page: https://github.com/Koldim2001/YOLO-Patch-Based-Inference
 Author: Koldim2001
 License: AGPL-3.0 license
 Keywords: python,yolov8,yolov9,rtdetr,sam,object detection,instance segmentation,patch-based inference,small object detection,yolov8-seg,image patching,yolo visualization,slice-based inference,slicing inference,inference visualization,patchify,ultralytics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -46,28 +46,29 @@
 
 __Check this Colab examples:__
                          
 YOLO-Patch-Based-Inference Example - [Open in Colab](https://colab.research.google.com/drive/1FUao91GyB-ojGRN_okUxYyfagTT9tdsP?usp=sharing)
 
 Example of using various functions for visualizing basic YOLOv8/v9 inference results and handling overlapping crops - [Open in Colab](https://colab.research.google.com/drive/1eM4o1e0AUQrS1mLDpcgK9HKInWEvnaMn?usp=sharing)
 
+
 ## Usage
 
 ### 1. Patch-Based-Inference
-To carry out patch-based inference of YOLO models using our library, you need to follow a sequential procedure. First, you create an instance of the MakeCropsDetectThem class, providing all desired parameters related to YOLO inference and the patch segmentation principle.<br/> Subsequently, you pass the obtained object of this class to CombineDetections, which facilitates the consolidation of all predictions from each overlapping crop, followed by intelligent suppression of duplicates. <br/>Upon completion, you receive the result, from which you can extract the desired outcome of frame processing.
+To carry out patch-based inference of YOLO models using our library, you need to follow a sequential procedure. First, you create an instance of the `MakeCropsDetectThem` class, providing all desired parameters related to YOLO inference and the patch segmentation principle.<br/> Subsequently, you pass the obtained object of this class to `CombineDetections`, which facilitates the consolidation of all predictions from each overlapping crop, followed by intelligent suppression of duplicates. <br/>Upon completion, you receive the result, from which you can extract the desired outcome of frame processing.
 
 The output obtained from the process includes several attributes that can be leveraged for further analysis or visualization:
 
 1. img: This attribute contains the original image on which the inference was performed. It provides context for the detected objects.
 
 2. confidences: This attribute holds the confidence scores associated with each detected object. These scores indicate the model's confidence level in the accuracy of its predictions.
 
 3. boxes: These bounding boxes are represented as a list of lists, where each list contains four values: [x_min, y_min, x_max, y_max]. These values correspond to the coordinates of the top-left and bottom-right corners of each bounding box.
 
-4. masks: If available, this attribute provides segmentation masks corresponding to the detected objects. These masks can be used to precisely delineate object boundaries.
+4. polygons: If available, this attribute provides a list containing NumPy arrays of polygon coordinates that represent segmentation masks corresponding to the detected objects. These polygons can be utilized to accurately outline the boundaries of each object.
 
 5. classes_ids: This attribute contains the class IDs assigned to each detected object. These IDs correspond to specific object classes defined during the model training phase.
 
 6. classes_names: These are the human-readable names corresponding to the class IDs. They provide semantic labels for the detected objects, making the results easier to interpret.
 
 ```python
 import cv2
@@ -91,15 +92,15 @@
 )
 result = CombineDetections(element_crops, nms_threshold=0.25, match_metric='IOS')  
 
 # Final Results:
 img=result.image
 confidences=result.filtered_confidences
 boxes=result.filtered_boxes
-masks=result.filtered_masks
+polygons=result.filtered_polygons
 classes_ids=result.filtered_classes_id
 classes_names=result.filtered_classes_names
 ```
 
 #### Explanation of possible input arguments:
 
 **MakeCropsDetectThem**
@@ -115,33 +116,38 @@
 - **segment** (*bool*): Whether to perform segmentation (YOLOv8-seg).
 - **shape_x** (*int*): Size of the crop in the x-coordinate.
 - **shape_y** (*int*): Size of the crop in the y-coordinate.
 - **overlap_x** (*float*): Percentage of overlap along the x-axis.
 - **overlap_y** (*float*): Percentage of overlap along the y-axis.
 - **show_crops** (*bool*): Whether to visualize the cropping.
 - **resize_initial_size** (*bool*): Whether to resize the results to the original image size (ps: slow operation).
+- **memory_optimize** (*bool*): Memory optimization option for segmentation (less accurate results when enabled).
 
 **CombineDetections**
 Class implementing combining masks/boxes from multiple crops + NMS (Non-Maximum Suppression).\
 **Args:**
 - **element_crops** (*MakeCropsDetectThem*): Object containing crop information.
 - **nms_threshold** (*float*): IoU/IoS threshold for non-maximum suppression.
 - **match_metric** (*str*): Matching metric, either 'IOU' or 'IOS'.
-- **intelligent_sorter** (*bool*): Enable sorting by area and rounded confidence parameter. If False, sorting will be done only by confidence (usual nms). (Dafault is True)
+- **intelligent_sorter** (*bool*): Enable sorting by area and rounded confidence parameter. 
+            If False, sorting will be done only by confidence (usual nms). (Dafault is True)
+
+
 
 ---
 ### 2. Custom inference visualization:
 Visualizes custom results of object detection or segmentation on an image.
 
 **Args:**
 - **img** (*numpy.ndarray*): The input image in BGR format.
 - **boxes** (*list*): A list of bounding boxes in the format [x_min, y_min, x_max, y_max].
 - **classes_ids** (*list*): A list of class IDs for each detection.
 - **confidences** (*list*): A list of confidence scores corresponding to each bounding box. Default is an empty list.
 - **classes_names** (*list*): A list of class names corresponding to the class IDs. Default is an empty list.
+- **polygons** (*list*): A list containing NumPy arrays of polygon coordinates that represent segmentation masks.
 - **masks** (*list*): A list of masks. Default is an empty list.
 - **segment** (*bool*): Whether to perform instance segmentation. Default is False.
 - **show_boxes** (*bool*): Whether to show bounding boxes. Default is True.
 - **show_class** (*bool*): Whether to show class labels. Default is True.
 - **fill_mask** (*bool*): Whether to fill the segmented regions with color. Default is False.
 - **alpha** (*float*): The transparency of filled masks. Default is 0.3.
 - **color_class_background** (*tuple*): The background BGR color for class labels. Default is (0, 0, 255) (red).
@@ -151,28 +157,61 @@
 - **font_scale** (*float*): The scale factor for font size. Default is 1.5.
 - **delta_colors** (*int*): The random seed offset for color variation. Default is seed=0.
 - **dpi** (*int*): Final visualization size (plot is bigger when dpi is higher). Default is 150.
 - **random_object_colors** (*bool*): If true, colors for each object are selected randomly. Default is False.
 - **show_confidences** (*bool*): If true and show_class=True, confidences near class are visualized. Default is False.
 - **axis_off** (*bool*): If true, axis is turned off in the final visualization. Default is True.
 - **show_classes_list** (*list*): If empty, visualize all classes. Otherwise, visualize only classes in the list.
-- **return_image_array** (*bool*): If True, the function returns the image (BGR np.array) instead of displaying it. Default is False.
+- **return_image_array** (*bool*): If True, the function returns the image (BGR np.array) instead of displaying it. 
+                                   Default is False.
 
 
 Example of using:
 ```python
 from patched_yolo_infer import visualize_results
 
 # Assuming result is an instance of the CombineDetections class
 result = CombineDetections(...) 
 
 # Visualizing the results using the visualize_results function
 visualize_results(
     img=result.image,
     confidences=result.filtered_confidences,
     boxes=result.filtered_boxes,
-    masks=result.filtered_masks,
+    polygons=result.filtered_polygons,
     classes_ids=result.filtered_classes_id,
     classes_names=result.filtered_classes_names,
     segment=False,
 )
+```
+
+---
+
+## __HOW TO IMPROVE THE QUALITY OF THE ALGORITHM FOR THE TASK OF INSTANCE SEGMENTATION:__
+
+In this approach, all operations under the hood are performed on binary masks of recognized objects. Storing these masks consumes a lot of memory, so this method requires more RAM and slightly more processing time. However, the accuracy of recognition significantly improves, which is especially noticeable in cases where there are many objects of different sizes and they are densely packed. Therefore, we recommend using this approach in production if accuracy is important and not speed, and if your computational resources allow storing hundreds of binary masks in RAM.
+
+The difference in the approach to using the function lies in specifying the parameter ```memory_optimize=False``` in the ```MakeCropsDetectThem``` class.
+In such a case, the informative values after processing will be the following:
+
+1. img: This attribute contains the original image on which the inference was performed. It provides context for the detected objects.
+
+2. confidences: This attribute holds the confidence scores associated with each detected object. These scores indicate the model's confidence level in the accuracy of its predictions.
+
+3. boxes: These bounding boxes are represented as a list of lists, where each list contains four values: [x_min, y_min, x_max, y_max]. These values correspond to the coordinates of the top-left and bottom-right corners of each bounding box.
+
+4. masks: This attribute provides segmentation binary masks corresponding to the detected objects. These masks can be used to precisely delineate object boundaries.
+
+5. classes_ids: This attribute contains the class IDs assigned to each detected object. These IDs correspond to specific object classes defined during the model training phase.
+
+6. classes_names: These are the human-readable names corresponding to the class IDs. They provide semantic labels for the detected objects, making the results easier to interpret.
+
+
+Here's how you can obtain them:
+```python
+img=result.image
+confidences=result.filtered_confidences
+boxes=result.filtered_boxes
+masks=result.filtered_masks
+classes_ids=result.filtered_classes_id
+classes_names=result.filtered_classes_names
 ```
```

### Comparing `patched_yolo_infer-1.1.2/patched_yolo_infer.egg-info/SOURCES.txt` & `patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `patched_yolo_infer-1.1.2/setup.py` & `patched_yolo_infer-1.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 pwd = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(pwd, "patched_yolo_infer/README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
-VERSION = '1.1.2'
+VERSION = '1.1.3'
 DESCRIPTION = '''YOLO-Patch-Based-Inference for detection/segmentation of small objects in images.'''
 
 setup(
     name="patched_yolo_infer",
     version=VERSION,
     license="AGPL-3.0 license",
     url="https://github.com/Koldim2001/YOLO-Patch-Based-Inference",
```

