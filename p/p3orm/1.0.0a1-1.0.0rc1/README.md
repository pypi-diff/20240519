# Comparing `tmp/p3orm-1.0.0a1.tar.gz` & `tmp/p3orm-1.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "p3orm-1.0.0a1.tar", max compression
+gzip compressed data, was "p3orm-1.0.0rc1.tar", max compression
```

## Comparing `p3orm-1.0.0a1.tar` & `p3orm-1.0.0rc1.tar`

### file list

```diff
@@ -1,12 +1,13 @@
--rw-r--r--   0        0        0     1081 2023-12-22 22:03:07.068553 p3orm-1.0.0a1/LICENSE
--rw-r--r--   0        0        0     3598 2023-12-22 22:03:07.068553 p3orm-1.0.0a1/README.md
--rw-r--r--   0        0        0       30 2023-12-22 22:03:07.080553 p3orm-1.0.0a1/p3orm/__init__.py
--rw-r--r--   0        0        0        0 2023-12-22 22:03:07.080553 p3orm-1.0.0a1/p3orm/drivers/__init__.py
--rw-r--r--   0        0        0     1497 2023-12-22 22:03:07.080553 p3orm-1.0.0a1/p3orm/drivers/base.py
--rw-r--r--   0        0        0    11446 2023-12-22 22:03:07.080553 p3orm-1.0.0a1/p3orm/drivers/postgres.py
--rw-r--r--   0        0        0      150 2023-12-22 22:03:07.080553 p3orm-1.0.0a1/p3orm/exceptions.py
--rw-r--r--   0        0        0        0 2023-12-22 22:03:07.080553 p3orm-1.0.0a1/p3orm/py.typed
--rw-r--r--   0        0        0     7192 2023-12-22 22:03:07.080553 p3orm-1.0.0a1/p3orm/table.py
--rw-r--r--   0        0        0     2956 2023-12-22 22:03:07.080553 p3orm-1.0.0a1/p3orm/utils.py
--rw-r--r--   0        0        0     2048 2023-12-22 22:03:07.080553 p3orm-1.0.0a1/pyproject.toml
--rw-r--r--   0        0        0     4457 1970-01-01 00:00:00.000000 p3orm-1.0.0a1/PKG-INFO
+-rw-r--r--   0        0        0     1081 2024-05-19 01:49:08.353168 p3orm-1.0.0rc1/LICENSE
+-rw-r--r--   0        0        0     3598 2024-05-19 01:49:08.353168 p3orm-1.0.0rc1/README.md
+-rw-r--r--   0        0        0      335 2024-05-19 01:49:08.365168 p3orm-1.0.0rc1/p3orm/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-19 01:49:08.365168 p3orm-1.0.0rc1/p3orm/drivers/__init__.py
+-rw-r--r--   0        0        0      358 2024-05-19 01:49:08.365168 p3orm-1.0.0rc1/p3orm/drivers/base.py
+-rw-r--r--   0        0        0    18366 2024-05-19 01:49:08.365168 p3orm-1.0.0rc1/p3orm/drivers/postgres.py
+-rw-r--r--   0        0        0      213 2024-05-19 01:49:08.365168 p3orm-1.0.0rc1/p3orm/exceptions.py
+-rw-r--r--   0        0        0     2867 2024-05-19 01:49:08.365168 p3orm-1.0.0rc1/p3orm/fields.py
+-rw-r--r--   0        0        0        0 2024-05-19 01:49:08.365168 p3orm-1.0.0rc1/p3orm/py.typed
+-rw-r--r--   0        0        0     7970 2024-05-19 01:49:08.365168 p3orm-1.0.0rc1/p3orm/table.py
+-rw-r--r--   0        0        0     4219 2024-05-19 01:49:08.365168 p3orm-1.0.0rc1/p3orm/utils.py
+-rw-r--r--   0        0        0     1965 2024-05-19 01:49:08.365168 p3orm-1.0.0rc1/pyproject.toml
+-rw-r--r--   0        0        0     4266 1970-01-01 00:00:00.000000 p3orm-1.0.0rc1/PKG-INFO
```

### Comparing `p3orm-1.0.0a1/LICENSE` & `p3orm-1.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `p3orm-1.0.0a1/README.md` & `p3orm-1.0.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `p3orm-1.0.0a1/p3orm/table.py` & `p3orm-1.0.0rc1/p3orm/table.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,134 +1,162 @@
 from __future__ import annotations
 
