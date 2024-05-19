# Comparing `tmp/project_ppchem_tools_kit-0.1.1.tar.gz` & `tmp/project_ppchem_tools_kit-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "project_ppchem_tools_kit-0.1.1.tar", max compression
+gzip compressed data, was "project_ppchem_tools_kit-0.1.2.tar", max compression
```

## Comparing `project_ppchem_tools_kit-0.1.1.tar` & `project_ppchem_tools_kit-0.1.2.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0     1096 2024-05-17 13:18:42.194501 project_ppchem_tools_kit-0.1.1/LICENSE
--rw-r--r--   0        0        0     6815 2024-05-19 09:06:31.287575 project_ppchem_tools_kit-0.1.1/README.md
--rw-r--r--   0        0        0      650 2024-05-19 09:17:30.424278 project_ppchem_tools_kit-0.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-16 20:44:57.565187 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/__init__.py
--rw-r--r--   0        0        0      566 2024-05-18 16:20:56.501812 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/add_data_point.py
--rw-r--r--   0        0        0      376 2024-05-19 09:11:37.994019 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/bind_enter.py
--rw-r--r--   0        0        0      672 2024-05-18 17:45:23.130803 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/browse_excel_file.py
--rw-r--r--   0        0        0      164 2024-05-18 17:45:23.131373 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/clear_input.py
--rw-r--r--   0        0        0      504 2024-05-19 07:44:17.259322 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/copy_text.py
--rw-r--r--   0        0        0      979 2024-05-19 09:11:37.994184 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/create_radio_button.py
--rw-r--r--   0        0        0     2704 2024-05-19 09:11:37.993513 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/display_graph.py
--rw-r--r--   0        0        0     2147 2024-05-18 16:20:56.504673 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/display_max_point_and_coords.py
--rw-r--r--   0        0        0     1574 2024-05-17 12:06:36.279430 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/display_molecule.py
--rw-r--r--   0        0        0      581 2024-05-18 16:20:56.505034 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/display_result.py
--rw-r--r--   0        0        0     6226 2024-05-19 07:58:29.644129 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/error_calculation_interface.py
--rw-r--r--   0        0        0     9287 2024-05-18 13:16:11.687288 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/graph_function.py
--rw-r--r--   0        0        0     1646 2024-05-19 09:11:38.148414 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/linear_regression.py
--rw-r--r--   0        0        0     1064 2024-05-19 09:11:38.148314 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/make_graph.py
--rw-r--r--   0        0        0      371 2024-05-16 10:14:47.990043 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/name_to_smiles.py
--rw-r--r--   0        0        0      226 2024-05-18 17:45:23.132897 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/on_closing.py
--rw-r--r--   0        0        0      358 2024-05-19 09:11:37.994342 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/on_radio_select.py
--rw-r--r--   0        0        0     1784 2024-05-19 09:11:37.993793 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/open_graph_settings_window.py
--rw-r--r--   0        0        0     2504 2024-05-19 09:11:37.993466 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/process_input.py
--rw-r--r--   0        0        0      212 2024-05-19 08:19:40.701466 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/relative_to_assets.py
--rw-r--r--   0        0        0      147 2024-05-18 16:20:56.506233 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/select_all.py
--rw-r--r--   0        0        0      391 2024-05-18 16:20:56.506577 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_axes_color.py
--rw-r--r--   0        0        0      526 2024-05-18 16:20:56.506862 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_background_color.py
--rw-r--r--   0        0        0      619 2024-05-18 16:20:56.507221 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_custom_labels_and_title.py
--rw-r--r--   0        0        0      184 2024-05-18 16:20:56.507696 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_grid_color.py
--rw-r--r--   0        0        0      270 2024-05-18 16:20:56.508228 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_label_color.py
--rw-r--r--   0        0        0      432 2024-05-18 16:20:56.508577 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_line_color.py
--rw-r--r--   0        0        0      492 2024-05-18 16:20:56.508962 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_scale.py
--rw-r--r--   0        0        0      231 2024-05-16 10:14:47.987920 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/smiles_to_molar_mass.py
--rw-r--r--   0        0        0      124 2024-05-18 16:20:56.509235 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/toggle_grid.py
--rw-r--r--   0        0        0      573 2024-05-18 17:45:23.133845 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/update_clock.py
--rw-r--r--   0        0        0      908 2024-05-19 08:54:54.692946 project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/welcome_message.py
--rw-r--r--   0        0        0     7754 1970-01-01 00:00:00.000000 project_ppchem_tools_kit-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1096 2024-05-17 13:18:42.194501 project_ppchem_tools_kit-0.1.2/LICENSE
+-rw-r--r--   0        0        0     6807 2024-05-19 09:21:08.365245 project_ppchem_tools_kit-0.1.2/README.md
+-rw-r--r--   0        0        0      650 2024-05-19 09:23:03.273767 project_ppchem_tools_kit-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 20:44:57.565187 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/__init__.py
+-rw-r--r--   0        0        0      566 2024-05-18 16:20:56.501812 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/add_data_point.py
+-rw-r--r--   0        0        0      376 2024-05-19 09:11:37.994019 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/bind_enter.py
+-rw-r--r--   0        0        0      672 2024-05-18 17:45:23.130803 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/browse_excel_file.py
+-rw-r--r--   0        0        0      164 2024-05-18 17:45:23.131373 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/clear_input.py
+-rw-r--r--   0        0        0      504 2024-05-19 07:44:17.259322 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/copy_text.py
+-rw-r--r--   0        0        0      979 2024-05-19 09:11:37.994184 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/create_radio_button.py
+-rw-r--r--   0        0        0     2704 2024-05-19 09:11:37.993513 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/display_graph.py
+-rw-r--r--   0        0        0     2147 2024-05-18 16:20:56.504673 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/display_max_point_and_coords.py
+-rw-r--r--   0        0        0     1574 2024-05-17 12:06:36.279430 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/display_molecule.py
+-rw-r--r--   0        0        0      581 2024-05-18 16:20:56.505034 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/display_result.py
+-rw-r--r--   0        0        0     6226 2024-05-19 07:58:29.644129 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/error_calculation_interface.py
+-rw-r--r--   0        0        0     9287 2024-05-18 13:16:11.687288 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/graph_function.py
+-rw-r--r--   0        0        0     1646 2024-05-19 09:11:38.148414 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/linear_regression.py
+-rw-r--r--   0        0        0     1064 2024-05-19 09:11:38.148314 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/make_graph.py
+-rw-r--r--   0        0        0      371 2024-05-16 10:14:47.990043 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/name_to_smiles.py
+-rw-r--r--   0        0        0      226 2024-05-18 17:45:23.132897 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/on_closing.py
+-rw-r--r--   0        0        0      358 2024-05-19 09:11:37.994342 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/on_radio_select.py
+-rw-r--r--   0        0        0     1784 2024-05-19 09:11:37.993793 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/open_graph_settings_window.py
+-rw-r--r--   0        0        0     2504 2024-05-19 09:11:37.993466 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/process_input.py
+-rw-r--r--   0        0        0      212 2024-05-19 08:19:40.701466 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/relative_to_assets.py
+-rw-r--r--   0        0        0      147 2024-05-18 16:20:56.506233 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/select_all.py
+-rw-r--r--   0        0        0      391 2024-05-18 16:20:56.506577 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/set_axes_color.py
+-rw-r--r--   0        0        0      526 2024-05-18 16:20:56.506862 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/set_background_color.py
+-rw-r--r--   0        0        0      619 2024-05-18 16:20:56.507221 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/set_custom_labels_and_title.py
+-rw-r--r--   0        0        0      184 2024-05-18 16:20:56.507696 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/set_grid_color.py
+-rw-r--r--   0        0        0      270 2024-05-18 16:20:56.508228 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/set_label_color.py
+-rw-r--r--   0        0        0      432 2024-05-18 16:20:56.508577 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/set_line_color.py
+-rw-r--r--   0        0        0      492 2024-05-18 16:20:56.508962 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/set_scale.py
+-rw-r--r--   0        0        0      231 2024-05-16 10:14:47.987920 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/smiles_to_molar_mass.py
+-rw-r--r--   0        0        0      124 2024-05-18 16:20:56.509235 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/toggle_grid.py
+-rw-r--r--   0        0        0      573 2024-05-18 17:45:23.133845 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/update_clock.py
+-rw-r--r--   0        0        0      908 2024-05-19 08:54:54.692946 project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/welcome_message.py
+-rw-r--r--   0        0        0     7746 1970-01-01 00:00:00.000000 project_ppchem_tools_kit-0.1.2/PKG-INFO
```

### Comparing `project_ppchem_tools_kit-0.1.1/LICENSE` & `project_ppchem_tools_kit-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/README.md` & `project_ppchem_tools_kit-0.1.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -171,10 +171,11 @@
 ## 📜 License
 <a id="license"></a>
 
 This project is licensed under the MIT License. See the LICENSE file for details.
 
 ## 📸 Screenshots
 <a id="screenshots"></a>
