# Comparing `tmp/marqo-3.4.0.tar.gz` & `tmp/marqo-3.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "marqo-3.4.0.tar", last modified: Wed May 15 03:45:37 2024, max compression
+gzip compressed data, was "marqo-3.5.0.tar", last modified: Sun May 19 13:53:03 2024, max compression
```

## Comparing `marqo-3.4.0.tar` & `marqo-3.5.0.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:45:37.433856 marqo-3.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-05-15 03:45:31.000000 marqo-3.4.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-05-15 03:45:37.433856 marqo-3.4.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-05-15 03:45:31.000000 marqo-3.4.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-15 03:45:31.000000 marqo-3.4.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 03:45:37.433856 marqo-3.4.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1096 2024-05-15 03:45:31.000000 marqo-3.4.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:45:37.425856 marqo-3.4.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:45:37.429856 marqo-3.4.0/src/marqo/
--rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/_httprequests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12255 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/cloud_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/default_instance_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/enums.py
--rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    43308 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/instance_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/marqo_cloud_instance_mappings.py
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/marqo_logging.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:45:37.433856 marqo-3.4.0/src/marqo/models/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/models/create_index_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/models/marqo_cloud.py
--rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/models/marqo_index.py
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/models/marqo_models.py
--rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/models/search_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-15 03:45:31.000000 marqo-3.4.0/src/marqo/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 03:45:37.433856 marqo-3.4.0/src/marqo.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    22641 2024-05-15 03:45:37.000000 marqo-3.4.0/src/marqo.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-15 03:45:37.000000 marqo-3.4.0/src/marqo.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 03:45:37.000000 marqo-3.4.0/src/marqo.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 03:45:37.000000 marqo-3.4.0/src/marqo.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-15 03:45:37.000000 marqo-3.4.0/src/marqo.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:53:03.371167 marqo-3.5.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    10151 2024-05-19 13:52:57.000000 marqo-3.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    22642 2024-05-19 13:53:03.371167 marqo-3.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22031 2024-05-19 13:52:57.000000 marqo-3.5.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-19 13:52:57.000000 marqo-3.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 13:53:03.371167 marqo-3.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-19 13:52:57.000000 marqo-3.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:53:03.363167 marqo-3.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:53:03.367167 marqo-3.5.0/src/marqo/
+-rw-r--r--   0 runner    (1001) docker     (127)      247 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5529 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/_httprequests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12255 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      997 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/cloud_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      904 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/default_instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6105 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43308 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4194 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/marqo_cloud_instance_mappings.py
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/marqo_logging.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:53:03.371167 marqo-3.5.0/src/marqo/models/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2980 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/models/create_index_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/models/marqo_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2314 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/models/marqo_index.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/models/marqo_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)      794 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/models/search_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2140 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-19 13:52:57.000000 marqo-3.5.0/src/marqo/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 13:53:03.371167 marqo-3.5.0/src/marqo.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    22642 2024-05-19 13:53:03.000000 marqo-3.5.0/src/marqo.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-19 13:53:03.000000 marqo-3.5.0/src/marqo.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 13:53:03.000000 marqo-3.5.0/src/marqo.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       83 2024-05-19 13:53:03.000000 marqo-3.5.0/src/marqo.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-05-19 13:53:03.000000 marqo-3.5.0/src/marqo.egg-info/top_level.txt
```

### Comparing `marqo-3.4.0/LICENSE` & `marqo-3.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/PKG-INFO` & `marqo-3.5.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 3.4.0
+Version: 3.5.0
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: urllib3<2.0.0,>=1.26.0
-Requires-Dist: pydantic<2.0.0
+Requires-Dist: pydantic>=2.0.0
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: packaging
 
 <p align="center">
 <img src="https://uploads-ssl.webflow.com/62dfa8e3960a6e2b47dc7fae/62fdf9cef684e6f16158b094_MARQO%20LOGO-UPDATED-GREEN.svg" width="50%" height="40%">
 </p>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: marqo Version: 3.4.0 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 3.5.0 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests Requires-Dist: urllib3<2.0.0,>=1.26.0 Requires-
