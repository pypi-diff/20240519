# Comparing `tmp/acb-0.5.9.tar.gz` & `tmp/acb-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "acb-0.5.9.tar", last modified: Sat Mar  9 15:07:54 2024, max compression
+gzip compressed data, was "acb-0.6.0.tar", last modified: Sun May 19 15:51:54 2024, max compression
```

## Comparing `acb-0.5.9.tar` & `acb-0.6.0.tar`

### file list

```diff
@@ -1,63 +1,66 @@
--rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 acb-0.5.9/LICENSE
--rw-r--r--   0        0        0      877 2024-02-25 15:01:48.403334 acb-0.5.9/README.md
--rw-r--r--   0        0        0      880 2024-02-09 10:50:18.605994 acb-0.5.9/acb/__init__.py
--rw-r--r--   0        0        0      819 2024-01-16 17:26:09.434218 acb-0.5.9/acb/actions/__init__.py
--rw-r--r--   0        0        0     1180 2023-10-09 11:44:35.662080 acb-0.5.9/acb/actions/compress.py
--rw-r--r--   0        0        0     4765 2023-12-09 09:30:31.322361 acb-0.5.9/acb/actions/encode.py
--rw-r--r--   0        0        0      897 2023-10-11 15:39:52.116219 acb-0.5.9/acb/actions/hash.py
--rw-r--r--   0        0        0     5580 2024-02-09 17:39:47.412433 acb-0.5.9/acb/adapters/__init__.py
--rw-r--r--   0        0        0       60 2023-11-04 13:17:17.290924 acb-0.5.9/acb/adapters/app/__init__.py
--rw-r--r--   0        0        0      242 2024-02-09 17:35:46.026715 acb-0.5.9/acb/adapters/app/_base.py
--rw-r--r--   0        0        0     1286 2024-02-09 17:35:46.099339 acb-0.5.9/acb/adapters/app/main.py
--rw-r--r--   0        0        0       62 2023-11-04 13:17:17.342044 acb-0.5.9/acb/adapters/cache/__init__.py
--rw-r--r--   0        0        0     1610 2024-03-02 10:09:36.352462 acb-0.5.9/acb/adapters/cache/_base.py
--rw-r--r--   0        0        0      828 2024-02-04 19:59:42.029846 acb-0.5.9/acb/adapters/cache/memory.py
--rw-r--r--   0        0        0     1635 2024-02-09 18:00:21.800300 acb-0.5.9/acb/adapters/cache/redis.py
--rw-r--r--   0        0        0       60 2023-11-04 13:17:17.324879 acb-0.5.9/acb/adapters/dns/__init__.py
--rw-r--r--   0        0        0     1044 2024-02-08 21:13:44.164932 acb-0.5.9/acb/adapters/dns/_base.py
--rw-r--r--   0        0        0     4880 2024-02-04 19:48:52.688550 acb-0.5.9/acb/adapters/dns/cloud_dns.py
--rw-r--r--   0        0        0       61 2023-11-04 13:17:17.317246 acb-0.5.9/acb/adapters/ftpd/__init__.py
--rw-r--r--   0        0        0      192 2024-02-08 21:13:44.096140 acb-0.5.9/acb/adapters/ftpd/_base.py
--rw-r--r--   0        0        0      927 2024-02-09 17:35:46.084380 acb-0.5.9/acb/adapters/ftpd/ftp.py
--rw-r--r--   0        0        0     1186 2024-02-09 11:37:04.876043 acb-0.5.9/acb/adapters/ftpd/sftp.py
--rw-r--r--   0        0        0       63 2023-11-04 13:17:17.311082 acb-0.5.9/acb/adapters/logger/__init__.py
--rw-r--r--   0        0        0      154 2024-02-08 21:13:44.117416 acb-0.5.9/acb/adapters/logger/_base.py
--rw-r--r--   0        0        0     3333 2024-02-09 09:30:31.991719 acb-0.5.9/acb/adapters/logger/loguru.py
--rw-r--r--   0        0        0       36 2023-11-06 07:39:19.522148 acb-0.5.9/acb/adapters/logger/structlog.py
--rw-r--r--   0        0        0       67 2023-11-04 13:17:17.331356 acb-0.5.9/acb/adapters/monitoring/__init__.py
--rw-r--r--   0        0        0      223 2024-02-09 11:37:04.889721 acb-0.5.9/acb/adapters/monitoring/_base.py
--rw-r--r--   0        0        0      720 2024-02-04 19:48:52.574105 acb-0.5.9/acb/adapters/monitoring/sentry.py
--rw-r--r--   0        0        0       62 2023-11-04 13:17:17.303819 acb-0.5.9/acb/adapters/nosql/__init__.py
--rw-r--r--   0        0        0      210 2024-02-08 14:44:50.391598 acb-0.5.9/acb/adapters/nosql/_base.py
--rw-r--r--   0        0        0       36 2023-11-06 07:39:19.537543 acb-0.5.9/acb/adapters/nosql/firestore.py
--rw-r--r--   0        0        0       32 2023-11-06 07:39:19.533503 acb-0.5.9/acb/adapters/nosql/mongodb.py
--rw-r--r--   0        0        0      531 2023-09-27 19:36:20.695500 acb-0.5.9/acb/adapters/nosql/redis.py
--rw-r--r--   0        0        0       65 2023-11-04 13:17:17.335837 acb-0.5.9/acb/adapters/requests/__init__.py
--rw-r--r--   0        0        0     1028 2024-02-09 09:59:55.837594 acb-0.5.9/acb/adapters/requests/_base.py
--rw-r--r--   0        0        0     1673 2024-02-09 17:35:46.206206 acb-0.5.9/acb/adapters/requests/httpx.py
--rw-r--r--   0        0        0       63 2024-03-01 14:14:36.276395 acb-0.5.9/acb/adapters/secret/__init__.py
--rw-r--r--   0        0        0      776 2024-03-01 14:28:02.408356 acb-0.5.9/acb/adapters/secret/_base.py
--rw-r--r--   0        0        0       44 2023-11-06 07:39:19.541900 acb-0.5.9/acb/adapters/secret/infisical.py
--rw-r--r--   0        0        0     4617 2024-03-01 14:28:02.414547 acb-0.5.9/acb/adapters/secret/secret_manager.py
--rw-r--r--   0        0        0       61 2023-11-04 13:17:17.297294 acb-0.5.9/acb/adapters/smtp/__init__.py
--rw-r--r--   0        0        0     1264 2024-02-08 21:13:44.252071 acb-0.5.9/acb/adapters/smtp/_base.py
--rw-r--r--   0        0        0      513 2024-02-04 19:48:52.578362 acb-0.5.9/acb/adapters/smtp/gmail.py
--rw-r--r--   0        0        0     8886 2024-02-09 13:11:23.103262 acb-0.5.9/acb/adapters/smtp/mailgun.py
--rw-r--r--   0        0        0       60 2024-01-24 11:37:13.631301 acb-0.5.9/acb/adapters/sql/__init__.py
--rw-r--r--   0        0        0    12235 2024-02-09 13:11:23.094473 acb-0.5.9/acb/adapters/sql/_backup.py
--rw-r--r--   0        0        0     5572 2024-03-09 15:03:14.357031 acb-0.5.9/acb/adapters/sql/_base.py
--rw-r--r--   0        0        0       26 2024-02-08 14:45:26.613293 acb-0.5.9/acb/adapters/sql/_migrate.py
--rw-r--r--   0        0        0      316 2024-03-09 14:44:51.517804 acb-0.5.9/acb/adapters/sql/mysql.py
--rw-r--r--   0        0        0       32 2023-11-06 07:39:19.528015 acb-0.5.9/acb/adapters/sql/pgsql.py
--rw-r--r--   0        0        0       64 2023-11-04 13:17:17.284637 acb-0.5.9/acb/adapters/storage/__init__.py
--rw-r--r--   0        0        0     5464 2024-03-02 09:47:43.464852 acb-0.5.9/acb/adapters/storage/_base.py
--rw-r--r--   0        0        0      368 2023-10-16 10:33:57.704006 acb-0.5.9/acb/adapters/storage/azure.py
--rw-r--r--   0        0        0     1456 2023-12-29 09:18:35.395587 acb-0.5.9/acb/adapters/storage/cloud_storage.py
--rw-r--r--   0        0        0      548 2024-02-04 19:48:52.633037 acb-0.5.9/acb/adapters/storage/file.py
--rw-r--r--   0        0        0      326 2024-02-04 19:48:52.631331 acb-0.5.9/acb/adapters/storage/memory.py
--rw-r--r--   0        0        0      381 2023-10-16 10:33:57.717425 acb-0.5.9/acb/adapters/storage/s3.py
--rw-r--r--   0        0        0    10433 2024-03-01 14:34:19.424984 acb-0.5.9/acb/config.py
--rw-r--r--   0        0        0     1955 2024-02-09 20:35:55.823253 acb-0.5.9/acb/debug.py
--rw-r--r--   0        0        0      587 2024-01-13 20:57:32.759244 acb-0.5.9/acb/depends.py
--rw-r--r--   0        0        0     3377 2024-03-09 15:07:54.600770 acb-0.5.9/pyproject.toml
--rw-r--r--   0        0        0     3601 1970-01-01 00:00:00.000000 acb-0.5.9/PKG-INFO
+-rw-r--r--   0        0        0     1531 2023-04-13 18:37:22.056785 acb-0.6.0/LICENSE
+-rw-r--r--   0        0        0      877 2024-02-25 15:01:48.403334 acb-0.6.0/README.md
+-rw-r--r--   0        0        0      880 2024-02-09 10:50:18.605994 acb-0.6.0/acb/__init__.py
+-rw-r--r--   0        0        0      819 2024-01-16 17:26:09.434218 acb-0.6.0/acb/actions/__init__.py
+-rw-r--r--   0        0        0     1180 2023-10-09 11:44:35.662080 acb-0.6.0/acb/actions/compress.py
+-rw-r--r--   0        0        0     4784 2024-03-18 08:07:46.797620 acb-0.6.0/acb/actions/encode.py
+-rw-r--r--   0        0        0      897 2023-10-11 15:39:52.116219 acb-0.6.0/acb/actions/hash.py
+-rw-r--r--   0        0        0     5526 2024-03-18 07:52:52.122921 acb-0.6.0/acb/adapters/__init__.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:17:17.290924 acb-0.6.0/acb/adapters/app/__init__.py
+-rw-r--r--   0        0        0      242 2024-02-09 17:35:46.026715 acb-0.6.0/acb/adapters/app/_base.py
+-rw-r--r--   0        0        0     1286 2024-02-09 17:35:46.099339 acb-0.6.0/acb/adapters/app/main.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:17:17.342044 acb-0.6.0/acb/adapters/cache/__init__.py
+-rw-r--r--   0        0        0     1610 2024-03-02 10:09:36.352462 acb-0.6.0/acb/adapters/cache/_base.py
+-rw-r--r--   0        0        0      828 2024-02-04 19:59:42.029846 acb-0.6.0/acb/adapters/cache/memory.py
+-rw-r--r--   0        0        0     1635 2024-02-09 18:00:21.800300 acb-0.6.0/acb/adapters/cache/redis.py
+-rw-r--r--   0        0        0       60 2023-11-04 13:17:17.324879 acb-0.6.0/acb/adapters/dns/__init__.py
+-rw-r--r--   0        0        0     1044 2024-02-08 21:13:44.164932 acb-0.6.0/acb/adapters/dns/_base.py
+-rw-r--r--   0        0        0     4880 2024-02-04 19:48:52.688550 acb-0.6.0/acb/adapters/dns/cloud_dns.py
+-rw-r--r--   0        0        0       61 2023-11-04 13:17:17.317246 acb-0.6.0/acb/adapters/ftpd/__init__.py
+-rw-r--r--   0        0        0      192 2024-02-08 21:13:44.096140 acb-0.6.0/acb/adapters/ftpd/_base.py
+-rw-r--r--   0        0        0      927 2024-02-09 17:35:46.084380 acb-0.6.0/acb/adapters/ftpd/ftp.py
+-rw-r--r--   0        0        0     1186 2024-02-09 11:37:04.876043 acb-0.6.0/acb/adapters/ftpd/sftp.py
+-rw-r--r--   0        0        0       63 2023-11-04 13:17:17.311082 acb-0.6.0/acb/adapters/logger/__init__.py
+-rw-r--r--   0        0        0      154 2024-02-08 21:13:44.117416 acb-0.6.0/acb/adapters/logger/_base.py
+-rw-r--r--   0        0        0     3512 2024-04-12 00:33:56.007870 acb-0.6.0/acb/adapters/logger/loguru.py
+-rw-r--r--   0        0        0       36 2023-11-06 07:39:19.522148 acb-0.6.0/acb/adapters/logger/structlog.py
+-rw-r--r--   0        0        0       63 2024-02-07 20:56:24.207919 acb-0.6.0/acb/adapters/models/__init__.py
+-rw-r--r--   0        0        0      247 2024-05-19 15:42:40.075662 acb-0.6.0/acb/adapters/models/_base.py
+-rw-r--r--   0        0        0     2361 2024-05-19 15:48:46.214106 acb-0.6.0/acb/adapters/models/default.py
+-rw-r--r--   0        0        0       67 2023-11-04 13:17:17.331356 acb-0.6.0/acb/adapters/monitoring/__init__.py
+-rw-r--r--   0        0        0      223 2024-02-09 11:37:04.889721 acb-0.6.0/acb/adapters/monitoring/_base.py
+-rw-r--r--   0        0        0      720 2024-02-04 19:48:52.574105 acb-0.6.0/acb/adapters/monitoring/sentry.py
+-rw-r--r--   0        0        0       62 2023-11-04 13:17:17.303819 acb-0.6.0/acb/adapters/nosql/__init__.py
+-rw-r--r--   0        0        0      210 2024-02-08 14:44:50.391598 acb-0.6.0/acb/adapters/nosql/_base.py
+-rw-r--r--   0        0        0       36 2023-11-06 07:39:19.537543 acb-0.6.0/acb/adapters/nosql/firestore.py
+-rw-r--r--   0        0        0       32 2023-11-06 07:39:19.533503 acb-0.6.0/acb/adapters/nosql/mongodb.py
+-rw-r--r--   0        0        0      531 2023-09-27 19:36:20.695500 acb-0.6.0/acb/adapters/nosql/redis.py
+-rw-r--r--   0        0        0       65 2023-11-04 13:17:17.335837 acb-0.6.0/acb/adapters/requests/__init__.py
+-rw-r--r--   0        0        0     1028 2024-02-09 09:59:55.837594 acb-0.6.0/acb/adapters/requests/_base.py
+-rw-r--r--   0        0        0     1673 2024-02-09 17:35:46.206206 acb-0.6.0/acb/adapters/requests/httpx.py
+-rw-r--r--   0        0        0       63 2024-03-01 14:14:36.276395 acb-0.6.0/acb/adapters/secret/__init__.py
+-rw-r--r--   0        0        0      776 2024-03-01 14:28:02.408356 acb-0.6.0/acb/adapters/secret/_base.py
+-rw-r--r--   0        0        0       44 2023-11-06 07:39:19.541900 acb-0.6.0/acb/adapters/secret/infisical.py
+-rw-r--r--   0        0        0     4617 2024-03-01 14:28:02.414547 acb-0.6.0/acb/adapters/secret/secret_manager.py
+-rw-r--r--   0        0        0       61 2023-11-04 13:17:17.297294 acb-0.6.0/acb/adapters/smtp/__init__.py
+-rw-r--r--   0        0        0     1264 2024-02-08 21:13:44.252071 acb-0.6.0/acb/adapters/smtp/_base.py
+-rw-r--r--   0        0        0      513 2024-02-04 19:48:52.578362 acb-0.6.0/acb/adapters/smtp/gmail.py
+-rw-r--r--   0        0        0     8886 2024-02-09 13:11:23.103262 acb-0.6.0/acb/adapters/smtp/mailgun.py
+-rw-r--r--   0        0        0       60 2024-01-24 11:37:13.631301 acb-0.6.0/acb/adapters/sql/__init__.py
+-rw-r--r--   0        0        0    12235 2024-02-09 13:11:23.094473 acb-0.6.0/acb/adapters/sql/_backup.py
+-rw-r--r--   0        0        0     6668 2024-04-02 07:53:33.461560 acb-0.6.0/acb/adapters/sql/_base.py
+-rw-r--r--   0        0        0       26 2024-02-08 14:45:26.613293 acb-0.6.0/acb/adapters/sql/_migrate.py
+-rw-r--r--   0        0        0      253 2024-03-09 15:10:21.640219 acb-0.6.0/acb/adapters/sql/mysql.py
+-rw-r--r--   0        0        0       32 2023-11-06 07:39:19.528015 acb-0.6.0/acb/adapters/sql/pgsql.py
+-rw-r--r--   0        0        0       64 2023-11-04 13:17:17.284637 acb-0.6.0/acb/adapters/storage/__init__.py
+-rw-r--r--   0        0        0     5464 2024-03-02 09:47:43.464852 acb-0.6.0/acb/adapters/storage/_base.py
+-rw-r--r--   0        0        0      368 2023-10-16 10:33:57.704006 acb-0.6.0/acb/adapters/storage/azure.py
+-rw-r--r--   0        0        0     1456 2023-12-29 09:18:35.395587 acb-0.6.0/acb/adapters/storage/cloud_storage.py
+-rw-r--r--   0        0        0      548 2024-02-04 19:48:52.633037 acb-0.6.0/acb/adapters/storage/file.py
+-rw-r--r--   0        0        0      326 2024-02-04 19:48:52.631331 acb-0.6.0/acb/adapters/storage/memory.py
+-rw-r--r--   0        0        0      381 2023-10-16 10:33:57.717425 acb-0.6.0/acb/adapters/storage/s3.py
+-rw-r--r--   0        0        0    10433 2024-04-02 07:37:38.490567 acb-0.6.0/acb/config.py
+-rw-r--r--   0        0        0     2212 2024-04-02 07:49:59.744042 acb-0.6.0/acb/debug.py
+-rw-r--r--   0        0        0      587 2024-01-13 20:57:32.759244 acb-0.6.0/acb/depends.py
+-rw-r--r--   0        0        0     3444 2024-05-19 15:51:54.369318 acb-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     3633 1970-01-01 00:00:00.000000 acb-0.6.0/PKG-INFO
```

### Comparing `acb-0.5.9/LICENSE` & `acb-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/README.md` & `acb-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/__init__.py` & `acb-0.6.0/acb/__init__.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/actions/__init__.py` & `acb-0.6.0/acb/actions/__init__.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/actions/compress.py` & `acb-0.6.0/acb/actions/compress.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/actions/encode.py` & `acb-0.6.0/acb/actions/encode.py`

 * *Files 7% similar despite different names*

```diff
@@ -71,16 +71,16 @@
     pickle: t.Callable[..., t.Any]
     serializers: dict[str, t.Callable[..., t.Any]]
     path: t.Optional[AsyncPath] = None
     action: t.Optional[str] = None
     sort_keys: bool = True
     use_list: bool = False
     secure: bool = False
