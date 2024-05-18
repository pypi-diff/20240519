# Comparing `tmp/dash_pydantic_form-0.1.3.tar.gz` & `tmp/dash_pydantic_form-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dash_pydantic_form-0.1.3.tar", last modified: Thu May 16 13:13:21 2024, max compression
+gzip compressed data, was "dash_pydantic_form-0.1.4.tar", last modified: Sat May 18 23:41:17 2024, max compression
```

## Comparing `dash_pydantic_form-0.1.3.tar` & `dash_pydantic_form-0.1.4.tar`

### file list

```diff
@@ -1,44 +1,47 @@
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 13:13:21.093371 dash_pydantic_form-0.1.3/
--rw-r--r--   0 renaud    (1000) renaud    (1000)     3231 2024-04-25 01:57:38.000000 dash_pydantic_form-0.1.3/.gitignore
--rw-r--r--   0 renaud    (1000) renaud    (1000)      406 2024-05-11 12:42:14.000000 dash_pydantic_form-0.1.3/.pre-commit-config.yaml
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 13:13:21.083371 dash_pydantic_form-0.1.3/.vscode/
--rw-r--r--   0 renaud    (1000) renaud    (1000)      834 2024-05-12 04:37:36.000000 dash_pydantic_form-0.1.3/.vscode/launch.json
--rw-r--r--   0 renaud    (1000) renaud    (1000)      523 2024-05-16 13:12:46.000000 dash_pydantic_form-0.1.3/CHANGELOG.md
--rw-r--r--   0 renaud    (1000) renaud    (1000)     8673 2024-05-16 13:13:21.093371 dash_pydantic_form-0.1.3/PKG-INFO
--rw-r--r--   0 renaud    (1000) renaud    (1000)     7970 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/README.md
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 13:13:21.083371 dash_pydantic_form-0.1.3/dash_pydantic_form/
--rw-r--r--   0 renaud    (1000) renaud    (1000)      749 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/__init__.py
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 13:13:21.093371 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1609 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/__init__.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1399 2024-05-16 13:02:52.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/all_fields.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)    21910 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/base_fields.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)    18943 2024-05-14 13:01:55.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/editabletable_field.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1994 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/markdown_field.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)     8536 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/model_field.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)    21436 2024-05-14 13:16:15.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/fields/model_list_field.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)     2145 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/form_section.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)      944 2024-05-11 12:54:05.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/ids.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)    17989 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/model_form.py
--rw-r--r--   0 renaud    (1000) renaud    (1000)     8201 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/pydantic_form_scripts.js
--rw-r--r--   0 renaud    (1000) renaud    (1000)     2102 2024-05-14 12:37:15.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/pydantic_form_styles.css
--rw-r--r--   0 renaud    (1000) renaud    (1000)     8782 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/dash_pydantic_form/utils.py
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 13:13:21.093371 dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/
--rw-r--r--   0 renaud    (1000) renaud    (1000)     8673 2024-05-16 13:13:21.000000 dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/PKG-INFO
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1072 2024-05-16 13:13:21.000000 dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/SOURCES.txt
--rw-r--r--   0 renaud    (1000) renaud    (1000)        1 2024-05-16 13:13:21.000000 dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/dependency_links.txt
--rw-r--r--   0 renaud    (1000) renaud    (1000)      116 2024-05-16 13:13:21.000000 dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/requires.txt
--rw-r--r--   0 renaud    (1000) renaud    (1000)       36 2024-05-16 13:13:21.000000 dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/top_level.txt
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 13:13:21.093371 dash_pydantic_form-0.1.3/docs/
--rw-r--r--   0 renaud    (1000) renaud    (1000)       87 2024-05-12 09:51:29.000000 dash_pydantic_form-0.1.3/docs/_config.yml
--rw-r--r--   0 renaud    (1000) renaud    (1000)       21 2024-05-12 09:47:47.000000 dash_pydantic_form-0.1.3/docs/index.md
-drwxr-xr-x   0 renaud    (1000) renaud    (1000)        0 2024-05-16 13:13:21.093371 dash_pydantic_form-0.1.3/images/
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)    47789 2024-05-13 11:27:16.000000 dash_pydantic_form-0.1.3/images/conditionnally-visible-field.gif
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)    55763 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/images/discriminated-union.gif
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)    15290 2024-05-13 11:17:07.000000 dash_pydantic_form-0.1.3/images/editable-table.png
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)     4506 2024-05-13 11:00:42.000000 dash_pydantic_form-0.1.3/images/form-sections.png
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)    12406 2024-05-13 11:12:08.000000 dash_pydantic_form-0.1.3/images/model-list.png
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)     8028 2024-05-13 11:00:37.000000 dash_pydantic_form-0.1.3/images/nested-model.png
--rwxr-xr-x   0 renaud    (1000) renaud    (1000)    16764 2024-05-13 10:21:46.000000 dash_pydantic_form-0.1.3/images/simple-form.png
--rw-r--r--   0 renaud    (1000) renaud    (1000)     1186 2024-05-16 13:00:11.000000 dash_pydantic_form-0.1.3/pyproject.toml
--rw-r--r--   0 renaud    (1000) renaud    (1000)       38 2024-05-16 13:13:21.093371 dash_pydantic_form-0.1.3/setup.cfg
--rw-r--r--   0 renaud    (1000) renaud    (1000)     7517 2024-05-16 13:12:27.000000 dash_pydantic_form-0.1.3/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.177666 dash_pydantic_form-0.1.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.169666 dash_pydantic_form-0.1.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.173666 dash_pydantic_form-0.1.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1188 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/.github/workflows/publish.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3231 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.173666 dash_pydantic_form-0.1.4/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      662 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-05-18 23:41:17.177666 dash_pydantic_form-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.173666 dash_pydantic_form-0.1.4/dash_pydantic_form/
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.173666 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)     1609 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/all_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21910 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/base_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18943 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/editabletable_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1994 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/markdown_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8536 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/model_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)    21436 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/fields/model_list_field.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2029 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/form_section.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/ids.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18731 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/model_form.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8662 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/pydantic_form_scripts.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2102 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/pydantic_form_styles.css
+-rw-r--r--   0 runner    (1001) docker     (127)     8782 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/dash_pydantic_form/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.177666 dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8672 2024-05-18 23:41:17.000000 dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-18 23:41:17.000000 dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-18 23:41:17.000000 dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-05-18 23:41:17.000000 dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-18 23:41:17.000000 dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.173666 dash_pydantic_form-0.1.4/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/docs/_config.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/docs/index.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-18 23:41:17.177666 dash_pydantic_form-0.1.4/images/
+-rwxr-xr-x   0 runner    (1001) docker     (127)    47789 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/images/conditionnally-visible-field.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    55763 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/images/discriminated-union.gif
+-rwxr-xr-x   0 runner    (1001) docker     (127)    15290 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/images/editable-table.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4506 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/images/form-sections.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    12406 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/images/model-list.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)     8028 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/images/nested-model.png
+-rwxr-xr-x   0 runner    (1001) docker     (127)    16764 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/images/simple-form.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1186 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-18 23:41:17.177666 dash_pydantic_form-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     7517 2024-05-18 23:41:07.000000 dash_pydantic_form-0.1.4/usage.py
```

### Comparing `dash_pydantic_form-0.1.3/.gitignore` & `dash_pydantic_form-0.1.4/.gitignore`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/.vscode/launch.json` & `dash_pydantic_form-0.1.4/.vscode/launch.json`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/CHANGELOG.md` & `dash_pydantic_form-0.1.4/CHANGELOG.md`

 * *Files 17% similar despite different names*

```diff
@@ -2,14 +2,18 @@
 All notable changes to this project will be documented in this file.
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 and this project adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html).
 
 ## [Unreleased]
 
