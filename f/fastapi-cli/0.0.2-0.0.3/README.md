# Comparing `tmp/fastapi_cli-0.0.2.tar.gz` & `tmp/fastapi_cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi_cli-0.0.2.tar", last modified: Thu May  2 21:50:17 2024, max compression
+gzip compressed data, was "fastapi_cli-0.0.3.tar", last modified: Tue May  7 19:03:41 2024, max compression
```

## Comparing `fastapi_cli-0.0.2.tar` & `fastapi_cli-0.0.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0     1086 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/LICENSE
--rw-r--r--   0        0        0     5053 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/README.md
--rw-r--r--   0        0        0     1718 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/pdm_build.py
--rw-r--r--   0        0        0     3047 2024-05-02 21:50:17.219287 fastapi_cli-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       80 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/requirements-tests.txt
--rw-r--r--   0        0        0       60 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/requirements.txt
--rwxr-xr-x   0        0        0       87 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/scripts/format.sh
--rwxr-xr-x   0        0        0      110 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/scripts/lint.sh
--rwxr-xr-x   0        0        0      124 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/scripts/test-cov-html.sh
--rwxr-xr-x   0        0        0       70 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/scripts/test.sh
--rw-r--r--   0        0        0       22 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/src/fastapi_cli/__init__.py
--rw-r--r--   0        0        0       30 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/src/fastapi_cli/__main__.py
--rw-r--r--   0        0        0     8754 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/src/fastapi_cli/cli.py
--rw-r--r--   0        0        0     5285 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/src/fastapi_cli/discover.py
--rw-r--r--   0        0        0       47 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/src/fastapi_cli/exceptions.py
--rw-r--r--   0        0        0      664 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/src/fastapi_cli/logging.py
--rw-r--r--   0        0        0        0 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/src/fastapi_cli/py.typed
--rw-r--r--   0        0        0        0 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/tests/__init__.py
--rw-r--r--   0        0        0       28 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/tests/assets/broken_package/mod/__init__.py
--rw-r--r--   0        0        0      148 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/tests/assets/broken_package/mod/app.py
--rw-r--r--   0        0        0       52 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/tests/assets/broken_package/utils.py
--rw-r--r--   0        0        0      119 2024-05-02 21:50:14.427237 fastapi_cli-0.0.2/tests/assets/default_files/default_api/api.py
--rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app/api.py
--rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app/app.py
--rw-r--r--   0        0        0        0 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_api/app/__init__.py
--rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_api/app/api.py
--rw-r--r--   0        0        0        0 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_app/app/__init__.py
--rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_app/app/api.py
--rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_app/app/app.py
--rw-r--r--   0        0        0        0 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_main/app/__init__.py
--rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_main/app/api.py
--rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_main/app/app.py
--rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_main/app/main.py
--rw-r--r--   0        0        0        0 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_non_default/app/__init__.py
--rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_app_dir_non_default/app/nondefault.py
--rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_main/api.py
--rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_main/app.py
--rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/default_main/main.py
--rw-r--r--   0        0        0      119 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/default_files/non_default/nonstandard.py
--rw-r--r--   0        0        0       64 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/package/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/package/core/__init__.py
--rw-r--r--   0        0        0       55 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/package/core/utils.py
--rw-r--r--   0        0        0       28 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/package/mod/__init__.py
--rw-r--r--   0        0        0      359 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/package/mod/api.py
--rw-r--r--   0        0        0      447 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/package/mod/app.py
--rw-r--r--   0        0        0      271 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/package/mod/other.py
--rw-r--r--   0        0        0      371 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/single_file_api.py
--rw-r--r--   0        0        0      463 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/single_file_app.py
--rw-r--r--   0        0        0      279 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/assets/single_file_other.py
--rw-r--r--   0        0        0      530 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/conftest.py
--rw-r--r--   0        0        0     8393 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/test_cli.py
--rw-r--r--   0        0        0     3905 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/test_utils_default_dir.py
--rw-r--r--   0        0        0     4046 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/test_utils_default_file.py
--rw-r--r--   0        0        0    20671 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/test_utils_package.py
--rw-r--r--   0        0        0     4993 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/test_utils_single_file.py
--rw-r--r--   0        0        0      325 2024-05-02 21:50:14.431237 fastapi_cli-0.0.2/tests/utils.py
--rw-r--r--   0        0        0     6780 1970-01-01 00:00:00.000000 fastapi_cli-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1086 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/LICENSE
+-rw-r--r--   0        0        0     5228 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/README.md
+-rw-r--r--   0        0        0     1718 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/pdm_build.py
+-rw-r--r--   0        0        0     3047 2024-05-07 19:03:41.257601 fastapi_cli-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      142 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/requirements-tests.txt
+-rw-r--r--   0        0        0       60 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/requirements.txt
+-rwxr-xr-x   0        0        0       87 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/scripts/format.sh
+-rwxr-xr-x   0        0        0      110 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/scripts/lint.sh
+-rwxr-xr-x   0        0        0      124 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/scripts/test-cov-html.sh
+-rwxr-xr-x   0        0        0       70 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/scripts/test.sh
+-rw-r--r--   0        0        0       22 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/src/fastapi_cli/__init__.py
+-rw-r--r--   0        0        0       30 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/src/fastapi_cli/__main__.py
+-rw-r--r--   0        0        0     9032 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/src/fastapi_cli/cli.py
+-rw-r--r--   0        0        0     5285 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/src/fastapi_cli/discover.py
+-rw-r--r--   0        0        0       47 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/src/fastapi_cli/exceptions.py
+-rw-r--r--   0        0        0      664 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/src/fastapi_cli/logging.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/src/fastapi_cli/py.typed
+-rw-r--r--   0        0        0        0 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/tests/__init__.py
+-rw-r--r--   0        0        0       28 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/tests/assets/broken_package/mod/__init__.py
+-rw-r--r--   0        0        0      148 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/tests/assets/broken_package/mod/app.py
+-rw-r--r--   0        0        0       52 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/tests/assets/broken_package/utils.py
+-rw-r--r--   0        0        0      119 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/tests/assets/default_files/default_api/api.py
+-rw-r--r--   0        0        0      119 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/tests/assets/default_files/default_app/api.py
+-rw-r--r--   0        0        0      119 2024-05-07 19:03:38.469576 fastapi_cli-0.0.3/tests/assets/default_files/default_app/app.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/default_app_dir_api/app/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/default_app_dir_api/app/api.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/default_app_dir_app/app/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/default_app_dir_app/app/api.py
+-rw-r--r--   0        0        0      119 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/default_app_dir_app/app/app.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/default_app_dir_main/app/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/default_app_dir_main/app/api.py
+-rw-r--r--   0        0        0      119 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/default_app_dir_main/app/app.py
+-rw-r--r--   0        0        0      119 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/default_app_dir_main/app/main.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/default_app_dir_non_default/app/__init__.py
+-rw-r--r--   0        0        0      119 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/default_app_dir_non_default/app/nondefault.py
+-rw-r--r--   0        0        0      119 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/default_main/api.py
+-rw-r--r--   0        0        0      119 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/default_main/app.py
+-rw-r--r--   0        0        0      119 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/default_main/main.py
+-rw-r--r--   0        0        0      119 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/default_files/non_default/nonstandard.py
+-rw-r--r--   0        0        0       64 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/package/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/package/core/__init__.py
+-rw-r--r--   0        0        0       55 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/package/core/utils.py
+-rw-r--r--   0        0        0       28 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/package/mod/__init__.py
+-rw-r--r--   0        0        0      359 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/package/mod/api.py
+-rw-r--r--   0        0        0      447 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/package/mod/app.py
+-rw-r--r--   0        0        0      271 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/package/mod/other.py
+-rw-r--r--   0        0        0      371 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/single_file_api.py
+-rw-r--r--   0        0        0      463 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/single_file_app.py
+-rw-r--r--   0        0        0      279 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/assets/single_file_other.py
+-rw-r--r--   0        0        0      530 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/conftest.py
+-rw-r--r--   0        0        0     8706 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/test_cli.py
+-rw-r--r--   0        0        0     3905 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/test_utils_default_dir.py
+-rw-r--r--   0        0        0     4046 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/test_utils_default_file.py
+-rw-r--r--   0        0        0    20671 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/test_utils_package.py
+-rw-r--r--   0        0        0     4993 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/test_utils_single_file.py
+-rw-r--r--   0        0        0      325 2024-05-07 19:03:38.473576 fastapi_cli-0.0.3/tests/utils.py
+-rw-r--r--   0        0        0     6955 1970-01-01 00:00:00.000000 fastapi_cli-0.0.3/PKG-INFO
```

### Comparing `fastapi_cli-0.0.2/LICENSE` & `fastapi_cli-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fastapi_cli-0.0.2/README.md` & `fastapi_cli-0.0.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -78,14 +78,16 @@
 
 That command line program called `fastapi` is **FastAPI CLI**.
 
 FastAPI CLI takes the path to your Python program and automatically detects the variable with the FastAPI (commonly named `app`) and how to import it, and then serves it.
 
 For production you would use `fastapi run` instead. 🚀
 