-    secret_key: str = ""
-    secure_salt: str = ""
+    secret_key: t.Optional[str] = None
+    secure_salt: t.Optional[str] = None
     serializer: t.Optional[t.Callable[..., t.Any]] = None
 
     def __init__(self) -> None:
         self.serializers = serializers.__dict__
         for s in self.serializers:
             setattr(self, s, self.__call__)
 
@@ -107,15 +107,15 @@
         return calling_method.group(1), calling_method.group(2)  # type: ignore
 
     def get_serializer(self, serializer: t.Any) -> t.Any:
         return (
             serializer
             if not self.secure
             else SecureSerializer(
-                secret_key=self.secret_key,
+                secret_key=self.secret_key,  # type: ignore
                 salt=self.secure_salt,
                 serializer=serializer,
                 signer_kwargs=dict(digest_method=blake3),
             )
         )
 
     async def __call__(
@@ -127,19 +127,19 @@
         secret_key: t.Optional[SecretStr] = None,
         secure_salt: t.Optional[SecretStr] = None,
         **kwargs: object,
     ) -> dict[str, str] | bytes:
         self.path = path
         self.sort_keys = sort_keys
         self.use_list = use_list
-        self.secret_key = "" if not secret_key else secret_key.get_secret_value()
-        self.secure_salt = "" if not secure_salt else secure_salt.get_secret_value()
+        self.secret_key = secret_key.get_secret_value() if secret_key else None
+        self.secure_salt = secure_salt.get_secret_value() if secure_salt else None
         self.action, serializer_name = self.get_vars(sys._getframe(1))
         self.secure = all((secret_key, secure_salt))
