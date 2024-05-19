# Comparing `tmp/easy_gui_jupyter-2024.5.19.tar.gz` & `tmp/easy_gui_jupyter-2024.5.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easy_gui_jupyter-2024.5.19.tar", max compression
+gzip compressed data, was "easy_gui_jupyter-2024.5.8.tar", max compression
```

## Comparing `easy_gui_jupyter-2024.5.19.tar` & `easy_gui_jupyter-2024.5.8.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1104 2024-05-08 10:31:35.279760 easy_gui_jupyter-2024.5.19/LICENSE.txt
--rw-r--r--   0        0        0     2674 2024-05-08 10:29:30.553206 easy_gui_jupyter-2024.5.19/README.md
--rw-r--r--   0        0        0      115 2024-05-19 16:20:30.033036 easy_gui_jupyter-2024.5.19/easy_gui_jupyter/__init__.py
--rw-r--r--   0        0        0    10677 2024-05-19 16:42:55.440671 easy_gui_jupyter-2024.5.19/easy_gui_jupyter/easy_gui_jupyter.py
--rw-r--r--   0        0        0      839 2024-05-19 16:43:19.154617 easy_gui_jupyter-2024.5.19/pyproject.toml
--rw-r--r--   0        0        0     3352 1970-01-01 00:00:00.000000 easy_gui_jupyter-2024.5.19/PKG-INFO
+-rw-r--r--   0        0        0     1104 2024-05-08 10:31:35.279760 easy_gui_jupyter-2024.5.8/LICENSE.txt
+-rw-r--r--   0        0        0     2674 2024-05-08 10:29:30.553206 easy_gui_jupyter-2024.5.8/README.md
+-rw-r--r--   0        0        0       52 2024-05-08 11:08:51.866358 easy_gui_jupyter-2024.5.8/easy_gui_jupyter/__init__.py
+-rw-r--r--   0        0        0     9311 2024-05-08 11:08:51.867208 easy_gui_jupyter-2024.5.8/easy_gui_jupyter/easy_gui_jupyter.py
+-rw-r--r--   0        0        0      840 2024-05-08 14:12:51.366763 easy_gui_jupyter-2024.5.8/pyproject.toml
+-rw-r--r--   0        0        0     3312 1970-01-01 00:00:00.000000 easy_gui_jupyter-2024.5.8/PKG-INFO
```

### Comparing `easy_gui_jupyter-2024.5.19/LICENSE.txt` & `easy_gui_jupyter-2024.5.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easy_gui_jupyter-2024.5.19/README.md` & `easy_gui_jupyter-2024.5.8/README.md`

 * *Files identical despite different names*

### Comparing `easy_gui_jupyter-2024.5.19/easy_gui_jupyter/easy_gui_jupyter.py` & `easy_gui_jupyter-2024.5.8/easy_gui_jupyter/easy_gui_jupyter.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,58 +1,18 @@
 """
 A module to help simplify the create of GUIs in Jupyter notebooks using ipywidgets.
 """
 
+import os
 import yaml
 from ipyfilechooser import FileChooser
 
 import ipywidgets as widgets
 from IPython.display import display, clear_output
 
-from pathlib import Path
-
-CONFIG_FILE = Path.home() / ".easy_gui" / "easy_gui.yml"
-
-
-def get_config(title: str):
-    """
-    Get the configuration dictionary without needing to initialize the GUI.
-
-    :param title: title of the GUI
-    """
-
-    if not CONFIG_FILE.exists():
-        return {}
-
-    with open(CONFIG_FILE, "r") as f:
-        cfg = yaml.load(f, Loader=yaml.SafeLoader)
-
-    if title is None:
-        return cfg
-    elif title in cfg:
-        return cfg[title]
-    else:
-        return {}
-
-
-def save_config(title: str, cfg: dict):
-    """
-    Save the configuration dictionary to a file.
-
-    :param title: title of the GUI
-    :param cfg: configuration dictionary
-    """
-    CONFIG_FILE.parent.mkdir(exist_ok=True)
-
-    base_config = get_config(None)  # loads the config file
-    base_config[title] = cfg
-
-    with open(CONFIG_FILE, "w") as f:
-        yaml.dump(base_config, f)
-
 
 class EasyGUI:
     """
     A class to simplify the creation of GUIs in Jupyter notebooks using ipywidgets.
 
     Args:
         title (str): The title of the GUI.
@@ -86,24 +46,37 @@
     Note:
         This class simplifies the creation of GUIs in Jupyter notebooks using ipywidgets. It provides a variety of methods for adding different types of widgets to the GUI, and it allows for saving and loading widget values to maintain user settings across sessions.
     """
 
     def __init__(self, title="basic_gui", width="50%"):
         """
         Container for widgets.
-        :param title: title of the widget container
         :param width: width of the widget container
         """
         self._layout = widgets.Layout(width=width)
         self._style = {"description_width": "initial"}
         self._widgets = {}
         self._nLabels = 0
         self._main_display = widgets.VBox()
         self._title = title
