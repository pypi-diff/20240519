# Comparing `tmp/datayoga_core-1.98.0.tar.gz` & `tmp/datayoga_core-1.99.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datayoga_core-1.98.0.tar", max compression
+gzip compressed data, was "datayoga_core-1.99.0.tar", max compression
```

## Comparing `datayoga_core-1.98.0.tar` & `datayoga_core-1.99.0.tar`

### file list

```diff
@@ -1,104 +1,104 @@
--rw-r--r--   0        0        0     5118 2023-10-31 10:08:01.960775 datayoga_core-1.98.0/README.md
--rw-r--r--   0        0        0     2692 2023-10-31 10:08:21.372943 datayoga_core-1.98.0/pyproject.toml
--rw-r--r--   0        0        0     3558 2023-10-31 10:08:01.960775 datayoga_core-1.98.0/src/datayoga_core/__init__.py
--rw-r--r--   0        0        0     2900 2023-10-31 10:08:01.960775 datayoga_core-1.98.0/src/datayoga_core/block.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.960775 datayoga_core-1.98.0/src/datayoga_core/blocks/__init__.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.960775 datayoga_core-1.98.0/src/datayoga_core/blocks/add_field/__init__.py
--rw-r--r--   0        0        0     1548 2023-10-31 10:08:01.960775 datayoga_core-1.98.0/src/datayoga_core/blocks/add_field/block.py
--rw-r--r--   0        0        0     2062 2023-10-31 10:08:01.960775 datayoga_core-1.98.0/src/datayoga_core/blocks/add_field/block.schema.json
--rw-r--r--   0        0        0     3345 2023-10-31 10:08:01.960775 datayoga_core-1.98.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.960775 datayoga_core-1.98.0/src/datayoga_core/blocks/azure/read_event_hub/__init__.py
--rw-r--r--   0        0        0     4348 2023-10-31 10:08:01.960775 datayoga_core-1.98.0/src/datayoga_core/blocks/azure/read_event_hub/block.py
--rw-r--r--   0        0        0     1232 2023-10-31 10:08:01.960775 datayoga_core-1.98.0/src/datayoga_core/blocks/azure/read_event_hub/block.schema.json
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.960775 datayoga_core-1.98.0/src/datayoga_core/blocks/cassandra/__init__.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.960775 datayoga_core-1.98.0/src/datayoga_core/blocks/cassandra/write/__init__.py
--rw-r--r--   0        0        0     4609 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/cassandra/write/block.py
--rw-r--r--   0        0        0     1751 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/cassandra/write/block.schema.json
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/files/read_csv/__init__.py
--rw-r--r--   0        0        0     2023 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/files/read_csv/block.py
--rw-r--r--   0        0        0     1665 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/files/read_csv/block.schema.json
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/filter/__init__.py
--rw-r--r--   0        0        0     1100 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/filter/block.py
--rw-r--r--   0        0        0      464 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/filter/block.schema.json
--rw-r--r--   0        0        0     4200 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/filter/tests/test_filter.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/http/receiver/__init__.py
--rw-r--r--   0        0        0     1755 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/http/receiver/block.py
--rw-r--r--   0        0        0      468 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/http/receiver/block.schema.json
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/jinja_template/__init__.py
--rw-r--r--   0        0        0     1551 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/jinja_template/block.py
--rw-r--r--   0        0        0      571 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/jinja_template/block.schema.json
--rw-r--r--   0        0        0     2102 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/jinja_template/tests/test_jinja_template.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/map/__init__.py
--rw-r--r--   0        0        0     2517 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/map/block.py
--rw-r--r--   0        0        0     1167 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/map/block.schema.json
--rw-r--r--   0        0        0     6070 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/map/tests/test_map.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/parquet/__init__.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/parquet/read/__init__.py
--rw-r--r--   0        0        0     1115 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/parquet/read/block.py
--rw-r--r--   0        0        0      352 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/parquet/read/block.schema.json
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/parquet/write/__init__.py
--rw-r--r--   0        0        0     1271 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/parquet/write/block.py
--rw-r--r--   0        0        0      352 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/parquet/write/block.schema.json
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/redis/__init__.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/redis/lookup/__init__.py
--rw-r--r--   0        0        0     2566 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/redis/lookup/block.py
--rw-r--r--   0        0        0      888 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/redis/lookup/block.schema.json
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/redis/read_stream/__init__.py
--rw-r--r--   0        0        0     2589 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/redis/read_stream/block.py
--rw-r--r--   0        0        0      586 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json
--rw-r--r--   0        0        0     1947 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/redis/utils.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/redis/write/__init__.py
--rw-r--r--   0        0        0     2097 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/redis/write/block.py
--rw-r--r--   0        0        0      886 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/redis/write/block.schema.json
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/relational/__init__.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/relational/read/__init__.py
--rw-r--r--   0        0        0     1616 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/relational/read/block.py
--rw-r--r--   0        0        0     1315 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/relational/read/block.schema.json
--rw-r--r--   0        0        0     1669 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/relational/utils.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/relational/write/__init__.py
--rw-r--r--   0        0        0    10167 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/relational/write/block.py
--rw-r--r--   0        0        0     3312 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/relational/write/block.schema.json
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/remove_field/__init__.py
--rw-r--r--   0        0        0     1182 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/remove_field/block.py
--rw-r--r--   0        0        0     1182 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/remove_field/block.schema.json
--rw-r--r--   0        0        0     1893 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/rename_field/__init__.py
--rw-r--r--   0        0        0     1942 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/rename_field/block.py
--rw-r--r--   0        0        0     1716 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/rename_field/block.schema.json
--rw-r--r--   0        0        0     2279 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/sequence/__init__.py
--rw-r--r--   0        0        0      436 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/sequence/block.py
--rw-r--r--   0        0        0      517 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/sequence/block.schema.json
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/std/__init__.py
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/std/read/__init__.py
--rw-r--r--   0        0        0     1299 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/std/read/block.py
--rw-r--r--   0        0        0       75 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/std/read/block.schema.json
--rw-r--r--   0        0        0        0 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/std/write/__init__.py
--rw-r--r--   0        0        0      870 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/std/write/block.py
--rw-r--r--   0        0        0       76 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/blocks/std/write/block.schema.json
--rw-r--r--   0        0        0      337 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/context.py
--rw-r--r--   0        0        0     7581 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/expression.py
--rw-r--r--   0        0        0     8300 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/jmespath_custom_functions.py
--rw-r--r--   0        0        0    10326 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/job.py
--rw-r--r--   0        0        0      116 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/opcode.py
--rw-r--r--   0        0        0      739 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/producer.py
--rw-r--r--   0        0        0      522 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/prometheus.py
--rw-r--r--   0        0        0       23 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/resources/scaffold/.gitignore
--rw-r--r--   0        0        0      955 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/resources/scaffold/README.md
--rw-r--r--   0        0        0      151 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/resources/scaffold/connections.yaml
--rw-r--r--   0        0        0      188 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/resources/scaffold/data/sample.csv
--rw-r--r--   0        0        0      444 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/resources/scaffold/jobs/sample/hello.yaml
--rw-r--r--   0        0        0      981 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/resources/schemas/connections/cassandra.schema.json
--rw-r--r--   0        0        0     1169 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/resources/schemas/connections/mysql.schema.json
--rw-r--r--   0        0        0     1489 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/resources/schemas/connections/oracle.schema.json
--rw-r--r--   0        0        0     1270 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/resources/schemas/connections/postgresql.schema.json
--rw-r--r--   0        0        0     1272 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/resources/schemas/connections/redis.schema.json
--rw-r--r--   0        0        0     1009 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/resources/schemas/connections/sqlserver.schema.json
--rw-r--r--   0        0        0      981 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/resources/schemas/connections.schema.json
--rw-r--r--   0        0        0     1833 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/resources/schemas/job.schema.json
--rw-r--r--   0        0        0     1048 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/result.py
--rw-r--r--   0        0        0     5505 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/step.py
--rw-r--r--   0        0        0     2112 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/step_buffer.py
--rw-r--r--   0        0        0     4770 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/utils.py
--rw-r--r--   0        0        0     2485 2023-10-31 10:08:01.964775 datayoga_core-1.98.0/src/datayoga_core/write_utils.py
--rw-r--r--   0        0        0     8037 1970-01-01 00:00:00.000000 datayoga_core-1.98.0/PKG-INFO
+-rw-r--r--   0        0        0     5118 2023-10-31 12:57:35.748486 datayoga_core-1.99.0/README.md
+-rw-r--r--   0        0        0     2692 2023-10-31 12:57:53.828581 datayoga_core-1.99.0/pyproject.toml
+-rw-r--r--   0        0        0     3558 2023-10-31 12:57:35.748486 datayoga_core-1.99.0/src/datayoga_core/__init__.py
+-rw-r--r--   0        0        0     2900 2023-10-31 12:57:35.748486 datayoga_core-1.99.0/src/datayoga_core/block.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.748486 datayoga_core-1.99.0/src/datayoga_core/blocks/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.748486 datayoga_core-1.99.0/src/datayoga_core/blocks/add_field/__init__.py
+-rw-r--r--   0        0        0     1548 2023-10-31 12:57:35.748486 datayoga_core-1.99.0/src/datayoga_core/blocks/add_field/block.py
+-rw-r--r--   0        0        0     2062 2023-10-31 12:57:35.748486 datayoga_core-1.99.0/src/datayoga_core/blocks/add_field/block.schema.json
+-rw-r--r--   0        0        0     3345 2023-10-31 12:57:35.748486 datayoga_core-1.99.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.748486 datayoga_core-1.99.0/src/datayoga_core/blocks/azure/read_event_hub/__init__.py
+-rw-r--r--   0        0        0     4348 2023-10-31 12:57:35.748486 datayoga_core-1.99.0/src/datayoga_core/blocks/azure/read_event_hub/block.py
+-rw-r--r--   0        0        0     1232 2023-10-31 12:57:35.748486 datayoga_core-1.99.0/src/datayoga_core/blocks/azure/read_event_hub/block.schema.json
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.748486 datayoga_core-1.99.0/src/datayoga_core/blocks/cassandra/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.748486 datayoga_core-1.99.0/src/datayoga_core/blocks/cassandra/write/__init__.py
+-rw-r--r--   0        0        0     4609 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/cassandra/write/block.py
+-rw-r--r--   0        0        0     1751 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/cassandra/write/block.schema.json
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/files/read_csv/__init__.py
+-rw-r--r--   0        0        0     2023 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/files/read_csv/block.py
+-rw-r--r--   0        0        0     1665 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/files/read_csv/block.schema.json
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/filter/__init__.py
+-rw-r--r--   0        0        0     1100 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/filter/block.py
+-rw-r--r--   0        0        0      464 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/filter/block.schema.json
+-rw-r--r--   0        0        0     4200 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/filter/tests/test_filter.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/http/receiver/__init__.py
+-rw-r--r--   0        0        0     1755 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/http/receiver/block.py
+-rw-r--r--   0        0        0      468 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/http/receiver/block.schema.json
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/jinja_template/__init__.py
+-rw-r--r--   0        0        0     1551 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/jinja_template/block.py
+-rw-r--r--   0        0        0      571 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/jinja_template/block.schema.json
+-rw-r--r--   0        0        0     2102 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/jinja_template/tests/test_jinja_template.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/map/__init__.py
+-rw-r--r--   0        0        0     2517 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/map/block.py
+-rw-r--r--   0        0        0     1167 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/map/block.schema.json
+-rw-r--r--   0        0        0     6070 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/map/tests/test_map.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/parquet/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/parquet/read/__init__.py
+-rw-r--r--   0        0        0     1115 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/parquet/read/block.py
+-rw-r--r--   0        0        0      352 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/parquet/read/block.schema.json
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/parquet/write/__init__.py
+-rw-r--r--   0        0        0     1271 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/parquet/write/block.py
+-rw-r--r--   0        0        0      352 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/parquet/write/block.schema.json
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/redis/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/redis/lookup/__init__.py
+-rw-r--r--   0        0        0     2566 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/redis/lookup/block.py
+-rw-r--r--   0        0        0      888 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/redis/lookup/block.schema.json
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/redis/read_stream/__init__.py
+-rw-r--r--   0        0        0     2589 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/redis/read_stream/block.py
+-rw-r--r--   0        0        0      586 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json
+-rw-r--r--   0        0        0     1947 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/redis/utils.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/redis/write/__init__.py
+-rw-r--r--   0        0        0     2097 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/redis/write/block.py
+-rw-r--r--   0        0        0      886 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/redis/write/block.schema.json
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/relational/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/relational/read/__init__.py
+-rw-r--r--   0        0        0     1616 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/relational/read/block.py
+-rw-r--r--   0        0        0     1315 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/relational/read/block.schema.json
+-rw-r--r--   0        0        0     1669 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/relational/utils.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/relational/write/__init__.py
+-rw-r--r--   0        0        0    10167 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/relational/write/block.py
+-rw-r--r--   0        0        0     3312 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/relational/write/block.schema.json
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/remove_field/__init__.py
+-rw-r--r--   0        0        0     1182 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/remove_field/block.py
+-rw-r--r--   0        0        0     1182 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/remove_field/block.schema.json
+-rw-r--r--   0        0        0     1893 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/rename_field/__init__.py
+-rw-r--r--   0        0        0     1942 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/rename_field/block.py
+-rw-r--r--   0        0        0     1716 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/rename_field/block.schema.json
+-rw-r--r--   0        0        0     2279 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/sequence/__init__.py
+-rw-r--r--   0        0        0      436 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/sequence/block.py
+-rw-r--r--   0        0        0      517 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/sequence/block.schema.json
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/std/__init__.py
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/std/read/__init__.py
+-rw-r--r--   0        0        0     1299 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/std/read/block.py
+-rw-r--r--   0        0        0       75 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/std/read/block.schema.json
+-rw-r--r--   0        0        0        0 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/std/write/__init__.py
+-rw-r--r--   0        0        0      870 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/std/write/block.py
+-rw-r--r--   0        0        0       76 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/blocks/std/write/block.schema.json
+-rw-r--r--   0        0        0      337 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/context.py
+-rw-r--r--   0        0        0     7581 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/expression.py
+-rw-r--r--   0        0        0     8300 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/jmespath_custom_functions.py
+-rw-r--r--   0        0        0    10326 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/job.py
+-rw-r--r--   0        0        0      116 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/opcode.py
+-rw-r--r--   0        0        0      739 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/producer.py
+-rw-r--r--   0        0        0      522 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/prometheus.py
+-rw-r--r--   0        0        0       23 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/resources/scaffold/.gitignore
+-rw-r--r--   0        0        0      955 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/resources/scaffold/README.md
+-rw-r--r--   0        0        0      151 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/resources/scaffold/connections.yaml
+-rw-r--r--   0        0        0      188 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/resources/scaffold/data/sample.csv
+-rw-r--r--   0        0        0      444 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/resources/scaffold/jobs/sample/hello.yaml
+-rw-r--r--   0        0        0     1079 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/resources/schemas/connections/cassandra.schema.json
+-rw-r--r--   0        0        0     1289 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/resources/schemas/connections/mysql.schema.json
+-rw-r--r--   0        0        0     1584 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/resources/schemas/connections/oracle.schema.json
+-rw-r--r--   0        0        0     1400 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/resources/schemas/connections/postgresql.schema.json
+-rw-r--r--   0        0        0     1366 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/resources/schemas/connections/redis.schema.json
+-rw-r--r--   0        0        0     1139 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/resources/schemas/connections/sqlserver.schema.json
+-rw-r--r--   0        0        0      981 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/resources/schemas/connections.schema.json
+-rw-r--r--   0        0        0     1833 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/resources/schemas/job.schema.json
+-rw-r--r--   0        0        0     1048 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/result.py
+-rw-r--r--   0        0        0     5505 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/step.py
+-rw-r--r--   0        0        0     2112 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/step_buffer.py
+-rw-r--r--   0        0        0     4770 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/utils.py
+-rw-r--r--   0        0        0     2485 2023-10-31 12:57:35.752486 datayoga_core-1.99.0/src/datayoga_core/write_utils.py
+-rw-r--r--   0        0        0     8037 1970-01-01 00:00:00.000000 datayoga_core-1.99.0/PKG-INFO
```

### Comparing `datayoga_core-1.98.0/README.md` & `datayoga_core-1.99.0/README.md`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/pyproject.toml` & `datayoga_core-1.99.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "datayoga-core"
-version = "1.98.0"
+version = "1.99.0"
 description = "DataYoga for Python"
 authors = ["DataYoga <admin@datayoga.io>"]
 license = "Apache-2.0"
 readme = "README.md"
 include = [
 ]
```