+Internally, **FastAPI CLI** uses <a href="https://www.uvicorn.org" class="external-link" target="_blank">Uvicorn</a>, a high-performance, production-ready, ASGI server. 😎
+
 ## `fastapi dev`
 
 When you run `fastapi dev`, it will run on development mode.
 
 By default, it will have **auto-reload** enabled, so it will automatically reload the server when you make changes to your code. This is resource intensive and could be less stable than without it, you should only use it for development.
 
 By default it will listen on the IP address `127.0.0.1`, which is the IP for your machine to communicate with itself alone (`localhost`).
```

#### html2text {}

```diff
@@ -26,24 +26,26 @@
 _a_w_e_s_o_m_e_a_p_p_'_]_ _I_N_F_O_:_ _U_v_i_c_o_r_n_ _r_u_n_n_i_n_g_ _o_n_ _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_ _(_P_r_e_s_s_ _C_T_R_L_+_C_ _t_o
 _q_u_i_t_)_ _I_N_F_O_:_ _S_t_a_r_t_e_d_ _r_e_l_o_a_d_e_r_ _p_r_o_c_e_s_s_ _[_5_6_3_4_5_]_ _u_s_i_n_g_ _W_a_t_c_h_F_i_l_e_s_ _I_N_F_O_:_ _S_t_a_r_t_e_d
 _s_e_r_v_e_r_ _p_r_o_c_e_s_s_ _[_5_6_3_5_2_]_ _I_N_F_O_:_ _W_a_i_t_i_n_g_ _f_o_r_ _a_p_p_l_i_c_a_t_i_o_n_ _s_t_a_r_t_u_p_._ _I_N_F_O_:_ _A_p_p_l_i_c_a_t_i_o_n
 _s_t_a_r_t_u_p_ _c_o_m_p_l_e_t_e_._ _`_`_`
 _T_h_a_t_ _c_o_m_m_a_n_d_ _l_i_n_e_ _p_r_o_g_r_a_m_ _c_a_l_l_e_d_ _`_f_a_s_t_a_p_i_`_ _i_s_ _*_*_F_a_s_t_A_P_I_ _C_L_I_*_*_._ _F_a_s_t_A_P_I_ _C_L_I
 _t_a_k_e_s_ _t_h_e_ _p_a_t_h_ _t_o_ _y_o_u_r_ _P_y_t_h_o_n_ _p_r_o_g_r_a_m_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _d_e_t_e_c_t_s_ _t_h_e_ _v_a_r_i_a_b_l_e
 _w_i_t_h_ _t_h_e_ _F_a_s_t_A_P_I_ _(_c_o_m_m_o_n_l_y_ _n_a_m_e_d_ _`_a_p_p_`_)_ _a_n_d_ _h_o_w_ _t_o_ _i_m_p_o_r_t_ _i_t_,_ _a_n_d_ _t_h_e_n_ _s_e_r_v_e_s
-_i_t_._ _F_o_r_ _p_r_o_d_u_c_t_i_o_n_ _y_o_u_ _w_o_u_l_d_ _u_s_e_ _`_f_a_s_t_a_p_i_ _r_u_n_`_ _i_n_s_t_e_a_d_._ _ð____ _#_#_ _`_f_a_s_t_a_p_i_ _d_e_v_`
-_W_h_e_n_ _y_o_u_ _r_u_n_ _`_f_a_s_t_a_p_i_ _d_e_v_`_,_ _i_t_ _w_i_l_l_ _r_u_n_ _o_n_ _d_e_v_e_l_o_p_m_e_n_t_ _m_o_d_e_._ _B_y_ _d_e_f_a_u_l_t_,_ _i_t
-_w_i_l_l_ _h_a_v_e_ _*_*_a_u_t_o_-_r_e_l_o_a_d_*_*_ _e_n_a_b_l_e_d_,_ _s_o_ _i_t_ _w_i_l_l_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _r_e_l_o_a_d_ _t_h_e_ _s_e_r_v_e_r
-_w_h_e_n_ _y_o_u_ _m_a_k_e_ _c_h_a_n_g_e_s_ _t_o_ _y_o_u_r_ _c_o_d_e_._ _T_h_i_s_ _i_s_ _r_e_s_o_u_r_c_e_ _i_n_t_e_n_s_i_v_e_ _a_n_d_ _c_o_u_l_d_ _b_e
-_l_e_s_s_ _s_t_a_b_l_e_ _t_h_a_n_ _w_i_t_h_o_u_t_ _i_t_,_ _y_o_u_ _s_h_o_u_l_d_ _o_n_l_y_ _u_s_e_ _i_t_ _f_o_r_ _d_e_v_e_l_o_p_m_e_n_t_._ _B_y_ _d_e_f_a_u_l_t
-_i_t_ _w_i_l_l_ _l_i_s_t_e_n_ _o_n_ _t_h_e_ _I_P_ _a_d_d_r_e_s_s_ _`_1_2_7_._0_._0_._1_`_,_ _w_h_i_c_h_ _i_s_ _t_h_e_ _I_P_ _f_o_r_ _y_o_u_r_ _m_a_c_h_i_n_e
-_t_o_ _c_o_m_m_u_n_i_c_a_t_e_ _w_i_t_h_ _i_t_s_e_l_f_ _a_l_o_n_e_ _(_`_l_o_c_a_l_h_o_s_t_`_)_._ _#_#_ _`_f_a_s_t_a_p_i_ _r_u_n_`_ _W_h_e_n_ _y_o_u_ _r_u_n
-_`_f_a_s_t_a_p_i_ _r_u_n_`_,_ _i_t_ _w_i_l_l_ _r_u_n_ _o_n_ _p_r_o_d_u_c_t_i_o_n_ _m_o_d_e_ _b_y_ _d_e_f_a_u_l_t_._ _I_t_ _w_i_l_l_ _h_a_v_e_ _*_*_a_u_t_o_-
-_r_e_l_o_a_d_ _d_i_s_a_b_l_e_d_*_*_ _b_y_ _d_e_f_a_u_l_t_._ _I_t_ _w_i_l_l_ _l_i_s_t_e_n_ _o_n_ _t_h_e_ _I_P_ _a_d_d_r_e_s_s_ _`_0_._0_._0_._0_`_,_ _w_h_i_c_h
-_m_e_a_n_s_ _a_l_l_ _t_h_e_ _a_v_a_i_l_a_b_l_e_ _I_P_ _a_d_d_r_e_s_s_e_s_,_ _t_h_i_s_ _w_a_y_ _i_t_ _w_i_l_l_ _b_e_ _p_u_b_l_i_c_l_y_ _a_c_c_e_s_s_i_b_l_e
-_t_o_ _a_n_y_o_n_e_ _t_h_a_t_ _c_a_n_ _c_o_m_m_u_n_i_c_a_t_e_ _w_i_t_h_ _t_h_e_ _m_a_c_h_i_n_e_._ _T_h_i_s_ _i_s_ _h_o_w_ _y_o_u_ _w_o_u_l_d_ _n_o_r_m_a_l_l_y
-_r_u_n_ _i_t_ _i_n_ _p_r_o_d_u_c_t_i_o_n_,_ _f_o_r_ _e_x_a_m_p_l_e_,_ _i_n_ _a_ _c_o_n_t_a_i_n_e_r_._ _I_n_ _m_o_s_t_ _c_a_s_e_s_ _y_o_u_ _w_o_u_l_d_ _(_a_n_d
-_s_h_o_u_l_d_)_ _h_a_v_e_ _a_ _"_t_e_r_m_i_n_a_t_i_o_n_ _p_r_o_x_y_"_ _h_a_n_d_l_i_n_g_ _H_T_T_P_S_ _f_o_r_ _y_o_u_ _o_n_ _t_o_p_,_ _t_h_i_s_ _w_i_l_l
-_d_e_p_e_n_d_ _o_n_ _h_o_w_ _y_o_u_ _d_e_p_l_o_y_ _y_o_u_r_ _a_p_p_l_i_c_a_t_i_o_n_,_ _y_o_u_r_ _p_r_o_v_i_d_e_r_ _m_i_g_h_t_ _d_o_ _t_h_i_s_ _f_o_r_ _y_o_u_,
-_o_r_ _y_o_u_ _m_i_g_h_t_ _n_e_e_d_ _t_o_ _s_e_t_ _i_t_ _u_p_ _y_o_u_r_s_e_l_f_._ _Y_o_u_ _c_a_n_ _l_e_a_r_n_ _m_o_r_e_ _a_b_o_u_t_ _i_t_ _i_n_ _t_h_e
-_F_a_s_t_A_P_I_ _D_e_p_l_o_y_m_e_n_t_ _d_o_c_u_m_e_n_t_a_t_i_o_n_._ _#_#_ _L_i_c_e_n_s_e_ _T_h_i_s_ _p_r_o_j_e_c_t_ _i_s_ _l_i_c_e_n_s_e_d_ _u_n_d_e_r_ _t_h_e
-_t_e_r_m_s_ _o_f_ _t_h_e_ _M_I_T_ _l_i_c_e_n_s_e_.
+_i_t_._ _F_o_r_ _p_r_o_d_u_c_t_i_o_n_ _y_o_u_ _w_o_u_l_d_ _u_s_e_ _`_f_a_s_t_a_p_i_ _r_u_n_`_ _i_n_s_t_e_a_d_._ _ð____ _I_n_t_e_r_n_a_l_l_y_,
+_*_*_F_a_s_t_A_P_I_ _C_L_I_*_*_ _u_s_e_s_ _U_v_i_c_o_r_n_,_ _a_ _h_i_g_h_-_p_e_r_f_o_r_m_a_n_c_e_,_ _p_r_o_d_u_c_t_i_o_n_-_r_e_a_d_y_,_ _A_S_G_I
+_s_e_r_v_e_r_._ _ð____ _#_#_ _`_f_a_s_t_a_p_i_ _d_e_v_`_ _W_h_e_n_ _y_o_u_ _r_u_n_ _`_f_a_s_t_a_p_i_ _d_e_v_`_,_ _i_t_ _w_i_l_l_ _r_u_n_ _o_n
+_d_e_v_e_l_o_p_m_e_n_t_ _m_o_d_e_._ _B_y_ _d_e_f_a_u_l_t_,_ _i_t_ _w_i_l_l_ _h_a_v_e_ _*_*_a_u_t_o_-_r_e_l_o_a_d_*_*_ _e_n_a_b_l_e_d_,_ _s_o_ _i_t_ _w_i_l_l
+_a_u_t_o_m_a_t_i_c_a_l_l_y_ _r_e_l_o_a_d_ _t_h_e_ _s_e_r_v_e_r_ _w_h_e_n_ _y_o_u_ _m_a_k_e_ _c_h_a_n_g_e_s_ _t_o_ _y_o_u_r_ _c_o_d_e_._ _T_h_i_s_ _i_s
+_r_e_s_o_u_r_c_e_ _i_n_t_e_n_s_i_v_e_ _a_n_d_ _c_o_u_l_d_ _b_e_ _l_e_s_s_ _s_t_a_b_l_e_ _t_h_a_n_ _w_i_t_h_o_u_t_ _i_t_,_ _y_o_u_ _s_h_o_u_l_d_ _o_n_l_y
+_u_s_e_ _i_t_ _f_o_r_ _d_e_v_e_l_o_p_m_e_n_t_._ _B_y_ _d_e_f_a_u_l_t_ _i_t_ _w_i_l_l_ _l_i_s_t_e_n_ _o_n_ _t_h_e_ _I_P_ _a_d_d_r_e_s_s
+_`_1_2_7_._0_._0_._1_`_,_ _w_h_i_c_h_ _i_s_ _t_h_e_ _I_P_ _f_o_r_ _y_o_u_r_ _m_a_c_h_i_n_e_ _t_o_ _c_o_m_m_u_n_i_c_a_t_e_ _w_i_t_h_ _i_t_s_e_l_f_ _a_l_o_n_e
+_(_`_l_o_c_a_l_h_o_s_t_`_)_._ _#_#_ _`_f_a_s_t_a_p_i_ _r_u_n_`_ _W_h_e_n_ _y_o_u_ _r_u_n_ _`_f_a_s_t_a_p_i_ _r_u_n_`_,_ _i_t_ _w_i_l_l_ _r_u_n_ _o_n
+_p_r_o_d_u_c_t_i_o_n_ _m_o_d_e_ _b_y_ _d_e_f_a_u_l_t_._ _I_t_ _w_i_l_l_ _h_a_v_e_ _*_*_a_u_t_o_-_r_e_l_o_a_d_ _d_i_s_a_b_l_e_d_*_*_ _b_y_ _d_e_f_a_u_l_t_.
+_I_t_ _w_i_l_l_ _l_i_s_t_e_n_ _o_n_ _t_h_e_ _I_P_ _a_d_d_r_e_s_s_ _`_0_._0_._0_._0_`_,_ _w_h_i_c_h_ _m_e_a_n_s_ _a_l_l_ _t_h_e_ _a_v_a_i_l_a_b_l_e_ _I_P
+_a_d_d_r_e_s_s_e_s_,_ _t_h_i_s_ _w_a_y_ _i_t_ _w_i_l_l_ _b_e_ _p_u_b_l_i_c_l_y_ _a_c_c_e_s_s_i_b_l_e_ _t_o_ _a_n_y_o_n_e_ _t_h_a_t_ _c_a_n
+_c_o_m_m_u_n_i_c_a_t_e_ _w_i_t_h_ _t_h_e_ _m_a_c_h_i_n_e_._ _T_h_i_s_ _i_s_ _h_o_w_ _y_o_u_ _w_o_u_l_d_ _n_o_r_m_a_l_l_y_ _r_u_n_ _i_t_ _i_n
+_p_r_o_d_u_c_t_i_o_n_,_ _f_o_r_ _e_x_a_m_p_l_e_,_ _i_n_ _a_ _c_o_n_t_a_i_n_e_r_._ _I_n_ _m_o_s_t_ _c_a_s_e_s_ _y_o_u_ _w_o_u_l_d_ _(_a_n_d_ _s_h_o_u_l_d_)
+_h_a_v_e_ _a_ _"_t_e_r_m_i_n_a_t_i_o_n_ _p_r_o_x_y_"_ _h_a_n_d_l_i_n_g_ _H_T_T_P_S_ _f_o_r_ _y_o_u_ _o_n_ _t_o_p_,_ _t_h_i_s_ _w_i_l_l_ _d_e_p_e_n_d_ _o_n
+_h_o_w_ _y_o_u_ _d_e_p_l_o_y_ _y_o_u_r_ _a_p_p_l_i_c_a_t_i_o_n_,_ _y_o_u_r_ _p_r_o_v_i_d_e_r_ _m_i_g_h_t_ _d_o_ _t_h_i_s_ _f_o_r_ _y_o_u_,_ _o_r_ _y_o_u
+_m_i_g_h_t_ _n_e_e_d_ _t_o_ _s_e_t_ _i_t_ _u_p_ _y_o_u_r_s_e_l_f_._ _Y_o_u_ _c_a_n_ _l_e_a_r_n_ _m_o_r_e_ _a_b_o_u_t_ _i_t_ _i_n_ _t_h_e_ _F_a_s_t_A_P_I
+_D_e_p_l_o_y_m_e_n_t_ _d_o_c_u_m_e_n_t_a_t_i_o_n_._ _#_#_ _L_i_c_e_n_s_e_ _T_h_i_s_ _p_r_o_j_e_c_t_ _i_s_ _l_i_c_e_n_s_e_d_ _u_n_d_e_r_ _t_h_e_ _t_e_r_m_s
+_o_f_ _t_h_e_ _M_I_T_ _l_i_c_e_n_s_e_.
```