-        self.cfg = get_config(title)
+        self._cfg = {title: {}}
+        self.cfg = self._cfg[title]
+
+        # Get the user's home folder
+        self._home_folder = os.path.expanduser("~")
+        self._config_folder = os.path.join(self._home_folder, ".nanopyx")
+        if not os.path.exists(self._config_folder):
+            os.makedirs(self._config_folder)
+
+        self._config_file = os.path.join(self._config_folder, "easy_gui.yml")
+        if os.path.exists(self._config_file):
+            with open(self._config_file, "r") as f:
+                self._cfg = yaml.load(f, Loader=yaml.FullLoader)
+                if title in self._cfg:
+                    self.cfg = self._cfg[title]
 
     def __getitem__(self, tag: str) -> widgets.Widget:
         return self._widgets[tag]
 
     def __len__(self) -> int:
         return len(self._widgets)
 
@@ -125,65 +98,43 @@
         :param args: args for the widget
         :param kwargs: kwargs for the widget
         """
         self._widgets[tag] = widgets.Button(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
-    def add_text(self, tag, *args, remember_value=False, **kwargs):
+    def add_text(self, tag, *args, **kwargs):
         """
         Add a text widget to the container.
         :param tag: tag to identify the widget
         :param args: args for the widget
-        :param remember_value: remember the last value
         :param kwargs: kwargs for the widget
 
         Example:
             >>> gui = EasyGUI()
             >>> gui.add_text("text", value="Hello, world!")
         """
-        if remember_value and tag in self.cfg:
-            kwargs["value"] = str(self.cfg[tag])
-
         self._widgets[tag] = widgets.Text(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
-    def add_textarea(self, tag, *args, remember_value=False, **kwargs):
-        """
-        Add a textarea widget to the container.
-        :param tag: tag to identify the widget
-        :param args: args for the widget
-        :param remember_value: remember the last value
-        :param kwargs: kwargs for the widget
-        """
-        if remember_value and tag in self.cfg:
-            kwargs["value"] = str(self.cfg[tag])
-        self._widgets[tag] = widgets.Textarea(
-            *args, **kwargs, layout=self._layout, style=self._style
-        )
-
-        self._widgets[tag] = widgets.Textarea(
-            *args, **kwargs, layout=self._layout, style=self._style
-        )
-
     def add_int_slider(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a integer slider widget to the container.
         :param tag: tag to identify the widget
         :param args: args for the widget
         :param remember_value: remember the last value
         :param kwargs: kwargs for the widget
         """
         if (
             remember_value
             and tag in self.cfg
             and kwargs["min"] <= self.cfg[tag] <= kwargs["max"]
         ):
