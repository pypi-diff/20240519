# Comparing `tmp/rococo_test-1.0.1.tar.gz` & `tmp/rococo_test-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rococo_test-1.0.1.tar", last modified: Sun May 19 10:21:51 2024, max compression
+gzip compressed data, was "rococo_test-1.0.2.tar", last modified: Sun May 19 11:22:42 2024, max compression
```

## Comparing `rococo_test-1.0.1.tar` & `rococo_test-1.0.2.tar`

### file list

```diff
@@ -1,80 +1,80 @@
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.384080 rococo_test-1.0.1/
--rw-r--r--   0 kote       (501) staff       (20)     1067 2024-05-05 21:58:39.000000 rococo_test-1.0.1/LICENSE
--rw-r--r--   0 kote       (501) staff       (20)    28901 2024-05-19 10:21:51.383732 rococo_test-1.0.1/PKG-INFO
--rw-r--r--   0 kote       (501) staff       (20)    28462 2024-05-05 21:58:39.000000 rococo_test-1.0.1/README.md
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.367351 rococo_test-1.0.1/rococo/
--rw-r--r--   0 kote       (501) staff       (20)        0 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/__init__.py
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.367745 rococo_test-1.0.1/rococo/auth/
--rw-r--r--   0 kote       (501) staff       (20)      180 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/auth/__init__.py
--rw-r--r--   0 kote       (501) staff       (20)     2599 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/auth/tokens.py
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.368112 rococo_test-1.0.1/rococo/config/
--rw-r--r--   0 kote       (501) staff       (20)      115 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/config/__init__.py
--rw-r--r--   0 kote       (501) staff       (20)     4328 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/config/config.py
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.368967 rococo_test-1.0.1/rococo/data/
--rw-r--r--   0 kote       (501) staff       (20)      155 2024-05-10 07:25:06.000000 rococo_test-1.0.1/rococo/data/__init__.py
--rw-r--r--   0 kote       (501) staff       (20)     2436 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/data/base.py
--rw-r--r--   0 kote       (501) staff       (20)     2841 2024-05-19 10:12:55.000000 rococo_test-1.0.1/rococo/data/mongodb.py
--rw-r--r--   0 kote       (501) staff       (20)     8098 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/data/mysql.py
--rw-r--r--   0 kote       (501) staff       (20)     6828 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/data/surrealdb.py
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.370002 rococo_test-1.0.1/rococo/emailing/
--rw-r--r--   0 kote       (501) staff       (20)      399 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/emailing/__init__.py
--rw-r--r--   0 kote       (501) staff       (20)      480 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/emailing/base.py
--rw-r--r--   0 kote       (501) staff       (20)     1574 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/emailing/config.py
--rw-r--r--   0 kote       (501) staff       (20)      151 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/emailing/enums.py
--rw-r--r--   0 kote       (501) staff       (20)     1118 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/emailing/factory.py
--rw-r--r--   0 kote       (501) staff       (20)     1558 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/emailing/mailjet.py
--rw-r--r--   0 kote       (501) staff       (20)      334 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/emailing/ses.py
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.370628 rococo_test-1.0.1/rococo/messaging/
--rw-r--r--   0 kote       (501) staff       (20)      171 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/messaging/__init__.py
--rw-r--r--   0 kote       (501) staff       (20)     1477 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/messaging/base.py
--rw-r--r--   0 kote       (501) staff       (20)     6111 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/messaging/rabbitmq.py
--rw-r--r--   0 kote       (501) staff       (20)     3985 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/messaging/sqs.py
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.372291 rococo_test-1.0.1/rococo/models/
--rw-r--r--   0 kote       (501) staff       (20)      336 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/__init__.py
--rw-r--r--   0 kote       (501) staff       (20)      420 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/email.py
--rw-r--r--   0 kote       (501) staff       (20)      597 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/login_method.py
--rw-r--r--   0 kote       (501) staff       (20)      639 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/organization.py
--rw-r--r--   0 kote       (501) staff       (20)      379 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/otp_method.py
--rw-r--r--   0 kote       (501) staff       (20)      221 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/person.py
--rw-r--r--   0 kote       (501) staff       (20)      827 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/person_organization_role.py
--rw-r--r--   0 kote       (501) staff       (20)      416 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/recovery_code.py
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.375524 rococo_test-1.0.1/rococo/models/surrealdb/
--rw-r--r--   0 kote       (501) staff       (20)      283 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/surrealdb/__init__.py
--rw-r--r--   0 kote       (501) staff       (20)      452 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/surrealdb/email.py
--rw-r--r--   0 kote       (501) staff       (20)      647 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/surrealdb/login_method.py
--rw-r--r--   0 kote       (501) staff       (20)      653 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/surrealdb/organization.py
--rw-r--r--   0 kote       (501) staff       (20)      472 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/surrealdb/otp_method.py
--rw-r--r--   0 kote       (501) staff       (20)      235 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/surrealdb/person.py
--rw-r--r--   0 kote       (501) staff       (20)      877 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/surrealdb/person_organization_role.py
--rw-r--r--   0 kote       (501) staff       (20)     2055 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/models/surrealdb/surreal_versioned_model.py
--rw-r--r--   0 kote       (501) staff       (20)     8576 2024-05-13 22:33:15.000000 rococo_test-1.0.1/rococo/models/versioned_model.py
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.376009 rococo_test-1.0.1/rococo/repositories/
--rw-r--r--   0 kote       (501) staff       (20)       43 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/repositories/__init__.py
--rw-r--r--   0 kote       (501) staff       (20)     3351 2024-05-14 00:36:03.000000 rococo_test-1.0.1/rococo/repositories/base_repository.py
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.376464 rococo_test-1.0.1/rococo/repositories/mongodb/
--rw-r--r--   0 kote       (501) staff       (20)        0 2024-05-09 14:11:44.000000 rococo_test-1.0.1/rococo/repositories/mongodb/__init__.py
--rw-r--r--   0 kote       (501) staff       (20)     5400 2024-05-19 10:08:55.000000 rococo_test-1.0.1/rococo/repositories/mongodb/mongodb_repository.py
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.377377 rococo_test-1.0.1/rococo/repositories/mysql/
--rw-r--r--   0 kote       (501) staff       (20)       46 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/repositories/mysql/__init__.py
--rw-r--r--   0 kote       (501) staff       (20)    12602 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/repositories/mysql/mysql_repository.py
--rw-r--r--   0 kote       (501) staff       (20)      666 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/repositories/mysql/organization_repository.py
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.378756 rococo_test-1.0.1/rococo/repositories/surrealdb/
--rw-r--r--   0 kote       (501) staff       (20)      287 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/repositories/surrealdb/__init__.py
--rw-r--r--   0 kote       (501) staff       (20)      687 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/repositories/surrealdb/organization_repository.py
--rw-r--r--   0 kote       (501) staff       (20)     1879 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/repositories/surrealdb/person_organization_role_repository.py
--rw-r--r--   0 kote       (501) staff       (20)    12105 2024-05-05 21:58:39.000000 rococo_test-1.0.1/rococo/repositories/surrealdb/surreal_db_repository.py
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.383193 rococo_test-1.0.1/rococo_test.egg-info/
--rw-r--r--   0 kote       (501) staff       (20)    28901 2024-05-19 10:21:51.000000 rococo_test-1.0.1/rococo_test.egg-info/PKG-INFO
--rw-r--r--   0 kote       (501) staff       (20)     1985 2024-05-19 10:21:51.000000 rococo_test-1.0.1/rococo_test.egg-info/SOURCES.txt
--rw-r--r--   0 kote       (501) staff       (20)        1 2024-05-19 10:21:51.000000 rococo_test-1.0.1/rococo_test.egg-info/dependency_links.txt
--rw-r--r--   0 kote       (501) staff       (20)       80 2024-05-19 10:21:51.000000 rococo_test-1.0.1/rococo_test.egg-info/requires.txt
--rw-r--r--   0 kote       (501) staff       (20)       13 2024-05-19 10:21:51.000000 rococo_test-1.0.1/rococo_test.egg-info/top_level.txt
--rw-r--r--   0 kote       (501) staff       (20)       38 2024-05-19 10:21:51.384129 rococo_test-1.0.1/setup.cfg
--rw-r--r--   0 kote       (501) staff       (20)      639 2024-05-19 10:21:47.000000 rococo_test-1.0.1/setup.py
-drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 10:21:51.382783 rococo_test-1.0.1/tests/
--rw-r--r--   0 kote       (501) staff       (20)        0 2024-05-05 21:58:39.000000 rococo_test-1.0.1/tests/__init__.py
--rw-r--r--   0 kote       (501) staff       (20)     5290 2024-05-13 22:53:08.000000 rococo_test-1.0.1/tests/base_repository_test.py
--rw-r--r--   0 kote       (501) staff       (20)     2007 2024-05-05 21:58:39.000000 rococo_test-1.0.1/tests/config_test.py
--rw-r--r--   0 kote       (501) staff       (20)     2241 2024-05-05 21:58:39.000000 rococo_test-1.0.1/tests/model_test.py
--rw-r--r--   0 kote       (501) staff       (20)     2493 2024-05-15 01:11:02.000000 rococo_test-1.0.1/tests/mongodb_repository_test.py
--rw-r--r--   0 kote       (501) staff       (20)     3004 2024-05-13 20:46:54.000000 rococo_test-1.0.1/tests/surreal_db_repository_test.py
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.406369 rococo_test-1.0.2/
+-rw-r--r--   0 kote       (501) staff       (20)     1067 2024-05-05 21:58:39.000000 rococo_test-1.0.2/LICENSE
+-rw-r--r--   0 kote       (501) staff       (20)    28901 2024-05-19 11:22:42.405940 rococo_test-1.0.2/PKG-INFO
+-rw-r--r--   0 kote       (501) staff       (20)    28462 2024-05-05 21:58:39.000000 rococo_test-1.0.2/README.md
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.389936 rococo_test-1.0.2/rococo/
+-rw-r--r--   0 kote       (501) staff       (20)        0 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/__init__.py
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.390434 rococo_test-1.0.2/rococo/auth/
+-rw-r--r--   0 kote       (501) staff       (20)      180 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/auth/__init__.py
+-rw-r--r--   0 kote       (501) staff       (20)     2599 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/auth/tokens.py
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.390912 rococo_test-1.0.2/rococo/config/
+-rw-r--r--   0 kote       (501) staff       (20)      115 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/config/__init__.py
+-rw-r--r--   0 kote       (501) staff       (20)     4328 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/config/config.py
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.392141 rococo_test-1.0.2/rococo/data/
+-rw-r--r--   0 kote       (501) staff       (20)      155 2024-05-10 07:25:06.000000 rococo_test-1.0.2/rococo/data/__init__.py
+-rw-r--r--   0 kote       (501) staff       (20)     2436 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/data/base.py
+-rw-r--r--   0 kote       (501) staff       (20)     2841 2024-05-19 10:12:55.000000 rococo_test-1.0.2/rococo/data/mongodb.py
+-rw-r--r--   0 kote       (501) staff       (20)     8098 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/data/mysql.py
+-rw-r--r--   0 kote       (501) staff       (20)     6828 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/data/surrealdb.py
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.393572 rococo_test-1.0.2/rococo/emailing/
+-rw-r--r--   0 kote       (501) staff       (20)      399 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/emailing/__init__.py
+-rw-r--r--   0 kote       (501) staff       (20)      480 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/emailing/base.py
+-rw-r--r--   0 kote       (501) staff       (20)     1574 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/emailing/config.py
+-rw-r--r--   0 kote       (501) staff       (20)      151 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/emailing/enums.py
+-rw-r--r--   0 kote       (501) staff       (20)     1118 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/emailing/factory.py
+-rw-r--r--   0 kote       (501) staff       (20)     1558 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/emailing/mailjet.py
+-rw-r--r--   0 kote       (501) staff       (20)      334 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/emailing/ses.py
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.394528 rococo_test-1.0.2/rococo/messaging/
+-rw-r--r--   0 kote       (501) staff       (20)      171 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/messaging/__init__.py
+-rw-r--r--   0 kote       (501) staff       (20)     1477 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/messaging/base.py
+-rw-r--r--   0 kote       (501) staff       (20)     6111 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/messaging/rabbitmq.py
+-rw-r--r--   0 kote       (501) staff       (20)     3985 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/messaging/sqs.py
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.396915 rococo_test-1.0.2/rococo/models/
+-rw-r--r--   0 kote       (501) staff       (20)      336 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/__init__.py
+-rw-r--r--   0 kote       (501) staff       (20)      420 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/email.py
+-rw-r--r--   0 kote       (501) staff       (20)      597 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/login_method.py
+-rw-r--r--   0 kote       (501) staff       (20)      639 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/organization.py
+-rw-r--r--   0 kote       (501) staff       (20)      379 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/otp_method.py
+-rw-r--r--   0 kote       (501) staff       (20)      221 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/person.py
+-rw-r--r--   0 kote       (501) staff       (20)      827 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/person_organization_role.py
+-rw-r--r--   0 kote       (501) staff       (20)      416 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/recovery_code.py
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.399632 rococo_test-1.0.2/rococo/models/surrealdb/
+-rw-r--r--   0 kote       (501) staff       (20)      283 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/surrealdb/__init__.py
+-rw-r--r--   0 kote       (501) staff       (20)      452 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/surrealdb/email.py
+-rw-r--r--   0 kote       (501) staff       (20)      647 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/surrealdb/login_method.py
+-rw-r--r--   0 kote       (501) staff       (20)      653 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/surrealdb/organization.py
+-rw-r--r--   0 kote       (501) staff       (20)      472 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/surrealdb/otp_method.py
+-rw-r--r--   0 kote       (501) staff       (20)      235 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/surrealdb/person.py
+-rw-r--r--   0 kote       (501) staff       (20)      877 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/surrealdb/person_organization_role.py
+-rw-r--r--   0 kote       (501) staff       (20)     2055 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/models/surrealdb/surreal_versioned_model.py
+-rw-r--r--   0 kote       (501) staff       (20)     8576 2024-05-13 22:33:15.000000 rococo_test-1.0.2/rococo/models/versioned_model.py
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.400230 rococo_test-1.0.2/rococo/repositories/
+-rw-r--r--   0 kote       (501) staff       (20)       43 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/repositories/__init__.py
+-rw-r--r--   0 kote       (501) staff       (20)     3351 2024-05-14 00:36:03.000000 rococo_test-1.0.2/rococo/repositories/base_repository.py
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.400625 rococo_test-1.0.2/rococo/repositories/mongodb/
+-rw-r--r--   0 kote       (501) staff       (20)        0 2024-05-09 14:11:44.000000 rococo_test-1.0.2/rococo/repositories/mongodb/__init__.py
+-rw-r--r--   0 kote       (501) staff       (20)     5478 2024-05-19 11:21:34.000000 rococo_test-1.0.2/rococo/repositories/mongodb/mongodb_repository.py
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.401448 rococo_test-1.0.2/rococo/repositories/mysql/
+-rw-r--r--   0 kote       (501) staff       (20)       46 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/repositories/mysql/__init__.py
+-rw-r--r--   0 kote       (501) staff       (20)    12602 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/repositories/mysql/mysql_repository.py
+-rw-r--r--   0 kote       (501) staff       (20)      666 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/repositories/mysql/organization_repository.py
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.402663 rococo_test-1.0.2/rococo/repositories/surrealdb/
+-rw-r--r--   0 kote       (501) staff       (20)      287 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/repositories/surrealdb/__init__.py
+-rw-r--r--   0 kote       (501) staff       (20)      687 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/repositories/surrealdb/organization_repository.py
+-rw-r--r--   0 kote       (501) staff       (20)     1879 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/repositories/surrealdb/person_organization_role_repository.py
+-rw-r--r--   0 kote       (501) staff       (20)    12105 2024-05-05 21:58:39.000000 rococo_test-1.0.2/rococo/repositories/surrealdb/surreal_db_repository.py
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.405401 rococo_test-1.0.2/rococo_test.egg-info/
+-rw-r--r--   0 kote       (501) staff       (20)    28901 2024-05-19 11:22:42.000000 rococo_test-1.0.2/rococo_test.egg-info/PKG-INFO
+-rw-r--r--   0 kote       (501) staff       (20)     1985 2024-05-19 11:22:42.000000 rococo_test-1.0.2/rococo_test.egg-info/SOURCES.txt
+-rw-r--r--   0 kote       (501) staff       (20)        1 2024-05-19 11:22:42.000000 rococo_test-1.0.2/rococo_test.egg-info/dependency_links.txt
+-rw-r--r--   0 kote       (501) staff       (20)       80 2024-05-19 11:22:42.000000 rococo_test-1.0.2/rococo_test.egg-info/requires.txt
+-rw-r--r--   0 kote       (501) staff       (20)       13 2024-05-19 11:22:42.000000 rococo_test-1.0.2/rococo_test.egg-info/top_level.txt
+-rw-r--r--   0 kote       (501) staff       (20)       38 2024-05-19 11:22:42.406453 rococo_test-1.0.2/setup.cfg
+-rw-r--r--   0 kote       (501) staff       (20)      639 2024-05-19 11:22:41.000000 rococo_test-1.0.2/setup.py
+drwxr-xr-x   0 kote       (501) staff       (20)        0 2024-05-19 11:22:42.405050 rococo_test-1.0.2/tests/
+-rw-r--r--   0 kote       (501) staff       (20)        0 2024-05-05 21:58:39.000000 rococo_test-1.0.2/tests/__init__.py
+-rw-r--r--   0 kote       (501) staff       (20)     5290 2024-05-13 22:53:08.000000 rococo_test-1.0.2/tests/base_repository_test.py
+-rw-r--r--   0 kote       (501) staff       (20)     2007 2024-05-05 21:58:39.000000 rococo_test-1.0.2/tests/config_test.py
+-rw-r--r--   0 kote       (501) staff       (20)     2241 2024-05-05 21:58:39.000000 rococo_test-1.0.2/tests/model_test.py
+-rw-r--r--   0 kote       (501) staff       (20)     2493 2024-05-15 01:11:02.000000 rococo_test-1.0.2/tests/mongodb_repository_test.py
+-rw-r--r--   0 kote       (501) staff       (20)     3004 2024-05-13 20:46:54.000000 rococo_test-1.0.2/tests/surreal_db_repository_test.py
```

### Comparing `rococo_test-1.0.1/LICENSE` & `rococo_test-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/PKG-INFO` & `rococo_test-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rococo_test
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python library to help build things the way we want them built
 Author: Jay Grieves
 Author-email: jaygrieves@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rococo_test-1.0.1/README.md` & `rococo_test-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/auth/tokens.py` & `rococo_test-1.0.2/rococo/auth/tokens.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/config/config.py` & `rococo_test-1.0.2/rococo/config/config.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/data/base.py` & `rococo_test-1.0.2/rococo/data/base.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/data/mongodb.py` & `rococo_test-1.0.2/rococo/data/mongodb.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/data/mysql.py` & `rococo_test-1.0.2/rococo/data/mysql.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/data/surrealdb.py` & `rococo_test-1.0.2/rococo/data/surrealdb.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/emailing/config.py` & `rococo_test-1.0.2/rococo/emailing/config.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/emailing/factory.py` & `rococo_test-1.0.2/rococo/emailing/factory.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/emailing/mailjet.py` & `rococo_test-1.0.2/rococo/emailing/mailjet.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/messaging/base.py` & `rococo_test-1.0.2/rococo/messaging/base.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/messaging/rabbitmq.py` & `rococo_test-1.0.2/rococo/messaging/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/messaging/sqs.py` & `rococo_test-1.0.2/rococo/messaging/sqs.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/models/login_method.py` & `rococo_test-1.0.2/rococo/models/login_method.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/models/organization.py` & `rococo_test-1.0.2/rococo/models/organization.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/models/person_organization_role.py` & `rococo_test-1.0.2/rococo/models/person_organization_role.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/models/surrealdb/login_method.py` & `rococo_test-1.0.2/rococo/models/surrealdb/login_method.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/models/surrealdb/organization.py` & `rococo_test-1.0.2/rococo/models/surrealdb/organization.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/models/surrealdb/person_organization_role.py` & `rococo_test-1.0.2/rococo/models/surrealdb/person_organization_role.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/models/surrealdb/surreal_versioned_model.py` & `rococo_test-1.0.2/rococo/models/surrealdb/surreal_versioned_model.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/models/versioned_model.py` & `rococo_test-1.0.2/rococo/models/versioned_model.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/repositories/base_repository.py` & `rococo_test-1.0.2/rococo/repositories/base_repository.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/repositories/mongodb/mongodb_repository.py` & `rococo_test-1.0.2/rococo/repositories/mongodb/mongodb_repository.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,15 +23,14 @@
             db_adapter: MongoDBAdapter,
             model: Type[VersionedModel],
             message_adapter: MessageAdapter,
             queue_name: str,
             user_id: UUID = None
     ):
         super().__init__(db_adapter, model, message_adapter, queue_name, user_id=user_id)
