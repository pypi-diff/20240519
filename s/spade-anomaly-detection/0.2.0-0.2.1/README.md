# Comparing `tmp/spade_anomaly_detection-0.2.0.tar.gz` & `tmp/spade_anomaly_detection-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spade_anomaly_detection-0.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "spade_anomaly_detection-0.2.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `spade_anomaly_detection-0.2.0.tar` & `spade_anomaly_detection-0.2.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0    30078 2024-05-08 15:23:07.509925 spade_anomaly_detection-0.2.0/LICENSE
--rw-r--r--   0        0        0    14507 2024-05-08 15:23:07.509925 spade_anomaly_detection-0.2.0/README.md
--rw-r--r--   0        0        0     2743 2024-05-08 15:23:07.509925 spade_anomaly_detection-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1808 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/Dockerfile
--rw-r--r--   0        0        0     1384 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/__init__.py
--rw-r--r--   0        0        0    26819 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_loader.py
--rw-r--r--   0        0        0     1198 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/__init__.py
--rw-r--r--   0        0        0    29960 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/bq_dataset.py
--rw-r--r--   0        0        0     2055 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/bq_dataset_test_utils.py
--rw-r--r--   0        0        0     4475 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/bq_utils.py
--rw-r--r--   0        0        0    36573 2024-05-08 15:23:07.513925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/feature_metadata.py
--rw-r--r--   0        0        0     1570 2024-05-08 15:23:07.517925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/README.md
--rw-r--r--   0        0        0  3671818 2024-05-08 15:23:07.529925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/covertype_pnu_10000.csv
--rw-r--r--   0        0        0 36719403 2024-05-08 15:23:07.657925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/covertype_pnu_100000.csv
--rw-r--r--   0        0        0  3689614 2024-05-08 15:23:07.677925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/covertype_pu_labeled.csv
--rw-r--r--   0        0        0   582290 2024-05-08 15:23:07.677925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/drug_train_pu_labeled.csv
--rw-r--r--   0        0        0    42111 2024-05-08 15:23:07.677925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/thyroid_labeled.csv
--rw-r--r--   0        0        0    11656 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/occ_ensemble.py
--rw-r--r--   0        0        0     9364 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/parameters.py
--rw-r--r--   0        0        0      746 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/requirements.txt
--rw-r--r--   0        0        0    23357 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/runner.py
--rwxr-xr-x   0        0        0     1146 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/scripts/build_and_push_image.sh
--rw-r--r--   0        0        0     3578 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/scripts/run_cloud_spade_experiment.sh
--rw-r--r--   0        0        0     6333 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/supervised_model.py
--rw-r--r--   0        0        0    11178 2024-05-08 15:23:07.681925 spade_anomaly_detection-0.2.0/spade_anomaly_detection/task.py
--rw-r--r--   0        0        0    16300 1970-01-01 00:00:00.000000 spade_anomaly_detection-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    30078 2024-05-19 00:11:15.195628 spade_anomaly_detection-0.2.1/LICENSE
+-rw-r--r--   0        0        0    14507 2024-05-19 00:11:15.195628 spade_anomaly_detection-0.2.1/README.md
+-rw-r--r--   0        0        0     2723 2024-05-19 00:11:15.195628 spade_anomaly_detection-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1808 2024-05-19 00:11:15.195628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/Dockerfile
+-rw-r--r--   0        0        0     1384 2024-05-19 00:11:15.195628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/__init__.py
+-rw-r--r--   0        0        0    27516 2024-05-19 00:11:15.195628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_loader.py
+-rw-r--r--   0        0        0     1198 2024-05-19 00:11:15.199628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/__init__.py
+-rw-r--r--   0        0        0    30172 2024-05-19 00:11:15.199628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/bq_dataset.py
+-rw-r--r--   0        0        0     2055 2024-05-19 00:11:15.199628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/bq_dataset_test_utils.py
+-rw-r--r--   0        0        0     4475 2024-05-19 00:11:15.199628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/bq_utils.py
+-rw-r--r--   0        0        0    36573 2024-05-19 00:11:15.199628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/feature_metadata.py
+-rw-r--r--   0        0        0     1570 2024-05-19 00:11:15.199628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/README.md
+-rw-r--r--   0        0        0  3671818 2024-05-19 00:11:15.211628 spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/covertype_pnu_10000.csv
+-rw-r--r--   0        0        0 36719403 2024-05-19 00:11:15.335627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/covertype_pnu_100000.csv
+-rw-r--r--   0        0        0  3689614 2024-05-19 00:11:15.347627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/covertype_pu_labeled.csv
+-rw-r--r--   0        0        0   582290 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/drug_train_pu_labeled.csv
+-rw-r--r--   0        0        0    42111 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/thyroid_labeled.csv
+-rw-r--r--   0        0        0    11656 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/occ_ensemble.py
+-rw-r--r--   0        0        0     9364 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/parameters.py
+-rw-r--r--   0        0        0      746 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/requirements.txt
+-rw-r--r--   0        0        0    23357 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/runner.py
+-rwxr-xr-x   0        0        0     1146 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/scripts/build_and_push_image.sh
+-rw-r--r--   0        0        0     3578 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/scripts/run_cloud_spade_experiment.sh
+-rw-r--r--   0        0        0     6333 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/supervised_model.py
+-rw-r--r--   0        0        0    11178 2024-05-19 00:11:15.351627 spade_anomaly_detection-0.2.1/spade_anomaly_detection/task.py
+-rw-r--r--   0        0        0    16300 1970-01-01 00:00:00.000000 spade_anomaly_detection-0.2.1/PKG-INFO
```

### Comparing `spade_anomaly_detection-0.2.0/LICENSE` & `spade_anomaly_detection-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/README.md` & `spade_anomaly_detection-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/pyproject.toml` & `spade_anomaly_detection-0.2.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 [project]
 # Project metadata. Available keys are documented at:
 # https://packaging.python.org/en/latest/specifications/declaring-project-metadata
 name = "spade_anomaly_detection"