-Dist: pydantic<2.0.0 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
+Dist: pydantic>=2.0.0 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
 packaging
           [https://uploads-ssl.webflow.com/62dfa8e3960a6e2b47dc7fae/
            62fdf9cef684e6f16158b094_MARQO%20LOGO-UPDATED-GREEN.svg]
   _WW_ee_bb_ss_ii_tt_ee || _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn || _DD_ee_mm_oo_ss || _DD_ii_ss_cc_oo_uu_rr_ss_ee || _SS_ll_aa_cc_kk_ _CC_oo_mm_mm_uu_nn_ii_tt_yy || _MM_aa_rr_qq_oo_ _CC_ll_oo_uu_dd
      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_m_a_r_q_o_?_l_a_b_e_l_=_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/
 _w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_m_a_r_q_o_-_a_i_/_m_a_r_q_o_/_u_n_i_t___t_e_s_t___2_0_0_g_b___C_I_._y_m_l_?_b_r_a_n_c_h_=_m_a_i_n_l_i_n_e_]_[_h_t_t_p_s_:_/_/
```

### Comparing `marqo-3.4.0/README.md` & `marqo-3.5.0/README.md`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/setup.py` & `marqo-3.5.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,24 +5,24 @@
     long_description = fh.read()
 
 setup(
     install_requires=[
         # client:
         "requests",
         "urllib3<2.0.0, >=1.26.0",
-        "pydantic<2.0.0",
+        "pydantic>=2.0.0",
         "typing-extensions>=4.5.0",
         "packaging"
     ],
     tests_require=[
         "pytest",
         "tox"
     ],
     name="marqo",
-    version="3.4.0",
+    version="3.5.0",
     author="marqo org",
     author_email="org@marqo.io",
     description="Tensor search for humans",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src", exclude=("tests*",)),
     keywords="search python marqo opensearch tensor neural semantic vector embedding",
```

### Comparing `marqo-3.4.0/src/marqo/_httprequests.py` & `marqo-3.5.0/src/marqo/_httprequests.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/client.py` & `marqo-3.5.0/src/marqo/client.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/cloud_helpers.py` & `marqo-3.5.0/src/marqo/cloud_helpers.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/config.py` & `marqo-3.5.0/src/marqo/config.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/default_instance_mappings.py` & `marqo-3.5.0/src/marqo/default_instance_mappings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/enums.py` & `marqo-3.5.0/src/marqo/enums.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/errors.py` & `marqo-3.5.0/src/marqo/errors.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/index.py` & `marqo-3.5.0/src/marqo/index.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/instance_mappings.py` & `marqo-3.5.0/src/marqo/instance_mappings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/marqo_cloud_instance_mappings.py` & `marqo-3.5.0/src/marqo/marqo_cloud_instance_mappings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/models/create_index_settings.py` & `marqo-3.5.0/src/marqo/models/create_index_settings.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/models/marqo_cloud.py` & `marqo-3.5.0/src/marqo/models/marqo_cloud.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/models/marqo_index.py` & `marqo-3.5.0/src/marqo/models/marqo_index.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/models/marqo_models.py` & `marqo-3.5.0/src/marqo/models/marqo_models.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from pydantic import BaseModel
 
 
 class MarqoBaseModel(BaseModel):
     class Config:
-        allow_population_by_field_name = True  # accept both real name and alias (if present)
+        populate_by_name = True  # accept both real name and alias (if present)
         validate_assignment = True
 
 
 class StrictBaseModel(MarqoBaseModel):
     class Config(MarqoBaseModel.Config):
         extra = "forbid"
 
 
 class ImmutableBaseModel(MarqoBaseModel):
     class Config(MarqoBaseModel.Config):
-        allow_mutation = False
+        frozen = True
 
 
 class ImmutableStrictBaseModel(StrictBaseModel, ImmutableBaseModel):
     class Config(StrictBaseModel.Config, ImmutableBaseModel.Config):
         pass
```

### Comparing `marqo-3.4.0/src/marqo/models/search_models.py` & `marqo-3.5.0/src/marqo/models/search_models.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/utils.py` & `marqo-3.5.0/src/marqo/utils.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo/version.py` & `marqo-3.5.0/src/marqo/version.py`

 * *Files identical despite different names*

### Comparing `marqo-3.4.0/src/marqo.egg-info/PKG-INFO` & `marqo-3.5.0/src/marqo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: marqo
-Version: 3.4.0
+Version: 3.5.0
 Summary: Tensor search for humans
 Author: marqo org
 Author-email: org@marqo.io
 Keywords: search python marqo opensearch tensor neural semantic vector embedding
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: requests
 Requires-Dist: urllib3<2.0.0,>=1.26.0
-Requires-Dist: pydantic<2.0.0
+Requires-Dist: pydantic>=2.0.0
 Requires-Dist: typing-extensions>=4.5.0
 Requires-Dist: packaging
 
 <p align="center">
 <img src="https://uploads-ssl.webflow.com/62dfa8e3960a6e2b47dc7fae/62fdf9cef684e6f16158b094_MARQO%20LOGO-UPDATED-GREEN.svg" width="50%" height="40%">
 </p>
```

#### html2text {}

```diff
@@ -1,15 +1,15 @@
-Metadata-Version: 2.1 Name: marqo Version: 3.4.0 Summary: Tensor search for
+Metadata-Version: 2.1 Name: marqo Version: 3.5.0 Summary: Tensor search for
 humans Author: marqo org Author-email: org@marqo.io Keywords: search python
 marqo opensearch tensor neural semantic vector embedding Classifier:
 Programming Language :: Python :: 3.8 Classifier: License :: OSI Approved ::
 Apache Software License Classifier: Operating System :: OS Independent
 Requires-Python: >=3 Description-Content-Type: text/markdown License-File:
 LICENSE Requires-Dist: requests Requires-Dist: urllib3<2.0.0,>=1.26.0 Requires-
-Dist: pydantic<2.0.0 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
+Dist: pydantic>=2.0.0 Requires-Dist: typing-extensions>=4.5.0 Requires-Dist:
 packaging
           [https://uploads-ssl.webflow.com/62dfa8e3960a6e2b47dc7fae/
            62fdf9cef684e6f16158b094_MARQO%20LOGO-UPDATED-GREEN.svg]
   _WW_ee_bb_ss_ii_tt_ee || _DD_oo_cc_uu_mm_ee_nn_tt_aa_tt_ii_oo_nn || _DD_ee_mm_oo_ss || _DD_ii_ss_cc_oo_uu_rr_ss_ee || _SS_ll_aa_cc_kk_ _CC_oo_mm_mm_uu_nn_ii_tt_yy || _MM_aa_rr_qq_oo_ _CC_ll_oo_uu_dd
      _[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_b_a_d_g_e_/_L_i_c_e_n_s_e_-_A_p_a_c_h_e_%_2_0_2_._0_-_b_l_u_e_._s_v_g_]_[_h_t_t_p_s_:_/_/
 _i_m_g_._s_h_i_e_l_d_s_._i_o_/_p_y_p_i_/_v_/_m_a_r_q_o_?_l_a_b_e_l_=_P_y_P_I_]_[_h_t_t_p_s_:_/_/_i_m_g_._s_h_i_e_l_d_s_._i_o_/_g_i_t_h_u_b_/_a_c_t_i_o_n_s_/
 _w_o_r_k_f_l_o_w_/_s_t_a_t_u_s_/_m_a_r_q_o_-_a_i_/_m_a_r_q_o_/_u_n_i_t___t_e_s_t___2_0_0_g_b___C_I_._y_m_l_?_b_r_a_n_c_h_=_m_a_i_n_l_i_n_e_]_[_h_t_t_p_s_:_/_/
```

### Comparing `marqo-3.4.0/src/marqo.egg-info/SOURCES.txt` & `marqo-3.5.0/src/marqo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

