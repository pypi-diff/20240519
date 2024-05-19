# Comparing `tmp/fleekapi-0.1.23.tar.gz` & `tmp/fleekapi-0.1.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fleekapi-0.1.23.tar", last modified: Sun May 19 13:08:17 2024, max compression
+gzip compressed data, was "fleekapi-0.1.24.tar", last modified: Sun May 19 14:23:22 2024, max compression
```

## Comparing `fleekapi-0.1.23.tar` & `fleekapi-0.1.24.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 13:08:17.465890 fleekapi-0.1.23/
--rw-r--r--   0 hasan     (1002) hasan     (1002)     7724 2024-05-19 13:08:17.465890 fleekapi-0.1.23/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     6861 2024-05-19 12:22:45.000000 fleekapi-0.1.23/README.md
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 13:08:17.457890 fleekapi-0.1.23/fleekapi/
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       25 2024-05-19 13:07:08.000000 fleekapi-0.1.23/fleekapi/__init__.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3855 2024-05-19 07:09:46.000000 fleekapi-0.1.23/fleekapi/app.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      673 2024-05-18 17:00:00.000000 fleekapi-0.1.23/fleekapi/middleware.py
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      970 2024-05-19 07:00:05.000000 fleekapi-0.1.23/fleekapi/response.py
-drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 13:08:17.465890 fleekapi-0.1.23/fleekapi.egg-info/
--rw-r--r--   0 hasan     (1002) hasan     (1002)     7724 2024-05-19 13:08:17.000000 fleekapi-0.1.23/fleekapi.egg-info/PKG-INFO
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      258 2024-05-19 13:08:17.000000 fleekapi-0.1.23/fleekapi.egg-info/SOURCES.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-19 13:08:17.000000 fleekapi-0.1.23/fleekapi.egg-info/dependency_links.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)      122 2024-05-19 13:08:17.000000 fleekapi-0.1.23/fleekapi.egg-info/requires.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-19 13:08:17.000000 fleekapi-0.1.23/fleekapi.egg-info/top_level.txt
--rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-19 13:08:17.465890 fleekapi-0.1.23/setup.cfg
--rw-rw-r--   0 hasan     (1002) hasan     (1002)     3980 2024-05-19 13:08:12.000000 fleekapi-0.1.23/setup.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 14:23:22.078345 fleekapi-0.1.24/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     1085 2024-05-19 13:25:10.000000 fleekapi-0.1.24/LICENCE
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     7782 2024-05-19 14:23:22.074345 fleekapi-0.1.24/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     6866 2024-05-19 13:15:32.000000 fleekapi-0.1.24/README.md
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 14:23:22.070345 fleekapi-0.1.24/fleekapi/
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       26 2024-05-19 13:15:32.000000 fleekapi-0.1.24/fleekapi/__init__.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     3856 2024-05-19 13:15:32.000000 fleekapi-0.1.24/fleekapi/app.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      674 2024-05-19 13:15:32.000000 fleekapi-0.1.24/fleekapi/middleware.py
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      972 2024-05-19 13:15:32.000000 fleekapi-0.1.24/fleekapi/response.py
+drwxrwxr-x   0 hasan     (1002) hasan     (1002)        0 2024-05-19 14:23:22.074345 fleekapi-0.1.24/fleekapi.egg-info/
+-rw-r--r--   0 hasan     (1002) hasan     (1002)     7782 2024-05-19 14:23:21.000000 fleekapi-0.1.24/fleekapi.egg-info/PKG-INFO
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      266 2024-05-19 14:23:21.000000 fleekapi-0.1.24/fleekapi.egg-info/SOURCES.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        1 2024-05-19 14:23:21.000000 fleekapi-0.1.24/fleekapi.egg-info/dependency_links.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)      138 2024-05-19 14:23:21.000000 fleekapi-0.1.24/fleekapi.egg-info/requires.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)        9 2024-05-19 14:23:21.000000 fleekapi-0.1.24/fleekapi.egg-info/top_level.txt
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)       38 2024-05-19 14:23:22.078345 fleekapi-0.1.24/setup.cfg
+-rw-rw-r--   0 hasan     (1002) hasan     (1002)     4004 2024-05-19 14:23:03.000000 fleekapi-0.1.24/setup.py
```

### Comparing `fleekapi-0.1.23/PKG-INFO` & `fleekapi-0.1.24/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 Metadata-Version: 2.1
 Name: fleekapi
