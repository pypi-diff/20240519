# Comparing `tmp/patched_yolo_infer-1.1.3.tar.gz` & `tmp/patched_yolo_infer-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "patched_yolo_infer-1.1.3.tar", last modified: Sun May 19 17:44:33 2024, max compression
+gzip compressed data, was "patched_yolo_infer-1.2.0.tar", last modified: Sun May 19 20:49:44 2024, max compression
```

## Comparing `patched_yolo_infer-1.1.3.tar` & `patched_yolo_infer-1.2.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxrwx   0        0        0        0 2024-05-19 17:44:33.910807 patched_yolo_infer-1.1.3/
--rw-rw-rw-   0        0        0    35184 2024-03-29 07:50:02.000000 patched_yolo_infer-1.1.3/LICENSE.txt
--rw-rw-rw-   0        0        0    12908 2024-05-19 17:44:33.910807 patched_yolo_infer-1.1.3/PKG-INFO
--rw-rw-rw-   0        0        0    13286 2024-05-19 17:40:50.000000 patched_yolo_infer-1.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-19 17:44:33.893389 patched_yolo_infer-1.1.3/patched_yolo_infer/
--rw-rw-rw-   0        0        0      262 2024-03-14 20:52:00.000000 patched_yolo_infer-1.1.3/patched_yolo_infer/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 17:44:33.902874 patched_yolo_infer-1.1.3/patched_yolo_infer/elements/
--rw-rw-rw-   0        0        0     6841 2024-05-19 16:18:07.000000 patched_yolo_infer-1.1.3/patched_yolo_infer/elements/CropElement.py
--rw-rw-rw-   0        0        0        0 2024-03-14 21:13:30.000000 patched_yolo_infer-1.1.3/patched_yolo_infer/elements/__init__.py
--rw-rw-rw-   0        0        0    16850 2024-05-19 14:49:58.000000 patched_yolo_infer-1.1.3/patched_yolo_infer/functions_extra.py
-drwxrwxrwx   0        0        0        0 2024-05-19 17:44:33.909833 patched_yolo_infer-1.1.3/patched_yolo_infer/nodes/
--rw-rw-rw-   0        0        0    13486 2024-05-19 07:54:44.000000 patched_yolo_infer-1.1.3/patched_yolo_infer/nodes/CombineDetections.py
--rw-rw-rw-   0        0        0     8716 2024-05-19 16:09:46.000000 patched_yolo_infer-1.1.3/patched_yolo_infer/nodes/MakeCropsDetectThem.py
--rw-rw-rw-   0        0        0        0 2024-03-14 21:13:13.000000 patched_yolo_infer-1.1.3/patched_yolo_infer/nodes/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-19 17:44:33.902874 patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/
--rw-rw-rw-   0        0        0    12908 2024-05-19 17:44:33.000000 patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      532 2024-05-19 17:44:33.000000 patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-19 17:44:33.000000 patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       49 2024-05-19 17:44:33.000000 patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2024-05-19 17:44:33.000000 patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-19 17:44:33.912316 patched_yolo_infer-1.1.3/setup.cfg
--rw-rw-rw-   0        0        0     1695 2024-05-19 17:43:52.000000 patched_yolo_infer-1.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 20:49:44.478240 patched_yolo_infer-1.2.0/
+-rw-rw-rw-   0        0        0    35184 2024-03-29 07:50:02.000000 patched_yolo_infer-1.2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0    12855 2024-05-19 20:49:44.478240 patched_yolo_infer-1.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0    17797 2024-05-19 20:12:36.000000 patched_yolo_infer-1.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 20:49:44.456036 patched_yolo_infer-1.2.0/patched_yolo_infer/
+-rw-rw-rw-   0        0        0      262 2024-03-14 20:52:00.000000 patched_yolo_infer-1.2.0/patched_yolo_infer/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 20:49:44.475282 patched_yolo_infer-1.2.0/patched_yolo_infer/elements/
+-rw-rw-rw-   0        0        0     6841 2024-05-19 16:18:07.000000 patched_yolo_infer-1.2.0/patched_yolo_infer/elements/CropElement.py
+-rw-rw-rw-   0        0        0        0 2024-03-14 21:13:30.000000 patched_yolo_infer-1.2.0/patched_yolo_infer/elements/__init__.py
+-rw-rw-rw-   0        0        0    16850 2024-05-19 14:49:58.000000 patched_yolo_infer-1.2.0/patched_yolo_infer/functions_extra.py
+drwxrwxrwx   0        0        0        0 2024-05-19 20:49:44.478030 patched_yolo_infer-1.2.0/patched_yolo_infer/nodes/
+-rw-rw-rw-   0        0        0    13547 2024-05-19 17:57:19.000000 patched_yolo_infer-1.2.0/patched_yolo_infer/nodes/CombineDetections.py
+-rw-rw-rw-   0        0        0     8716 2024-05-19 17:59:53.000000 patched_yolo_infer-1.2.0/patched_yolo_infer/nodes/MakeCropsDetectThem.py
+-rw-rw-rw-   0        0        0        0 2024-03-14 21:13:13.000000 patched_yolo_infer-1.2.0/patched_yolo_infer/nodes/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-19 20:49:44.473633 patched_yolo_infer-1.2.0/patched_yolo_infer.egg-info/
+-rw-rw-rw-   0        0        0    12855 2024-05-19 20:49:44.000000 patched_yolo_infer-1.2.0/patched_yolo_infer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2024-05-19 20:49:44.000000 patched_yolo_infer-1.2.0/patched_yolo_infer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 20:49:44.000000 patched_yolo_infer-1.2.0/patched_yolo_infer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       49 2024-05-19 20:49:44.000000 patched_yolo_infer-1.2.0/patched_yolo_infer.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-05-19 20:49:44.000000 patched_yolo_infer-1.2.0/patched_yolo_infer.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-19 20:49:44.479934 patched_yolo_infer-1.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1695 2024-05-19 20:12:47.000000 patched_yolo_infer-1.2.0/setup.py
```

### Comparing `patched_yolo_infer-1.1.3/LICENSE.txt` & `patched_yolo_infer-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `patched_yolo_infer-1.1.3/PKG-INFO` & `patched_yolo_infer-1.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: patched_yolo_infer
-Version: 1.1.3
+Version: 1.2.0
 Summary: YOLO-Patch-Based-Inference for detection/segmentation of small objects in images.
 Home-page: https://github.com/Koldim2001/YOLO-Patch-Based-Inference
 Author: Koldim2001
 License: AGPL-3.0 license
 Keywords: python,yolov8,yolov9,rtdetr,sam,object detection,instance segmentation,patch-based inference,small object detection,yolov8-seg,image patching,yolo visualization,slice-based inference,slicing inference,inference visualization,patchify,ultralytics
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -124,16 +124,15 @@
 
 **CombineDetections**
 Class implementing combining masks/boxes from multiple crops + NMS (Non-Maximum Suppression).\
 **Args:**
 - **element_crops** (*MakeCropsDetectThem*): Object containing crop information.
 - **nms_threshold** (*float*): IoU/IoS threshold for non-maximum suppression.
 - **match_metric** (*str*): Matching metric, either 'IOU' or 'IOS'.
-- **intelligent_sorter** (*bool*): Enable sorting by area and rounded confidence parameter. 
-            If False, sorting will be done only by confidence (usual nms). (Dafault is True)
+- **intelligent_sorter** (*bool*): Enable sorting by area and rounded confidence parameter. If False, sorting will be done only by confidence (usual nms). (Dafault is True)
 
 
 
 ---
 ### 2. Custom inference visualization:
 Visualizes custom results of object detection or segmentation on an image.
 
@@ -157,16 +156,15 @@
 - **font_scale** (*float*): The scale factor for font size. Default is 1.5.
 - **delta_colors** (*int*): The random seed offset for color variation. Default is seed=0.
 - **dpi** (*int*): Final visualization size (plot is bigger when dpi is higher). Default is 150.
 - **random_object_colors** (*bool*): If true, colors for each object are selected randomly. Default is False.
 - **show_confidences** (*bool*): If true and show_class=True, confidences near class are visualized. Default is False.
 - **axis_off** (*bool*): If true, axis is turned off in the final visualization. Default is True.
 - **show_classes_list** (*list*): If empty, visualize all classes. Otherwise, visualize only classes in the list.
-- **return_image_array** (*bool*): If True, the function returns the image (BGR np.array) instead of displaying it. 
-                                   Default is False.
+- **return_image_array** (*bool*): If True, the function returns the image (BGR np.array) instead of displaying it. Default is False.
 
 
 Example of using:
 ```python
 from patched_yolo_infer import visualize_results
 
 # Assuming result is an instance of the CombineDetections class
