# Comparing `tmp/tahrir_api-1.0.0.tar.gz` & `tmp/tahrir_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tahrir_api-1.0.0.tar", max compression
+gzip compressed data, was "tahrir_api-1.1.0.tar", max compression
```

## Comparing `tahrir_api-1.0.0.tar` & `tahrir_api-1.1.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
--rw-r--r--   0        0        0    35147 2024-03-06 10:08:38.072854 tahrir_api-1.0.0/LICENSE
--rw-r--r--   0        0        0     2510 2024-03-06 10:08:38.072854 tahrir_api-1.0.0/README.rst
--rw-r--r--   0        0        0      273 2024-04-12 13:36:07.983534 tahrir_api-1.0.0/examples/awardbadge.py
--rw-r--r--   0        0        0      519 2024-04-12 13:36:07.983534 tahrir_api-1.0.0/examples/fossboxbadge.py
--rw-r--r--   0        0        0     2028 2024-04-16 15:15:50.859264 tahrir_api-1.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-06 10:08:38.073854 tahrir_api-1.0.0/tahrir_api/__init__.py
--rw-r--r--   0        0        0    30886 2024-04-16 12:57:13.118516 tahrir_api-1.0.0/tahrir_api/dbapi.py
--rw-r--r--   0        0        0      154 2024-03-06 10:08:38.072854 tahrir_api-1.0.0/tahrir_api/migrations/README
--rw-r--r--   0        0        0      946 2024-03-06 10:08:38.072854 tahrir_api-1.0.0/tahrir_api/migrations/alembic.ini
--rw-r--r--   0        0        0     2121 2024-04-16 14:29:37.990720 tahrir_api-1.0.0/tahrir_api/migrations/env.py
--rw-r--r--   0        0        0      532 2024-04-16 14:33:44.206257 tahrir_api-1.0.0/tahrir_api/migrations/script.py.mako
--rw-r--r--   0        0        0      432 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tahrir_api/migrations/versions/139ec7ed17b7_add_a_rank_column_to.py
--rw-r--r--   0        0        0      445 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tahrir_api/migrations/versions/16943d9088cf_fix_foreign_key_mism.py
--rw-r--r--   0        0        0      609 2024-04-16 14:29:37.990720 tahrir_api-1.0.0/tahrir_api/migrations/versions/24282792d72a_add_created_by_field.py
--rw-r--r--   0        0        0      490 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tahrir_api/migrations/versions/2879ed5a6297_issued_for.py
--rw-r--r--   0        0        0      707 2024-04-16 14:29:37.990720 tahrir_api-1.0.0/tahrir_api/migrations/versions/39583332f4ea_add_profile_fields_t.py
--rw-r--r--   0        0        0     1037 2024-04-16 14:29:37.990720 tahrir_api-1.0.0/tahrir_api/migrations/versions/3c7fd5b4e2c2_add_two_new_columns_.py
--rw-r--r--   0        0        0      618 2024-04-16 14:29:37.990720 tahrir_api-1.0.0/tahrir_api/migrations/versions/4099fa344171_add_last_login.py
--rw-r--r--   0        0        0      507 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tahrir_api/migrations/versions/420c02357a1b_add_created_on_field.py
--rw-r--r--   0        0        0      510 2024-04-16 14:29:37.990720 tahrir_api-1.0.0/tahrir_api/migrations/versions/508367dcbbb5_add_an_stl_column_fo.py
--rw-r--r--   0        0        0      500 2024-04-16 14:29:37.990720 tahrir_api-1.0.0/tahrir_api/migrations/versions/5791a2b9fb6a_add_tags_field_to_ba.py
--rw-r--r--   0        0        0      735 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tahrir_api/migrations/versions/ce541796a7_add_authz_table.py
--rw-r--r--   0        0        0     2429 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tahrir_api/migrations/versions/e7040e76728_create_new_tables_for_quest.py
--rw-r--r--   0        0        0      526 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tahrir_api/migrations/versions/fa1d309e8c3_add_created_on_field.py
--rw-r--r--   0        0        0     9931 2024-04-16 12:54:03.656878 tahrir_api-1.0.0/tahrir_api/model.py
--rw-r--r--   0        0        0        0 2024-03-06 10:08:38.073854 tahrir_api-1.0.0/tahrir_api/scripts/__init__.py
--rw-r--r--   0        0        0     2705 2024-04-15 17:04:27.316278 tahrir_api-1.0.0/tahrir_api/scripts/populateseries.py
--rw-r--r--   0        0        0      383 2024-04-16 05:45:07.833267 tahrir_api-1.0.0/tahrir_api/scripts/syncdb.py
--rw-r--r--   0        0        0     1445 2024-04-16 06:02:37.465169 tahrir_api-1.0.0/tahrir_api/scripts/utils.py
--rw-r--r--   0        0        0      838 2024-04-15 16:33:53.573885 tahrir_api-1.0.0/tahrir_api/utils.py
--rw-r--r--   0        0        0        0 2024-03-06 10:08:38.073854 tahrir_api-1.0.0/tests/__init__.py
--rw-r--r--   0        0        0      408 2024-04-16 06:24:32.846311 tahrir_api-1.0.0/tests/conftest.py
--rw-r--r--   0        0        0     5578 2024-04-16 06:42:32.863046 tahrir_api-1.0.0/tests/test_dbapi.py
--rw-r--r--   0        0        0     4909 2024-04-16 14:29:37.991720 tahrir_api-1.0.0/tests/test_ranking.py
--rw-r--r--   0        0        0     3786 1970-01-01 00:00:00.000000 tahrir_api-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0    35147 2024-05-18 08:43:14.545872 tahrir_api-1.1.0/LICENSE
+-rw-r--r--   0        0        0     2510 2024-05-18 08:43:14.545872 tahrir_api-1.1.0/README.rst
+-rw-r--r--   0        0        0      273 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/examples/awardbadge.py
+-rw-r--r--   0        0        0      519 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/examples/fossboxbadge.py
+-rw-r--r--   0        0        0     2209 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/__init__.py
+-rw-r--r--   0        0        0    31012 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/dbapi.py
+-rw-r--r--   0        0        0      154 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/README
+-rw-r--r--   0        0        0      946 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/alembic.ini
+-rw-r--r--   0        0        0     2121 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/env.py
+-rw-r--r--   0        0        0      532 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/script.py.mako
+-rw-r--r--   0        0        0      432 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/versions/139ec7ed17b7_add_a_rank_column_to.py
+-rw-r--r--   0        0        0      445 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/versions/16943d9088cf_fix_foreign_key_mism.py
+-rw-r--r--   0        0        0      609 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/versions/24282792d72a_add_created_by_field.py
+-rw-r--r--   0        0        0      490 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/versions/2879ed5a6297_issued_for.py
+-rw-r--r--   0        0        0      707 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/versions/39583332f4ea_add_profile_fields_t.py
+-rw-r--r--   0        0        0     1037 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/versions/3c7fd5b4e2c2_add_two_new_columns_.py
+-rw-r--r--   0        0        0      466 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/versions/3d3fb9e59e7b_add_person_avatar.py
+-rw-r--r--   0        0        0      618 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/versions/4099fa344171_add_last_login.py
+-rw-r--r--   0        0        0      507 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/versions/420c02357a1b_add_created_on_field.py
+-rw-r--r--   0        0        0      510 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/versions/508367dcbbb5_add_an_stl_column_fo.py
+-rw-r--r--   0        0        0      500 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/versions/5791a2b9fb6a_add_tags_field_to_ba.py
+-rw-r--r--   0        0        0      735 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/versions/ce541796a7_add_authz_table.py
+-rw-r--r--   0        0        0     2429 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/versions/e7040e76728_create_new_tables_for_quest.py
+-rw-r--r--   0        0        0      526 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/migrations/versions/fa1d309e8c3_add_created_on_field.py
+-rw-r--r--   0        0        0     9769 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/model.py
+-rw-r--r--   0        0        0        0 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/scripts/__init__.py
+-rw-r--r--   0        0        0      840 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/scripts/populate_avatars.py
+-rw-r--r--   0        0        0     2705 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/scripts/populateseries.py
+-rw-r--r--   0        0        0      383 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/scripts/syncdb.py
+-rw-r--r--   0        0        0     1443 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/scripts/utils.py
+-rw-r--r--   0        0        0      838 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tahrir_api/utils.py
+-rw-r--r--   0        0        0        0 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tests/__init__.py
+-rw-r--r--   0        0        0      408 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tests/conftest.py
+-rw-r--r--   0        0        0     5578 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tests/test_dbapi.py
+-rw-r--r--   0        0        0     4909 2024-05-18 08:43:14.549872 tahrir_api-1.1.0/tests/test_ranking.py
+-rw-r--r--   0        0        0     3878 1970-01-01 00:00:00.000000 tahrir_api-1.1.0/PKG-INFO
```

### Comparing `tahrir_api-1.0.0/LICENSE` & `tahrir_api-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/README.rst` & `tahrir_api-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/examples/fossboxbadge.py` & `tahrir_api-1.1.0/examples/fossboxbadge.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/pyproject.toml` & `tahrir_api-1.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tahrir-api"
-version = "1.0.0"
+version = "1.1.0"
 description = "An API for interacting with the Tahrir database"
 
 license = "GPLv3+"
 
 authors = [
   "Ross Delinger <rdelinge@redhat.com>",
   "Fedora Infrastructure <admin@fedoraproject.org>",
@@ -38,26 +38,34 @@
 simplejson = "^3.19.2"
 sqlalchemy = "^2.0.29"
 arrow = "^1.3.0"
 alembic = "^1.13.1"
 fedora-messaging = "^3.5.0"
 tahrir-messages = "^1.0.2"
 sqlalchemy-helpers = ">=0.13.0"
+fasjson-client = {version = "^1.0.8", optional = true}
 
 
 [tool.poetry.group.dev.dependencies]
 coverage = {extras = ["toml"], version = ">=7.4.4"}
 black = ">=24.3.0"
 ruff = ">=0.3.5"
 pytest = ">=8.1.1"
 pytest-cov = ">=5.0.0"
 
+[tool.poetry.extras]
+scripts = [
+  "fasjson-client",
+]
+
 [tool.poetry.scripts]
 sync_tahrir_db = "tahrir_api.scripts.syncdb:main"
 populate_series_in_tahrir_db = "tahrir_api.scripts.populateseries:main"
+tahrir-populate-avatars = "tahrir_api.scripts.populate_avatars:main"
+
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 100
```

### Comparing `tahrir_api-1.0.0/tahrir_api/dbapi.py` & `tahrir_api-1.1.0/tahrir_api/dbapi.py`

 * *Files 1% similar despite different names*

```diff
@@ -560,38 +560,43 @@
         if self.person_exists(email=person_email):
             self.session.delete(self.get_person(person_email))
             self.session.flush()
             return person_email
         return False
 
     @autocommit
-    def add_person(self, email, nickname=None, website=None, bio=None):
+    def add_person(self, email, nickname=None, website=None, bio=None, avatar=None):
         """
         Add a new Person to the database
 
         :type email: str
         :param email: This Person's email address
 
         :type nickname: str
         :param nickname: This Person's nickname
 
         :type website: str
         :param website: This Person's website
 
-        :type website: str
+        :type bio: str
         :param bio: This Person's bio
+
+        :type avatar: str
+        :param avatar: This Person's avatar
         """
 
         if not self.person_exists(email=email):
             # If no nickname is specified, just use the first bit of their
             # email as a convenient default.
             if not nickname:
                 nickname = email.split("@")[0]
 
-            new_person = Person(email=email, nickname=nickname, website=website, bio=bio)
+            new_person = Person(
+                email=email, nickname=nickname, website=website, bio=bio, _avatar=avatar
+            )
             self.session.add(new_person)
             self.session.flush()
 
             return email
         return False
 
     @autocommit
@@ -635,15 +640,15 @@
 
         :type created_by: str
         :param created_by_email: User email of creator
 
         """
 
         if not self.badge_exists(badge_id):
-            raise ValueError("No such badge %r" % badge_id)
+            raise ValueError(f"No such badge {badge_id!r}")
 
         created_on = created_on or datetime.now(timezone.utc)
         expires_on = expires_on or (created_on + timedelta(hours=1))
         if self.person_exists(email=created_by_email):
             created_by = self.get_person(created_by_email).id
         else:
             created_by = self.session.query(Person).first().id
```

### Comparing `tahrir_api-1.0.0/tahrir_api/migrations/alembic.ini` & `tahrir_api-1.1.0/tahrir_api/migrations/alembic.ini`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/tahrir_api/migrations/env.py` & `tahrir_api-1.1.0/tahrir_api/migrations/env.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/tahrir_api/migrations/script.py.mako` & `tahrir_api-1.1.0/tahrir_api/migrations/script.py.mako`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/tahrir_api/migrations/versions/24282792d72a_add_created_by_field.py` & `tahrir_api-1.1.0/tahrir_api/migrations/versions/24282792d72a_add_created_by_field.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/tahrir_api/migrations/versions/39583332f4ea_add_profile_fields_t.py` & `tahrir_api-1.1.0/tahrir_api/migrations/versions/39583332f4ea_add_profile_fields_t.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/tahrir_api/migrations/versions/3c7fd5b4e2c2_add_two_new_columns_.py` & `tahrir_api-1.1.0/tahrir_api/migrations/versions/3c7fd5b4e2c2_add_two_new_columns_.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/tahrir_api/migrations/versions/4099fa344171_add_last_login.py` & `tahrir_api-1.1.0/tahrir_api/migrations/versions/4099fa344171_add_last_login.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/tahrir_api/migrations/versions/ce541796a7_add_authz_table.py` & `tahrir_api-1.1.0/tahrir_api/migrations/versions/ce541796a7_add_authz_table.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/tahrir_api/migrations/versions/e7040e76728_create_new_tables_for_quest.py` & `tahrir_api-1.1.0/tahrir_api/migrations/versions/e7040e76728_create_new_tables_for_quest.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/tahrir_api/migrations/versions/fa1d309e8c3_add_created_on_field.py` & `tahrir_api-1.1.0/tahrir_api/migrations/versions/fa1d309e8c3_add_created_on_field.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/tahrir_api/model.py` & `tahrir_api-1.1.0/tahrir_api/model.py`

 * *Files 3% similar despite different names*

```diff
@@ -136,14 +136,15 @@
         )
 
 
 class Person(DeclarativeBase):
     __tablename__ = "persons"
     id = Column(Integer, unique=True, primary_key=True)
     email = Column(Unicode(128), nullable=False, unique=True)
+    _avatar = Column(Unicode(128), nullable=True)
     authorizations = relationship("Authorization", backref="person")
     assertions = relationship("Assertion", backref="person")
     nickname = Column(Unicode(128), unique=True)
     website = Column(Unicode(128))
     bio = Column(Unicode(140))
     created_on = Column(DateTime, nullable=False, default=datetime.datetime.now)
     last_login = Column(DateTime, nullable=True, default=None)
@@ -153,28 +154,21 @@
     # indicates that they have not been ranked yet at all.
     rank = Column(Integer, default=None)
 
     def __repr__(self):
         return f"<Person: '{self.nickname} <{self.email}>'"
 
     @property
-    def gravatar_link(self):
-        d, s = "mm", 24
-        hash = self.email_md5
-        url = f"http://www.gravatar.com/avatar/{hash}?s={s}&d={d}"
-        return url
-
-    @property
-    def email_md5(self):
-        return hashlib.md5(self.email.encode("utf-8")).hexdigest()
-
-    @property
     def email_sha1(self):
         return hashlib.sha1(self.email.encode("utf-8")).hexdigest()
 
+    @property
+    def avatar(self):
+        return self._avatar or self.email
+
     def __str__(self):
         return str(self.email)
 
     def as_dict(self):
         return dict(
             email=self.email,
             id=self.id,
```

### Comparing `tahrir_api-1.0.0/tahrir_api/scripts/populateseries.py` & `tahrir_api-1.1.0/tahrir_api/scripts/populateseries.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/tahrir_api/scripts/utils.py` & `tahrir_api-1.1.0/tahrir_api/scripts/utils.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,15 +15,15 @@
     if name:
         section = name
     return path, section
 
 
 def get_db_manager_from_paste(config_uri):
     path, section = _getpathsec(config_uri, "pyramid")
-    config_name = "config:%s" % path
+    config_name = f"config:{path}"
     here_dir = os.getcwd()
 
     global_conf = None
     if "OPENSHIFT_APP_NAME" in os.environ:
         if "OPENSHIFT_MYSQL_DB_URL" in os.environ:
             template = "{OPENSHIFT_MYSQL_DB_URL}{OPENSHIFT_APP_NAME}"
         elif "OPENSHIFT_POSTGRESQL_DB_URL" in os.environ:
```

### Comparing `tahrir_api-1.0.0/tahrir_api/utils.py` & `tahrir_api-1.1.0/tahrir_api/utils.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/tests/test_dbapi.py` & `tahrir_api-1.1.0/tests/test_dbapi.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/tests/test_ranking.py` & `tahrir_api-1.1.0/tests/test_ranking.py`

 * *Files identical despite different names*

### Comparing `tahrir_api-1.0.0/PKG-INFO` & `tahrir_api-1.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tahrir-api
-Version: 1.0.0
+Version: 1.1.0
 Summary: An API for interacting with the Tahrir database
 Home-page: https://github.com/fedora-infra/tahrir-api
 License: GPLv3+
 Author: Ross Delinger
 Author-email: rdelinge@redhat.com
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Framework :: Pyramid
@@ -13,16 +13,18 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Internet :: WWW/HTTP
+Provides-Extra: scripts
 Requires-Dist: alembic (>=1.13.1,<2.0.0)
 Requires-Dist: arrow (>=1.3.0,<2.0.0)
+Requires-Dist: fasjson-client (>=1.0.8,<2.0.0) ; extra == "scripts"
 Requires-Dist: fedora-messaging (>=3.5.0,<4.0.0)
 Requires-Dist: pastedeploy (>=3.1.0,<4.0.0)
 Requires-Dist: pygments (>=2.17.2,<3.0.0)
 Requires-Dist: simplejson (>=3.19.2,<4.0.0)
 Requires-Dist: sqlalchemy (>=2.0.29,<3.0.0)
 Requires-Dist: sqlalchemy-helpers (>=0.13.0)
 Requires-Dist: tahrir-messages (>=1.0.2,<2.0.0)
```