-            kwargs["value"] = int(self.cfg[tag])
+            kwargs["value"] = self.cfg[tag]
         self._widgets[tag] = widgets.IntSlider(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
     def add_float_slider(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a float slider widget to the container.
@@ -244,18 +195,14 @@
     def add_dropdown(self, tag, *args, remember_value=False, **kwargs):
         """
         Add a dropdown widget to the container.
         :param tag: tag to identify the widget
         :param args: args for the widget
         :param remember_value: remember the last value
         :param kwargs: kwargs for the widget
-
-        Example:
-            >>> gui = EasyGUI()
-            >>> gui.add_dropdown("dropdown", options=["A", "B", "C"])
         """
         if remember_value and tag in self.cfg and self.cfg[tag] in kwargs["options"]:
             kwargs["value"] = self.cfg[tag]
         self._widgets[tag] = widgets.Dropdown(
             *args, **kwargs, layout=self._layout, style=self._style
         )
 
@@ -275,22 +222,17 @@
     def save_settings(self):
         # remember widget values for next time and store them in a config file
         for tag in self._widgets:
             if tag.startswith("label_"):
                 pass
             elif hasattr(self._widgets[tag], "value"):
                 self.cfg[tag] = self._widgets[tag].value
-
-        save_config(self._title, self.cfg)
-
-    def restore_default_settings(self):
-        # restore default settings
-        save_config(self._title, {})
-        self.clear()
-        self.show()
+        self._cfg[self._title] = self.cfg
+        with open(self._config_file, "w") as f:
+            yaml.dump(self._cfg, f)
 
     def show(self):
         """
         Show the widgets in the container.
         """
         # display the widgets
         self._main_display.children = tuple(self._widgets.values())
```

### Comparing `easy_gui_jupyter-2024.5.19/pyproject.toml` & `easy_gui_jupyter-2024.5.8/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,37 @@
-[build-system]
-requires = [ "poetry-core",]
-build-backend = "poetry.core.masonry.api"
-
 [tool.poetry]
 name = "easy_gui_jupyter"
-version = "2024.05.19"
+version = "2024.05.08"
 description = "Simplify the creation of GUI elements in Jupyter notebooks"
-authors = [ "Ricardo Henriques <ricardo@henriqueslab.org>", "Bruno Saraiva <bruno.msaraiva2@gmail.com>", "António Brito <antmsbrito95@gmail.com>",]
+authors = [    
+    "Ricardo Henriques <ricardo@henriqueslab.org>", 
+    "Bruno Saraiva <bruno.msaraiva2@gmail.com>",
+    "António Brito <antmsbrito95@gmail.com>"
+    ]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 ipython = "^8.24.0"
 ipywidgets = "^8.1.2"
 ipyfilechooser = "^0.6.0"
 pyyaml = "^6.0.1"
-toml = "^0.10.2"
-
-[tool.pytest.ini_options]
-testpaths = [ "tests",]
-addopts = "--nbmake -n=auto"
 
 [tool.poetry.group.dev.dependencies]
 pre-commit = "^3.7.0"
 ipykernel = "^6.29.4"
 ruff = "^0.4.3"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.2.0"
 pytest-xdist = "^3.6.1"
 nbmake = "^1.5.3"
 gptrepo = "^1.0.3"
+
+[tool.pytest.ini_options]
+testpaths = ["tests"]
+addopts = "--nbmake -n=auto"
+
+[build-system]
+requires = ["poetry-core"]
+build-backend = "poetry.core.masonry.api"
+
```

### Comparing `easy_gui_jupyter-2024.5.19/PKG-INFO` & `easy_gui_jupyter-2024.5.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 Metadata-Version: 2.1
 Name: easy_gui_jupyter
-Version: 2024.5.19
+Version: 2024.5.8
 Summary: Simplify the creation of GUI elements in Jupyter notebooks
 Author: Ricardo Henriques
 Author-email: ricardo@henriqueslab.org
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: ipyfilechooser (>=0.6.0,<0.7.0)
 Requires-Dist: ipython (>=8.24.0,<9.0.0)
 Requires-Dist: ipywidgets (>=8.1.2,<9.0.0)
 Requires-Dist: pyyaml (>=6.0.1,<7.0.0)
-Requires-Dist: toml (>=0.10.2,<0.11.0)
 Description-Content-Type: text/markdown
 
 # Easy GUI Jupyter
 
 Easy GUI Jupyter is a Python library that simplifies the creation of graphical user interfaces (GUIs) in Jupyter notebooks using ipywidgets. It provides a convenient way to add various types of widgets to your Jupyter notebooks, making it easier to interact with your code and visualize results.
 
 ## Features
```