-        if not self.secure and (len(self.secret_key) and len(self.secure_salt)):
+        if not self.secure and (secret_key or secure_salt):
             warn(
                 f"{serializer_name.title()} serializer won't sign "
                 f"objects unless both "
                 f"secret_key and secure_salt are set"
             )
         self.serializer = self.get_serializer(self.serializers[serializer_name])
         return await self.process(obj, **kwargs)  # type: ignore
```

### Comparing `acb-0.5.9/acb/actions/hash.py` & `acb-0.6.0/acb/actions/hash.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/__init__.py` & `acb-0.6.0/acb/adapters/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,19 +22,15 @@
 settings_path: Path = Path(base_path / "settings")
 app_settings_path: Path = settings_path / "app.yml"
 adapter_settings_path: Path = settings_path / "adapters.yml"
 
 
 def get_adapter(category: str) -> Adapter | None:
     _adapter = next(
-        (
-            a
-            for a in adapter_registry.get()
-            if a.category == category and a.enabled is True
-        ),
+        (a for a in adapter_registry.get() if a.category == category and a.enabled),
         None,
     )
     return _adapter
 
 
 def get_installed_adapters() -> list[Adapter]:
     return [a for a in adapter_registry.get() if a.installed]
```

### Comparing `acb-0.5.9/acb/adapters/app/main.py` & `acb-0.6.0/acb/adapters/app/main.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/cache/_base.py` & `acb-0.6.0/acb/adapters/cache/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/cache/memory.py` & `acb-0.6.0/acb/adapters/cache/memory.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/cache/redis.py` & `acb-0.6.0/acb/adapters/cache/redis.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/dns/_base.py` & `acb-0.6.0/acb/adapters/dns/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/dns/cloud_dns.py` & `acb-0.6.0/acb/adapters/dns/cloud_dns.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/ftpd/ftp.py` & `acb-0.6.0/acb/adapters/ftpd/ftp.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/ftpd/sftp.py` & `acb-0.6.0/acb/adapters/ftpd/sftp.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/logger/loguru.py` & `acb-0.6.0/acb/adapters/logger/loguru.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,19 +14,20 @@
 
 class LoggerSettings(LoggerBaseSettings):
     serialize: t.Optional[bool] = False
     format: t.Optional[dict[str, str]] = dict(
         time="<b><e>[</e> <w>{time:YYYY-MM-DD HH:mm:ss.SSS}</w> <e>]</e></b>",
         level=" <level>{level:>8}</level>",
         sep=" <b><w>in</w></b> ",
-        name="{extra[mod_name]:>18}",
+        name="<b>{extra[mod_name]:>18}</b>",
         line="<b><e>[</e><w>{line:^5}</w><e>]</e></b>",
         message="  <level>{message}</level>",
     )
     level_per_module: t.Optional[dict[str, str]] = {}
