# Comparing `tmp/clerk_django-1.0.2.tar.gz` & `tmp/clerk_django-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clerk_django-1.0.2.tar", last modified: Sat May 11 09:53:41 2024, max compression
+gzip compressed data, was "clerk_django-1.0.3.tar", last modified: Sun May 19 17:22:00 2024, max compression
```

## Comparing `clerk_django-1.0.2.tar` & `clerk_django-1.0.3.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2024-05-11 09:53:41.906357 clerk_django-1.0.2/
--rw-rw-rw-   0        0        0     1083 2024-05-11 08:24:33.000000 clerk_django-1.0.2/LICENSE
--rw-rw-rw-   0        0        0     1708 2024-05-11 09:53:41.905358 clerk_django-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0        0 2024-05-11 08:00:01.000000 clerk_django-1.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-11 09:53:41.867358 clerk_django-1.0.2/clerk_django/
--rw-rw-rw-   0        0        0        0 2024-04-26 11:18:38.000000 clerk_django-1.0.2/clerk_django/__init__.py
--rw-rw-rw-   0        0        0     2183 2024-05-11 09:28:06.000000 clerk_django-1.0.2/clerk_django/client.py
-drwxrwxrwx   0        0        0        0 2024-05-11 09:53:41.888359 clerk_django-1.0.2/clerk_django/middlewares/
--rw-rw-rw-   0        0        0        0 2024-04-25 21:50:04.000000 clerk_django-1.0.2/clerk_django/middlewares/__init__.py
--rw-rw-rw-   0        0        0     2034 2024-05-11 09:32:38.000000 clerk_django-1.0.2/clerk_django/middlewares/clerk.py
-drwxrwxrwx   0        0        0        0 2024-05-11 09:53:41.893356 clerk_django-1.0.2/clerk_django/permissions/
--rw-rw-rw-   0        0        0        0 2024-05-04 07:24:02.000000 clerk_django-1.0.2/clerk_django/permissions/__init__.py
--rw-rw-rw-   0        0        0      277 2024-04-26 07:06:29.000000 clerk_django-1.0.2/clerk_django/permissions/clerk.py
-drwxrwxrwx   0        0        0        0 2024-05-11 09:53:41.903356 clerk_django-1.0.2/clerk_django/resources/
--rw-rw-rw-   0        0        0       60 2024-04-26 12:14:18.000000 clerk_django-1.0.2/clerk_django/resources/__init__.py
--rw-rw-rw-   0        0        0     1963 2024-04-26 17:21:03.000000 clerk_django-1.0.2/clerk_django/resources/user.py
-drwxrwxrwx   0        0        0        0 2024-05-11 09:53:41.904358 clerk_django-1.0.2/clerk_django.egg-info/
--rw-rw-rw-   0        0        0     1708 2024-05-11 09:53:41.000000 clerk_django-1.0.2/clerk_django.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      467 2024-05-11 09:53:41.000000 clerk_django-1.0.2/clerk_django.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-11 09:53:41.000000 clerk_django-1.0.2/clerk_django.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-11 09:53:41.000000 clerk_django-1.0.2/clerk_django.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2024-05-11 09:53:41.000000 clerk_django-1.0.2/clerk_django.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      675 2024-05-11 09:53:27.000000 clerk_django-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-11 09:53:41.906357 clerk_django-1.0.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-19 17:22:00.610461 clerk_django-1.0.3/
+-rw-rw-rw-   0        0        0     1083 2024-05-11 08:24:33.000000 clerk_django-1.0.3/LICENSE
+-rw-rw-rw-   0        0        0     4983 2024-05-19 17:22:00.609462 clerk_django-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3188 2024-05-19 17:16:38.000000 clerk_django-1.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-19 17:22:00.591463 clerk_django-1.0.3/clerk_django/
+-rw-rw-rw-   0        0        0        0 2024-04-26 11:18:38.000000 clerk_django-1.0.3/clerk_django/__init__.py
+-rw-rw-rw-   0        0        0     2183 2024-05-11 10:08:36.000000 clerk_django-1.0.3/clerk_django/client.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:22:00.605461 clerk_django-1.0.3/clerk_django/middlewares/
+-rw-rw-rw-   0        0        0        0 2024-04-25 21:50:04.000000 clerk_django-1.0.3/clerk_django/middlewares/__init__.py
+-rw-rw-rw-   0        0        0     2034 2024-05-11 09:32:38.000000 clerk_django-1.0.3/clerk_django/middlewares/clerk.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:22:00.607462 clerk_django-1.0.3/clerk_django/permissions/
+-rw-rw-rw-   0        0        0        0 2024-05-04 07:24:02.000000 clerk_django-1.0.3/clerk_django/permissions/__init__.py
+-rw-rw-rw-   0        0        0      277 2024-04-26 07:06:29.000000 clerk_django-1.0.3/clerk_django/permissions/clerk.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:22:00.608461 clerk_django-1.0.3/clerk_django/resources/
+-rw-rw-rw-   0        0        0       60 2024-04-26 12:14:18.000000 clerk_django-1.0.3/clerk_django/resources/__init__.py
+-rw-rw-rw-   0        0        0     1977 2024-05-19 17:05:08.000000 clerk_django-1.0.3/clerk_django/resources/user.py
+drwxrwxrwx   0        0        0        0 2024-05-19 17:22:00.608461 clerk_django-1.0.3/clerk_django.egg-info/
+-rw-rw-rw-   0        0        0     4983 2024-05-19 17:22:00.000000 clerk_django-1.0.3/clerk_django.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      467 2024-05-19 17:22:00.000000 clerk_django-1.0.3/clerk_django.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-19 17:22:00.000000 clerk_django-1.0.3/clerk_django.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-19 17:22:00.000000 clerk_django-1.0.3/clerk_django.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2024-05-19 17:22:00.000000 clerk_django-1.0.3/clerk_django.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      777 2024-05-19 17:21:44.000000 clerk_django-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-19 17:22:00.610461 clerk_django-1.0.3/setup.cfg
```

### Comparing `clerk_django-1.0.2/LICENSE` & `clerk_django-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `clerk_django-1.0.2/clerk_django/client.py` & `clerk_django-1.0.3/clerk_django/client.py`

 * *Files identical despite different names*

