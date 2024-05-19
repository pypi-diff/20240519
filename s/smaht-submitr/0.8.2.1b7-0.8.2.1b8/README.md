# Comparing `tmp/smaht_submitr-0.8.2.1b7.tar.gz` & `tmp/smaht_submitr-0.8.2.1b8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smaht_submitr-0.8.2.1b7.tar", max compression
+gzip compressed data, was "smaht_submitr-0.8.2.1b8.tar", max compression
```

## Comparing `smaht_submitr-0.8.2.1b7.tar` & `smaht_submitr-0.8.2.1b8.tar`

### file list

```diff
@@ -1,68 +1,70 @@
--rw-r--r--   0        0        0     1098 2024-05-17 20:22:50.753718 smaht_submitr-0.8.2.1b7/LICENSE.txt
--rw-r--r--   0        0        0     2602 2024-05-17 20:22:50.753718 smaht_submitr-0.8.2.1b7/README.rst
--rw-r--r--   0        0        0     3465 2024-05-17 20:22:50.793718 smaht_submitr-0.8.2.1b7/pyproject.toml
--rw-r--r--   0        0        0        0 2024-05-17 20:22:50.793718 smaht_submitr-0.8.2.1b7/submitr/__init__.py
--rw-r--r--   0        0        0      731 2024-05-17 20:22:50.793718 smaht_submitr-0.8.2.1b7/submitr/base.py
--rw-r--r--   0        0        0      294 2024-05-17 20:22:50.793718 smaht_submitr-0.8.2.1b7/submitr/exceptions.py
--rw-r--r--   0        0        0    17885 2024-05-17 20:22:50.793718 smaht_submitr-0.8.2.1b7/submitr/file_for_upload.py
--rw-r--r--   0        0        0    11097 2024-05-17 20:22:50.793718 smaht_submitr-0.8.2.1b7/submitr/metadata_template.py
--rw-r--r--   0        0        0     2628 2024-05-17 20:22:50.793718 smaht_submitr-0.8.2.1b7/submitr/output.py
--rw-r--r--   0        0        0      353 2024-05-17 20:22:50.793718 smaht_submitr-0.8.2.1b7/submitr/rclone/__init__.py
--rw-r--r--   0        0        0     6343 2024-05-17 20:22:50.793718 smaht_submitr-0.8.2.1b7/submitr/rclone/rclone_amazon.py
--rw-r--r--   0        0        0     9291 2024-05-17 20:22:50.793718 smaht_submitr-0.8.2.1b7/submitr/rclone/rclone_commands.py
--rw-r--r--   0        0        0     6986 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/rclone/rclone_config.py
--rw-r--r--   0        0        0     9916 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/rclone/rclone_google.py
--rw-r--r--   0        0        0     5152 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/rclone/rclone_installation.py
--rw-r--r--   0        0        0     3187 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/rclone/rclone_utils.py
--rw-r--r--   0        0        0    11817 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/rclone/rcloner.py
--rw-r--r--   0        0        0    19885 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/rclone/testing/rclone_utils_for_testing_amazon.py
--rw-r--r--   0        0        0     8157 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/rclone/testing/rclone_utils_for_testing_google.py
--rw-r--r--   0        0        0    17135 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/s3_upload.py
--rw-r--r--   0        0        0     3512 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/s3_utils.py
--rw-r--r--   0        0        0        0 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/scripts/__init__.py
--rw-r--r--   0        0        0     4779 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/scripts/check_submission.py
--rw-r--r--   0        0        0     9895 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/scripts/cli_utils.py
--rw-r--r--   0        0        0     2824 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/scripts/get_metadata_template.py
--rw-r--r--   0        0        0     1822 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/scripts/list_submissions.py
--rw-r--r--   0        0        0      940 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/scripts/make_sample_fastq_file.py
--rw-r--r--   0        0        0     5483 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/scripts/rcloner.py
--rw-r--r--   0        0        0     7143 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/scripts/resume_uploads.py
--rw-r--r--   0        0        0     1368 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/scripts/show_upload_info.py
--rw-r--r--   0        0        0     1572 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/scripts/submit_genelist.py
--rw-r--r--   0        0        0    21810 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/scripts/submit_metadata_bundle.py
--rw-r--r--   0        0        0     3437 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/scripts/submit_ontology.py
--rw-r--r--   0        0        0     1616 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/scripts/upload_item_data.py
--rw-r--r--   0        0        0    28731 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/scripts/view_portal_object.py
--rw-r--r--   0        0        0   127795 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/submission.py
--rw-r--r--   0        0        0    14817 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/submission_uploads.py
--rw-r--r--   0        0        0        0 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/__init__.py
--rw-r--r--   0        0        0      355 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/conftest_settings.py
--rw-r--r--   0        0        0      163 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/data/f1_R1.fastq.gz
--rw-r--r--   0        0        0      165 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/data/f1_R2.fastq.gz
--rw-r--r--   0        0        0      167 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/data/f2_R1.fastq.gz
--rw-r--r--   0        0        0      164 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/data/f2_R2.fastq.gz
--rw-r--r--   0        0        0      272 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/data/simulated_bundle.json
--rw-r--r--   0        0        0    10870 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/data/submission_simple.xlsx
--rw-r--r--   0        0        0    10875 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/data/submission_simple2.xlsx
--rw-r--r--   0        0        0    13306 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/data/submission_test.xlsx
--rw-r--r--   0        0        0    13192 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/data/submission_test_with_errors.xlsx
--rw-r--r--   0        0        0      169 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/data/test1_R1.fastq.gz
--rw-r--r--   0        0        0      168 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/data/test1_R2.fastq.gz
--rw-r--r--   0        0        0     1333 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/test_base.py
--rw-r--r--   0        0        0     2629 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/test_check_submission.py
--rw-r--r--   0        0        0      551 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/test_exceptions.py
--rw-r--r--   0        0        0    12067 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/test_file_for_upload.py
--rw-r--r--   0        0        0     1620 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/test_make_sample_fastq_file.py
--rw-r--r--   0        0        0     1421 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/test_misc.py
--rw-r--r--   0        0        0    43766 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/test_rclone_support.py
--rw-r--r--   0        0        0    11766 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/test_resume_uploads.py
--rw-r--r--   0        0        0    37993 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/test_submission.py
--rw-r--r--   0        0        0     2836 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/test_submit_genelist.py
--rw-r--r--   0        0        0     6874 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/test_submit_metadata_bundle.py
--rw-r--r--   0        0        0     3013 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/test_submit_ontology.py
--rw-r--r--   0        0        0     1300 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/test_testing_helpers.py
--rw-r--r--   0        0        0     4353 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/test_utils.py
--rw-r--r--   0        0        0     1351 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/testing_helpers.py
--rw-r--r--   0        0        0     3863 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/tests/testing_rclone_helpers.py
--rw-r--r--   0        0        0     8677 2024-05-17 20:22:50.797718 smaht_submitr-0.8.2.1b7/submitr/utils.py
--rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 smaht_submitr-0.8.2.1b7/PKG-INFO
+-rw-r--r--   0        0        0     1098 2024-05-19 01:57:37.499175 smaht_submitr-0.8.2.1b8/LICENSE.txt
+-rw-r--r--   0        0        0     2602 2024-05-19 01:57:37.499175 smaht_submitr-0.8.2.1b8/README.rst
+-rw-r--r--   0        0        0     3465 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/__init__.py
+-rw-r--r--   0        0        0      731 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/base.py
+-rw-r--r--   0        0        0      294 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/exceptions.py
+-rw-r--r--   0        0        0    17885 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/file_for_upload.py
+-rw-r--r--   0        0        0    11097 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/metadata_template.py
+-rw-r--r--   0        0        0     2628 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/output.py
+-rw-r--r--   0        0        0      353 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/__init__.py
+-rw-r--r--   0        0        0     6343 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_amazon.py
+-rw-r--r--   0        0        0     9391 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_commands.py
+-rw-r--r--   0        0        0     6986 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_config.py
+-rw-r--r--   0        0        0     9916 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_google.py
+-rw-r--r--   0        0        0     5152 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_installation.py
+-rw-r--r--   0        0        0     3348 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_utils.py
+-rw-r--r--   0        0        0    11817 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/rcloner.py
+-rw-r--r--   0        0        0    19885 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/testing/rclone_utils_for_testing_amazon.py
+-rw-r--r--   0        0        0     8157 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/rclone/testing/rclone_utils_for_testing_google.py
+-rw-r--r--   0        0        0    17135 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/s3_upload.py
+-rw-r--r--   0        0        0     3512 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/s3_utils.py
+-rw-r--r--   0        0        0        0 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/__init__.py
+-rw-r--r--   0        0        0     4779 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/check_submission.py
+-rw-r--r--   0        0        0     9895 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/cli_utils.py
+-rw-r--r--   0        0        0     2824 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/get_metadata_template.py
+-rw-r--r--   0        0        0     1822 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/list_submissions.py
+-rw-r--r--   0        0        0      940 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/make_sample_fastq_file.py
+-rw-r--r--   0        0        0     5483 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/rcloner.py
+-rw-r--r--   0        0        0     7143 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/resume_uploads.py
+-rw-r--r--   0        0        0     1368 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/show_upload_info.py
+-rw-r--r--   0        0        0     1572 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/submit_genelist.py
+-rw-r--r--   0        0        0    21810 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3437 2024-05-19 01:57:37.539176 smaht_submitr-0.8.2.1b8/submitr/scripts/submit_ontology.py
+-rw-r--r--   0        0        0     1616 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/scripts/upload_item_data.py
+-rw-r--r--   0        0        0    28731 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/scripts/view_portal_object.py
+-rw-r--r--   0        0        0   127795 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/submission.py
+-rw-r--r--   0        0        0    14817 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/submission_uploads.py
+-rw-r--r--   0        0        0        0 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/__init__.py
+-rw-r--r--   0        0        0      355 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/conftest_settings.py
+-rw-r--r--   0        0        0      163 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/data/f1_R1.fastq.gz
+-rw-r--r--   0        0        0      165 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/data/f1_R2.fastq.gz
+-rw-r--r--   0        0        0      167 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/data/f2_R1.fastq.gz
+-rw-r--r--   0        0        0      164 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/data/f2_R2.fastq.gz
+-rw-r--r--   0        0        0     6395 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/data/ingestion_submission.json
+-rw-r--r--   0        0        0  1032804 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/data/profiles.json
+-rw-r--r--   0        0        0      272 2024-05-19 01:57:37.543176 smaht_submitr-0.8.2.1b8/submitr/tests/data/simulated_bundle.json
+-rw-r--r--   0        0        0    10870 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_simple.xlsx
+-rw-r--r--   0        0        0    10875 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_simple2.xlsx
+-rw-r--r--   0        0        0    13306 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_test.xlsx
+-rw-r--r--   0        0        0    13192 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_test_with_errors.xlsx
+-rw-r--r--   0        0        0      169 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/data/test1_R1.fastq.gz
+-rw-r--r--   0        0        0      168 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/data/test1_R2.fastq.gz
+-rw-r--r--   0        0        0     1333 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_base.py
+-rw-r--r--   0        0        0     2629 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_check_submission.py
+-rw-r--r--   0        0        0      551 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_exceptions.py
+-rw-r--r--   0        0        0    12067 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_file_for_upload.py
+-rw-r--r--   0        0        0     1620 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_make_sample_fastq_file.py
+-rw-r--r--   0        0        0     1421 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_misc.py
+-rw-r--r--   0        0        0    48503 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_rclone_support.py
+-rw-r--r--   0        0        0    11766 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_resume_uploads.py
+-rw-r--r--   0        0        0    37993 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_submission.py
+-rw-r--r--   0        0        0     2836 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_submit_genelist.py
+-rw-r--r--   0        0        0     6874 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_submit_metadata_bundle.py
+-rw-r--r--   0        0        0     3013 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_submit_ontology.py
+-rw-r--r--   0        0        0     1300 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_testing_helpers.py
+-rw-r--r--   0        0        0     4353 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/test_utils.py
+-rw-r--r--   0        0        0     1351 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/testing_helpers.py
+-rw-r--r--   0        0        0     5085 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/tests/testing_rclone_helpers.py
+-rw-r--r--   0        0        0     8677 2024-05-19 01:57:37.547176 smaht_submitr-0.8.2.1b8/submitr/utils.py
+-rw-r--r--   0        0        0     4030 1970-01-01 00:00:00.000000 smaht_submitr-0.8.2.1b8/PKG-INFO
```

### Comparing `smaht_submitr-0.8.2.1b7/LICENSE.txt` & `smaht_submitr-0.8.2.1b8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/README.rst` & `smaht_submitr-0.8.2.1b8/README.rst`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/pyproject.toml` & `smaht_submitr-0.8.2.1b8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smaht-submitr"
-version = "0.8.2.1b7"  # TODO: To become 0.8.3
+version = "0.8.2.1b8"  # TODO: To become 0.8.3
 description = "Support for uploading file submissions to SMAHT."
 # TODO: Update this email address when a more specific one is available for SMaHT.
 authors = ["SMaHT DAC <smhelp@hms-dbmi.atlassian.net >"]
 license = "MIT"
 readme = "README.rst"
 keywords = ["submitr", "smaht"]
 homepage = "https://github.com/smaht-dac/submitr"
```

