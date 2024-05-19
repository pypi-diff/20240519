# Comparing `tmp/mlcbase-1.2.0a2.tar.gz` & `tmp/mlcbase-1.2.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcbase-1.2.0a2.tar", last modified: Wed May 15 07:28:15 2024, max compression
+gzip compressed data, was "mlcbase-1.2.0a3.tar", last modified: Sun May 19 07:38:57 2024, max compression
```

## Comparing `mlcbase-1.2.0a2.tar` & `mlcbase-1.2.0a3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 07:28:15.485004 mlcbase-1.2.0a2/
--rw-rw-rw-   0        0        0    11558 2024-04-20 07:09:17.000000 mlcbase-1.2.0a2/LICENSE
--rw-rw-rw-   0        0        0       41 2024-05-13 14:46:22.000000 mlcbase-1.2.0a2/MANIFEST.in
--rw-rw-rw-   0        0        0    19168 2024-05-15 07:28:15.482906 mlcbase-1.2.0a2/PKG-INFO
--rw-rw-rw-   0        0        0     5042 2024-05-15 07:27:18.000000 mlcbase-1.2.0a2/README.md
--rw-rw-rw-   0        0        0     1047 2024-05-15 07:27:31.000000 mlcbase-1.2.0a2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-15 07:28:15.485004 mlcbase-1.2.0a2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-05-15 07:28:15.423405 mlcbase-1.2.0a2/src/
-drwxrwxrwx   0        0        0        0 2024-05-15 07:28:15.466844 mlcbase-1.2.0a2/src/mlcbase/
--rw-rw-rw-   0        0        0     3709 2024-05-15 07:19:57.000000 mlcbase-1.2.0a2/src/mlcbase/__init__.py
--rw-rw-rw-   0        0        0     1752 2024-04-20 07:06:20.000000 mlcbase-1.2.0a2/src/mlcbase/conifg.py
--rw-rw-rw-   0        0        0    43449 2024-05-15 07:00:02.000000 mlcbase-1.2.0a2/src/mlcbase/database.py
--rw-rw-rw-   0        0        0    12386 2024-05-15 07:00:05.000000 mlcbase-1.2.0a2/src/mlcbase/email.py
--rw-rw-rw-   0        0        0     2504 2024-05-15 07:01:49.000000 mlcbase-1.2.0a2/src/mlcbase/encrypt_password.py
--rw-rw-rw-   0        0        0     7514 2024-05-15 07:02:11.000000 mlcbase-1.2.0a2/src/mlcbase/entrypt_aes.py
--rw-rw-rw-   0        0        0    22679 2024-05-15 07:02:47.000000 mlcbase-1.2.0a2/src/mlcbase/entrypt_rsa.py
--rw-rw-rw-   0        0        0    13142 2024-05-15 07:04:34.000000 mlcbase-1.2.0a2/src/mlcbase/file.py
--rw-rw-rw-   0        0        0     6969 2024-05-15 07:05:32.000000 mlcbase-1.2.0a2/src/mlcbase/image_io.py
--rw-rw-rw-   0        0        0    12280 2024-05-15 07:06:21.000000 mlcbase-1.2.0a2/src/mlcbase/loading.py
--rw-rw-rw-   0        0        0    10177 2024-05-15 07:14:59.000000 mlcbase-1.2.0a2/src/mlcbase/logger.py
--rw-rw-rw-   0        0        0     6507 2024-05-13 14:41:07.000000 mlcbase-1.2.0a2/src/mlcbase/misc.py
--rw-rw-rw-   0        0        0    13544 2024-05-15 07:08:16.000000 mlcbase-1.2.0a2/src/mlcbase/otp.py
--rw-rw-rw-   0        0        0     3148 2024-05-15 07:16:32.000000 mlcbase-1.2.0a2/src/mlcbase/register.py
--rw-rw-rw-   0        0        0    23594 2024-05-15 07:10:39.000000 mlcbase-1.2.0a2/src/mlcbase/remote_connect.py
--rw-rw-rw-   0        0        0     6392 2024-05-15 07:14:32.000000 mlcbase-1.2.0a2/src/mlcbase/timer.py
--rw-rw-rw-   0        0        0   179948 2024-05-15 07:09:43.000000 mlcbase-1.2.0a2/src/mlcbase/vault.py
-drwxrwxrwx   0        0        0        0 2024-05-15 07:28:15.480799 mlcbase-1.2.0a2/src/mlcbase.egg-info/
--rw-rw-rw-   0        0        0    19168 2024-05-15 07:28:15.000000 mlcbase-1.2.0a2/src/mlcbase.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      619 2024-05-15 07:28:15.000000 mlcbase-1.2.0a2/src/mlcbase.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 07:28:15.000000 mlcbase-1.2.0a2/src/mlcbase.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      126 2024-05-15 07:28:15.000000 mlcbase-1.2.0a2/src/mlcbase.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-05-15 07:28:15.000000 mlcbase-1.2.0a2/src/mlcbase.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-19 07:38:57.902948 mlcbase-1.2.0a3/
+-rw-rw-rw-   0        0        0    11558 2024-04-20 07:09:17.000000 mlcbase-1.2.0a3/LICENSE
+-rw-rw-rw-   0        0        0       41 2024-05-13 14:46:22.000000 mlcbase-1.2.0a3/MANIFEST.in
+-rw-rw-rw-   0        0        0    19168 2024-05-19 07:38:57.902440 mlcbase-1.2.0a3/PKG-INFO
+-rw-rw-rw-   0        0        0     5042 2024-05-15 07:27:18.000000 mlcbase-1.2.0a3/README.md
+-rw-rw-rw-   0        0        0     1047 2024-05-19 07:38:29.000000 mlcbase-1.2.0a3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 07:38:57.902948 mlcbase-1.2.0a3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-19 07:38:57.885139 mlcbase-1.2.0a3/src/
+drwxrwxrwx   0        0        0        0 2024-05-19 07:38:57.897853 mlcbase-1.2.0a3/src/mlcbase/
+-rw-rw-rw-   0        0        0     3709 2024-05-19 07:32:39.000000 mlcbase-1.2.0a3/src/mlcbase/__init__.py
+-rw-rw-rw-   0        0        0     1752 2024-04-20 07:06:20.000000 mlcbase-1.2.0a3/src/mlcbase/conifg.py
+-rw-rw-rw-   0        0        0    43449 2024-05-19 07:18:36.000000 mlcbase-1.2.0a3/src/mlcbase/database.py
+-rw-rw-rw-   0        0        0    12386 2024-05-15 07:00:05.000000 mlcbase-1.2.0a3/src/mlcbase/email.py
+-rw-rw-rw-   0        0        0     2504 2024-05-15 07:01:49.000000 mlcbase-1.2.0a3/src/mlcbase/encrypt_password.py
+-rw-rw-rw-   0        0        0     7514 2024-05-15 07:02:11.000000 mlcbase-1.2.0a3/src/mlcbase/entrypt_aes.py
+-rw-rw-rw-   0        0        0    22679 2024-05-15 07:02:47.000000 mlcbase-1.2.0a3/src/mlcbase/entrypt_rsa.py
+-rw-rw-rw-   0        0        0    13142 2024-05-15 07:04:34.000000 mlcbase-1.2.0a3/src/mlcbase/file.py
+-rw-rw-rw-   0        0        0     6969 2024-05-15 07:05:32.000000 mlcbase-1.2.0a3/src/mlcbase/image_io.py
+-rw-rw-rw-   0        0        0    12787 2024-05-19 07:31:33.000000 mlcbase-1.2.0a3/src/mlcbase/loading.py
+-rw-rw-rw-   0        0        0    10177 2024-05-15 07:14:59.000000 mlcbase-1.2.0a3/src/mlcbase/logger.py
+-rw-rw-rw-   0        0        0     6507 2024-05-13 14:41:07.000000 mlcbase-1.2.0a3/src/mlcbase/misc.py
+-rw-rw-rw-   0        0        0    13544 2024-05-15 07:08:16.000000 mlcbase-1.2.0a3/src/mlcbase/otp.py
+-rw-rw-rw-   0        0        0     3148 2024-05-15 07:16:32.000000 mlcbase-1.2.0a3/src/mlcbase/register.py
+-rw-rw-rw-   0        0        0    23594 2024-05-15 07:10:39.000000 mlcbase-1.2.0a3/src/mlcbase/remote_connect.py
+-rw-rw-rw-   0        0        0     6392 2024-05-15 07:14:32.000000 mlcbase-1.2.0a3/src/mlcbase/timer.py
+-rw-rw-rw-   0        0        0   179948 2024-05-15 07:09:43.000000 mlcbase-1.2.0a3/src/mlcbase/vault.py
+drwxrwxrwx   0        0        0        0 2024-05-19 07:38:57.901444 mlcbase-1.2.0a3/src/mlcbase.egg-info/
+-rw-rw-rw-   0        0        0    19168 2024-05-19 07:38:57.000000 mlcbase-1.2.0a3/src/mlcbase.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      619 2024-05-19 07:38:57.000000 mlcbase-1.2.0a3/src/mlcbase.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 07:38:57.000000 mlcbase-1.2.0a3/src/mlcbase.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      126 2024-05-19 07:38:57.000000 mlcbase-1.2.0a3/src/mlcbase.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-05-19 07:38:57.000000 mlcbase-1.2.0a3/src/mlcbase.egg-info/top_level.txt
```

### Comparing `mlcbase-1.2.0a2/LICENSE` & `mlcbase-1.2.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/PKG-INFO` & `mlcbase-1.2.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcbase
-Version: 1.2.0a2
+Version: 1.2.0a3
 Summary: The base module of all MuLingCloud modules and applications.
 Author-email: Weiming Chen <wm_chen@yeah.net>, Yuanshuang Sun <sunsun5544@126.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mlcbase-1.2.0a2/README.md` & `mlcbase-1.2.0a3/README.md`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/pyproject.toml` & `mlcbase-1.2.0a3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlcbase"
-version = "1.2.0a2"
+version = "1.2.0a3"
 authors = [
     {name = "Weiming Chen", email = "wm_chen@yeah.net"},
     {name = "Yuanshuang Sun", email = "sunsun5544@126.com"}
 ]
 description = "The base module of all MuLingCloud modules and applications."
 readme = {"file" = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.7"
```