```

### Comparing `patched_yolo_infer-1.1.3/README.md` & `patched_yolo_infer-1.2.0/patched_yolo_infer.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,222 +1,215 @@
-# YOLO-Patch-Based-Inference
-
-This library facilitates various visualizations of inference results from ultralytics segmentation/detection models, including cropping with overlays, as well as **a patch-based inference algorithm enabling the detection of small objects in images**. It caters to both object detection and instance segmentation tasks.
-
-**Model Support**: The library offers support for multiple ultralytics deep learning models, such as YOLOv8, YOLOv8-seg, YOLOv9, YOLOv9-seg, FastSAM, and RTDETR. Users can select from pre-trained options or utilize custom-trained models to best meet their task requirements.
-
-## Installation
-You can install the library via pip:
-
-```bash
-pip install patched_yolo_infer
-```
-
-[![PyPI Version](https://img.shields.io/pypi/v/patched-yolo-infer.svg)](https://pypi.org/project/patched-yolo-infer/) - Click here to visit the PyPI page for `patched-yolo-infer`, where you can find more information and documentation.
-
-Note: If CUDA support is available, it's recommended to pre-install PyTorch with CUDA support before installing the library. Otherwise, the CPU version will be installed by default.
-
----
-
-</details>
-
-## Notebooks
-
-Interactive notebooks are provided to showcase the functionality of the library. These notebooks cover batch-inference procedures for detection, instance segmentation, inference custom visualization, and more. Each notebook is paired with a tutorial on YouTube, making it easy to learn and implement features.
-
-
-
-| **Topic** | **Notebook** | **YouTube** |
-| ----- | -------- | ------- |
-| [Patch-Based-Inference Example][nb_example1] | [![Open In Colab][colab_badge]][colab_ex1] |<div align="center">[<img width=30% alt="Youtube Video" src=https://raw.githubusercontent.com/ultralytics/assets/main/social/logo-social-youtube-rect.png>][yt_link1] |
-| [Example of utilizing a function to visualize basic Ultralytics model inference results and managing overlapping image crops][nb_example2] | [![Open In Colab][colab_badge]][colab_ex2] | <div align="center">[<img width=30% alt="Youtube Video" src=https://raw.githubusercontent.com/ultralytics/assets/main/social/logo-social-youtube-rect.png>][yt_link2] |
-
-
-For Russian users, there is a detailed video presentation of this project. YouTube video in Russian is available at this [__link__](https://youtu.be/ihch6pIZtQg).
-
----
-## Examples:
-
-#### Detection example:
-<img src="readme_content/getection.gif" alt="Detection" width="800">
-
-#### Instance Segmentation example 1:
-<img src="readme_content/segment_1.gif" alt="Segmentation" width="800">
-
-#### Instance Segmentation example 2:
-<img src="readme_content/segment_2.gif" alt="Segmentation" width="800">
-
----
-## Usage
-
-### 1. Patch-Based-Inference
-To carry out patch-based inference of YOLO models using our library, you need to follow a sequential procedure. First, you create an instance of the `MakeCropsDetectThem` class, providing all desired parameters related to YOLO inference and the patch segmentation principle.<br/> Subsequently, you pass the obtained object of this class to `CombineDetections`, which facilitates the consolidation of all predictions from each overlapping crop, followed by intelligent suppression of duplicates. <br/>Upon completion, you receive the result, from which you can extract the desired outcome of frame processing.
-
-The output obtained from the process includes several attributes that can be leveraged for further analysis or visualization:
-
-1. img: This attribute contains the original image on which the inference was performed. It provides context for the detected objects.
-
-2. confidences: This attribute holds the confidence scores associated with each detected object. These scores indicate the model's confidence level in the accuracy of its predictions.
-
-3. boxes: These bounding boxes are represented as a list of lists, where each list contains four values: [x_min, y_min, x_max, y_max]. These values correspond to the coordinates of the top-left and bottom-right corners of each bounding box.
-
-4. polygons: If available, this attribute provides a list containing NumPy arrays of polygon coordinates that represent segmentation masks corresponding to the detected objects. These polygons can be utilized to accurately outline the boundaries of each object.
-
-5. classes_ids: This attribute contains the class IDs assigned to each detected object. These IDs correspond to specific object classes defined during the model training phase.
-
-6. classes_names: These are the human-readable names corresponding to the class IDs. They provide semantic labels for the detected objects, making the results easier to interpret.
-
-```python
-import cv2
-from patched_yolo_infer import MakeCropsDetectThem, CombineDetections
-
-# Load the image 
-img_path = 'test_image.jpg'
-img = cv2.imread(img_path)
-
-element_crops = MakeCropsDetectThem(
-    image=img,
-    model_path="yolov8m.pt",
-    segment=False,
-    shape_x=640,
-    shape_y=640,
-    overlap_x=50,
-    overlap_y=50,
-    conf=0.5,
-    iou=0.7,
-    resize_initial_size=True,
-)
-result = CombineDetections(element_crops, nms_threshold=0.25, match_metric='IOS')  
-
-# Final Results:
-img=result.image
-confidences=result.filtered_confidences
-boxes=result.filtered_boxes
-polygons=result.filtered_polygons
-classes_ids=result.filtered_classes_id
-classes_names=result.filtered_classes_names
-```
-
-#### Explanation of possible input arguments:
-
-**MakeCropsDetectThem**
-Class implementing cropping and passing crops through a neural network for detection/segmentation.\
-**Args:**
-- **image** (*np.ndarray*): Input image BGR.
-- **model_path** (*str*): Path to the YOLO model.
-- **model** (*ultralytics model*) Pre-initialized model object. If provided, the model will be used directly instead of loading from model_path.
-- **imgsz** (*int*): Size of the input image for inference YOLO.
-- **conf** (*float*): Confidence threshold for detections YOLO.
-- **iou** (*float*): IoU threshold for non-maximum suppression YOLOv8 of single crop.
-- **classes_list** (*List[int] or None*): List of classes to filter detections. If None, all classes are considered. Defaults to None.
-- **segment** (*bool*): Whether to perform segmentation (YOLOv8-seg).
-- **shape_x** (*int*): Size of the crop in the x-coordinate.
-- **shape_y** (*int*): Size of the crop in the y-coordinate.
-- **overlap_x** (*float*): Percentage of overlap along the x-axis.
-- **overlap_y** (*float*): Percentage of overlap along the y-axis.
-- **show_crops** (*bool*): Whether to visualize the cropping.
-- **resize_initial_size** (*bool*): Whether to resize the results to the original image size (ps: slow operation).
-- **memory_optimize** (*bool*): Memory optimization option for segmentation (less accurate results when enabled).
-
-**CombineDetections**
-Class implementing combining masks/boxes from multiple crops + NMS (Non-Maximum Suppression).\
-**Args:**
-- **element_crops** (*MakeCropsDetectThem*): Object containing crop information.
-- **nms_threshold** (*float*): IoU/IoS threshold for non-maximum suppression.
-- **match_metric** (*str*): Matching metric, either 'IOU' or 'IOS'.
-- **intelligent_sorter** (*bool*): Enable sorting by area and rounded confidence parameter. 
-            If False, sorting will be done only by confidence (usual nms). (Dafault is True)
-
-
-
----
-### 2. Custom inference visualization:
-Visualizes custom results of object detection or segmentation on an image.
-
-**Args:**
-- **img** (*numpy.ndarray*): The input image in BGR format.
-- **boxes** (*list*): A list of bounding boxes in the format [x_min, y_min, x_max, y_max].
-- **classes_ids** (*list*): A list of class IDs for each detection.
-- **confidences** (*list*): A list of confidence scores corresponding to each bounding box. Default is an empty list.
-- **classes_names** (*list*): A list of class names corresponding to the class IDs. Default is an empty list.
-- **polygons** (*list*): A list containing NumPy arrays of polygon coordinates that represent segmentation masks.
-- **masks** (*list*): A list of masks. Default is an empty list.
-- **segment** (*bool*): Whether to perform instance segmentation. Default is False.
-- **show_boxes** (*bool*): Whether to show bounding boxes. Default is True.
-- **show_class** (*bool*): Whether to show class labels. Default is True.
-- **fill_mask** (*bool*): Whether to fill the segmented regions with color. Default is False.
-- **alpha** (*float*): The transparency of filled masks. Default is 0.3.
-- **color_class_background** (*tuple*): The background BGR color for class labels. Default is (0, 0, 255) (red).
-- **color_class_text** (*tuple*): The text color for class labels. Default is (255, 255, 255) (white).
-- **thickness** (*int*): The thickness of bounding box and text. Default is 4.
-- **font**: The font type for class labels. Default is cv2.FONT_HERSHEY_SIMPLEX.
-- **font_scale** (*float*): The scale factor for font size. Default is 1.5.
-- **delta_colors** (*int*): The random seed offset for color variation. Default is seed=0.
-- **dpi** (*int*): Final visualization size (plot is bigger when dpi is higher). Default is 150.
-- **random_object_colors** (*bool*): If true, colors for each object are selected randomly. Default is False.
-- **show_confidences** (*bool*): If true and show_class=True, confidences near class are visualized. Default is False.
-- **axis_off** (*bool*): If true, axis is turned off in the final visualization. Default is True.
-- **show_classes_list** (*list*): If empty, visualize all classes. Otherwise, visualize only classes in the list.
-- **return_image_array** (*bool*): If True, the function returns the image (BGR np.array) instead of displaying it. 
-                                   Default is False.
-
-
-Example of using:
-```python
-from patched_yolo_infer import visualize_results
-
-# Assuming result is an instance of the CombineDetections class
-result = CombineDetections(...) 
-
-# Visualizing the results using the visualize_results function
-visualize_results(
-    img=result.image,
-    confidences=result.filtered_confidences,
-    boxes=result.filtered_boxes,
-    polygons=result.filtered_polygons,
-    classes_ids=result.filtered_classes_id,
-    classes_names=result.filtered_classes_names,
-    segment=False,
-)
+Metadata-Version: 2.1
+Name: patched-yolo-infer
+Version: 1.2.0
+Summary: YOLO-Patch-Based-Inference for detection/segmentation of small objects in images.
+Home-page: https://github.com/Koldim2001/YOLO-Patch-Based-Inference
+Author: Koldim2001
+License: AGPL-3.0 license
+Keywords: python,yolov8,yolov9,rtdetr,sam,object detection,instance segmentation,patch-based inference,small object detection,yolov8-seg,image patching,yolo visualization,slice-based inference,slicing inference,inference visualization,patchify,ultralytics
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: numpy
+Requires-Dist: opencv-python
+Requires-Dist: matplotlib
+Requires-Dist: torch
+Requires-Dist: ultralytics
+
+
+# YOLO-Patch-Based-Inference
+
+This library facilitates various visualizations of inference results from ultralytics segmentation/detection models, including cropping with overlays, as well as **a patch-based inference algorithm enabling the detection/instance segmentation of small objects in images**. 
+
+**Model Support**: The library offers support for multiple ultralytics deep learning models, such as YOLOv8, YOLOv9, SAM, and RTDETR. Users can select from pre-trained options or utilize custom-trained models to best meet their task requirements.
+
+
+## Installation
+You can install the library via pip:
+
+```bash
+pip install patched_yolo_infer
+```
+
+Note: If CUDA support is available, it's recommended to pre-install PyTorch with CUDA support before installing the library. Otherwise, the CPU version will be installed by default.
+
+
+</details>
+
+## Notebooks
+
+Interactive notebooks are provided to showcase the functionality of the library. These notebooks cover batch inference procedures for detection, instance segmentation, custom visualization of inference, and more. Each notebook is paired with a tutorial on YouTube, making it easy to learn and implement features. Check the GitHub page for the current links to the videos: https://github.com/Koldim2001/YOLO-Patch-Based-Inference
+
+__Check this Colab examples:__
+                         
+YOLO-Patch-Based-Inference Example - [Open in Colab](https://colab.research.google.com/drive/1FUao91GyB-ojGRN_okUxYyfagTT9tdsP?usp=sharing)
+
+Example of using various functions for visualizing basic YOLOv8/v9 inference results and handling overlapping crops - [Open in Colab](https://colab.research.google.com/drive/1eM4o1e0AUQrS1mLDpcgK9HKInWEvnaMn?usp=sharing)
+
+
+## Usage
+
+### 1. Patch-Based-Inference
+To carry out patch-based inference of YOLO models using our library, you need to follow a sequential procedure. First, you create an instance of the `MakeCropsDetectThem` class, providing all desired parameters related to YOLO inference and the patch segmentation principle.<br/> Subsequently, you pass the obtained object of this class to `CombineDetections`, which facilitates the consolidation of all predictions from each overlapping crop, followed by intelligent suppression of duplicates. <br/>Upon completion, you receive the result, from which you can extract the desired outcome of frame processing.
+
+The output obtained from the process includes several attributes that can be leveraged for further analysis or visualization:
+
+1. img: This attribute contains the original image on which the inference was performed. It provides context for the detected objects.
+
+2. confidences: This attribute holds the confidence scores associated with each detected object. These scores indicate the model's confidence level in the accuracy of its predictions.
+
+3. boxes: These bounding boxes are represented as a list of lists, where each list contains four values: [x_min, y_min, x_max, y_max]. These values correspond to the coordinates of the top-left and bottom-right corners of each bounding box.
+
+4. polygons: If available, this attribute provides a list containing NumPy arrays of polygon coordinates that represent segmentation masks corresponding to the detected objects. These polygons can be utilized to accurately outline the boundaries of each object.
+
+5. classes_ids: This attribute contains the class IDs assigned to each detected object. These IDs correspond to specific object classes defined during the model training phase.
+
+6. classes_names: These are the human-readable names corresponding to the class IDs. They provide semantic labels for the detected objects, making the results easier to interpret.
+
+```python
+import cv2
+from patched_yolo_infer import MakeCropsDetectThem, CombineDetections
+
+# Load the image 
+img_path = 'test_image.jpg'
+img = cv2.imread(img_path)
+
+element_crops = MakeCropsDetectThem(
+    image=img,
+    model_path="yolov8m.pt",
+    segment=False,
+    shape_x=640,
+    shape_y=640,
+    overlap_x=50,
+    overlap_y=50,
+    conf=0.5,
+    iou=0.7,
+    resize_initial_size=True,
+)
+result = CombineDetections(element_crops, nms_threshold=0.25, match_metric='IOS')  
+
+# Final Results:
+img=result.image
+confidences=result.filtered_confidences
+boxes=result.filtered_boxes
+polygons=result.filtered_polygons
+classes_ids=result.filtered_classes_id
+classes_names=result.filtered_classes_names
+```
+
+#### Explanation of possible input arguments:
+
+**MakeCropsDetectThem**
+Class implementing cropping and passing crops through a neural network for detection/segmentation.\
+**Args:**
+- **image** (*np.ndarray*): Input image BGR.
+- **model_path** (*str*): Path to the YOLO model.
+- **model** (*ultralytics model*) Pre-initialized model object. If provided, the model will be used directly instead of loading from model_path.
+- **imgsz** (*int*): Size of the input image for inference YOLO.
+- **conf** (*float*): Confidence threshold for detections YOLO.
+- **iou** (*float*): IoU threshold for non-maximum suppression YOLOv8 of single crop.
+- **classes_list** (*List[int] or None*): List of classes to filter detections. If None, all classes are considered. Defaults to None.
+- **segment** (*bool*): Whether to perform segmentation (YOLOv8-seg).
+- **shape_x** (*int*): Size of the crop in the x-coordinate.
+- **shape_y** (*int*): Size of the crop in the y-coordinate.
+- **overlap_x** (*float*): Percentage of overlap along the x-axis.
+- **overlap_y** (*float*): Percentage of overlap along the y-axis.
+- **show_crops** (*bool*): Whether to visualize the cropping.
+- **resize_initial_size** (*bool*): Whether to resize the results to the original image size (ps: slow operation).
+- **memory_optimize** (*bool*): Memory optimization option for segmentation (less accurate results when enabled).
+
+**CombineDetections**
+Class implementing combining masks/boxes from multiple crops + NMS (Non-Maximum Suppression).\
+**Args:**
+- **element_crops** (*MakeCropsDetectThem*): Object containing crop information.
+- **nms_threshold** (*float*): IoU/IoS threshold for non-maximum suppression.
+- **match_metric** (*str*): Matching metric, either 'IOU' or 'IOS'.
+- **intelligent_sorter** (*bool*): Enable sorting by area and rounded confidence parameter. If False, sorting will be done only by confidence (usual nms). (Dafault is True)
+
+
+
+---
+### 2. Custom inference visualization:
+Visualizes custom results of object detection or segmentation on an image.
+
+**Args:**
+- **img** (*numpy.ndarray*): The input image in BGR format.
+- **boxes** (*list*): A list of bounding boxes in the format [x_min, y_min, x_max, y_max].
+- **classes_ids** (*list*): A list of class IDs for each detection.
+- **confidences** (*list*): A list of confidence scores corresponding to each bounding box. Default is an empty list.
+- **classes_names** (*list*): A list of class names corresponding to the class IDs. Default is an empty list.
+- **polygons** (*list*): A list containing NumPy arrays of polygon coordinates that represent segmentation masks.
+- **masks** (*list*): A list of masks. Default is an empty list.
+- **segment** (*bool*): Whether to perform instance segmentation. Default is False.
+- **show_boxes** (*bool*): Whether to show bounding boxes. Default is True.
+- **show_class** (*bool*): Whether to show class labels. Default is True.
+- **fill_mask** (*bool*): Whether to fill the segmented regions with color. Default is False.
+- **alpha** (*float*): The transparency of filled masks. Default is 0.3.
+- **color_class_background** (*tuple*): The background BGR color for class labels. Default is (0, 0, 255) (red).
+- **color_class_text** (*tuple*): The text color for class labels. Default is (255, 255, 255) (white).
+- **thickness** (*int*): The thickness of bounding box and text. Default is 4.
+- **font**: The font type for class labels. Default is cv2.FONT_HERSHEY_SIMPLEX.
+- **font_scale** (*float*): The scale factor for font size. Default is 1.5.
+- **delta_colors** (*int*): The random seed offset for color variation. Default is seed=0.
+- **dpi** (*int*): Final visualization size (plot is bigger when dpi is higher). Default is 150.
+- **random_object_colors** (*bool*): If true, colors for each object are selected randomly. Default is False.
+- **show_confidences** (*bool*): If true and show_class=True, confidences near class are visualized. Default is False.
+- **axis_off** (*bool*): If true, axis is turned off in the final visualization. Default is True.
+- **show_classes_list** (*list*): If empty, visualize all classes. Otherwise, visualize only classes in the list.
+- **return_image_array** (*bool*): If True, the function returns the image (BGR np.array) instead of displaying it. Default is False.
+
+
+Example of using:
+```python
+from patched_yolo_infer import visualize_results
+
+# Assuming result is an instance of the CombineDetections class
+result = CombineDetections(...) 
+
+# Visualizing the results using the visualize_results function
+visualize_results(
+    img=result.image,
+    confidences=result.filtered_confidences,
+    boxes=result.filtered_boxes,
+    polygons=result.filtered_polygons,
+    classes_ids=result.filtered_classes_id,
+    classes_names=result.filtered_classes_names,
+    segment=False,
+)
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
-
----
----
-
-## __HOW TO IMPROVE THE QUALITY OF THE ALGORITHM FOR THE TASK OF INSTANCE SEGMENTATION:__
-
-In this approach, all operations under the hood are performed on binary masks of recognized objects. Storing these masks consumes a lot of memory, so this method requires more RAM and slightly more processing time. However, the accuracy of recognition significantly improves, which is especially noticeable in cases where there are many objects of different sizes and they are densely packed. Therefore, we recommend using this approach in production if accuracy is important and not speed, and if your computational resources allow storing hundreds of binary masks in RAM.
-
-The difference in the approach to using the function lies in specifying the parameter ```memory_optimize=False``` in the ```MakeCropsDetectThem``` class.
-In such a case, the informative values after processing will be the following:
-
-1. img: This attribute contains the original image on which the inference was performed. It provides context for the detected objects.
-
-2. confidences: This attribute holds the confidence scores associated with each detected object. These scores indicate the model's confidence level in the accuracy of its predictions.
-
-3. boxes: These bounding boxes are represented as a list of lists, where each list contains four values: [x_min, y_min, x_max, y_max]. These values correspond to the coordinates of the top-left and bottom-right corners of each bounding box.
-
-4. masks: This attribute provides segmentation binary masks corresponding to the detected objects. These masks can be used to precisely delineate object boundaries.
-
-5. classes_ids: This attribute contains the class IDs assigned to each detected object. These IDs correspond to specific object classes defined during the model training phase.
-
-6. classes_names: These are the human-readable names corresponding to the class IDs. They provide semantic labels for the detected objects, making the results easier to interpret.
-
-
-Here's how you can obtain them:
-```python
-img=result.image
-confidences=result.filtered_confidences
-boxes=result.filtered_boxes
-masks=result.filtered_masks
-classes_ids=result.filtered_classes_id
-classes_names=result.filtered_classes_names
-```
-
-
-[nb_example1]: https://nbviewer.org/github/Koldim2001/YOLO-Patch-Based-Inference/blob/main/examples/example_patch_based_inference.ipynb
-[colab_badge]: https://colab.research.google.com/assets/colab-badge.svg
-[colab_ex1]: https://colab.research.google.com/drive/1FUao91GyB-ojGRN_okUxYyfagTT9tdsP?usp=sharing
-[yt_link1]: https://youtu.be/IfbNOLROym4
-[nb_example2]: https://nbviewer.org/github/Koldim2001/YOLO-Patch-Based-Inference/blob/main/examples/example_extra_functions.ipynb
-[colab_ex2]: https://colab.research.google.com/drive/1eM4o1e0AUQrS1mLDpcgK9HKInWEvnaMn?usp=sharing
-[yt_link2]: https://youtu.be/nBQuWa63188
```

### Comparing `patched_yolo_infer-1.1.3/patched_yolo_infer/elements/CropElement.py` & `patched_yolo_infer-1.2.0/patched_yolo_infer/elements/CropElement.py`

 * *Files identical despite different names*

### Comparing `patched_yolo_infer-1.1.3/patched_yolo_infer/functions_extra.py` & `patched_yolo_infer-1.2.0/patched_yolo_infer/functions_extra.py`

 * *Files identical despite different names*

### Comparing `patched_yolo_infer-1.1.3/patched_yolo_infer/nodes/CombineDetections.py` & `patched_yolo_infer-1.2.0/patched_yolo_infer/nodes/CombineDetections.py`

 * *Files 1% similar despite different names*

```diff
@@ -52,29 +52,29 @@
         else:
             self.image = element_crops.crops[0].source_image_resized
 
         self.nms_threshold = nms_threshold  # IOU or IOS treshold for NMS
         self.match_metric = match_metric 
         self.intelligent_sorter = intelligent_sorter # enable sorting by area and confidence parameter
 
-        # combinate detections of all patches
+        # Combinate detections of all patches
         (
             self.detected_conf_list_full,
             self.detected_xyxy_list_full,
             self.detected_masks_list_full,
             self.detected_cls_id_list_full,
             self.detected_polygons_list_full
         ) = self.combinate_detections(crops=self.crops)
 
         self.detected_cls_names_list_full = [
             self.class_names[value] for value in self.detected_cls_id_list_full
         ]  # make str list
 
         # Invoke the NMS for segmentation masks method for filtering predictions
-        if len(self.detected_masks_list_full)>0:
+        if len(self.detected_masks_list_full) > 0:
 
             self.filtered_indices = self.nms(
                 self.detected_conf_list_full,
                 self.detected_xyxy_list_full,
                 self.match_metric,
                 self.nms_threshold,
                 self.detected_masks_list_full,
@@ -92,19 +92,21 @@
 
         # Apply filtering (nms output indeces) to the prediction lists
         self.filtered_confidences = [self.detected_conf_list_full[i] for i in self.filtered_indices]
         self.filtered_boxes = [self.detected_xyxy_list_full[i] for i in self.filtered_indices]
         self.filtered_classes_id = [self.detected_cls_id_list_full[i] for i in self.filtered_indices]
         self.filtered_classes_names = [self.detected_cls_names_list_full[i] for i in self.filtered_indices]
 
+        # Masks filtering:
         if element_crops.segment and not element_crops.memory_optimize:
             self.filtered_masks = [self.detected_masks_list_full[i] for i in self.filtered_indices]
         else:
             self.filtered_masks = []
         
+        # Polygons filtering:
         if element_crops.segment and element_crops.memory_optimize:
             self.filtered_polygons = [self.detected_polygons_list_full[i] for i in self.filtered_indices]
         else:
             self.filtered_polygons = []
 
     def combinate_detections(self, crops):
         """
```

### Comparing `patched_yolo_infer-1.1.3/patched_yolo_infer/nodes/MakeCropsDetectThem.py` & `patched_yolo_infer-1.2.0/patched_yolo_infer/nodes/MakeCropsDetectThem.py`

 * *Files 0% similar despite different names*

```diff
@@ -58,15 +58,15 @@
         model_path="yolov8m.pt",
         imgsz=640,
         conf=0.5,
         iou=0.7,
         classes_list=None,
         segment=False,
         shape_x=700,
-        shape_y=700,
+        shape_y=600,
         overlap_x=25,
         overlap_y=25,
         show_crops=False,
         resize_initial_size=False,
         model=None,
         memory_optimize=True
     ) -> None:
```

### Comparing `patched_yolo_infer-1.1.3/patched_yolo_infer.egg-info/SOURCES.txt` & `patched_yolo_infer-1.2.0/patched_yolo_infer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `patched_yolo_infer-1.1.3/setup.py` & `patched_yolo_infer-1.2.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 pwd = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(pwd, "patched_yolo_infer/README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
 
-VERSION = '1.1.3'
+VERSION = '1.2.0'
 DESCRIPTION = '''YOLO-Patch-Based-Inference for detection/segmentation of small objects in images.'''
 
 setup(
     name="patched_yolo_infer",
     version=VERSION,
     license="AGPL-3.0 license",
     url="https://github.com/Koldim2001/YOLO-Patch-Based-Inference",
```