+    level_colors: t.Optional[dict[str, str]] = {}
     settings: t.Optional[dict[str, t.Any]] = {}
 
     @depends.inject
     def __init__(self, config: Config = depends(), **values: t.Any) -> None:
         super().__init__(**values)
         self.serialize = True if config.deployed else False
         self.level_per_module = {m: "DEBUG" if v else "INFO" for m, v in debug.items()}
@@ -67,15 +68,17 @@
 
         self.remove()
         self.configure(
             patcher=lambda record: record["extra"].update(  # type: ignore
                 mod_name=patch_name(record)
             )
         )
-        self.add(sys.stderr, **config.logger.settings)
+        self.add(sys.stdout, **config.logger.settings)
+        for level, color in config.logger.level_colors.items():
+            self.level(level.upper(), color=f"<{color}>")
         if config.deployed:
             self.level = config.logger.deployed_level
         if config.debug.logger:
             self.debug("debug")
             self.info("info")
             self.warning("warning")
             self.error("error")
```

### Comparing `acb-0.5.9/acb/adapters/monitoring/sentry.py` & `acb-0.6.0/acb/adapters/monitoring/sentry.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/nosql/redis.py` & `acb-0.6.0/acb/adapters/nosql/redis.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/requests/_base.py` & `acb-0.6.0/acb/adapters/requests/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/requests/httpx.py` & `acb-0.6.0/acb/adapters/requests/httpx.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/secret/_base.py` & `acb-0.6.0/acb/adapters/secret/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/secret/secret_manager.py` & `acb-0.6.0/acb/adapters/secret/secret_manager.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/smtp/_base.py` & `acb-0.6.0/acb/adapters/smtp/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/smtp/gmail.py` & `acb-0.6.0/acb/adapters/smtp/gmail.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/smtp/mailgun.py` & `acb-0.6.0/acb/adapters/smtp/mailgun.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/sql/_backup.py` & `acb-0.6.0/acb/adapters/sql/_backup.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/sql/_base.py` & `acb-0.6.0/acb/adapters/sql/_base.py`

 * *Files 10% similar despite different names*

```diff
@@ -3,21 +3,23 @@
 from functools import cached_property
 
 import nest_asyncio
 from acb.adapters import AdapterBase
 from acb.config import Config
 from acb.config import gen_password
 from acb.config import Settings