### Comparing `smaht_submitr-0.8.2.1b7/submitr/base.py` & `smaht_submitr-0.8.2.1b8/submitr/base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/file_for_upload.py` & `smaht_submitr-0.8.2.1b8/submitr/file_for_upload.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/metadata_template.py` & `smaht_submitr-0.8.2.1b8/submitr/metadata_template.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/output.py` & `smaht_submitr-0.8.2.1b8/submitr/output.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/rclone/rclone_amazon.py` & `smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_amazon.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/rclone/rclone_commands.py` & `smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,14 +141,15 @@
     def _execute(command: List[str]) -> subprocess.CompletedProcess:
         DEBUG(f"RCLONE-COMMAND: {' '.join(command)}")
         result = subprocess.run(command, capture_output=True, universal_newlines=True)
         DEBUG(f"RCLONE-COMMAND-OUTPUT: {normalize_string(result.stdout)}")
         DEBUG(f"RCLONE-COMMAND-RESULT: {result.returncode}")
         return result
 
+    # All this parsing stuff is so that we can use our dcicutils.progress_bar with the rclone copy.
     _RCLONE_PROGRESS_UNITS = {"KiB": 2**10, "MiB": 2**20, "GiB": 2**30, "TiB": 2**40, "PiB": 2**50, "B": 1}
     _RCLONE_PROGRESS_PATTERN = rf".*Transferred:\s*(\d+(?:\.\d+)?)\s*({'|'.join(_RCLONE_PROGRESS_UNITS.keys())}).*"
     _RCLONE_PROGRESS_REGEX = re.compile(_RCLONE_PROGRESS_PATTERN)
     _RCLONE_SIZE_PATERN = r".*\((\d+) Byte\)"
     _RCLONE_SIZE_REGEX = re.compile(_RCLONE_SIZE_PATERN)
 
     @staticmethod
