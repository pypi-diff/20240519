# Comparing `tmp/tencentcloud-sdk-python-sms-3.0.998.tar.gz` & `tmp/tencentcloud-sdk-python-sms-3.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/tencentcloud-sdk-python-sms-3.0.998.tar", last modified: Fri Oct 13 00:34:58 2023, max compression
+gzip compressed data, was "dist/tencentcloud-sdk-python-sms-3.0.999.tar", last modified: Mon Oct 16 00:34:10 2023, max compression
```

## Comparing `tencentcloud-sdk-python-sms-3.0.998.tar` & `tencentcloud-sdk-python-sms-3.0.999.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:34:58.000000 tencentcloud-sdk-python-sms-3.0.998/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:34:58.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud/
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-13 00:34:57.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:34:58.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:34:58.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20210111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:34:57.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20210111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104906 2023-10-13 00:34:57.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20210111/models.py
--rw-r--r--   0 root         (0) root         (0)    19344 2023-10-13 00:34:57.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20210111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28405 2023-10-13 00:34:57.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20210111/sms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:34:57.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:34:58.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20190711/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:34:57.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20190711/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93677 2023-10-13 00:34:57.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20190711/models.py
--rw-r--r--   0 root         (0) root         (0)    18522 2023-10-13 00:34:57.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20190711/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    26631 2023-10-13 00:34:57.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20190711/sms_client.py
--rw-r--r--   0 root         (0) root         (0)     1659 2023-10-13 00:34:58.000000 tencentcloud-sdk-python-sms-3.0.998/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      737 2023-10-13 00:34:57.000000 tencentcloud-sdk-python-sms-3.0.998/README.rst
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:34:58.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud_sdk_python_sms.egg-info/
--rw-r--r--   0 root         (0) root         (0)       13 2023-10-13 00:34:58.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud_sdk_python_sms.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       39 2023-10-13 00:34:58.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud_sdk_python_sms.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1659 2023-10-13 00:34:58.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud_sdk_python_sms.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      653 2023-10-13 00:34:58.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 00:34:58.000000 tencentcloud-sdk-python-sms-3.0.998/tencentcloud_sdk_python_sms.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       88 2023-10-13 00:34:58.000000 tencentcloud-sdk-python-sms-3.0.998/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1072 2023-10-13 00:34:57.000000 tencentcloud-sdk-python-sms-3.0.998/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud/
+-rw-r--r--   0 root         (0) root         (0)      630 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20210111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20210111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104906 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20210111/models.py
+-rw-r--r--   0 root         (0) root         (0)    19344 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20210111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28405 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20210111/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20190711/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20190711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93677 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20190711/models.py
+-rw-r--r--   0 root         (0) root         (0)    18522 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20190711/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    26631 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20190711/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      737 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud_sdk_python_sms.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       13 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud_sdk_python_sms.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud_sdk_python_sms.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1659 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud_sdk_python_sms.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      653 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/tencentcloud_sdk_python_sms.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       88 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1072 2023-10-16 00:34:10.000000 tencentcloud-sdk-python-sms-3.0.999/setup.py
```

### Comparing `tencentcloud-sdk-python-sms-3.0.998/tencentcloud/__init__.py` & `tencentcloud-sdk-python-sms-3.0.999/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.998'
+__version__ = '3.0.999'
```

### Comparing `tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20210111/models.py` & `tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20210111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20210111/errorcodes.py` & `tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20210111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20210111/sms_client.py` & `tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20210111/sms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20190711/models.py` & `tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20190711/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20190711/errorcodes.py` & `tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20190711/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.998/tencentcloud/sms/v20190711/sms_client.py` & `tencentcloud-sdk-python-sms-3.0.999/tencentcloud/sms/v20190711/sms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.998/PKG-INFO` & `tencentcloud-sdk-python-sms-3.0.999/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sms
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Sms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sms-3.0.998/README.rst` & `tencentcloud-sdk-python-sms-3.0.999/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.998/tencentcloud_sdk_python_sms.egg-info/PKG-INFO` & `tencentcloud-sdk-python-sms-3.0.999/tencentcloud_sdk_python_sms.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: tencentcloud-sdk-python-sms
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud Sms SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Author-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Description: ============================
         Tencent Cloud SDK for Python
```

### Comparing `tencentcloud-sdk-python-sms-3.0.998/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-sms-3.0.999/tencentcloud_sdk_python_sms.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-sms-3.0.998/setup.py` & `tencentcloud-sdk-python-sms-3.0.999/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import tencentcloud
 
 ROOT = os.path.dirname(__file__)
 
 setup(
     name='tencentcloud-sdk-python-sms',
-    install_requires=["tencentcloud-sdk-python-common==3.0.998"],
+    install_requires=["tencentcloud-sdk-python-common==3.0.999"],
     version=tencentcloud.__version__,
     description='Tencent Cloud Sms SDK for Python',
     long_description=open('README.rst').read(),
     author='Tencent Cloud',
     url='https://github.com/TencentCloud/tencentcloud-sdk-python',
     maintainer_email="tencentcloudapi@tencent.com",
     scripts=[],
```