+from acb.debug import debug
 from acb.depends import depends
 from aioconsole import ainput
 from aioconsole import aprint
 from pydantic import SecretStr
 from sqlalchemy import inspect
 from sqlalchemy import log as sqlalchemy_log
 from sqlalchemy import pool
+from sqlalchemy import text
 from sqlalchemy.engine import URL
 from sqlalchemy.exc import OperationalError
 from sqlalchemy.ext.asyncio import AsyncConnection
 from sqlalchemy.ext.asyncio import AsyncEngine
 from sqlalchemy.ext.asyncio import create_async_engine
 from sqlalchemy_utils import create_database
 from sqlalchemy_utils import database_exists
@@ -35,15 +37,15 @@
     pool_pre_ping: t.Optional[bool] = False
     poolclass: t.Optional[t.Any] = None
     host: SecretStr = SecretStr("127.0.0.1")
     user: SecretStr = SecretStr("root")
     password: SecretStr = SecretStr(gen_password())
     _url: t.Optional[URL] = None
     _async_url: t.Optional[URL] = None
-    engine_kwargs: t.Optional[dict[str, t.Any | None]] = {}
+    engine_kwargs: dict[str, t.Any] = {}
     backup_enabled: bool = False
     backup_bucket: str | None = None
 
     @depends.inject
     def __init__(self, config: Config = depends(), **values: t.Any) -> None:
         super().__init__(**values)
         url_kwargs = dict(
@@ -51,18 +53,27 @@
             username=self.user.get_secret_value(),
             password=self.password.get_secret_value(),
             host=("127.0.0.1" if not config.deployed else self.host.get_secret_value()),
             port=self.port,
             database=config.app.name,
         )
         self.poolclass = getattr(pool, self.poolclass) if self.poolclass else None
