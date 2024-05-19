# Comparing `tmp/fastblocks-0.3.9.tar.gz` & `tmp/fastblocks-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastblocks-0.3.9.tar", last modified: Thu Apr 11 14:55:14 2024, max compression
+gzip compressed data, was "fastblocks-0.4.0.tar", last modified: Sun May 19 17:35:23 2024, max compression
```

## Comparing `fastblocks-0.3.9.tar` & `fastblocks-0.4.0.tar`

### file list

```diff
@@ -1,33 +1,41 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.3.9/LICENSE
--rw-r--r--   0        0        0     1024 2023-09-28 16:26:56.729322 fastblocks-0.3.9/README.md
--rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 fastblocks-0.3.9/fastblocks/Dockerfile
--rw-r--r--   0        0        0       80 2024-04-11 14:21:21.798764 fastblocks-0.3.9/fastblocks/__init__.py
--rw-r--r--   0        0        0      191 2024-01-19 13:43:05.790330 fastblocks-0.3.9/fastblocks/__main__.py
--rw-r--r--   0        0        0       61 2024-01-16 17:26:09.440085 fastblocks-0.3.9/fastblocks/actions/__init__.py
--rw-r--r--   0        0        0      407 2023-12-10 08:11:45.418815 fastblocks-0.3.9/fastblocks/actions/minify.py
--rw-r--r--   0        0        0        0 2024-02-08 21:10:42.403063 fastblocks-0.3.9/fastblocks/adapters/__init__.py
--rw-r--r--   0        0        0       62 2023-11-04 13:50:49.302945 fastblocks-0.3.9/fastblocks/adapters/admin/__init__.py
--rw-r--r--   0        0        0       96 2024-02-05 00:13:09.758290 fastblocks-0.3.9/fastblocks/adapters/admin/_base.py
--rw-r--r--   0        0        0     2988 2024-02-09 12:51:23.096080 fastblocks-0.3.9/fastblocks/adapters/admin/sqladmin.py
--rw-r--r--   0        0        0       60 2023-11-04 13:49:17.900293 fastblocks-0.3.9/fastblocks/adapters/app/__init__.py
--rw-r--r--   0        0        0      312 2024-02-24 10:37:18.246405 fastblocks-0.3.9/fastblocks/adapters/app/_base.py
--rw-r--r--   0        0        0     2669 2024-03-31 09:28:05.032996 fastblocks-0.3.9/fastblocks/adapters/app/main.py
--rw-r--r--   0        0        0       61 2024-01-24 11:58:07.288190 fastblocks-0.3.9/fastblocks/adapters/auth/__init__.py
--rw-r--r--   0        0        0     1977 2024-04-11 14:20:14.024549 fastblocks-0.3.9/fastblocks/adapters/auth/_base.py
--rw-r--r--   0        0        0        0 2024-01-24 11:37:07.550854 fastblocks-0.3.9/fastblocks/adapters/auth/basic.py
--rw-r--r--   0        0        0       62 2023-11-04 13:50:49.307356 fastblocks-0.3.9/fastblocks/adapters/fonts/__init__.py
--rw-r--r--   0        0        0      222 2024-02-05 00:13:09.776789 fastblocks-0.3.9/fastblocks/adapters/fonts/_base.py
--rw-r--r--   0        0        0     1230 2024-02-05 00:13:09.786522 fastblocks-0.3.9/fastblocks/adapters/fonts/google.py
--rw-r--r--   0        0        0        0 2023-09-24 01:35:41.606537 fastblocks-0.3.9/fastblocks/adapters/sitemap/__init__.py
--rw-r--r--   0        0        0      883 2024-01-19 21:08:44.846106 fastblocks-0.3.9/fastblocks/adapters/sitemap/sitemap.py
--rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 fastblocks-0.3.9/fastblocks/adapters/style/__init__.py
--rw-r--r--   0        0        0     3812 2024-03-09 09:26:05.815486 fastblocks-0.3.9/fastblocks/adapters/style/_base.py
--rw-r--r--   0        0        0      118 2024-03-09 09:10:00.894074 fastblocks-0.3.9/fastblocks/adapters/style/bulma.py
--rw-r--r--   0        0        0       66 2023-11-04 13:50:49.311428 fastblocks-0.3.9/fastblocks/adapters/templates/__init__.py
--rw-r--r--   0        0        0      332 2024-03-03 09:36:13.663071 fastblocks-0.3.9/fastblocks/adapters/templates/_base.py
--rw-r--r--   0        0        0      758 2023-10-13 23:22:41.140320 fastblocks-0.3.9/fastblocks/adapters/templates/_filters.py
--rw-r--r--   0        0        0    14759 2024-03-04 14:04:06.525893 fastblocks-0.3.9/fastblocks/adapters/templates/jinja2.py
--rw-r--r--   0        0        0     3593 2024-04-11 14:20:14.047979 fastblocks-0.3.9/fastblocks/applications.py
--rw-r--r--   0        0        0     3056 2024-03-04 14:52:11.154976 fastblocks-0.3.9/fastblocks/middleware.py
--rw-r--r--   0        0        0     3052 2024-04-11 14:55:14.493559 fastblocks-0.3.9/pyproject.toml
--rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 fastblocks-0.3.9/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 fastblocks-0.4.0/LICENSE
+-rw-r--r--   0        0        0     1024 2023-09-28 16:26:56.729322 fastblocks-0.4.0/README.md
+-rw-r--r--   0        0        0      256 2023-10-15 06:30:11.975198 fastblocks-0.4.0/fastblocks/Dockerfile
+-rw-r--r--   0        0        0       80 2024-04-11 14:21:21.798764 fastblocks-0.4.0/fastblocks/__init__.py
+-rw-r--r--   0        0        0      191 2024-01-19 13:43:05.790330 fastblocks-0.4.0/fastblocks/__main__.py
+-rw-r--r--   0        0        0       61 2024-01-16 17:26:09.440085 fastblocks-0.4.0/fastblocks/actions/__init__.py
+-rw-r--r--   0        0        0      407 2023-12-10 08:11:45.418815 fastblocks-0.4.0/fastblocks/actions/minify.py
+-rw-r--r--   0        0        0        0 2024-02-08 21:10:42.403063 fastblocks-0.4.0/fastblocks/adapters/__init__.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:50:49.302945 fastblocks-0.4.0/fastblocks/adapters/admin/__init__.py
+-rw-r--r--   0        0        0      211 2024-05-19 17:32:35.741801 fastblocks-0.4.0/fastblocks/adapters/admin/_base.py
+-rw-r--r--   0        0        0     1286 2024-05-19 17:26:14.359108 fastblocks-0.4.0/fastblocks/adapters/admin/sqladmin.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:49:17.900293 fastblocks-0.4.0/fastblocks/adapters/app/__init__.py
+-rw-r--r--   0        0        0      312 2024-02-24 10:37:18.246405 fastblocks-0.4.0/fastblocks/adapters/app/_base.py
+-rw-r--r--   0        0        0     2778 2024-05-19 17:20:16.124648 fastblocks-0.4.0/fastblocks/adapters/app/main.py
+-rw-r--r--   0        0        0       61 2024-01-24 11:58:07.288190 fastblocks-0.4.0/fastblocks/adapters/auth/__init__.py
+-rw-r--r--   0        0        0     2021 2024-04-15 14:56:18.634894 fastblocks-0.4.0/fastblocks/adapters/auth/_base.py
+-rw-r--r--   0        0        0        0 2024-01-24 11:37:07.550854 fastblocks-0.4.0/fastblocks/adapters/auth/basic.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:50:49.307356 fastblocks-0.4.0/fastblocks/adapters/fonts/__init__.py
+-rw-r--r--   0        0        0      272 2024-04-15 14:56:18.661746 fastblocks-0.4.0/fastblocks/adapters/fonts/_base.py
+-rw-r--r--   0        0        0     1230 2024-02-05 00:13:09.786522 fastblocks-0.4.0/fastblocks/adapters/fonts/google.py
+-rw-r--r--   0        0        0       63 2024-02-07 11:18:36.653787 fastblocks-0.4.0/fastblocks/adapters/routes/__init__.py
+-rw-r--r--   0        0        0      148 2024-02-07 21:14:30.088129 fastblocks-0.4.0/fastblocks/adapters/routes/_base.py
+-rw-r--r--   0        0        0     3447 2024-05-19 17:32:35.905030 fastblocks-0.4.0/fastblocks/adapters/routes/default.py
+-rw-r--r--   0        0        0        0 2023-09-24 01:35:41.606537 fastblocks-0.4.0/fastblocks/adapters/sitemap/__init__.py
+-rw-r--r--   0        0        0      150 2024-04-15 14:56:18.653833 fastblocks-0.4.0/fastblocks/adapters/sitemap/_base.py
+-rw-r--r--   0        0        0      883 2024-01-19 21:08:44.846106 fastblocks-0.4.0/fastblocks/adapters/sitemap/sitemap.py
+-rw-r--r--   0        0        0        0 2023-09-28 14:57:22.545553 fastblocks-0.4.0/fastblocks/adapters/style/__init__.py
+-rw-r--r--   0        0        0     3812 2024-03-09 09:26:05.815486 fastblocks-0.4.0/fastblocks/adapters/style/_base.py
+-rw-r--r--   0        0        0      118 2024-03-09 09:10:00.894074 fastblocks-0.4.0/fastblocks/adapters/style/bulma.py
+-rw-r--r--   0        0        0       66 2023-11-04 13:50:49.311428 fastblocks-0.4.0/fastblocks/adapters/templates/__init__.py
+-rw-r--r--   0        0        0      332 2024-03-03 09:36:13.663071 fastblocks-0.4.0/fastblocks/adapters/templates/_base.py
+-rw-r--r--   0        0        0      758 2023-10-13 23:22:41.140320 fastblocks-0.4.0/fastblocks/adapters/templates/_filters.py
+-rw-r--r--   0        0        0    14822 2024-04-11 21:18:24.305113 fastblocks-0.4.0/fastblocks/adapters/templates/jinja2.py
+-rw-r--r--   0        0        0     3593 2024-04-11 14:20:14.047979 fastblocks-0.4.0/fastblocks/applications.py
+-rw-r--r--   0        0        0     3056 2024-03-04 14:52:11.154976 fastblocks-0.4.0/fastblocks/middleware.py
+-rw-r--r--   0        0        0      301 2024-03-11 12:41:28.420083 fastblocks-0.4.0/fastblocks/templates/admin/bootstrap/blocks/display_menu.html
+-rw-r--r--   0        0        0     1127 2024-03-04 16:21:30.478801 fastblocks-0.4.0/fastblocks/templates/admin/bootstrap/blocks/menu_category.html
+-rw-r--r--   0        0        0      422 2024-03-04 16:21:30.466542 fastblocks-0.4.0/fastblocks/templates/admin/bootstrap/blocks/menu_item.html
+-rw-r--r--   0        0        0     1965 2024-04-15 14:32:35.783285 fastblocks-0.4.0/fastblocks/templates/admin/bootstrap/layout.html
+-rw-r--r--   0        0        0     3052 2024-05-19 17:35:23.713216 fastblocks-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 fastblocks-0.4.0/PKG-INFO
```

### Comparing `fastblocks-0.3.9/LICENSE` & `fastblocks-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.9/README.md` & `fastblocks-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.9/fastblocks/adapters/app/main.py` & `fastblocks-0.4.0/fastblocks/adapters/app/main.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,27 +1,25 @@
 import typing as t
 from contextlib import asynccontextmanager
 from time import perf_counter
 
 from acb.adapters import get_adapter
 from acb.adapters import import_adapter
 from acb.config import Config