+## [0.1.4] - 2024-05-19
+### Added
+- Allow form submit on Enter press (optional as it may break some field renders and more complex forms)
+
 ## [0.1.3] - 2024-05-16
 ### Added
 - Discriminated Model union #2
 
 ## [0.1.2] - 2024-05-16
 ### Added
 - MarkdownField
```

### Comparing `dash_pydantic_form-0.1.3/PKG-INFO` & `dash_pydantic_form-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.3
+Version: 0.1.4
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
@@ -42,15 +42,15 @@
 class Employee(BaseModel):
     first_name: str = Field(title="First name")
     last_name: str = Field(title="Last name")
     office: Literal["au", "uk", "us", "fr"] = Field(title="Office")
     joined: date = Field(title="Employment date")
 ```
 
-Then you can get an auto-generated form with `ModelForm`, leveraging [dash-mantine-components](https://dash-mantine-components.com) (vercion 0.14) for form inputs.
+Then you can get an auto-generated form with `ModelForm`, leveraging [dash-mantine-components](https://dash-mantine-components.com) (version 0.14) for form inputs.
 
 ```py
 from dash_pydantic_form import ModelForm
 
 # somewhere in your layout:
 form = ModelForm(
     Employee,
@@ -264,15 +264,15 @@
         "only_bob": fields.Textarea(
             visible=("first_name", "==", "Bob"),
         )
     },
 )
 ```
 
-![Conditionnally visible field](images/conditionnally-visible-field.gif)
+![Conditionally visible field](images/conditionnally-visible-field.gif)
 
 `visible` accepts a boolean, a 3-tuple or list of 3-tuples with format: (field, operator, value). The available operators are:
 * "=="
 * "!="
 * "in"
 * "not in"
 * "array_contains"
```