+        debug(self.poolclass)
+        debug(type(self.poolclass))
         self._url = URL.create(**url_kwargs)  # type: ignore
+        debug(self._url)
         async_url_kwargs = dict(drivername=self._async_driver)
         self._async_url = URL.create(**(url_kwargs | async_url_kwargs))  # type: ignore
-        self.engine_kwargs["echo"] = config.debug.sql  # type: ignore
+        debug(self._async_url)
+        self.engine_kwargs["echo"] = (
+            "debug" if config.logger.verbose else config.debug.sql
+        )
+        self.engine_kwargs["echo_pool"] = (
+            "debug" if config.logger.verbose else config.debug.sql
+        )
         self.engine_kwargs = (  # type: ignore
             dict(poolclass=self.poolclass, pool_pre_ping=self.pool_pre_ping)
             | self.engine_kwargs
         )
 
 
 class SqlBase(AdapterBase):
@@ -77,19 +88,16 @@
     @cached_property
     def session(self) -> AsyncSession:
         return AsyncSession(self.engine, expire_on_commit=False)
 
     async def create(self, demo: bool = False) -> None:
         try:
             self.exists = database_exists(self.config.sql._url)
-            if self.exists:
-                self.logger.debug("Sql database exists")
         except OperationalError:
             self.exists = False
