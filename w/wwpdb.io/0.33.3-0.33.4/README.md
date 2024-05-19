# Comparing `tmp/wwpdb.io-0.33.3.tar.gz` & `tmp/wwpdb_io-0.33.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wwpdb.io-0.33.3.tar", last modified: Fri Feb  2 17:36:55 2024, max compression
+gzip compressed data, was "wwpdb_io-0.33.4.tar", last modified: Sun May 19 17:22:59 2024, max compression
```

## Comparing `wwpdb.io-0.33.3.tar` & `wwpdb_io-0.33.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-02 17:36:55.178523 wwpdb.io-0.33.3/
--rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-02-02 17:36:55.178523 wwpdb.io-0.33.3/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)      764 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/README.md
--rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-02-02 17:36:55.178523 wwpdb.io-0.33.3/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (127)     2027 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-02 17:36:55.170523 wwpdb.io-0.33.3/wwpdb/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-02 17:36:55.174523 wwpdb.io-0.33.3/wwpdb/io/
--rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-02 17:36:55.174523 wwpdb.io-0.33.3/wwpdb/io/cvs/
--rw-r--r--   0 vsts      (1001) docker     (127)    30369 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/cvs/CvsAdmin.py
--rw-r--r--   0 vsts      (1001) docker     (127)     8868 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/cvs/CvsUtility.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/cvs/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-02 17:36:55.174523 wwpdb.io-0.33.3/wwpdb/io/file/
--rwxr-xr-x   0 vsts      (1001) docker     (127)    24712 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/file/DataExchange.py
--rw-r--r--   0 vsts      (1001) docker     (127)    20256 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/file/DataFile.py
--rwxr-xr-x   0 vsts      (1001) docker     (127)    19073 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/file/DataMaintenance.py
--rw-r--r--   0 vsts      (1001) docker     (127)    19244 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/file/ValidateXml.py
--rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/file/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5643 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/file/mmCIFUtil.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-02 17:36:55.174523 wwpdb.io-0.33.3/wwpdb/io/graphics/
--rw-r--r--   0 vsts      (1001) docker     (127)    21126 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/graphics/GraphicsContext3D.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/graphics/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-02 17:36:55.178523 wwpdb.io-0.33.3/wwpdb/io/locator/
--rw-r--r--   0 vsts      (1001) docker     (127)     7982 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/locator/ChemRefPathInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)    46235 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/locator/DataReference.py
--rw-r--r--   0 vsts      (1001) docker     (127)    28453 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/locator/PathInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6396 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/locator/ReleaseFileNames.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3718 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/locator/ReleasePathInfo.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/locator/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2669 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/locator/localFTPPathInfo.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-02 17:36:55.178523 wwpdb.io-0.33.3/wwpdb/io/misc/
--rw-r--r--   0 vsts      (1001) docker     (127)     4800 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/misc/Compression.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3765 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/misc/FormatOut.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2157 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/misc/SendEmail.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/misc/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-02 17:36:55.178523 wwpdb.io-0.33.3/wwpdb/io/sftp/
--rw-r--r--   0 vsts      (1001) docker     (127)     2301 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/sftp/ArchiveIoBase.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7319 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/sftp/ArchiveIoSftp.py
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-02-02 17:35:25.000000 wwpdb.io-0.33.3/wwpdb/io/sftp/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-02-02 17:36:55.178523 wwpdb.io-0.33.3/wwpdb.io.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-02-02 17:36:55.000000 wwpdb.io-0.33.3/wwpdb.io.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     1017 2024-02-02 17:36:55.000000 wwpdb.io-0.33.3/wwpdb.io.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-02 17:36:55.000000 wwpdb.io-0.33.3/wwpdb.io.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-02-02 17:36:31.000000 wwpdb.io-0.33.3/wwpdb.io.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      102 2024-02-02 17:36:55.000000 wwpdb.io-0.33.3/wwpdb.io.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-02-02 17:36:55.000000 wwpdb.io-0.33.3/wwpdb.io.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 17:22:59.406447 wwpdb_io-0.33.4/
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-05-19 17:22:59.406447 wwpdb_io-0.33.4/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      764 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/README.md
+-rw-r--r--   0 vsts      (1001) docker     (127)      108 2024-05-19 17:22:59.406447 wwpdb_io-0.33.4/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2027 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 17:22:59.402447 wwpdb_io-0.33.4/wwpdb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 17:22:59.402447 wwpdb_io-0.33.4/wwpdb/io/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 17:22:59.402447 wwpdb_io-0.33.4/wwpdb/io/cvs/
+-rw-r--r--   0 vsts      (1001) docker     (127)    30537 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/cvs/CvsAdmin.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     8868 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/cvs/CvsUtility.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/cvs/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 17:22:59.402447 wwpdb_io-0.33.4/wwpdb/io/file/
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    24712 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/file/DataExchange.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    20471 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/file/DataFile.py
+-rwxr-xr-x   0 vsts      (1001) docker     (127)    19145 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/file/DataMaintenance.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    19244 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/file/ValidateXml.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      152 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/file/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5643 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/file/mmCIFUtil.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 17:22:59.402447 wwpdb_io-0.33.4/wwpdb/io/graphics/
+-rw-r--r--   0 vsts      (1001) docker     (127)    21126 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/graphics/GraphicsContext3D.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/graphics/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 17:22:59.406447 wwpdb_io-0.33.4/wwpdb/io/locator/
+-rw-r--r--   0 vsts      (1001) docker     (127)     7982 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/locator/ChemRefPathInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    46235 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/locator/DataReference.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    28453 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/locator/PathInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6396 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/locator/ReleaseFileNames.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3718 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/locator/ReleasePathInfo.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/locator/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2669 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/locator/localFTPPathInfo.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 17:22:59.406447 wwpdb_io-0.33.4/wwpdb/io/misc/
+-rw-r--r--   0 vsts      (1001) docker     (127)     4800 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/misc/Compression.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3765 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/misc/FormatOut.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2157 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/misc/SendEmail.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/misc/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 17:22:59.406447 wwpdb_io-0.33.4/wwpdb/io/sftp/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2301 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/sftp/ArchiveIoBase.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7319 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/sftp/ArchiveIoSftp.py
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-05-19 17:21:58.000000 wwpdb_io-0.33.4/wwpdb/io/sftp/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-05-19 17:22:59.406447 wwpdb_io-0.33.4/wwpdb.io.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)      958 2024-05-19 17:22:59.000000 wwpdb_io-0.33.4/wwpdb.io.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1017 2024-05-19 17:22:59.000000 wwpdb_io-0.33.4/wwpdb.io.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-19 17:22:59.000000 wwpdb_io-0.33.4/wwpdb.io.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-05-19 17:22:42.000000 wwpdb_io-0.33.4/wwpdb.io.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      102 2024-05-19 17:22:59.000000 wwpdb_io-0.33.4/wwpdb.io.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        6 2024-05-19 17:22:59.000000 wwpdb_io-0.33.4/wwpdb.io.egg-info/top_level.txt
```

### Comparing `wwpdb.io-0.33.3/LICENSE` & `wwpdb_io-0.33.4/LICENSE`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/PKG-INFO` & `wwpdb_io-0.33.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.io
-Version: 0.33.3
+Version: 0.33.4
 Summary: wwPDB Python Configuration Parsing
 Home-page: https://github.com/rcsb/py-wwpdb_io
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.io-0.33.3/README.md` & `wwpdb_io-0.33.4/README.md`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/setup.py` & `wwpdb_io-0.33.4/setup.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/cvs/CvsAdmin.py` & `wwpdb_io-0.33.4/wwpdb/io/cvs/CvsAdmin.py`

 * *Files 0% similar despite different names*

```diff
@@ -645,54 +645,62 @@
         if self._wrkPath is None:
             self._makeTempWorkingDir()
         errPath = self._getErrorFilePath()
         if self._setCvsRoot():
             cmd = " cd " + os.path.join(self.__sandBoxTopPath, projectDir) + " ; "
             if message is not None and len(message) > 0:
                 qm = ' -m "' + message + '" '
