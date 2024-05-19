# Comparing `tmp/all_repos_envvar-1.1.5.tar.gz` & `tmp/all_repos_envvar-1.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "all_repos_envvar-1.1.5.tar", max compression
+gzip compressed data, was "all_repos_envvar-1.1.6.tar", max compression
```

## Comparing `all_repos_envvar-1.1.5.tar` & `all_repos_envvar-1.1.6.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1068 2024-03-05 11:44:26.291701 all_repos_envvar-1.1.5/LICENSE
--rw-r--r--   0        0        0     4938 2024-03-05 11:44:26.291701 all_repos_envvar-1.1.5/README.md
--rw-r--r--   0        0        0     3253 2024-03-05 11:44:27.319706 all_repos_envvar-1.1.5/pyproject.toml
--rw-r--r--   0        0        0       22 2024-03-05 11:44:27.323706 all_repos_envvar-1.1.5/src/all_repos_envvar/__init__.py
--rw-r--r--   0        0        0      614 2024-03-05 11:44:26.291701 all_repos_envvar-1.1.5/src/all_repos_envvar/mixin.py
--rw-r--r--   0        0        0      211 2024-03-05 11:44:26.291701 all_repos_envvar-1.1.5/src/all_repos_envvar/push.py
--rw-r--r--   0        0        0        0 2024-03-05 11:44:26.291701 all_repos_envvar-1.1.5/src/all_repos_envvar/py.typed
--rw-r--r--   0        0        0      212 2024-03-05 11:44:26.291701 all_repos_envvar-1.1.5/src/all_repos_envvar/source.py
--rw-r--r--   0        0        0     6336 1970-01-01 00:00:00.000000 all_repos_envvar-1.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-19 10:25:24.944847 all_repos_envvar-1.1.6/LICENSE
+-rw-r--r--   0        0        0     5583 2024-05-19 10:25:24.944847 all_repos_envvar-1.1.6/README.md
+-rw-r--r--   0        0        0     3209 2024-05-19 10:25:26.672854 all_repos_envvar-1.1.6/pyproject.toml
+-rw-r--r--   0        0        0       22 2024-05-19 10:25:26.672854 all_repos_envvar-1.1.6/src/all_repos_envvar/__init__.py
+-rw-r--r--   0        0        0      614 2024-05-19 10:25:24.944847 all_repos_envvar-1.1.6/src/all_repos_envvar/mixin.py
+-rw-r--r--   0        0        0      211 2024-05-19 10:25:24.944847 all_repos_envvar-1.1.6/src/all_repos_envvar/push.py
+-rw-r--r--   0        0        0        0 2024-05-19 10:25:24.944847 all_repos_envvar-1.1.6/src/all_repos_envvar/py.typed
+-rw-r--r--   0        0        0      212 2024-05-19 10:25:24.944847 all_repos_envvar-1.1.6/src/all_repos_envvar/source.py
+-rw-r--r--   0        0        0     6981 1970-01-01 00:00:00.000000 all_repos_envvar-1.1.6/PKG-INFO
```

### Comparing `all_repos_envvar-1.1.5/LICENSE` & `all_repos_envvar-1.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `all_repos_envvar-1.1.5/README.md` & `all_repos_envvar-1.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -31,14 +31,17 @@
 
 **Source Code**: <a href="https://github.com/browniebroke/all-repos-envvar" target="_blank">https://github.com/browniebroke/all-repos-envvar</a>
 
 ---
 
 An all-repos extension to read values from environment variables.
 
+> [!IMPORTANT]
+> As of [all-repos v1.25](https://github.com/asottile/all-repos/releases/tag/v1.25.0), you may not need this package, see [section below](#why)
+
 ## Installation
 
 Install this via pip (or your favourite package manager):
 
 `pip install all-repos-envvar`
 
 ## Usage
@@ -55,15 +58,21 @@
   "push": "all_repos_envvar.push",
   "push_settings": {
     "username": "browniebroke"
   }
 }
 ```
 
