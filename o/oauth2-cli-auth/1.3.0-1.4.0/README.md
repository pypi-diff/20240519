# Comparing `tmp/oauth2_cli_auth-1.3.0.tar.gz` & `tmp/oauth2_cli_auth-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oauth2_cli_auth-1.3.0.tar", max compression
+gzip compressed data, was "oauth2_cli_auth-1.4.0.tar", max compression
```

## Comparing `oauth2_cli_auth-1.3.0.tar` & `oauth2_cli_auth-1.4.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1068 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/LICENSE
--rw-r--r--   0        0        0     7510 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/README.md
--rw-r--r--   0        0        0      338 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/oauth2_cli_auth/__init__.py
--rw-r--r--   0        0        0      495 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/oauth2_cli_auth/_timeout.py
--rw-r--r--   0        0        0      769 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/oauth2_cli_auth/_urllib_util.py
--rw-r--r--   0        0        0     4080 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/oauth2_cli_auth/code_grant.py
--rw-r--r--   0        0        0      221 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/oauth2_cli_auth/conftest.py
--rw-r--r--   0        0        0     7512 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/oauth2_cli_auth/http_server.py
--rw-r--r--   0        0        0      985 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/oauth2_cli_auth/simplified_flow.py
--rw-r--r--   0        0        0     1235 2024-05-16 08:37:14.046018 oauth2_cli_auth-1.3.0/pyproject.toml
--rw-r--r--   0        0        0     8605 1970-01-01 00:00:00.000000 oauth2_cli_auth-1.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-05-19 15:31:23.929041 oauth2_cli_auth-1.4.0/LICENSE
+-rw-r--r--   0        0        0     7510 2024-05-19 15:31:23.929041 oauth2_cli_auth-1.4.0/README.md
+-rw-r--r--   0        0        0      338 2024-05-19 15:31:23.929041 oauth2_cli_auth-1.4.0/oauth2_cli_auth/__init__.py
+-rw-r--r--   0        0        0      495 2024-05-19 15:31:23.929041 oauth2_cli_auth-1.4.0/oauth2_cli_auth/_timeout.py
+-rw-r--r--   0        0        0      769 2024-05-19 15:31:23.929041 oauth2_cli_auth-1.4.0/oauth2_cli_auth/_urllib_util.py
+-rw-r--r--   0        0        0     4065 2024-05-19 15:31:23.929041 oauth2_cli_auth-1.4.0/oauth2_cli_auth/code_grant.py
+-rw-r--r--   0        0        0      221 2024-05-19 15:31:23.929041 oauth2_cli_auth-1.4.0/oauth2_cli_auth/conftest.py
+-rw-r--r--   0        0        0     7701 2024-05-19 15:31:23.929041 oauth2_cli_auth-1.4.0/oauth2_cli_auth/http_server.py
+-rw-r--r--   0        0        0     1017 2024-05-19 15:31:23.929041 oauth2_cli_auth-1.4.0/oauth2_cli_auth/simplified_flow.py
+-rw-r--r--   0        0        0     1723 2024-05-19 15:31:23.933041 oauth2_cli_auth-1.4.0/pyproject.toml
+-rw-r--r--   0        0        0     8605 1970-01-01 00:00:00.000000 oauth2_cli_auth-1.4.0/PKG-INFO
```

### Comparing `oauth2_cli_auth-1.3.0/LICENSE` & `oauth2_cli_auth-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oauth2_cli_auth-1.3.0/README.md` & `oauth2_cli_auth-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `oauth2_cli_auth-1.3.0/oauth2_cli_auth/_urllib_util.py` & `oauth2_cli_auth-1.4.0/oauth2_cli_auth/_urllib_util.py`

 * *Files identical despite different names*

### Comparing `oauth2_cli_auth-1.3.0/oauth2_cli_auth/code_grant.py` & `oauth2_cli_auth-1.4.0/oauth2_cli_auth/code_grant.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+"""
+Functionality to work with OAuth2 code grant
+"""
 import base64
 import urllib.parse
 import urllib.request
 import webbrowser
 from collections.abc import Callable
 from dataclasses import dataclass
 
@@ -30,14 +33,19 @@
             token_url=config.get("token_endpoint"),
             client_id=client_id,
             scopes=scopes,
         )
 
 
 def load_oidc_config(odic_well_known_endpoint: str) -> dict:
+    """
+    Load OIDC configuration from the well known configuration endpoint
+
+    :param odic_well_known_endpoint: Endpoint to load configuration from
+    """
     config = _load_json(odic_well_known_endpoint)
     return config
 
 
 def open_browser(url: str, print_open_browser_instruction: Callable[[str], None] | None = print) -> None:
     """
     Open browser using webbrowser module and show message about URL open
@@ -72,16 +80,14 @@
 ) -> dict:
     """
     Exchange a code for an access token using the endpoints from client info and return the entire response
 
     :param client_info: Info about oauth2 client
     :param redirect_uri: Callback URL
     :param code: Code to redeem
-    :param access_token_field: Name of the field containing the access token to use. This might differ depending on
-                              the provider you are using. For example for Auth0 you have to set this to id_token
     :return: Response from OAuth2 endpoint
     """
     headers = {
         "Content-Type": "application/x-www-form-urlencoded",
         "Authorization": "Basic " + base64.b64encode(f"{client_info.client_id}:".encode()).decode(),
     }