-<img width="1002" alt="Capture d’écran 2024-05-18 à 16 44 09" src="https://github.com/sgrunber/Project-ppchem-tools-kit/assets/160881864/a44379f4-8cf2-4ac8-b370-36fee552ee6a">
+<img width="1002" alt="Capture d’écran 2024-05-18 à 16 44 09" src="https://github.com/sgrunber/Project-ppchem-tools-kit/raw/main/docs/source/_static/images/screen.png">
+
```

#### html2text {}

```diff
@@ -69,9 +69,9 @@
 entry: ```bibtex @misc{project-ppchem-tools-kit, title = {Project-ppchem-tools-
 kit}, author = {{MÃ©loÃ© Enzinger & SÃ©bastien Grunberg}}, year = {2024},
 publisher = {GitHub}, journal = {GitHub Repository}, howpublished = {\url
 {https://github.com/username/Project-ppchem-tools-kit}} } ``` ### Chicago Style
 ```bash Enzinger, MÃ©loÃ©, and SÃ©bastien Grunberg. 2024. Project-ppchem-tools-
 kit. Computer software. GitHub. https://github.com/username/Project-ppchem-
 tools-kit.` ``` ## ð License This project is licensed under the MIT License.
-See the LICENSE file for details. ## ð¸ Screenshots[Capture dâeÌcran 2024-
-05-18 aÌ 16 44 09]
+See the LICENSE file for details. ## ð¸ Screenshots[Capture dâÃ©cran 2024-
+05-18 Ã  16 44 09]
```