-I wanted this feature, but it looks like it won't be implemented in the main repo, hence this little extension. The source module extends `all_repos.source.github` and the push module extends `all_repos.push.github_pull_request`
+The source module extends `all_repos.source.github` and the push module extends `all_repos.push.github_pull_request`.
+
+## Why
+
+I wanted this feature, but at the time, it looked like [it would never be implemented in the main repo](https://github.com/asottile/all-repos/issues/79), hence this little extension. Since then, the author of all-repos apparently changed their mind and support for reading from environment variable [was added in early 2023](https://github.com/asottile/all-repos/pull/275), and it's now included since release v1.25.0.
+
+The only extra feature that this package provides is to read from `.env` file, but this can be achieved by more general solutions like [`direnv`](https://direnv.net).
 
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
```

#### html2text {}

```diff
@@ -1,26 +1,34 @@
 # all-repos-envvar
                      _[_C_I_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_b_l_a_c_k_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 --- **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_b_r_o_w_n_i_e_b_r_o_k_e_/_a_l_l_-_r_e_p_o_s_-_e_n_v_v_a_r --- An
-all-repos extension to read values from environment variables. ## Installation
-Install this via pip (or your favourite package manager): `pip install all-
-repos-envvar` ## Usage This library should be installed alongside `all-repos`
-so that it's findable at import time. It provides a custom `source` and `push`
-to get the GitHub API key from an environment variable `GITHUB_API_KEY`
-(reading from and `.env` file is also supported), allowing you to omit it from
-the config: ```json { "output_dir": "output", "source":
+all-repos extension to read values from environment variables. > [!IMPORTANT] >
+As of [all-repos v1.25](https://github.com/asottile/all-repos/releases/tag/
+v1.25.0), you may not need this package, see [section below](#why) ##
+Installation Install this via pip (or your favourite package manager): `pip
+install all-repos-envvar` ## Usage This library should be installed alongside
+`all-repos` so that it's findable at import time. It provides a custom `source`
+and `push` to get the GitHub API key from an environment variable
+`GITHUB_API_KEY` (reading from and `.env` file is also supported), allowing you
+to omit it from the config: ```json { "output_dir": "output", "source":
 "all_repos_envvar.source", "source_settings": { "username": "browniebroke" },
 "push": "all_repos_envvar.push", "push_settings": { "username": "browniebroke"
-} } ``` I wanted this feature, but it looks like it won't be implemented in the
-main repo, hence this little extension. The source module extends
-`all_repos.source.github` and the push module extends
-`all_repos.push.github_pull_request` ## Contributors â¨ Thanks goes to these
-wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+} } ``` The source module extends `all_repos.source.github` and the push module
+extends `all_repos.push.github_pull_request`. ## Why I wanted this feature, but
+at the time, it looked like [it would never be implemented in the main repo]
+(https://github.com/asottile/all-repos/issues/79), hence this little extension.
+Since then, the author of all-repos apparently changed their mind and support
+for reading from environment variable [was added in early 2023](https://
+github.com/asottile/all-repos/pull/275), and it's now included since release
+v1.25.0. The only extra feature that this package provides is to read from
+`.env` file, but this can be achieved by more general solutions like [`direnv`]
+(https://direnv.net). ## Contributors â¨ Thanks goes to these wonderful people
+([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
   _BB_rr_uu_nn_oo_ _AA_ll_ll_aa
 
 _ð___» _ð__¤_ _ð___
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! ## Credits This package was created with [Cookiecutter](https://
```

### Comparing `all_repos_envvar-1.1.5/pyproject.toml` & `all_repos_envvar-1.1.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,22 @@
 [tool.poetry]
 name = "all-repos-envvar"
-version = "1.1.5"
+version = "1.1.6"
 description = "An all-repos extension to read values from environment variables."
 authors = ["Bruno Alla <alla.brunoo@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/browniebroke/all-repos-envvar"
 documentation = "https://all-repos-envvar.readthedocs.io"
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Intended Audience :: Developers",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries",
-    "Programming Language :: Python :: 3.12",
 ]
 packages = [
     { include = "all_repos_envvar", from = "src" },
 ]
 
 [tool.poetry.urls]
 "Bug Tracker" = "https://github.com/browniebroke/all-repos-envvar/issues"
@@ -28,15 +27,15 @@
 [tool.poetry.dependencies]
 python = "^3.8"
 all-repos = ">=1"
 environs = ">=10.0"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^8.0"
-pytest-cov = "^4.0"
+pytest-cov = "^5.0.0"
 
 [tool.semantic_release]
 version_toml = ["pyproject.toml:tool.poetry.version"]
 version_variables = [
     "src/all_repos_envvar/__init__.py:__version__",
 ]
 build_command = "pip install poetry && poetry build"
```

### Comparing `all_repos_envvar-1.1.5/src/all_repos_envvar/mixin.py` & `all_repos_envvar-1.1.6/src/all_repos_envvar/mixin.py`

 * *Files identical despite different names*

### Comparing `all_repos_envvar-1.1.5/PKG-INFO` & `all_repos_envvar-1.1.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: all-repos-envvar
-Version: 1.1.5
+Version: 1.1.6
 Summary: An all-repos extension to read values from environment variables.
 Home-page: https://github.com/browniebroke/all-repos-envvar
 License: MIT
 Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -62,14 +62,17 @@
 
 **Source Code**: <a href="https://github.com/browniebroke/all-repos-envvar" target="_blank">https://github.com/browniebroke/all-repos-envvar</a>
 
 ---
 
 An all-repos extension to read values from environment variables.
 
+> [!IMPORTANT]
+> As of [all-repos v1.25](https://github.com/asottile/all-repos/releases/tag/v1.25.0), you may not need this package, see [section below](#why)
+
 ## Installation
 
 Install this via pip (or your favourite package manager):
 
 `pip install all-repos-envvar`
 
 ## Usage
@@ -86,15 +89,21 @@
   "push": "all_repos_envvar.push",
   "push_settings": {
     "username": "browniebroke"
   }
 }
 ```
 
-I wanted this feature, but it looks like it won't be implemented in the main repo, hence this little extension. The source module extends `all_repos.source.github` and the push module extends `all_repos.push.github_pull_request`
+The source module extends `all_repos.source.github` and the push module extends `all_repos.push.github_pull_request`.
+
+## Why
+
+I wanted this feature, but at the time, it looked like [it would never be implemented in the main repo](https://github.com/asottile/all-repos/issues/79), hence this little extension. Since then, the author of all-repos apparently changed their mind and support for reading from environment variable [was added in early 2023](https://github.com/asottile/all-repos/pull/275), and it's now included since release v1.25.0.
+
+The only extra feature that this package provides is to read from `.env` file, but this can be achieved by more general solutions like [`direnv`](https://direnv.net).
 
 ## Contributors ✨
 
 Thanks goes to these wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
 <!-- prettier-ignore-start -->
 <!-- ALL-CONTRIBUTORS-LIST:START - Do not remove or modify this section -->
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: all-repos-envvar Version: 1.1.5 Summary: An all-
+Metadata-Version: 2.1 Name: all-repos-envvar Version: 1.1.6 Summary: An all-
 repos extension to read values from environment variables. Home-page: https://
 github.com/browniebroke/all-repos-envvar License: MIT Author: Bruno Alla
 Author-email: alla.brunoo@gmail.com Requires-Python: >=3.8,<4.0 Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License Classifier: Natural Language
 :: English Classifier: Operating System :: OS Independent Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
@@ -17,28 +17,36 @@
 @browniebroke Project-URL: Repository, https://github.com/browniebroke/all-
 repos-envvar Project-URL: Twitter, https://twitter.com/_BrunoAlla Description-
 Content-Type: text/markdown # all-repos-envvar
                      _[_C_I_ _S_t_a_t_u_s_]_[_T_e_s_t_ _c_o_v_e_r_a_g_e_ _p_e_r_c_e_n_t_a_g_e_]
                           _[_P_o_e_t_r_y_]_[_b_l_a_c_k_]_[_p_r_e_-_c_o_m_m_i_t_]
               _[_P_y_P_I_ _V_e_r_s_i_o_n_][Supported Python versions][License]
 --- **Source Code**: _h_t_t_p_s_:_/_/_g_i_t_h_u_b_._c_o_m_/_b_r_o_w_n_i_e_b_r_o_k_e_/_a_l_l_-_r_e_p_o_s_-_e_n_v_v_a_r --- An
-all-repos extension to read values from environment variables. ## Installation
-Install this via pip (or your favourite package manager): `pip install all-
-repos-envvar` ## Usage This library should be installed alongside `all-repos`
-so that it's findable at import time. It provides a custom `source` and `push`
-to get the GitHub API key from an environment variable `GITHUB_API_KEY`
-(reading from and `.env` file is also supported), allowing you to omit it from
-the config: ```json { "output_dir": "output", "source":
+all-repos extension to read values from environment variables. > [!IMPORTANT] >
+As of [all-repos v1.25](https://github.com/asottile/all-repos/releases/tag/
+v1.25.0), you may not need this package, see [section below](#why) ##
+Installation Install this via pip (or your favourite package manager): `pip
+install all-repos-envvar` ## Usage This library should be installed alongside
+`all-repos` so that it's findable at import time. It provides a custom `source`
+and `push` to get the GitHub API key from an environment variable
+`GITHUB_API_KEY` (reading from and `.env` file is also supported), allowing you
+to omit it from the config: ```json { "output_dir": "output", "source":
 "all_repos_envvar.source", "source_settings": { "username": "browniebroke" },
 "push": "all_repos_envvar.push", "push_settings": { "username": "browniebroke"
-} } ``` I wanted this feature, but it looks like it won't be implemented in the
-main repo, hence this little extension. The source module extends
-`all_repos.source.github` and the push module extends
-`all_repos.push.github_pull_request` ## Contributors â¨ Thanks goes to these
-wonderful people ([emoji key](https://allcontributors.org/docs/en/emoji-key)):
+} } ``` The source module extends `all_repos.source.github` and the push module
+extends `all_repos.push.github_pull_request`. ## Why I wanted this feature, but
+at the time, it looked like [it would never be implemented in the main repo]
+(https://github.com/asottile/all-repos/issues/79), hence this little extension.
+Since then, the author of all-repos apparently changed their mind and support
+for reading from environment variable [was added in early 2023](https://
+github.com/asottile/all-repos/pull/275), and it's now included since release
+v1.25.0. The only extra feature that this package provides is to read from
+`.env` file, but this can be achieved by more general solutions like [`direnv`]
+(https://direnv.net). ## Contributors â¨ Thanks goes to these wonderful people
+([emoji key](https://allcontributors.org/docs/en/emoji-key)):
 
   _BB_rr_uu_nn_oo_ _AA_ll_ll_aa
 
 _ð___» _ð__¤_ _ð___
 This project follows the [all-contributors](https://github.com/all-
 contributors/all-contributors) specification. Contributions of any kind
 welcome! ## Credits This package was created with [Cookiecutter](https://
```

