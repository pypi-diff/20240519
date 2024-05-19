# Comparing `tmp/maat-machine-0.1.1b2.tar.gz` & `tmp/maat-machine-0.1.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maat-machine-0.1.1b2.tar", max compression
+gzip compressed data, was "maat-machine-0.1.1b3.tar", max compression
```

## Comparing `maat-machine-0.1.1b2.tar` & `maat-machine-0.1.1b3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1091 2024-05-13 12:20:29.203050 maat-machine-0.1.1b2/LICENSE
--rw-r--r--   0        0        0        0 2024-05-13 12:20:29.219736 maat-machine-0.1.1b2/README.md
--rw-r--r--   0        0        0        0 2024-05-13 12:20:29.219736 maat-machine-0.1.1b2/maat_machine/__init__.py
--rw-r--r--   0        0        0      661 2024-05-13 12:20:29.219736 maat-machine-0.1.1b2/maat_machine/archive.py
--rw-r--r--   0        0        0     3792 2024-05-14 18:11:36.200710 maat-machine-0.1.1b2/maat_machine/data_images.py
--rw-r--r--   0        0        0     6844 2024-05-13 12:20:29.219736 maat-machine-0.1.1b2/maat_machine/directory_tree.py
--rw-r--r--   0        0        0     2265 2024-05-13 12:20:29.219736 maat-machine-0.1.1b2/maat_machine/filesystem.py
--rw-r--r--   0        0        0       84 2024-05-13 12:20:29.219736 maat-machine-0.1.1b2/maat_machine/logging.py
--rw-r--r--   0        0        0        0 2024-05-13 12:20:29.219736 maat-machine-0.1.1b2/maat_machine/model/__init__.py
--rw-r--r--   0        0        0    12417 2024-05-19 08:55:42.230553 maat-machine-0.1.1b2/maat_machine/model/cv.py
--rw-r--r--   0        0        0      761 2024-05-13 12:20:29.219736 maat-machine-0.1.1b2/maat_machine/model/utils.py
--rw-r--r--   0        0        0      513 2024-05-13 12:20:29.219736 maat-machine-0.1.1b2/maat_machine/packages.py
--rw-r--r--   0        0        0      111 2024-05-13 12:20:29.219736 maat-machine-0.1.1b2/maat_machine/plots.py
--rw-r--r--   0        0        0     2189 2024-05-13 12:20:29.219736 maat-machine-0.1.1b2/maat_machine/pprint.py
--rw-r--r--   0        0        0       76 2024-05-13 12:20:29.219736 maat-machine-0.1.1b2/maat_machine/time.py
--rw-r--r--   0        0        0     1858 2024-05-13 12:20:29.219736 maat-machine-0.1.1b2/maat_machine/utils.py
--rw-r--r--   0        0        0      670 2024-05-19 08:56:00.709574 maat-machine-0.1.1b2/pyproject.toml
--rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 maat-machine-0.1.1b2/setup.py
--rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 maat-machine-0.1.1b2/PKG-INFO
+-rw-r--r--   0        0        0     1091 2024-05-13 12:20:29.203050 maat-machine-0.1.1b3/LICENSE
+-rw-r--r--   0        0        0        0 2024-05-13 12:20:29.219736 maat-machine-0.1.1b3/README.md
+-rw-r--r--   0        0        0        0 2024-05-13 12:20:29.219736 maat-machine-0.1.1b3/maat_machine/__init__.py
+-rw-r--r--   0        0        0      661 2024-05-13 12:20:29.219736 maat-machine-0.1.1b3/maat_machine/archive.py
+-rw-r--r--   0        0        0     3792 2024-05-14 18:11:36.200710 maat-machine-0.1.1b3/maat_machine/data_images.py
+-rw-r--r--   0        0        0     6844 2024-05-13 12:20:29.219736 maat-machine-0.1.1b3/maat_machine/directory_tree.py
+-rw-r--r--   0        0        0     2265 2024-05-13 12:20:29.219736 maat-machine-0.1.1b3/maat_machine/filesystem.py
+-rw-r--r--   0        0        0       84 2024-05-13 12:20:29.219736 maat-machine-0.1.1b3/maat_machine/logging.py
+-rw-r--r--   0        0        0        0 2024-05-13 12:20:29.219736 maat-machine-0.1.1b3/maat_machine/model/__init__.py
+-rw-r--r--   0        0        0    12787 2024-05-19 10:09:46.115966 maat-machine-0.1.1b3/maat_machine/model/cv.py
+-rw-r--r--   0        0        0      761 2024-05-13 12:20:29.219736 maat-machine-0.1.1b3/maat_machine/model/utils.py
+-rw-r--r--   0        0        0      513 2024-05-13 12:20:29.219736 maat-machine-0.1.1b3/maat_machine/packages.py
+-rw-r--r--   0        0        0      111 2024-05-13 12:20:29.219736 maat-machine-0.1.1b3/maat_machine/plots.py
+-rw-r--r--   0        0        0     2189 2024-05-13 12:20:29.219736 maat-machine-0.1.1b3/maat_machine/pprint.py
+-rw-r--r--   0        0        0       76 2024-05-13 12:20:29.219736 maat-machine-0.1.1b3/maat_machine/time.py
+-rw-r--r--   0        0        0     1858 2024-05-13 12:20:29.219736 maat-machine-0.1.1b3/maat_machine/utils.py
+-rw-r--r--   0        0        0      670 2024-05-19 10:12:00.982745 maat-machine-0.1.1b3/pyproject.toml
+-rw-r--r--   0        0        0      927 1970-01-01 00:00:00.000000 maat-machine-0.1.1b3/setup.py
+-rw-r--r--   0        0        0      762 1970-01-01 00:00:00.000000 maat-machine-0.1.1b3/PKG-INFO
```

### Comparing `maat-machine-0.1.1b2/LICENSE` & `maat-machine-0.1.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.1b2/maat_machine/archive.py` & `maat-machine-0.1.1b3/maat_machine/archive.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.1b2/maat_machine/data_images.py` & `maat-machine-0.1.1b3/maat_machine/data_images.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.1b2/maat_machine/directory_tree.py` & `maat-machine-0.1.1b3/maat_machine/directory_tree.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.1b2/maat_machine/filesystem.py` & `maat-machine-0.1.1b3/maat_machine/filesystem.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.1b2/maat_machine/model/cv.py` & `maat-machine-0.1.1b3/maat_machine/model/cv.py`

 * *Files 10% similar despite different names*

```diff
@@ -65,14 +65,18 @@
 
         self.dense_layer_array = dense_layer_array
         self.dense_activation = dense_activation
         self.dense_activation_parameter = dense_activation_parameter
         self.dense_dropout = dense_dropout
 
         self.model = None