+            else:
+                qm = ""
             cmd += "cvs -d " + self._cvsRoot + " add " + relProjectPath + self._getRedirect(fileNameOut=errPath, fileNameErr=errPath) + " ; "
             cmd += "cvs -d " + self._cvsRoot + " commit " + qm + relProjectPath + self._getRedirect(fileNameOut=errPath, fileNameErr=errPath, append=True) + " ; "
         else:
             cmd = None
         return cmd
 
     def __getCommitCmd(self, projectDir, relProjectPath, message="Automated update"):
         if self._wrkPath is None:
             self._makeTempWorkingDir()
         errPath = self._getErrorFilePath()
         if self._setCvsRoot():
             cmd = " cd " + os.path.join(self.__sandBoxTopPath, projectDir) + " ; "
             if message is not None and len(message) > 0:
                 qm = ' -m "' + message + '" '
+            else:
+                qm = ""
             cmd += "cvs -d " + self._cvsRoot + " commit " + qm + relProjectPath + self._getRedirect(fileNameOut=errPath, fileNameErr=errPath, append=True) + " ; "
         else:
             cmd = None
         return cmd
 
     def __getRemoveCommitCmd(self, projectDir, relProjectPath, message="File removed"):
         if self._wrkPath is None:
             self._makeTempWorkingDir()
         errPath = self._getErrorFilePath()
         if self._setCvsRoot():
             cmd = " cd " + os.path.join(self.__sandBoxTopPath, projectDir) + " ; "
             if message is not None and len(message) > 0:
                 qm = ' -m "' + message + '" '