### Comparing `mlcbase-1.2.0a2/src/mlcbase/__init__.py` & `mlcbase-1.2.0a3/src/mlcbase/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,15 +44,15 @@
     "VaultSecretEngineKV2", "VaultSecretEngineTOTP", "VaultSecretEngineTransit", "MySQLAPI", "SQLiteAPI", 
     "SSH", "SFTP", "SMTPAPI", "Registry", "DATABASE", "EMAIL", "SECRET", "FILEOPT", "IMAGEIO", "REMOTE", "is_type", 
     "is_bytes", "is_str", "is_int", "is_float", "is_bool", "is_list", "is_dict", "is_tuple", "is_path", "is_url", 
     "is_base64", "random_hex", "random_otp_secret", "get_mac_address", "is_canonical_version", "parse_version"
 ]
 
 
-__version__ = "1.2.0a2"
+__version__ = "1.2.0a3"
 TYPE_NAME = "module"
 NAME = "mlcbase"
 DESCRIPTION = "The base module of all MuLingCloud modules and applications."
 
 
 if not hasattr(__import__(NAME), NAME):
     from colorama import Fore
```

### Comparing `mlcbase-1.2.0a2/src/mlcbase/conifg.py` & `mlcbase-1.2.0a3/src/mlcbase/conifg.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/src/mlcbase/database.py` & `mlcbase-1.2.0a3/src/mlcbase/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,27 +42,27 @@
 class MySQLAPI:
     def __init__(self, 
                  host: str, 
                  port: int,
                  user: str,
                  database: str,
                  password: str,
-                 charset: str = 'utf-8',
+                 charset: str = 'utf8',
                  work_dir: Optional[PathLikeType] = None, 
                  logger: Optional[Logger] = None,
                  quiet: bool = False):
         """An api for MySQL database
 
         Args:
             host (str)
             port (int)
             user (str)
             database (str)
             password (str)
-            charset (str, optional): Defaults to 'utf-8'.
+            charset (str, optional): Defaults to 'utf8'.
             work_dir (Optional[PathLikeType], optional): will save the log file to "work_dir/log/" if 
                                                          work_dir is specified. Defaults to None.
             logger (Optional[Logger], optional): Defaults to None.
             quiet (bool, optional): whether the logger to run in quiet mode. Defaults to False.
         """
         self.work_dir = Path(work_dir) if work_dir is not None else None
         self.logger = self._set_logger(logger, quiet)