+        self.image_data_generator = None
+        self.train_generator = None
+        self.validation_generator = None
+        self.test_generator = None
 
     def create_cnn_model(self):
         model = keras.Sequential()
         model.add(lktf.Input(shape=self.input_shape, name='input'))
 
         for i, conv_layer_config in list(enumerate(self.conv_layer_array)):
             conv_filters_i, conv_kernel_i, layers_i = conv_layer_config
@@ -167,38 +171,43 @@
         display(data_frame.sample(10))
         display(np.unique(labels))
 
         image_data_generator = tkpi.ImageDataGenerator(
             rescale=1.0/255,
             validation_split=self.validation_split
         )
+        self.image_data_generator = image_data_generator
+
         train_generator = image_data_generator.flow_from_dataframe(
             dataframe=data_frame,
             x_col=self.file_path_column_name,
             y_col=self.label_column_name,
             color_mode="rgb",
             class_mode="categorical",
             target_size=(self.input_shape[0], self.input_shape[1]),
             batch_size=self.batch_size,
             seed=137,
             suffle=True,
             subset='training'
         )
+        self.train_generator = train_generator
+
         validation_generator = image_data_generator.flow_from_dataframe(
             dataframe=data_frame,
             x_col=self.file_path_column_name,
             y_col=self.label_column_name,
             color_mode="rgb",
             class_mode="categorical",
             target_size=(self.input_shape[0], self.input_shape[1]),
             batch_size=self.batch_size,
             seed=137,
             suffle=True,
             subset='validation'
         )