```

### Comparing `smaht_submitr-0.8.2.1b7/submitr/rclone/rclone_config.py` & `smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_config.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/rclone/rclone_google.py` & `smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_google.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -56,22 +56,22 @@
         # Override from RCloneConfig base class because for some reason with this ping command,
         # for which we actually use rclone lsd, we need to specify the project_number for Google.
         args = ["--gcs-project-number", project] if (project := self.project) else None
         with self.config_file() as config_file:
             return RCloneCommands.ping_command(source=f"{self.name}:", config=config_file, args=args)
 
     @property
-    def location(self) -> Optional[str]:
-        return self.credentials.location if self.credentials else None
-
-    @property
     def service_account_file(self) -> Optional[str]:
         return self.credentials.service_account_file if self.credentials else None
 
     @property
+    def location(self) -> Optional[str]:
+        return self.credentials.location if self.credentials else None
+
+    @property
     def project(self) -> Optional[str]:
         """
         Returns the Google project name (or number - either) associated with the account identified
         by the service account file (if any) or with the system (e.g. if running on a GCE instance).
         FYI only place needed was for rclone lsd comment which we use as a ping.
         """
         if self._project:
```

### Comparing `smaht_submitr-0.8.2.1b7/submitr/rclone/rclone_installation.py` & `smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_installation.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/rclone/rclone_utils.py` & `smaht_submitr-0.8.2.1b8/submitr/rclone/rclone_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,17 @@
         if value := cloud_path.normalize(value):
             if (separator_index := value.find(cloud_path.separator)) > 0:
                 return value[separator_index + 1:]
         return ""
 
     @staticmethod
     def bucket_and_key(bucket: str, key: Optional[str] = None) -> Tuple[Optional[str], Optional[str]]:
+        if isinstance(bucket, str):
+            if bucket.lower().startswith("s3://") or bucket.lower().startswith("gs://"):
+                bucket = bucket[5:]
         if not (bucket_and_key := cloud_path.join(bucket, key)):
             return None, None
         if cloud_path.has_separator(bucket_and_key):
             bucket = cloud_path.bucket(bucket_and_key)
             key = cloud_path.key(bucket_and_key)
             return bucket, key
         else:
```

### Comparing `smaht_submitr-0.8.2.1b7/submitr/rclone/rcloner.py` & `smaht_submitr-0.8.2.1b8/submitr/rclone/rcloner.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/rclone/testing/rclone_utils_for_testing_amazon.py` & `smaht_submitr-0.8.2.1b8/submitr/rclone/testing/rclone_utils_for_testing_amazon.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/rclone/testing/rclone_utils_for_testing_google.py` & `smaht_submitr-0.8.2.1b8/submitr/rclone/testing/rclone_utils_for_testing_google.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/s3_upload.py` & `smaht_submitr-0.8.2.1b8/submitr/s3_upload.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/s3_utils.py` & `smaht_submitr-0.8.2.1b8/submitr/s3_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/scripts/check_submission.py` & `smaht_submitr-0.8.2.1b8/submitr/scripts/check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/scripts/cli_utils.py` & `smaht_submitr-0.8.2.1b8/submitr/scripts/cli_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/scripts/get_metadata_template.py` & `smaht_submitr-0.8.2.1b8/submitr/scripts/get_metadata_template.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/scripts/list_submissions.py` & `smaht_submitr-0.8.2.1b8/submitr/scripts/list_submissions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/scripts/make_sample_fastq_file.py` & `smaht_submitr-0.8.2.1b8/submitr/scripts/make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/scripts/rcloner.py` & `smaht_submitr-0.8.2.1b8/submitr/scripts/rcloner.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/scripts/resume_uploads.py` & `smaht_submitr-0.8.2.1b8/submitr/scripts/resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/scripts/show_upload_info.py` & `smaht_submitr-0.8.2.1b8/submitr/scripts/show_upload_info.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/scripts/submit_genelist.py` & `smaht_submitr-0.8.2.1b8/submitr/scripts/submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/scripts/submit_metadata_bundle.py` & `smaht_submitr-0.8.2.1b8/submitr/scripts/submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/scripts/submit_ontology.py` & `smaht_submitr-0.8.2.1b8/submitr/scripts/submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/scripts/upload_item_data.py` & `smaht_submitr-0.8.2.1b8/submitr/scripts/upload_item_data.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/scripts/view_portal_object.py` & `smaht_submitr-0.8.2.1b8/submitr/scripts/view_portal_object.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/submission.py` & `smaht_submitr-0.8.2.1b8/submitr/submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/submission_uploads.py` & `smaht_submitr-0.8.2.1b8/submitr/submission_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/data/submission_simple.xlsx` & `smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_simple.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/data/submission_simple2.xlsx` & `smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_simple2.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/data/submission_test.xlsx` & `smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_test.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/data/submission_test_with_errors.xlsx` & `smaht_submitr-0.8.2.1b8/submitr/tests/data/submission_test_with_errors.xlsx`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/test_base.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/test_check_submission.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/test_check_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/test_exceptions.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/test_exceptions.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/test_file_for_upload.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/test_file_for_upload.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/test_make_sample_fastq_file.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/test_make_sample_fastq_file.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/test_misc.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/test_misc.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/test_rclone_support.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/test_rclone_support.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,31 +1,35 @@
 from contextlib import contextmanager
 from enum import Enum
 import json
 import os
 import pytest
 from typing import Optional, Tuple
+from unittest.mock import patch as mock_patch
 from dcicutils.file_utils import are_files_equal, compute_file_md5, normalize_path
-from dcicutils.misc_utils import create_short_uuid
+from dcicutils.misc_utils import create_uuid
 from dcicutils.tmpfile_utils import (
     create_temporary_file_name, remove_temporary_file,
     temporary_directory, temporary_file, temporary_random_file)
 from submitr.file_for_upload import FilesForUpload
 from submitr.rclone.rcloner import RCloner
 from submitr.rclone.rclone_config import RCloneConfig
 from submitr.rclone.rclone_amazon import AmazonCredentials, RCloneAmazon
 from submitr.rclone.rclone_google import GoogleCredentials, RCloneGoogle
 from submitr.rclone.rclone_utils import cloud_path
 from submitr.rclone.testing.rclone_utils_for_testing_amazon import AwsCredentials, AwsS3
 from submitr.rclone.testing.rclone_utils_for_testing_google import GcpCredentials, Gcs
 from submitr.rclone.rclone_installation import RCloneInstallation
 from submitr.s3_upload import upload_file_to_aws_s3
 from submitr.s3_utils import get_s3_key_metadata
-from submitr.tests.testing_rclone_helpers import (
-    setup_module as rclone_setup_module, teardown_module as rclone_teardown_module, Mock_LocalStorage)
+import submitr.submission_uploads  # noqa
+from submitr.submission_uploads import do_any_uploads  # noqa/xyzzy
+from submitr.tests.testing_rclone_helpers import (  # noqa/xyzzy
+    setup_module as rclone_setup_module, teardown_module as rclone_teardown_module,
+    load_test_data_json, Mock_LocalStorage, Mock_Portal, RANDOM_TMPFILE_SIZE)
 
 
 pytestmark = pytest.mark.integration
 
 
 # Integration tests for RCloner related functionality within smaht-submitr.
 # Need valid AWS credentials (currently for: smaht-wolf).
@@ -77,15 +81,15 @@
             yield tmp_file_path, os.path.basename(tmp_file_path)
 
     def file_name_to_key_name(self, file_name: str) -> str:
         # Assumed that the given file name is just that, a file base name, not a path name.
         if not (self.use_cloud_subfolder_key is True):
             return file_name
         else:
-            return cloud_path.join(f"{Env.test_file_prefix}{create_short_uuid(length=8)}", file_name)
+            return cloud_path.join(f"{Env.test_file_prefix}{create_uuid()}", file_name)
 
 
 class EnvAmazon(Env):
 
     class CredentialsType(Enum):
         TEMPORARY = "temporary"
         TEMPORARY_KEY_SPECIFIC = "temporary-key-specific"
@@ -610,48 +614,89 @@
             assert are_files_equal(tmp_test_file_path, tmp_destination_file)
         with temporary_directory() as tmp_destination_directory:
             RCloner().copy(tmp_test_file_path, tmp_destination_directory, copyto=False)
             assert are_files_equal(tmp_test_file_path,
                                    os.path.join(tmp_destination_directory, os.path.basename(tmp_test_file_path)))
 
 
-def test_rclone_google_to_amazon_more() -> None:
-
-    filesize = 1235
+def test_rclone_local_to_google_copy_to_bucket() -> None:
+    # Just an aside (ran across while testing); make sure copyto=False works for sub-folder.
+    filesize = 1234
+    env_google = EnvGoogle()
     filesystem = Mock_LocalStorage()
-    file_one = "subdir/test_file_one.fastq"
-    file_two = "test_file_two.fastq"
-    filesystem.create_files(file_one, nbytes=filesize)
-    # env_amazon = EnvAmazon(use_cloud_subfolder_key=True)
-    env_google = EnvGoogle(use_cloud_subfolder_key=True)
-    bucket_google = f"{env_google.bucket}/test-{create_short_uuid(31)}"
+    filesystem.create_files(file_one := "subdir/test_file_one.fastq", nbytes=filesize)
+    # Bucket is really "bucket" - bucket plus optional sub-folder, which RCloneConfig is designed to handle.
+    subfolder = f"test-{create_uuid()}"
+    bucket_google = cloud_path.join(env_google.bucket, subfolder)
     credentials_google = env_google.credentials()
     rclone_google = RCloneGoogle(credentials_google, bucket=bucket_google)
     rcloner = RCloner(destination=rclone_google)
+    assert rcloner.copy_to_bucket(os.path.join(filesystem.root, file_one)) is True
+    assert env_google.gcs_non_rclone().file_exists(cloud_path.join(bucket_google, os.path.basename(file_one))) is True
+    assert env_google.gcs_non_rclone().file_exists(bucket_google, os.path.basename(file_one)) is True
+    assert env_google.gcs_non_rclone().file_size(cloud_path.join(bucket_google, os.path.basename(file_one))) == filesize
+    assert env_google.gcs_non_rclone().file_size(bucket_google, os.path.basename(file_one)) == filesize
+    assert (env_google.gcs_non_rclone().file_checksum(cloud_path.join(bucket_google, os.path.basename(file_one))) ==
+            compute_file_md5(os.path.join(filesystem.root, file_one)))
+    assert env_google.gcs_non_rclone().delete_file(rclone_google.bucket, os.path.basename(file_one)) is True
+    assert env_google.gcs_non_rclone().file_exists(rclone_google.bucket, os.path.basename(file_one)) is False
+
+
+def test_rclone_local_to_amazon_copy_to_bucket() -> None:
+    # Just an aside (ran across while testing); make sure copyto=False works for sub-folder.
+    filesize = 1236
+    env_amazon = EnvAmazon()
+    filesystem = Mock_LocalStorage()
+    filesystem.create_files(file_one := "subdir/test_file_one.fastq", nbytes=filesize)
+    # Bucket is really "bucket" - bucket plus optional sub-folder, which RCloneConfig is designed to handle.
+    subfolder = f"test-{create_uuid()}"
+    bucket_amazon = cloud_path.join(env_amazon.bucket, subfolder)
+    credentials_amazon = env_amazon.credentials()
+    rclone_amazon = RCloneAmazon(credentials_amazon, bucket=bucket_amazon)
+    rcloner = RCloner(destination=rclone_amazon)
+    assert rcloner.copy_to_bucket(os.path.join(filesystem.root, file_one)) is True
+    assert env_amazon.s3_non_rclone().file_exists(cloud_path.join(bucket_amazon, os.path.basename(file_one))) is True
+    assert env_amazon.s3_non_rclone().file_exists(bucket_amazon, os.path.basename(file_one)) is True
+    assert env_amazon.s3_non_rclone().file_size(cloud_path.join(bucket_amazon, os.path.basename(file_one))) == filesize
+    assert env_amazon.s3_non_rclone().file_size(bucket_amazon, os.path.basename(file_one)) == filesize
+    assert (env_amazon.s3_non_rclone().file_checksum(cloud_path.join(bucket_amazon, os.path.basename(file_one))) ==
+            compute_file_md5(os.path.join(filesystem.root, file_one)))
+    assert env_amazon.s3_non_rclone().delete_file(bucket_amazon, os.path.basename(file_one)) is True
+    assert env_amazon.s3_non_rclone().file_exists(bucket_amazon, os.path.basename(file_one)) is False
+
+
+def test_rclone_upload_file_to_aws_s3() -> None:
+
+    filesystem = Mock_LocalStorage(file_one := "subdir/test_file_one.fastq",
+                                   file_two := "test_file_two.fastq",
+                                   nbytes=(filesize := 1235))
+    env_google = EnvGoogle()
+    bucket_google = f"{env_google.bucket}/test-{create_uuid()}"
+    rclone_google = RCloneGoogle(env_google.credentials(), bucket=bucket_google)
+    rcloner = RCloner(destination=rclone_google)
     # Note that the second destination argument to RCloner.copy can be
     # unspecified meaning that it will be the *bucket* ("bucket" - can be
     assert rcloner.copy_to_bucket(os.path.join(filesystem.root, file_one)) is True
     assert env_google.gcs_non_rclone().file_size(cloud_path.join(bucket_google, os.path.basename(file_one))) == filesize
     assert env_google.gcs_non_rclone().file_size(bucket_google, os.path.basename(file_one)) == filesize
-    files = [{"filename": file_one},
-             {"filename": file_two}]
+    files = [{"filename": file_one}, {"filename": file_two}]
     files_for_upload = FilesForUpload.assemble(files,
                                                main_search_directory=filesystem.root,
                                                main_search_directory_recursively=True,
                                                config_google=rclone_google)
     assert len(files_for_upload) == 2
     assert files_for_upload[0].found is True
     assert files_for_upload[0].found_local is True
     assert files_for_upload[0].found_google is True
     assert files_for_upload[0].path_local == os.path.join(filesystem.root, file_one)
     assert files_for_upload[0].size_local == filesize
-    assert len(files_for_upload[0].checksum_local) > 0
+    assert files_for_upload[0].checksum_local == compute_file_md5(os.path.join(filesystem.root, file_one))
     assert files_for_upload[0].path_google == cloud_path.join(bucket_google, files_for_upload[0].name)
     assert files_for_upload[0].size_google == filesize
-    assert len(files_for_upload[0].checksum_google) > 0
+    assert files_for_upload[0].checksum_google == compute_file_md5(os.path.join(filesystem.root, file_one))
     # Found both locally and in Google; ambiguous, as favor_local starts as None;
     # so these return False/None; favor_local normally gets resolved in review function.
     assert files_for_upload[0].favor_local is None
     assert files_for_upload[0].from_local is False
     assert files_for_upload[0].from_google is False
     assert files_for_upload[0].path is None
     assert files_for_upload[0].size is None
@@ -665,80 +710,106 @@
     assert len(files_for_upload[0].checksum) > 0
     files_for_upload[0]._favor_local = False  # normally resolved by FileForUpload.review
     assert files_for_upload[0].favor_local is False
     assert files_for_upload[0].from_local is False
     assert files_for_upload[0].from_google is True
     assert files_for_upload[0].path == cloud_path.join(rclone_google.bucket, files_for_upload[0].name)
     assert files_for_upload[0].size == filesize
-    assert len(files_for_upload[0].checksum) > 0
+    assert files_for_upload[0].checksum == compute_file_md5(os.path.join(filesystem.root, file_one))
+    assert files_for_upload[1].found is True
+    assert files_for_upload[1].found_local is True
+    assert files_for_upload[1].found_google is False
+    assert files_for_upload[1].favor_local is True
+    assert files_for_upload[1].from_local is True
+    assert files_for_upload[1].from_google is False
+    assert files_for_upload[1].path == os.path.join(filesystem.root, file_two)
+    assert files_for_upload[1].size == filesize
+    assert files_for_upload[1].checksum == compute_file_md5(os.path.join(filesystem.root, file_two))
 
     env_amazon = EnvAmazon()
-    s3_key = f"test-{create_short_uuid(31)}/SMAFIPIGC8NG.fastq"
+    s3_key = f"test-{create_uuid()}/SMAFIPIGC8NG.fastq"
     s3_uri = f"s3://{env_amazon.bucket}/{s3_key}"
     credentials_amazon = env_amazon.temporary_credentials(env_amazon.bucket, s3_key)
     # FYI the output of this looks something like this (but not specifically checking for now):
     # ▶ Upload: test_file_one.fastq (1.21 KB) ...
     #   - From: gs://smaht-submitr-rclone-testing/test_file_one.fastq
     #   -   To: s3://smaht-unit-testing-files/test-9eFJ8iZHG5ayrTEuSvz7G4upKVJdtpJ/SMAFIPIGC8NG.fastq
     # ▶ Upload progress ✓ 100% ◀|###########| 1234/1235 | 1.16 MB/s | 00:00 | ETA: 00:00
     # ▶ Upload progress ✓ 100% ◀|###########| 1235/1235 | 3.53 KB/s | 00:00 | ETA: 00:00
     # Verifying upload: test_file_one.fastq ... OK
     upload_file_to_aws_s3(file=files_for_upload[0],
                           s3_uri=s3_uri,
-                          aws_credentials=credentials_amazon.to_dictionary())
+                          aws_credentials=credentials_amazon.to_dictionary(environment_names=True))
     assert env_amazon.s3_non_rclone().file_exists(env_amazon.bucket, s3_key) is True
     assert env_amazon.s3_non_rclone().file_size(env_amazon.bucket, s3_key) == filesize
     assert (env_amazon.s3_non_rclone().file_checksum(env_amazon.bucket, s3_key) ==
             compute_file_md5(os.path.join(filesystem.root, file_one)))
     s3_key_metadata = get_s3_key_metadata(credentials_amazon.to_dictionary(environment_names=False),
                                           env_amazon.bucket, s3_key)
     assert isinstance(s3_key_metadata, dict)
     assert s3_key_metadata["size"] == filesize
     assert s3_key_metadata["size"] == filesize
     assert s3_key_metadata["md5"] == compute_file_md5(os.path.join(filesystem.root, file_one))
     assert s3_key_metadata["md5_source"] == "google-cloud-storage"
-    assert env_amazon.s3_non_rclone().delete_file(env_amazon.bucket, s3_key)
-    assert env_google.gcs_non_rclone().delete_file(rclone_google.bucket, files_for_upload[0].name)
+    assert env_amazon.s3_non_rclone().delete_file(env_amazon.bucket, s3_key) is True
+    assert env_amazon.s3_non_rclone().file_exists(env_amazon.bucket, s3_key) is False
+    assert env_google.gcs_non_rclone().delete_file(rclone_google.bucket, files_for_upload[0].name) is True
+    assert env_google.gcs_non_rclone().file_exists(rclone_google.bucket, files_for_upload[0].name) is False
 
 
-def test_rclone_local_to_google_copy_to_bucket() -> None:
-    # Just an aside (ran across while testing); make sure copyto=False works for sub-folder.
-    filesize = 1234
-    env_google = EnvGoogle(use_cloud_subfolder_key=True)
+def test_rclone_do_any_uploads() -> None:
     filesystem = Mock_LocalStorage()
-    filesystem.create_files(file_one := "subdir/test_file_one.fastq", nbytes=filesize)
-    # Bucket is really "bucket" - bucket plus optional sub-folder, which RCloneConfig is designed to handle.
-    subfolder = f"test-{create_short_uuid(31)}"
-    bucket_google = cloud_path.join(env_google.bucket, subfolder)
-    credentials_google = env_google.credentials()
-    rclone_google = RCloneGoogle(credentials_google, bucket=bucket_google)
+    metadata_file = "metadata_file.xlsx"
+    test_file_subdirectory = "subdir"
+    test_file_one = "test_file_one.fastq"
+    test_file_two = "test_file_two.fastq"
+    filesystem.create_files(file_one := os.path.join(test_file_subdirectory, test_file_one), metadata_file)
+    env_google = EnvGoogle()
+    env_amazon = EnvAmazon()
+    rclone_google = RCloneGoogle(env_google.credentials(), bucket=f"{env_google.bucket}/test-{create_uuid()}")
     rcloner = RCloner(destination=rclone_google)
-    assert rcloner.copy_to_bucket(os.path.join(filesystem.root, file_one)) is True
-    assert env_google.gcs_non_rclone().file_exists(cloud_path.join(bucket_google, os.path.basename(file_one))) is True
-    assert env_google.gcs_non_rclone().file_exists(bucket_google, os.path.basename(file_one)) is True
-    assert env_google.gcs_non_rclone().file_size(cloud_path.join(bucket_google, os.path.basename(file_one))) == filesize
-    assert env_google.gcs_non_rclone().file_size(bucket_google, os.path.basename(file_one)) == filesize
-    assert (env_google.gcs_non_rclone().file_checksum(cloud_path.join(bucket_google, os.path.basename(file_one))) ==
-            compute_file_md5(os.path.join(filesystem.root, file_one)))
-    assert env_google.gcs_non_rclone().delete_file(rclone_google.bucket, os.path.basename(file_one))
-
+    assert rcloner.copy_to_key(filesystem.path(file_one), key_google := test_file_two) is True
+    assert env_google.gcs_non_rclone().file_exists(rclone_google.bucket, key_google) is True
+    assert env_google.gcs_non_rclone().file_size(rclone_google.bucket, key_google) == RANDOM_TMPFILE_SIZE
+
+    uploaded_uris_amazon = []
+
+    def mocked_generate_credentials_for_upload(file, uuid, portal):
+        nonlocal env_amazon, uploaded_uris_amazon
+        bucket_amazon = f"{env_amazon.bucket}/test-{create_uuid()}"
+        key_amazon = f"SMA-{create_uuid()}.fastq"
+        aws_s3_uri = f"s3://{bucket_amazon}/{key_amazon}"
+        uploaded_uris_amazon.append(aws_s3_uri)
+        aws_credentials = env_amazon.temporary_credentials(bucket_amazon,
+                                                           key_amazon).to_dictionary(environment_names=True)
+        aws_kms_key_id = AMAZON_KMS_KEY_ID
+        return aws_s3_uri, aws_credentials, aws_kms_key_id
 
-def test_rclone_local_to_amazon_copy_to_bucket() -> None:
-    # Just an aside (ran across while testing); make sure copyto=False works for sub-folder.
-    filesize = 1236
-    env_amazon = EnvAmazon(use_cloud_subfolder_key=True)
-    filesystem = Mock_LocalStorage()
-    filesystem.create_files(file_one := "subdir/test_file_one.fastq", nbytes=filesize)
-    # Bucket is really "bucket" - bucket plus optional sub-folder, which RCloneConfig is designed to handle.
-    subfolder = f"test-{create_short_uuid(31)}"
-    bucket_amazon = cloud_path.join(env_amazon.bucket, subfolder)
-    credentials_amazon = env_amazon.credentials()
-    rclone_amazon = RCloneAmazon(credentials_amazon, bucket=bucket_amazon)
-    rcloner = RCloner(destination=rclone_amazon)
-    assert rcloner.copy_to_bucket(os.path.join(filesystem.root, file_one)) is True
-    assert env_amazon.s3_non_rclone().file_exists(cloud_path.join(bucket_amazon, os.path.basename(file_one))) is True
-    assert env_amazon.s3_non_rclone().file_exists(bucket_amazon, os.path.basename(file_one)) is True
-    assert env_amazon.s3_non_rclone().file_size(cloud_path.join(bucket_amazon, os.path.basename(file_one))) == filesize
-    assert env_amazon.s3_non_rclone().file_size(bucket_amazon, os.path.basename(file_one)) == filesize
-    assert (env_amazon.s3_non_rclone().file_checksum(cloud_path.join(bucket_amazon, os.path.basename(file_one))) ==
-            compute_file_md5(os.path.join(filesystem.root, file_one)))
-    assert env_amazon.s3_non_rclone().delete_file(bucket_amazon, os.path.basename(file_one))
+    # TODO
+    # To call do_any_uploads we need a Portal object which needs mock its get_schema_type, is_schema_type,
+    # is_schema_file_type functions; no need to mock get_metadata, patch_metadata, get_health, which are also
+    # called from submission_uploads module, so long as we don't pass a IngestionSubmission UUID to do_any_uploads,
+    # but rather pass files dictionary; and also need to mock submission_uploads.generate_credentials_for_upload.
+    # Alternatively, easier, is just provide a StructuredDataSet with a simple upload_files property which is an
+    # list of dictionary with file names.
+    with (mock_patch("submitr.submission_uploads.generate_credentials_for_upload") as mock_generate_credentials_for_upload,  # noqa
+          mock_patch("submitr.submission_uploads.yes_or_no", return_value="yes")):
+        ingestion_submission_object = load_test_data_json("ingestion_submission")  # noqa/xyzzy
+        mock_generate_credentials_for_upload.side_effect = mocked_generate_credentials_for_upload
+        do_any_uploads(ingestion_submission_object,
+                       metadata_file=metadata_file,
+                       main_search_directory=os.path.join(filesystem.root, test_file_subdirectory),
+                       main_search_directory_recursively=True,
+                       config_google=rclone_google,
+                       portal=Mock_Portal(),
+                       review_only=False,
+                       verbose=False)
+
+    for uploaded_uri_amazon in uploaded_uris_amazon:
+        bucket_amazon, key_amazon = cloud_path.bucket_and_key(uploaded_uri_amazon)
+        assert env_amazon.s3_non_rclone().file_exists(bucket_amazon, key_amazon) is True
+        assert env_amazon.s3_non_rclone().delete_file(bucket_amazon, key_amazon) is True
+        assert env_amazon.s3_non_rclone().file_exists(bucket_amazon, key_amazon) is False
+
+    # Cleanup.
+    assert env_google.gcs_non_rclone().delete_file(rclone_google.bucket, key_google) is True
+    assert env_google.gcs_non_rclone().file_exists(rclone_google.bucket, key_google) is False
```

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/test_resume_uploads.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/test_resume_uploads.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/test_submission.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/test_submission.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/test_submit_genelist.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/test_submit_genelist.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/test_submit_metadata_bundle.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/test_submit_metadata_bundle.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/test_submit_ontology.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/test_submit_ontology.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/test_testing_helpers.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/test_testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/test_utils.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/testing_helpers.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/testing_helpers.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/submitr/tests/testing_rclone_helpers.py` & `smaht_submitr-0.8.2.1b8/submitr/tests/testing_rclone_helpers.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,12 @@
+import json
 import os
 import tempfile
 from dcicutils.file_utils import create_random_file, compute_file_md5, get_file_size, normalize_path