-Version: 0.1.23
+Version: 0.1.24
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/FleekAPI
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
+License-File: LICENCE
 Requires-Dist: gunicorn==22.0.0
 Requires-Dist: Jinja2==3.1.4
 Requires-Dist: parse==1.20.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-wsgi-adapter==0.4.1
 Requires-Dist: WebOb==1.8.7
 Requires-Dist: whitenoise==6.6.0
+Requires-Dist: icecream==2.1.3
 
 
 # FleekAPI
-![purpose](https://img.shields.io/badge/purpose-learning-green.svg)
 
+![purpose](https://img.shields.io/badge/purpose-learning-green.svg)
 
-FleekAPI is a Python Web Framework built for learning purposes. The plan is to learn how frameworks are built by implementing their features,
+FleekAPI is a Python Web Framework built for learning purposes. The plan is to learn how frameworks are built by
+implementing their features,
 writing blog posts about them and keeping the codebase as simple as possible.
 
 It is a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 
 ## Inspiration
 
-I was inspired to make a web framework after reading [Jakhongir Rakhmonov](https://t.me/jakhonrakhmonov)'s [blog post](https://t.me/jakhonrakhmonov/419)
-about how he built a web framework and became an open source maintainer. He wrote about how thrilling the experience has been for him so I decided I would give it a try as well.
-Thank you much, [Jakhongir](https://github.com/rahmonov). Go check out [Alcazar by Jakhongir Rakhmonov](https://github.com/rahmonov/alcazar).
+I was inspired to make a web framework after reading [Jakhongir Rakhmonov](https://t.me/jakhonrakhmonov)'
+s [blog post](https://t.me/jakhonrakhmonov/419)
+about how he built a web framework and became an open source maintainer. He wrote about how thrilling the experience has
+been for him so I decided I would give it a try as well.
+Thank you much, [Jakhongir](https://github.com/rahmonov). Go check
+out [Alcazar by Jakhongir Rakhmonov](https://github.com/rahmonov/alcazar).
 If you like him, show some love by staring his repos.
 
 ## Quick Start
 
 Install it:
 
 ```bash
@@ -106,91 +112,100 @@
 ```python
 @app.route("/{name:l}")
 class GreetingHandler:
     def get(self, req, resp, name):
         resp.text = f"Hello, {name}"
 ```
 
-This handler will only allow `GET` requests. That is, `POST` and others will be rejected. The same thing can be done with
+This handler will only allow `GET` requests. That is, `POST` and others will be rejected. The same thing can be done
+with
 function based handlers in the following way:
 
 ```python
 @app.route("/", allowed_methods=["get"])
 def home(req, resp):
     resp.text = "Hello, this is a home page."
 ```
 
 Note that if you specify `methods` for class based handlers, they will be ignored.
 
 ## Unit Tests
 
-The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in fixtures
-that you may want to use when writing unit tests with FleekAPI. The first one is `app` which is an instance of the main `FleekAPI` class:
+The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in
+fixtures
+that you may want to use when writing unit tests with FleekAPI. The first one is `app` which is an instance of the
+main `FleekAPI` class:
 
 ```python
 def test_route_overlap_throws_exception(app):
     @app.route("/")
     def home(req, resp):
         resp.text = "Welcome Home."
 
     with pytest.raises(AssertionError):
         @app.route("/")
         def home2(req, resp):
             resp.text = "Welcome Home2."
 ```
 
-The other one is `client` that you can use to send HTTP requests to your handlers. It is based on the famous [requests](http://docs.python-requests.org/en/master/) and it should feel very familiar:
+The other one is `client` that you can use to send HTTP requests to your handlers. It is based on the
+famous [requests](http://docs.python-requests.org/en/master/) and it should feel very familiar:
 
 ```python
 def test_parameterized_route(app, client):
     @app.route("/{name}")
     def hello(req, resp, name):
         resp.text = f"hey {name}"
 
     assert client.get(url("/matthew")).text == "hey matthew"
 ```
 
-Note that there is a `url()` function used. It is used to generate the absolute url of the request given a relative url. Import it before usage:
+Note that there is a `url()` function used. It is used to generate the absolute url of the request given a relative url.
+Import it before usage:
 
 ```python
 from fleekapi.utils.tests import url
 ```
 
 ## Templates
 
 [//]: # (The default folder for templates is `templates`. You can change it when initializing the main `FleekAPI&#40;&#41;` class:)
 
 [//]: # ()
+
 [//]: # (```python)
 
 [//]: # (app = FleekAPI&#40;templates_dir="templates_dir_name"&#41;)
 
 [//]: # (```)
 
 [//]: # ()
+
 [//]: # (Then you can use HTML files in that folder like so in a handler:)
 
 ```python
 @app.route("/show/template")
 def handler_with_template(req, resp):
     resp.html = app.template("example.html", context={"title": "Awesome Framework", "body": "welcome to the future!"})
 ```
 
 ## Static Files
 
 [//]: # (Just like templates, the default folder for static files is `static` and you can override it:)
 
 [//]: # ()
+
 [//]: # (```python)
 
 [//]: # (app = FleekAPI&#40;static_dir="static_dir_name"&#41;)
 
 [//]: # (```)
 
 [//]: # ()
+
 [//]: # (Then you can use the files inside this folder in HTML files:)
 
 ```html
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
@@ -205,15 +220,16 @@
     <p>This is a paragraph</p>
 </body>
 </html>
 ```
 
 ## Custom Exception Handler
 
-Sometimes, depending on the exception raised, you may want to do a certain action. For such cases, you can register an exception handler:
+Sometimes, depending on the exception raised, you may want to do a certain action. For such cases, you can register an
+exception handler:
 
 ```python
 def on_exception(req, resp, exception):
     if isinstance(exception, HTTPError):
         if exception.status == 404:
             resp.text = "Unfortunately the thing you were looking for was not found"
         else:
@@ -225,20 +241,23 @@
         else:
             print("These unexpected exceptions should be logged.")
 
 app = FleekAPI(debug=False)
 app.add_exception_handler(on_exception)
 ```
 
-This exception handler will catch 404 HTTPErrors and change the text to `"Unfortunately the thing you were looking for was not found"`. For other HTTPErrors, it will simply
-show the exception message. If the raised exception is not an HTTPError and if `debug` is set to True, it will show the exception and its traceback. Otherwise, it will log it.
+This exception handler will catch 404 HTTPErrors and change the text
+to `"Unfortunately the thing you were looking for was not found"`. For other HTTPErrors, it will simply
+show the exception message. If the raised exception is not an HTTPError and if `debug` is set to True, it will show the
+exception and its traceback. Otherwise, it will log it.
 
 ## Middleware
 
-You can create custom middleware classes by inheriting from the `fleekapi.middleware.Middleware` class and override its two methods
+You can create custom middleware classes by inheriting from the `fleekapi.middleware.Middleware` class and override its
+two methods
 that are called before and after each request:
 
 ```python
 from fleekapi import FleekAPI
 from fleekapi.middleware import Middleware
 
 app = FleekAPI()
@@ -264,9 +283,10 @@
 - Support for templates
 - Support for static files
 - Custom exception handler
 - Middleware
 
 ## Note
 
-It is extremely raw and will hopefully keep improving. If you are interested in knowing how a particular feature is implemented in other
+It is extremely raw and will hopefully keep improving. If you are interested in knowing how a particular feature is
+implemented in other
 frameworks, please open an issue and we will hopefully implement and explain it.
```

### Comparing `fleekapi-0.1.23/README.md` & `fleekapi-0.1.24/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 # FleekAPI
-![purpose](https://img.shields.io/badge/purpose-learning-green.svg)
 
+![purpose](https://img.shields.io/badge/purpose-learning-green.svg)
 
-FleekAPI is a Python Web Framework built for learning purposes. The plan is to learn how frameworks are built by implementing their features,
+FleekAPI is a Python Web Framework built for learning purposes. The plan is to learn how frameworks are built by
+implementing their features,
 writing blog posts about them and keeping the codebase as simple as possible.
 
 It is a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 
 ## Inspiration
 
-I was inspired to make a web framework after reading [Jakhongir Rakhmonov](https://t.me/jakhonrakhmonov)'s [blog post](https://t.me/jakhonrakhmonov/419)
-about how he built a web framework and became an open source maintainer. He wrote about how thrilling the experience has been for him so I decided I would give it a try as well.
-Thank you much, [Jakhongir](https://github.com/rahmonov). Go check out [Alcazar by Jakhongir Rakhmonov](https://github.com/rahmonov/alcazar).
+I was inspired to make a web framework after reading [Jakhongir Rakhmonov](https://t.me/jakhonrakhmonov)'
+s [blog post](https://t.me/jakhonrakhmonov/419)
+about how he built a web framework and became an open source maintainer. He wrote about how thrilling the experience has
+been for him so I decided I would give it a try as well.
+Thank you much, [Jakhongir](https://github.com/rahmonov). Go check
+out [Alcazar by Jakhongir Rakhmonov](https://github.com/rahmonov/alcazar).
 If you like him, show some love by staring his repos.
 
 ## Quick Start
 
 Install it:
 
 ```bash
@@ -81,91 +85,100 @@
 ```python
 @app.route("/{name:l}")
 class GreetingHandler:
     def get(self, req, resp, name):
         resp.text = f"Hello, {name}"
 ```
 
-This handler will only allow `GET` requests. That is, `POST` and others will be rejected. The same thing can be done with
+This handler will only allow `GET` requests. That is, `POST` and others will be rejected. The same thing can be done
+with
 function based handlers in the following way:
 
 ```python
 @app.route("/", allowed_methods=["get"])
 def home(req, resp):
     resp.text = "Hello, this is a home page."
 ```
 
 Note that if you specify `methods` for class based handlers, they will be ignored.
 
 ## Unit Tests
 
-The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in fixtures
-that you may want to use when writing unit tests with FleekAPI. The first one is `app` which is an instance of the main `FleekAPI` class:
+The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in
+fixtures
+that you may want to use when writing unit tests with FleekAPI. The first one is `app` which is an instance of the
+main `FleekAPI` class:
 
 ```python
 def test_route_overlap_throws_exception(app):
     @app.route("/")
     def home(req, resp):
         resp.text = "Welcome Home."
 
     with pytest.raises(AssertionError):
         @app.route("/")
         def home2(req, resp):
             resp.text = "Welcome Home2."
 ```
 
-The other one is `client` that you can use to send HTTP requests to your handlers. It is based on the famous [requests](http://docs.python-requests.org/en/master/) and it should feel very familiar:
+The other one is `client` that you can use to send HTTP requests to your handlers. It is based on the
+famous [requests](http://docs.python-requests.org/en/master/) and it should feel very familiar:
 
 ```python
 def test_parameterized_route(app, client):
     @app.route("/{name}")
     def hello(req, resp, name):
         resp.text = f"hey {name}"
 
     assert client.get(url("/matthew")).text == "hey matthew"
 ```
 
-Note that there is a `url()` function used. It is used to generate the absolute url of the request given a relative url. Import it before usage:
+Note that there is a `url()` function used. It is used to generate the absolute url of the request given a relative url.
+Import it before usage:
 
 ```python
 from fleekapi.utils.tests import url
 ```
 
 ## Templates
 
 [//]: # (The default folder for templates is `templates`. You can change it when initializing the main `FleekAPI&#40;&#41;` class:)
 
 [//]: # ()
+
 [//]: # (```python)
 
 [//]: # (app = FleekAPI&#40;templates_dir="templates_dir_name"&#41;)
 
 [//]: # (```)
 
 [//]: # ()
+
 [//]: # (Then you can use HTML files in that folder like so in a handler:)
 
 ```python
 @app.route("/show/template")
 def handler_with_template(req, resp):
     resp.html = app.template("example.html", context={"title": "Awesome Framework", "body": "welcome to the future!"})
 ```
 
 ## Static Files
 
 [//]: # (Just like templates, the default folder for static files is `static` and you can override it:)
 
 [//]: # ()
+
 [//]: # (```python)
 
 [//]: # (app = FleekAPI&#40;static_dir="static_dir_name"&#41;)
 
 [//]: # (```)
 
 [//]: # ()
+
 [//]: # (Then you can use the files inside this folder in HTML files:)
 
 ```html
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
@@ -180,15 +193,16 @@
     <p>This is a paragraph</p>
 </body>
 </html>
 ```
 
 ## Custom Exception Handler
 
-Sometimes, depending on the exception raised, you may want to do a certain action. For such cases, you can register an exception handler:
+Sometimes, depending on the exception raised, you may want to do a certain action. For such cases, you can register an
+exception handler:
 
 ```python
 def on_exception(req, resp, exception):
     if isinstance(exception, HTTPError):
         if exception.status == 404:
             resp.text = "Unfortunately the thing you were looking for was not found"
         else:
@@ -200,20 +214,23 @@
         else:
             print("These unexpected exceptions should be logged.")
 
 app = FleekAPI(debug=False)
 app.add_exception_handler(on_exception)
 ```
 
-This exception handler will catch 404 HTTPErrors and change the text to `"Unfortunately the thing you were looking for was not found"`. For other HTTPErrors, it will simply
-show the exception message. If the raised exception is not an HTTPError and if `debug` is set to True, it will show the exception and its traceback. Otherwise, it will log it.
+This exception handler will catch 404 HTTPErrors and change the text
+to `"Unfortunately the thing you were looking for was not found"`. For other HTTPErrors, it will simply
+show the exception message. If the raised exception is not an HTTPError and if `debug` is set to True, it will show the
+exception and its traceback. Otherwise, it will log it.
 
 ## Middleware
 
-You can create custom middleware classes by inheriting from the `fleekapi.middleware.Middleware` class and override its two methods
+You can create custom middleware classes by inheriting from the `fleekapi.middleware.Middleware` class and override its
+two methods
 that are called before and after each request:
 
 ```python
 from fleekapi import FleekAPI
 from fleekapi.middleware import Middleware
 
 app = FleekAPI()
@@ -239,9 +256,10 @@
 - Support for templates
 - Support for static files
 - Custom exception handler
 - Middleware
 
 ## Note
 
-It is extremely raw and will hopefully keep improving. If you are interested in knowing how a particular feature is implemented in other
+It is extremely raw and will hopefully keep improving. If you are interested in knowing how a particular feature is
+implemented in other
 frameworks, please open an issue and we will hopefully implement and explain it.
```

### Comparing `fleekapi-0.1.23/fleekapi/app.py` & `fleekapi-0.1.24/fleekapi/app.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -116,8 +116,8 @@
         template = self.template_env.get_template(template_name).render(**context)
         return template
 
     def add_exception_handler(self, exception_handler):
         self.exception_handler = exception_handler
 
     def add_middleware(self, middleware_cls):
-        self.middleware.add(middleware_cls)
+        self.middleware.add(middleware_cls)
```

### Comparing `fleekapi-0.1.23/fleekapi/middleware.py` & `fleekapi-0.1.24/fleekapi/middleware.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -19,8 +19,8 @@
         response = self.app.handle_request(request)
         self.process_response(request, response)
         return response
 
     def __call__(self, environ, start_response):
         request = Request(environ)
         response = self.app.handle_request(request)
-        return response(environ, start_response)
+        return response(environ, start_response)
```

### Comparing `fleekapi-0.1.23/fleekapi/response.py` & `fleekapi-0.1.24/fleekapi/response.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 
 from webob import Response as WebResponse
 
+
 class Response:
     def __init__(self):
         self.json = None
         self.html = None
         self.text = None
         self.content_type = None
         self.body = b''
@@ -26,8 +27,8 @@
         self.set_body_and_content_type()
 
         response = WebResponse(
             body=self.body,
             content_type=self.content_type,
             status=self.status_code,
         )
-        return response(environ, start_response)
+        return response(environ, start_response)
```

### Comparing `fleekapi-0.1.23/fleekapi.egg-info/PKG-INFO` & `fleekapi-0.1.24/fleekapi.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,46 +1,52 @@
 Metadata-Version: 2.1
 Name: fleekapi
-Version: 0.1.23
+Version: 0.1.24
 Summary: My short description for my project.
 Home-page: https://github.com/under-script/FleekAPI
 Author: Yunusov Abdulmajid
 Author-email: abdulmajidyunusov18@gmail.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.9.0
 Description-Content-Type: text/markdown
+License-File: LICENCE
 Requires-Dist: gunicorn==22.0.0
 Requires-Dist: Jinja2==3.1.4
 Requires-Dist: parse==1.20.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: requests-wsgi-adapter==0.4.1
 Requires-Dist: WebOb==1.8.7
 Requires-Dist: whitenoise==6.6.0
+Requires-Dist: icecream==2.1.3
 
 
 # FleekAPI
-![purpose](https://img.shields.io/badge/purpose-learning-green.svg)
 
+![purpose](https://img.shields.io/badge/purpose-learning-green.svg)
 
-FleekAPI is a Python Web Framework built for learning purposes. The plan is to learn how frameworks are built by implementing their features,
+FleekAPI is a Python Web Framework built for learning purposes. The plan is to learn how frameworks are built by
+implementing their features,
 writing blog posts about them and keeping the codebase as simple as possible.
 
 It is a WSGI framework and can be used with any WSGI application server such as Gunicorn.
 
 ## Inspiration
 
-I was inspired to make a web framework after reading [Jakhongir Rakhmonov](https://t.me/jakhonrakhmonov)'s [blog post](https://t.me/jakhonrakhmonov/419)
-about how he built a web framework and became an open source maintainer. He wrote about how thrilling the experience has been for him so I decided I would give it a try as well.
-Thank you much, [Jakhongir](https://github.com/rahmonov). Go check out [Alcazar by Jakhongir Rakhmonov](https://github.com/rahmonov/alcazar).
+I was inspired to make a web framework after reading [Jakhongir Rakhmonov](https://t.me/jakhonrakhmonov)'
+s [blog post](https://t.me/jakhonrakhmonov/419)
+about how he built a web framework and became an open source maintainer. He wrote about how thrilling the experience has
+been for him so I decided I would give it a try as well.
+Thank you much, [Jakhongir](https://github.com/rahmonov). Go check
+out [Alcazar by Jakhongir Rakhmonov](https://github.com/rahmonov/alcazar).
 If you like him, show some love by staring his repos.
 
 ## Quick Start
 
 Install it:
 
 ```bash
@@ -106,91 +112,100 @@
 ```python
 @app.route("/{name:l}")
 class GreetingHandler:
     def get(self, req, resp, name):
         resp.text = f"Hello, {name}"
 ```
 
-This handler will only allow `GET` requests. That is, `POST` and others will be rejected. The same thing can be done with
+This handler will only allow `GET` requests. That is, `POST` and others will be rejected. The same thing can be done
+with
 function based handlers in the following way:
 
 ```python
 @app.route("/", allowed_methods=["get"])
 def home(req, resp):
     resp.text = "Hello, this is a home page."
 ```
 
 Note that if you specify `methods` for class based handlers, they will be ignored.
 
 ## Unit Tests
 
-The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in fixtures
-that you may want to use when writing unit tests with FleekAPI. The first one is `app` which is an instance of the main `FleekAPI` class:
+The recommended way of writing unit tests is with [pytest](https://docs.pytest.org/en/latest/). There are two built in
+fixtures
+that you may want to use when writing unit tests with FleekAPI. The first one is `app` which is an instance of the
+main `FleekAPI` class:
 
 ```python
 def test_route_overlap_throws_exception(app):
     @app.route("/")
     def home(req, resp):
         resp.text = "Welcome Home."
 
     with pytest.raises(AssertionError):
         @app.route("/")
         def home2(req, resp):
             resp.text = "Welcome Home2."
 ```
 
-The other one is `client` that you can use to send HTTP requests to your handlers. It is based on the famous [requests](http://docs.python-requests.org/en/master/) and it should feel very familiar:
+The other one is `client` that you can use to send HTTP requests to your handlers. It is based on the
+famous [requests](http://docs.python-requests.org/en/master/) and it should feel very familiar:
 
 ```python
 def test_parameterized_route(app, client):
     @app.route("/{name}")
     def hello(req, resp, name):
         resp.text = f"hey {name}"
 
     assert client.get(url("/matthew")).text == "hey matthew"
 ```
 
-Note that there is a `url()` function used. It is used to generate the absolute url of the request given a relative url. Import it before usage:
+Note that there is a `url()` function used. It is used to generate the absolute url of the request given a relative url.
+Import it before usage:
 
 ```python
 from fleekapi.utils.tests import url
 ```
 
 ## Templates
 
 [//]: # (The default folder for templates is `templates`. You can change it when initializing the main `FleekAPI&#40;&#41;` class:)
 
 [//]: # ()
+
 [//]: # (```python)
 
 [//]: # (app = FleekAPI&#40;templates_dir="templates_dir_name"&#41;)
 
 [//]: # (```)
 
 [//]: # ()
+
 [//]: # (Then you can use HTML files in that folder like so in a handler:)
 
 ```python
 @app.route("/show/template")
 def handler_with_template(req, resp):
     resp.html = app.template("example.html", context={"title": "Awesome Framework", "body": "welcome to the future!"})
 ```
 
 ## Static Files
 
 [//]: # (Just like templates, the default folder for static files is `static` and you can override it:)
 
 [//]: # ()
+
 [//]: # (```python)
 
 [//]: # (app = FleekAPI&#40;static_dir="static_dir_name"&#41;)
 
 [//]: # (```)
 
 [//]: # ()
+
 [//]: # (Then you can use the files inside this folder in HTML files:)
 
 ```html
 <!DOCTYPE html>
 <html lang="en">
 
 <head>
@@ -205,15 +220,16 @@
     <p>This is a paragraph</p>
 </body>
 </html>
 ```
 
 ## Custom Exception Handler
 
-Sometimes, depending on the exception raised, you may want to do a certain action. For such cases, you can register an exception handler:
+Sometimes, depending on the exception raised, you may want to do a certain action. For such cases, you can register an
+exception handler:
 
 ```python
 def on_exception(req, resp, exception):
     if isinstance(exception, HTTPError):
         if exception.status == 404:
             resp.text = "Unfortunately the thing you were looking for was not found"
         else:
@@ -225,20 +241,23 @@
         else:
             print("These unexpected exceptions should be logged.")
 
 app = FleekAPI(debug=False)
 app.add_exception_handler(on_exception)
 ```
 
-This exception handler will catch 404 HTTPErrors and change the text to `"Unfortunately the thing you were looking for was not found"`. For other HTTPErrors, it will simply
-show the exception message. If the raised exception is not an HTTPError and if `debug` is set to True, it will show the exception and its traceback. Otherwise, it will log it.
+This exception handler will catch 404 HTTPErrors and change the text
+to `"Unfortunately the thing you were looking for was not found"`. For other HTTPErrors, it will simply
+show the exception message. If the raised exception is not an HTTPError and if `debug` is set to True, it will show the
+exception and its traceback. Otherwise, it will log it.
 
 ## Middleware
 
-You can create custom middleware classes by inheriting from the `fleekapi.middleware.Middleware` class and override its two methods
+You can create custom middleware classes by inheriting from the `fleekapi.middleware.Middleware` class and override its
+two methods
 that are called before and after each request:
 
 ```python
 from fleekapi import FleekAPI
 from fleekapi.middleware import Middleware
 
 app = FleekAPI()
@@ -264,9 +283,10 @@
 - Support for templates
 - Support for static files
 - Custom exception handler
 - Middleware
 
 ## Note
 
-It is extremely raw and will hopefully keep improving. If you are interested in knowing how a particular feature is implemented in other
+It is extremely raw and will hopefully keep improving. If you are interested in knowing how a particular feature is
+implemented in other
 frameworks, please open an issue and we will hopefully implement and explain it.
```

### Comparing `fleekapi-0.1.23/setup.py` & `fleekapi-0.1.24/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,26 +14,27 @@
 # Package meta-data.
 NAME = 'fleekapi'
 DESCRIPTION = 'My short description for my project.'
 URL = 'https://github.com/under-script/FleekAPI'
 EMAIL = 'abdulmajidyunusov18@gmail.com'
 AUTHOR = 'Yunusov Abdulmajid'
 REQUIRES_PYTHON = '>=3.9.0'
-VERSION = '0.1.23'
+VERSION = '0.1.24'
 
 # What packages are required for this module to be executed?
 REQUIRED = [
     # 'requests', 'maya', 'records',
     "gunicorn==22.0.0",
     "Jinja2==3.1.4",
     "parse==1.20.1",
     "requests==2.31.0",
     "requests-wsgi-adapter==0.4.1",
     "WebOb==1.8.7",
     "whitenoise==6.6.0",
+    "icecream==2.1.3",
 ]
 
 # What packages are optional?
 EXTRAS = {
     # 'fancy feature': ['django'],
 }
 
@@ -131,8 +132,8 @@
         'Programming Language :: Python :: Implementation :: CPython',
         'Programming Language :: Python :: Implementation :: PyPy'
     ],
     # $ setup.py publish support.
     cmdclass={
         'upload': UploadCommand,
     },
-)
+)
```

