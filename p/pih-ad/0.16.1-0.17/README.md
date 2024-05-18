# Comparing `tmp/pih-ad-0.16.1.tar.gz` & `tmp/pih-ad-0.17.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pih-ad-0.16.1.tar", last modified: Wed May 15 03:55:57 2024, max compression
+gzip compressed data, was "pih-ad-0.17.tar", last modified: Sat May 18 23:46:56 2024, max compression
```

## Comparing `pih-ad-0.16.1.tar` & `pih-ad-0.17.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 03:55:57.416124 pih-ad-0.16.1/
-drwxrwxrwx   0        0        0        0 2024-05-15 03:55:56.648331 pih-ad-0.16.1/ActiveDirectoryService/
--rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-ad-0.16.1/ActiveDirectoryService/__init__.py
--rw-rw-rw-   0        0        0      157 2024-02-10 00:14:06.000000 pih-ad-0.16.1/ActiveDirectoryService/__main__.py
--rw-rw-rw-   0        0        0    18164 2024-05-15 03:51:22.000000 pih-ad-0.16.1/ActiveDirectoryService/api.py
--rw-rw-rw-   0        0        0     1582 2024-05-15 03:55:38.000000 pih-ad-0.16.1/ActiveDirectoryService/const.py
--rw-rw-rw-   0        0        0    15731 2024-05-15 03:55:33.000000 pih-ad-0.16.1/ActiveDirectoryService/service.py
--rw-rw-rw-   0        0        0      342 2024-05-15 03:55:57.384892 pih-ad-0.16.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-05-15 03:55:57.338004 pih-ad-0.16.1/pih_ad.egg-info/
--rw-rw-rw-   0        0        0      342 2024-05-15 03:55:56.000000 pih-ad-0.16.1/pih_ad.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      347 2024-05-15 03:55:56.000000 pih-ad-0.16.1/pih_ad.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 03:55:56.000000 pih-ad-0.16.1/pih_ad.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       65 2024-05-15 03:55:56.000000 pih-ad-0.16.1/pih_ad.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       22 2024-05-15 03:55:56.000000 pih-ad-0.16.1/pih_ad.egg-info/requires.txt
--rw-rw-rw-   0        0        0       23 2024-05-15 03:55:56.000000 pih-ad-0.16.1/pih_ad.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 03:55:57.431751 pih-ad-0.16.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-18 23:46:56.208669 pih-ad-0.17/
+drwxrwxrwx   0        0        0        0 2024-05-18 23:46:55.752679 pih-ad-0.17/ActiveDirectoryService/
+-rw-rw-rw-   0        0        0        0 2022-08-10 08:09:48.000000 pih-ad-0.17/ActiveDirectoryService/__init__.py
+-rw-rw-rw-   0        0        0      157 2024-02-10 00:14:06.000000 pih-ad-0.17/ActiveDirectoryService/__main__.py
+-rw-rw-rw-   0        0        0    18268 2024-05-18 23:42:52.000000 pih-ad-0.17/ActiveDirectoryService/api.py
+-rw-rw-rw-   0        0        0     1580 2024-05-18 23:43:40.000000 pih-ad-0.17/ActiveDirectoryService/const.py
+-rw-rw-rw-   0        0        0    15696 2024-05-18 23:46:38.000000 pih-ad-0.17/ActiveDirectoryService/service.py
+-rw-rw-rw-   0        0        0      340 2024-05-18 23:46:56.161835 pih-ad-0.17/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-05-18 23:46:56.083679 pih-ad-0.17/pih_ad.egg-info/
+-rw-rw-rw-   0        0        0      340 2024-05-18 23:46:55.000000 pih-ad-0.17/pih_ad.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-05-18 23:46:55.000000 pih-ad-0.17/pih_ad.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-18 23:46:55.000000 pih-ad-0.17/pih_ad.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       65 2024-05-18 23:46:55.000000 pih-ad-0.17/pih_ad.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       22 2024-05-18 23:46:55.000000 pih-ad-0.17/pih_ad.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       23 2024-05-18 23:46:55.000000 pih-ad-0.17/pih_ad.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-18 23:46:56.224304 pih-ad-0.17/setup.cfg
```

### Comparing `pih-ad-0.16.1/ActiveDirectoryService/api.py` & `pih-ad-0.17/ActiveDirectoryService/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from collections import defaultdict
 from pyad.adcomputer import ADComputer
 from pyad.adcontainer import ADContainer
 from pyad.adgroup import ADObject, ADGroup
 
 import ipih
 
-from pih import A
+from pih import A, strdict
 from pih.consts.errors import NotAccesable
 from pih.collections import FullName, User
 from ActiveDirectoryService.const import *
 from pih.tools import if_else, j, n, nn, lw, ne, escs
 
 
 class ActiveDirectoryApi:
@@ -68,15 +68,15 @@
         query_result = [] if ad_query.get_row_count() == 0 else ad_query.get_results()
         result: list[dict[str, str]] = []
         for item in query_result:
             result.append(item)
         return result
 
     @staticmethod