### Comparing `dash_pydantic_form-0.1.3/README.md` & `dash_pydantic_form-0.1.4/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 class Employee(BaseModel):
     first_name: str = Field(title="First name")
     last_name: str = Field(title="Last name")
     office: Literal["au", "uk", "us", "fr"] = Field(title="Office")
     joined: date = Field(title="Employment date")
 ```
 
-Then you can get an auto-generated form with `ModelForm`, leveraging [dash-mantine-components](https://dash-mantine-components.com) (vercion 0.14) for form inputs.
+Then you can get an auto-generated form with `ModelForm`, leveraging [dash-mantine-components](https://dash-mantine-components.com) (version 0.14) for form inputs.
 
 ```py
 from dash_pydantic_form import ModelForm
 
 # somewhere in your layout:
 form = ModelForm(
     Employee,
@@ -244,15 +244,15 @@
         "only_bob": fields.Textarea(
             visible=("first_name", "==", "Bob"),
         )
     },
 )
 ```
 
-![Conditionnally visible field](images/conditionnally-visible-field.gif)
+![Conditionally visible field](images/conditionnally-visible-field.gif)
 
 `visible` accepts a boolean, a 3-tuple or list of 3-tuples with format: (field, operator, value). The available operators are:
 * "=="
 * "!="
 * "in"
 * "not in"
 * "array_contains"
```

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form/__init__.py` & `dash_pydantic_form-0.1.4/dash_pydantic_form/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form/fields/__init__.py` & `dash_pydantic_form-0.1.4/dash_pydantic_form/fields/__init__.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form/fields/all_fields.py` & `dash_pydantic_form-0.1.4/dash_pydantic_form/fields/all_fields.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form/fields/base_fields.py` & `dash_pydantic_form-0.1.4/dash_pydantic_form/fields/base_fields.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form/fields/editabletable_field.py` & `dash_pydantic_form-0.1.4/dash_pydantic_form/fields/editabletable_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form/fields/markdown_field.py` & `dash_pydantic_form-0.1.4/dash_pydantic_form/fields/markdown_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form/fields/model_field.py` & `dash_pydantic_form-0.1.4/dash_pydantic_form/fields/model_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form/fields/model_list_field.py` & `dash_pydantic_form-0.1.4/dash_pydantic_form/fields/model_list_field.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form/form_section.py` & `dash_pydantic_form-0.1.4/dash_pydantic_form/form_section.py`

 * *Files 8% similar despite different names*

```diff
@@ -42,17 +42,16 @@
     render: Literal["accordion", "tabs", "steps"]
         how the sections should be rendered. Possible values: "accordion", "tabs", "steps".
         Default "accordion".
     excluded_fields: list[str] | None
         List of field names to exclude from the form altogether, optional.
     render_kwargs: dict | None
         Additional render kwargs passed to the section render functions, optional.
-        See :meth:`dash_pydantic_form.model_form.ModelForm.render_accordion_sections`,
-        :meth:`dash_pydantic_form.model_form.ModelForm.render_tabs_sections` and
-        :meth:`dash_pydantic_form.model_form.ModelForm.render_steps_sections`
+        See `ModelForm.render_accordion_sections`, `ModelForm.render_tabs_sections` and
+        `ModelForm.render_steps_sections`
     """
 
     sections: list[FormSection]
     remaining_fields_position: Position = "top"
     render: SectionRender = "accordion"
     excluded_fields: list[str] | None = None
     render_kwargs: dict | None = None
```

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form/ids.py` & `dash_pydantic_form-0.1.4/dash_pydantic_form/ids.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form/model_form.py` & `dash_pydantic_form-0.1.4/dash_pydantic_form/model_form.py`

 * *Files 2% similar despite different names*

```diff
@@ -62,22 +62,26 @@
         All-in-one component ID
     form_id: str
         Form ID, can be used to create multiple forms on the same page. When working with databases
         this could be the document / record ID.
     fields_repr: dict[str, dict | BaseField] | None
         Mapping between field name and field representation. If not provided, default field
         representations will be used based on the field annotation.
-        See :meth:`dash_pydantic_form.fields.get_default_repr`.
+        See `fields.get_default_repr`.
     sections: Sections | None
-        List of form sections (optional). See :class:`dash_pydantic_form.form_section.Sections`.
+        List of form sections (optional). See `Sections`.
+    submit_on_enter: bool
+        Whether to submit the form on enter. Default False.
+        Note: this may break the behaviour of some fields (e.g. editable table), use with caution.
     """
 
     class ids:
         """Model form ids."""
 