-        self.db = db_adapter.db
 
 
     def _process_data_before_save(self, instance: VersionedModel):
         """Method to convert VersionedModel instance to a data dictionary that can be inserted in MongoDB"""
         super()._process_data_before_save(instance)
         data = instance.as_dict(convert_datetime_to_iso_string=False, convert_uuids=True)
         for field in fields(instance):
@@ -54,15 +53,15 @@
 
             data[field.name] = field_value
         return data
 
     def get_move_entity_to_audit_table_query(self, table, entity_id):
         instance = self.get_one(table, "", {'entity_id': entity_id})
         if instance:
-            self.db[f"{table}_audit"].insert_one(instance)
+            self._insert(instance, f"{table}_audit")
     
     def get_save_query(self, table, data):
         self.db[table].find_one_and_update(
             {'entity_id': data.get("entity_id")},
             {'$set': data},
         )
     
@@ -74,15 +73,16 @@
             if send_message:
                 # This assumes that the instance is now in post-saved state with all the new DB updates
                 message = json.dumps(instance.as_dict(convert_datetime_to_iso_string=True))
                 self.message_adapter.send_message(self.queue_name, message)
         return instance
 
     def _insert(self, data: Dict, collection_name: str):
-        self.db[collection_name].insert_one(data)
+        with self.adapter:
+            self.db[collection_name].insert_one(data)
 
     def create(self, data: Dict, collection_name: str):
         return self.update(data, collection_name)
 
     def create_many(self, data: List[Dict], collection_name: str):
         documents = []
         for item in data:
@@ -105,29 +105,30 @@
 
     def get_one(self, collection_name: str, index: str, query: Dict):
         base_query = {'latest': True, 'active': True}
         if query:
             base_query.update(query)
 
         kwargs = {"hint": index} if index else {}
-        data = self.db[collection_name].find_one(base_query, **kwargs)
-        if data:
-            return data
+        with self.adapter:
+            data = self.db[collection_name].find_one(base_query, **kwargs)
+            if data:
+                return data
             
 
     def get_all(self, collection_name: str, index: str, query: Dict = None):
         base_query = {'latest': True, 'active': True}
         if query:
             base_query.update(query)
-
-        data = self.db[collection_name].find(
-            base_query, hint=index
-        )
-        if data:
-            return data
+        with self.adapter:
+            data = self.db[collection_name].find(
+                base_query, hint=index
+            )
+            if data:
+                return data
         return []
 
     def get_count(self, collection_name: str, index: str, query: Dict):
         query.update(dict(latest=True, active=True))
         return self.db[collection_name].count_documents(query, hint=index)
 
     def create_index(self, collection_name: str, columns: List, index_name: str, partial_filter: Dict):
```

### Comparing `rococo_test-1.0.1/rococo/repositories/mysql/mysql_repository.py` & `rococo_test-1.0.2/rococo/repositories/mysql/mysql_repository.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/repositories/mysql/organization_repository.py` & `rococo_test-1.0.2/rococo/repositories/mysql/organization_repository.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/repositories/surrealdb/organization_repository.py` & `rococo_test-1.0.2/rococo/repositories/surrealdb/organization_repository.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/repositories/surrealdb/person_organization_role_repository.py` & `rococo_test-1.0.2/rococo/repositories/surrealdb/person_organization_role_repository.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo/repositories/surrealdb/surreal_db_repository.py` & `rococo_test-1.0.2/rococo/repositories/surrealdb/surreal_db_repository.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/rococo_test.egg-info/PKG-INFO` & `rococo_test-1.0.2/rococo_test.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rococo_test
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python library to help build things the way we want them built
 Author: Jay Grieves
 Author-email: jaygrieves@gmail.com
 License: MIT
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `rococo_test-1.0.1/rococo_test.egg-info/SOURCES.txt` & `rococo_test-1.0.2/rococo_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/setup.py` & `rococo_test-1.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='rococo_test',
-    version='1.0.1',
+    version='1.0.2',
     packages=find_packages(),
     # url='https://github.com/EcorRouge/rococo',
     license='MIT',
     author='Jay Grieves',
     author_email='jaygrieves@gmail.com',
     description='A Python library to help build things the way we want them built',
     long_description=open('README.md').read(),
```

### Comparing `rococo_test-1.0.1/tests/base_repository_test.py` & `rococo_test-1.0.2/tests/base_repository_test.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/tests/config_test.py` & `rococo_test-1.0.2/tests/config_test.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/tests/model_test.py` & `rococo_test-1.0.2/tests/model_test.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/tests/mongodb_repository_test.py` & `rococo_test-1.0.2/tests/mongodb_repository_test.py`

 * *Files identical despite different names*

### Comparing `rococo_test-1.0.1/tests/surreal_db_repository_test.py` & `rococo_test-1.0.2/tests/surreal_db_repository_test.py`

 * *Files identical despite different names*

