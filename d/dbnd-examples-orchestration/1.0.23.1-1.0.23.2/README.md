# Comparing `tmp/dbnd-examples-orchestration-1.0.23.1.tar.gz` & `tmp/dbnd-examples-orchestration-1.0.23.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-examples-orchestration-1.0.23.1.tar", last modified: Thu May 16 10:18:11 2024, max compression
+gzip compressed data, was "dbnd-examples-orchestration-1.0.23.2.tar", last modified: Sun May 19 17:25:06 2024, max compression
```

## Comparing `dbnd-examples-orchestration-1.0.23.1.tar` & `dbnd-examples-orchestration-1.0.23.2.tar`

### file list

```diff
@@ -1,247 +1,247 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.666571 dbnd-examples-orchestration-1.0.23.1/
--rw-rw-rw-   0 root         (0) root         (0)    11347 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)     1672 2024-05-16 10:18:11.666571 dbnd-examples-orchestration-1.0.23.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      276 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.632568 dbnd-examples-orchestration-1.0.23.1/data/
--rw-rw-rw-   0 root         (0) root         (0)      735 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/examples_config.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.620567 dbnd-examples-orchestration-1.0.23.1/data/partitioned_data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.632568 dbnd-examples-orchestration-1.0.23.1/data/partitioned_data/2018-09-01/
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/partitioned_data/2018-09-01/file.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.632568 dbnd-examples-orchestration-1.0.23.1/data/partitioned_data/2018-09-02/
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/partitioned_data/2018-09-02/file.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.634568 dbnd-examples-orchestration-1.0.23.1/data/partitioned_data/2018-09-03/
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/partitioned_data/2018-09-03/file.csv
--rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/partitioned_data/2018-09-03/file2.csv
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/people.txt
--rw-rw-rw-   0 root         (0) root         (0)    33543 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/pipeline_train_seed_data.csv
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.634568 dbnd-examples-orchestration-1.0.23.1/data/raw_logs/
--rw-rw-rw-   0 root         (0) root         (0)        8 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/raw_logs/2018-06-20.txt
--rw-rw-rw-   0 root         (0) root         (0)        8 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/raw_logs/2018-06-21.txt
--rw-rw-rw-   0 root         (0) root         (0)        8 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/raw_logs/2018-06-22.txt
--rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/vegetables_for_greek_salad.txt
--rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/vegetables_for_pasta_salad.txt
--rw-rw-rw-   0 root         (0) root         (0)   264426 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/wine_quality.csv
--rw-rw-rw-   0 root         (0) root         (0)    69193 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/wine_quality.csv.gz
--rw-rw-rw-   0 root         (0) root         (0)    79704 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/wine_quality.py27.parquet
--rw-rw-rw-   0 root         (0) root         (0)    19832 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/wine_quality.py36.parquet
--rw-rw-rw-   0 root         (0) root         (0)    37722 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/data/wine_quality_minimized.csv
--rw-rw-rw-   0 root         (0) root         (0)     2125 2024-05-16 10:18:11.667571 dbnd-examples-orchestration-1.0.23.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1170 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.621567 dbnd-examples-orchestration-1.0.23.1/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.635568 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/
--rw-rw-rw-   0 root         (0) root         (0)      408 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/_plugin.py
--rw-rw-rw-   0 root         (0) root         (0)      183 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/conftest.py
--rw-rw-rw-   0 root         (0) root         (0)     2193 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.636568 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/
--rw-rw-rw-   0 root         (0) root         (0)      199 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.637569 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/
--rw-rw-rw-   0 root         (0) root         (0)     3600 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/pom.xml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.621567 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.621567 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.621567 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.621567 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.621567 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.637569 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/
--rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/AddDressing.java
--rw-rw-rw-   0 root         (0) root         (0)     1150 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/Cut.java
--rw-rw-rw-   0 root         (0) root         (0)     2073 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCount.java
--rw-rw-rw-   0 root         (0) root         (0)     2438 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCountWithHtml.java
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.638569 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.640569 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      789 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_decorator.py
--rw-rw-rw-   0 root         (0) root         (0)     1787 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_decorator2.py
--rw-rw-rw-   0 root         (0) root         (0)      959 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_logging.py
--rw-rw-rw-   0 root         (0) root         (0)     1834 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_marshaller_excel.py
--rw-rw-rw-   0 root         (0) root         (0)      830 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_marshaller_override.py
--rw-rw-rw-   0 root         (0) root         (0)     2499 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_output_factory.py
--rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_output_location.py
--rw-rw-rw-   0 root         (0) root         (0)     1294 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_paramester_user_object.py
--rw-rw-rw-   0 root         (0) root         (0)     1323 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_target.py
--rw-rw-rw-   0 root         (0) root         (0)     2171 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_value_type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.640569 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_airflow/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_airflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1464 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_airflow/scheduled_dbnd_check.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.641569 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_aws/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_aws/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.641569 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_aws/airflow/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_aws/airflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2215 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_aws/airflow/scheduled_sensor.py
--rw-rw-rw-   0 root         (0) root         (0)     3587 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_aws/ingest_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     2707 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_aws/sync_operators.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.642569 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_docker/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_docker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      302 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_docker/docker_run_task_test.py
--rw-rw-rw-   0 root         (0) root         (0)     2048 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_docker/dockerized_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.642569 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.642569 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_bigquery/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_bigquery/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      221 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_bigquery/wine_quality_big_query.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.643569 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count.py
--rw-rw-rw-   0 root         (0) root         (0)     4971 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count_inline.py
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/parameters.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.643569 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/pybeam/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/pybeam/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     5128 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/pybeam/wordcount.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.645569 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2337 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/read_from_multiple_sources.py
--rw-rw-rw-   0 root         (0) root         (0)     1508 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/salad_spark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.645569 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/
--rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      870 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/add_dressing.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/cut_salad.py
--rw-rw-rw-   0 root         (0) root         (0)     1833 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/word_count.py
--rw-rw-rw-   0 root         (0) root         (0)     3679 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/spark_config_examples.py
--rw-rw-rw-   0 root         (0) root         (0)     3060 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/word_count.py
--rw-rw-rw-   0 root         (0) root         (0)     2781 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/word_count_with_deequ.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.647570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/report.py
--rw-rw-rw-   0 root         (0) root         (0)     1986 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/salad.py
--rw-rw-rw-   0 root         (0) root         (0)     2060 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/top_artists.py
--rw-rw-rw-   0 root         (0) root         (0)     2382 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/top_artists__as_task_class.py
--rw-rw-rw-   0 root         (0) root         (0)     5924 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/wine_quality.py
--rw-rw-rw-   0 root         (0) root         (0)     8019 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/wine_quality_as_notebook.ipynb
--rw-rw-rw-   0 root         (0) root         (0)     5305 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/wine_quality_as_task_class.py
--rw-rw-rw-   0 root         (0) root         (0)   123099 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/wine_quality_pipeline.png
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.649570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      846 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/dynamic_tasks_with_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      398 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/example_dict_of_data_frames.py
--rw-rw-rw-   0 root         (0) root         (0)     1196 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/example_folder.py
--rw-rw-rw-   0 root         (0) root         (0)     1559 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/example_output_per_id.py
--rw-rw-rw-   0 root         (0) root         (0)     4591 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/partitioned_by_day.py
--rw-rw-rw-   0 root         (0) root         (0)     1385 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/partitioned_calculations_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     1539 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/partitioned_data_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     2150 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/partitioned_inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/pipeline_with_sub_runs.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.650570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_mxnet/
--rw-rw-rw-   0 root         (0) root         (0)      223 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_mxnet/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2630 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_mxnet/data.py
--rw-rw-rw-   0 root         (0) root         (0)     5015 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_mxnet/mxnet_digit_mnist.py
--rw-rw-rw-   0 root         (0) root         (0)     4472 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_mxnet/mxnet_fashion_mnist.py
--rw-rw-rw-   0 root         (0) root         (0)     1112 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_mxnet/mxnet_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.651570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/
--rw-rw-rw-   0 root         (0) root         (0)      233 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     8593 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/amazon_video_reviews.py
--rw-rw-rw-   0 root         (0) root         (0)     9476 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/mnist.py
--rw-rw-rw-   0 root         (0) root         (0)      617 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/mnist_pytorch.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.652570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sklearn/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3353 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sklearn/generate.py
--rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sklearn/run_example.sh
--rw-rw-rw-   0 root         (0) root         (0)     2617 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sklearn/sklearn_example.py
--rw-rw-rw-   0 root         (0) root         (0)     7708 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sklearn/train_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     5622 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sklearn/train_via_spark.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.653570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/
--rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3062 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/iris.py
--rw-rw-rw-   0 root         (0) root         (0)     3997 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/tf_iris.py
--rw-rw-rw-   0 root         (0) root         (0)     4735 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/tf_simple.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.654570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/
--rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T01_tasks_and_pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     1318 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T02_task_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T03_task_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)     2265 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T11_data_wiring.py
--rw-rw-rw-   0 root         (0) root         (0)     1773 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T12_data_pandas_and_numpy.py
--rw-rw-rw-   0 root         (0) root         (0)      894 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T21_task_that_calls_other_tasks.py
--rw-rw-rw-   0 root         (0) root         (0)     1030 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T22_user_class_as_task.py
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.654570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/
--rw-rw-rw-   0 root         (0) root         (0)      176 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.654570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.655570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      304 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.655570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/environment_configuration/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/environment_configuration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.656570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/k8s_integration/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/k8s_integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1038 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/k8s_integration/test_doc_kubernetes_engine_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      517 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/k8s_integration/test_doc_setup_k8s_cluster.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.656570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/object_configuration/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/object_configuration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      311 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/object_configuration/test_doc_configuration_layers.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.657570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/quickstart/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/quickstart/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3749 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/quickstart/test_doc_orchestration_quickstart.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.658570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1279 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_accessing_run_results.py
--rw-rw-rw-   0 root         (0) root         (0)     1511 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_accessing_task_meta.py
--rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_overriding_configuration_in_cli.py
--rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_run_a_task_in_python.py
--rw-rw-rw-   0 root         (0) root         (0)      310 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_running_pipelines.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.659570 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1241 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_debug_spark_task_locally.py
--rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      649 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_dataframes.py
--rw-rw-rw-   0 root         (0) root         (0)      457 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_engine_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     1747 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_orchestration.py
--rw-rw-rw-   0 root         (0) root         (0)      287 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_task_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)     1644 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_tasks_pipelines.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.661571 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_decorated_dags.py
--rw-rw-rw-   0 root         (0) root         (0)     1605 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_inputs.py
--rw-rw-rw-   0 root         (0) root         (0)     1328 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_orchestrating_tasks_and_pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     4496 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_task_definitions_as_a_class.py
--rw-rw-rw-   0 root         (0) root         (0)     3325 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_task_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)      984 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_tasks_pipeline_data.py
--rw-rw-rw-   0 root         (0) root         (0)     2221 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_tasks_wiring_at_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_doc_faq.py
--rw-rw-rw-   0 root         (0) root         (0)      732 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_doc_object_configuration.py
--rw-rw-rw-   0 root         (0) root         (0)      947 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_doc_task_configuration_defaults.py
--rw-rw-rw-   0 root         (0) root         (0)     1721 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_doc_task_object.py
--rw-rw-rw-   0 root         (0) root         (0)     3400 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_quick_start_wine_quality.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.661571 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      305 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/conftest.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.662571 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/customizations/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/customizations/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/customizations/test_custom_decorators.py
--rw-rw-rw-   0 root         (0) root         (0)     2610 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/customizations/test_feature_custom.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/customizations/test_run_with_custom_targets.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.662571 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/dbnd_spark/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/dbnd_spark/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1863 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/dbnd_spark/test_spark_task.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.664571 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/examples/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/examples/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      941 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/examples/test_example_salad.py
--rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/examples/test_report.py
--rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/examples/test_salad.py
--rw-rw-rw-   0 root         (0) root         (0)      657 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/examples/test_top_artist.py
--rw-rw-rw-   0 root         (0) root         (0)     2371 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/examples/test_wine_quality.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.664571 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/features/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/features/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      424 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/features/test_dynamic_tasks_with_pipeline.py
--rw-rw-rw-   0 root         (0) root         (0)     1414 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/features/test_feature_by_day_prod.py
--rw-rw-rw-   0 root         (0) root         (0)     1781 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/features/test_feature_input_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)     1606 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/features/test_feature_partitions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.665571 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/tool_sklearn/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/tool_sklearn/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/tool_sklearn/test_sklearn_linear_reg_pipeline.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.666571 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/
--rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      652 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/test_T01_tasks_and_pipelines.py
--rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/test_T02_task_parameters.py
--rw-rw-rw-   0 root         (0) root         (0)     1059 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/test_T03_task_outputs.py
--rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/test_T12_pandas_numpy.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 10:18:11.636568 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1672 2024-05-16 10:18:11.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    14849 2024-05-16 10:18:11.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 10:18:11.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       73 2024-05-16 10:18:11.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 10:18:11.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)      239 2024-05-16 10:18:11.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       28 2024-05-16 10:18:11.000000 dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration.egg-info/top_level.txt
--rw-rw-rw-   0 root         (0) root         (0)     2225 2024-05-16 10:17:47.000000 dbnd-examples-orchestration-1.0.23.1/tox.ini
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.241647 dbnd-examples-orchestration-1.0.23.2/
+-rw-rw-rw-   0 root         (0) root         (0)    11347 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-05-19 17:25:06.241647 dbnd-examples-orchestration-1.0.23.2/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      276 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.205644 dbnd-examples-orchestration-1.0.23.2/data/
+-rw-rw-rw-   0 root         (0) root         (0)      735 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/examples_config.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.196643 dbnd-examples-orchestration-1.0.23.2/data/partitioned_data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.205644 dbnd-examples-orchestration-1.0.23.2/data/partitioned_data/2018-09-01/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/partitioned_data/2018-09-01/file.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.206644 dbnd-examples-orchestration-1.0.23.2/data/partitioned_data/2018-09-02/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/partitioned_data/2018-09-02/file.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.206644 dbnd-examples-orchestration-1.0.23.2/data/partitioned_data/2018-09-03/
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/partitioned_data/2018-09-03/file.csv
+-rw-rw-rw-   0 root         (0) root         (0)       18 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/partitioned_data/2018-09-03/file2.csv
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/people.txt
+-rw-rw-rw-   0 root         (0) root         (0)    33543 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/pipeline_train_seed_data.csv
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.206644 dbnd-examples-orchestration-1.0.23.2/data/raw_logs/
+-rw-rw-rw-   0 root         (0) root         (0)        8 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/raw_logs/2018-06-20.txt
+-rw-rw-rw-   0 root         (0) root         (0)        8 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/raw_logs/2018-06-21.txt
+-rw-rw-rw-   0 root         (0) root         (0)        8 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/raw_logs/2018-06-22.txt
+-rw-rw-rw-   0 root         (0) root         (0)       32 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/vegetables_for_greek_salad.txt
+-rw-rw-rw-   0 root         (0) root         (0)       22 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/vegetables_for_pasta_salad.txt
+-rw-rw-rw-   0 root         (0) root         (0)   264426 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/wine_quality.csv
+-rw-rw-rw-   0 root         (0) root         (0)    69193 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/wine_quality.csv.gz
+-rw-rw-rw-   0 root         (0) root         (0)    79704 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/wine_quality.py27.parquet
+-rw-rw-rw-   0 root         (0) root         (0)    19832 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/wine_quality.py36.parquet
+-rw-rw-rw-   0 root         (0) root         (0)    37722 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/data/wine_quality_minimized.csv
+-rw-rw-rw-   0 root         (0) root         (0)     2125 2024-05-19 17:25:06.243647 dbnd-examples-orchestration-1.0.23.2/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1170 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.196643 dbnd-examples-orchestration-1.0.23.2/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.207644 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/
+-rw-rw-rw-   0 root         (0) root         (0)      408 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      529 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/_plugin.py
+-rw-rw-rw-   0 root         (0) root         (0)      183 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/conftest.py
+-rw-rw-rw-   0 root         (0) root         (0)     2193 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.209644 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/
+-rw-rw-rw-   0 root         (0) root         (0)      199 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.209644 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/
+-rw-rw-rw-   0 root         (0) root         (0)     3600 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/pom.xml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.197643 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.197643 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.197643 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.197643 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.197643 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.210644 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       60 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/AddDressing.java
+-rw-rw-rw-   0 root         (0) root         (0)     1150 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/Cut.java
+-rw-rw-rw-   0 root         (0) root         (0)     2073 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCount.java
+-rw-rw-rw-   0 root         (0) root         (0)     2438 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCountWithHtml.java
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.210644 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.213645 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      789 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_decorator.py
+-rw-rw-rw-   0 root         (0) root         (0)     1787 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_decorator2.py
+-rw-rw-rw-   0 root         (0) root         (0)      959 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_logging.py
+-rw-rw-rw-   0 root         (0) root         (0)     1834 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_marshaller_excel.py
+-rw-rw-rw-   0 root         (0) root         (0)      830 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_marshaller_override.py
+-rw-rw-rw-   0 root         (0) root         (0)     2499 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_output_factory.py
+-rw-rw-rw-   0 root         (0) root         (0)      535 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_output_location.py
+-rw-rw-rw-   0 root         (0) root         (0)     1294 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_paramester_user_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     1323 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_target.py
+-rw-rw-rw-   0 root         (0) root         (0)     2171 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_value_type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.213645 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_airflow/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_airflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1464 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_airflow/scheduled_dbnd_check.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.214645 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_aws/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_aws/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.214645 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_aws/airflow/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_aws/airflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2215 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_aws/airflow/scheduled_sensor.py
+-rw-rw-rw-   0 root         (0) root         (0)     3587 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_aws/ingest_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2707 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_aws/sync_operators.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.215645 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_docker/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_docker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      302 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_docker/docker_run_task_test.py
+-rw-rw-rw-   0 root         (0) root         (0)     2048 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_docker/dockerized_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.215645 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.216645 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_bigquery/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_bigquery/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      221 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_bigquery/wine_quality_big_query.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.217645 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      562 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count.py
+-rw-rw-rw-   0 root         (0) root         (0)     4971 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count_inline.py
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/parameters.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.217645 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/pybeam/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/pybeam/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     5128 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/pybeam/wordcount.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.218645 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2337 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/read_from_multiple_sources.py
+-rw-rw-rw-   0 root         (0) root         (0)     1508 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/salad_spark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.219645 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/
+-rw-rw-rw-   0 root         (0) root         (0)      149 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      870 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/add_dressing.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/cut_salad.py
+-rw-rw-rw-   0 root         (0) root         (0)     1833 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/word_count.py
+-rw-rw-rw-   0 root         (0) root         (0)     3679 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/spark_config_examples.py
+-rw-rw-rw-   0 root         (0) root         (0)     3060 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/word_count.py
+-rw-rw-rw-   0 root         (0) root         (0)     2781 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/word_count_with_deequ.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.221645 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2544 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/report.py
+-rw-rw-rw-   0 root         (0) root         (0)     1986 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/salad.py
+-rw-rw-rw-   0 root         (0) root         (0)     2060 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/top_artists.py
+-rw-rw-rw-   0 root         (0) root         (0)     2382 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/top_artists__as_task_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     5924 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/wine_quality.py
+-rw-rw-rw-   0 root         (0) root         (0)     8019 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/wine_quality_as_notebook.ipynb
+-rw-rw-rw-   0 root         (0) root         (0)     5305 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/wine_quality_as_task_class.py
+-rw-rw-rw-   0 root         (0) root         (0)   123099 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/wine_quality_pipeline.png
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.223646 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      846 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/dynamic_tasks_with_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      398 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/example_dict_of_data_frames.py
+-rw-rw-rw-   0 root         (0) root         (0)     1196 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/example_folder.py
+-rw-rw-rw-   0 root         (0) root         (0)     1559 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/example_output_per_id.py
+-rw-rw-rw-   0 root         (0) root         (0)     4591 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/partitioned_by_day.py
+-rw-rw-rw-   0 root         (0) root         (0)     1385 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/partitioned_calculations_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1539 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/partitioned_data_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     2150 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/partitioned_inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1516 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/pipeline_with_sub_runs.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.224646 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_mxnet/
+-rw-rw-rw-   0 root         (0) root         (0)      223 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_mxnet/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2630 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_mxnet/data.py
+-rw-rw-rw-   0 root         (0) root         (0)     5015 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_mxnet/mxnet_digit_mnist.py
+-rw-rw-rw-   0 root         (0) root         (0)     4472 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_mxnet/mxnet_fashion_mnist.py
+-rw-rw-rw-   0 root         (0) root         (0)     1112 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_mxnet/mxnet_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.225646 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/
+-rw-rw-rw-   0 root         (0) root         (0)      233 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     8593 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/amazon_video_reviews.py
+-rw-rw-rw-   0 root         (0) root         (0)     9476 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/mnist.py
+-rw-rw-rw-   0 root         (0) root         (0)      617 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/mnist_pytorch.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.226646 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3353 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sklearn/generate.py
+-rw-rw-rw-   0 root         (0) root         (0)     1326 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sklearn/run_example.sh
+-rw-rw-rw-   0 root         (0) root         (0)     2617 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sklearn/sklearn_example.py
+-rw-rw-rw-   0 root         (0) root         (0)     7708 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sklearn/train_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     5622 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sklearn/train_via_spark.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.227646 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/
+-rw-rw-rw-   0 root         (0) root         (0)      151 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3062 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/iris.py
+-rw-rw-rw-   0 root         (0) root         (0)     3997 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/tf_iris.py
+-rw-rw-rw-   0 root         (0) root         (0)     4735 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/tf_simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.228646 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/
+-rw-rw-rw-   0 root         (0) root         (0)     1123 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T01_tasks_and_pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     1318 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T02_task_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1757 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T03_task_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     2265 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T11_data_wiring.py
+-rw-rw-rw-   0 root         (0) root         (0)     1773 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T12_data_pandas_and_numpy.py
+-rw-rw-rw-   0 root         (0) root         (0)      894 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T21_task_that_calls_other_tasks.py
+-rw-rw-rw-   0 root         (0) root         (0)     1030 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T22_user_class_as_task.py
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.229646 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/
+-rw-rw-rw-   0 root         (0) root         (0)      176 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.229646 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.230646 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      304 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.230646 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/environment_configuration/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/environment_configuration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.231646 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/k8s_integration/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/k8s_integration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1038 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/k8s_integration/test_doc_kubernetes_engine_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      517 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/k8s_integration/test_doc_setup_k8s_cluster.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.232646 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/object_configuration/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/object_configuration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      311 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/object_configuration/test_doc_configuration_layers.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.232646 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/quickstart/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/quickstart/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     3749 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/quickstart/test_doc_orchestration_quickstart.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.233646 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1279 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_accessing_run_results.py
+-rw-rw-rw-   0 root         (0) root         (0)     1511 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_accessing_task_meta.py
+-rw-rw-rw-   0 root         (0) root         (0)      440 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_overriding_configuration_in_cli.py
+-rw-rw-rw-   0 root         (0) root         (0)      591 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_run_a_task_in_python.py
+-rw-rw-rw-   0 root         (0) root         (0)      310 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_running_pipelines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.235647 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1241 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_debug_spark_task_locally.py
+-rw-rw-rw-   0 root         (0) root         (0)      609 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      649 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_dataframes.py
+-rw-rw-rw-   0 root         (0) root         (0)      457 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_engine_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1747 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_orchestration.py
+-rw-rw-rw-   0 root         (0) root         (0)      287 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_task_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)     1644 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_tasks_pipelines.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.237647 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1023 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_decorated_dags.py
+-rw-rw-rw-   0 root         (0) root         (0)     1605 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_inputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1328 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_orchestrating_tasks_and_pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     4496 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1163 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_task_definitions_as_a_class.py
+-rw-rw-rw-   0 root         (0) root         (0)     3325 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_task_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)      984 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_tasks_pipeline_data.py
+-rw-rw-rw-   0 root         (0) root         (0)     2221 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_tasks_wiring_at_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)      361 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_doc_faq.py
+-rw-rw-rw-   0 root         (0) root         (0)      732 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_doc_object_configuration.py
+-rw-rw-rw-   0 root         (0) root         (0)      947 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_doc_task_configuration_defaults.py
+-rw-rw-rw-   0 root         (0) root         (0)     1721 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_doc_task_object.py
+-rw-rw-rw-   0 root         (0) root         (0)     3400 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_quick_start_wine_quality.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.237647 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      305 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/conftest.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.238647 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/customizations/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/customizations/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      314 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/customizations/test_custom_decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)     2610 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/customizations/test_feature_custom.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/customizations/test_run_with_custom_targets.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.238647 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/dbnd_spark/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/dbnd_spark/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1863 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/dbnd_spark/test_spark_task.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.240647 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/examples/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/examples/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      941 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/examples/test_example_salad.py
+-rw-rw-rw-   0 root         (0) root         (0)      497 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/examples/test_report.py
+-rw-rw-rw-   0 root         (0) root         (0)      357 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/examples/test_salad.py
+-rw-rw-rw-   0 root         (0) root         (0)      657 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/examples/test_top_artist.py
+-rw-rw-rw-   0 root         (0) root         (0)     2371 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/examples/test_wine_quality.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.240647 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/features/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/features/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      424 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/features/test_dynamic_tasks_with_pipeline.py
+-rw-rw-rw-   0 root         (0) root         (0)     1414 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/features/test_feature_by_day_prod.py
+-rw-rw-rw-   0 root         (0) root         (0)     1781 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/features/test_feature_input_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)     1606 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/features/test_feature_partitions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.240647 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/tool_sklearn/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/tool_sklearn/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      459 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/tool_sklearn/test_sklearn_linear_reg_pipeline.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.241647 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/
+-rw-rw-rw-   0 root         (0) root         (0)       48 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      652 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/test_T01_tasks_and_pipelines.py
+-rw-rw-rw-   0 root         (0) root         (0)     1704 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/test_T02_task_parameters.py
+-rw-rw-rw-   0 root         (0) root         (0)     1059 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/test_T03_task_outputs.py
+-rw-rw-rw-   0 root         (0) root         (0)      414 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/test_T12_pandas_numpy.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-19 17:25:06.209644 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1672 2024-05-19 17:25:06.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    14849 2024-05-19 17:25:06.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 17:25:06.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       73 2024-05-19 17:25:06.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-19 17:25:06.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      239 2024-05-19 17:25:06.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       28 2024-05-19 17:25:06.000000 dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration.egg-info/top_level.txt
+-rw-rw-rw-   0 root         (0) root         (0)     2225 2024-05-19 17:24:43.000000 dbnd-examples-orchestration-1.0.23.2/tox.ini
```

### Comparing `dbnd-examples-orchestration-1.0.23.1/LICENSE` & `dbnd-examples-orchestration-1.0.23.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/PKG-INFO` & `dbnd-examples-orchestration-1.0.23.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-examples-orchestration
-Version: 1.0.23.1
+Version: 1.0.23.2
 Summary: Machine Learning Orchestration
 Home-page: https://github.com/databand-ai/dbnd
 Author: Evgeny Shulman
 Author-email: evgeny.shulman@databand.ai
 Maintainer: Evgeny Shulman
 Maintainer-email: evgeny.shulman@databand.ai
 Project-URL: Documentation, https://dbnd.readme.io/