+        form = partial(form_base_id, "_pydf-form")
         main = partial(form_base_id, "_pydf-main")
         accordion = partial(form_base_id, "_pydf-accordion")
         tabs = partial(form_base_id, "_pydf-tabs")
         steps = partial(form_base_id, "_pydf-steps")
         steps_save = partial(form_base_id, "_pydf-steps-save")
         steps_next = partial(form_base_id, "_pydf-steps-next")
         steps_previous = partial(form_base_id, "_pydf-steps-previous")
@@ -89,14 +93,15 @@
         self,
         item: BaseModel | type[BaseModel],
         aio_id: str,
         form_id: str,
         path: str = "",
         fields_repr: dict[str, Union["BaseField", dict]] | None = None,
         sections: Sections | None = None,
+        submit_on_enter: bool = False,
         discriminator: str | None = None,
     ) -> None:
         from dash_pydantic_form.fields import get_default_repr
 
         with contextlib.suppress(Exception):
             if issubclass(item, BaseModel):
                 item = item.model_construct()
@@ -203,15 +208,25 @@
                         "sections": sections.model_dump(mode="json") if sections else None,
                         "fields_repr": fields_repr_dicts,
                     },
                     id=self.ids.form_specs_store(aio_id, form_id, path),
                 )
             )
 
-        super().__init__(children=children)
+        super().__init__(
+            children=children,
+            **(
+                {
+                    "id": self.ids.form(aio_id, form_id, path),
+                    "data-entersubmits": submit_on_enter,
+                }
+                if not path
+                else {}
+            ),
+        )
 
     @classmethod
     def grid(cls, children: Children, **kwargs):
         """Create the responsive grid for a field."""
         return dmc.SimpleGrid(children, cols={"base": 1, "sm": 4}, className="pydantic-form-grid", **kwargs)
 
     @classmethod
@@ -417,14 +432,21 @@
 clientside_callback(
     ClientsideFunction(namespace="pydf", function_name="getValues"),
     Output(ModelForm.ids.main(MATCH, MATCH), "data"),
     Input(common_ids.value_field(MATCH, MATCH, ALL, ALL, ALL), "value"),
     Input(common_ids.checked_field(MATCH, MATCH, ALL, ALL, ALL), "checked"),
 )
 
