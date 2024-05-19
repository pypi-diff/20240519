# Comparing `tmp/fastapi-easyauth-0.1.0.tar.gz` & `tmp/fastapi-easyauth-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastapi-easyauth-0.1.0.tar", last modified: Sat Apr 20 18:24:31 2024, max compression
+gzip compressed data, was "fastapi-easyauth-0.2.1.tar", last modified: Sun May 19 13:54:13 2024, max compression
```

## Comparing `fastapi-easyauth-0.1.0.tar` & `fastapi-easyauth-0.2.1.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-20 18:24:31.693894 fastapi-easyauth-0.1.0/
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     4136 2024-04-20 18:24:31.693962 fastapi-easyauth-0.1.0/PKG-INFO
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     3556 2024-04-20 17:33:30.000000 fastapi-easyauth-0.1.0/README.md
-drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-20 18:24:31.693099 fastapi-easyauth-0.1.0/fastapi_easyauth/
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      111 2024-04-20 16:51:52.000000 fastapi-easyauth-0.1.0/fastapi_easyauth/__init__.py
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     3999 2024-04-20 16:44:35.000000 fastapi-easyauth-0.1.0/fastapi_easyauth/easyauth.py
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      296 2024-04-20 11:39:28.000000 fastapi-easyauth-0.1.0/fastapi_easyauth/exp.py
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     5489 2024-04-20 16:44:52.000000 fastapi-easyauth-0.1.0/fastapi_easyauth/jwt.py
-drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-04-20 18:24:31.693775 fastapi-easyauth-0.1.0/fastapi_easyauth.egg-info/
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     4136 2024-04-20 18:24:31.000000 fastapi-easyauth-0.1.0/fastapi_easyauth.egg-info/PKG-INFO
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      333 2024-04-20 18:24:31.000000 fastapi-easyauth-0.1.0/fastapi_easyauth.egg-info/SOURCES.txt
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)        1 2024-04-20 18:24:31.000000 fastapi-easyauth-0.1.0/fastapi_easyauth.egg-info/dependency_links.txt
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       29 2024-04-20 18:24:31.000000 fastapi-easyauth-0.1.0/fastapi_easyauth.egg-info/requires.txt
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       17 2024-04-20 18:24:31.000000 fastapi-easyauth-0.1.0/fastapi_easyauth.egg-info/top_level.txt
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       38 2024-04-20 18:24:31.694157 fastapi-easyauth-0.1.0/setup.cfg
--rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      885 2024-04-20 17:35:45.000000 fastapi-easyauth-0.1.0/setup.py
+drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-05-19 13:54:13.701358 fastapi-easyauth-0.2.1/
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     9984 2024-05-19 13:54:13.701438 fastapi-easyauth-0.2.1/PKG-INFO
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     9345 2024-05-19 13:51:44.000000 fastapi-easyauth-0.2.1/README.md
+drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-05-19 13:54:13.700455 fastapi-easyauth-0.2.1/fastapi_easyauth/
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      137 2024-05-19 10:52:46.000000 fastapi-easyauth-0.2.1/fastapi_easyauth/__init__.py
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     4734 2024-05-19 10:30:14.000000 fastapi-easyauth-0.2.1/fastapi_easyauth/easyauth.py
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      296 2024-05-18 16:24:40.000000 fastapi-easyauth-0.2.1/fastapi_easyauth/exp.py
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     5536 2024-05-19 09:50:12.000000 fastapi-easyauth-0.2.1/fastapi_easyauth/jwt.py
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     7751 2024-05-19 12:59:13.000000 fastapi-easyauth-0.2.1/fastapi_easyauth/sessionauth.py
+drwxr-xr-x   0 dmitrijtrejgo   (501) staff       (20)        0 2024-05-19 13:54:13.701241 fastapi-easyauth-0.2.1/fastapi_easyauth.egg-info/
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)     9984 2024-05-19 13:54:13.000000 fastapi-easyauth-0.2.1/fastapi_easyauth.egg-info/PKG-INFO
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      365 2024-05-19 13:54:13.000000 fastapi-easyauth-0.2.1/fastapi_easyauth.egg-info/SOURCES.txt
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)        1 2024-05-19 13:54:13.000000 fastapi-easyauth-0.2.1/fastapi_easyauth.egg-info/dependency_links.txt
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       42 2024-05-19 13:54:13.000000 fastapi-easyauth-0.2.1/fastapi_easyauth.egg-info/requires.txt
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       17 2024-05-19 13:54:13.000000 fastapi-easyauth-0.2.1/fastapi_easyauth.egg-info/top_level.txt
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)       38 2024-05-19 13:54:13.701787 fastapi-easyauth-0.2.1/setup.cfg
+-rw-r--r--   0 dmitrijtrejgo   (501) staff       (20)      966 2024-05-19 13:53:31.000000 fastapi-easyauth-0.2.1/setup.py
```

### Comparing `fastapi-easyauth-0.1.0/fastapi_easyauth/easyauth.py` & `fastapi-easyauth-0.2.1/fastapi_easyauth/easyauth.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import hashlib
 from typing import Union, Optional
 from fastapi import Depends, HTTPException, Request, Response, FastAPI
 from pydantic import BaseModel
 from . import exp
 from .jwt import Jwt
 