-    def get_computer_description_list(dn: str) -> list[dict[str, Any]]:
+    def get_computer_description_list(dn: str) -> list[strdict]:
         property_container: ADContainer = ADContainer.from_dn(
             A.CT_AD.PROPERTY_COMPUTER_DN
         )
         property_list: list[ADGroup] = property_container.get_children(False)
         computer_property_map: dict[str, int] = defaultdict(int)
         property_item: ADGroup
         for property_item in property_list:
@@ -89,31 +89,32 @@
             property_member_item: ADObject
             for property_member_item in property_member_list:
                 computer_property_map[property_member_item.name] |= ws_property.value
         ad_query: ADQuery = ADQuery()
         name_field_name: str = A.CT_FNC.NAME
         description_field_name: str = A.CT_FNC.DESCRIPTION
         ad_query.execute_query(
-            attributes=[name_field_name, description_field_name],
+            attributes=[name_field_name, description_field_name, A.CT_FNC.DN],
             base_dn=dn,
             where_clause="objectClass = 'computer'",
         )
         query_result: list = (
             [] if ad_query.get_row_count() == 0 else ad_query.get_results()
         )
-        result: list[dict[str, Any]] = []
+        result: list[strdict] = []
         for query_item in query_result:
-            query_item[A.CT_FNC.PROPERTIES] = computer_property_map[
-                query_item[name_field_name]
-            ]
-            query_item[description_field_name] = A.D.get_first_item(
-                query_item[description_field_name]
-            )
-            query_item[A.CT_FNC.DN] = dn
-            result.append(query_item)
+            if query_item[A.CT_FNC.DN].find(A.CT_AD.INCATIVE_OU_NAME) == -1:
+                query_item[A.CT_FNC.PROPERTIES] = computer_property_map[
+                    query_item[name_field_name]
+                ]
+                query_item[description_field_name] = A.D.get_first_item(
+                    query_item[description_field_name]
+                )
+                query_item[A.CT_FNC.DN] = dn
+                result.append(query_item)
         return result
 
     @staticmethod
     def get_user_existance_status_for_child_in_user_home_directory() -> (
         list[UserExistanceStatusItem]
     ):
         return ActiveDirectoryApi.get_user_existance_status_for_child_in_directory(
@@ -217,15 +218,15 @@
     @staticmethod
     def query_by(
         search_attribute: str,
         search_value: str,
         fields: list[str],
         base_dn: str = A.CT_AD.ACTIVE_USERS_CONTAINER_DN,
         ad_query=DEFAULT_AD_QUERY,
-    ) -> dict[str, Any] | None:
+    ) -> strdict | None:
         if search_attribute.find("name") != -1:
             if search_value != A.CT_AD.SEARCH_ALL_PATTERN:
                 search_value = j((A.CT_AD.SEARCH_ALL_PATTERN, search_value, A.CT_AD.SEARCH_ALL_PATTERN))
         if search_value == "":
             search_value = A.CT_AD.SEARCH_ALL_PATTERN
         ad_query.execute_query(
             attributes=fields,
@@ -233,15 +234,15 @@
             where_clause=f"objectClass = 'user' and objectCategory = 'person' and {search_attribute} = '{search_value}'",
         )
         if ad_query.get_row_count() == 0:
             return None
         return ad_query.get_results()
 
     @staticmethod
-    def find_by_in_dn(attribute: str, value: str, base_dn: str) -> list[dict[str, Any]]:
+    def find_by_in_dn(attribute: str, value: str, base_dn: str) -> list[strdict]:
         fields: list[str] = A.CT_FC.AD.USER.get_name_list()
         query_result = (
             ActiveDirectoryApi.query_by(attribute, value, fields, base_dn) or []
         )
         result: list[dict] = []
         for query_item in query_result:
             result_item: dict = {}
```

### Comparing `pih-ad-0.16.1/ActiveDirectoryService/const.py` & `pih-ad-0.17/ActiveDirectoryService/const.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 from pih.collections.service import ServiceDescription
 
 
 NAME: str = "ActiveDirectory"
 
 HOST = Hosts.DC2
 
-VERSION: str = "0.16.1"
+VERSION: str = "0.17"
 
 PACKAGES: tuple[str, ...] = ("pyad", "pywin32", "wmi")
 
 SD: ServiceDescription = ServiceDescription(
     name=NAME,
     description="Active directory service",
     host=HOST.NAME,
```

### Comparing `pih-ad-0.16.1/ActiveDirectoryService/service.py` & `pih-ad-0.17/ActiveDirectoryService/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -53,16 +53,15 @@
                 if sc == SC.get_user_by_full_name:
                     return get_user_by_attribute(
                         A.CT_FNC.SEARCH_ATTRIBUTE_NAME,
                         A.D.fullname_to_string(pl.next(FullName())),
                         pl.next(),
                     )
                 if sc == SC.get_users_by_name:
-                    value: str | None = pl.next()
-                    value = lw(value)
+                    value: str | None = lw(pl.next())
                     active: bool | None = pl.next()
                     cached: bool | None = pl.next()
                     strict_comparison: bool | None = pl.next()
                     cached = A.D.check_not_none(cached, cached, A.S_U.use_cache())
                     if cached:
                         user_cache_list: list[strdict] = A.D.as_list(DH.user_cache)
```