+clientside_callback(
+    ClientsideFunction(namespace="pydf", function_name="listenToSubmit"),
+    Output(ModelForm.ids.form(MATCH, MATCH), "id"),
+    Input(ModelForm.ids.form(MATCH, MATCH), "id"),
+    State(ModelForm.ids.form(MATCH, MATCH), "data-entersubmits"),
+)
+
 
 @callback(
     Output(fields.Model.ids.form_wrapper(MATCH, MATCH, MATCH, MATCH), "children"),
     Input(common_ids.value_field(MATCH, MATCH, MATCH, MATCH, "discriminator"), "value"),
     State(ModelForm.ids.main(MATCH, MATCH), "data"),
     State(ModelForm.ids.model_store(MATCH, MATCH), "data"),
     State(ModelForm.ids.form_specs_store(MATCH, MATCH, MATCH), "data"),
```

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form/pydantic_form_scripts.js` & `dash_pydantic_form-0.1.4/dash_pydantic_form/pydantic_form_scripts.js`

 * *Files 2% similar despite different names*

#### js-beautify {}

```diff
@@ -278,8 +278,24 @@
         const trigger = dash_clientside.callback_context.triggered
         if (!trigger || trigger.length === 0) return dash_clientside.no_update
         const trigger_id = JSON.parse(trigger[0].prop_id.split(".")[0])
         if (trigger_id.part.includes("next")) return Math.min(active + 1, nSteps)
         if (trigger_id.part.includes("previous")) return Math.max(0, active - 1)
         return dash_clientside.no_update
     },
+    listenToSubmit: (id, enterSubmits) => {
+        const el = document.getElementById(
+            JSON.stringify(id, Object.keys(id).sort())
+        )
+        if (el && enterSubmits) {
+            el.addEventListener("keypress", event => {
+                if (event.key === "Enter" && event.target.tagName === "INPUT") {
+                    event.preventDefault()
+                    dash_clientside.set_props(id, {
+                        "data-submit": 1
+                    })
+                }
+            })
+        }
+        return dash_clientside.no_update
+    },
 }
```

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form/pydantic_form_styles.css` & `dash_pydantic_form-0.1.4/dash_pydantic_form/pydantic_form_styles.css`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form/utils.py` & `dash_pydantic_form-0.1.4/dash_pydantic_form/utils.py`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/PKG-INFO` & `dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dash-pydantic-form
-Version: 0.1.3
+Version: 0.1.4
 Summary: Create Dash forms from pydantic objects
 Author-email: Renaud Lainé <renaud.laine@enea-consulting.com>
 License: Copyright ENEA Australia Pty Ltd - All Rights Reserved. Proprietary and confidential
 Project-URL: Source, https://github.com/RenaudLN/dash-pydantic-form
 Requires-Python: <3.13,>=3.10
 Description-Content-Type: text/markdown
 Requires-Dist: dash
@@ -42,15 +42,15 @@
 class Employee(BaseModel):
     first_name: str = Field(title="First name")
     last_name: str = Field(title="Last name")
     office: Literal["au", "uk", "us", "fr"] = Field(title="Office")
     joined: date = Field(title="Employment date")
 ```
 
-Then you can get an auto-generated form with `ModelForm`, leveraging [dash-mantine-components](https://dash-mantine-components.com) (vercion 0.14) for form inputs.
+Then you can get an auto-generated form with `ModelForm`, leveraging [dash-mantine-components](https://dash-mantine-components.com) (version 0.14) for form inputs.
 
 ```py
 from dash_pydantic_form import ModelForm
 
 # somewhere in your layout:
 form = ModelForm(
     Employee,
@@ -264,15 +264,15 @@
         "only_bob": fields.Textarea(
             visible=("first_name", "==", "Bob"),
         )
     },
 )
 ```
 
-![Conditionnally visible field](images/conditionnally-visible-field.gif)
+![Conditionally visible field](images/conditionnally-visible-field.gif)
 
 `visible` accepts a boolean, a 3-tuple or list of 3-tuples with format: (field, operator, value). The available operators are:
 * "=="
 * "!="
 * "in"
 * "not in"
 * "array_contains"
```

### Comparing `dash_pydantic_form-0.1.3/dash_pydantic_form.egg-info/SOURCES.txt` & `dash_pydantic_form-0.1.4/dash_pydantic_form.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 .pre-commit-config.yaml
 CHANGELOG.md
 README.md
 pyproject.toml
 usage.py
+.github/workflows/publish.yaml
 .vscode/launch.json
 dash_pydantic_form/__init__.py
 dash_pydantic_form/form_section.py
 dash_pydantic_form/ids.py
 dash_pydantic_form/model_form.py
 dash_pydantic_form/pydantic_form_scripts.js
 dash_pydantic_form/pydantic_form_styles.css
```

### Comparing `dash_pydantic_form-0.1.3/images/conditionnally-visible-field.gif` & `dash_pydantic_form-0.1.4/images/conditionnally-visible-field.gif`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/images/discriminated-union.gif` & `dash_pydantic_form-0.1.4/images/discriminated-union.gif`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/images/editable-table.png` & `dash_pydantic_form-0.1.4/images/editable-table.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/images/form-sections.png` & `dash_pydantic_form-0.1.4/images/form-sections.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/images/model-list.png` & `dash_pydantic_form-0.1.4/images/model-list.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/images/nested-model.png` & `dash_pydantic_form-0.1.4/images/nested-model.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/images/simple-form.png` & `dash_pydantic_form-0.1.4/images/simple-form.png`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/pyproject.toml` & `dash_pydantic_form-0.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dash_pydantic_form-0.1.3/usage.py` & `dash_pydantic_form-0.1.4/usage.py`

 * *Files identical despite different names*

