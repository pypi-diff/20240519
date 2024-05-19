# Comparing `tmp/phc-ingestion-0.8.8.tar.gz` & `tmp/phc-ingestion-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "phc-ingestion-0.8.8.tar", last modified: Mon Apr 29 10:13:02 2024, max compression
+gzip compressed data, was "phc-ingestion-0.8.9.tar", last modified: Wed May  1 21:02:45 2024, max compression
```

## Comparing `phc-ingestion-0.8.8.tar` & `phc-ingestion-0.8.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
--rw-r--r--   0        0        0       16 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/PYPI.md
--rw-r--r--   0        0        0        0 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/__init__.py
--rw-r--r--   0        0        0       61 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/__init__.py
--rw-r--r--   0        0        0     1257 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/process.py
--rw-r--r--   0        0        0        0 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/__init__.py
--rw-r--r--   0        0        0     4441 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/cnv.py
--rw-r--r--   0        0        0     1640 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/detect_genome_ref.py
--rw-r--r--   0        0        0      507 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/ga4gh.py
--rw-r--r--   0        0        0      770 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/hla.py
--rw-r--r--   0        0        0    12312 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/ihc.py
--rw-r--r--   0        0        0      555 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/interpretation.py
--rw-r--r--   0        0        0     4706 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/json.py
--rw-r--r--   0        0        0     9536 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/metadata.py
--rw-r--r--   0        0        0     2051 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/specimen_details.py
--rw-r--r--   0        0        0     4599 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/structural.py
--rw-r--r--   0        0        0      482 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/tar.py
--rw-r--r--   0        0        0      372 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/tests.py
--rw-r--r--   0        0        0     1027 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/tmb.py
--rw-r--r--   0        0        0     1595 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/tsv.py
--rw-r--r--   0        0        0     3440 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/caris/util/vcf.py
--rw-r--r--   0        0        0       49 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/foundation/__init__.py
--rw-r--r--   0        0        0     3151 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/foundation/process.py
--rw-r--r--   0        0        0        0 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/foundation/util/__init__.py
--rw-r--r--   0        0        0     4215 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/foundation/util/cnv.py
--rw-r--r--   0        0        0     5937 2024-04-29 10:12:29.487288 phc-ingestion-0.8.8/ingestion/foundation/util/fnv.py
--rw-r--r--   0        0        0    10987 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/foundation/util/ga4gh.py
--rw-r--r--   0        0        0      405 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/foundation/util/interpretation.py
--rw-r--r--   0        0        0     2163 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/foundation/util/vcf_etl.py
--rw-r--r--   0        0        0        0 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/generic/__init__.py
--rw-r--r--   0        0        0     1548 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/generic/process.py
--rw-r--r--   0        0        0     2814 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/generic/utils.py
--rw-r--r--   0        0        0       46 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/nextgen/__init__.py
--rw-r--r--   0        0        0     3074 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/nextgen/process.py
--rw-r--r--   0        0        0     3484 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/nextgen/util/alteration_table.py
--rw-r--r--   0        0        0      297 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/nextgen/util/interpretation.py
--rw-r--r--   0        0        0     1132 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/nextgen/util/manifest_helpers.py
--rw-r--r--   0        0        0     2287 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/nextgen/util/process_cnv.py
--rw-r--r--   0        0        0     8346 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/nextgen/util/process_manifest.py
--rw-r--r--   0        0        0     5566 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/nextgen/util/process_structural.py
--rw-r--r--   0        0        0     7344 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/nextgen/util/process_vcf.py
--rw-r--r--   0        0        0       22 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/nextgen/util/types.py
--rw-r--r--   0        0        0   408290 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/resources/GRCh37_map.csv.gz
--rw-r--r--   0        0        0   612373 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/resources/GRCh38_map.csv.gz
--rw-r--r--   0        0        0        0 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/shared_util/__init__.py
--rw-r--r--   0        0        0     1669 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/shared_util/coords_to_genes.py
--rw-r--r--   0        0        0      876 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/shared_util/gene_to_coords.py
--rw-r--r--   0        0        0      162 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/shared_util/open_maybe_gzipped.py
--rw-r--r--   0        0        0       68 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/shared_util/types.py
--rw-r--r--   0        0        0     5398 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/vcf_standardization/Variant.py
--rw-r--r--   0        0        0        0 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/vcf_standardization/__init__.py
--rw-r--r--   0        0        0     2289 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/vcf_standardization/standardize.py
--rw-r--r--   0        0        0        0 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/vcf_standardization/util/__init__.py
--rw-r--r--   0        0        0     1061 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/vcf_standardization/util/af_helpers.py
--rw-r--r--   0        0        0      823 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/vcf_standardization/util/dp_helpers.py
--rw-r--r--   0        0        0     2471 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/ingestion/vcf_standardization/util/read_write.py
--rw-r--r--   0        0        0     1009 2024-04-29 10:12:29.491288 phc-ingestion-0.8.8/pyproject.toml
--rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-05-01 21:02:22.042424 phc-ingestion-0.8.9/PYPI.md
+-rw-r--r--   0        0        0        0 2024-05-01 21:02:22.042424 phc-ingestion-0.8.9/ingestion/__init__.py
+-rw-r--r--   0        0        0       61 2024-05-01 21:02:22.042424 phc-ingestion-0.8.9/ingestion/caris/__init__.py
+-rw-r--r--   0        0        0     1257 2024-05-01 21:02:22.042424 phc-ingestion-0.8.9/ingestion/caris/process.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:02:22.042424 phc-ingestion-0.8.9/ingestion/caris/util/__init__.py
+-rw-r--r--   0        0        0     4441 2024-05-01 21:02:22.042424 phc-ingestion-0.8.9/ingestion/caris/util/cnv.py
+-rw-r--r--   0        0        0     1640 2024-05-01 21:02:22.042424 phc-ingestion-0.8.9/ingestion/caris/util/detect_genome_ref.py
+-rw-r--r--   0        0        0      507 2024-05-01 21:02:22.042424 phc-ingestion-0.8.9/ingestion/caris/util/ga4gh.py
+-rw-r--r--   0        0        0      770 2024-05-01 21:02:22.042424 phc-ingestion-0.8.9/ingestion/caris/util/hla.py
+-rw-r--r--   0        0        0    12312 2024-05-01 21:02:22.042424 phc-ingestion-0.8.9/ingestion/caris/util/ihc.py
+-rw-r--r--   0        0        0      555 2024-05-01 21:02:22.042424 phc-ingestion-0.8.9/ingestion/caris/util/interpretation.py
+-rw-r--r--   0        0        0     4706 2024-05-01 21:02:22.042424 phc-ingestion-0.8.9/ingestion/caris/util/json.py
+-rw-r--r--   0        0        0     9536 2024-05-01 21:02:22.042424 phc-ingestion-0.8.9/ingestion/caris/util/metadata.py
+-rw-r--r--   0        0        0     2051 2024-05-01 21:02:22.042424 phc-ingestion-0.8.9/ingestion/caris/util/specimen_details.py
+-rw-r--r--   0        0        0     4599 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/caris/util/structural.py
+-rw-r--r--   0        0        0      482 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/caris/util/tar.py
+-rw-r--r--   0        0        0      372 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/caris/util/tests.py
+-rw-r--r--   0        0        0     1027 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/caris/util/tmb.py
+-rw-r--r--   0        0        0     1595 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/caris/util/tsv.py
+-rw-r--r--   0        0        0     3440 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/caris/util/vcf.py
+-rw-r--r--   0        0        0       49 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/foundation/__init__.py
+-rw-r--r--   0        0        0     3151 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/foundation/process.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/foundation/util/__init__.py
+-rw-r--r--   0        0        0     4215 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/foundation/util/cnv.py
+-rw-r--r--   0        0        0     5937 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/foundation/util/fnv.py
+-rw-r--r--   0        0        0    10987 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/foundation/util/ga4gh.py
+-rw-r--r--   0        0        0      405 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/foundation/util/interpretation.py
+-rw-r--r--   0        0        0     2163 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/foundation/util/vcf_etl.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/generic/__init__.py
+-rw-r--r--   0        0        0     1548 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/generic/process.py
+-rw-r--r--   0        0        0     2814 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/generic/utils.py
+-rw-r--r--   0        0        0       46 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/nextgen/__init__.py
+-rw-r--r--   0        0        0     3074 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/nextgen/process.py
+-rw-r--r--   0        0        0     3484 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/nextgen/util/alteration_table.py
+-rw-r--r--   0        0        0      297 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/nextgen/util/interpretation.py
+-rw-r--r--   0        0        0     1132 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/nextgen/util/manifest_helpers.py
+-rw-r--r--   0        0        0     2287 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/nextgen/util/process_cnv.py
+-rw-r--r--   0        0        0     8346 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/nextgen/util/process_manifest.py
+-rw-r--r--   0        0        0     5566 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/nextgen/util/process_structural.py
+-rw-r--r--   0        0        0     7890 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/nextgen/util/process_vcf.py
+-rw-r--r--   0        0        0       22 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/nextgen/util/types.py
+-rw-r--r--   0        0        0   408290 2024-05-01 21:02:22.046424 phc-ingestion-0.8.9/ingestion/resources/GRCh37_map.csv.gz
+-rw-r--r--   0        0        0   612373 2024-05-01 21:02:22.050424 phc-ingestion-0.8.9/ingestion/resources/GRCh38_map.csv.gz
+-rw-r--r--   0        0        0        0 2024-05-01 21:02:22.050424 phc-ingestion-0.8.9/ingestion/shared_util/__init__.py
+-rw-r--r--   0        0        0     1669 2024-05-01 21:02:22.050424 phc-ingestion-0.8.9/ingestion/shared_util/coords_to_genes.py
+-rw-r--r--   0        0        0      876 2024-05-01 21:02:22.050424 phc-ingestion-0.8.9/ingestion/shared_util/gene_to_coords.py
+-rw-r--r--   0        0        0      162 2024-05-01 21:02:22.050424 phc-ingestion-0.8.9/ingestion/shared_util/open_maybe_gzipped.py
+-rw-r--r--   0        0        0       68 2024-05-01 21:02:22.050424 phc-ingestion-0.8.9/ingestion/shared_util/types.py
+-rw-r--r--   0        0        0     5398 2024-05-01 21:02:22.050424 phc-ingestion-0.8.9/ingestion/vcf_standardization/Variant.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:02:22.050424 phc-ingestion-0.8.9/ingestion/vcf_standardization/__init__.py
+-rw-r--r--   0        0        0     2289 2024-05-01 21:02:22.050424 phc-ingestion-0.8.9/ingestion/vcf_standardization/standardize.py
+-rw-r--r--   0        0        0        0 2024-05-01 21:02:22.050424 phc-ingestion-0.8.9/ingestion/vcf_standardization/util/__init__.py
+-rw-r--r--   0        0        0     1061 2024-05-01 21:02:22.050424 phc-ingestion-0.8.9/ingestion/vcf_standardization/util/af_helpers.py
+-rw-r--r--   0        0        0      823 2024-05-01 21:02:22.050424 phc-ingestion-0.8.9/ingestion/vcf_standardization/util/dp_helpers.py
+-rw-r--r--   0        0        0     2471 2024-05-01 21:02:22.050424 phc-ingestion-0.8.9/ingestion/vcf_standardization/util/read_write.py
+-rw-r--r--   0        0        0     1009 2024-05-01 21:02:22.050424 phc-ingestion-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0      269 1970-01-01 00:00:00.000000 phc-ingestion-0.8.9/PKG-INFO
```

### Comparing `phc-ingestion-0.8.8/ingestion/caris/process.py` & `phc-ingestion-0.8.9/ingestion/caris/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/caris/util/cnv.py` & `phc-ingestion-0.8.9/ingestion/caris/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/caris/util/detect_genome_ref.py` & `phc-ingestion-0.8.9/ingestion/caris/util/detect_genome_ref.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/caris/util/hla.py` & `phc-ingestion-0.8.9/ingestion/caris/util/hla.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/caris/util/ihc.py` & `phc-ingestion-0.8.9/ingestion/caris/util/ihc.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/caris/util/interpretation.py` & `phc-ingestion-0.8.9/ingestion/caris/util/interpretation.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/caris/util/json.py` & `phc-ingestion-0.8.9/ingestion/caris/util/json.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/caris/util/metadata.py` & `phc-ingestion-0.8.9/ingestion/caris/util/metadata.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/caris/util/specimen_details.py` & `phc-ingestion-0.8.9/ingestion/caris/util/specimen_details.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/caris/util/structural.py` & `phc-ingestion-0.8.9/ingestion/caris/util/structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/caris/util/tmb.py` & `phc-ingestion-0.8.9/ingestion/caris/util/tmb.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/caris/util/tsv.py` & `phc-ingestion-0.8.9/ingestion/caris/util/tsv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/caris/util/vcf.py` & `phc-ingestion-0.8.9/ingestion/caris/util/vcf.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/foundation/process.py` & `phc-ingestion-0.8.9/ingestion/foundation/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/foundation/util/cnv.py` & `phc-ingestion-0.8.9/ingestion/foundation/util/cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/foundation/util/fnv.py` & `phc-ingestion-0.8.9/ingestion/foundation/util/fnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/foundation/util/ga4gh.py` & `phc-ingestion-0.8.9/ingestion/foundation/util/ga4gh.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/foundation/util/vcf_etl.py` & `phc-ingestion-0.8.9/ingestion/foundation/util/vcf_etl.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/generic/process.py` & `phc-ingestion-0.8.9/ingestion/generic/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/generic/utils.py` & `phc-ingestion-0.8.9/ingestion/generic/utils.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/nextgen/process.py` & `phc-ingestion-0.8.9/ingestion/nextgen/process.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/nextgen/util/alteration_table.py` & `phc-ingestion-0.8.9/ingestion/nextgen/util/alteration_table.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/nextgen/util/manifest_helpers.py` & `phc-ingestion-0.8.9/ingestion/nextgen/util/manifest_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/nextgen/util/process_cnv.py` & `phc-ingestion-0.8.9/ingestion/nextgen/util/process_cnv.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/nextgen/util/process_manifest.py` & `phc-ingestion-0.8.9/ingestion/nextgen/util/process_manifest.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/nextgen/util/process_structural.py` & `phc-ingestion-0.8.9/ingestion/nextgen/util/process_structural.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/nextgen/util/process_vcf.py` & `phc-ingestion-0.8.9/ingestion/nextgen/util/process_vcf.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import gzip
+import re
 import shutil
 from logging import Logger