+            else:
+                qm = ""
             cmd += "cvs -d " + self._cvsRoot + " remove -f " + relProjectPath + self._getRedirect(fileNameOut=errPath, fileNameErr=errPath) + " ; "
             cmd += "cvs -d " + self._cvsRoot + " commit " + qm + relProjectPath + self._getRedirect(fileNameOut=errPath, fileNameErr=errPath, append=True) + " ; "
         else:
             cmd = None
         return cmd
 
     def __getRemoveDirCommitCmd(self, projectDir, relProjectPath, message="Directory removed"):
         if self._wrkPath is None:
             self._makeTempWorkingDir()
         errPath = self._getErrorFilePath()
         if self._setCvsRoot():
             cmd = " cd " + os.path.join(self.__sandBoxTopPath, projectDir) + " ; "
             if message is not None and len(message) > 0:
                 qm = ' -m "' + message + '" '
+            else:
+                qm = ""
             cmd += "cvs -d " + self._cvsRoot + " remove " + relProjectPath + self._getRedirect(fileNameOut=errPath, fileNameErr=errPath) + " ; "
             cmd += "cvs -d " + self._cvsRoot + " commit " + qm + relProjectPath + self._getRedirect(fileNameOut=errPath, fileNameErr=errPath, append=True) + " ; "
             cmd += " rm -rf " + relProjectPath + self._getRedirect(fileNameOut=errPath, fileNameErr=errPath, append=True) + " ; "
         else:
             cmd = None
         return cmd
```

### Comparing `wwpdb.io-0.33.3/wwpdb/io/cvs/CvsUtility.py` & `wwpdb_io-0.33.4/wwpdb/io/cvs/CvsUtility.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/file/DataExchange.py` & `wwpdb_io-0.33.4/wwpdb/io/file/DataExchange.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/file/DataFile.py` & `wwpdb_io-0.33.4/wwpdb/io/file/DataFile.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,17 @@
         else:
             if (self.srcType == "zlib") or (self.srcType == "gzip"):
                 cmdP1 = "zcat " + self.srcPath
             elif self.srcType == "bzip":
                 cmdP1 = "bzcat " + self.srcPath
             elif self.srcType is None:
                 cmdP1 = "cat " + self.srcPath
+            else:
+                # Should provide an error
+                cmdP1 = "cat " + self.srcPath
 
             if op == "copy":
                 redir = " > "
             elif op == "append":
                 redir = " >> "
             else:
                 redir = " > "