+import dataclasses
 import typing
 from dataclasses import dataclass
-from typing import TYPE_CHECKING, Any, ClassVar, Type, get_args
+from typing import TYPE_CHECKING, Any, Callable, ClassVar, Generator, Generic, Type, TypeVar, get_args
 
-import attrs
-import pypika
 from pypika.dialects import PostgreSQLQueryBuilder
+from pypika.terms import Field as PyPikaField
 
-from p3orm.exceptions import MisingPrimaryKeyException, MissingTablename, P3ormException
+from p3orm.exceptions import (
+    MisingPrimaryKeyException,
+    MissingTablename,
+    P3ormException,
+    UnloadedRelationshipException,
+)
 from p3orm.fields import PormField, PormRelationship, RelationshipType
 from p3orm.utils import is_optional
 
 if TYPE_CHECKING:
-    from p3orm.drivers.base import Driver
+    from p3orm import Driver
+
+T = TypeVar("T", bound="Table")
 
 
 class TableMemo:
     table: Type[Table]
     pk: list[PormField]
     fields: dict[str, PormField]
     columns: dict[str, PormField]
-    relationships: dict[str, PormRelationship]
-    factory: Type
+    relationships: dict[str, PormRelationship[Any]]
+    factory: Type[Any]
     record_t_kwarg_map: dict[str, str]
     record_kwarg_map: dict[str, str]
     driver: Driver
 
 
 TABLES: dict[Type[Table], TableMemo] = {}
 
 
-def querybuilder():
+def querybuilder() -> PostgreSQLQueryBuilder:
     return PostgreSQLQueryBuilder()
 
 
 @dataclass
-class UNLOADED_RELATIONSIP[T]:
+class UNLOADED_RELATIONSHIP(Generic[T]):
     name: str
     data_type: Type[T]
 
+    def __get__(self, _: Table, owner: Type[Table]):
+        raise UnloadedRelationshipException(f"<{owner}> relationship {self.name=} not loaded")
+
     def __repr__(self) -> str:
         name = self.name
-        # if is_optional(self.data_type):
-        #     type = self.data_type
-        # else:
-        #     type = self.data_type.__name__
         type = self.data_type
 
         return f"<UNLOADED RELATIONSHIP {name=} {type=}>"
 
+    def __bool__(self) -> bool:
+        return False
+
 
 @dataclass
-class DB_GENERATED[T]:
+class DB_GENERATED(Generic[T]):
     name: str
     column: str
     data_type: Type[T]
 
     def __repr__(self) -> str:
-        name = self.name
+        table = self.name
         column = self.column
-        # if is_optional(self.data_type):
-        #     type = self.data_type
-        # else:
-        #     type = self.data_type.__name__
         type = self.data_type
 
-        return f"<DB WILL SET VALUE {name=} {column=} {type=}>"
+        return f"<DB WILL SET VALUE {table=} {column=} {type=}>"
 
 
 @typing.dataclass_transform()
 class TableMeta(type):
-    def from_(cls: Type[Table]) -> PostgreSQLQueryBuilder:
+    def from_(cls: Type[Table]) -> PostgreSQLQueryBuilder:  # type: ignore
         return querybuilder().from_(cls.__tablename__)
 
-    def select(cls: Type[Table]) -> PostgreSQLQueryBuilder:
-        return cls.from_().select("*")
+    def select(cls: Type[Table], what: Any = None) -> PostgreSQLQueryBuilder:  # type: ignore
+        return cls.from_().select(what or "*")
 