-
         if (
             self.config.debug.sql
             and not (self.config.deployed or self.config.debug.production)
             and self.exists
         ):
             msg = (
                 "\n\nRESETTING THE SQL DATABASE WILL CAUSE ALL OF YOUR"
@@ -107,14 +115,16 @@
             if delete_db.upper().strip() == "Y":
                 drop_database(self.config.sql._url)
                 self.logger.warning("Sql database dropped")
                 self.exists = database_exists(self.config.sql._url)
         if not self.exists:
             create_database(self.config.sql._url)
             self.logger.debug("Sql database created")
+        else:
+            self.logger.debug("Sql database exists")
 
     @asynccontextmanager
     async def get_session(self) -> t.AsyncGenerator[AsyncSession, None]:
         async with self.session as sess:
             yield sess
 
     @asynccontextmanager
@@ -129,20 +139,39 @@
 
     async def init(
         self,
     ) -> None:
         sqlalchemy_log._add_default_handler = lambda x: None  # type: ignore
         await self.create()
         async with self.get_conn() as conn:
-            # if self.config.debug.sql:
-            #     sql = text("DROP TABLE IF EXISTS alembic_version")
-            #     await conn.execute(sql)
+            if self.config.debug.sql:
+                ps = await conn.execute(text("SHOW FULL PROCESSLIST"))
+                # inno = await conn.execute(text("SHOW INNODB STATUS"))
+                # debug(inno)
+                show_ps = [p for p in ps]
+                debug(show_ps)
+                ids = [
+                    a[0]
+                    for a in show_ps
+                    if (
+                        a[1] == self.config.sql.user.get_secret_value()
+                        and a[3] == self.config.app.name
+                        # and a[3] == "gmb"
+                    )
+                ]
+                debug(ids)
+                # if force:
+                # for id in ids:
+                #     await conn.execute(text(f"KILL {id}"))
+                #     sql = text("DROP TABLE IF EXISTS alembic_version")
+                #     await conn.execute(sql)
             action = "Creating" if not self.exists else "Updating"
             self.logger.info(f"{action} database tables...")
             try:
+                await conn.run_sync(SQLModel.metadata.drop_all)
                 await conn.run_sync(SQLModel.metadata.create_all)
             except Exception as e:
                 self.logger.error(e)
             if not self.exists:
                 table_names = await conn.run_sync(self.get_table_names)
                 for name in table_names:
                     self.logger.debug(f"Created table: {name}")
```

### Comparing `acb-0.5.9/acb/adapters/storage/_base.py` & `acb-0.6.0/acb/adapters/storage/_base.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/storage/cloud_storage.py` & `acb-0.6.0/acb/adapters/storage/cloud_storage.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/adapters/storage/file.py` & `acb-0.6.0/acb/adapters/storage/file.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/config.py` & `acb-0.6.0/acb/config.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/acb/debug.py` & `acb-0.6.0/acb/debug.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,22 @@
+import asyncio
 import logging
 import typing as t
 from pathlib import Path
-from pprint import pformat
 from time import perf_counter
 
 from acb.adapters import import_adapter
 from acb.config import adapter_registry
 from acb.config import Config
 from acb.depends import depends
-from icecream import colorizedStderrPrint
+from aioconsole import aprint
+from devtools import pformat
+from icecream import colorize
 from icecream import ic as debug
+from icecream import supportTerminalColorsInWindows
 
 Logger = import_adapter()
 
 config = depends.get(Config)
 
 
 def get_calling_module() -> Path | None:
@@ -33,26 +36,32 @@
         if a.category == "logger" and a.name == "loguru"
     ):
         logger.patch(lambda record: record.update(name=mod.name)).debug(  # type: ignore
             msg
         )
 
 