### Comparing `fastapi_cli-0.0.2/pdm_build.py` & `fastapi_cli-0.0.3/pdm_build.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli-0.0.2/pyproject.toml` & `fastapi_cli-0.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -30,17 +30,17 @@
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
     "License :: OSI Approved :: MIT License",
 ]
 dependencies = [
     "typer >= 0.12.3",
     "fastapi",
-    "uvicorn[standard] >= 0.29.0",
+    "uvicorn[standard] >= 0.15.0",
 ]
-version = "0.0.2"
+version = "0.0.3"
 
 [project.license]
 text = "MIT"
 
 [project.optional-dependencies]
 
 [project.urls]
```

### Comparing `fastapi_cli-0.0.2/src/fastapi_cli/cli.py` & `fastapi_cli-0.0.3/src/fastapi_cli/cli.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,14 +47,15 @@
 
 def _run(
     path: Union[Path, None] = None,
     *,
     host: str = "127.0.0.1",
     port: int = 8000,
     reload: bool = True,
+    workers: Union[int, None] = None,
     root_path: str = "",
     command: str,
     app: Union[str, None] = None,
     proxy_headers: bool = False,
 ) -> None:
     try:
         use_uvicorn_app = get_import_string(path=path, app_name=app)
@@ -81,14 +82,15 @@
         )
     print(Padding(panel, 1))
     uvicorn.run(
         app=use_uvicorn_app,
         host=host,
         port=port,
         reload=reload,
+        workers=workers,
         root_path=root_path,
         proxy_headers=proxy_headers,
     )
 
 
 @app.command()
 def dev(
@@ -196,14 +198,20 @@
     ] = 8000,
     reload: Annotated[
         bool,
         typer.Option(
             help="Enable auto-reload of the server when (code) files change. This is [bold]resource intensive[/bold], use it only during development."
         ),
     ] = False,