@@ -226,14 +229,17 @@
                 cmdP2 = " |  compress -cf - " + redir + self.dstPath
             elif self.dstType == "gzip":
                 cmdP2 = " |  gzip " + redir + self.dstPath
             elif self.dstType == "bzip":
                 cmdP2 = " | bzip2 " + redir + self.dstPath
             elif self.dstType is None:
                 cmdP2 = redir + self.dstPath
+            else:
+                # Should log an error somehow
+                cmdP2 = redir + self.dstPath
 
             cmd = cmdP1 + cmdP2
             return os.system(cmd)
 
     def __compare(self):
         """Compare srcPath to dstPath converting compression according to
            file extension (.Z, .gz, .bz ).
```

### Comparing `wwpdb.io-0.33.3/wwpdb/io/file/DataMaintenance.py` & `wwpdb_io-0.33.4/wwpdb/io/file/DataMaintenance.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,14 +205,17 @@
         try:
             if fileSource == "archive":
                 pth = self.__pI.getArchivePath(dataSetId)
                 snPth = os.path.join(basePath, "archive", dataSetId)
             elif fileSource == "deposit":
                 pth = self.__pI.getDepositPath(dataSetId)
                 snPth = os.path.join(basePath, "deposit", dataSetId)
+            else:
+                pth = "."
+                snPth = "."
 
             fPattern = self.__pI.getFilePathVersionTemplate(
                 dataSetId=dataSetId,
                 wfInstanceId=wfInstanceId,
                 contentType=contentType,
                 formatType=formatType,
                 fileSource=fileSource,
```

### Comparing `wwpdb.io-0.33.3/wwpdb/io/file/ValidateXml.py` & `wwpdb_io-0.33.4/wwpdb/io/file/ValidateXml.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/file/mmCIFUtil.py` & `wwpdb_io-0.33.4/wwpdb/io/file/mmCIFUtil.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/graphics/GraphicsContext3D.py` & `wwpdb_io-0.33.4/wwpdb/io/graphics/GraphicsContext3D.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/locator/ChemRefPathInfo.py` & `wwpdb_io-0.33.4/wwpdb/io/locator/ChemRefPathInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/locator/DataReference.py` & `wwpdb_io-0.33.4/wwpdb/io/locator/DataReference.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/locator/PathInfo.py` & `wwpdb_io-0.33.4/wwpdb/io/locator/PathInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/locator/ReleaseFileNames.py` & `wwpdb_io-0.33.4/wwpdb/io/locator/ReleaseFileNames.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/locator/ReleasePathInfo.py` & `wwpdb_io-0.33.4/wwpdb/io/locator/ReleasePathInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/locator/localFTPPathInfo.py` & `wwpdb_io-0.33.4/wwpdb/io/locator/localFTPPathInfo.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/misc/Compression.py` & `wwpdb_io-0.33.4/wwpdb/io/misc/Compression.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/misc/FormatOut.py` & `wwpdb_io-0.33.4/wwpdb/io/misc/FormatOut.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/misc/SendEmail.py` & `wwpdb_io-0.33.4/wwpdb/io/misc/SendEmail.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/sftp/ArchiveIoBase.py` & `wwpdb_io-0.33.4/wwpdb/io/sftp/ArchiveIoBase.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb/io/sftp/ArchiveIoSftp.py` & `wwpdb_io-0.33.4/wwpdb/io/sftp/ArchiveIoSftp.py`

 * *Files identical despite different names*

### Comparing `wwpdb.io-0.33.3/wwpdb.io.egg-info/PKG-INFO` & `wwpdb_io-0.33.4/wwpdb.io.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wwpdb.io
-Version: 0.33.3
+Version: 0.33.4
 Summary: wwPDB Python Configuration Parsing
 Home-page: https://github.com/rcsb/py-wwpdb_io
 Author: Ezra Peisach
 Author-email: ezra.peisach@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `wwpdb.io-0.33.3/wwpdb.io.egg-info/SOURCES.txt` & `wwpdb_io-0.33.4/wwpdb.io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