+
 from ingestion.nextgen.util.alteration_table import extract_variant_table
 
 
 class Variant:
     def __init__(self, fields):
         self.chr_pos = fields[0]
         self.info = []
@@ -115,15 +117,19 @@
 
         elif sequence_type == "germline":
             working.calculate_af()
             working.prune_var()
 
         if sequence_type == "somatic" and not short_variant_table.empty:
             split_var[7] = add_vendsig_to_info(
-                working.pruned_info, short_variant_table, split_var[0], int(split_var[1])
+                working.pruned_info,
+                short_variant_table,
+                split_var[0],
+                int(split_var[1]),
+                log,
             )
         else:
             split_var[7] = f"{working.pruned_info};VENDSIG=Unknown"
         split_var[8] = working.pruned_frmt
         split_var[9] = working.pruned_smpl
         vcf_out.append("\t".join(split_var))
 
@@ -184,19 +190,35 @@
         return "VENDSIG=Likely pathogenic"
     elif vendsig in ["VUS"]:
         return "VENDSIG=Uncertain significance"
     else:
         raise RuntimeError(f"Unable to map vendor significance: {vendsig}")
 
 
-def add_vendsig_to_info(info: str, short_var_table, chrom: str, pos: str) -> str:
+def extract_chrom_pos_from_gene_string(chr_pos: str, log: Logger) -> tuple[str, int]:
+    """
+    Parses chromosome and position from a gene string from the alteration table.
+
+    Returns ("", 0) if no match is found.
+    """
+
+    pattern = r"^.*\((chr\d+):(\d+).*\).*$"
+    match = re.match(pattern, chr_pos)
+    if not match:
+        log.warn(f"Failed to extract chrom and pos from gene string")
+        return ("", 0)
+    chrom = match.group(1)
+    pos = int(match.group(2))
+    return (chrom, pos)
+
+
+def add_vendsig_to_info(info: str, short_var_table, chrom: str, pos: int, log: Logger) -> str:
     mapped_vendsig = None
     for index, row in short_var_table.iterrows():