### Comparing `clerk_django-1.0.2/clerk_django/middlewares/clerk.py` & `clerk_django-1.0.3/clerk_django/middlewares/clerk.py`

 * *Files identical despite different names*

### Comparing `clerk_django-1.0.2/clerk_django/resources/user.py` & `clerk_django-1.0.3/clerk_django/resources/user.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,36 +16,36 @@
     
     def getOrganizationMembershipList(self, user_id, params={}):
         return self._client.get(f'{self.base_url}/{user_id}/organization_memberships', params=params)
     
     def getUserOauthAccessToken(self, user_id, provider):
         return self._client.get(f'{self.base_url}/{user_id}/oauth_access_tokens/{provider}')
     
-    def createUser(self, data={}):
-        return self._client.post(f'{self.base_url}', data=data)
+    def createUser(self, params={}):
+        return self._client.post(f'{self.base_url}', data=params)
     
     def verifyPassword(self, user_id, password):
         return self._client.post(f'{self.base_url}/{user_id}/verify_password', data={"password":password})
     
     def banUser(self, user_id):
         return self._client.post(f'{self.base_url}/{user_id}/ban')
     
     def unbanUser(self, user_id):
         return self._client.post(f'{self.base_url}/{user_id}/unban')
     
     def lockUser(self, user_id):
         return self._client.post(f'{self.base_url}/{user_id}/lock')
     
-    def lockUser(self, user_id):
+    def unlockUser(self, user_id):
         return self._client.post(f'{self.base_url}/{user_id}/unlock')
     
-    def updateUser(self, data={}):
-        return self._client.patch(f'{self.base_url}', data=data)
+    def updateUser(self, params={}):
+        return self._client.patch(f'{self.base_url}', data=params)
     
-    def updateUserMetadata(self,user_id, data={}):
-        return self._client.patch(f'{self.base_url}/{user_id}/metadata', data=data)
+    def updateUserMetadata(self,user_id, params={}):
+        return self._client.patch(f'{self.base_url}/{user_id}/metadata', data=params)
     
     def deleteUser(self, user_id):
         return self._client.delete(f'{self.base_url}/{user_id}')
     
     def disableUserMFA(self, user_id):
         return self._client.delete(f'{self.base_url}/{user_id}/mfa')
```