-    def delete(cls: Type[Table]) -> PostgreSQLQueryBuilder:
+    def delete(cls: Type[Table]) -> PostgreSQLQueryBuilder:  # type: ignore
         return querybuilder().delete().from_(cls.__tablename__)
 
-    def update(cls: Type[Table]) -> PostgreSQLQueryBuilder:
+    def update(cls: Type[Table]) -> PostgreSQLQueryBuilder:  # type: ignore
         return querybuilder().update(cls.__tablename__)
 
 
+# we need to check instead of checking directly because a __meta__ = True class
+# will pass that down to all children. so we determine if __meta__ is set on the
+# class itself, not on any parents, and then use that to determine
+# tl;dr table is meta if that class, and that class specifically, has __meta__ set to True
+def _is_meta_table(cls: Type[Table]) -> bool:
+    if hasattr(cls, "__meta__"):
+        if "__meta__" in cls.__dict__:
+            return cls.__dict__["__meta__"]
+
+    return False
+
+
+def create_dataclass(
+    class_name: str,
+    fields: list[str | tuple[str, type] | tuple[str, type, dataclasses.Field]],
+) -> type:
+    return dataclasses.make_dataclass(
+        class_name,
+        fields,
+        slots=True,
+        match_args=True,
+        kw_only=True,
+    )
+
+
+"""
+def create_factory(
+    class_name: str,
+    fields: list[str | tuple[str, type] | tuple[str, type, Any]],
+):
+    def __init__(self, **kwargs):
+        init_kwargs = {}
+        for field in fields:
+            match field:
+                case str(field_name):
+                    ...
+                case (field_name, field_type):
+                    ...
+                case (field_name, field_type, field_default):
+                    ...
+"""
+
+
 class Table(metaclass=TableMeta):
     __tablename__: ClassVar[str]
     __meta__: ClassVar[bool] = False
 
     __memo__: ClassVar[TableMemo]
 
-    # @classmethod
-    # async def fetch_one[T](cls: Type[T | Self], /, criterion: Criterion) -> T:
-    #     parameterized_criterion, query_args = parameterize(criterion)
-    #
-    #     query: QueryBuilder = cls.select().where(parameterized_criterion)
-    #     query = query.limit(2)
-    #
-    def __new__(cls, /, **create_fields: dict[str, Any]):
+    def __new__(cls, /, **create_fields: dict[str, Any]):  # type: ignore
+        # TODO: cython? teehee
         if not (hasattr(cls, "__memo__") and (memo := cls.__memo__)):
             raise P3ormException(f"table {cls} not initalized")
 
-        obj = memo.factory(**create_fields)
-        for field_name, field in memo.fields.items():
-            if field.db_gen:
-                setattr(
-                    obj,
-                    field_name,
-                    DB_GENERATED[field._data_type](
-                        name=field_name,
-                        column=field.column_name,
-                        data_type=field._data_type,
-                    ),
-                )
+        return memo.factory(**create_fields)
 
-        for field_name, relationship in memo.relationships.items():
-            setattr(
-                obj,
-                field_name,
-                UNLOADED_RELATIONSIP[relationship._data_type](
-                    name=field_name,
-                    data_type=relationship._data_type,
-                ),
-            )
+    @classmethod
+    def __validate(cls, v: Table | Any, _) -> Table:
+        assert cls.__name__ == v.__class__.__name__, f"must be a valid {cls.__name__}"
+        return v
 
-        return obj
+    @classmethod
+    def __get_validators__(cls) -> Generator[Callable, None, None]:
+        yield cls.__validate
 
     @classmethod
     def _init_stuff(cls, driver: Driver) -> TableMemo:
         memo = TableMemo()
         memo.table = cls
         memo.driver = driver
         memo.fields = {}
