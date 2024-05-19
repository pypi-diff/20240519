# Comparing `tmp/radprompter-1.0.tar.gz` & `tmp/radprompter-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "radprompter-1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "radprompter-1.0.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `radprompter-1.0.tar` & `radprompter-1.0.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.0/.DS_Store
--rw-r--r--   0        0        0     3133 2024-05-14 20:12:30.669307 radprompter-1.0/.gitignore
--rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.0/LICENSE
--rw-r--r--   0        0        0      133 2024-05-15 19:08:43.183784 radprompter-1.0/Plan.md
--rw-r--r--   0        0        0       13 2024-05-14 18:23:37.432717 radprompter-1.0/README.md
--rw-r--r--   0        0        0    12401 2024-05-14 18:23:37.432957 radprompter-1.0/demo.ipynb
--rw-r--r--   0        0        0    23670 2024-05-15 19:39:22.162953 radprompter-1.0/demo_no_CoT.ipynb
--rw-r--r--   0        0        0     4382 2024-05-14 19:04:54.672733 radprompter-1.0/demo_prompt_no_CoT.toml
--rw-r--r--   0        0        0      501 2024-05-19 14:17:34.694359 radprompter-1.0/pyproject.toml
--rw-r--r--   0        0        0      209 2024-05-19 14:13:32.246085 radprompter-1.0/radprompter/__init__.py
--rw-r--r--   0        0        0       59 2024-05-14 18:54:49.737505 radprompter-1.0/radprompter/clients/__init__.py
--rw-r--r--   0        0        0     3530 2024-05-14 18:54:06.476384 radprompter-1.0/radprompter/clients/clients.py
--rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.0/radprompter/prompts/__init__.py
--rw-r--r--   0        0        0     9910 2024-05-15 19:08:28.731272 radprompter-1.0/radprompter/prompts/prompts.py
--rw-r--r--   0        0        0     5654 2024-05-19 01:17:51.277168 radprompter-1.0/radprompter/radprompter.py
--rw-r--r--   0        0        0     3212 2024-05-19 14:13:26.546120 radprompter-1.0/radprompter/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
--rw-r--r--   0        0        0    16157 2024-05-19 01:12:35.057063 radprompter-1.0/radprompter/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb
--rw-r--r--   0        0        0     4488 2024-05-19 01:05:24.865041 radprompter-1.0/radprompter/tutorials/4_Using-Schemas/4_Using-Schemas.toml
--rw-r--r--   0        0        0    19240 2024-05-19 01:12:53.117189 radprompter-1.0/radprompter/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb
--rw-r--r--   0        0        0     4051 2024-05-19 01:05:24.865144 radprompter-1.0/radprompter/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml
--rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.0/radprompter/tutorials/README.md
--rw-r--r--   0        0        0     4256 2024-05-15 19:04:25.647961 radprompter-1.0/sample_prompt copy.toml
--rw-r--r--   0        0        0     4350 2024-05-15 19:04:16.915270 radprompter-1.0/sample_prompt.toml
--rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.0/sample_reports/sample_report_1.txt
--rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.0/sample_reports/sample_report_2.txt
--rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.0/sample_reports/sample_report_3.txt
--rw-r--r--   0        0        0      420 1970-01-01 00:00:00.000000 radprompter-1.0/PKG-INFO
+-rw-r--r--   0        0        0     6148 2024-05-15 00:50:49.718415 radprompter-1.0.1/.DS_Store
+-rw-r--r--   0        0        0     3133 2024-05-14 20:12:30.669307 radprompter-1.0.1/.gitignore
+-rw-r--r--   0        0        0    11357 2024-05-14 18:23:37.432618 radprompter-1.0.1/LICENSE
+-rw-r--r--   0        0        0      133 2024-05-15 19:08:43.183784 radprompter-1.0.1/Plan.md
+-rw-r--r--   0        0        0       13 2024-05-14 18:23:37.432717 radprompter-1.0.1/README.md
+-rw-r--r--   0        0        0    12401 2024-05-14 18:23:37.432957 radprompter-1.0.1/demo.ipynb
+-rw-r--r--   0        0        0    23670 2024-05-15 19:39:22.162953 radprompter-1.0.1/demo_no_CoT.ipynb
+-rw-r--r--   0        0        0     4382 2024-05-14 19:04:54.672733 radprompter-1.0.1/demo_prompt_no_CoT.toml
+-rw-r--r--   0        0        0      643 2024-05-19 14:19:18.563305 radprompter-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      211 2024-05-19 14:19:58.379367 radprompter-1.0.1/radprompter/__init__.py
+-rw-r--r--   0        0        0       59 2024-05-14 18:54:49.737505 radprompter-1.0.1/radprompter/clients/__init__.py
+-rw-r--r--   0        0        0     3530 2024-05-14 18:54:06.476384 radprompter-1.0.1/radprompter/clients/clients.py
+-rw-r--r--   0        0        0       27 2024-05-14 22:18:09.544596 radprompter-1.0.1/radprompter/prompts/__init__.py
+-rw-r--r--   0        0        0     9910 2024-05-15 19:08:28.731272 radprompter-1.0.1/radprompter/prompts/prompts.py
+-rw-r--r--   0        0        0     5654 2024-05-19 01:17:51.277168 radprompter-1.0.1/radprompter/radprompter.py
+-rw-r--r--   0        0        0     3212 2024-05-19 14:13:26.546120 radprompter-1.0.1/radprompter/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb
+-rw-r--r--   0        0        0    16157 2024-05-19 01:12:35.057063 radprompter-1.0.1/radprompter/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb
+-rw-r--r--   0        0        0     4488 2024-05-19 01:05:24.865041 radprompter-1.0.1/radprompter/tutorials/4_Using-Schemas/4_Using-Schemas.toml
+-rw-r--r--   0        0        0    19240 2024-05-19 01:12:53.117189 radprompter-1.0.1/radprompter/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb
+-rw-r--r--   0        0        0     4051 2024-05-19 01:05:24.865144 radprompter-1.0.1/radprompter/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml
+-rw-r--r--   0        0        0        0 2024-05-15 18:54:34.909069 radprompter-1.0.1/radprompter/tutorials/README.md
+-rw-r--r--   0        0        0     4256 2024-05-15 19:04:25.647961 radprompter-1.0.1/sample_prompt copy.toml
+-rw-r--r--   0        0        0     4350 2024-05-15 19:04:16.915270 radprompter-1.0.1/sample_prompt.toml
+-rw-r--r--   0        0        0     1089 2024-05-14 18:23:37.434577 radprompter-1.0.1/sample_reports/sample_report_1.txt
+-rw-r--r--   0        0        0     1388 2024-05-14 18:23:37.434671 radprompter-1.0.1/sample_reports/sample_report_2.txt
+-rw-r--r--   0        0        0     1374 2024-05-14 18:23:37.434764 radprompter-1.0.1/sample_reports/sample_report_3.txt
+-rw-r--r--   0        0        0      526 1970-01-01 00:00:00.000000 radprompter-1.0.1/PKG-INFO
```

### Comparing `radprompter-1.0/.DS_Store` & `radprompter-1.0.1/.DS_Store`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/.gitignore` & `radprompter-1.0.1/.gitignore`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/LICENSE` & `radprompter-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/demo.ipynb` & `radprompter-1.0.1/demo.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/demo_no_CoT.ipynb` & `radprompter-1.0.1/demo_no_CoT.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/demo_prompt_no_CoT.toml` & `radprompter-1.0.1/demo_prompt_no_CoT.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/radprompter/clients/clients.py` & `radprompter-1.0.1/radprompter/clients/clients.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/radprompter/prompts/prompts.py` & `radprompter-1.0.1/radprompter/prompts/prompts.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/radprompter/radprompter.py` & `radprompter-1.0.1/radprompter/radprompter.py`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/radprompter/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb` & `radprompter-1.0.1/radprompter/tutorials/01_Basic-Usecase/01_Basic-Usecase.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/radprompter/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb` & `radprompter-1.0.1/radprompter/tutorials/4_Using-Schemas/4_Using-Schemas.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/radprompter/tutorials/4_Using-Schemas/4_Using-Schemas.toml` & `radprompter-1.0.1/radprompter/tutorials/4_Using-Schemas/4_Using-Schemas.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/radprompter/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb` & `radprompter-1.0.1/radprompter/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.ipynb`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/radprompter/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml` & `radprompter-1.0.1/radprompter/tutorials/5_Assistant-Prefill/5_Assistant-Prefill.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/sample_prompt copy.toml` & `radprompter-1.0.1/sample_prompt copy.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/sample_prompt.toml` & `radprompter-1.0.1/sample_prompt.toml`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/sample_reports/sample_report_1.txt` & `radprompter-1.0.1/sample_reports/sample_report_1.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/sample_reports/sample_report_2.txt` & `radprompter-1.0.1/sample_reports/sample_report_2.txt`

 * *Files identical despite different names*

### Comparing `radprompter-1.0/sample_reports/sample_report_3.txt` & `radprompter-1.0.1/sample_reports/sample_report_3.txt`

 * *Files identical despite different names*

