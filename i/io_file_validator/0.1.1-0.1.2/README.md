# Comparing `tmp/io_file_validator-0.1.1.tar.gz` & `tmp/io_file_validator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "io_file_validator-0.1.1.tar", max compression
+gzip compressed data, was "io_file_validator-0.1.2.tar", max compression
```

## Comparing `io_file_validator-0.1.1.tar` & `io_file_validator-0.1.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     2021 2024-05-19 20:14:40.719542 io_file_validator-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-19 20:14:40.719542 io_file_validator-0.1.1/io_file_validator/__init__.py
--rw-r--r--   0        0        0     4008 2024-05-19 20:14:40.719542 io_file_validator-0.1.1/io_file_validator/validator.py
--rw-r--r--   0        0        0     1071 2024-05-19 20:14:40.719542 io_file_validator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     2711 1970-01-01 00:00:00.000000 io_file_validator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     2440 2024-05-19 20:18:32.790594 io_file_validator-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2024-05-19 20:18:32.790594 io_file_validator-0.1.2/io_file_validator/__init__.py
+-rw-r--r--   0        0        0     4008 2024-05-19 20:18:32.790594 io_file_validator-0.1.2/io_file_validator/validator.py
+-rw-r--r--   0        0        0     1071 2024-05-19 20:18:32.794594 io_file_validator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3130 1970-01-01 00:00:00.000000 io_file_validator-0.1.2/PKG-INFO
```

### Comparing `io_file_validator-0.1.1/README.md` & `io_file_validator-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,64 +1,85 @@
+Metadata-Version: 2.1
+Name: io_file_validator
+Version: 0.1.2
+Summary: File Validator Tool helps you validate your data with a plethora of formats
+Author: Manrique Vargas
+Author-email: machomaxg@gmail.com
+Requires-Python: >=3.10,<4.0
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: pandera[io] (>=0.7.2,<0.8.0)
+Requires-Dist: pipx (>=1.5.0,<2.0.0)
+Requires-Dist: pytest (==7.4.0)
+Requires-Dist: requests (==2.31.0)
+Requires-Dist: validators (>=0.28.1,<0.29.0)
+Requires-Dist: wheel
+Description-Content-Type: text/markdown
+
 # Welcome to IO Bytes File Validator!
 
 
-[![Test](https://github.com/resilientinfrastructure/file-validator/actions/workflows/e2e.yml/badge.svg)](https://github.com/resilientinfrastructure/file-validator/actions/workflows/publish_pypi.yml)
+[![Test](https://github.com/resilientinfrastructure/io-file-validator/actions/workflows/e2e.yml/badge.svg)](https://github.com/resilientinfrastructure/io-file-validator/actions/workflows/publish_pypi.yml)
 
 Data Validator is your go-to tool for clean data ingestion and validation, seamlessly integrating IO Byte Files and validation tools like Panderas to make your data processing tasks a breeze.
 
 ## Features
 
 - **Easy Data Ingestion:** Select your file format (CSV or JSON) and provide a URL to a Panderas schema.
 - **Streamlined Validation:** With just a few clicks, submit your selections and validate your data effortlessly.
 
 
-## file-validator
+## io-file-validator
 
 ## Installation instructions
 
 ```sh
-pip install file-validator
+pip install io-file-validator
 ```
 
 ## Usage instructions
 
-```python
-
-from file_validator.validator import ValidatorDataframe
-
-validated_df = run_validate_file()
-
-st.write(validated_df)
-```
-
-
-## Instructions
 
 ### Step 1: Select File Format
-Choose the file format you want to ingest. Whether it's CSV or JSON, file-validator has got you covered.
+Choose the file format you want to ingest. Whether it's CSV or JSON, io-file-validator has got you covered.
 
 ### Step 2: Provide Panderas Schema URL
 Enter the URL to the Panderas schema you want to use for validation. Don't worry, we support various schema sources to suit your needs.
 
+Sample code:
 
-[Go to Demo](https://youtu.be/9Ry_A9LgrbQ)
 
-[![Video](http://img.youtube.com/vi/9Ry_A9LgrbQ/0.jpg)](https://youtu.be/9Ry_A9LgrbQ)
+```python
 
+from file_validator.validator import ValidatorDataframe
+validator = ValidatorDataframe(
+        url="https://raw.githubusercontent.com/resilientinfrastructure/standards/main/panderas_schema.yml",
+        file_format="csv",
+    )
+parent_path = Path(__file__).parent
+sample_file_path = parent_path.resolve() / "data" / "sample_prices.csv"
+
+with open(sample_file_path, "rb") as sample_file:
+    file_contents = sample_file.read()
+    sample_file_bytesio = BytesIO(file_contents)
+    yaml_content = validator.get_yaml_content(validator.url)
+    validated_df = validator.load_and_validate_file(my_upload=sample_file_bytesio, yaml_content=yaml_content)
+
+```
 
 ## Run Tests
 To ensure everything is functioning smoothly, run the tests using the following commands:
 
 ## Run the App
-Ready to see file-validator in action? Simply run the following command:
-
-
+Ready to see io-file-validator in action? Simply run the following command:
 
 ## Contributions
 We welcome contributions from the community! If you have any ideas, bug fixes, or enhancements, feel free to submit a pull request.
 
 ## Feedback
-We'd love to hear your feedback! Whether you have suggestions for improvement or just want to share your experience using file-validator, don't hesitate to reach out.
+We'd love to hear your feedback! Whether you have suggestions for improvement or just want to share your experience using io-file-validator, don't hesitate to reach out.
 
-Happy data ingesting with file-validator!
+Happy data ingesting with io-file-validator!
 
-Feel free to customize it further to better suit your project's tone and style!
+Feel free to customize it further to better suit your project's tone and style!
```

### Comparing `io_file_validator-0.1.1/io_file_validator/validator.py` & `io_file_validator-0.1.2/io_file_validator/validator.py`

 * *Files identical despite different names*

### Comparing `io_file_validator-0.1.1/pyproject.toml` & `io_file_validator-0.1.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "io_file_validator"
-version = "0.1.1"
+version = "0.1.2"
 description = "File Validator Tool helps you validate your data with a plethora of formats"
 authors = ["Manrique Vargas <machomaxg@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 validators = "^0.28.1"
```