-        ref_chrom = row["gene"].split(" ")[1].split(":")[0].strip("(")
-        ref_pos = int(row["gene"].split(" ")[1].split(":")[1])
+        ref_chrom, ref_pos = extract_chrom_pos_from_gene_string(row["gene"], log)
 
         if ref_chrom == chrom:
             if ref_pos == pos or ref_pos + 1 == pos or ref_pos - 1 == pos:
                 mapped_vendsig = map_vendsig(row["info"])
 
     if not mapped_vendsig:
         mapped_vendsig = "VENDSIG=Unknown"
```

### Comparing `phc-ingestion-0.8.8/ingestion/resources/GRCh37_map.csv.gz` & `phc-ingestion-0.8.9/ingestion/resources/GRCh37_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/resources/GRCh38_map.csv.gz` & `phc-ingestion-0.8.9/ingestion/resources/GRCh38_map.csv.gz`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/shared_util/coords_to_genes.py` & `phc-ingestion-0.8.9/ingestion/shared_util/coords_to_genes.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/shared_util/gene_to_coords.py` & `phc-ingestion-0.8.9/ingestion/shared_util/gene_to_coords.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/vcf_standardization/Variant.py` & `phc-ingestion-0.8.9/ingestion/vcf_standardization/Variant.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/vcf_standardization/standardize.py` & `phc-ingestion-0.8.9/ingestion/vcf_standardization/standardize.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/vcf_standardization/util/af_helpers.py` & `phc-ingestion-0.8.9/ingestion/vcf_standardization/util/af_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/vcf_standardization/util/dp_helpers.py` & `phc-ingestion-0.8.9/ingestion/vcf_standardization/util/dp_helpers.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/ingestion/vcf_standardization/util/read_write.py` & `phc-ingestion-0.8.9/ingestion/vcf_standardization/util/read_write.py`

 * *Files identical despite different names*

### Comparing `phc-ingestion-0.8.8/pyproject.toml` & `phc-ingestion-0.8.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "phc-ingestion"
-version = "0.8.8"
+version = "0.8.9"
 description = "Functions for LifeOmic PHC genomic ingestions"
 authors = [
     { name = "LifeOmic Development", email = "development@lifeomic.com" },
 ]
 dependencies = [
     "lifeomic-logging>=0.3.2,<0.4.0",
     "xmltodict==0.13.0",
```