+from dcicutils.structured_data import Portal
 from dcicutils.tmpfile_utils import (
     is_temporary_directory, remove_temporary_directory)
 from submitr.rclone import RCloneConfig, RCloneAmazon, RCloneGoogle
 
 TMPDIR = None
 RANDOM_TMPFILE_SIZE = 2048
 
@@ -79,14 +81,39 @@
 
 
 class Mock_LocalStorage(Mock_CloudStorage):
     # Might as well also use Mock_CloudStorage for easy
     # local file system test file setup for convenience.
     def __init__(self, *args, **kwargs):
         super().__init__(subdir="local")
+        self.create_files(*args, **kwargs)
     def create_files(self, *args, **kwargs):  # noqa
         super()._create_files_for_testing(*args, **kwargs)
     def create_file(self, *args, **kwargs):  # noqa
         super()._create_file_for_testing(*args, **kwargs)
     @property  # noqa
     def root(self):
         return super()._root()
+    def path(self, path):  # noqa
+        return os.path.join(self.root, path) if (path := normalize_path(path)) else None
+
+
+class Mock_Portal(Portal):
+    # Designed to handle calls to get_schemas, get_schema, get_schema_type, is_schema_type, is_schema_file_type.
+    # which can all be done be simply overriding get_schemas which reads a static/snapshot (2024-05-18) copy
+    # of the schemas as returned by the /profiles/ (trailing slash required there btw) endpoint.
+    def __init__(self):  # noqa
+        dummy_key = {"key": "dummy", "secret": "dummy"}
+        super().__init__(dummy_key)
+        self._schemas = None
+    def get_schemas(self) -> dict:  # noqa
+        if not self._schemas:
+            self._schemas = load_test_data_json("profiles")
+        return self._schemas
+
+
+def load_test_data_json(file):
+    this_directory = os.path.dirname(os.path.abspath(__file__))
+    test_data_directory = os.path.join(this_directory, "data")
+    test_data_file = os.path.join(test_data_directory, file if file.endswith(".json") else f"{file}.json")
+    with open(test_data_file, "r") as f:
+        return json.load(f)
```

### Comparing `smaht_submitr-0.8.2.1b7/submitr/utils.py` & `smaht_submitr-0.8.2.1b8/submitr/utils.py`

 * *Files identical despite different names*

### Comparing `smaht_submitr-0.8.2.1b7/PKG-INFO` & `smaht_submitr-0.8.2.1b8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smaht-submitr
-Version: 0.8.2.1b7
+Version: 0.8.2.1b8
 Summary: Support for uploading file submissions to SMAHT.
 Home-page: https://github.com/smaht-dac/submitr
 License: MIT
 Keywords: submitr,smaht
 Author: SMaHT DAC
 Author-email: smhelp@hms-dbmi.atlassian.net 
 Requires-Python: >=3.8.0,<3.13
```