-from acb.debug import debug
 from acb.depends import depends
-
 from fastblocks.applications import FastBlocks
 from ._base import AppBase
 from ._base import AppBaseSettings
 
 main_start = perf_counter()
 
 Logger = import_adapter()
 Cache = import_adapter()
-Sql = import_adapter()
 Auth = import_adapter()
+Models = import_adapter()
 
 
 class AppSettings(AppBaseSettings):
     url: str = "http://localhost:8000"
 
     @depends.inject
     def __init__(self, config: Config = depends(), **data: t.Any) -> None:
@@ -29,41 +27,45 @@
         self.url = self.url if not config.deployed else f"https://{self.domain}"
 
 
 class App(FastBlocks, AppBase):
     def __init__(self) -> None:
         super().__init__(lifespan=self.lifespan)
 
-    @depends.inject
     async def init(self) -> None:
         self.templates = depends.get(import_adapter("templates")).app
         self.routes.extend(depends.get(import_adapter("routes")).routes)
-        for route in self.routes:
-            debug(route)
 
     @asynccontextmanager
     @depends.inject
     async def lifespan(
         self,
         app: FastBlocks,
         cache: Cache = depends(),  # type: ignore
         auth: Auth = depends(),  # type: ignore
-        sql: Sql = depends(),  # type: ignore
     ) -> t.AsyncGenerator[None, None]:
+        if (
+            not self.config.deployed
+            and self.config.debug.cache
+            and not self.config.debug.production
+        ):
+            await cache.delete_match("*")
+
         if get_adapter("admin").enabled:
             admin = depends.get(import_adapter("admin"))
             admin.__init__(
                 app,
-                engine=sql.engine,
+                engine=depends.get(import_adapter("sql")).engine,
                 title=self.config.admin.title,
                 debug=self.config.debug.admin,
                 base_url=self.config.admin.url,
                 logo_url=self.config.admin.logo_url,
                 authentication_backend=auth,
             )
+            self.router.routes.insert(0, self.router.routes.pop())
 
         async def post_startup() -> None:
             if not self.config.deployed:
                 from aioconsole import aprint
                 from pyfiglet import Figlet
 
                 fig = Figlet(font="slant", width=90, justify="center")
@@ -73,12 +75,11 @@
 
         await post_startup()
         main_start_time = perf_counter() - main_start
         self.logger.info(f"App started in {main_start_time} s")
         yield
         await cache.close()
         self.logger.error("Application shut down")
-        self.logger.complete()
 
 
 depends.set(App)
 app = depends.get(App)
```

### Comparing `fastblocks-0.3.9/fastblocks/adapters/auth/_base.py` & `fastblocks-0.4.0/fastblocks/adapters/auth/_base.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 import typing as t
 from abc import ABC
 from abc import abstractmethod
 from contextvars import ContextVar
 
