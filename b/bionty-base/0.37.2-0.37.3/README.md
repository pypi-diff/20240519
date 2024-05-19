# Comparing `tmp/bionty-base-0.37.2.tar.gz` & `tmp/bionty_base-0.37.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bionty-base-0.37.2.tar", last modified: Fri Apr  5 12:56:37 2024, max compression
+gzip compressed data, was "bionty_base-0.37.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `bionty-base-0.37.2.tar` & `bionty_base-0.37.3.tar`

### file list

```diff
@@ -1,84 +1,84 @@
--rw-r--r--   0        0        0     3169 2024-04-05 12:50:11.730131 bionty-base-0.37.2/.github/workflows/build.yml
--rw-r--r--   0        0        0      555 2024-03-07 15:08:48.176384 bionty-base-0.37.2/.github/workflows/check_ontologies_reachable.yml
--rw-r--r--   0        0        0      133 2024-03-07 15:08:48.176384 bionty-base-0.37.2/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-04-05 12:50:11.733464 bionty-base-0.37.2/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0      504 2024-04-05 12:50:11.733464 bionty-base-0.37.2/.github/workflows/update_ontologies.yml
--rw-r--r--   0        0        0     2115 2024-03-07 15:08:48.176384 bionty-base-0.37.2/.gitignore
--rw-r--r--   0        0        0     1512 2024-03-07 15:08:48.176384 bionty-base-0.37.2/.pre-commit-config.yaml
--rw-r--r--   0        0        0    11357 2024-03-07 15:08:48.176384 bionty-base-0.37.2/LICENSE
--rw-r--r--   0        0        0     3116 2024-03-07 15:08:48.176384 bionty-base-0.37.2/README.md
--rw-r--r--   0        0        0     1894 2024-04-05 12:51:42.647382 bionty-base-0.37.2/bionty_base/__init__.py
--rw-r--r--   0        0        0     1605 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/_display_sources.py
--rw-r--r--   0        0        0     3863 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/_ontology.py
--rw-r--r--   0        0        0    24162 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/_public_ontology.py
--rw-r--r--   0        0        0     2615 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/_settings.py
--rw-r--r--   0        0        0      524 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/_sync_sources.py
--rw-r--r--   0        0        0      111 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/dev/__init__.py
--rw-r--r--   0        0        0     8456 2024-03-21 12:01:31.389175 bionty-base-0.37.2/bionty_base/dev/_handle_sources.py
--rw-r--r--   0        0        0     5154 2024-03-21 12:01:31.389175 bionty-base-0.37.2/bionty_base/dev/_io.py
--rw-r--r--   0        0        0     1021 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/dev/_md5.py
--rw-r--r--   0        0        0        0 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/__init__.py
--rw-r--r--   0        0        0     1370 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_bfxpipeline.py
--rw-r--r--   0        0        0      682 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_biosample.py
--rw-r--r--   0        0        0      804 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_cellline.py
--rw-r--r--   0        0        0      728 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_cellmarker.py
--rw-r--r--   0        0        0      817 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_celltype.py
--rw-r--r--   0        0        0      913 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_developmentalstage.py
--rw-r--r--   0        0        0     1164 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_disease.py
--rw-r--r--   0        0        0      810 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_drug.py
--rw-r--r--   0        0        0      831 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_ethnicity.py
--rw-r--r--   0        0        0     4387 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_experimentalfactor.py
--rw-r--r--   0        0        0    10086 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_gene.py
--rw-r--r--   0        0        0     2570 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_organism.py
--rw-r--r--   0        0        0      855 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_pathway.py
--rw-r--r--   0        0        0     1420 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_phenotype.py
--rw-r--r--   0        0        0      685 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_protein.py
--rw-r--r--   0        0        0     1486 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_shared_docstrings.py
--rw-r--r--   0        0        0      799 2024-03-07 15:08:48.179717 bionty-base-0.37.2/bionty_base/entities/_tissue.py
--rw-r--r--   0        0        0    11067 2024-04-05 12:50:11.733464 bionty-base-0.37.2/bionty_base/sources/sources.yaml
--rw-r--r--   0        0        0    47474 2024-04-05 12:50:11.733464 bionty-base-0.37.2/docs/changelog.md
--rw-r--r--   0        0        0     1015 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/developer/updating_source.md
--rw-r--r--   0        0        0      200 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/guide.md
--rw-r--r--   0        0        0     3335 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/guide/comparison.md
--rw-r--r--   0        0        0     1455 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/guide/concepts.md
--rw-r--r--   0        0        0     3796 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/guide/config.md
--rw-r--r--   0        0        0     3694 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/guide/extend.md
--rw-r--r--   0        0        0     7453 2024-03-08 14:34:27.000329 bionty-base-0.37.2/docs/guide/ontology.ipynb
--rw-r--r--   0        0        0      358 2024-03-08 14:34:26.970329 bionty-base-0.37.2/docs/guide/search.ipynb
--rw-r--r--   0        0        0     7536 2024-03-08 14:34:27.026996 bionty-base-0.37.2/docs/guide/sources.ipynb
--rw-r--r--   0        0        0      160 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/guide/test_notebooks.py
--rw-r--r--   0        0        0      981 2024-03-08 14:34:27.026996 bionty-base-0.37.2/docs/guide/validate.ipynb
--rw-r--r--   0        0        0      126 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/index.md
--rw-r--r--   0        0        0       59 2024-03-07 15:08:48.179717 bionty-base-0.37.2/docs/reference.md
--rw-r--r--   0        0        0      146 2024-03-07 15:08:48.179717 bionty-base-0.37.2/lamin-project.yaml
--rw-r--r--   0        0        0      869 2024-04-04 08:31:23.478547 bionty-base-0.37.2/noxfile.py
--rw-r--r--   0        0        0     4093 2024-04-04 08:31:23.481881 bionty-base-0.37.2/pyproject.toml
--rw-r--r--   0        0        0      666 2024-03-07 15:08:48.179717 bionty-base-0.37.2/scripts/bfxpipelines_info/custom_pipelines.json
--rw-r--r--   0        0        0     1494 2024-03-07 15:08:48.179717 bionty-base-0.37.2/scripts/check_ontologies_reachable.py
--rw-r--r--   0        0        0     1290 2024-03-07 15:08:48.179717 bionty-base-0.37.2/scripts/determine_md5s.py
--rw-r--r--   0        0        0     3433 2024-03-07 15:08:48.179717 bionty-base-0.37.2/scripts/generate_bfxpipelines.py
--rw-r--r--   0        0        0     1127 2024-03-07 15:08:48.179717 bionty-base-0.37.2/scripts/update_new_ontologies.py
--rw-r--r--   0        0        0     1789 2024-03-07 15:08:48.179717 bionty-base-0.37.2/scripts/upload_new_ontologies.py
--rw-r--r--   0        0        0     6980 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/dev/test_handle_sources.py
--rw-r--r--   0        0        0      532 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/dev/test_io.py
--rw-r--r--   0        0        0      550 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_bfxpipeline.py
--rw-r--r--   0        0        0      163 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_biosample.py
--rw-r--r--   0        0        0      569 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_cellline.py
--rw-r--r--   0        0        0      918 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_cellmarker.py
--rw-r--r--   0        0        0      609 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_celltype.py
--rw-r--r--   0        0        0      632 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_developmentalstage.py
--rw-r--r--   0        0        0     2967 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_disease.py
--rw-r--r--   0        0        0      600 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_drug.py
--rw-r--r--   0        0        0      575 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_ethnicity.py
--rw-r--r--   0        0        0     1066 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_experimentalfactor.py
--rw-r--r--   0        0        0     2396 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_gene.py
--rw-r--r--   0        0        0      871 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_organism.py
--rw-r--r--   0        0        0     1179 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_pathway.py
--rw-r--r--   0        0        0     3020 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_phenotype.py
--rw-r--r--   0        0        0      579 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_protein.py
--rw-r--r--   0        0        0      596 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/entities/test_tissue.py
--rw-r--r--   0        0        0     1486 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/test_bionty.py
--rw-r--r--   0        0        0      627 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/test_lamindb.py
--rw-r--r--   0        0        0      767 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/test_md5.py
--rw-r--r--   0        0        0      418 2024-03-07 15:08:48.179717 bionty-base-0.37.2/tests/test_ontology.py
--rw-r--r--   0        0        0     4305 1970-01-01 00:00:00.000000 bionty-base-0.37.2/PKG-INFO
+-rw-r--r--   0        0        0     3169 2024-04-05 12:02:36.195663 bionty_base-0.37.3/.github/workflows/build.yml
+-rw-r--r--   0        0        0      555 2024-02-05 06:48:01.378180 bionty_base-0.37.3/.github/workflows/check_ontologies_reachable.yml
+-rw-r--r--   0        0        0      133 2024-02-05 06:48:01.378260 bionty_base-0.37.3/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-04-05 12:02:36.196803 bionty_base-0.37.3/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0      504 2024-04-05 12:02:36.197387 bionty_base-0.37.3/.github/workflows/update_ontologies.yml
+-rw-r--r--   0        0        0     2115 2024-02-05 06:48:01.378514 bionty_base-0.37.3/.gitignore
+-rw-r--r--   0        0        0     1512 2024-02-05 06:48:01.378597 bionty_base-0.37.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    11357 2024-02-05 06:48:01.378739 bionty_base-0.37.3/LICENSE
+-rw-r--r--   0        0        0     3116 2024-02-05 16:15:26.529099 bionty_base-0.37.3/README.md
+-rw-r--r--   0        0        0     1890 2024-05-19 08:47:29.354937 bionty_base-0.37.3/bionty_base/__init__.py
+-rw-r--r--   0        0        0     1605 2024-02-05 06:48:01.379069 bionty_base-0.37.3/bionty_base/_display_sources.py
+-rw-r--r--   0        0        0     3862 2024-05-15 10:24:22.301446 bionty_base-0.37.3/bionty_base/_ontology.py
+-rw-r--r--   0        0        0    23685 2024-05-15 10:24:22.302146 bionty_base-0.37.3/bionty_base/_public_ontology.py
+-rw-r--r--   0        0        0     2529 2024-05-15 12:40:17.107468 bionty_base-0.37.3/bionty_base/_settings.py
+-rw-r--r--   0        0        0      524 2024-02-05 06:48:01.379500 bionty_base-0.37.3/bionty_base/_sync_sources.py
+-rw-r--r--   0        0        0      111 2024-02-05 06:48:01.379634 bionty_base-0.37.3/bionty_base/dev/__init__.py
+-rw-r--r--   0        0        0     8456 2024-03-27 07:46:53.422612 bionty_base-0.37.3/bionty_base/dev/_handle_sources.py
+-rw-r--r--   0        0        0     5154 2024-03-27 07:46:53.423500 bionty_base-0.37.3/bionty_base/dev/_io.py
+-rw-r--r--   0        0        0     1021 2024-02-05 06:48:01.380009 bionty_base-0.37.3/bionty_base/dev/_md5.py
+-rw-r--r--   0        0        0        0 2024-02-05 06:48:01.380085 bionty_base-0.37.3/bionty_base/entities/__init__.py
+-rw-r--r--   0        0        0     1539 2024-05-15 10:24:22.302535 bionty_base-0.37.3/bionty_base/entities/_bfxpipeline.py
+-rw-r--r--   0        0        0      682 2024-02-05 06:48:01.380275 bionty_base-0.37.3/bionty_base/entities/_biosample.py
+-rw-r--r--   0        0        0      804 2024-02-05 06:48:01.380385 bionty_base-0.37.3/bionty_base/entities/_cellline.py
+-rw-r--r--   0        0        0      728 2024-02-05 06:48:01.380477 bionty_base-0.37.3/bionty_base/entities/_cellmarker.py
+-rw-r--r--   0        0        0      817 2024-02-05 06:48:01.380571 bionty_base-0.37.3/bionty_base/entities/_celltype.py
+-rw-r--r--   0        0        0      913 2024-02-05 06:48:01.380672 bionty_base-0.37.3/bionty_base/entities/_developmentalstage.py
+-rw-r--r--   0        0        0     1164 2024-02-05 06:48:01.380762 bionty_base-0.37.3/bionty_base/entities/_disease.py
+-rw-r--r--   0        0        0      810 2024-02-05 06:48:01.380840 bionty_base-0.37.3/bionty_base/entities/_drug.py
+-rw-r--r--   0        0        0      831 2024-02-05 06:48:01.380920 bionty_base-0.37.3/bionty_base/entities/_ethnicity.py
+-rw-r--r--   0        0        0     4349 2024-05-17 06:51:00.826274 bionty_base-0.37.3/bionty_base/entities/_experimentalfactor.py
+-rw-r--r--   0        0        0    10086 2024-02-05 06:48:01.381189 bionty_base-0.37.3/bionty_base/entities/_gene.py
+-rw-r--r--   0        0        0     2570 2024-02-05 06:48:01.381291 bionty_base-0.37.3/bionty_base/entities/_organism.py
+-rw-r--r--   0        0        0      855 2024-02-05 06:48:01.381377 bionty_base-0.37.3/bionty_base/entities/_pathway.py
+-rw-r--r--   0        0        0     1420 2024-02-05 06:48:01.381466 bionty_base-0.37.3/bionty_base/entities/_phenotype.py
+-rw-r--r--   0        0        0      685 2024-02-05 06:48:01.381538 bionty_base-0.37.3/bionty_base/entities/_protein.py
+-rw-r--r--   0        0        0     1486 2024-02-05 06:48:01.381623 bionty_base-0.37.3/bionty_base/entities/_shared_docstrings.py
+-rw-r--r--   0        0        0      799 2024-02-05 06:48:01.381715 bionty_base-0.37.3/bionty_base/entities/_tissue.py
+-rw-r--r--   0        0        0    13870 2024-05-17 06:51:00.826909 bionty_base-0.37.3/bionty_base/sources.yaml
+-rw-r--r--   0        0        0    50271 2024-05-17 06:51:00.827439 bionty_base-0.37.3/docs/changelog.md
+-rw-r--r--   0        0        0     1015 2024-02-05 06:48:01.382428 bionty_base-0.37.3/docs/developer/updating_source.md
+-rw-r--r--   0        0        0      200 2024-02-05 06:48:01.382533 bionty_base-0.37.3/docs/guide.md
+-rw-r--r--   0        0        0     3335 2024-02-05 06:48:01.382681 bionty_base-0.37.3/docs/guide/comparison.md
+-rw-r--r--   0        0        0     1455 2024-02-05 06:48:01.382797 bionty_base-0.37.3/docs/guide/concepts.md
+-rw-r--r--   0        0        0     3796 2024-02-05 06:48:01.382919 bionty_base-0.37.3/docs/guide/config.md
+-rw-r--r--   0        0        0     3694 2024-02-05 06:48:01.383015 bionty_base-0.37.3/docs/guide/extend.md
+-rw-r--r--   0        0        0     7453 2024-02-05 06:48:01.383225 bionty_base-0.37.3/docs/guide/ontology.ipynb
+-rw-r--r--   0        0        0      358 2024-02-05 06:48:01.383355 bionty_base-0.37.3/docs/guide/search.ipynb
+-rw-r--r--   0        0        0     7536 2024-02-05 06:48:01.383558 bionty_base-0.37.3/docs/guide/sources.ipynb
+-rw-r--r--   0        0        0      160 2024-02-05 06:48:01.383648 bionty_base-0.37.3/docs/guide/test_notebooks.py
+-rw-r--r--   0        0        0      981 2024-02-05 06:48:01.383731 bionty_base-0.37.3/docs/guide/validate.ipynb
+-rw-r--r--   0        0        0      126 2024-02-05 06:48:01.383842 bionty_base-0.37.3/docs/index.md
+-rw-r--r--   0        0        0       59 2024-02-05 06:48:01.383923 bionty_base-0.37.3/docs/reference.md
+-rw-r--r--   0        0        0      146 2024-02-05 06:48:01.384003 bionty_base-0.37.3/lamin-project.yaml
+-rw-r--r--   0        0        0      869 2024-03-27 07:46:53.424783 bionty_base-0.37.3/noxfile.py
+-rw-r--r--   0        0        0     4093 2024-03-27 07:46:53.424973 bionty_base-0.37.3/pyproject.toml
+-rw-r--r--   0        0        0     3079 2024-05-15 10:24:22.304374 bionty_base-0.37.3/scripts/bfxpipelines_info/custom_pipelines.json
+-rw-r--r--   0        0        0     1482 2024-05-15 12:40:17.108723 bionty_base-0.37.3/scripts/check_ontologies_reachable.py
+-rw-r--r--   0        0        0     1290 2024-02-05 06:48:01.384561 bionty_base-0.37.3/scripts/determine_md5s.py
+-rw-r--r--   0        0        0     3433 2024-02-05 06:48:01.384646 bionty_base-0.37.3/scripts/generate_bfxpipelines.py
+-rw-r--r--   0        0        0     1127 2024-02-05 06:48:01.384730 bionty_base-0.37.3/scripts/update_new_ontologies.py
+-rw-r--r--   0        0        0     1774 2024-05-15 10:24:22.304581 bionty_base-0.37.3/scripts/upload_new_ontologies.py
+-rw-r--r--   0        0        0     6980 2024-02-05 06:48:01.385073 bionty_base-0.37.3/tests/dev/test_handle_sources.py
+-rw-r--r--   0        0        0      532 2024-02-05 06:48:01.385163 bionty_base-0.37.3/tests/dev/test_io.py
+-rw-r--r--   0        0        0      550 2024-05-15 10:24:22.304787 bionty_base-0.37.3/tests/entities/test_bfxpipeline.py
+-rw-r--r--   0        0        0      163 2024-02-05 06:48:01.385366 bionty_base-0.37.3/tests/entities/test_biosample.py
+-rw-r--r--   0        0        0      569 2024-02-05 06:48:01.385481 bionty_base-0.37.3/tests/entities/test_cellline.py
+-rw-r--r--   0        0        0      918 2024-02-05 06:48:01.385574 bionty_base-0.37.3/tests/entities/test_cellmarker.py
+-rw-r--r--   0        0        0      609 2024-02-05 06:48:01.385685 bionty_base-0.37.3/tests/entities/test_celltype.py
+-rw-r--r--   0        0        0      632 2024-02-05 06:48:01.385772 bionty_base-0.37.3/tests/entities/test_developmentalstage.py
+-rw-r--r--   0        0        0     2967 2024-02-05 06:48:01.385867 bionty_base-0.37.3/tests/entities/test_disease.py
+-rw-r--r--   0        0        0      600 2024-02-05 06:48:01.385954 bionty_base-0.37.3/tests/entities/test_drug.py
+-rw-r--r--   0        0        0      575 2024-02-05 06:48:01.386043 bionty_base-0.37.3/tests/entities/test_ethnicity.py
+-rw-r--r--   0        0        0     1066 2024-02-05 06:48:01.386120 bionty_base-0.37.3/tests/entities/test_experimentalfactor.py
+-rw-r--r--   0        0        0     2396 2024-02-05 06:48:01.386201 bionty_base-0.37.3/tests/entities/test_gene.py
+-rw-r--r--   0        0        0      871 2024-02-05 06:48:01.386289 bionty_base-0.37.3/tests/entities/test_organism.py
+-rw-r--r--   0        0        0     1179 2024-02-05 06:48:01.386364 bionty_base-0.37.3/tests/entities/test_pathway.py
+-rw-r--r--   0        0        0     3020 2024-02-05 06:48:01.386437 bionty_base-0.37.3/tests/entities/test_phenotype.py
+-rw-r--r--   0        0        0      579 2024-02-05 06:48:01.386521 bionty_base-0.37.3/tests/entities/test_protein.py
+-rw-r--r--   0        0        0      596 2024-02-05 06:48:01.386618 bionty_base-0.37.3/tests/entities/test_tissue.py
+-rw-r--r--   0        0        0     1486 2024-02-05 06:48:01.386705 bionty_base-0.37.3/tests/test_bionty.py
+-rw-r--r--   0        0        0      627 2024-02-05 06:48:01.386784 bionty_base-0.37.3/tests/test_lamindb.py
+-rw-r--r--   0        0        0      767 2024-02-05 06:48:01.386854 bionty_base-0.37.3/tests/test_md5.py
+-rw-r--r--   0        0        0      418 2024-02-05 06:48:01.386929 bionty_base-0.37.3/tests/test_ontology.py
+-rw-r--r--   0        0        0     4305 1970-01-01 00:00:00.000000 bionty_base-0.37.3/PKG-INFO
```