### Comparing `datayoga_core-1.98.0/src/datayoga_core/__init__.py` & `datayoga_core-1.99.0/src/datayoga_core/__init__.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/block.py` & `datayoga_core-1.99.0/src/datayoga_core/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/add_field/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/add_field/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/add_field/block.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/blocks/add_field/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/add_field/tests/test_add_field.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/azure/read_event_hub/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/azure/read_event_hub/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/azure/read_event_hub/block.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/blocks/azure/read_event_hub/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/cassandra/write/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/cassandra/write/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/cassandra/write/block.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/blocks/cassandra/write/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/files/read_csv/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/files/read_csv/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/files/read_csv/block.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/blocks/files/read_csv/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/filter/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/filter/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/filter/tests/test_filter.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/filter/tests/test_filter.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/http/receiver/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/http/receiver/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/jinja_template/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/jinja_template/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/jinja_template/block.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/blocks/jinja_template/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/jinja_template/tests/test_jinja_template.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/jinja_template/tests/test_jinja_template.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/map/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/map/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/map/block.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/blocks/map/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/map/tests/test_map.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/map/tests/test_map.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/parquet/read/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/parquet/read/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/parquet/write/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/parquet/write/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/redis/lookup/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/redis/lookup/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/redis/lookup/block.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/blocks/redis/lookup/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/redis/read_stream/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/redis/read_stream/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/blocks/redis/read_stream/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/redis/utils.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/redis/utils.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/redis/write/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/redis/write/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/redis/write/block.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/blocks/redis/write/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/relational/read/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/relational/read/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/relational/read/block.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/blocks/relational/read/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/relational/utils.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/relational/utils.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/relational/write/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/relational/write/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/relational/write/block.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/blocks/relational/write/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/remove_field/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/remove_field/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/remove_field/block.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/blocks/remove_field/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/remove_field/tests/test_remove_field.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/rename_field/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/rename_field/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/rename_field/block.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/blocks/rename_field/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/rename_field/tests/test_rename_field.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/sequence/block.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/blocks/sequence/block.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/std/read/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/std/read/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/blocks/std/write/block.py` & `datayoga_core-1.99.0/src/datayoga_core/blocks/std/write/block.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/expression.py` & `datayoga_core-1.99.0/src/datayoga_core/expression.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/jmespath_custom_functions.py` & `datayoga_core-1.99.0/src/datayoga_core/jmespath_custom_functions.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/job.py` & `datayoga_core-1.99.0/src/datayoga_core/job.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/producer.py` & `datayoga_core-1.99.0/src/datayoga_core/producer.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/prometheus.py` & `datayoga_core-1.99.0/src/datayoga_core/prometheus.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/resources/scaffold/README.md` & `datayoga_core-1.99.0/src/datayoga_core/resources/scaffold/README.md`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/resources/schemas/connections/cassandra.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/resources/schemas/connections/mysql.schema.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3305555555555556%*

 * *Differences: {"'description'": "'Schema for configuring MySQL database connection parameters'",*

 * * "'examples'": "[OrderedDict([('hr', OrderedDict([('type', 'mysql'), ('host', 'localhost'), "*

 * *               "('port', 3306), ('database', 'hr'), ('user', 'myuser'), ('password', 'mypass'), "*

 * *               "('connect_args', OrderedDict([('ssl_ca', '/opt/ssl/ca.crt'), ('ssl_cert', "*

 * *               "'/opt/ssl/client.crt'), ('ssl_key', '/opt/ssl/client.key')]))]))])]",*

 * * "'properties'": "{'port': {'description': 'DB port', delet […]*

```diff
@@ -1,58 +1,62 @@
 {
-    "additionalProperties": false,
-    "description": "Cassandra",
+    "description": "Schema for configuring MySQL database connection parameters",
     "examples": [
         {
-            "cache": {
-                "database": "myDB",
-                "hosts": [
-                    "localhost"
-                ],
-                "password": "myPassword",
-                "port": 9042,
-                "type": "cassandra",
-                "user": "myUser"
+            "hr": {
+                "connect_args": {
+                    "ssl_ca": "/opt/ssl/ca.crt",
+                    "ssl_cert": "/opt/ssl/client.crt",
+                    "ssl_key": "/opt/ssl/client.key"
+                },
+                "database": "hr",
+                "host": "localhost",
+                "password": "mypass",
+                "port": 3306,
+                "type": "mysql",
+                "user": "myuser"
             }
         }
     ],
     "properties": {
+        "connect_args": {
+            "additionalProperties": true,
+            "description": "Additional arguments to use when connecting to the DB",
+            "type": "object"
+        },
         "database": {
             "description": "DB name",
             "type": "string"
         },
-        "hosts": {
-            "description": "Cassandra hosts",
-            "items": {
-                "title": "Address of Cassandra node",
-                "type": "string"
-            },
-            "type": "array"
+        "host": {
+            "description": "DB host",
+            "type": "string"
         },
         "password": {
             "description": "DB password",
             "type": "string"
         },
         "port": {
-            "default": 9042,
-            "description": "Cassandra DB port",
+            "description": "DB port",
             "maximum": 65535,
             "minimum": 1,
             "type": "integer"
         },
-        "type": {
-            "description": "DB type",
-            "enum": [
-                "cassandra"
-            ],
-            "type": "string"
+        "query_args": {
+            "additionalProperties": true,
+            "description": "Additional query string arguments to use when connecting to the DB",
+            "type": "object"
         },
         "user": {
             "description": "DB user",
             "type": "string"
         }
     },
     "required": [
         "type",
-        "hosts"
-    ]
+        "host",
+        "database",
+        "user"
+    ],
+    "title": "MySQL",
+    "type": "object"
 }
```

### Comparing `datayoga_core-1.98.0/src/datayoga_core/resources/schemas/connections/mysql.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/resources/schemas/connections/sqlserver.schema.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.48809523809523814%*

 * *Differences: {"'description'": "'Schema for configuring SQL Server database connection parameters'",*

 * * "'examples'": "{0: {'hr': {'type': 'sqlserver', 'port': 1433, delete: ['connect_args']}}}",*

 * * "'title'": "'SQL Server'",*

 * * "'type'": "'object'"}*

```diff
@@ -1,21 +1,17 @@
 {
+    "description": "Schema for configuring SQL Server database connection parameters",
     "examples": [
         {
             "hr": {
-                "connect_args": {
-                    "ssl_ca": "/opt/ssl/ca.crt",
-                    "ssl_cert": "/opt/ssl/client.crt",
-                    "ssl_key": "/opt/ssl/client.key"
-                },
                 "database": "hr",
                 "host": "localhost",
                 "password": "mypass",
-                "port": 3306,
-                "type": "mysql",
+                "port": 1433,
+                "type": "sqlserver",
                 "user": "myuser"
             }
         }
     ],
     "properties": {
         "connect_args": {
             "additionalProperties": true,
@@ -51,9 +47,11 @@
         }
     },
     "required": [
         "type",
         "host",
         "database",
         "user"
-    ]
+    ],
+    "title": "SQL Server",
+    "type": "object"
 }
```

### Comparing `datayoga_core-1.98.0/src/datayoga_core/resources/schemas/connections/oracle.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/resources/schemas/connections/oracle.schema.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5833333333333334%*

 * *Differences: {"'description'": "'Schema for configuring Oracle database connection parameters'",*

 * * "'title'": "'Oracle'",*

 * * "'type'": "'object'"}*

```diff
@@ -1,9 +1,9 @@
 {
-    "description": "Oracle",
+    "description": "Schema for configuring Oracle database connection parameters",
     "examples": [
         {
             "hr": {
                 "database": "orcl",
                 "host": "localhost",
                 "oracle_thick_mode": true,
                 "oracle_thick_mode_lib_dir": "/opt/oracle/instantclient_21_8/",
@@ -62,9 +62,11 @@
         }
     },
     "required": [
         "type",
         "host",
         "database",
         "user"
-    ]
+    ],
+    "title": "Oracle",
+    "type": "object"
 }
```

### Comparing `datayoga_core-1.98.0/src/datayoga_core/resources/schemas/connections/postgresql.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/resources/schemas/connections/postgresql.schema.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.5%*

 * *Differences: {"'description'": "'Schema for configuring PostgreSQL database connection parameters'",*

 * * "'title'": "'PostgreSQL'",*

 * * "'type'": "'object'"}*

```diff
@@ -1,8 +1,9 @@
 {
+    "description": "Schema for configuring PostgreSQL database connection parameters",
     "examples": [
         {
             "hr": {
                 "connect_args": {
                     "connect_timeout": 10
                 },
                 "database": "postgres",
@@ -55,9 +56,11 @@
         }
     },
     "required": [
         "type",
         "host",
         "database",
         "user"
-    ]
+    ],
+    "title": "PostgreSQL",
+    "type": "object"
 }
```

### Comparing `datayoga_core-1.98.0/src/datayoga_core/resources/schemas/connections/redis.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/resources/schemas/connections/cassandra.schema.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.44632034632034634%*

 * *Differences: {"'description'": "'Schema for configuring Cassandra database connection parameters'",*

 * * "'examples'": "{0: {'cache': {'type': 'cassandra', 'port': 9042, 'hosts': ['localhost'], "*

 * *               "'database': 'myDB', 'user': 'myUser', 'password': 'myPassword', delete: "*

 * *               "['host']}}}",*

 * * "'properties'": "{'type': {'enum': ['cassandra']}, 'port': {'description': 'Cassandra DB port', "*

 * *                 "'default': 9042}, 'user': {'description': 'DB user'}, 'password': "*

 * *                 "{'descript […]*

```diff
@@ -1,75 +1,60 @@
 {
     "additionalProperties": false,
-    "dependentRequired": {
-        "cert": [
-            "key"
-        ],
-        "key": [
-            "cert"
-        ],
-        "key_password": [
-            "key"
-        ],
-        "user": [
-            "password"
-        ]
-    },
-    "description": "Redis",
+    "description": "Schema for configuring Cassandra database connection parameters",
     "examples": [
         {
             "cache": {
-                "host": "localhost",
-                "port": 6379,
-                "type": "redis"
+                "database": "myDB",
+                "hosts": [
+                    "localhost"
+                ],
+                "password": "myPassword",
+                "port": 9042,
+                "type": "cassandra",
+                "user": "myUser"
             }
         }
     ],
     "properties": {
-        "cacert": {
-            "title": "CA certificate file to verify with",
+        "database": {
+            "description": "DB name",
             "type": "string"
         },
-        "cert": {
-            "title": "Client certificate file to authenticate with",
-            "type": "string"
-        },
-        "host": {
-            "description": "Redis DB host",
-            "type": "string"
-        },
-        "key": {
-            "title": "Private key file to authenticate with",
-            "type": "string"
-        },
-        "key_password": {
-            "title": "Password for unlocking an encrypted private key",
-            "type": "string"
+        "hosts": {
+            "description": "Cassandra hosts",
+            "items": {
+                "title": "Address of Cassandra node",
+                "type": "string"
+            },
+            "type": "array"
         },
         "password": {
-            "description": "Redis DB password",
+            "description": "DB password",
             "type": "string"
         },
         "port": {
-            "description": "Redis DB port",
+            "default": 9042,
+            "description": "Cassandra DB port",
             "maximum": 65535,
             "minimum": 1,
             "type": "integer"
         },
         "type": {
             "description": "DB type",
             "enum": [
-                "redis"
+                "cassandra"
             ],
             "type": "string"
         },
         "user": {
-            "description": "Redis DB user",
+            "description": "DB user",
             "type": "string"
         }
     },
     "required": [
         "type",
-        "host",
-        "port"
-    ]
+        "hosts"
+    ],
+    "title": "Cassandra",
+    "type": "object"
 }
```

### Comparing `datayoga_core-1.98.0/src/datayoga_core/resources/schemas/connections/sqlserver.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/resources/schemas/connections.schema.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Differences: {'replace': "OrderedDict([('title', 'Connections'), ('description', 'Connection catalog'), "*

 * *            "('type', ['object', 'null']), ('patternProperties', OrderedDict([('.', "*

 * *            "OrderedDict([('type', 'object'), ('properties', OrderedDict([('type', "*

 * *            "OrderedDict([('description', 'DB type'), ('type', 'string'), ('enum', ['cassandra', "*

 * *            "'mysql', 'postgresql', 'redis', 'sqlserver'])])), ('driver', "*

 * *            "OrderedDict([('description', 'Explicit driver to use, if not […]*

```diff
@@ -1,54 +1,44 @@
 {
-    "examples": [
-        {
-            "hr": {
-                "database": "hr",
-                "host": "localhost",
-                "password": "mypass",
-                "port": 1433,
-                "type": "sqlserver",
-                "user": "myuser"
-            }
-        }
-    ],
-    "properties": {
-        "connect_args": {
-            "additionalProperties": true,
-            "description": "Additional arguments to use when connecting to the DB",
-            "type": "object"
-        },
-        "database": {
-            "description": "DB name",
-            "type": "string"
-        },
-        "host": {
-            "description": "DB host",
-            "type": "string"
-        },
-        "password": {
-            "description": "DB password",
-            "type": "string"
-        },
-        "port": {
-            "description": "DB port",
-            "maximum": 65535,
-            "minimum": 1,
-            "type": "integer"
-        },
-        "query_args": {
-            "additionalProperties": true,
-            "description": "Additional query string arguments to use when connecting to the DB",
+    "description": "Connection catalog",
+    "patternProperties": {
+        ".": {
+            "properties": {
+                "connect_args": {
+                    "description": "Additional arguments to use when connecting to the DB",
+                    "type": "object"
+                },
+                "debug": {
+                    "default": false,
+                    "description": "Echo all SQL commands to stdout",
+                    "title": "Debug mode",
+                    "type": "boolean"
+                },
+                "driver": {
+                    "description": "Explicit driver to use, if not using default",
+                    "type": "string"
+                },
+                "query_args": {
+                    "description": "Additional query string arguments to use when connecting to the DB",
+                    "type": "object"
+                },
+                "type": {
+                    "description": "DB type",
+                    "enum": [
+                        "cassandra",
+                        "mysql",
+                        "postgresql",
+                        "redis",
+                        "sqlserver"
+                    ],
+                    "type": "string"
+                }
+            },
             "type": "object"
-        },
-        "user": {
-            "description": "DB user",
-            "type": "string"
         }
     },
-    "required": [
-        "type",
-        "host",
-        "database",
-        "user"
+    "title": "Connections",
+    "type": [
+        "object",
+        "null"
     ]
 }
```

### Comparing `datayoga_core-1.98.0/src/datayoga_core/resources/schemas/job.schema.json` & `datayoga_core-1.99.0/src/datayoga_core/resources/schemas/job.schema.json`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/result.py` & `datayoga_core-1.99.0/src/datayoga_core/result.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/step.py` & `datayoga_core-1.99.0/src/datayoga_core/step.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/step_buffer.py` & `datayoga_core-1.99.0/src/datayoga_core/step_buffer.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/utils.py` & `datayoga_core-1.99.0/src/datayoga_core/utils.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/src/datayoga_core/write_utils.py` & `datayoga_core-1.99.0/src/datayoga_core/write_utils.py`

 * *Files identical despite different names*

### Comparing `datayoga_core-1.98.0/PKG-INFO` & `datayoga_core-1.99.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datayoga-core
-Version: 1.98.0
+Version: 1.99.0
 Summary: DataYoga for Python
 License: Apache-2.0
 Author: DataYoga
 Author-email: admin@datayoga.io
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