@@ -146,78 +174,72 @@
                 if isinstance(field := getattr(table, field_name), PormField):
                     field._field_name = field_name
                     field._data_type = type_hints[field_name]
 
                     if not hasattr(field, "column_name"):
                         field.column_name = field_name
 
-                    field._pypika_field = pypika.Field(
-                        name=field.column_name,
-                        table=pypika.Table(cls.__tablename__),
-                    )
+                    field._pypika_field = PyPikaField(name=field.column_name)
 
                     memo.fields[field_name] = field
                     memo.columns[field.column_name] = field
                     memo.record_kwarg_map[field.column_name] = field_name
                     memo.record_t_kwarg_map[f"{cls.__tablename__}.{field.column_name}"] = field_name
 
                     if field.pk:
                         memo.pk.append(field)
 
                 elif isinstance(relationship := getattr(cls, field_name), PormRelationship):
-                    if relationship.relationship_type == RelationshipType.foreign_key:
+                    if relationship.relationship_type in (RelationshipType.foreign_key, RelationshipType.reverse_one):
                         relationship._data_type = type_hints[field_name]
                     else:
                         relationship._data_type = get_args(type_hints[field_name])[0]
 
                     relationship._field_name = field_name
                     memo.relationships[field_name] = relationship
 
         if len(memo.pk) == 0:
             raise MisingPrimaryKeyException(f"{cls.__name__} must have at least 1 column to uniquely identify rows")
 
         # tack on the model factory
-        factory_fields: dict[str, attrs.Attribute] = {}
+        factory_fields: list[str | tuple[str, type] | tuple[str, type, dataclasses.Field]] = []
         for field_name, field in memo.fields.items():
-            field_kwargs = {}
-            field_kwargs["type"] = field._data_type
+            field_opts = [field_name, field._data_type]
 
             if field.db_default or field.db_gen:
-                field_kwargs["default"] = DB_GENERATED[field._data_type](
-                    name=field_name, column=field.column_name, data_type=field._data_type
+                field_opts.append(
+                    dataclasses.field(
+                        default_factory=lambda: DB_GENERATED[field._data_type](
+                            name=field_name, column=field.column_name, data_type=field._data_type
+                        )
+                    )
                 )
             elif is_optional(field._data_type):
-                field_kwargs["default"] = None
+                field_opts.append(dataclasses.field(default=None))
 
-            factory_fields[field_name] = attrs.field(**field_kwargs)
+            factory_fields.append(tuple(field_opts))
 
         for field_name, relationship in memo.relationships.items():
-            factory_fields[field_name] = attrs.field(
-                type=relationship._data_type,
-                default=UNLOADED_RELATIONSIP[relationship._data_type](
-                    name=field_name, data_type=relationship._data_type
-                ),
+            factory_fields.append(
+                (
+                    field_name,
+                    relationship._data_type,
+                    dataclasses.field(
+                        default_factory=lambda: UNLOADED_RELATIONSHIP[relationship._data_type](  # type: ignore -> typeshed says this returns T, but it returns Field[T]
+                            name=field_name, data_type=relationship._data_type
+                        )
+                    ),
+                )
             )
 
-        memo.factory = attrs.make_class(
-            name=cls.__name__,
-            attrs=factory_fields,
-            kw_only=True,
-            slots=True,
-        )
+        memo.factory = create_dataclass(cls.__name__, factory_fields)
 
         TABLES[cls] = memo
         cls.__memo__ = memo
-        print(f"SETTING {cls=} {cls.__memo__=}")
         return memo
 
     def __init_subclass__(cls) -> None:
-        if cls.__meta__:
+        if _is_meta_table(cls):
             return
 
         if not cls.__tablename__:
             raise MissingTablename(f"{cls} is missing a __tablename__ property")
-
-            # prepare all the criterion so they all know which table they belong to
-
-            # for field in fields:
-            ...
```

### Comparing `p3orm-1.0.0a1/pyproject.toml` & `p3orm-1.0.0rc1/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,47 @@
 [tool.poetry]
 name = "p3orm"
-version = "1.0.0-alpha.1"
-description = "Utilitarian Python ORM for Postgres/SQLite, backed by asyncpg/aiosqlite, Pydantic, and PyPika"
+version = "1.0.0rc1"
+description = "Utilitarian Python ORM for Postgres, backed by asyncpg and PyPika"
 authors = ["Rafal Stapinski <stapinskirafal@gmail.com>"]
-keywords = ["postgres", "sqlite", "async", "orm"]
+keywords = ["postgres", "async", "orm"]
 readme = "README.md"
 license = "MIT"
 homepage = "https://rafalstapinski.github.io/p3orm"
 repository = "https://github.com/rafalstapinski/p3orm"
-packages = [
-  {include = "p3orm"},
-  {include = "p3orm/py.typed"},
-]
+packages = [{ include = "p3orm" }, { include = "p3orm/py.typed" }]
 
 [tool.poetry.dependencies]
 python = "^3.12"
-attrs = "^23.1.0"
-asyncpg = {version = "^0.29.0", optional = true}
-aiosqlite = {version = "^0.19.0", optional = true}
+asyncpg = { version = "0.29.0" }
 pypika = "^0.48.9"
 
 [tool.poetry.extras]
-sqlite = ["aiosqlite"]
-postgres = ["asyncpg"]
+pydantic = ["pydantic"]
 
 [tool.poetry.group.dev.dependencies]
 tomli = "^2.0.1"
 asyncpg = "^0.29.0"
 aiosqlite = "^0.19.0"
 ruff = "^0.1.6"
 isort = "^5.12.0"
 mypy = "^1.7.1"
 black = "^23.12.0"
 pylint = "^3.0.3"
+pydantic = "^2.7.1"
 
 [tool.poetry.group.publish.dependencies]
 mkdocs = "^1.5.3"
 mkdocs-material = "^9.4.14"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^7.4.3"
 pytest-asyncio = "^0.21.1"
 pytest-postgresql = "^5.0.0"
-psycopg = {extras = ["binary"], version = "^3.1.13"}
+psycopg = { extras = ["binary"], version = "^3.1.13" }
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
 line-length = 120
@@ -85,7 +80,10 @@
 warn_unused_configs = true
 show_error_codes = true
 show_column_numbers = true
 ignore_missing_imports = false
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
+
+[tool.basedpyright]
+typeCheckingMode = "basic"
```

### Comparing `p3orm-1.0.0a1/PKG-INFO` & `p3orm-1.0.0rc1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,22 @@
 Metadata-Version: 2.1
 Name: p3orm
-Version: 1.0.0a1
-Summary: Utilitarian Python ORM for Postgres/SQLite, backed by asyncpg/aiosqlite, Pydantic, and PyPika
+Version: 1.0.0rc1
+Summary: Utilitarian Python ORM for Postgres, backed by asyncpg and PyPika
 Home-page: https://rafalstapinski.github.io/p3orm
 License: MIT
-Keywords: postgres,sqlite,async,orm
+Keywords: postgres,async,orm
 Author: Rafal Stapinski
 Author-email: stapinskirafal@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
-Provides-Extra: postgres
-Provides-Extra: sqlite
-Requires-Dist: aiosqlite (>=0.19.0,<0.20.0) ; extra == "sqlite"
-Requires-Dist: asyncpg (>=0.29.0,<0.30.0) ; extra == "postgres"
-Requires-Dist: attrs (>=23.1.0,<24.0.0)
+Provides-Extra: pydantic
+Requires-Dist: asyncpg (==0.29.0)
 Requires-Dist: pypika (>=0.48.9,<0.49.0)
 Project-URL: Repository, https://github.com/rafalstapinski/p3orm
 Description-Content-Type: text/markdown
 
 # p3orm
 
 <a href="https://rafalstapinski.github.io/p3orm">
```