### Comparing `bionty-base-0.37.2/.github/workflows/build.yml` & `bionty_base-0.37.3/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/.github/workflows/check_ontologies_reachable.yml` & `bionty_base-0.37.3/.github/workflows/check_ontologies_reachable.yml`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/.github/workflows/latest-changes.yml` & `bionty_base-0.37.3/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/.gitignore` & `bionty_base-0.37.3/.gitignore`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/.pre-commit-config.yaml` & `bionty_base-0.37.3/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/LICENSE` & `bionty_base-0.37.3/LICENSE`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/README.md` & `bionty_base-0.37.3/README.md`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/__init__.py` & `bionty_base-0.37.3/bionty_base/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,28 +35,28 @@
    PublicOntologyField
 
 PublicOntology sources:
 
 .. autosummary::
    :toctree: .
 
-    display_available_sources
-    display_currently_used_sources
-    reset_sources
-    settings
+   display_available_sources
+   display_currently_used_sources
+   reset_sources
+   settings
 
 External API:
 
 .. autosummary::
    :toctree: .
 
    Ontology
 """
 
-__version__ = "0.37.2"  # denote release candidate for 0.1.0 with 0.1rc1
+__version__ = "0.37.3"  # denote release candidate for 0.1.0 with 0.1rc1
 
 from ._sync_sources import sync_sources
 
 sync_sources()
 
 # dynamic classes
 from . import dev
```

### Comparing `bionty-base-0.37.2/bionty_base/_display_sources.py` & `bionty_base-0.37.3/bionty_base/_display_sources.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/_ontology.py` & `bionty_base-0.37.3/bionty_base/_ontology.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,10 +106,10 @@
 
         df = pd.DataFrame(
             df_values,
             columns=["ontology_id", "name", "definition", "synonyms", "parents"],
         ).set_index("ontology_id")
 
         # needed to avoid erroring in .lookup()
-        df["name"].fillna("", inplace=True)
+        df["name"] = df["name"].fillna("")
 
         return df
```

### Comparing `bionty-base-0.37.2/bionty_base/_public_ontology.py` & `bionty_base-0.37.3/bionty_base/_public_ontology.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,22 +113,14 @@
         # fmt: off
         representation = (
             f"PublicOntology\n"
             f"Entity: {self.__class__.__name__}\n"
             f"Organism: {self.organism}\n"
             f"Source: {self.source}, {self.version}\n"
             f"#terms: {self._df.shape[0] if hasattr(self, '_df') else ''}\n\n"
-            f"📖 .df(): ontology reference table\n"
-            f"🔎 .lookup(): autocompletion of terms\n"
-            f"🎯 .search(): free text search of terms\n"
-            f"✅ .validate(): strictly validate values\n"
-            f"🧐 .inspect(): full inspection of values\n"
-            f"👽 .standardize(): convert to standardized names\n"
-            f"🪜 .diff(): difference between two versions\n"
-            f"🔗 .to_pronto(): Pronto.Ontology object"
         )
         # fmt: on
         return representation
 
     @property
     def organism(self):
         """The `name` of `Organism`."""
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `bionty-base-0.37.2/bionty_base/_settings.py` & `bionty_base-0.37.3/bionty_base/_settings.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,24 +71,20 @@
 
     @versionsdir.setter
     def versionsdir(self, versionsdir: Union[str, Path]):
         self._versionsdir = Path(versionsdir).resolve()
         self._versionsdir.mkdir(exist_ok=True, parents=True)  # type: ignore
 
     @property
-    def sources_dir(self):
-        return ROOT_DIR / "sources"
-
-    @property
     def local_sources(self):
         return self.versionsdir / "sources_local.yaml"
 
     @property
     def public_sources(self):
-        return self.sources_dir / "sources.yaml"
+        return ROOT_DIR / "sources.yaml"
 
     @property
     def current_sources(self):
         return self.versionsdir / ".current_sources.yaml"
 
     @property
     def lamindb_sources(self):
```

### Comparing `bionty-base-0.37.2/bionty_base/_sync_sources.py` & `bionty_base-0.37.3/bionty_base/_sync_sources.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/dev/_handle_sources.py` & `bionty_base-0.37.3/bionty_base/dev/_handle_sources.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/dev/_io.py` & `bionty_base-0.37.3/bionty_base/dev/_io.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/dev/_md5.py` & `bionty_base-0.37.3/bionty_base/dev/_md5.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_bfxpipeline.py` & `bionty_base-0.37.3/bionty_base/entities/_bfxpipeline.py`

 * *Files 10% similar despite different names*

```diff
@@ -32,21 +32,24 @@
             ".parquet", ".json"
         )
         s3_bionty_assets("bfxpipelines.json", Path(localpath))
         with open(localpath) as f:
             data = json.load(f)
 
         df = pd.DataFrame(data).transpose()
+        df.drop("versions", inplace=True, axis=1)
+        df.rename(columns={"id": "ontology_id"}, inplace=True)
+        df.set_index("ontology_id", inplace=True, drop=True)
 
-        return df.reset_index()
+        return df
 
     def df(self) -> pd.DataFrame:
         """Pandas DataFrame of the ontology.
 
         Returns:
             A Pandas DataFrame of the ontology.
 
         Examples:
             >>> import bionty_base as bt
             >>> bt.BFXPipeline().df()
         """
-        return self._df.set_index("id")
+        return self._df.set_index("ontology_id")
```

### Comparing `bionty-base-0.37.2/bionty_base/entities/_biosample.py` & `bionty_base-0.37.3/bionty_base/entities/_biosample.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_cellline.py` & `bionty_base-0.37.3/bionty_base/entities/_cellline.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_cellmarker.py` & `bionty_base-0.37.3/bionty_base/entities/_cellmarker.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_celltype.py` & `bionty_base-0.37.3/bionty_base/entities/_celltype.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_developmentalstage.py` & `bionty_base-0.37.3/bionty_base/entities/_developmentalstage.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_disease.py` & `bionty_base-0.37.3/bionty_base/entities/_disease.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_drug.py` & `bionty_base-0.37.3/bionty_base/entities/_drug.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_ethnicity.py` & `bionty_base-0.37.3/bionty_base/entities/_ethnicity.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_experimentalfactor.py` & `bionty_base-0.37.3/bionty_base/entities/_experimentalfactor.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from functools import cached_property
 from typing import Dict, Literal, Optional
 
 import pandas as pd
 from lamin_utils import logger
 
 from bionty_base._ontology import Ontology
 from bionty_base._public_ontology import PublicOntology
```

### Comparing `bionty-base-0.37.2/bionty_base/entities/_gene.py` & `bionty_base-0.37.3/bionty_base/entities/_gene.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_organism.py` & `bionty_base-0.37.3/bionty_base/entities/_organism.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_pathway.py` & `bionty_base-0.37.3/bionty_base/entities/_pathway.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_phenotype.py` & `bionty_base-0.37.3/bionty_base/entities/_phenotype.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_protein.py` & `bionty_base-0.37.3/bionty_base/entities/_protein.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_shared_docstrings.py` & `bionty_base-0.37.3/bionty_base/entities/_shared_docstrings.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/entities/_tissue.py` & `bionty_base-0.37.3/bionty_base/entities/_tissue.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/bionty_base/sources/sources.yaml` & `bionty_base-0.37.3/bionty_base/sources.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,11 +1,17 @@
-version: "0.2.5"
+version: "0.2.6"
 Organism:
   ensembl:
     vertebrates:
+      release-112:
+        url: https://ftp.ensembl.org/pub/release-112/species_EnsemblVertebrates.txt
+        md5: 0ec37e77f4bc2d0b0b47c6c62b9f122d
+      release-111:
+        url: https://ftp.ensembl.org/pub/release-111/species_EnsemblVertebrates.txt
+        md5: 2846df83899eaa61f8043db4c036e883
       release-110:
         url: https://ftp.ensembl.org/pub/release-110/species_EnsemblVertebrates.txt
         md5: f3faf95648d3a2b50fd3625456739706
       release-109:
         url: https://ftp.ensembl.org/pub/release-109/species_EnsemblVertebrates.txt
         md5: 7595bb989f5fec07eaca5e2138f67bd4
       release-108:
@@ -35,28 +41,46 @@
         url: s3://bionty-assets/df_all__ncbitaxon__2023-06-20__Organism.parquet
         md5: 00d97ba65627f1cd65636d2df22ea76c
     name: NCBItaxon Ontology
     website: https://github.com/obophenotype/ncbitaxon
 Gene:
   ensembl:
     human:
+      release-112:
+        url: s3://bionty-assets/df_human__ensembl__release-112__Gene.parquet
+        md5: 4ccda4d88720a326737376c534e8446b
+      release-111:
+        url: s3://bionty-assets/df_human__ensembl__release-111__Gene.parquet
+        md5: f9183bc44abb34459984e137b5de8af1
       release-110:
         url: s3://bionty-assets/df_human__ensembl__release-110__Gene.parquet
         md5: 832f3947e83664588d419608a469b528
       release-109:
         url: s3://bionty-assets/human_ensembl_release-109_Gene_lookup.parquet
         md5: 72da9968c74e96d136a489a6102a4546
     mouse:
+      release-112:
+        url: s3://bionty-assets/df_mouse__ensembl__release-112__Gene.parquet
+        md5: 519cf7b8acc3c948274f66f3155a3210
+      release-111:
+        url: s3://bionty-assets/df_mouse__ensembl__release-111__Gene.parquet
+        md5: 5c071655347458307ac92b208f3c903a
       release-110:
         url: s3://bionty-assets/df_mouse__ensembl__release-110__Gene.parquet
         md5: fa4ce130f2929aefd7ac3bc8eaf0c4de
       release-109:
         url: s3://bionty-assets/mouse_ensembl_release-109_Gene_lookup.parquet
         md5: 08a1165061151b270b985317322bd2ed
     saccharomyces cerevisiae:
+      release-112:
+        url: s3://bionty-assets/df_saccharomyces cerevisiae__ensembl__release-112__Gene.parquet
+        md5: 11775126b101233525a0a9e2dd64edae
+      release-111:
+        url: s3://bionty-assets/df_saccharomyces cerevisiae__ensembl__release-111__Gene.parquet
+        md5: a15fab1d9d15a56d32fd2fd8a8fa250a
       release-110:
         url: s3://bionty-assets/df_saccharomyces cerevisiae__ensembl__release-110__Gene.parquet
         md5: 2e59495a3e87ea6575e408697dd73459
     name: Ensembl
     website: https://www.ensembl.org
 Protein:
   uniprot:
@@ -95,14 +119,17 @@
         url: https://data.bioontology.org/ontologies/CLO/submissions/65/download?apikey=8b5b7825-538d-40e0-9e9e-5ab9274a9aeb
         md5: ea58a1010b7e745702a8397a526b3a33
     name: Cell Line Ontology
     website: https://bioportal.bioontology.org/ontologies/CLO
 CellType:
   cl:
     all:
+      2024-02-13:
+        url: http://purl.obolibrary.org/obo/cl/releases/2024-02-13/cl.owl
+        mod5: d6d962b58c48f372c2c98b71e0833242
       2023-08-24:
         url: http://purl.obolibrary.org/obo/cl/releases/2023-08-24/cl.owl
         md5: 46e7dd89421f1255cf0191eca1548f73
       2023-04-20:
         url: http://purl.obolibrary.org/obo/cl/releases/2023-04-20/cl-base.owl
         md5: 58cdc1545f0d35e6fce76a65331b00fb
       2023-02-15:
@@ -112,14 +139,17 @@
         url: http://purl.obolibrary.org/obo/cl/releases/2022-08-16/cl.owl
         md5: d0655766574e63f3fe5ed56d3c030880
     name: Cell Ontology
     website: https://obophenotype.github.io/cell-ontology
 Tissue:
   uberon:
     all:
+      2024-02-20:
+        url: http://purl.obolibrary.org/obo/uberon/releases/2024-02-20/uberon.owl
+        md5: 2048667b5fdf93192384bdf53cafba18
       2023-09-05:
         url: http://purl.obolibrary.org/obo/uberon/releases/2023-09-05/uberon.owl
         md5: abcee3ede566d1311d758b853ccdf5aa
       2023-04-19:
         url: http://purl.obolibrary.org/obo/uberon/releases/2023-04-19/uberon.owl
         md5: 5611dd1375d5a95ac7d7de8e25e6016f
       2023-02-14:
@@ -129,14 +159,17 @@
         url: http://purl.obolibrary.org/obo/uberon/releases/2022-08-19/uberon.owl
         md5: c7c958a1ee48fdce146f2c1763eed27e
     name: Uberon multi-species anatomy ontology
     website: http://obophenotype.github.io/uberon
 Disease:
   mondo:
     all:
+      2024-02-06:
+        url: http://purl.obolibrary.org/obo/mondo/releases/2024-02-06/mondo.owl
+        md5: 78914fa236773c5ea6605f7570df6245
       2023-08-02:
         url: http://purl.obolibrary.org/obo/mondo/releases/2023-08-02/mondo.owl
         md5: 7f33767422042eec29f08b501fc851db
       2023-04-04:
         url: http://purl.obolibrary.org/obo/mondo/releases/2023-04-04/mondo.owl
         md5: 700c43dd9ba51aecc7a8edfc3bc2dab1
       2023-02-06:
@@ -145,14 +178,17 @@
       2022-10-11:
         url: http://purl.obolibrary.org/obo/mondo/releases/2022-10-11/mondo.owl
         md5: 04b808d05c2c2e81430b20a0e87552bb
     name: Mondo Disease Ontology
     website: https://mondo.monarchinitiative.org
   doid:
     human:
+      2024-01-31:
+        url: http://purl.obolibrary.org/obo/doid/releases/2024-01-31/doid.obo
+        md5: b36c15a4610757094f8db64b78ae2693
       2023-03-31:
         url: http://purl.obolibrary.org/obo/doid/releases/2023-03-31/doid.obo
         md5: 64f083a1e47867c307c8eae308afc3bb
       2023-01-30:
         url: http://purl.obolibrary.org/obo/doid/releases/2023-01-30/doid.obo
         md5: 9f0c92ad2896dda82195e9226a06dc36
     name: Human Disease Ontology
@@ -168,49 +204,61 @@
       icd-10-2020:
         url: s3://bionty-assets/df_human__icd__icd-10-2020__Disease.parquet
         md5: 93ec5734fcc2edd64686d5ffc6f6105f
       icd-9-2011:
         url: s3://bionty-assets/df_human__icd__icd-9-2011__Disease.parquet
         md5: cb3aefb3c4f7b2c47bf3de38453350c7
     name: International Classification of Diseases (ICD)
-    website: https://www.cdc.gov/nchs/icd/icd9cm.htm
+    website: https://www.who.int/standards/classifications/classification-of-diseases
 ExperimentalFactor:
   efo:
     all:
+      3.63.0:
+        url: http://www.ebi.ac.uk/efo/releases/v3.63.0/efo.owl
+        md5: 603e6f6981d53d501c5921aa3940b095
       3.57.0:
         url: http://www.ebi.ac.uk/efo/releases/v3.57.0/efo.owl
         md5: 2ecafc69b3aba7bdb31ad99438505c05
       3.48.0:
         url: http://www.ebi.ac.uk/efo/releases/v3.48.0/efo.owl
         md5: 3367e9a9ae3dee9113024e5108c49091
     name: The Experimental Factor Ontology
     website: https://bioportal.bioontology.org/ontologies/EFO
 Phenotype:
   hp:
     human:
+      2024-03-06:
+        url: https://github.com/obophenotype/human-phenotype-ontology/releases/download/v2024-03-06/hp.owl
+        md5: 36b0d00c24a68edb9131707bc146a4c7
       2023-06-17:
         url: https://github.com/obophenotype/human-phenotype-ontology/releases/download/v2023-06-17/hp.owl
         md5: 65e8d96bc81deb893163927063b10c06
       2023-04-05:
         url: https://github.com/obophenotype/human-phenotype-ontology/releases/download/v2023-04-05/hp.owl
         md5: bdf866e11d37cf6fd2aef25c325b2c8a
       2023-01-27:
         url: https://github.com/obophenotype/human-phenotype-ontology/releases/download/v2023-01-27/hp.owl
         md5: ceeb3ada771908deef620d74cd8e6b0f
     name: Human Phenotype Ontology
     website: https://hpo.jax.org
   mp:
     mammalian:
+      2024-02-07:
+        url: https://github.com/mgijax/mammalian-phenotype-ontology/releases/download/v2024-02-07/mp.owl
+        md5: 31c27ed2c7d5774f8b20a77e4e1fd278
       2023-05-31:
         url: https://github.com/mgijax/mammalian-phenotype-ontology/releases/download/v2023-05-31/mp.owl
         md5: be89052cf6d9c0b6197038fe347ef293
     name: Mammalian Phenotype Ontology
     website: https://github.com/mgijax/mammalian-phenotype-ontology
   zp:
     zebrafish:
+      2024-01-22:
+        url: https://github.com/obophenotype/zebrafish-phenotype-ontology/releases/download/v2024-01-22/zp.owl
+        md5: 01600a5d392419b27fc567362d4cfff8
       2022-12-17:
         url: https://github.com/obophenotype/zebrafish-phenotype-ontology/releases/download/v2022-12-17/zp.owl
         md5: 03430b567bf153216c0fa4c3440b3b24
     name: Zebrafish Phenotype Ontology
     website: https://github.com/obophenotype/zebrafish-phenotype-ontology
   phe:
     human:
@@ -232,14 +280,17 @@
       2023-05-10:
         url: https://data.bioontology.org/ontologies/GO/submissions/1814/download?apikey=8b5b7825-538d-40e0-9e9e-5ab9274a9aeb
         md5: e9845499eadaef2418f464cd7e9ac92e
     name: Gene Ontology
     website: http://geneontology.org
   pw:
     all:
+      7.82:
+        url: https://data.bioontology.org/ontologies/PW/submissions/112/download?apikey=8b5b7825-538d-40e0-9e9e-5ab9274a9aeb
+        md5: 392eb131d0513f9a186128ea4935edc9
       7.79:
         url: https://data.bioontology.org/ontologies/PW/submissions/109/download?apikey=8b5b7825-538d-40e0-9e9e-5ab9274a9aeb
         md5: 02e2337bb1ab7cc4332ef6acc4cbdfa6
     name: Pathway Ontology
     website: https://www.ebi.ac.uk/ols/ontologies/pw
 BFXPipeline:
   lamin:
@@ -248,14 +299,17 @@
         url: s3://bionty-assets/bfxpipelines.json
         md5: a7eff57a256994692fba46e0199ffc94
     name: Bioinformatics Pipeline
     website: https://lamin.ai
 Drug:
   dron:
     all:
+      2024-03-02:
+        url: https://data.bioontology.org/ontologies/DRON/submissions/22/download?apikey=8b5b7825-538d-40e0-9e9e-5ab9274a9aeb
+        md5: 84138459de4f65034e979f4e46783747
       2023-03-10:
         url: https://data.bioontology.org/ontologies/DRON/submissions/17/download?apikey=8b5b7825-538d-40e0-9e9e-5ab9274a9aeb
         md5: 75e86011158fae76bb46d96662a33ba3
     name: Drug Ontology
     website: https://bioportal.bioontology.org/ontologies/DRON
 DevelopmentalStage:
   hsapdv:
```

### Comparing `bionty-base-0.37.2/docs/changelog.md` & `bionty_base-0.37.3/docs/changelog.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,30 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+✨ New ontology: Gene-ensembl-111/112 | [578](https://github.com/laminlabs/bionty-base/pull/578) | [Zethson](https://github.com/Zethson) | 2024-05-16 |
+ ✨ New ontology: ExperimentalFactor-efo-3.63 | [577](https://github.com/laminlabs/bionty-base/pull/577) | [Zethson](https://github.com/Zethson) | 2024-05-15 |
+✨ New ontology: CellType-cl-2024-02-13 | [576](https://github.com/laminlabs/bionty-base/pull/576) | [Zethson](https://github.com/Zethson) | 2024-05-15 |
+:sparkles: New Ontology: Tissue-uberon-2024-02-20 | [575](https://github.com/laminlabs/bionty-base/pull/575) | [Zethson](https://github.com/Zethson) | 2024-05-15 |
+✨ New ontology: Organism-ensembl-release-111 and Organism-ensembl-release-112 | [574](https://github.com/laminlabs/bionty-base/pull/574) | [sunnyosun](https://github.com/sunnyosun) | 2024-05-15 |
+:sparkles: New Ontology: Disease-mondo-2024-02-06 | [572](https://github.com/laminlabs/bionty-base/pull/572) | [Zethson](https://github.com/Zethson) | 2024-05-15 |
+:sparkles: New Ontology: Disease-DOID-2024-01-31 | [571](https://github.com/laminlabs/bionty-base/pull/571) | [Zethson](https://github.com/Zethson) | 2024-05-15 |
+:sparkles: New Ontology: Phenotype-hp-2024-03-06 | [570](https://github.com/laminlabs/bionty-base/pull/570) | [Zethson](https://github.com/Zethson) | 2024-05-15 |
+:sparkles: New Ontology: Phenotype-mp-2024-02-07 | [569](https://github.com/laminlabs/bionty-base/pull/569) | [Zethson](https://github.com/Zethson) | 2024-05-15 |
+:sparkles: New ontology: Phenotype-zp-2024-01-22 | [568](https://github.com/laminlabs/bionty-base/pull/568) | [Zethson](https://github.com/Zethson) | 2024-05-15 |
+:sparkles: New ontology: Pathway-pw-7.82 | [567](https://github.com/laminlabs/bionty-base/pull/567) | [Zethson](https://github.com/Zethson) | 2024-05-15 |
+:sparkles: Add latest Drug source | [566](https://github.com/laminlabs/bionty-base/pull/566) | [Zethson](https://github.com/Zethson) | 2024-05-15 |
+🚚 Move out sources.yml | [565](https://github.com/laminlabs/bionty-base/pull/565) | [sunnyosun](https://github.com/sunnyosun) | 2024-05-15 |
+Update BFXPipeline | [564](https://github.com/laminlabs/bionty-base/pull/564) | [Zethson](https://github.com/Zethson) | 2024-05-02 |
+password is deprecated | [562](https://github.com/laminlabs/bionty-base/pull/562) | [falexwolf](https://github.com/falexwolf) | 2024-04-25 |
+Use more general ICD website as source | [561](https://github.com/laminlabs/bionty-base/pull/561) | [Zethson](https://github.com/Zethson) | 2024-04-11 |
+Pandas 3.0.0 fix | [560](https://github.com/laminlabs/bionty-base/pull/560) | [Zethson](https://github.com/Zethson) | 2024-04-11 |
+Remove functions from __repr__ | [559](https://github.com/laminlabs/bionty-base/pull/559) | [Zethson](https://github.com/Zethson) | 2024-04-11 |
 Add new ICD 10-CM | [554](https://github.com/laminlabs/bionty-base/pull/554) | [Zethson](https://github.com/Zethson) | 2024-04-04 |
 🔇 Remove py version warning | [553](https://github.com/laminlabs/bionty-base/pull/553) | [sunnyosun](https://github.com/sunnyosun) | 2024-03-27 | 0.37.1
 Switch to uv for CI | [552](https://github.com/laminlabs/bionty-base/pull/552) | [Zethson](https://github.com/Zethson) | 2024-03-24 |
 🐛 Catch ClientError | [549](https://github.com/laminlabs/bionty-base/pull/549) | [Koncopd](https://github.com/Koncopd) | 2024-03-14 |
 Fix reset message | [545](https://github.com/laminlabs/bionty-base/pull/545) | [Zethson](https://github.com/Zethson) | 2024-03-13 |
 📝 Added validate example to docstring | [542](https://github.com/laminlabs/bionty-base/pull/542) | [sunnyosun](https://github.com/sunnyosun) | 2024-03-01 |
 🚚 Rename repo to `bionty-base` | [539](https://github.com/laminlabs/bionty-base/pull/539) | [sunnyosun](https://github.com/sunnyosun) | 2024-01-29 | 0.37.0
```

### Comparing `bionty-base-0.37.2/docs/developer/updating_source.md` & `bionty_base-0.37.3/docs/developer/updating_source.md`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/docs/guide/comparison.md` & `bionty_base-0.37.3/docs/guide/comparison.md`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/docs/guide/concepts.md` & `bionty_base-0.37.3/docs/guide/concepts.md`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/docs/guide/config.md` & `bionty_base-0.37.3/docs/guide/config.md`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/docs/guide/extend.md` & `bionty_base-0.37.3/docs/guide/extend.md`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/docs/guide/ontology.ipynb` & `bionty_base-0.37.3/docs/guide/ontology.ipynb`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/docs/guide/sources.ipynb` & `bionty_base-0.37.3/docs/guide/sources.ipynb`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/docs/guide/validate.ipynb` & `bionty_base-0.37.3/docs/guide/validate.ipynb`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/noxfile.py` & `bionty_base-0.37.3/noxfile.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/pyproject.toml` & `bionty_base-0.37.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/scripts/check_ontologies_reachable.py` & `bionty_base-0.37.3/scripts/check_ontologies_reachable.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import urllib.request
 from http.client import BadStatusLine
 from pathlib import Path
 from urllib.error import HTTPError, URLError
 
 import yaml  # type:ignore
 
-VERSIONS_FILE_PATH = Path.cwd() / "bionty_base" / "sources" / "sources.yaml"
+VERSIONS_FILE_PATH = Path.cwd() / "bionty_base" / "sources.yaml"
 
 
 def extract_urls_from_yaml(yaml_file):
     with open(yaml_file) as file:
         yaml_data = yaml.safe_load(file)
         urls = []
```

### Comparing `bionty-base-0.37.2/scripts/determine_md5s.py` & `bionty_base-0.37.3/scripts/determine_md5s.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/scripts/generate_bfxpipelines.py` & `bionty_base-0.37.3/scripts/generate_bfxpipelines.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/scripts/update_new_ontologies.py` & `bionty_base-0.37.3/scripts/update_new_ontologies.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/scripts/upload_new_ontologies.py` & `bionty_base-0.37.3/scripts/upload_new_ontologies.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-def _upload_ontology_artifacts(instance: str, lamindb_user: str, lamindb_password: str):
+def _upload_ontology_artifacts(instance: str, lamin_user: str, lamin_api_key: str):
     import bionty_base as bt
     import lamindb as ln
     from bionty_base._public_ontology import encode_filenames
     from bionty_base._settings import settings
 
-    ln.setup.login(lamindb_user, password=lamindb_password)
+    ln.setup.login(lamin_user, key=lamin_api_key)
     ln.setup.load(instance)
 
     queryset = ln.File.select().all()
 
     files = []
     for entity, row in bt.display_available_sources().iterrows():
         parquet_filename, ontology_filename = encode_filenames(
```

### Comparing `bionty-base-0.37.2/tests/dev/test_handle_sources.py` & `bionty_base-0.37.3/tests/dev/test_handle_sources.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/dev/test_io.py` & `bionty_base-0.37.3/tests/dev/test_io.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/entities/test_bfxpipeline.py` & `bionty_base-0.37.3/tests/entities/test_bfxpipeline.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import bionty_base as bt
 import pandas as pd
 
 
 def test_lamin_bfxpipeline_inspect_name():
     df = pd.DataFrame(
         index=[
-            "nf-core methylseq v2.3.0",
-            "Cell Ranger v7.1.0",
+            "nf-core methylseq v2.6.0",
+            "Cell Ranger v8.0.0",
             "This bfx pipeline does not exist",
         ]
     )
 
     bfxp = bt.BFXPipeline(source="lamin")
     inspected_df = bfxp.inspect(df.index, field=bfxp.name, return_df=True)
```

### Comparing `bionty-base-0.37.2/tests/entities/test_cellline.py` & `bionty_base-0.37.3/tests/entities/test_cellline.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/entities/test_cellmarker.py` & `bionty_base-0.37.3/tests/entities/test_cellmarker.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/entities/test_celltype.py` & `bionty_base-0.37.3/tests/entities/test_celltype.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/entities/test_developmentalstage.py` & `bionty_base-0.37.3/tests/entities/test_developmentalstage.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/entities/test_disease.py` & `bionty_base-0.37.3/tests/entities/test_disease.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/entities/test_drug.py` & `bionty_base-0.37.3/tests/entities/test_drug.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/entities/test_ethnicity.py` & `bionty_base-0.37.3/tests/entities/test_ethnicity.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/entities/test_experimentalfactor.py` & `bionty_base-0.37.3/tests/entities/test_experimentalfactor.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/entities/test_gene.py` & `bionty_base-0.37.3/tests/entities/test_gene.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/entities/test_organism.py` & `bionty_base-0.37.3/tests/entities/test_organism.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/entities/test_pathway.py` & `bionty_base-0.37.3/tests/entities/test_pathway.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/entities/test_phenotype.py` & `bionty_base-0.37.3/tests/entities/test_phenotype.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/entities/test_protein.py` & `bionty_base-0.37.3/tests/entities/test_protein.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/entities/test_tissue.py` & `bionty_base-0.37.3/tests/entities/test_tissue.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/test_bionty.py` & `bionty_base-0.37.3/tests/test_bionty.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/test_lamindb.py` & `bionty_base-0.37.3/tests/test_lamindb.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/tests/test_md5.py` & `bionty_base-0.37.3/tests/test_md5.py`

 * *Files identical despite different names*

### Comparing `bionty-base-0.37.2/PKG-INFO` & `bionty_base-0.37.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bionty-base
-Version: 0.37.2
+Version: 0.37.3
 Summary: Bionty.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