@@ -77,17 +77,18 @@
             self.logger.success('database connected')
             self.__host = host
             self.__port = port
             self.__user = user
             self.__database = database
             self.__password = password
             self.__charset = charset
+            self.is_connect = True
         except ConnectionError as e:
             self.logger.error(f'database connect error: {str(e)}')
-            raise ConnectionError(f'database connect error: {str(e)}')
+            self.is_connect = False
         
     def ping(self):
         try:
             self.conn.ping()
         except:
             self.logger.info('reconnecting to database...')
             del self.conn
@@ -653,17 +654,18 @@
             if self.in_memory:
                 path = ":memory:"
             else:
                 path = self.db_path
             self.conn = sqlite3.connect(path)
             self.cursor = self.conn.cursor()
             self.logger.success('database connected')
+            self.is_connect = True
         except ConnectionError as e:
             self.logger.error(f'database connect error: {str(e)}')
-            raise ConnectionError(f'database connect error: {str(e)}')
+            self.is_connect = False
         
     def create_table(self,
                      table_name: Optional[str] = None, 
                      table_config: Optional[List[dict]] = None, 
                      sql_command: Optional[str] = None,
                      exist_ok: bool = True):
         """create data table
```

### Comparing `mlcbase-1.2.0a2/src/mlcbase/email.py` & `mlcbase-1.2.0a3/src/mlcbase/email.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/src/mlcbase/encrypt_password.py` & `mlcbase-1.2.0a3/src/mlcbase/encrypt_password.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/src/mlcbase/entrypt_aes.py` & `mlcbase-1.2.0a3/src/mlcbase/entrypt_aes.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/src/mlcbase/entrypt_rsa.py` & `mlcbase-1.2.0a3/src/mlcbase/entrypt_rsa.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/src/mlcbase/file.py` & `mlcbase-1.2.0a3/src/mlcbase/file.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/src/mlcbase/image_io.py` & `mlcbase-1.2.0a3/src/mlcbase/image_io.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/src/mlcbase/loading.py` & `mlcbase-1.2.0a3/src/mlcbase/loading.py`

 * *Files 8% similar despite different names*

```diff
@@ -33,29 +33,32 @@
 from .register import FILEOPT
 from .misc import is_dict, is_list, is_int
 
 PathLikeType = Union[str, Path]
 
 
 @FILEOPT.register_module()
-def load_json(path: PathLikeType, logger: Optional[Logger] = None):
+def load_json(path: PathLikeType, 
+              encoding: Optional[str] = None,
+              logger: Optional[Logger] = None):
     """load json file to a dict
 
     Args:
         path (PathLikeType)