### Comparing `project_ppchem_tools_kit-0.1.1/pyproject.toml` & `project_ppchem_tools_kit-0.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "Project-ppchem-tools-kit"
-version = "0.1.1"
+version = "0.1.2"
 description = "Basic Chemistry Toolkit"
 authors = ["Méloé Enzinger <meloe.enzinger@epfl.ch> and Sébastien Grunberg <sebastien.grunberg@epfl.ch>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/add_data_point.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/add_data_point.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/browse_excel_file.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/browse_excel_file.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/create_radio_button.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/create_radio_button.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/display_graph.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/display_graph.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/display_max_point_and_coords.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/display_max_point_and_coords.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/display_molecule.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/display_molecule.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/display_result.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/display_result.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/error_calculation_interface.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/error_calculation_interface.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/graph_function.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/graph_function.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/linear_regression.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/linear_regression.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/make_graph.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/make_graph.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/open_graph_settings_window.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/open_graph_settings_window.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/process_input.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/process_input.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_background_color.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/set_background_color.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/set_custom_labels_and_title.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/set_custom_labels_and_title.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/update_clock.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/update_clock.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/src/project_ppchem_tools_kit/welcome_message.py` & `project_ppchem_tools_kit-0.1.2/src/project_ppchem_tools_kit/welcome_message.py`

 * *Files identical despite different names*

### Comparing `project_ppchem_tools_kit-0.1.1/PKG-INFO` & `project_ppchem_tools_kit-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Project-ppchem-tools-kit
-Version: 0.1.1
+Version: 0.1.2
 Summary: Basic Chemistry Toolkit
 License: MIT
 Author: Méloé Enzinger
 Author-email: meloe.enzinger@epfl.ch> and Sébastien Grunberg <sebastien.grunberg@epfl.ch
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -197,11 +197,12 @@
 ## 📜 License
 <a id="license"></a>
 
 This project is licensed under the MIT License. See the LICENSE file for details.
 
 ## 📸 Screenshots
 <a id="screenshots"></a>
-<img width="1002" alt="Capture d’écran 2024-05-18 à 16 44 09" src="https://github.com/sgrunber/Project-ppchem-tools-kit/assets/160881864/a44379f4-8cf2-4ac8-b370-36fee552ee6a">
+<img width="1002" alt="Capture d’écran 2024-05-18 à 16 44 09" src="https://github.com/sgrunber/Project-ppchem-tools-kit/raw/main/docs/source/_static/images/screen.png">
+
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: Project-ppchem-tools-kit Version: 0.1.1 Summary:
+Metadata-Version: 2.1 Name: Project-ppchem-tools-kit Version: 0.1.2 Summary:
 Basic Chemistry Toolkit License: MIT Author: MÃ©loÃ© Enzinger Author-email:
 meloe.enzinger@epfl.ch> and SÃ©bastien Grunberg
 epfl.ch Requires-Python: >=3.10,<4.0 Classifier: License :: OSI Approved :: MIT
 License Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.10 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12 Requires-Dist: matplotlib
 (==3.7.2) Requires-Dist: numpy (>=1.26.4,<2.0.0) Requires-Dist: numpy5
@@ -82,9 +82,9 @@
 entry: ```bibtex @misc{project-ppchem-tools-kit, title = {Project-ppchem-tools-
 kit}, author = {{MÃ©loÃ© Enzinger & SÃ©bastien Grunberg}}, year = {2024},
 publisher = {GitHub}, journal = {GitHub Repository}, howpublished = {\url
 {https://github.com/username/Project-ppchem-tools-kit}} } ``` ### Chicago Style
 ```bash Enzinger, MÃ©loÃ©, and SÃ©bastien Grunberg. 2024. Project-ppchem-tools-
 kit. Computer software. GitHub. https://github.com/username/Project-ppchem-
 tools-kit.` ``` ## ð License This project is licensed under the MIT License.
-See the LICENSE file for details. ## ð¸ Screenshots[Capture dâeÌcran 2024-
-05-18 aÌ 16 44 09]
+See the LICENSE file for details. ## ð¸ Screenshots[Capture dâÃ©cran 2024-
+05-18 Ã  16 44 09]
```