```

### Comparing `dbnd-examples-orchestration-1.0.23.1/data/examples_config.cfg` & `dbnd-examples-orchestration-1.0.23.2/data/examples_config.cfg`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/data/pipeline_train_seed_data.csv` & `dbnd-examples-orchestration-1.0.23.2/data/pipeline_train_seed_data.csv`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/data/wine_quality.csv` & `dbnd-examples-orchestration-1.0.23.2/data/wine_quality.csv`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/data/wine_quality.csv.gz` & `dbnd-examples-orchestration-1.0.23.2/data/wine_quality.csv.gz`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/data/wine_quality.py27.parquet` & `dbnd-examples-orchestration-1.0.23.2/data/wine_quality.py27.parquet`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/data/wine_quality.py36.parquet` & `dbnd-examples-orchestration-1.0.23.2/data/wine_quality.py36.parquet`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/data/wine_quality_minimized.csv` & `dbnd-examples-orchestration-1.0.23.2/data/wine_quality_minimized.csv`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/setup.cfg` & `dbnd-examples-orchestration-1.0.23.2/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [metadata]
-version = 1.0.23.1
+version = 1.0.23.2
 license_file = LICENSE
 description = Machine Learning Orchestration
 long_description_content_type = text/markdown
 long_description = file: README.md
 platforms = any
 author = Evgeny Shulman
 author_email = evgeny.shulman@databand.ai
```