+        encoding (str, optional): Defaults to None.
         logger (Optional[Logger], optional): Defaults to None.
 
     Returns:
         ConfigDict or None: return a ConfigDict if success, return None if fail
     """
     assert Path(path).exists(), 'json load error: the file is not exist'
     assert Path(path).suffix.lower() == '.json', 'json load error: the suffix must be .json'
 
     try:
-        with open(path, 'r') as f:
+        with open(path, 'r', encoding=encoding) as f:
             data = json.load(f)
         if is_list(data):
             return data
         else:
             return ConfigDict(data)
     except OSError as e:
         if logger is not None:
@@ -64,59 +67,64 @@
     
 
 @FILEOPT.register_module()
 def save_json(data: Union[list, dict],
               path: PathLikeType,
               ensure_ascii: bool = True,
               indent: Optional[int] = 4,
-              logger: Optional[Logger] = None,):
+              encoding: Optional[str] = None,
+              logger: Optional[Logger] = None):
     """save data to a json file
 
     Args:
         data (Union[List, Dict])
         path (PathLikeType)
         ensure_ascii (Optional[bool]): when ensure_ascii=False, allow non-ASCII characters in the file. 
                                        Defaults to True.
         indent (Optional[int]): spaces to use for indentation. Defaults to 4.
+        encoding (str, optional): Defaults to None.
         logger (Optional[Logger]): Defaults to None.
 
     Returns:
         bool: return True if success, return False if fail
     """
     assert is_dict(data) or is_list(data), 'json save error: the saving data must be "dict" or "list" type'
     assert Path(path).suffix.lower() == '.json', 'json save error: the suffix must be .json'
     if indent is not None:
         assert is_int(indent), 'json save error: the indent must be "int" type'
     
     try:
-        with open(path, 'w') as f:
+        with open(path, 'w', encoding=encoding) as f:
             json.dump(data, f, ensure_ascii=ensure_ascii, indent=indent)
         return True
     except OSError as e:
         if logger is not None:
             logger.error(f'json save error: {str(e)}')
         return False
     
 
 @FILEOPT.register_module()
-def load_yaml(path: PathLikeType, logger: Optional[Logger] = None):
+def load_yaml(path: PathLikeType, 
+              encoding: Optional[str] = None,
+              logger: Optional[Logger] = None):
     """load yaml file to a dict
 
     Args:
         path (PathLikeType)