```

### Comparing `oauth2_cli_auth-1.3.0/oauth2_cli_auth/http_server.py` & `oauth2_cli_auth-1.4.0/oauth2_cli_auth/http_server.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,21 @@
+"""
+Local HTTP server logic
+"""
 from http.server import BaseHTTPRequestHandler, HTTPServer
 from string import Template
 from typing import Optional
 from urllib.parse import parse_qs, urlparse
 from oauth2_cli_auth._timeout import _method_with_timeout, TimeoutException
 
 
 class CallbackPageTemplate:
+    """
+    Holder for callback page assets and template
+    """
     SUCCESS_SVG = """
     <svg xmlns="http://www.w3.org/2000/svg" width="154px" height="154px">
         <g fill="none" stroke="#22AE73" stroke-width="2">
             <circle cx="77" cy="77" r="72" style="stroke-dasharray:480px, 480px; stroke-dashoffset: 960px;"></circle>
             <circle id="colored" fill="#22AE73" cx="77" cy="77" r="72" style="stroke-dasharray:480px, 480px; stroke-dashoffset: 960px;"></circle>
             <polyline class="st0" stroke="#fff" stroke-width="10" points="43.5,77.8 63.7,97.9 112.2,49.4 " style="stroke-dasharray:100px, 100px; stroke-dashoffset: 200px;"/>
         </g>
@@ -145,14 +151,17 @@
             title=title,
             message=message,
             svg=self.ERROR_SVG if has_error else self.SUCCESS_SVG,
         )
 
 
 class OAuthRedirectHandler(BaseHTTPRequestHandler):
+    """
+    HTTPRequest Handler that is intended to be used as oauth2 callback page
+    """
     callback_template = CallbackPageTemplate()
 
     def log_message(self, format, *args):
         # silence the log messages
         pass
 
     def do_GET(self):
```

### Comparing `oauth2_cli_auth-1.3.0/oauth2_cli_auth/simplified_flow.py` & `oauth2_cli_auth-1.4.0/oauth2_cli_auth/simplified_flow.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,23 @@
+"""
+Ready to use workflows
+"""
 from oauth2_cli_auth import OAuthCallbackHttpServer, get_auth_url, exchange_code_for_access_token, OAuth2ClientInfo, \
     open_browser
 
 
 def get_access_token_with_browser_open(client_info: OAuth2ClientInfo, server_port: int = 8080) -> str:
     """
     Provides a simplified API to:
 
     - Spin up the callback server
     - Open the browser with the authorization URL
     - Wait for the code to arrive
     - Get access token from code
+
     :param client_info: Client Info for Oauth2 Interaction
     :param server_port: Port of the local web server to spin up
     :return: Access Token
     """
     callback_server = OAuthCallbackHttpServer(server_port)
     auth_url = get_auth_url(client_info, callback_server.callback_url)
     open_browser(auth_url)
```

### Comparing `oauth2_cli_auth-1.3.0/pyproject.toml` & `oauth2_cli_auth-1.4.0/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "oauth2-cli-auth"
-version = "1.3.0"
+version = "1.4.0"
 description = "Authenticate against OAuth2 Provider in Python CLIs"
 authors = ["Timo Reymann <mail@timo-reymann.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/timo-reymann/python-oauth2-cli-auth"
 packages = [
     { include = "oauth2_cli_auth" }
@@ -36,17 +36,38 @@
 url = "https://test.pypi.org/legacy/"
 priority="explicit"
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.4.3"
 coverage = "^7.3.2"
 pdoc3 = "^0.10.0"
+setuptools = "^69.5.1"
+pydoctor = "^23.9.1"
 
 [tool.coverage.run]
 omit = [".*", "*/site-packages/*", "*/*_test.py"]
 
 [tool.coverage.report]
 fail_under = 70
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
+
+[tool.pydoctor]
+verbose = 0
+warnings-as-errors = true
+
+intersphinx = ["https://docs.python.org/3/objects.inv"]
+docformat = "restructuredtext"
+html-output = "gh-pages"
+
+add-package = ["oauth2_cli_auth"]
+project-name = "oauth2_cli_auth"
+project-url = "https://github.com/timo-reymann/python-oauth2-cli-auth"
+privacy = [
+    "HIDDEN:oauth2_cli_auth.*_test",
+    "HIDDEN:oauth2_cli_auth.conftest"
+]
+
+theme = "base"
+template-dir = "pydoctor-theme"
```

### Comparing `oauth2_cli_auth-1.3.0/PKG-INFO` & `oauth2_cli_auth-1.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oauth2-cli-auth
-Version: 1.3.0
+Version: 1.4.0
 Summary: Authenticate against OAuth2 Provider in Python CLIs
 Home-page: https://github.com/timo-reymann/python-oauth2-cli-auth
 License: MIT
 Author: Timo Reymann
 Author-email: mail@timo-reymann.de
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
```