+def colorized_stderr_print(s: str) -> None:
+    colored = colorize(s)
+    with supportTerminalColorsInWindows():
+        asyncio.run(aprint(colored, use_stderr=True))
+
+
 def print_debug_info(msg: str) -> t.Any:
     mod = get_calling_module()
     if mod:
         if config.deployed or config.debug.production:
             patch_record(mod, msg)
         else:
-            colorizedStderrPrint(msg)
+            colorized_stderr_print(msg)
 
 
 debug_args = dict(
     outputFunction=print_debug_info,
-    argToStringFunction=lambda o: pformat(o, sort_dicts=False),
+    argToStringFunction=lambda o: pformat(o, highlight=False),
 )
 debug.configureOutput(
     prefix="    debug:  ",
     includeContext=True,
     **debug_args,
 )
 if config.deployed or config.debug.production:
```

### Comparing `acb-0.5.9/acb/depends.py` & `acb-0.6.0/acb/depends.py`

 * *Files identical despite different names*

### Comparing `acb-0.5.9/pyproject.toml` & `acb-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,14 +12,19 @@
 [tool.ruff]
 line-length = 88
 target-version = "py312"
 fix = true
 show-fixes = true
 output-format = "full"
 
+[tool.ruff.lint]
+ignore = [
+    "F821",
+]
+
 [tool.ruff.lint.isort]
 force-single-line = true
 
 [tool.ruff.lint.mccabe]
 max-complexity = 10
 
 [tool.ruff.lint.pydocstyle]
@@ -32,38 +37,38 @@
 
 [tool.creosote]
 paths = [
     "acb",
 ]
 deps-file = "pyproject.toml"
 exclude-deps = [
-    "phonenumbers",
-    "pyyaml",
-    "autotyping",
-    "pre-commit",
-    "ulid-py",
     "pdm",
     "pdm-bump",
+    "pre-commit",
+    "autotyping",
     "pyfiglet",
+    "pyyaml",
+    "ulid-py",
     "pytest",
+    "phonenumbers",
     "alive-progress",
 ]
 
 [tool.refurb]
 enable_all = true
 
 [tool.bandit]
 target = [
     "acb",
 ]
 skips = [
     "B603",
+    "B404",
     "B403",
     "B113",
-    "B404",
 ]
 
 [tool.pyright]
 verboseOutput = true
 include = [
     "acb",
 ]
@@ -84,15 +89,15 @@
 [tool.codespell]
 skip = "*/data/*"
 quiet-level = 3
 ignore-words-list = "crate,uptodate"
 
 [project]
 name = "acb"
-version = "0.5.9"
+version = "0.6.0"
 description = "Asynchronous Component Base"
 dependencies = [
     "itsdangerous>=2.1.2",
     "arrow>=1.3.0",
     "dill>=0.3.8",
     "blake3>=0.4.1",
     "loguru>=0.7.2",
@@ -105,14 +110,15 @@
     "pyfiglet>=1.0.2",
     "alive-progress>=3.1.5",
     "inflection>=0.5.1",
     "aiopath>=0.7.7",
     "pyyaml>=6.0.1",
     "google-crc32c>=1.5.0",
     "pydantic[email]>=2.6.1",
+    "devtools>=0.12.2",
 ]
 requires-python = ">=3.12"
 readme = "README.md"
 authors = [
     { name = "lesleslie", email = "les@wedgwoodwebworks.com" },
 ]
 classifiers = [
```

### Comparing `acb-0.5.9/PKG-INFO` & `acb-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: acb
-Version: 0.5.9
+Version: 0.6.0
 Summary: Asynchronous Component Base
 Author-Email: lesleslie <les@wedgwoodwebworks.com>
 License: BSD-3-Clause
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Framework :: Pydantic
@@ -32,14 +32,15 @@
 Requires-Dist: pyfiglet>=1.0.2
 Requires-Dist: alive-progress>=3.1.5
 Requires-Dist: inflection>=0.5.1
 Requires-Dist: aiopath>=0.7.7
 Requires-Dist: pyyaml>=6.0.1
 Requires-Dist: google-crc32c>=1.5.0
 Requires-Dist: pydantic[email]>=2.6.1
+Requires-Dist: devtools>=0.12.2
 Requires-Dist: cashews[redis]>=7.0.0; extra == "cache"
 Requires-Dist: gcsfs>=2024.2.0; extra == "storage"
 Requires-Dist: s3fs>=2024.2.0; extra == "storage"
 Requires-Dist: adlfs>=2024.2.0; extra == "storage"
 Requires-Dist: google-cloud-dns>=0.35.0; extra == "dns"
 Requires-Dist: validators>=0.22.0; extra == "dns"
 Requires-Dist: httpx[http2]>=0.26.0; extra == "requests"
```