+        encoding (str, optional): Defaults to None.
         logger (Optional[Logger], optional): Defaults to None.
 
     Returns:
         ConfigDict or None: return a ConfigDict if success, return None if fail
     """
     assert Path(path).exists(), 'yaml load error: the file is not exist'
     assert Path(path).suffix.lower() in [".yml", ".yaml"], 'yaml load error: the suffix must be .yml or .yaml'
 
     try:
-        with open(path, 'r') as f:
+        with open(path, 'r', encoding=encoding) as f:
             data = yaml.load(f, Loader=yaml.SafeLoader)
         if is_list(data):
             return data
         else:
             return ConfigDict(data)
     except OSError as e:
         if logger is not None:
@@ -124,32 +132,34 @@
         return None
     
 
 @FILEOPT.register_module()
 def save_yaml(data: Union[dict, list], 
               path: PathLikeType, 
               allow_unicode: bool = False,
+              encoding: Optional[str] = None,
               logger: Optional[Logger] = None):
     """save data to a yaml file
 
     Args:
         data (dict)
         path (PathLikeType)
         allow_unicode (bool, optional): when allow_unicode=True, allow unicode characters 
                                         in the file. Defaults to False.
+        encoding (str, optional): Defaults to None.
         logger (Optional[Logger], optional): Defaults to None.
 
     Returns:
         bool: return True if success, return False if fail
     """
     assert is_dict(data) or is_list(data), 'yaml save error: the saving data must be "dict" or "list" type'
     assert Path(path).suffix.lower() in [".yml", ".yaml"], 'yaml save error: the suffix must be .yml or .yaml'
 
     try:
-        with open(path, 'w') as f:
+        with open(path, 'w', encoding=encoding) as f:
             yaml.dump(data, f, Dumper=yaml.SafeDumper, allow_unicode=allow_unicode)
         return True
     except OSError as e:
         if logger is not None:
             logger.error(f'yaml save error: {str(e)}')
         return False
```

### Comparing `mlcbase-1.2.0a2/src/mlcbase/logger.py` & `mlcbase-1.2.0a3/src/mlcbase/logger.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/src/mlcbase/misc.py` & `mlcbase-1.2.0a3/src/mlcbase/misc.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/src/mlcbase/otp.py` & `mlcbase-1.2.0a3/src/mlcbase/otp.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/src/mlcbase/register.py` & `mlcbase-1.2.0a3/src/mlcbase/register.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/src/mlcbase/remote_connect.py` & `mlcbase-1.2.0a3/src/mlcbase/remote_connect.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/src/mlcbase/timer.py` & `mlcbase-1.2.0a3/src/mlcbase/timer.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/src/mlcbase/vault.py` & `mlcbase-1.2.0a3/src/mlcbase/vault.py`

 * *Files identical despite different names*

### Comparing `mlcbase-1.2.0a2/src/mlcbase.egg-info/PKG-INFO` & `mlcbase-1.2.0a3/src/mlcbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcbase
-Version: 1.2.0a2
+Version: 1.2.0a3
 Summary: The base module of all MuLingCloud modules and applications.
 Author-email: Weiming Chen <wm_chen@yeah.net>, Yuanshuang Sun <sunsun5544@126.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 https://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `mlcbase-1.2.0a2/src/mlcbase.egg-info/SOURCES.txt` & `mlcbase-1.2.0a3/src/mlcbase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