### Comparing `dbnd-examples-orchestration-1.0.23.1/setup.py` & `dbnd-examples-orchestration-1.0.23.2/setup.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/_plugin.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/_plugin.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/data.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/data.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/pom.xml` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/pom.xml`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/Cut.java` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/Cut.java`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCount.java` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCount.java`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCountWithHtml.java` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/dbnd_spark/spark_jvm/src/main/java/ai/databand/examples/WordCountWithHtml.java`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_decorator.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_decorator.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_decorator2.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_decorator2.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_logging.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_logging.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_marshaller_excel.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_marshaller_excel.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_marshaller_override.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_marshaller_override.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_output_factory.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_output_factory.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_output_location.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_output_location.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_paramester_user_object.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_paramester_user_object.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_target.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_target.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/customizations/custom_value_type.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/customizations/custom_value_type.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_airflow/scheduled_dbnd_check.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_airflow/scheduled_dbnd_check.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_aws/airflow/scheduled_sensor.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_aws/airflow/scheduled_sensor.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_aws/ingest_pipeline.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_aws/ingest_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_aws/sync_operators.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_aws/sync_operators.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_docker/dockerized_pipeline.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_docker/dockerized_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count_inline.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/dataflow_word_count_inline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/pybeam/wordcount.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_gcp/tool_dataflow/pybeam/wordcount.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/read_from_multiple_sources.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/read_from_multiple_sources.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/salad_spark.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/salad_spark.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/add_dressing.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/add_dressing.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/cut_salad.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/cut_salad.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/word_count.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/scripts/word_count.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/spark_config_examples.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/spark_config_examples.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/word_count.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/word_count.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/dbnd_spark/word_count_with_deequ.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/dbnd_spark/word_count_with_deequ.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/report.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/report.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/salad.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/salad.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/top_artists.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/top_artists.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/top_artists__as_task_class.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/top_artists__as_task_class.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/wine_quality.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/wine_quality.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/wine_quality_as_notebook.ipynb` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/wine_quality_as_notebook.ipynb`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/wine_quality_as_task_class.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/wine_quality_as_task_class.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/examples/wine_quality_pipeline.png` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/examples/wine_quality_pipeline.png`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/dynamic_tasks_with_pipeline.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/dynamic_tasks_with_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/example_folder.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/example_folder.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/example_output_per_id.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/example_output_per_id.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/partitioned_by_day.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/partitioned_by_day.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/partitioned_calculations_pipeline.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/partitioned_calculations_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/partitioned_data_pipeline.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/partitioned_data_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/partitioned_inputs.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/partitioned_inputs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/features/pipeline_with_sub_runs.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/features/pipeline_with_sub_runs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_mxnet/data.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_mxnet/data.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_mxnet/mxnet_digit_mnist.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_mxnet/mxnet_digit_mnist.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_mxnet/mxnet_fashion_mnist.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_mxnet/mxnet_fashion_mnist.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_mxnet/mxnet_task.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_mxnet/mxnet_task.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/amazon_video_reviews.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/amazon_video_reviews.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/mnist.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/mnist.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/mnist_pytorch.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sagemaker/mnist_pytorch.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sklearn/generate.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sklearn/generate.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sklearn/run_example.sh` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sklearn/run_example.sh`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sklearn/sklearn_example.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sklearn/sklearn_example.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sklearn/train_pipeline.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sklearn/train_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_sklearn/train_via_spark.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_sklearn/train_via_spark.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/iris.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/iris.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/tf_iris.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/tf_iris.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/tf_simple.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tool_tensorflow/tf_simple.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T01_tasks_and_pipelines.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T01_tasks_and_pipelines.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T02_task_parameters.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T02_task_parameters.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T03_task_outputs.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T03_task_outputs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T11_data_wiring.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T11_data_wiring.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T12_data_pandas_and_numpy.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T12_data_pandas_and_numpy.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T21_task_that_calls_other_tasks.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T21_task_that_calls_other_tasks.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T22_user_class_as_task.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/orchestration/tutorial_syntax/T22_user_class_as_task.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/k8s_integration/test_doc_kubernetes_engine_configuration.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/k8s_integration/test_doc_kubernetes_engine_configuration.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/k8s_integration/test_doc_setup_k8s_cluster.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/k8s_integration/test_doc_setup_k8s_cluster.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/quickstart/test_doc_orchestration_quickstart.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/quickstart/test_doc_orchestration_quickstart.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_accessing_run_results.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_accessing_run_results.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_accessing_task_meta.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_accessing_task_meta.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_run_a_task_in_python.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/run/test_doc_run_a_task_in_python.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_debug_spark_task_locally.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_debug_spark_task_locally.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_configuration.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_configuration.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_dataframes.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_dataframes.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_orchestration.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_orchestration.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_tasks_pipelines.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/spark_integration/test_doc_spark_tasks_pipelines.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_decorated_dags.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_decorated_dags.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_inputs.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_inputs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_orchestrating_tasks_and_pipelines.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_orchestrating_tasks_and_pipelines.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_outputs.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_outputs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_task_definitions_as_a_class.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_task_definitions_as_a_class.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_task_parameters.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_task_parameters.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_tasks_pipeline_data.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_tasks_pipeline_data.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_tasks_wiring_at_pipeline.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/task_pipeline/test_doc_tasks_wiring_at_pipeline.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_doc_object_configuration.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_doc_object_configuration.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_doc_task_configuration_defaults.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_doc_task_configuration_defaults.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_doc_task_object.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_doc_task_object.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_quick_start_wine_quality.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/documentation/orchestration/test_quick_start_wine_quality.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/customizations/test_feature_custom.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/customizations/test_feature_custom.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/dbnd_spark/test_spark_task.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/dbnd_spark/test_spark_task.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/examples/test_example_salad.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/examples/test_example_salad.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/examples/test_top_artist.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/examples/test_top_artist.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/examples/test_wine_quality.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/examples/test_wine_quality.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/features/test_feature_by_day_prod.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/features/test_feature_by_day_prod.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/features/test_feature_input_outputs.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/features/test_feature_input_outputs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/features/test_feature_partitions.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/features/test_feature_partitions.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/test_T01_tasks_and_pipelines.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/test_T01_tasks_and_pipelines.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/test_T02_task_parameters.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/test_T02_task_parameters.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/test_T03_task_outputs.py` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration/tests/orchestration/tutorial_syntax/test_T03_task_outputs.py`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration.egg-info/PKG-INFO` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbnd-examples-orchestration
-Version: 1.0.23.1
+Version: 1.0.23.2
 Summary: Machine Learning Orchestration
 Home-page: https://github.com/databand-ai/dbnd
 Author: Evgeny Shulman
 Author-email: evgeny.shulman@databand.ai
 Maintainer: Evgeny Shulman
 Maintainer-email: evgeny.shulman@databand.ai
 Project-URL: Documentation, https://dbnd.readme.io/
```

### Comparing `dbnd-examples-orchestration-1.0.23.1/src/dbnd_examples_orchestration.egg-info/SOURCES.txt` & `dbnd-examples-orchestration-1.0.23.2/src/dbnd_examples_orchestration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbnd-examples-orchestration-1.0.23.1/tox.ini` & `dbnd-examples-orchestration-1.0.23.2/tox.ini`

 * *Files identical despite different names*