+    workers: Annotated[
+        Union[int, None],
+        typer.Option(
+            help="Use multiple worker processes. Mutually exclusive with the --reload flag."
+        ),
+    ] = None,
     root_path: Annotated[
         str,
         typer.Option(
             help="The root path is used to tell your app that it is being served to the outside world with some [bold]path prefix[/bold] set up in some termination proxy or similar."
         ),
     ] = "",
     app: Annotated[
@@ -245,14 +253,15 @@
     Otherwise, it uses the first [bold]FastAPI[/bold] app found in the imported module or package.
     """
     _run(
         path=path,
         host=host,
         port=port,
         reload=reload,
+        workers=workers,
         root_path=root_path,
         app=app,
         command="run",
         proxy_headers=proxy_headers,
     )
```

### Comparing `fastapi_cli-0.0.2/src/fastapi_cli/discover.py` & `fastapi_cli-0.0.3/src/fastapi_cli/discover.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli-0.0.2/src/fastapi_cli/logging.py` & `fastapi_cli-0.0.3/src/fastapi_cli/logging.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli-0.0.2/tests/conftest.py` & `fastapi_cli-0.0.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli-0.0.2/tests/test_cli.py` & `fastapi_cli-0.0.3/tests/test_cli.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,14 +22,15 @@
             assert mock_run.called
             assert mock_run.call_args
             assert mock_run.call_args.kwargs == {
                 "app": "single_file_app:app",
                 "host": "127.0.0.1",
                 "port": 8000,
                 "reload": True,
+                "workers": None,
                 "root_path": "",
                 "proxy_headers": True,
             }
         assert "Using import string single_file_app:app" in result.output
         assert (
             "╭────────── FastAPI CLI - Development mode ───────────╮" in result.output
         )
@@ -63,14 +64,15 @@
             assert mock_run.called
             assert mock_run.call_args
             assert mock_run.call_args.kwargs == {
                 "app": "single_file_app:api",
                 "host": "192.168.0.2",
                 "port": 8080,
                 "reload": False,
+                "workers": None,
                 "root_path": "/api",
                 "proxy_headers": False,
             }
         assert "Using import string single_file_app:api" in result.output
         assert (
             "╭────────── FastAPI CLI - Development mode ───────────╮" in result.output
         )
@@ -88,14 +90,15 @@
             assert mock_run.called
             assert mock_run.call_args
             assert mock_run.call_args.kwargs == {
                 "app": "single_file_app:app",
                 "host": "0.0.0.0",
                 "port": 8000,
                 "reload": False,
+                "workers": None,
                 "root_path": "",
                 "proxy_headers": True,
             }
         assert "Using import string single_file_app:app" in result.output
         assert (
             "╭─────────── FastAPI CLI - Production mode ───────────╮" in result.output
         )
@@ -114,14 +117,16 @@
                     "run",
                     "single_file_app.py",
                     "--host",
                     "192.168.0.2",
                     "--port",
                     "8080",
                     "--no-reload",
+                    "--workers",
+                    "2",
                     "--root-path",
                     "/api",
                     "--app",
                     "api",
                     "--no-proxy-headers",
                 ],
             )
@@ -129,14 +134,15 @@
             assert mock_run.called
             assert mock_run.call_args
             assert mock_run.call_args.kwargs == {
                 "app": "single_file_app:api",
                 "host": "192.168.0.2",
                 "port": 8080,
                 "reload": False,
+                "workers": 2,
                 "root_path": "/api",
                 "proxy_headers": False,
             }
         assert "Using import string single_file_app:api" in result.output
         assert (
             "╭─────────── FastAPI CLI - Production mode ───────────╮" in result.output
         )
@@ -167,14 +173,15 @@
     )
     assert "A path to a Python file or package directory" in result.output
     assert "The host to serve on." in result.output
     assert "The port to serve on." in result.output
     assert "Enable auto-reload of the server when (code) files change." in result.output
     assert "The root path is used to tell your app" in result.output
     assert "The name of the variable that contains the FastAPI app" in result.output
+    assert "Use multiple worker processes." not in result.output
 
 
 def test_run_help() -> None:
     result = runner.invoke(app, ["run", "--help"])
     assert result.exit_code == 0, result.output
     assert "Run a FastAPI app in production mode." in result.output
     assert (
@@ -187,14 +194,15 @@
     )
     assert "A path to a Python file or package directory" in result.output
     assert "The host to serve on." in result.output
     assert "The port to serve on." in result.output
     assert "Enable auto-reload of the server when (code) files change." in result.output
     assert "The root path is used to tell your app" in result.output
     assert "The name of the variable that contains the FastAPI app" in result.output
+    assert "Use multiple worker processes." in result.output
 
 
 def test_callback_help() -> None:
     result = runner.invoke(app, ["--help"])
     assert result.exit_code == 0, result.output
     assert "FastAPI CLI - The fastapi command line app." in result.output
     assert "Show the version and exit." in result.output
```

### Comparing `fastapi_cli-0.0.2/tests/test_utils_default_dir.py` & `fastapi_cli-0.0.3/tests/test_utils_default_dir.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli-0.0.2/tests/test_utils_default_file.py` & `fastapi_cli-0.0.3/tests/test_utils_default_file.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli-0.0.2/tests/test_utils_package.py` & `fastapi_cli-0.0.3/tests/test_utils_package.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli-0.0.2/tests/test_utils_single_file.py` & `fastapi_cli-0.0.3/tests/test_utils_single_file.py`

 * *Files identical despite different names*

### Comparing `fastapi_cli-0.0.2/PKG-INFO` & `fastapi_cli-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastapi-cli
-Version: 0.0.2
+Version: 0.0.3
 Summary: Run and manage FastAPI apps from the command line with FastAPI CLI. 🚀
 Home-page: https://github.com/tiangolo/fastapi-cli
 Author-Email: =?utf-8?q?Sebasti=C3=A1n_Ram=C3=ADrez?= <tiangolo@gmail.com>
 License: MIT
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: Operating System :: OS Independent
@@ -29,15 +29,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Documentation, https://fastapi.tiangolo.com
 Project-URL: Homepage, https://github.com/tiangolo/fastapi-cli
 Project-URL: Repository, https://github.com/tiangolo/fastapi-cli
 Requires-Python: >=3.8
 Requires-Dist: typer>=0.12.3
 Requires-Dist: fastapi
-Requires-Dist: uvicorn[standard]>=0.29.0
+Requires-Dist: uvicorn[standard]>=0.15.0
 Description-Content-Type: text/markdown
 
 # FastAPI CLI
 
 <a href="https://github.com/tiangolo/fastapi-cli/actions/workflows/test.yml" target="_blank">
     <img src="https://github.com/tiangolo/fastapi-cli/actions/workflows/test.yml/badge.svg" alt="Test">
 </a>
@@ -116,14 +116,16 @@
 
 That command line program called `fastapi` is **FastAPI CLI**.
 
 FastAPI CLI takes the path to your Python program and automatically detects the variable with the FastAPI (commonly named `app`) and how to import it, and then serves it.
 
 For production you would use `fastapi run` instead. 🚀
 
+Internally, **FastAPI CLI** uses <a href="https://www.uvicorn.org" class="external-link" target="_blank">Uvicorn</a>, a high-performance, production-ready, ASGI server. 😎
+
 ## `fastapi dev`
 
 When you run `fastapi dev`, it will run on development mode.
 
 By default, it will have **auto-reload** enabled, so it will automatically reload the server when you make changes to your code. This is resource intensive and could be less stable than without it, you should only use it for development.
 
 By default it will listen on the IP address `127.0.0.1`, which is the IP for your machine to communicate with itself alone (`localhost`).
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fastapi-cli Version: 0.0.2 Summary: Run and manage
+Metadata-Version: 2.1 Name: fastapi-cli Version: 0.0.3 Summary: Run and manage
 FastAPI apps from the command line with FastAPI CLI. ð Home-page: https://
 github.com/tiangolo/fastapi-cli Author-Email: =?utf-
 8?q?Sebasti=C3=A1n_Ram=C3=ADrez?=
 gmail.com> License: MIT Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators Classifier: Operating
 System :: OS Independent Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python Classifier: Topic :: Software
@@ -16,15 +16,15 @@
 3.7 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11 Classifier: Programming
 Language :: Python :: 3.12 Classifier: License :: OSI Approved :: MIT License
 Project-URL: Documentation, https://fastapi.tiangolo.com Project-URL: Homepage,
 https://github.com/tiangolo/fastapi-cli Project-URL: Repository, https://
 github.com/tiangolo/fastapi-cli Requires-Python: >=3.8 Requires-Dist:
-typer>=0.12.3 Requires-Dist: fastapi Requires-Dist: uvicorn[standard]>=0.29.0
+typer>=0.12.3 Requires-Dist: fastapi Requires-Dist: uvicorn[standard]>=0.15.0
 Description-Content-Type: text/markdown # FastAPI CLI _[_T_e_s_t_]_[_P_u_b_l_i_s_h_]
 _[_C_o_v_e_r_a_g_e_]_[_P_a_c_k_a_g_e_ _v_e_r_s_i_o_n_]_-_-_-_ _*_*_S_o_u_r_c_e_ _C_o_d_e_*_*_:_ _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_t_i_a_n_g_o_l_o_/
 _f_a_s_t_a_p_i_-_c_l_i_ _-_-_-_ _R_u_n_ _a_n_d_ _m_a_n_a_g_e_ _F_a_s_t_A_P_I_ _a_p_p_s_ _f_r_o_m_ _t_h_e_ _c_o_m_m_a_n_d_ _l_i_n_e_ _w_i_t_h_ _F_a_s_t_A_P_I
 _C_L_I_._ _ð____ _#_#_ _D_e_s_c_r_i_p_t_i_o_n_ _*_*_F_a_s_t_A_P_I_ _C_L_I_*_*_ _i_s_ _a_ _c_o_m_m_a_n_d_ _l_i_n_e_ _p_r_o_g_r_a_m_ _`_f_a_s_t_a_p_i_`
 _t_h_a_t_ _y_o_u_ _c_a_n_ _u_s_e_ _t_o_ _s_e_r_v_e_ _y_o_u_r_ _F_a_s_t_A_P_I_ _a_p_p_,_ _m_a_n_a_g_e_ _y_o_u_r_ _F_a_s_t_A_P_I_ _p_r_o_j_e_c_t_,_ _a_n_d
 _m_o_r_e_._ _W_h_e_n_ _y_o_u_ _i_n_s_t_a_l_l_ _F_a_s_t_A_P_I_ _(_e_._g_._ _w_i_t_h_ _`_p_i_p_ _i_n_s_t_a_l_l_ _f_a_s_t_a_p_i_`_)_,_ _i_t_ _i_n_c_l_u_d_e_s_ _a
 _p_a_c_k_a_g_e_ _c_a_l_l_e_d_ _`_f_a_s_t_a_p_i_-_c_l_i_`_,_ _t_h_i_s_ _p_a_c_k_a_g_e_ _p_r_o_v_i_d_e_s_ _t_h_e_ _`_f_a_s_t_a_p_i_`_ _c_o_m_m_a_n_d_ _i_n
@@ -49,24 +49,26 @@
 _a_w_e_s_o_m_e_a_p_p_'_]_ _I_N_F_O_:_ _U_v_i_c_o_r_n_ _r_u_n_n_i_n_g_ _o_n_ _h_t_t_p_:_/_/_1_2_7_._0_._0_._1_:_8_0_0_0_ _(_P_r_e_s_s_ _C_T_R_L_+_C_ _t_o
 _q_u_i_t_)_ _I_N_F_O_:_ _S_t_a_r_t_e_d_ _r_e_l_o_a_d_e_r_ _p_r_o_c_e_s_s_ _[_5_6_3_4_5_]_ _u_s_i_n_g_ _W_a_t_c_h_F_i_l_e_s_ _I_N_F_O_:_ _S_t_a_r_t_e_d
 _s_e_r_v_e_r_ _p_r_o_c_e_s_s_ _[_5_6_3_5_2_]_ _I_N_F_O_:_ _W_a_i_t_i_n_g_ _f_o_r_ _a_p_p_l_i_c_a_t_i_o_n_ _s_t_a_r_t_u_p_._ _I_N_F_O_:_ _A_p_p_l_i_c_a_t_i_o_n
 _s_t_a_r_t_u_p_ _c_o_m_p_l_e_t_e_._ _`_`_`
 _T_h_a_t_ _c_o_m_m_a_n_d_ _l_i_n_e_ _p_r_o_g_r_a_m_ _c_a_l_l_e_d_ _`_f_a_s_t_a_p_i_`_ _i_s_ _*_*_F_a_s_t_A_P_I_ _C_L_I_*_*_._ _F_a_s_t_A_P_I_ _C_L_I
 _t_a_k_e_s_ _t_h_e_ _p_a_t_h_ _t_o_ _y_o_u_r_ _P_y_t_h_o_n_ _p_r_o_g_r_a_m_ _a_n_d_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _d_e_t_e_c_t_s_ _t_h_e_ _v_a_r_i_a_b_l_e
 _w_i_t_h_ _t_h_e_ _F_a_s_t_A_P_I_ _(_c_o_m_m_o_n_l_y_ _n_a_m_e_d_ _`_a_p_p_`_)_ _a_n_d_ _h_o_w_ _t_o_ _i_m_p_o_r_t_ _i_t_,_ _a_n_d_ _t_h_e_n_ _s_e_r_v_e_s
-_i_t_._ _F_o_r_ _p_r_o_d_u_c_t_i_o_n_ _y_o_u_ _w_o_u_l_d_ _u_s_e_ _`_f_a_s_t_a_p_i_ _r_u_n_`_ _i_n_s_t_e_a_d_._ _ð____ _#_#_ _`_f_a_s_t_a_p_i_ _d_e_v_`
-_W_h_e_n_ _y_o_u_ _r_u_n_ _`_f_a_s_t_a_p_i_ _d_e_v_`_,_ _i_t_ _w_i_l_l_ _r_u_n_ _o_n_ _d_e_v_e_l_o_p_m_e_n_t_ _m_o_d_e_._ _B_y_ _d_e_f_a_u_l_t_,_ _i_t
-_w_i_l_l_ _h_a_v_e_ _*_*_a_u_t_o_-_r_e_l_o_a_d_*_*_ _e_n_a_b_l_e_d_,_ _s_o_ _i_t_ _w_i_l_l_ _a_u_t_o_m_a_t_i_c_a_l_l_y_ _r_e_l_o_a_d_ _t_h_e_ _s_e_r_v_e_r
-_w_h_e_n_ _y_o_u_ _m_a_k_e_ _c_h_a_n_g_e_s_ _t_o_ _y_o_u_r_ _c_o_d_e_._ _T_h_i_s_ _i_s_ _r_e_s_o_u_r_c_e_ _i_n_t_e_n_s_i_v_e_ _a_n_d_ _c_o_u_l_d_ _b_e
-_l_e_s_s_ _s_t_a_b_l_e_ _t_h_a_n_ _w_i_t_h_o_u_t_ _i_t_,_ _y_o_u_ _s_h_o_u_l_d_ _o_n_l_y_ _u_s_e_ _i_t_ _f_o_r_ _d_e_v_e_l_o_p_m_e_n_t_._ _B_y_ _d_e_f_a_u_l_t
-_i_t_ _w_i_l_l_ _l_i_s_t_e_n_ _o_n_ _t_h_e_ _I_P_ _a_d_d_r_e_s_s_ _`_1_2_7_._0_._0_._1_`_,_ _w_h_i_c_h_ _i_s_ _t_h_e_ _I_P_ _f_o_r_ _y_o_u_r_ _m_a_c_h_i_n_e
-_t_o_ _c_o_m_m_u_n_i_c_a_t_e_ _w_i_t_h_ _i_t_s_e_l_f_ _a_l_o_n_e_ _(_`_l_o_c_a_l_h_o_s_t_`_)_._ _#_#_ _`_f_a_s_t_a_p_i_ _r_u_n_`_ _W_h_e_n_ _y_o_u_ _r_u_n
-_`_f_a_s_t_a_p_i_ _r_u_n_`_,_ _i_t_ _w_i_l_l_ _r_u_n_ _o_n_ _p_r_o_d_u_c_t_i_o_n_ _m_o_d_e_ _b_y_ _d_e_f_a_u_l_t_._ _I_t_ _w_i_l_l_ _h_a_v_e_ _*_*_a_u_t_o_-
-_r_e_l_o_a_d_ _d_i_s_a_b_l_e_d_*_*_ _b_y_ _d_e_f_a_u_l_t_._ _I_t_ _w_i_l_l_ _l_i_s_t_e_n_ _o_n_ _t_h_e_ _I_P_ _a_d_d_r_e_s_s_ _`_0_._0_._0_._0_`_,_ _w_h_i_c_h
-_m_e_a_n_s_ _a_l_l_ _t_h_e_ _a_v_a_i_l_a_b_l_e_ _I_P_ _a_d_d_r_e_s_s_e_s_,_ _t_h_i_s_ _w_a_y_ _i_t_ _w_i_l_l_ _b_e_ _p_u_b_l_i_c_l_y_ _a_c_c_e_s_s_i_b_l_e
-_t_o_ _a_n_y_o_n_e_ _t_h_a_t_ _c_a_n_ _c_o_m_m_u_n_i_c_a_t_e_ _w_i_t_h_ _t_h_e_ _m_a_c_h_i_n_e_._ _T_h_i_s_ _i_s_ _h_o_w_ _y_o_u_ _w_o_u_l_d_ _n_o_r_m_a_l_l_y
-_r_u_n_ _i_t_ _i_n_ _p_r_o_d_u_c_t_i_o_n_,_ _f_o_r_ _e_x_a_m_p_l_e_,_ _i_n_ _a_ _c_o_n_t_a_i_n_e_r_._ _I_n_ _m_o_s_t_ _c_a_s_e_s_ _y_o_u_ _w_o_u_l_d_ _(_a_n_d
-_s_h_o_u_l_d_)_ _h_a_v_e_ _a_ _"_t_e_r_m_i_n_a_t_i_o_n_ _p_r_o_x_y_"_ _h_a_n_d_l_i_n_g_ _H_T_T_P_S_ _f_o_r_ _y_o_u_ _o_n_ _t_o_p_,_ _t_h_i_s_ _w_i_l_l
-_d_e_p_e_n_d_ _o_n_ _h_o_w_ _y_o_u_ _d_e_p_l_o_y_ _y_o_u_r_ _a_p_p_l_i_c_a_t_i_o_n_,_ _y_o_u_r_ _p_r_o_v_i_d_e_r_ _m_i_g_h_t_ _d_o_ _t_h_i_s_ _f_o_r_ _y_o_u_,
-_o_r_ _y_o_u_ _m_i_g_h_t_ _n_e_e_d_ _t_o_ _s_e_t_ _i_t_ _u_p_ _y_o_u_r_s_e_l_f_._ _Y_o_u_ _c_a_n_ _l_e_a_r_n_ _m_o_r_e_ _a_b_o_u_t_ _i_t_ _i_n_ _t_h_e
-_F_a_s_t_A_P_I_ _D_e_p_l_o_y_m_e_n_t_ _d_o_c_u_m_e_n_t_a_t_i_o_n_._ _#_#_ _L_i_c_e_n_s_e_ _T_h_i_s_ _p_r_o_j_e_c_t_ _i_s_ _l_i_c_e_n_s_e_d_ _u_n_d_e_r_ _t_h_e
-_t_e_r_m_s_ _o_f_ _t_h_e_ _M_I_T_ _l_i_c_e_n_s_e_.
+_i_t_._ _F_o_r_ _p_r_o_d_u_c_t_i_o_n_ _y_o_u_ _w_o_u_l_d_ _u_s_e_ _`_f_a_s_t_a_p_i_ _r_u_n_`_ _i_n_s_t_e_a_d_._ _ð____ _I_n_t_e_r_n_a_l_l_y_,
+_*_*_F_a_s_t_A_P_I_ _C_L_I_*_*_ _u_s_e_s_ _U_v_i_c_o_r_n_,_ _a_ _h_i_g_h_-_p_e_r_f_o_r_m_a_n_c_e_,_ _p_r_o_d_u_c_t_i_o_n_-_r_e_a_d_y_,_ _A_S_G_I
+_s_e_r_v_e_r_._ _ð____ _#_#_ _`_f_a_s_t_a_p_i_ _d_e_v_`_ _W_h_e_n_ _y_o_u_ _r_u_n_ _`_f_a_s_t_a_p_i_ _d_e_v_`_,_ _i_t_ _w_i_l_l_ _r_u_n_ _o_n
+_d_e_v_e_l_o_p_m_e_n_t_ _m_o_d_e_._ _B_y_ _d_e_f_a_u_l_t_,_ _i_t_ _w_i_l_l_ _h_a_v_e_ _*_*_a_u_t_o_-_r_e_l_o_a_d_*_*_ _e_n_a_b_l_e_d_,_ _s_o_ _i_t_ _w_i_l_l
+_a_u_t_o_m_a_t_i_c_a_l_l_y_ _r_e_l_o_a_d_ _t_h_e_ _s_e_r_v_e_r_ _w_h_e_n_ _y_o_u_ _m_a_k_e_ _c_h_a_n_g_e_s_ _t_o_ _y_o_u_r_ _c_o_d_e_._ _T_h_i_s_ _i_s
+_r_e_s_o_u_r_c_e_ _i_n_t_e_n_s_i_v_e_ _a_n_d_ _c_o_u_l_d_ _b_e_ _l_e_s_s_ _s_t_a_b_l_e_ _t_h_a_n_ _w_i_t_h_o_u_t_ _i_t_,_ _y_o_u_ _s_h_o_u_l_d_ _o_n_l_y
+_u_s_e_ _i_t_ _f_o_r_ _d_e_v_e_l_o_p_m_e_n_t_._ _B_y_ _d_e_f_a_u_l_t_ _i_t_ _w_i_l_l_ _l_i_s_t_e_n_ _o_n_ _t_h_e_ _I_P_ _a_d_d_r_e_s_s
+_`_1_2_7_._0_._0_._1_`_,_ _w_h_i_c_h_ _i_s_ _t_h_e_ _I_P_ _f_o_r_ _y_o_u_r_ _m_a_c_h_i_n_e_ _t_o_ _c_o_m_m_u_n_i_c_a_t_e_ _w_i_t_h_ _i_t_s_e_l_f_ _a_l_o_n_e
+_(_`_l_o_c_a_l_h_o_s_t_`_)_._ _#_#_ _`_f_a_s_t_a_p_i_ _r_u_n_`_ _W_h_e_n_ _y_o_u_ _r_u_n_ _`_f_a_s_t_a_p_i_ _r_u_n_`_,_ _i_t_ _w_i_l_l_ _r_u_n_ _o_n
+_p_r_o_d_u_c_t_i_o_n_ _m_o_d_e_ _b_y_ _d_e_f_a_u_l_t_._ _I_t_ _w_i_l_l_ _h_a_v_e_ _*_*_a_u_t_o_-_r_e_l_o_a_d_ _d_i_s_a_b_l_e_d_*_*_ _b_y_ _d_e_f_a_u_l_t_.
+_I_t_ _w_i_l_l_ _l_i_s_t_e_n_ _o_n_ _t_h_e_ _I_P_ _a_d_d_r_e_s_s_ _`_0_._0_._0_._0_`_,_ _w_h_i_c_h_ _m_e_a_n_s_ _a_l_l_ _t_h_e_ _a_v_a_i_l_a_b_l_e_ _I_P
+_a_d_d_r_e_s_s_e_s_,_ _t_h_i_s_ _w_a_y_ _i_t_ _w_i_l_l_ _b_e_ _p_u_b_l_i_c_l_y_ _a_c_c_e_s_s_i_b_l_e_ _t_o_ _a_n_y_o_n_e_ _t_h_a_t_ _c_a_n
+_c_o_m_m_u_n_i_c_a_t_e_ _w_i_t_h_ _t_h_e_ _m_a_c_h_i_n_e_._ _T_h_i_s_ _i_s_ _h_o_w_ _y_o_u_ _w_o_u_l_d_ _n_o_r_m_a_l_l_y_ _r_u_n_ _i_t_ _i_n
+_p_r_o_d_u_c_t_i_o_n_,_ _f_o_r_ _e_x_a_m_p_l_e_,_ _i_n_ _a_ _c_o_n_t_a_i_n_e_r_._ _I_n_ _m_o_s_t_ _c_a_s_e_s_ _y_o_u_ _w_o_u_l_d_ _(_a_n_d_ _s_h_o_u_l_d_)
+_h_a_v_e_ _a_ _"_t_e_r_m_i_n_a_t_i_o_n_ _p_r_o_x_y_"_ _h_a_n_d_l_i_n_g_ _H_T_T_P_S_ _f_o_r_ _y_o_u_ _o_n_ _t_o_p_,_ _t_h_i_s_ _w_i_l_l_ _d_e_p_e_n_d_ _o_n
+_h_o_w_ _y_o_u_ _d_e_p_l_o_y_ _y_o_u_r_ _a_p_p_l_i_c_a_t_i_o_n_,_ _y_o_u_r_ _p_r_o_v_i_d_e_r_ _m_i_g_h_t_ _d_o_ _t_h_i_s_ _f_o_r_ _y_o_u_,_ _o_r_ _y_o_u
+_m_i_g_h_t_ _n_e_e_d_ _t_o_ _s_e_t_ _i_t_ _u_p_ _y_o_u_r_s_e_l_f_._ _Y_o_u_ _c_a_n_ _l_e_a_r_n_ _m_o_r_e_ _a_b_o_u_t_ _i_t_ _i_n_ _t_h_e_ _F_a_s_t_A_P_I
+_D_e_p_l_o_y_m_e_n_t_ _d_o_c_u_m_e_n_t_a_t_i_o_n_._ _#_#_ _L_i_c_e_n_s_e_ _T_h_i_s_ _p_r_o_j_e_c_t_ _i_s_ _l_i_c_e_n_s_e_d_ _u_n_d_e_r_ _t_h_e_ _t_e_r_m_s
+_o_f_ _t_h_e_ _M_I_T_ _l_i_c_e_n_s_e_.
```

