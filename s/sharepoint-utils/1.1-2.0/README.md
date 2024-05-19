# Comparing `tmp/sharepoint_utils-1.1.tar.gz` & `tmp/sharepoint_utils-2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sharepoint_utils-1.1.tar", last modified: Sat Apr 27 10:28:25 2024, max compression
+gzip compressed data, was "sharepoint_utils-2.0.tar", last modified: Sun May 19 08:59:55 2024, max compression
```

## Comparing `sharepoint_utils-1.1.tar` & `sharepoint_utils-2.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-04-27 10:28:25.104755 sharepoint_utils-1.1/
--rw-rw-rw-   0        0        0     1083 2024-04-16 16:34:38.000000 sharepoint_utils-1.1/LICENSE.txt
--rw-rw-rw-   0        0        0     2104 2024-04-27 10:28:25.102964 sharepoint_utils-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-04-27 10:28:25.104755 sharepoint_utils-1.1/setup.cfg
--rw-rw-rw-   0        0        0      791 2024-04-27 10:24:50.000000 sharepoint_utils-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-04-27 10:28:25.074841 sharepoint_utils-1.1/sharepoint_utils/
--rw-rw-rw-   0        0        0     6128 2024-04-21 08:21:04.000000 sharepoint_utils-1.1/sharepoint_utils/ModuleRead.py
--rw-rw-rw-   0        0        0      416 2024-04-27 10:24:37.000000 sharepoint_utils-1.1/sharepoint_utils/__init__.py
--rw-rw-rw-   0        0        0     4333 2024-04-27 10:24:08.000000 sharepoint_utils-1.1/sharepoint_utils/main.py
-drwxrwxrwx   0        0        0        0 2024-04-27 10:28:25.101981 sharepoint_utils-1.1/sharepoint_utils.egg-info/
--rw-rw-rw-   0        0        0     2104 2024-04-27 10:28:24.000000 sharepoint_utils-1.1/sharepoint_utils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      304 2024-04-27 10:28:24.000000 sharepoint_utils-1.1/sharepoint_utils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-27 10:28:24.000000 sharepoint_utils-1.1/sharepoint_utils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-04-27 10:28:24.000000 sharepoint_utils-1.1/sharepoint_utils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       17 2024-04-27 10:28:24.000000 sharepoint_utils-1.1/sharepoint_utils.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 08:59:55.931819 sharepoint_utils-2.0/
+-rw-rw-rw-   0        0        0     1083 2024-04-16 16:34:38.000000 sharepoint_utils-2.0/LICENSE.txt
+-rw-rw-rw-   0        0        0     2777 2024-05-19 08:59:55.930822 sharepoint_utils-2.0/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-19 08:59:55.932918 sharepoint_utils-2.0/setup.cfg
+-rw-rw-rw-   0        0        0      785 2024-05-19 08:55:14.000000 sharepoint_utils-2.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-19 08:59:55.867405 sharepoint_utils-2.0/sharepoint_utils/
+-rw-rw-rw-   0        0        0     2269 2024-05-19 08:50:52.000000 sharepoint_utils-2.0/sharepoint_utils/ModuleGet.py
+-rw-rw-rw-   0        0        0     5437 2024-05-19 08:48:06.000000 sharepoint_utils-2.0/sharepoint_utils/ModuleRead.py
+-rw-rw-rw-   0        0        0      529 2024-05-19 08:51:30.000000 sharepoint_utils-2.0/sharepoint_utils/__init__.py
+-rw-rw-rw-   0        0        0     4326 2024-05-19 08:23:44.000000 sharepoint_utils-2.0/sharepoint_utils/main.py
+drwxrwxrwx   0        0        0        0 2024-05-19 08:59:55.928814 sharepoint_utils-2.0/sharepoint_utils.egg-info/
+-rw-rw-rw-   0        0        0     2777 2024-05-19 08:59:55.000000 sharepoint_utils-2.0/sharepoint_utils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      334 2024-05-19 08:59:55.000000 sharepoint_utils-2.0/sharepoint_utils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 08:59:55.000000 sharepoint_utils-2.0/sharepoint_utils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-19 08:59:55.000000 sharepoint_utils-2.0/sharepoint_utils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       17 2024-05-19 08:59:55.000000 sharepoint_utils-2.0/sharepoint_utils.egg-info/top_level.txt
```

### Comparing `sharepoint_utils-1.1/LICENSE.txt` & `sharepoint_utils-2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sharepoint_utils-1.1/setup.py` & `sharepoint_utils-2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 
 # Read the contents of README.md
 with open('README.md', 'r', encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='sharepoint_utils',
-    version='1.1',
+    version='2.0',
     author='Omkar Sutar',
-    description='Utility functions for working with SharePoint files',
+    description='Utility functions for working with SharePoint',
     long_description=long_description,
     long_description_content_type='text/markdown',  # This tells setuptools that the long description is in Markdown format
     packages=find_packages(),
     install_requires=[
         'pandas',
         'Office365-REST-Python-Client'
     ],
```

### Comparing `sharepoint_utils-1.1/sharepoint_utils/ModuleRead.py` & `sharepoint_utils-2.0/sharepoint_utils/ModuleRead.py`

 * *Files 24% similar despite different names*

```diff
@@ -53,74 +53,58 @@
     # Handle any exceptions that may occur during file reading
     except Exception as e:
         print('Problem reading files: ', e)
         return None
 
 #########################################################################################
 
-def get_folder_urls(ctx, document_library_relative_url: str):
+def read_file_from_different_library(ctx, file_url):
     """
-    Function to return a list of URLs of folders present in a given path in SharePoint.
+    Reads a file from custom library in SharePoint and returns its content as a Pandas DataFrame.
 
-    Parameters:
-        - ctx: SharePoint context object.
-        - document_library_relative_url (str): Relative URL of the document library.
+    Args:
+        ctx: SharePoint context (e.g., client context)
+        file_url: URL of the file on SharePoint
 
     Returns:
-        - List[str]: List of URLs of folders present in the given path.
-    """
-    # Getting the root folder of the document library
-    root_folder = ctx.web.get_folder_by_server_relative_path(document_library_relative_url)
-    ctx.load(root_folder, ["Folders"])
-    ctx.execute_query()
-
-    # Extracting the paths of Level 1 folders within the root folder
-    folder_urls = [f'{document_library_relative_url}/{folder.name}' for folder in root_folder.folders]
-    
-    return folder_urls
-
-# Example usage:
-# Assuming you have ctx already defined
-# ctx = get_sharepoint_context()  # Get SharePoint context
-
-#########################################################################################
-
-def get_file_paths(ctx, subfolder_urls_files: str):
+        pd.DataFrame: DataFrame containing the file content
     """
-    Function to return a list of paths of files present in a given subfolder in SharePoint.
-
-    Parameters:
-        - ctx: SharePoint context object.
-        - subfolder_urls_files (str): Relative URL of the subfolder containing files.
+    # Create a MemoryStream to hold the file content
+    memory_stream = BytesIO()
 
-    Returns:
-        - List[str]: List of paths of files present in the given subfolder.
-    """
-    # Get the root folder of the Level 2 folder
-    root_folder_level2 = ctx.web.get_folder_by_server_relative_path(subfolder_urls_files)
-    ctx.load(root_folder_level2, ["Files"])
-    ctx.execute_query()
-
-    # Initialize a list to store file paths
-    file_paths = []
-
-    # Iterate over files within the Level 2 folder
-    for file in root_folder_level2.files:
-        # Append the path of each file to the list
-        file_paths.append(f'{subfolder_urls_files}/{file.name}')
-
-    return file_paths
-
-# Example usage:
-# Assuming you have ctx already defined
-# ctx = get_sharepoint_context()  # Get SharePoint context
+    try:
+        # Download the file from SharePoint and write it to the MemoryStream
+        ctx.web.get_file_by_server_relative_path(file_url).download(memory_stream).execute_query()
+    except Exception as e:
+        print(f"Error downloading the file: {e}")
+        return None
 
+    try:
+        # Assuming 'file_content' contains your CSV or Excel data
+        file_content = memory_stream.getvalue()
+        
+        if file_url.lower().endswith(".csv"):
+            df = pd.read_csv(BytesIO(file_content))
+        else:
+            df = pd.read_excel(BytesIO(file_content))
+
+        return df
+    except pd.errors.ParserError as e:
+        print(f"Error parsing the file content: {e}")
+        return None
+    except Exception as e:
+        print(f"Unexpected error: {e}")
+        return None
+    finally:
+        # Close the MemoryStream (optional, but recommended)
+        memory_stream.close()
+        
 #########################################################################################
 
-def read_file_from_sharepoint(ctx, file_url, sheet_name=0):
+def read_file_from_default_library(ctx, file_url, sheet_name=0):
     """
     Function to read a file from SharePoint and return its content as a pandas DataFrame.
 
     Parameters:
         - file_url (str): URL of the file in SharePoint.
         - ctx: SharePoint context object.
         - sheet_name (str or int, optional): Name or index of the sheet to read (for Excel files). Defaults to 0.
```

### Comparing `sharepoint_utils-1.1/sharepoint_utils/main.py` & `sharepoint_utils-2.0/sharepoint_utils/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         return ctx
     else:
         print("Failed to authenticate with SharePoint.")
         return None
 
 #########################################################################################
 
-def upload_dataframe_to_sharepoint(ctx, folder_path, dataframe, file_name):
+def upload_dataframe_as_csv(ctx, folder_path, dataframe, file_name):
     """
     This function uploads a pandas DataFrame to a SharePoint folder as a CSV file.
 
     Parameters:
     ctx (ClientContext): The SharePoint ClientContext.
     folder_path (str): The server-relative URL of the SharePoint folder where the file will be uploaded.
     dataframe (DataFrame): The pandas DataFrame to be uploaded.
```

### Comparing `sharepoint_utils-1.1/sharepoint_utils.egg-info/PKG-INFO` & `sharepoint_utils-2.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,65 +1,71 @@
 Metadata-Version: 2.1
-Name: sharepoint-utils
-Version: 1.1
-Summary: Utility functions for working with SharePoint files
+Name: sharepoint_utils
+Version: 2.0
+Summary: Utility functions for working with SharePoint
 Author: Omkar Sutar
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
+
 # SharePoint Utility
 
-This Python package provides utility functions for working with SharePoint files & folders.
+The SharePoint Utility is a Python package designed to simplify the process of working with files and folders in SharePoint. It provides a set of utility functions that allow you to connect to SharePoint, read and upload files, and perform various operations on files and folders.
 
 ## Installation
-  
+
+To install the SharePoint Utility package, use the following pip command in your terminal:
+
 ```bash
-!pip  install  sharepoint-utils
+!pip install sharepoint-utils
 ```
+
 ## Usage
 
-### available functions
+The SharePoint Utility package provides several functions for connecting to SharePoint, reading and uploading files, and working with files and folders.
+
+### Available Functions
+
 ```python
-# functions for connection, reading and uploading files.
-from sharepoint_utils import  connect_to_sharepoint
-from sharepoint_utils import  upload_dataframe_to_sharepoint
-from sharepoint_utils import  read_file_from_sharepoint
-
-# functions for reading files and folders.
-from sharepoint_utils import  combine_files_into_dataframe
-from sharepoint_utils import  get_folder_urls
-from sharepoint_utils import  get_file_paths
-from sharepoint_utils import  copy_files_within_folders
+# Functions for establishing a connection, reading files, and uploading files.
+from sharepoint_utils import read_file_from_different_library
+from sharepoint_utils import read_file_from_default_library
+from sharepoint_utils import combine_files_into_dataframe
+from sharepoint_utils import copy_files_within_folders
+from sharepoint_utils import upload_dataframe_as_csv
+from sharepoint_utils import connect_to_sharepoint
+from sharepoint_utils import get_folder_url
+from sharepoint_utils import get_file_path
 ```
+
 ### Usage Examples
 
 ```python
-# Create connection to sharepoint
+# Establish a connection to SharePoint.
 sharepoint_ctx = connect_to_sharepoint('your_username', 'your_password', 'https://your_sharepoint_site_url')
 
-# Combine files into a DataFrame
+# Combine files into a DataFrame.
 folder_path = 'relative/folder/path'
 df = combine_files_into_dataframe(sharepoint_ctx, folder_path)
 
-# Upload DataFrame to SharePoint folder as a csv file
+# Upload a DataFrame to a SharePoint folder as a CSV file.
 folder_path = '/folder_path/'
-upload_dataframe_to_sharepoint(ctx, folder, df, 'your_file_name.csv')
+upload_dataframe_as_csv(ctx, folder, df, 'your_file_name.csv')
 
-# get sharepoint folder url as a list
-folder_urls  =  get_folder_urls(sharepoint_ctx, document_library_relative_url)
+# Retrieve SharePoint folder URLs as a list.
+folder_urls = get_folder_url(sharepoint_ctx, document_library_relative_url)
 print(folder_urls)
 
-# get sharepoint file path as a list
-file_paths  =  get_file_paths(sharepoint_ctx, subfolder_urls_files)
+# Retrieve SharePoint file paths as a list.
+file_paths = get_file_path(sharepoint_ctx, subfolder_urls_files)
 print(file_paths)
 
-# copy files from one folder to another within sharepoint site
+# Copy files from one folder to another within the SharePoint site.
 copy_files_within_folders(ctx, filepath , files_upload_to_path)
-``` 
-### Contributing
+```
 
-  
+## Contributing
 
-Contributions are welcome! If you have any suggestions or find any issues, please feel free to contact me.
+Contributions to the SharePoint Utility package are always welcome! If you have any suggestions for improvements or if you encounter any issues while using the package, please feel free to contact me. Your feedback and contributions will help make this package even better and more useful for everyone.
```