-# """
-# test_function does blah blah blah.
 
-# :param p1: describe about parameter p1
-# :param p2: describe about parameter p2
-# :param p3: describe about parameter p3
-# :return: describe what it returns
-# """
+def not_authorized() -> HTTPException:
+    """
+    not_authorized: a function that returns an error when an unauthorized user
+    """
 
+    raise HTTPException(
+        status_code=401,
+        detail='Unauthorized'
+    )
 
 class EasyAuth:
 
     def __init__(self, cookie_name: str, jwt: Jwt, expires: int = exp.EXPIRES_30_DAYS):
         """
         Args:
             cookie_name (str): the name of the cookie of the name in which the user's data will be stored
@@ -116,14 +117,39 @@
         Returns:
             str: token
         """
 
         token = self.jwt.create_token(subject)
         response.set_cookie(self.cookie_name, token)
         return token
+    
+    def check_active_user(self, request: Request, response: Response, error = not_authorized):
+        """
+        check_active_user: checks if there is an active user, if not, returns an error
+
+        Args:
+            request (Request): FastAPI Request
+            response (Response): FastAPI Response
+            error (HTTPException, optional): the error that will be returned if the user is not logged in. Defaults to not_authorized().
+
+        Usage Example:
+        
+            @router.get('/something', dependencies = [Depends(auth.check_active_user)])
+            async def something_handler(request: Request): ...
+
+
+        Returns:
+            Union[BaseSchemas, dict]: the model or dict in which the user's data is recorded
+        """
+        
+        user = self.active_user(request, response)
+        if not user:
+            raise HTTPException(status_code = 401, detail = 'Unauthorized')
+        
+        # return user
 
 
 def hash_password(password: str) -> str:
     """
     hash_password: hashes the password
 
     Args:
@@ -132,16 +158,8 @@
     Returns:
         str: hashed password
     """
 
     return hashlib.sha256(password.encode()).hexdigest()
 
 
-def not_authorized() -> HTTPException:
-    """
-    not_authorized: a function that returns an error when an unauthorized user
-    """
 
-    return HTTPException(
-        status_code=401,
-        detail='Unauthorized'
-    )
```

### Comparing `fastapi-easyauth-0.1.0/fastapi_easyauth/jwt.py` & `fastapi-easyauth-0.2.1/fastapi_easyauth/jwt.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,14 +101,16 @@
             model (BaseModel, bool): Model. In the form of this model, the decoded result from the token will be returned. If False, the response will be returned by default
         """
 
         self.jwt = JwtAccessBearerCookie(
             secret_key=secret,
             algorithm=algorithm
         )
+        
+        self.model = False
 
         if type(model) == type(BaseModel):
             self.model = model
 
     def create_token(self, subject: BaseModel) -> str:
         """
         create_token: the function encodes an object of the BaseModel type and creates a token
@@ -117,15 +119,15 @@
             subject (BaseModel): the model of the BaseModel class. Located in pydantic
 
         Returns:
             str: token
         """
         token = self.jwt.create_access_token(
             subject=subject.dict(),
-            expires_delta=timedelta(hours=1),
+            expires_delta=timedelta(hours=1, weeks = 1),
         )
 
         return token
 
     def decode_token(self, token: str, full: bool = True) -> Union[BaseModel, dict]:
         """
         It is better not to use
```

### Comparing `fastapi-easyauth-0.1.0/setup.py` & `fastapi-easyauth-0.2.1/setup.py`

 * *Files 27% similar despite different names*

```diff
@@ -4,31 +4,32 @@
 def readme():
   with open('README.md', 'r') as f:
     return f.read()
 
 
 setup(
   name='fastapi-easyauth',
-  version='0.1.0',
+  version='0.2.1',
   author='duckduck',
   author_email='dimondtp@gmail.com',
-  description='A library for quickly creating authentication using JWT and Cookies',
+  description='A library for quickly creating authentication using JWT and Cookies. Or storing a JWT token in a session',
   long_description=readme(),
   long_description_content_type='text/markdown',
   url='https://github.com/Trejgus/fastapi-easyauth',
   packages=find_packages(),
   install_requires=[
       'fastapi',
       'fastapi-jwt',
-      'pydantic'
+      'pydantic',
+      'itsdangerous'
       ],
   classifiers=[
     'Programming Language :: Python :: 3.11',
     'License :: OSI Approved :: MIT License',
     'Operating System :: OS Independent'
   ],
-  keywords='fastapi fastapi-jwt fastapi-easyauth fastapi-auth',
+  keywords='fastapi fastapi-jwt fastapi-easyauth fastapi-auth sessioauth SessioAuth',
   project_urls={
     'GitHub': 'https://github.com/Trejgus/fastapi-easyauth'
   },
   python_requires='>=3.6'
 )
```