-version = "0.2.0"
 description = "Semi-supervised Pseudo Labeler Anomaly Detection with Ensembling (SPADE) is a semi-supervised anomaly detection method that uses an ensemble of one class classifiers as the pseudo-labelers and supervised classifiers to achieve state of the art results especially on datasets with distribution mismatch between labeled and unlabeled samples."
 readme = "README.md"
 requires-python = ">=3.8"
 license = {file = "LICENSE"}
 authors = [{name = "spade_anomaly_detection authors", email="spade_anomaly_detection@google.com"}]
 classifiers = [  # List of https://pypi.org/classifiers/
     "License :: OSI Approved :: Apache Software License",
@@ -31,15 +30,15 @@
   "google-cloud-bigquery-storage[pandas,pyarrow,fastavro]==2.24.0",
   "google-cloud-storage==2.14.0",
   "cloudml-hypertune==0.1.0.dev6",
   "tensorflow_decision_forests==1.3.0"
 ]
 
 # `version` is automatically set by flit to use `spade_anomaly_detection.__version__`
-# dynamic = ["version"]
+dynamic = ["version"]
 
 [project.urls]
 homepage = "https://github.com/google-research/spade_anomaly_detection"
 repository = "https://github.com/google-research/spade_anomaly_detection"
 changelog = "https://github.com/google-research/spade_anomaly_detection/blob/main/CHANGELOG.md"
 # documentation = ""
```

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/Dockerfile` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/Dockerfile`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/__init__.py` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,8 +27,8 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """spade_anomaly_detection API."""
 
 # A new PyPI release will be pushed every time `__version__` is increased.
 # When changing this, also update the CHANGELOG.md.
-__version__ = '0.1.0'
+__version__ = '0.2.1'
```

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_loader.py` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -324,16 +324,17 @@
   def load_tf_dataset_from_bigquery(
       self,
       input_path: str,
       label_col_name: str,
       where_statements: Optional[List[str]] = None,
       ignore_columns: Optional[Sequence[str]] = None,
       batch_size: Optional[int] = None,
-      label_column_filter_value: Optional[int] = None,
+      label_column_filter_value: Optional[int | list[int]] = None,
       convert_features_to_float64: bool = False,
+      page_size: Optional[int] = None,
   ) -> tf.data.Dataset:
     """Loads a TensorFlow dataset from a BigQuery Table.
 
     Args:
       input_path: BigQuery string in the format 'project.dataset.table'.
       label_col_name: The name of the label column in the input BigQuery table.
       where_statements: A sequence of SQL where clauses that you wish to apply
@@ -342,53 +343,71 @@
         returned dataset. Default is None, meaning all columns are included.
       batch_size: The number of records the generator returns in a single call.
         Tune this depending on the size of the machines memory the algorithm is
         being executed on. The default value is None, which means that the
         dataset is not batched. In this case, when iterating through the
         dataset, it will yield one record per call instead of a batch of
         records.
-      label_column_filter_value: An integer used when filtering the label column
-        values. No value will result in all data returned from the table.
+      label_column_filter_value: An integer or list of integers used when
+        filtering the label column values. No value will result in all data
+        returned from the table.
       convert_features_to_float64: Set to True to cast the contents of the
         features columns to float64.
+      page_size: the pagination size to use when retrieving data from BigQuery.
+        A large value can result in fewer BQ calls, hence time savings.
 
     Returns:
       A TensorFlow dataset.
     """
     metadata_retrieval_options = None
 
     metadata_builder = None
 
     if label_column_filter_value is not None:
       where_statements = (
           list() if where_statements is None else where_statements
       )
-      where_statements.append(f'{label_col_name} = {label_column_filter_value}')
+      if isinstance(label_column_filter_value, int):
+        where_statements.append(
+            f'{label_col_name} = {label_column_filter_value}'
+        )
+      else:
+        where_statements.append(
+            f'CAST({label_col_name} AS INT64) IN '
+            f'UNNEST({label_column_filter_value})'
+        )
 
     if ignore_columns is not None:
       metadata_builder = feature_metadata.BigQueryMetadataBuilder(
           project_id=self.table_parts.project_id,
           bq_dataset_name=self.table_parts.bq_dataset_name,
           bq_table_name=self.table_parts.bq_table_name,
           ignore_columns=ignore_columns,
       )
 
     if where_statements:
-      metadata_retrieval_options = feature_metadata.MetadataRetrievalOptions(
-          where_clauses=where_statements
+      metadata_retrieval_options = (
+          feature_metadata.MetadataRetrievalOptions.get_none(
+              where_clauses=where_statements
+          )
       )
 
     tf_dataset, metadata = bq_dataset.get_dataset_and_metadata_for_table(
         table_path=input_path,
         batch_size=batch_size,
         with_mask=False,
         drop_remainder=True,
         metadata_options=metadata_retrieval_options,
         metadata_builder=metadata_builder,
+        page_size=page_size,
     )
+    options = tf.data.Options()
+    # Avoid a large warning output by TF Dataset.
+    options.deterministic = False
+    tf_dataset = tf_dataset.with_options(options)
 
     self.input_feature_metadata = metadata
 
     preprocess_fn = functools.partial(
         self._preprocess,
         label_col_name=label_col_name,
         convert_label_to_int=False,
```

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/__init__.py` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/bq_dataset.py` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/bq_dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -717,28 +717,31 @@
     metadata_options: Optional[
         feature_metadata.MetadataRetrievalOptions
     ] = None,
     metadata_builder: Optional[feature_metadata.BigQueryMetadataBuilder] = None,
     batch_size: int = 64,
     with_mask: bool = _WITH_MASK_DEFAULT,
     drop_remainder: bool = False,
+    page_size: Optional[int] = None,
 ) -> Tuple[tf.data.Dataset, feature_metadata.BigQueryTableMetadata]:
   """Gets the metadata and dataset for a BigQuery table.
 
   Args:
     table_path: The full path ('project.dataset.table') of the BigQuery table.
     table_parts: The parsed potions of the BigQuery table path.
     bigquery_client: The BigQuery Client object to use for getting the metadata.
     bigquery_storage_client: The BigQuery storage client to use for the dataset.
     metadata_options: The metadata retrieval options to use.
     metadata_builder: The metadata builder to use to get the metadata.
     batch_size: The batch size to use for the dataset. Default is 64.
     with_mask: Whether the dataset should be returned with a mask format. For
       more information see get_bigquery_dataset.
     drop_remainder: If true no partial batches will be yielded.
+    page_size: the pagination size to use when retrieving data from BigQuery. A
+      large value can result in fewer BQ calls, hence time savings.
 
   Returns:
     A tuple of the output dataset and metadata for the specified table.
 
   Raises:
     ValueError: If neither table_parts nor table_path are specified or both of
       them are.
@@ -779,10 +782,11 @@
       bqstorage_client=bigquery_storage_client,
       batch_size=batch_size,
       with_mask=with_mask,
       # Cache during prepare_dataset instead.
       cache_location=None,
       where_clauses=metadata_options.where_clauses,
       drop_remainder=drop_remainder,
+      page_size=page_size,
   )
 
   return dataset, all_metadata
```

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/bq_dataset_test_utils.py` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/bq_dataset_test_utils.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/bq_utils.py` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/bq_utils.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/data_utils/feature_metadata.py` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/data_utils/feature_metadata.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/README.md` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/README.md`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/covertype_pnu_10000.csv` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/covertype_pnu_10000.csv`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/covertype_pnu_100000.csv` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/covertype_pnu_100000.csv`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/covertype_pu_labeled.csv` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/covertype_pu_labeled.csv`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/drug_train_pu_labeled.csv` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/drug_train_pu_labeled.csv`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/example_data/thyroid_labeled.csv` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/example_data/thyroid_labeled.csv`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/occ_ensemble.py` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/occ_ensemble.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/parameters.py` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/parameters.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/requirements.txt` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/requirements.txt`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/runner.py` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/runner.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/scripts/build_and_push_image.sh` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/scripts/build_and_push_image.sh`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/scripts/run_cloud_spade_experiment.sh` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/scripts/run_cloud_spade_experiment.sh`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/supervised_model.py` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/supervised_model.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/spade_anomaly_detection/task.py` & `spade_anomaly_detection-0.2.1/spade_anomaly_detection/task.py`

 * *Files identical despite different names*

### Comparing `spade_anomaly_detection-0.2.0/PKG-INFO` & `spade_anomaly_detection-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: spade_anomaly_detection
-Version: 0.2.0
+Version: 0.2.1
 Summary: Semi-supervised Pseudo Labeler Anomaly Detection with Ensembling (SPADE) is a semi-supervised anomaly detection method that uses an ensemble of one class classifiers as the pseudo-labelers and supervised classifiers to achieve state of the art results especially on datasets with distribution mismatch between labeled and unlabeled samples.
 Keywords: anomaly detection,ensemble model,one class classifiers
 Author-email: spade_anomaly_detection authors <spade_anomaly_detection@google.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Intended Audience :: Science/Research
```