+        self.validation_generator = validation_generator
 
         result = self.model.fit(
             train_generator,
             epochs=self.epochs,
             validation_data=validation_generator,
         )
         return result
@@ -214,14 +223,15 @@
             batch_size=self.batch_size,
             seed=42,
             shuffle=False,
             color_mode="rgb",
             class_mode=None,
             target_size=(self.input_shape[0], self.input_shape[1]),
         )
+        self.test_generator = test_generator
         return self.model.predict(test_generator)
     
     def predict_from_dataframe(self, features: pd.DataFrame):
         labels_predicted_proba = self.predict_proba_from_dataframe(features)
         predicted_labels = np.argmax(labels_predicted_proba, axis=1)
         return predicted_labels
     
@@ -233,15 +243,15 @@
     def predict_proba_from_pil_image(self, image: pillow_images.Image):
         target_width = self.input_shape[1]
         target_height = self.input_shape[0]
         test_image = image.resize((target_width, target_height))
         test_image = test_image.convert('RGB')
         image_array = np.array(test_image, dtype='float64') / 255.0
         image_array = np.expand_dims(image_array, axis=0)
-        return self.model.predict(image_array) 
+        return self.model.predict(image_array)
 
     def predict_from_pil_image(self, image: pillow_images.Image):
         labels_predicted_proba = self.predict_proba_from_pil_image(image)
         predicted_label = np.argmax(labels_predicted_proba, axis=1)
         return predicted_label
 
     def save(self, directory_path: paths.Path):
```

### Comparing `maat-machine-0.1.1b2/maat_machine/model/utils.py` & `maat-machine-0.1.1b3/maat_machine/model/utils.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.1b2/maat_machine/packages.py` & `maat-machine-0.1.1b3/maat_machine/packages.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.1b2/maat_machine/pprint.py` & `maat-machine-0.1.1b3/maat_machine/pprint.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.1b2/maat_machine/utils.py` & `maat-machine-0.1.1b3/maat_machine/utils.py`

 * *Files identical despite different names*

### Comparing `maat-machine-0.1.1b2/pyproject.toml` & `maat-machine-0.1.1b3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "maat-machine"
-version = "0.1.1b2"
+version = "0.1.1b3"
 description = "Yet another package designed to simplify coding for data science and machine learning"
 authors = ["Dmitry Vlasov <dmitry.v.vlasov@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "maat_machine"}]
 
 [tool.poetry.dependencies]
```

### Comparing `maat-machine-0.1.1b2/setup.py` & `maat-machine-0.1.1b3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
  'pillow>=10.3.0,<11.0.0',
  'scikit-learn>=1.4.2,<2.0.0',
  'tensorflow==2.16.1',
  'tqdm>=4.66.4,<5.0.0']
 
 setup_kwargs = {
     'name': 'maat-machine',
-    'version': '0.1.1b2',
+    'version': '0.1.1b3',
     'description': 'Yet another package designed to simplify coding for data science and machine learning',
     'long_description': '',
     'author': 'Dmitry Vlasov',
     'author_email': 'dmitry.v.vlasov@gmail.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `maat-machine-0.1.1b2/PKG-INFO` & `maat-machine-0.1.1b3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maat-machine
-Version: 0.1.1b2
+Version: 0.1.1b3
 Summary: Yet another package designed to simplify coding for data science and machine learning
 License: MIT
 Author: Dmitry Vlasov
 Author-email: dmitry.v.vlasov@gmail.com
 Requires-Python: ==3.11.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