-from acb.config import AppSettings
+from acb.adapters import AdapterBase
+from acb.config import Settings
 from asgi_htmx import HtmxRequest
 from pydantic import EmailStr
 from pydantic import SecretStr
 from pydantic import UUID4
 from starlette.authentication import UnauthenticatedUser
 
 
-class AuthBaseSettings(AppSettings):
+class AuthBaseSettings(Settings):
     token_id: t.Optional[str] = None
     session_cookie: t.Optional[str] = None
 
 
-class AuthBase(ABC):
+class AuthBase(AdapterBase, ABC):
     _current_user: ContextVar[t.Any] = ContextVar(
         "current_user", default=UnauthenticatedUser()
     )
 
     @property
     def current_user(self) -> t.Any:
         return self._current_user.get()
```

### Comparing `fastblocks-0.3.9/fastblocks/adapters/fonts/google.py` & `fastblocks-0.4.0/fastblocks/adapters/fonts/google.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.9/fastblocks/adapters/sitemap/sitemap.py` & `fastblocks-0.4.0/fastblocks/adapters/sitemap/sitemap.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.9/fastblocks/adapters/style/_base.py` & `fastblocks-0.4.0/fastblocks/adapters/style/_base.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.9/fastblocks/adapters/templates/_filters.py` & `fastblocks-0.4.0/fastblocks/adapters/templates/_filters.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.9/fastblocks/adapters/templates/jinja2.py` & `fastblocks-0.4.0/fastblocks/adapters/templates/jinja2.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,14 +278,15 @@
         self.base = self.root / "base"
         self.style = self.root / config.app.style
         self.theme = self.style / config.app.theme
 
 
 class TemplatesSettings(TemplatesBaseSettings):
     loader: t.Optional[str] = None
+    cache_db: t.Optional[int] = 0
     extensions: list[str] = []
     delimiters: t.Optional[dict[str, str]] = dict(
         block_start_string="[%",
         block_end_string="%]",
         variable_start_string="[[",
         variable_end_string="]]",
         comment_start_string="[#",
@@ -341,15 +342,15 @@
                 ]
             )
         bytecode_cache = AsyncRedisBytecodeCache(
             prefix=self.config.app.name,
             password=self.config.cache.password.get_secret_value(),
             host=self.config.cache.host.get_secret_value(),
             port=self.config.cache.port,
-            db=0,
+            db=self.config.templates.cache_db,
         )
         env_configs = dict(extensions=_extensions, bytecode_cache=bytecode_cache)
         templates = AsyncJinja2Templates(template_paths.root, **env_configs)
         templates.env.loader = self.get_loader(
             template_paths, admin=admin
         ) or literal_eval(self.config.templates.loader)
         for ext in templates.env.extensions:
```

### Comparing `fastblocks-0.3.9/fastblocks/applications.py` & `fastblocks-0.4.0/fastblocks/applications.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.9/fastblocks/middleware.py` & `fastblocks-0.4.0/fastblocks/middleware.py`

 * *Files identical despite different names*

### Comparing `fastblocks-0.3.9/pyproject.toml` & `fastblocks-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "fastblocks"
-version = "0.3.9"
+version = "0.4.0"
 description = "Starlette based app for the rapid delivery HTMX/Jinja template blocks"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 maintainers = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
@@ -107,37 +107,37 @@
 
 [tool.creosote]
 paths = [
     "fastblocks",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
-    "pdm",
-    "autotyping",
+    "pre-commit",
     "pyfiglet",
-    "pdm-bump",
-    "phonenumbers",
     "libsass",
+    "phonenumbers",
+    "pdm-bump",
+    "pdm",
     "aiohttp",
+    "autotyping",
     "pytest",
-    "pre-commit",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "fastblocks",
 ]
 skips = [
-    "B603",
-    "B403",
     "B113",
     "B404",
+    "B403",
+    "B603",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "fastblocks",
 ]
```

### Comparing `fastblocks-0.3.9/PKG-INFO` & `fastblocks-0.4.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: fastblocks
-Version: 0.3.9
+Version: 0.4.0
 Summary: Starlette based app for the rapid delivery HTMX/Jinja template blocks
-Keywords: starlette htmx jinja httpx fastapi sqladmin sqlmodel pydantic sqlalchemy redis
+Keywords: starlette,htmx,jinja,httpx,fastapi,sqladmin,sqlmodel,pydantic,sqlalchemy,redis
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 Maintainer-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
```

