# Comparing `tmp/arctix-0.0.5.tar.gz` & `tmp/arctix-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arctix-0.0.5.tar", max compression
+gzip compressed data, was "arctix-0.0.6.tar", max compression
```

## Comparing `arctix-0.0.5.tar` & `arctix-0.0.6.tar`

### file list

```diff
@@ -1,36 +1,37 @@
--rw-r--r--   0        0        0     1501 2024-05-14 02:18:13.503896 arctix-0.0.5/LICENSE
--rw-r--r--   0        0        0     6674 2024-05-14 02:18:13.503896 arctix-0.0.5/README.md
--rw-r--r--   0        0        0     6664 2024-05-14 02:18:13.507896 arctix-0.0.5/pyproject.toml
--rw-r--r--   0        0        0       21 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/__init__.py
--rw-r--r--   0        0        0       43 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/dataset/__init__.py
--rw-r--r--   0        0        0    29056 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/dataset/breakfast.py
--rw-r--r--   0        0        0    26642 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/dataset/ego4d.py
--rw-r--r--   0        0        0    23865 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/dataset/epic_kitchen_100.py
--rw-r--r--   0        0        0    29698 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/dataset/multithumos.py
--rw-r--r--   0        0        0      247 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/testing/__init__.py
--rw-r--r--   0        0        0      538 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/testing/fixtures.py
--rw-r--r--   0        0        0       29 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/__init__.py
--rw-r--r--   0        0        0     3095 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/__init__.py
--rw-r--r--   0        0        0     6978 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/base.py
--rw-r--r--   0        0        0     6262 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/casting.py
--rw-r--r--   0        0        0     2107 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/function.py
--rw-r--r--   0        0        0     4084 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/json.py
--rw-r--r--   0        0        0     2914 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/replace.py
--rw-r--r--   0        0        0     3809 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/sequential.py
--rw-r--r--   0        0        0     4352 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/sorting.py
--rw-r--r--   0        0        0     3107 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/string.py
--rw-r--r--   0        0        0     3200 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/time.py
--rw-r--r--   0        0        0     4581 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/transformer/dataframe/vocab.py
--rw-r--r--   0        0        0       34 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/__init__.py
--rw-r--r--   0        0        0      276 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/dataframe/__init__.py
--rw-r--r--   0        0        0     1618 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/dataframe/removing.py
--rw-r--r--   0        0        0     1618 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/dataframe/vocab.py
--rw-r--r--   0        0        0     3196 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/download.py
--rw-r--r--   0        0        0     7145 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/imports.py
--rw-r--r--   0        0        0      190 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/iter/__init__.py
--rw-r--r--   0        0        0     3543 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/iter/path.py
--rw-r--r--   0        0        0     1325 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/mapping.py
--rw-r--r--   0        0        0     3234 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/masking.py
--rw-r--r--   0        0        0      596 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/noop.py
--rw-r--r--   0        0        0    14150 2024-05-14 02:18:13.507896 arctix-0.0.5/src/arctix/utils/vocab.py
--rw-r--r--   0        0        0     8034 1970-01-01 00:00:00.000000 arctix-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1501 2024-05-19 20:22:18.391373 arctix-0.0.6/LICENSE
+-rw-r--r--   0        0        0     6674 2024-05-19 20:22:18.391373 arctix-0.0.6/README.md
+-rw-r--r--   0        0        0     6664 2024-05-19 20:22:18.395373 arctix-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0       21 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/__init__.py
+-rw-r--r--   0        0        0       43 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/dataset/__init__.py
+-rw-r--r--   0        0        0    30673 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/dataset/breakfast.py
+-rw-r--r--   0        0        0    28758 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/dataset/ego4d.py
+-rw-r--r--   0        0        0    24748 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/dataset/epic_kitchen_100.py
+-rw-r--r--   0        0        0    31167 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/dataset/multithumos.py
+-rw-r--r--   0        0        0      247 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/testing/__init__.py
+-rw-r--r--   0        0        0      538 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/testing/fixtures.py
+-rw-r--r--   0        0        0       29 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/transformer/__init__.py
+-rw-r--r--   0        0        0     3503 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/transformer/dataframe/__init__.py
+-rw-r--r--   0        0        0     6978 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/transformer/dataframe/base.py
+-rw-r--r--   0        0        0     6262 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/transformer/dataframe/casting.py
+-rw-r--r--   0        0        0     5251 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/transformer/dataframe/diff.py
+-rw-r--r--   0        0        0     2107 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/transformer/dataframe/function.py
+-rw-r--r--   0        0        0     4084 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/transformer/dataframe/json.py
+-rw-r--r--   0        0        0     2914 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/transformer/dataframe/replace.py
+-rw-r--r--   0        0        0     3809 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/transformer/dataframe/sequential.py
+-rw-r--r--   0        0        0     4352 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/transformer/dataframe/sorting.py
+-rw-r--r--   0        0        0     3107 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/transformer/dataframe/string.py
+-rw-r--r--   0        0        0     3200 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/transformer/dataframe/time.py
+-rw-r--r--   0        0        0     4581 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/transformer/dataframe/vocab.py
+-rw-r--r--   0        0        0       34 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/utils/__init__.py
+-rw-r--r--   0        0        0      276 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/utils/dataframe/__init__.py
+-rw-r--r--   0        0        0     1618 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/utils/dataframe/removing.py
+-rw-r--r--   0        0        0     1618 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/utils/dataframe/vocab.py
+-rw-r--r--   0        0        0     3196 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/utils/download.py
+-rw-r--r--   0        0        0     7145 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/utils/imports.py
+-rw-r--r--   0        0        0      190 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/utils/iter/__init__.py
+-rw-r--r--   0        0        0     3543 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/utils/iter/path.py
+-rw-r--r--   0        0        0     1325 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/utils/mapping.py
+-rw-r--r--   0        0        0     3234 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/utils/masking.py
+-rw-r--r--   0        0        0      596 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/utils/noop.py
+-rw-r--r--   0        0        0    14150 2024-05-19 20:22:18.395373 arctix-0.0.6/src/arctix/utils/vocab.py
+-rw-r--r--   0        0        0     8034 1970-01-01 00:00:00.000000 arctix-0.0.6/PKG-INFO
```

### Comparing `arctix-0.0.5/LICENSE` & `arctix-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/README.md` & `arctix-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/pyproject.toml` & `arctix-0.0.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "arctix"
-version = "0.0.5"
+version = "0.0.6"
 description = ""
 readme = "README.md"
 authors = ["Thibaut Durand <durand.tibo+gh@gmail.com>"]
 homepage = "https://github.com/durandtibo/arctix"
 repository = "https://github.com/durandtibo/arctix"
 keywords = ["asynchronous time-series", "dataset", "preprocessing"]
 license = "BSD-3-Clause"
```

### Comparing `arctix-0.0.5/src/arctix/dataset/breakfast.py` & `arctix-0.0.6/src/arctix/dataset/breakfast.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,14 +109,15 @@
     ACTION_ID: str = "action_id"
     COOKING_ACTIVITY: str = "cooking_activity"
     COOKING_ACTIVITY_ID: str = "cooking_activity_id"
     END_TIME: str = "end_time"
     PERSON: str = "person"
     PERSON_ID: str = "person_id"
     START_TIME: str = "start_time"
+    START_TIME_DIFF: str = "start_time_diff"
     SEQUENCE_LENGTH: str = "sequence_length"
 
 
 class MetadataKeys:
     r"""Indicate the metadata keys."""
 
     VOCAB_ACTION: str = "vocab_action"
@@ -378,35 +379,36 @@
     ...         ],
     ...         Column.START_TIME: [1.0, 31.0, 151.0, 429.0, 576.0, 706.0, 1.0, 48.0, 216.0, 566.0],
     ...     },
     ... )
     >>> data, metadata = prepare_data(frame)
     >>> with pl.Config(tbl_cols=-1):
     ...     data
-    shape: (10, 8)
-    ┌─────────────┬───────────┬─────────────┬─────────────┬──────────┬────────┬───────────┬────────────┐
-    │ action      ┆ action_id ┆ cooking_act ┆ cooking_act ┆ end_time ┆ person ┆ person_id ┆ start_time │
-    │ ---         ┆ ---       ┆ ivity       ┆ ivity_id    ┆ ---      ┆ ---    ┆ ---       ┆ ---        │
-    │ str         ┆ i64       ┆ ---         ┆ ---         ┆ f64      ┆ str    ┆ i64       ┆ f64        │
-    │             ┆           ┆ str         ┆ i64         ┆          ┆        ┆           ┆            │
-    ╞═════════════╪═══════════╪═════════════╪═════════════╪══════════╪════════╪═══════════╪════════════╡
-    │ SIL         ┆ 0         ┆ cereals     ┆ 0           ┆ 30.0     ┆ P03    ┆ 0         ┆ 1.0        │
-    │ take_bowl   ┆ 2         ┆ cereals     ┆ 0           ┆ 150.0    ┆ P03    ┆ 0         ┆ 31.0       │
-    │ pour_cereal ┆ 5         ┆ cereals     ┆ 0           ┆ 428.0    ┆ P03    ┆ 0         ┆ 151.0      │
-    │ s           ┆           ┆             ┆             ┆          ┆        ┆           ┆            │
-    │ pour_milk   ┆ 1         ┆ cereals     ┆ 0           ┆ 575.0    ┆ P03    ┆ 0         ┆ 429.0      │
-    │ stir_cereal ┆ 3         ┆ cereals     ┆ 0           ┆ 705.0    ┆ P03    ┆ 0         ┆ 576.0      │
-    │ s           ┆           ┆             ┆             ┆          ┆        ┆           ┆            │
-    │ SIL         ┆ 0         ┆ cereals     ┆ 0           ┆ 836.0    ┆ P03    ┆ 0         ┆ 706.0      │
-    │ SIL         ┆ 0         ┆ milk        ┆ 1           ┆ 47.0     ┆ P54    ┆ 1         ┆ 1.0        │
-    │ pour_milk   ┆ 1         ┆ milk        ┆ 1           ┆ 215.0    ┆ P54    ┆ 1         ┆ 48.0       │
-    │ spoon_powde ┆ 4         ┆ milk        ┆ 1           ┆ 565.0    ┆ P54    ┆ 1         ┆ 216.0      │
-    │ r           ┆           ┆             ┆             ┆          ┆        ┆           ┆            │
-    │ SIL         ┆ 0         ┆ milk        ┆ 1           ┆ 747.0    ┆ P54    ┆ 1         ┆ 566.0      │
-    └─────────────┴───────────┴─────────────┴─────────────┴──────────┴────────┴───────────┴────────────┘
+    shape: (10, 9)
+    ┌───────────┬───────────┬──────────┬──────────┬──────────┬────────┬──────────┬──────────┬──────────┐
+    │ action    ┆ action_id ┆ cooking_ ┆ cooking_ ┆ end_time ┆ person ┆ person_i ┆ start_ti ┆ start_ti │
+    │ ---       ┆ ---       ┆ activity ┆ activity ┆ ---      ┆ ---    ┆ d        ┆ me       ┆ me_diff  │
+    │ str       ┆ i64       ┆ ---      ┆ _id      ┆ f64      ┆ str    ┆ ---      ┆ ---      ┆ ---      │
+    │           ┆           ┆ str      ┆ ---      ┆          ┆        ┆ i64      ┆ f64      ┆ f64      │
+    │           ┆           ┆          ┆ i64      ┆          ┆        ┆          ┆          ┆          │
+    ╞═══════════╪═══════════╪══════════╪══════════╪══════════╪════════╪══════════╪══════════╪══════════╡
+    │ SIL       ┆ 0         ┆ cereals  ┆ 0        ┆ 30.0     ┆ P03    ┆ 0        ┆ 1.0      ┆ 0.0      │
+    │ take_bowl ┆ 2         ┆ cereals  ┆ 0        ┆ 150.0    ┆ P03    ┆ 0        ┆ 31.0     ┆ 30.0     │
+    │ pour_cere ┆ 5         ┆ cereals  ┆ 0        ┆ 428.0    ┆ P03    ┆ 0        ┆ 151.0    ┆ 120.0    │
+    │ als       ┆           ┆          ┆          ┆          ┆        ┆          ┆          ┆          │
+    │ pour_milk ┆ 1         ┆ cereals  ┆ 0        ┆ 575.0    ┆ P03    ┆ 0        ┆ 429.0    ┆ 278.0    │
+    │ stir_cere ┆ 3         ┆ cereals  ┆ 0        ┆ 705.0    ┆ P03    ┆ 0        ┆ 576.0    ┆ 147.0    │
+    │ als       ┆           ┆          ┆          ┆          ┆        ┆          ┆          ┆          │
+    │ SIL       ┆ 0         ┆ cereals  ┆ 0        ┆ 836.0    ┆ P03    ┆ 0        ┆ 706.0    ┆ 130.0    │
+    │ SIL       ┆ 0         ┆ milk     ┆ 1        ┆ 47.0     ┆ P54    ┆ 1        ┆ 1.0      ┆ 0.0      │
+    │ pour_milk ┆ 1         ┆ milk     ┆ 1        ┆ 215.0    ┆ P54    ┆ 1        ┆ 48.0     ┆ 47.0     │
+    │ spoon_pow ┆ 4         ┆ milk     ┆ 1        ┆ 565.0    ┆ P54    ┆ 1        ┆ 216.0    ┆ 168.0    │
+    │ der       ┆           ┆          ┆          ┆          ┆        ┆          ┆          ┆          │
+    │ SIL       ┆ 0         ┆ milk     ┆ 1        ┆ 747.0    ┆ P54    ┆ 1        ┆ 566.0    ┆ 350.0    │
+    └───────────┴───────────┴──────────┴──────────┴──────────┴────────┴──────────┴──────────┴──────────┘
     >>> metadata
     {'vocab_action': Vocabulary(
       counter=Counter({'SIL': 4, 'pour_milk': 2, 'take_bowl': 1, 'stir_cereals': 1, 'spoon_powder': 1, 'pour_cereals': 1}),
       index_to_token=('SIL', 'pour_milk', 'take_bowl', 'stir_cereals', 'spoon_powder', 'pour_cereals'),
       token_to_index={'SIL': 0, 'pour_milk': 1, 'take_bowl': 2, 'stir_cereals': 3, 'spoon_powder': 4, 'pour_cereals': 5},
     ), 'vocab_activity': Vocabulary(
       counter=Counter({'cereals': 6, 'milk': 4}),
@@ -423,14 +425,19 @@
     vocab_action = generate_vocabulary(frame, col=Column.ACTION).sort_by_count()
     vocab_person = generate_vocabulary(frame, col=Column.PERSON).sort_by_count()
     vocab_activity = (
         generate_vocabulary(frame, col=Column.COOKING_ACTIVITY).sort_by_token().sort_by_count()
     )
     transformer = td.Sequential(
         [
+            td.TimeDiff(
+                group_cols=[Column.COOKING_ACTIVITY, Column.PERSON],
+                time_col=Column.START_TIME,
+                time_diff_col=Column.START_TIME_DIFF,
+            ),
             td.Sort(columns=[Column.COOKING_ACTIVITY, Column.PERSON, Column.START_TIME]),
             td.Cast(columns=[Column.START_TIME, Column.END_TIME], dtype=pl.Float64),
             td.StripChars(columns=[Column.ACTION, Column.PERSON, Column.COOKING_ACTIVITY]),
             td.Function(partial(filter_by_split, split=split)),
             td.TokenToIndex(
                 vocab=vocab_action, token_column=Column.ACTION, index_column=Column.ACTION_ID
             ),
@@ -496,45 +503,48 @@
     ...             "milk",
     ...         ],
     ...         Column.COOKING_ACTIVITY_ID: [0, 0, 0, 0, 0, 0, 1, 1, 1, 1],
     ...         Column.END_TIME: [30.0, 150.0, 428.0, 575.0, 705.0, 836.0, 47.0, 215.0, 565.0, 747.0],
     ...         Column.PERSON: ["P03", "P03", "P03", "P03", "P03", "P03", "P54", "P54", "P54", "P54"],
     ...         Column.PERSON_ID: [0, 0, 0, 0, 0, 0, 1, 1, 1, 1],
     ...         Column.START_TIME: [1.0, 31.0, 151.0, 429.0, 576.0, 706.0, 1.0, 48.0, 216.0, 566.0],
+    ...         Column.START_TIME_DIFF: [0.0, 30.0, 120.0, 278.0, 147.0, 130.0, 0.0, 47.0, 168.0, 350.0],
     ...     }
     ... )
     >>> groups = group_by_sequence(frame)
     >>> with pl.Config(tbl_cols=-1):
     ...     groups
-    shape: (2, 9)
-    ┌───────────┬───────────┬──────────┬──────────┬──────────┬────────┬──────────┬──────────┬──────────┐
-    │ action    ┆ action_id ┆ cooking_ ┆ cooking_ ┆ end_time ┆ person ┆ person_i ┆ sequence ┆ start_ti │
-    │ ---       ┆ ---       ┆ activity ┆ activity ┆ ---      ┆ ---    ┆ d        ┆ _length  ┆ me       │
-    │ list[str] ┆ list[i64] ┆ ---      ┆ _id      ┆ list[f64 ┆ str    ┆ ---      ┆ ---      ┆ ---      │
-    │           ┆           ┆ str      ┆ ---      ┆ ]        ┆        ┆ i64      ┆ i64      ┆ list[f64 │
-    │           ┆           ┆          ┆ i64      ┆          ┆        ┆          ┆          ┆ ]        │
-    ╞═══════════╪═══════════╪══════════╪══════════╪══════════╪════════╪══════════╪══════════╪══════════╡
-    │ ["SIL",   ┆ [0, 2, …  ┆ cereals  ┆ 0        ┆ [30.0,   ┆ P03    ┆ 0        ┆ 6        ┆ [1.0,    │
-    │ "take_bow ┆ 0]        ┆          ┆          ┆ 150.0, … ┆        ┆          ┆          ┆ 31.0, …  │
-    │ l", …     ┆           ┆          ┆          ┆ 836.0]   ┆        ┆          ┆          ┆ 706.0]   │
-    │ "SIL"]    ┆           ┆          ┆          ┆          ┆        ┆          ┆          ┆          │
-    │ ["SIL",   ┆ [0, 1, …  ┆ milk     ┆ 1        ┆ [47.0,   ┆ P54    ┆ 1        ┆ 4        ┆ [1.0,    │
-    │ "pour_mil ┆ 0]        ┆          ┆          ┆ 215.0, … ┆        ┆          ┆          ┆ 48.0, …  │
-    │ k", …     ┆           ┆          ┆          ┆ 747.0]   ┆        ┆          ┆          ┆ 566.0]   │
-    │ "SIL"]    ┆           ┆          ┆          ┆          ┆        ┆          ┆          ┆          │
-    └───────────┴───────────┴──────────┴──────────┴──────────┴────────┴──────────┴──────────┴──────────┘
+    shape: (2, 10)
+    ┌─────────┬─────────┬─────────┬─────────┬─────────┬────────┬─────────┬─────────┬─────────┬─────────┐
+    │ action  ┆ action_ ┆ cooking ┆ cooking ┆ end_tim ┆ person ┆ person_ ┆ sequenc ┆ start_t ┆ start_t │
+    │ ---     ┆ id      ┆ _activi ┆ _activi ┆ e       ┆ ---    ┆ id      ┆ e_lengt ┆ ime     ┆ ime_dif │
+    │ list[st ┆ ---     ┆ ty      ┆ ty_id   ┆ ---     ┆ str    ┆ ---     ┆ h       ┆ ---     ┆ f       │
+    │ r]      ┆ list[i6 ┆ ---     ┆ ---     ┆ list[f6 ┆        ┆ i64     ┆ ---     ┆ list[f6 ┆ ---     │
+    │         ┆ 4]      ┆ str     ┆ i64     ┆ 4]      ┆        ┆         ┆ i64     ┆ 4]      ┆ list[f6 │
+    │         ┆         ┆         ┆         ┆         ┆        ┆         ┆         ┆         ┆ 4]      │
+    ╞═════════╪═════════╪═════════╪═════════╪═════════╪════════╪═════════╪═════════╪═════════╪═════════╡
+    │ ["SIL", ┆ [0, 2,  ┆ cereals ┆ 0       ┆ [30.0,  ┆ P03    ┆ 0       ┆ 6       ┆ [1.0,   ┆ [0.0,   │
+    │ "take_b ┆ … 0]    ┆         ┆         ┆ 150.0,  ┆        ┆         ┆         ┆ 31.0, … ┆ 30.0, … │
+    │ owl", … ┆         ┆         ┆         ┆ …       ┆        ┆         ┆         ┆ 706.0]  ┆ 130.0]  │
+    │ "SIL"]  ┆         ┆         ┆         ┆ 836.0]  ┆        ┆         ┆         ┆         ┆         │
+    │ ["SIL", ┆ [0, 1,  ┆ milk    ┆ 1       ┆ [47.0,  ┆ P54    ┆ 1       ┆ 4       ┆ [1.0,   ┆ [0.0,   │
+    │ "pour_m ┆ … 0]    ┆         ┆         ┆ 215.0,  ┆        ┆         ┆         ┆ 48.0, … ┆ 47.0, … │
+    │ ilk", … ┆         ┆         ┆         ┆ …       ┆        ┆         ┆         ┆ 566.0]  ┆ 350.0]  │
+    │ "SIL"]  ┆         ┆         ┆         ┆ 747.0]  ┆        ┆         ┆         ┆         ┆         │
+    └─────────┴─────────┴─────────┴─────────┴─────────┴────────┴─────────┴─────────┴─────────┴─────────┘
 
     ```
     """
     data = frame.group_by([Column.PERSON_ID, Column.COOKING_ACTIVITY_ID]).agg(
         pl.first(Column.COOKING_ACTIVITY),
         pl.first(Column.PERSON),
         pl.col(Column.ACTION),
         pl.col(Column.ACTION_ID),
         pl.col(Column.START_TIME),
+        pl.col(Column.START_TIME_DIFF),
         pl.col(Column.END_TIME),
         pl.len().cast(pl.Int64).alias(Column.SEQUENCE_LENGTH),
     )
     transformer = td.Sequential(
         [
             td.Sort(columns=[Column.PERSON_ID, Column.COOKING_ACTIVITY_ID]),
             td.SortColumns(),
@@ -586,48 +596,55 @@
     ...             "milk",
     ...         ],
     ...         Column.COOKING_ACTIVITY_ID: [0, 0, 0, 0, 0, 0, 1, 1, 1, 1],
     ...         Column.END_TIME: [30.0, 150.0, 428.0, 575.0, 705.0, 836.0, 47.0, 215.0, 565.0, 747.0],
     ...         Column.PERSON: ["P03", "P03", "P03", "P03", "P03", "P03", "P54", "P54", "P54", "P54"],
     ...         Column.PERSON_ID: [0, 0, 0, 0, 0, 0, 1, 1, 1, 1],
     ...         Column.START_TIME: [1.0, 31.0, 151.0, 429.0, 576.0, 706.0, 1.0, 48.0, 216.0, 566.0],
+    ...         Column.START_TIME_DIFF: [0.0, 30.0, 120.0, 278.0, 147.0, 130.0, 0.0, 47.0, 168.0, 350.0],
     ...     }
     ... )
     >>> arrays = to_array(frame)
     >>> arrays
     {'action': masked_array(
       data=[['SIL', 'take_bowl', 'pour_cereals', 'pour_milk', 'stir_cereals',
              'SIL'],
             ['SIL', 'pour_milk', 'spoon_powder', 'SIL', --, --]],
       mask=[[False, False, False, False, False, False],
             [False, False, False, False,  True,  True]],
       fill_value='N/A',
-      dtype='<U12'), 'action_id': masked_array(
+      dtype='<U12'),
+      'action_id': masked_array(
       data=[[0, 2, 5, 1, 3, 0],
             [0, 1, 4, 0, --, --]],
       mask=[[False, False, False, False, False, False],
             [False, False, False, False,  True,  True]],
       fill_value=999999),
       'cooking_activity': array(['cereals', 'milk'], dtype='<U7'),
-      'cooking_activity_id': array([0, 1]),
-      'person': array(['P03', 'P54'], dtype='<U3'),
+      'cooking_activity_id': array([0, 1]), 'person': array(['P03', 'P54'], dtype='<U3'),
       'person_id': array([0, 1]),
       'sequence_length': array([6, 4]),
       'start_time': masked_array(
       data=[[1.0, 31.0, 151.0, 429.0, 576.0, 706.0],
             [1.0, 48.0, 216.0, 566.0, --, --]],
       mask=[[False, False, False, False, False, False],
             [False, False, False, False,  True,  True]],
+      fill_value=1e+20), 'start_time_diff': masked_array(
+      data=[[0.0, 30.0, 120.0, 278.0, 147.0, 130.0],
+            [0.0, 47.0, 168.0, 350.0, --, --]],
+      mask=[[False, False, False, False, False, False],
+            [False, False, False, False,  True,  True]],
       fill_value=1e+20), 'end_time': masked_array(
       data=[[30.0, 150.0, 428.0, 575.0, 705.0, 836.0],
             [47.0, 215.0, 565.0, 747.0, --, --]],
       mask=[[False, False, False, False, False, False],
             [False, False, False, False,  True,  True]],
       fill_value=1e+20)}
 
+
     ```
     """
     groups = group_by_sequence(frame)
     lengths = groups.get_column(Column.SEQUENCE_LENGTH).to_numpy()
     mask = generate_mask_from_lengths(lengths)
     return {
         Column.ACTION: np.ma.masked_array(
@@ -660,14 +677,23 @@
                 groups.get_column(Column.START_TIME).to_list(),
                 max_len=mask.shape[1],
                 dtype=np.float64,
                 padded_value=-1.0,
             ),
             mask=mask,
         ),
+        Column.START_TIME_DIFF: np.ma.masked_array(
+            data=convert_sequences_to_array(
+                groups.get_column(Column.START_TIME_DIFF).to_list(),
+                max_len=mask.shape[1],
+                dtype=np.float64,
+                padded_value=-1.0,
+            ),
+            mask=mask,
+        ),
         Column.END_TIME: np.ma.masked_array(
             data=convert_sequences_to_array(
                 groups.get_column(Column.END_TIME).to_list(),
                 max_len=mask.shape[1],
                 dtype=np.float64,
                 padded_value=-1.0,
             ),
@@ -719,27 +745,29 @@
     ...             "milk",
     ...         ],
     ...         Column.COOKING_ACTIVITY_ID: [0, 0, 0, 0, 0, 0, 1, 1, 1, 1],
     ...         Column.END_TIME: [30.0, 150.0, 428.0, 575.0, 705.0, 836.0, 47.0, 215.0, 565.0, 747.0],
     ...         Column.PERSON: ["P03", "P03", "P03", "P03", "P03", "P03", "P54", "P54", "P54", "P54"],
     ...         Column.PERSON_ID: [0, 0, 0, 0, 0, 0, 1, 1, 1, 1],
     ...         Column.START_TIME: [1.0, 31.0, 151.0, 429.0, 576.0, 706.0, 1.0, 48.0, 216.0, 566.0],
+    ...         Column.START_TIME_DIFF: [0.0, 30.0, 120.0, 278.0, 147.0, 130.0, 0.0, 47.0, 168.0, 350.0],
     ...     }
     ... )
     >>> data_list = to_list(frame)
     >>> data_list
     {'action': [['SIL', 'take_bowl', 'pour_cereals', 'pour_milk', 'stir_cereals', 'SIL'], ['SIL', 'pour_milk', 'spoon_powder', 'SIL']],
      'action_id': [[0, 2, 5, 1, 3, 0], [0, 1, 4, 0]],
      'cooking_activity': ['cereals', 'milk'],
      'cooking_activity_id': [0, 1],
      'end_time': [[30.0, 150.0, 428.0, 575.0, 705.0, 836.0], [47.0, 215.0, 565.0, 747.0]],
      'person': ['P03', 'P54'],
      'person_id': [0, 1],
      'sequence_length': [6, 4],
-     'start_time': [[1.0, 31.0, 151.0, 429.0, 576.0, 706.0], [1.0, 48.0, 216.0, 566.0]]}
+     'start_time': [[1.0, 31.0, 151.0, 429.0, 576.0, 706.0], [1.0, 48.0, 216.0, 566.0]],
+     'start_time_diff': [[0.0, 30.0, 120.0, 278.0, 147.0, 130.0], [0.0, 47.0, 168.0, 350.0]]}
 
     ```
     """
     return group_by_sequence(frame).to_dict(as_series=False)
 
 
 if __name__ == "__main__":  # pragma: no cover
```

### Comparing `arctix-0.0.5/src/arctix/dataset/ego4d.py` & `arctix-0.0.6/src/arctix/dataset/ego4d.py`

 * *Files 10% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     r"""Indicate the column names."""
 
     ACTION_END_FRAME: str = "action_clip_end_frame"
     ACTION_END_SEC: str = "action_clip_end_sec"
     ACTION_INDEX: str = "action_idx"
     ACTION_START_FRAME: str = "action_clip_start_frame"
     ACTION_START_SEC: str = "action_clip_start_sec"
+    ACTION_START_SEC_DIFF: str = "action_clip_start_sec_diff"
     CLIP_ID: str = "clip_uid"
     NOUN: str = "noun"
     NOUN_ID: str = "noun_label"
     VERB: str = "verb"
     VERB_ID: str = "verb_label"
     VIDEO_ID: str = "video_uid"
     SPLIT: str = "split"
@@ -273,21 +274,24 @@
     vocab = Vocabulary(Counter({token: 1 for token in data[name]}))
     if expected_size is not None and (count := len(vocab)) != expected_size:
         msg = f"Expected {expected_size} {name} but received {count:,}"
         raise RuntimeError(msg)
     return vocab
 
 
-def prepare_data(frame: pl.DataFrame, metadata: dict) -> tuple[pl.DataFrame, dict]:
+def prepare_data(
+    frame: pl.DataFrame, metadata: dict, group_col: str = Column.CLIP_ID
+) -> tuple[pl.DataFrame, dict]:
     r"""Prepare the data.
 
     Args:
         frame: The raw DataFrame.
         metadata: The metadata wich contains the vocabularies to
             convert verbs and nouns to index.
+        group_col: The column used to generate the sequences.
 
     Returns:
         A tuple containing the prepared data and the metadata.
 
     Example usage:
 
     ```pycon
@@ -309,36 +313,38 @@
     ...         Column.VERB_ID: [4, 2, 1, 1, 2],
     ...         Column.VIDEO_ID: ["video1", "video1", "video1", "video2", "video2"],
     ...     }
     ... )
     >>> data, metadata = prepare_data(frame, metadata={})
     >>> with pl.Config(tbl_cols=-1):
     ...     data
-    shape: (5, 12)
-    ┌────────┬────────┬────────┬───────┬───────┬───────┬───────┬───────┬───────┬───────┬───────┬───────┐
-    │ action ┆ action ┆ action ┆ actio ┆ actio ┆ clip_ ┆ noun  ┆ noun_ ┆ split ┆ verb  ┆ verb_ ┆ video │
-    │ _clip_ ┆ _clip_ ┆ _clip_ ┆ n_cli ┆ n_idx ┆ uid   ┆ ---   ┆ label ┆ ---   ┆ ---   ┆ label ┆ _uid  │
-    │ end_fr ┆ end_se ┆ start_ ┆ p_sta ┆ ---   ┆ ---   ┆ str   ┆ ---   ┆ str   ┆ str   ┆ ---   ┆ ---   │
-    │ ame    ┆ c      ┆ frame  ┆ rt_se ┆ i64   ┆ str   ┆       ┆ i64   ┆       ┆       ┆ i64   ┆ str   │
-    │ ---    ┆ ---    ┆ ---    ┆ c     ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       │
-    │ i64    ┆ f64    ┆ i64    ┆ ---   ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       │
-    │        ┆        ┆        ┆ f64   ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       │
-    ╞════════╪════════╪════════╪═══════╪═══════╪═══════╪═══════╪═══════╪═══════╪═══════╪═══════╪═══════╡
-    │ 47     ┆ 4.7    ┆ 23     ┆ 2.3   ┆ 0     ┆ clip1 ┆ noun2 ┆ 2     ┆ train ┆ verb4 ┆ 4     ┆ video │
-    │        ┆        ┆        ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆ 1     │
-    │ 82     ┆ 8.2    ┆ 39     ┆ 3.9   ┆ 1     ┆ clip1 ┆ noun3 ┆ 3     ┆ train ┆ verb2 ┆ 2     ┆ video │
-    │        ┆        ┆        ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆ 1     │
-    │ 102    ┆ 10.2   ┆ 74     ┆ 7.4   ┆ 2     ┆ clip1 ┆ noun1 ┆ 1     ┆ train ┆ verb1 ┆ 1     ┆ video │
-    │        ┆        ┆        ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆ 1     │
-    │ 74     ┆ 7.4    ┆ 12     ┆ 1.2   ┆ 0     ┆ clip2 ┆ noun1 ┆ 1     ┆ train ┆ verb1 ┆ 1     ┆ video │
-    │        ┆        ┆        ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆ 2     │
-    │ 142    ┆ 14.2   ┆ 82     ┆ 8.2   ┆ 1     ┆ clip2 ┆ noun2 ┆ 2     ┆ train ┆ verb2 ┆ 2     ┆ video │
-    │        ┆        ┆        ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆ 2     │
-    └────────┴────────┴────────┴───────┴───────┴───────┴───────┴───────┴───────┴───────┴───────┴───────┘
-
+    shape: (5, 13)
+    ┌─────┬─────┬─────┬────────┬───────┬───────┬───────┬───────┬───────┬───────┬───────┬───────┬───────┐
+    │ act ┆ act ┆ act ┆ action ┆ actio ┆ actio ┆ clip_ ┆ noun  ┆ noun_ ┆ split ┆ verb  ┆ verb_ ┆ video │
+    │ ion ┆ ion ┆ ion ┆ _clip_ ┆ n_cli ┆ n_idx ┆ uid   ┆ ---   ┆ label ┆ ---   ┆ ---   ┆ label ┆ _uid  │
+    │ _cl ┆ _cl ┆ _cl ┆ start_ ┆ p_sta ┆ ---   ┆ ---   ┆ str   ┆ ---   ┆ str   ┆ str   ┆ ---   ┆ ---   │
+    │ ip_ ┆ ip_ ┆ ip_ ┆ sec    ┆ rt_se ┆ i64   ┆ str   ┆       ┆ i64   ┆       ┆       ┆ i64   ┆ str   │
+    │ end ┆ end ┆ sta ┆ ---    ┆ c_dif ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       │
+    │ _fr ┆ _se ┆ rt_ ┆ f64    ┆ f     ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       │
+    │ ame ┆ c   ┆ fra ┆        ┆ ---   ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       │
+    │ --- ┆ --- ┆ me  ┆        ┆ f64   ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       │
+    │ i64 ┆ f64 ┆ --- ┆        ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       │
+    │     ┆     ┆ i64 ┆        ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       │
+    ╞═════╪═════╪═════╪════════╪═══════╪═══════╪═══════╪═══════╪═══════╪═══════╪═══════╪═══════╪═══════╡
+    │ 47  ┆ 4.7 ┆ 23  ┆ 2.3    ┆ 0.0   ┆ 0     ┆ clip1 ┆ noun2 ┆ 2     ┆ train ┆ verb4 ┆ 4     ┆ video │
+    │     ┆     ┆     ┆        ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆ 1     │
+    │ 82  ┆ 8.2 ┆ 39  ┆ 3.9    ┆ 1.6   ┆ 1     ┆ clip1 ┆ noun3 ┆ 3     ┆ train ┆ verb2 ┆ 2     ┆ video │
+    │     ┆     ┆     ┆        ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆ 1     │
+    │ 102 ┆ 10. ┆ 74  ┆ 7.4    ┆ 3.5   ┆ 2     ┆ clip1 ┆ noun1 ┆ 1     ┆ train ┆ verb1 ┆ 1     ┆ video │
+    │     ┆ 2   ┆     ┆        ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆ 1     │
+    │ 74  ┆ 7.4 ┆ 12  ┆ 1.2    ┆ 0.0   ┆ 0     ┆ clip2 ┆ noun1 ┆ 1     ┆ train ┆ verb1 ┆ 1     ┆ video │
+    │     ┆     ┆     ┆        ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆ 2     │
+    │ 142 ┆ 14. ┆ 82  ┆ 8.2    ┆ 7.0   ┆ 1     ┆ clip2 ┆ noun2 ┆ 2     ┆ train ┆ verb2 ┆ 2     ┆ video │
+    │     ┆ 2   ┆     ┆        ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆       ┆ 2     │
+    └─────┴─────┴─────┴────────┴───────┴───────┴───────┴───────┴───────┴───────┴───────┴───────┴───────┘
     >>> metadata
     {}
 
     ```
     """
     transformer = td.Sequential(
         [
@@ -349,15 +355,20 @@
                     Column.ACTION_START_FRAME,
                     Column.NOUN_ID,
                     Column.VERB_ID,
                 ],
                 dtype=pl.Int64,
             ),
             td.Cast(columns=[Column.ACTION_START_SEC, Column.ACTION_END_SEC], dtype=pl.Float64),
-            td.Sort(columns=[Column.VIDEO_ID, Column.CLIP_ID, Column.ACTION_INDEX]),
+            td.TimeDiff(
+                group_cols=[group_col],
+                time_col=Column.ACTION_START_SEC,
+                time_diff_col=Column.ACTION_START_SEC_DIFF,
+            ),
+            td.Sort(columns=[group_col, Column.ACTION_INDEX]),
             td.SortColumns(),
         ]
     )
     out = transformer.transform(frame)
     return out, metadata
 
 
@@ -379,58 +390,63 @@
     >>> from arctix.dataset.ego4d import Column, group_by_sequence
     >>> frame = pl.DataFrame(
     ...     {
     ...         Column.ACTION_END_FRAME: [47, 82, 102, 74, 142],
     ...         Column.ACTION_END_SEC: [4.7, 8.2, 10.2, 7.4, 14.2],
     ...         Column.ACTION_START_FRAME: [23, 39, 74, 12, 82],
     ...         Column.ACTION_START_SEC: [2.3, 3.9, 7.4, 1.2, 8.2],
+    ...         Column.ACTION_START_SEC_DIFF: [0.0, 1.6, 3.5, 0.0, 7.0],
     ...         Column.ACTION_INDEX: [0, 1, 2, 0, 1],
     ...         Column.CLIP_ID: ["clip1", "clip1", "clip1", "clip2", "clip2"],
     ...         Column.NOUN: ["noun2", "noun3", "noun1", "noun1", "noun2"],
     ...         Column.NOUN_ID: [2, 3, 1, 1, 2],
     ...         Column.SPLIT: ["train", "train", "train", "train", "train"],
     ...         Column.VERB: ["verb4", "verb2", "verb1", "verb1", "verb2"],
     ...         Column.VERB_ID: [4, 2, 1, 1, 2],
     ...         Column.VIDEO_ID: ["video1", "video1", "video1", "video2", "video2"],
     ...     }
     ... )
     >>> data = group_by_sequence(frame)
     >>> with pl.Config(tbl_cols=-1):
     ...     data
-    shape: (2, 11)
-    ┌─────────┬────────┬────────┬────────┬────────┬────────┬────────┬────────┬───────┬────────┬────────┐
-    │ action_ ┆ action ┆ action ┆ action ┆ clip_u ┆ noun   ┆ noun_l ┆ sequen ┆ split ┆ verb   ┆ verb_l │
-    │ clip_en ┆ _clip_ ┆ _clip_ ┆ _clip_ ┆ id     ┆ ---    ┆ abel   ┆ ce_len ┆ ---   ┆ ---    ┆ abel   │
-    │ d_frame ┆ end_se ┆ start_ ┆ start_ ┆ ---    ┆ list[s ┆ ---    ┆ gth    ┆ str   ┆ list[s ┆ ---    │
-    │ ---     ┆ c      ┆ frame  ┆ sec    ┆ str    ┆ tr]    ┆ list[i ┆ ---    ┆       ┆ tr]    ┆ list[i │
-    │ list[i6 ┆ ---    ┆ ---    ┆ ---    ┆        ┆        ┆ 64]    ┆ i64    ┆       ┆        ┆ 64]    │
-    │ 4]      ┆ list[f ┆ list[i ┆ list[f ┆        ┆        ┆        ┆        ┆       ┆        ┆        │
-    │         ┆ 64]    ┆ 64]    ┆ 64]    ┆        ┆        ┆        ┆        ┆       ┆        ┆        │
-    ╞═════════╪════════╪════════╪════════╪════════╪════════╪════════╪════════╪═══════╪════════╪════════╡
-    │ [47,    ┆ [4.7,  ┆ [23,   ┆ [2.3,  ┆ clip1  ┆ ["noun ┆ [2, 3, ┆ 3      ┆ train ┆ ["verb ┆ [4, 2, │
-    │ 82,     ┆ 8.2,   ┆ 39,    ┆ 3.9,   ┆        ┆ 2",    ┆ 1]     ┆        ┆       ┆ 4",    ┆ 1]     │
-    │ 102]    ┆ 10.2]  ┆ 74]    ┆ 7.4]   ┆        ┆ "noun3 ┆        ┆        ┆       ┆ "verb2 ┆        │
-    │         ┆        ┆        ┆        ┆        ┆ ", "no ┆        ┆        ┆       ┆ ", "ve ┆        │
-    │         ┆        ┆        ┆        ┆        ┆ un1"]  ┆        ┆        ┆       ┆ rb1"]  ┆        │
-    │ [74,    ┆ [7.4,  ┆ [12,   ┆ [1.2,  ┆ clip2  ┆ ["noun ┆ [1, 2] ┆ 2      ┆ train ┆ ["verb ┆ [1, 2] │
-    │ 142]    ┆ 14.2]  ┆ 82]    ┆ 8.2]   ┆        ┆ 1",    ┆        ┆        ┆       ┆ 1",    ┆        │
-    │         ┆        ┆        ┆        ┆        ┆ "noun2 ┆        ┆        ┆       ┆ "verb2 ┆        │
-    │         ┆        ┆        ┆        ┆        ┆ "]     ┆        ┆        ┆       ┆ "]     ┆        │
-    └─────────┴────────┴────────┴────────┴────────┴────────┴────────┴────────┴───────┴────────┴────────┘
+    shape: (2, 12)
+    ┌────────┬────────┬────────┬───────┬───────┬───────┬───────┬───────┬───────┬───────┬───────┬───────┐
+    │ action ┆ action ┆ action ┆ actio ┆ actio ┆ clip_ ┆ noun  ┆ noun_ ┆ seque ┆ split ┆ verb  ┆ verb_ │
+    │ _clip_ ┆ _clip_ ┆ _clip_ ┆ n_cli ┆ n_cli ┆ uid   ┆ ---   ┆ label ┆ nce_l ┆ ---   ┆ ---   ┆ label │
+    │ end_fr ┆ end_se ┆ start_ ┆ p_sta ┆ p_sta ┆ ---   ┆ list[ ┆ ---   ┆ ength ┆ str   ┆ list[ ┆ ---   │
+    │ ame    ┆ c      ┆ frame  ┆ rt_se ┆ rt_se ┆ str   ┆ str]  ┆ list[ ┆ ---   ┆       ┆ str]  ┆ list[ │
+    │ ---    ┆ ---    ┆ ---    ┆ c     ┆ c_dif ┆       ┆       ┆ i64]  ┆ i64   ┆       ┆       ┆ i64]  │
+    │ list[i ┆ list[f ┆ list[i ┆ ---   ┆ f     ┆       ┆       ┆       ┆       ┆       ┆       ┆       │
+    │ 64]    ┆ 64]    ┆ 64]    ┆ list[ ┆ ---   ┆       ┆       ┆       ┆       ┆       ┆       ┆       │
+    │        ┆        ┆        ┆ f64]  ┆ list[ ┆       ┆       ┆       ┆       ┆       ┆       ┆       │
+    │        ┆        ┆        ┆       ┆ f64]  ┆       ┆       ┆       ┆       ┆       ┆       ┆       │
+    ╞════════╪════════╪════════╪═══════╪═══════╪═══════╪═══════╪═══════╪═══════╪═══════╪═══════╪═══════╡
+    │ [47,   ┆ [4.7,  ┆ [23,   ┆ [2.3, ┆ [0.0, ┆ clip1 ┆ ["nou ┆ [2,   ┆ 3     ┆ train ┆ ["ver ┆ [4,   │
+    │ 82,    ┆ 8.2,   ┆ 39,    ┆ 3.9,  ┆ 1.6,  ┆       ┆ n2",  ┆ 3, 1] ┆       ┆       ┆ b4",  ┆ 2, 1] │
+    │ 102]   ┆ 10.2]  ┆ 74]    ┆ 7.4]  ┆ 3.5]  ┆       ┆ "noun ┆       ┆       ┆       ┆ "verb ┆       │
+    │        ┆        ┆        ┆       ┆       ┆       ┆ 3",   ┆       ┆       ┆       ┆ 2",   ┆       │
+    │        ┆        ┆        ┆       ┆       ┆       ┆ "noun ┆       ┆       ┆       ┆ "verb ┆       │
+    │        ┆        ┆        ┆       ┆       ┆       ┆ 1"]   ┆       ┆       ┆       ┆ 1"]   ┆       │
+    │ [74,   ┆ [7.4,  ┆ [12,   ┆ [1.2, ┆ [0.0, ┆ clip2 ┆ ["nou ┆ [1,   ┆ 2     ┆ train ┆ ["ver ┆ [1,   │
+    │ 142]   ┆ 14.2]  ┆ 82]    ┆ 8.2]  ┆ 7.0]  ┆       ┆ n1",  ┆ 2]    ┆       ┆       ┆ b1",  ┆ 2]    │
+    │        ┆        ┆        ┆       ┆       ┆       ┆ "noun ┆       ┆       ┆       ┆ "verb ┆       │
+    │        ┆        ┆        ┆       ┆       ┆       ┆ 2"]   ┆       ┆       ┆       ┆ 2"]   ┆       │
+    └────────┴────────┴────────┴───────┴───────┴───────┴───────┴───────┴───────┴───────┴───────┴───────┘
 
     ```
     """
     data = (
         frame.sort(by=[Column.VIDEO_ID, Column.CLIP_ID, Column.ACTION_INDEX])
         .group_by([group_col])
         .agg(
             pl.col(Column.ACTION_END_FRAME),
             pl.col(Column.ACTION_END_SEC),
             pl.col(Column.ACTION_START_FRAME),
             pl.col(Column.ACTION_START_SEC),
+            pl.col(Column.ACTION_START_SEC_DIFF),
             pl.col(Column.NOUN),
             pl.col(Column.NOUN_ID),
             pl.col(Column.VERB),
             pl.col(Column.VERB_ID),
             pl.first(Column.SPLIT),
             pl.len().cast(pl.Int64).alias(Column.SEQUENCE_LENGTH),
         )
@@ -462,14 +478,15 @@
     >>> from arctix.dataset.ego4d import Column, to_array
     >>> frame = pl.DataFrame(
     ...     {
     ...         Column.ACTION_END_FRAME: [47, 82, 102, 74, 142],
     ...         Column.ACTION_END_SEC: [4.7, 8.2, 10.2, 7.4, 14.2],
     ...         Column.ACTION_START_FRAME: [23, 39, 74, 12, 82],
     ...         Column.ACTION_START_SEC: [2.3, 3.9, 7.4, 1.2, 8.2],
+    ...         Column.ACTION_START_SEC_DIFF: [0.0, 1.6, 3.5, 0.0, 7.0],
     ...         Column.ACTION_INDEX: [0, 1, 2, 0, 1],
     ...         Column.CLIP_ID: ["clip1", "clip1", "clip1", "clip2", "clip2"],
     ...         Column.NOUN: ["noun2", "noun3", "noun1", "noun1", "noun2"],
     ...         Column.NOUN_ID: [2, 3, 1, 1, 2],
     ...         Column.SPLIT: ["train", "train", "train", "train", "train"],
     ...         Column.VERB: ["verb4", "verb2", "verb1", "verb1", "verb2"],
     ...         Column.VERB_ID: [4, 2, 1, 1, 2],
@@ -480,52 +497,67 @@
     >>> arrays
     {'noun': masked_array(
       data=[['noun2', 'noun3', 'noun1'],
             ['noun1', 'noun2', --]],
       mask=[[False, False, False],
             [False, False,  True]],
       fill_value='N/A',
-      dtype='<U5'), 'noun_label': masked_array(
+      dtype='<U5'),
+      'noun_label': masked_array(
       data=[[2, 3, 1],
             [1, 2, --]],
       mask=[[False, False, False],
             [False, False,  True]],
-      fill_value=999999), 'split': array(['train', 'train'], dtype='<U5'),
-      'sequence_length': array([3, 2]), 'action_clip_start_frame': masked_array(
+      fill_value=999999),
+      'split': array(['train', 'train'], dtype='<U5'),
+      'sequence_length': array([3, 2]),
+      'action_clip_start_frame': masked_array(
       data=[[23, 39, 74],
             [12, 82, --]],
       mask=[[False, False, False],
             [False, False,  True]],
-      fill_value=999999), 'action_clip_start_sec': masked_array(
+      fill_value=999999),
+      'action_clip_start_sec': masked_array(
       data=[[2.3, 3.9, 7.4],
             [1.2, 8.2, --]],
       mask=[[False, False, False],
             [False, False,  True]],
-      fill_value=1e+20), 'action_clip_end_frame': masked_array(
+      fill_value=1e+20),
+      'action_clip_start_sec_diff': masked_array(
+      data=[[0.0, 1.6, 3.5],
+            [0.0, 7.0, --]],
+      mask=[[False, False, False],
+            [False, False,  True]],
+      fill_value=1e+20),
+      'action_clip_end_frame': masked_array(
       data=[[47, 82, 102],
             [74, 142, --]],
       mask=[[False, False, False],
             [False, False,  True]],
-      fill_value=999999), 'action_clip_end_sec': masked_array(
+      fill_value=999999),
+      'action_clip_end_sec': masked_array(
       data=[[4.7, 8.2, 10.2],
             [7.4, 14.2, --]],
       mask=[[False, False, False],
             [False, False,  True]],
-      fill_value=1e+20), 'verb': masked_array(
+      fill_value=1e+20),
+      'verb': masked_array(
       data=[['verb4', 'verb2', 'verb1'],
             ['verb1', 'verb2', --]],
       mask=[[False, False, False],
             [False, False,  True]],
       fill_value='N/A',
-      dtype='<U5'), 'verb_label': masked_array(
+      dtype='<U5'),
+      'verb_label': masked_array(
       data=[[4, 2, 1],
             [1, 2, --]],
       mask=[[False, False, False],
             [False, False,  True]],
-      fill_value=999999), 'clip_uid': array(['clip1', 'clip2'], dtype='<U5')}
+      fill_value=999999),
+      'clip_uid': array(['clip1', 'clip2'], dtype='<U5')}
 
     ```
     """
     groups = group_by_sequence(frame, group_col)
     lengths = groups.get_column(Column.SEQUENCE_LENGTH).to_numpy()
     mask = generate_mask_from_lengths(lengths)
     return {
@@ -565,14 +597,23 @@
                 groups.get_column(Column.ACTION_START_SEC).to_list(),
                 max_len=mask.shape[1],
                 dtype=np.float64,
                 padded_value=-1.0,
             ),
             mask=mask,
         ),
+        Column.ACTION_START_SEC_DIFF: np.ma.masked_array(
+            data=convert_sequences_to_array(
+                groups.get_column(Column.ACTION_START_SEC_DIFF).to_list(),
+                max_len=mask.shape[1],
+                dtype=np.float64,
+                padded_value=-1.0,
+            ),
+            mask=mask,
+        ),
         Column.ACTION_END_FRAME: np.ma.masked_array(
             data=convert_sequences_to_array(
                 groups.get_column(Column.ACTION_END_FRAME).to_list(),
                 max_len=mask.shape[1],
                 dtype=np.int64,
                 padded_value=-1,
             ),
@@ -627,14 +668,15 @@
     >>> from arctix.dataset.ego4d import Column, to_list
     >>> frame = pl.DataFrame(
     ...     {
     ...         Column.ACTION_END_FRAME: [47, 82, 102, 74, 142],
     ...         Column.ACTION_END_SEC: [4.7, 8.2, 10.2, 7.4, 14.2],
     ...         Column.ACTION_START_FRAME: [23, 39, 74, 12, 82],
     ...         Column.ACTION_START_SEC: [2.3, 3.9, 7.4, 1.2, 8.2],
+    ...         Column.ACTION_START_SEC_DIFF: [0.0, 1.6, 3.5, 0.0, 7.0],
     ...         Column.ACTION_INDEX: [0, 1, 2, 0, 1],
     ...         Column.CLIP_ID: ["clip1", "clip1", "clip1", "clip2", "clip2"],
     ...         Column.NOUN: ["noun2", "noun3", "noun1", "noun1", "noun2"],
     ...         Column.NOUN_ID: [2, 3, 1, 1, 2],
     ...         Column.SPLIT: ["train", "train", "train", "train", "train"],
     ...         Column.VERB: ["verb4", "verb2", "verb1", "verb1", "verb2"],
     ...         Column.VERB_ID: [4, 2, 1, 1, 2],
@@ -643,14 +685,15 @@
     ... )
     >>> data_list = to_list(frame)
     >>> data_list
     {'action_clip_end_frame': [[47, 82, 102], [74, 142]],
      'action_clip_end_sec': [[4.7, 8.2, 10.2], [7.4, 14.2]],
      'action_clip_start_frame': [[23, 39, 74], [12, 82]],
      'action_clip_start_sec': [[2.3, 3.9, 7.4], [1.2, 8.2]],
+     'action_clip_start_sec_diff': [[0.0, 1.6, 3.5], [0.0, 7.0]],
      'clip_uid': ['clip1', 'clip2'],
      'noun': [['noun2', 'noun3', 'noun1'], ['noun1', 'noun2']],
      'noun_label': [[2, 3, 1], [1, 2]],
      'sequence_length': [3, 2],
      'split': ['train', 'train'],
      'verb': [['verb4', 'verb2', 'verb1'], ['verb1', 'verb2']],
      'verb_label': [[4, 2, 1], [1, 2]]}
```

### Comparing `arctix-0.0.5/src/arctix/dataset/epic_kitchen_100.py` & `arctix-0.0.6/src/arctix/dataset/epic_kitchen_100.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     NOUN: str = "noun"
     NOUN_ID: str = "noun_class"
     PARTICIPANT_ID: str = "participant_id"
     SEQUENCE_LENGTH: str = "sequence_length"
     START_FRAME: str = "start_frame"
     START_TIMESTAMP: str = "start_timestamp"
     START_TIME_SECOND: str = "start_time_second"
+    START_TIME_SECOND_DIFF: str = "start_time_second_diff"
     STOP_FRAME: str = "stop_frame"
     STOP_TIMESTAMP: str = "stop_timestamp"
     STOP_TIME_SECOND: str = "stop_time_second"
     VERB: str = "verb"
     VERB_ID: str = "verb_class"
     VIDEO_ID: str = "video_id"
 
@@ -405,51 +406,56 @@
     ...         Column.VERB_ID: pl.Int64,
     ...         Column.VIDEO_ID: pl.String,
     ...     },
     ... )
     >>> data, metadata = prepare_data(frame, metadata={})
     >>> with pl.Config(tbl_cols=-1):
     ...     data
-    shape: (3, 17)
-    ┌─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┐
-    │ all ┆ all ┆ nar ┆ nar ┆ nar ┆ nou ┆ nou ┆ par ┆ sta ┆ sta ┆ sta ┆ sto ┆ sto ┆ sto ┆ ver ┆ ver ┆ vid │
-    │ _no ┆ _no ┆ rat ┆ rat ┆ rat ┆ n   ┆ n_c ┆ tic ┆ rt_ ┆ rt_ ┆ rt_ ┆ p_f ┆ p_t ┆ p_t ┆ b   ┆ b_c ┆ eo_ │
-    │ un_ ┆ uns ┆ ion ┆ ion ┆ ion ┆ --- ┆ las ┆ ipa ┆ fra ┆ tim ┆ tim ┆ ram ┆ ime ┆ ime ┆ --- ┆ las ┆ id  │
-    │ cla ┆ --- ┆ --- ┆ _id ┆ _ti ┆ str ┆ s   ┆ nt_ ┆ me  ┆ e_s ┆ est ┆ e   ┆ _se ┆ sta ┆ str ┆ s   ┆ --- │
-    │ sse ┆ lis ┆ str ┆ --- ┆ mes ┆     ┆ --- ┆ id  ┆ --- ┆ eco ┆ amp ┆ --- ┆ con ┆ mp  ┆     ┆ --- ┆ str │
-    │ s   ┆ t[s ┆     ┆ str ┆ tam ┆     ┆ i64 ┆ --- ┆ i64 ┆ nd  ┆ --- ┆ i64 ┆ d   ┆ --- ┆     ┆ i64 ┆     │
-    │ --- ┆ tr] ┆     ┆     ┆ p   ┆     ┆     ┆ str ┆     ┆ --- ┆ tim ┆     ┆ --- ┆ tim ┆     ┆     ┆     │
-    │ lis ┆     ┆     ┆     ┆ --- ┆     ┆     ┆     ┆     ┆ f64 ┆ e   ┆     ┆ f64 ┆ e   ┆     ┆     ┆     │
-    │ t[i ┆     ┆     ┆     ┆ tim ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     │
-    │ 64] ┆     ┆     ┆     ┆ e   ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     │
-    ╞═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╡
-    │ [3] ┆ ["d ┆ ope ┆ P01 ┆ 00: ┆ doo ┆ 3   ┆ P01 ┆ 8   ┆ 0.1 ┆ 00: ┆ 202 ┆ 3.3 ┆ 00: ┆ ope ┆ 3   ┆ P01 │
-    │     ┆ oor ┆ n   ┆ _01 ┆ 00: ┆ r   ┆     ┆     ┆     ┆ 4   ┆ 00: ┆     ┆ 7   ┆ 00: ┆ n   ┆     ┆ _01 │
-    │     ┆ "]  ┆ doo ┆ _0  ┆ 01. ┆     ┆     ┆     ┆     ┆     ┆ 00. ┆     ┆     ┆ 03. ┆     ┆     ┆     │
-    │     ┆     ┆ r   ┆     ┆ 089 ┆     ┆     ┆     ┆     ┆     ┆ 140 ┆     ┆     ┆ 370 ┆     ┆     ┆     │
-    │ [11 ┆ ["l ┆ tur ┆ P01 ┆ 00: ┆ lig ┆ 114 ┆ P01 ┆ 262 ┆ 4.3 ┆ 00: ┆ 370 ┆ 6.1 ┆ 00: ┆ tur ┆ 6   ┆ P01 │
-    │ 4]  ┆ igh ┆ n   ┆ _01 ┆ 00: ┆ ht  ┆     ┆     ┆     ┆ 7   ┆ 00: ┆     ┆ 7   ┆ 00: ┆ n-o ┆     ┆ _01 │
-    │     ┆ t"] ┆ on  ┆ _1  ┆ 02. ┆     ┆     ┆     ┆     ┆     ┆ 04. ┆     ┆     ┆ 06. ┆ n   ┆     ┆     │
-    │     ┆     ┆ lig ┆     ┆ 629 ┆     ┆     ┆     ┆     ┆     ┆ 370 ┆     ┆     ┆ 170 ┆     ┆     ┆     │
-    │     ┆     ┆ ht  ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     │
-    │ [3] ┆ ["d ┆ clo ┆ P01 ┆ 00: ┆ doo ┆ 3   ┆ P01 ┆ 418 ┆ 6.9 ┆ 00: ┆ 569 ┆ 9.4 ┆ 00: ┆ clo ┆ 4   ┆ P01 │
-    │     ┆ oor ┆ se  ┆ _01 ┆ 00: ┆ r   ┆     ┆     ┆     ┆ 8   ┆ 00: ┆     ┆ 9   ┆ 00: ┆ se  ┆     ┆ _01 │
-    │     ┆ "]  ┆ doo ┆ _2  ┆ 05. ┆     ┆     ┆     ┆     ┆     ┆ 06. ┆     ┆     ┆ 09. ┆     ┆     ┆     │
-    │     ┆     ┆ r   ┆     ┆ 349 ┆     ┆     ┆     ┆     ┆     ┆ 980 ┆     ┆     ┆ 490 ┆     ┆     ┆     │
-    └─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┘
+    shape: (3, 18)
+    ┌─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┬─────┐
+    │ all ┆ all ┆ nar ┆ nar ┆ nar ┆ nou ┆ nou ┆ par ┆ sta ┆ sta ┆ sta ┆ sta ┆ sto ┆ sto ┆ sto ┆ ver ┆ ver ┆ vid │
+    │ _no ┆ _no ┆ rat ┆ rat ┆ rat ┆ n   ┆ n_c ┆ tic ┆ rt_ ┆ rt_ ┆ rt_ ┆ rt_ ┆ p_f ┆ p_t ┆ p_t ┆ b   ┆ b_c ┆ eo_ │
+    │ un_ ┆ uns ┆ ion ┆ ion ┆ ion ┆ --- ┆ las ┆ ipa ┆ fra ┆ tim ┆ tim ┆ tim ┆ ram ┆ ime ┆ ime ┆ --- ┆ las ┆ id  │
+    │ cla ┆ --- ┆ --- ┆ _id ┆ _ti ┆ str ┆ s   ┆ nt_ ┆ me  ┆ e_s ┆ e_s ┆ est ┆ e   ┆ _se ┆ sta ┆ str ┆ s   ┆ --- │
+    │ sse ┆ lis ┆ str ┆ --- ┆ mes ┆     ┆ --- ┆ id  ┆ --- ┆ eco ┆ eco ┆ amp ┆ --- ┆ con ┆ mp  ┆     ┆ --- ┆ str │
+    │ s   ┆ t[s ┆     ┆ str ┆ tam ┆     ┆ i64 ┆ --- ┆ i64 ┆ nd  ┆ nd_ ┆ --- ┆ i64 ┆ d   ┆ --- ┆     ┆ i64 ┆     │
+    │ --- ┆ tr] ┆     ┆     ┆ p   ┆     ┆     ┆ str ┆     ┆ --- ┆ dif ┆ tim ┆     ┆ --- ┆ tim ┆     ┆     ┆     │
+    │ lis ┆     ┆     ┆     ┆ --- ┆     ┆     ┆     ┆     ┆ f64 ┆ f   ┆ e   ┆     ┆ f64 ┆ e   ┆     ┆     ┆     │
+    │ t[i ┆     ┆     ┆     ┆ tim ┆     ┆     ┆     ┆     ┆     ┆ --- ┆     ┆     ┆     ┆     ┆     ┆     ┆     │
+    │ 64] ┆     ┆     ┆     ┆ e   ┆     ┆     ┆     ┆     ┆     ┆ f64 ┆     ┆     ┆     ┆     ┆     ┆     ┆     │
+    ╞═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╪═════╡
+    │ [3] ┆ ["d ┆ ope ┆ P01 ┆ 00: ┆ doo ┆ 3   ┆ P01 ┆ 8   ┆ 0.1 ┆ 0.0 ┆ 00: ┆ 202 ┆ 3.3 ┆ 00: ┆ ope ┆ 3   ┆ P01 │
+    │     ┆ oor ┆ n   ┆ _01 ┆ 00: ┆ r   ┆     ┆     ┆     ┆ 4   ┆     ┆ 00: ┆     ┆ 7   ┆ 00: ┆ n   ┆     ┆ _01 │
+    │     ┆ "]  ┆ doo ┆ _0  ┆ 01. ┆     ┆     ┆     ┆     ┆     ┆     ┆ 00. ┆     ┆     ┆ 03. ┆     ┆     ┆     │
+    │     ┆     ┆ r   ┆     ┆ 089 ┆     ┆     ┆     ┆     ┆     ┆     ┆ 140 ┆     ┆     ┆ 370 ┆     ┆     ┆     │
+    │ [11 ┆ ["l ┆ tur ┆ P01 ┆ 00: ┆ lig ┆ 114 ┆ P01 ┆ 262 ┆ 4.3 ┆ 4.2 ┆ 00: ┆ 370 ┆ 6.1 ┆ 00: ┆ tur ┆ 6   ┆ P01 │
+    │ 4]  ┆ igh ┆ n   ┆ _01 ┆ 00: ┆ ht  ┆     ┆     ┆     ┆ 7   ┆ 3   ┆ 00: ┆     ┆ 7   ┆ 00: ┆ n-o ┆     ┆ _01 │
+    │     ┆ t"] ┆ on  ┆ _1  ┆ 02. ┆     ┆     ┆     ┆     ┆     ┆     ┆ 04. ┆     ┆     ┆ 06. ┆ n   ┆     ┆     │
+    │     ┆     ┆ lig ┆     ┆ 629 ┆     ┆     ┆     ┆     ┆     ┆     ┆ 370 ┆     ┆     ┆ 170 ┆     ┆     ┆     │
+    │     ┆     ┆ ht  ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     ┆     │
+    │ [3] ┆ ["d ┆ clo ┆ P01 ┆ 00: ┆ doo ┆ 3   ┆ P01 ┆ 418 ┆ 6.9 ┆ 2.6 ┆ 00: ┆ 569 ┆ 9.4 ┆ 00: ┆ clo ┆ 4   ┆ P01 │
+    │     ┆ oor ┆ se  ┆ _01 ┆ 00: ┆ r   ┆     ┆     ┆     ┆ 8   ┆ 1   ┆ 00: ┆     ┆ 9   ┆ 00: ┆ se  ┆     ┆ _01 │
+    │     ┆ "]  ┆ doo ┆ _2  ┆ 05. ┆     ┆     ┆     ┆     ┆     ┆     ┆ 06. ┆     ┆     ┆ 09. ┆     ┆     ┆     │
+    │     ┆     ┆ r   ┆     ┆ 349 ┆     ┆     ┆     ┆     ┆     ┆     ┆ 980 ┆     ┆     ┆ 490 ┆     ┆     ┆     │
+    └─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┴─────┘
     >>> metadata
     {}
 
     ```
     """
     transformer = td.Sequential(
         [
-            td.Sort(columns=[Column.VIDEO_ID, Column.START_FRAME]),
             td.TimeToSecond(in_col=Column.START_TIMESTAMP, out_col=Column.START_TIME_SECOND),
             td.TimeToSecond(in_col=Column.STOP_TIMESTAMP, out_col=Column.STOP_TIME_SECOND),
+            td.TimeDiff(
+                group_cols=[Column.VIDEO_ID],
+                time_col=Column.START_TIME_SECOND,
+                time_diff_col=Column.START_TIME_SECOND_DIFF,
+            ),
+            td.Sort(columns=[Column.VIDEO_ID, Column.START_FRAME]),
             td.Cast(columns=[Column.START_TIME_SECOND, Column.STOP_TIME_SECOND], dtype=pl.Float64),
             td.SortColumns(),
         ]
     )
     out = transformer.transform(frame)
     return out, metadata
 
@@ -474,14 +480,15 @@
             pl.col(Column.NARRATION_ID),
             pl.col(Column.NARRATION_TIMESTAMP),
             pl.col(Column.NOUN),
             pl.col(Column.NOUN_ID),
             pl.col(Column.START_FRAME),
             pl.col(Column.START_TIMESTAMP),
             pl.col(Column.START_TIME_SECOND),
+            pl.col(Column.START_TIME_SECOND_DIFF),
             pl.col(Column.STOP_FRAME),
             pl.col(Column.STOP_TIMESTAMP),
             pl.col(Column.STOP_TIME_SECOND),
             pl.col(Column.VERB),
             pl.col(Column.VERB_ID),
             pl.len().cast(pl.Int64).alias(Column.SEQUENCE_LENGTH),
         )
@@ -562,14 +569,23 @@
                 groups.get_column(Column.START_TIME_SECOND).to_list(),
                 max_len=mask.shape[1],
                 dtype=np.float64,
                 padded_value=-1.0,
             ),
             mask=mask,
         ),
+        Column.START_TIME_SECOND_DIFF: np.ma.masked_array(
+            data=convert_sequences_to_array(
+                groups.get_column(Column.START_TIME_SECOND_DIFF).to_list(),
+                max_len=mask.shape[1],
+                dtype=np.float64,
+                padded_value=-1.0,
+            ),
+            mask=mask,
+        ),
         Column.STOP_FRAME: np.ma.masked_array(
             data=convert_sequences_to_array(
                 groups.get_column(Column.STOP_FRAME).to_list(),
                 max_len=mask.shape[1],
                 dtype=np.int64,
                 padded_value=-1,
             ),
```

### Comparing `arctix-0.0.5/src/arctix/dataset/multithumos.py` & `arctix-0.0.6/src/arctix/dataset/multithumos.py`

 * *Files 4% similar despite different names*

```diff
@@ -126,14 +126,15 @@
 
     ACTION: str = "action"
     ACTION_ID: str = "action_id"
     END_TIME: str = "end_time"
     SEQUENCE_LENGTH: str = "sequence_length"
     SPLIT: str = "split"
     START_TIME: str = "start_time"
+    START_TIME_DIFF: str = "start_time_diff"
     VIDEO: str = "video"
     VIDEO_ID: str = "video_id"
 
 
 class MetadataKeys:
     r"""Indicate the metadata keys."""
 
@@ -372,45 +373,50 @@
 
     ```pycon
 
     >>> import polars as pl
     >>> from arctix.dataset.multithumos import Column, prepare_data
     >>> frame = pl.DataFrame(
     ...     {
-    ...         Column.VIDEO: ["video_validation_1", "video_test_2", "video_validation_3", "video_test_4"],
+    ...         Column.VIDEO: ["video_validation_1", "video_test_2", "video_validation_1", "video_test_2"],
     ...         Column.START_TIME: [72.80, 44.00, 1.50, 17.57],
     ...         Column.END_TIME: [76.40, 50.90, 5.40, 18.33],
     ...         Column.ACTION: ["dribble", "dribble", "dribble", "guard"],
     ...     }
     ... )
     >>> data, metadata = prepare_data(frame)
     >>> data
-    shape: (4, 6)
-    ┌─────────┬───────────┬──────────┬────────────┬────────────┬────────────────────┐
-    │ action  ┆ action_id ┆ end_time ┆ split      ┆ start_time ┆ video              │
-    │ ---     ┆ ---       ┆ ---      ┆ ---        ┆ ---        ┆ ---                │
-    │ str     ┆ i64       ┆ f64      ┆ str        ┆ f64        ┆ str                │
-    ╞═════════╪═══════════╪══════════╪════════════╪════════════╪════════════════════╡
-    │ dribble ┆ 0         ┆ 50.9     ┆ test       ┆ 44.0       ┆ video_test_2       │
-    │ guard   ┆ 1         ┆ 18.33    ┆ test       ┆ 17.57      ┆ video_test_4       │
-    │ dribble ┆ 0         ┆ 76.4     ┆ validation ┆ 72.8       ┆ video_validation_1 │
-    │ dribble ┆ 0         ┆ 5.4      ┆ validation ┆ 1.5        ┆ video_validation_3 │
-    └─────────┴───────────┴──────────┴────────────┴────────────┴────────────────────┘
+    shape: (4, 7)
+    ┌─────────┬───────────┬──────────┬────────────┬────────────┬─────────────────┬────────────────────┐
+    │ action  ┆ action_id ┆ end_time ┆ split      ┆ start_time ┆ start_time_diff ┆ video              │
+    │ ---     ┆ ---       ┆ ---      ┆ ---        ┆ ---        ┆ ---             ┆ ---                │
+    │ str     ┆ i64       ┆ f64      ┆ str        ┆ f64        ┆ f64             ┆ str                │
+    ╞═════════╪═══════════╪══════════╪════════════╪════════════╪═════════════════╪════════════════════╡
+    │ guard   ┆ 1         ┆ 18.33    ┆ test       ┆ 17.57      ┆ 0.0             ┆ video_test_2       │
+    │ dribble ┆ 0         ┆ 50.9     ┆ test       ┆ 44.0       ┆ 26.43           ┆ video_test_2       │
+    │ dribble ┆ 0         ┆ 5.4      ┆ validation ┆ 1.5        ┆ 0.0             ┆ video_validation_1 │
+    │ dribble ┆ 0         ┆ 76.4     ┆ validation ┆ 72.8       ┆ 71.3            ┆ video_validation_1 │
+    └─────────┴───────────┴──────────┴────────────┴────────────┴─────────────────┴────────────────────┘
     >>> metadata
     {'vocab_action': Vocabulary(
       counter=Counter({'dribble': 3, 'guard': 1}),
       index_to_token=('dribble', 'guard'),
       token_to_index={'dribble': 0, 'guard': 1},
     )}
 
     ```
     """
     vocab_action = generate_vocabulary(frame, col=Column.ACTION).sort_by_count()
     transformer = td.Sequential(
         [
+            td.TimeDiff(
+                group_cols=[Column.VIDEO],
+                time_col=Column.START_TIME,
+                time_diff_col=Column.START_TIME_DIFF,
+            ),
             td.Sort(columns=[Column.VIDEO, Column.START_TIME]),
             td.Cast(columns=[Column.START_TIME, Column.END_TIME], dtype=pl.Float64),
             td.StripChars(columns=[Column.ACTION, Column.VIDEO]),
             td.TokenToIndex(
                 vocab=vocab_action, token_column=Column.ACTION, index_column=Column.ACTION_ID
             ),
             td.Function(generate_split_column),
@@ -560,14 +566,15 @@
     ...             "video_validation_1",
     ...             "video_validation_2",
     ...             "video_validation_2",
     ...             "video_validation_2",
     ...             "video_validation_2",
     ...         ],
     ...         Column.START_TIME: [1.50, 17.57, 79.30, 2.97, 4.54, 20.22, 27.42],
+    ...         Column.START_TIME_DIFF: [0.0, 16.07, 61.73, 0.0, 1.57, 15.68, 7.20],
     ...         Column.END_TIME: [5.40, 18.33, 83.90, 3.60, 5.07, 20.49, 30.23],
     ...         Column.ACTION: [
     ...             "dribble",
     ...             "guard",
     ...             "dribble",
     ...             "guard",
     ...             "guard",
@@ -584,36 +591,37 @@
     ...             "validation",
     ...             "validation",
     ...         ],
     ...     },
     ... )
     >>> groups = group_by_sequence(frame)
     >>> groups
-    shape: (2, 7)
-    ┌──────────────┬─────────────┬──────────────┬─────────────┬────────────┬─────────────┬─────────────┐
-    │ action       ┆ action_id   ┆ end_time     ┆ sequence_le ┆ split      ┆ start_time  ┆ video       │
-    │ ---          ┆ ---         ┆ ---          ┆ ngth        ┆ ---        ┆ ---         ┆ ---         │
-    │ list[str]    ┆ list[i64]   ┆ list[f64]    ┆ ---         ┆ str        ┆ list[f64]   ┆ str         │
-    │              ┆             ┆              ┆ i64         ┆            ┆             ┆             │
-    ╞══════════════╪═════════════╪══════════════╪═════════════╪════════════╪═════════════╪═════════════╡
-    │ ["dribble",  ┆ [1, 0, 1]   ┆ [5.4, 18.33, ┆ 3           ┆ validation ┆ [1.5,       ┆ video_valid │
-    │ "guard",     ┆             ┆ 83.9]        ┆             ┆            ┆ 17.57,      ┆ ation_1     │
-    │ "dribble"…   ┆             ┆              ┆             ┆            ┆ 79.3]       ┆             │
-    │ ["guard",    ┆ [0, 0, … 2] ┆ [3.6, 5.07,  ┆ 4           ┆ validation ┆ [2.97,      ┆ video_valid │
-    │ "guard", …   ┆             ┆ … 30.23]     ┆             ┆            ┆ 4.54, …     ┆ ation_2     │
-    │ "shoot"]     ┆             ┆              ┆             ┆            ┆ 27.42]      ┆             │
-    └──────────────┴─────────────┴──────────────┴─────────────┴────────────┴─────────────┴─────────────┘
+    shape: (2, 8)
+    ┌────────────┬────────────┬────────────┬───────────┬───────────┬───────────┬───────────┬───────────┐
+    │ action     ┆ action_id  ┆ end_time   ┆ sequence_ ┆ split     ┆ start_tim ┆ start_tim ┆ video     │
+    │ ---        ┆ ---        ┆ ---        ┆ length    ┆ ---       ┆ e         ┆ e_diff    ┆ ---       │
+    │ list[str]  ┆ list[i64]  ┆ list[f64]  ┆ ---       ┆ str       ┆ ---       ┆ ---       ┆ str       │
+    │            ┆            ┆            ┆ i64       ┆           ┆ list[f64] ┆ list[f64] ┆           │
+    ╞════════════╪════════════╪════════════╪═══════════╪═══════════╪═══════════╪═══════════╪═══════════╡
+    │ ["dribble" ┆ [1, 0, 1]  ┆ [5.4,      ┆ 3         ┆ validatio ┆ [1.5,     ┆ [0.0,     ┆ video_val │
+    │ , "guard", ┆            ┆ 18.33,     ┆           ┆ n         ┆ 17.57,    ┆ 16.07,    ┆ idation_1 │
+    │ "dribble"… ┆            ┆ 83.9]      ┆           ┆           ┆ 79.3]     ┆ 61.73]    ┆           │
+    │ ["guard",  ┆ [0, 0, …   ┆ [3.6,      ┆ 4         ┆ validatio ┆ [2.97,    ┆ [0.0,     ┆ video_val │
+    │ "guard", … ┆ 2]         ┆ 5.07, …    ┆           ┆ n         ┆ 4.54, …   ┆ 1.57, …   ┆ idation_2 │
+    │ "shoot"]   ┆            ┆ 30.23]     ┆           ┆           ┆ 27.42]    ┆ 7.2]      ┆           │
+    └────────────┴────────────┴────────────┴───────────┴───────────┴───────────┴───────────┴───────────┘
 
     ```
     """
     data = frame.group_by([Column.VIDEO]).agg(
         pl.first(Column.SPLIT),
         pl.col(Column.ACTION),
         pl.col(Column.ACTION_ID),
         pl.col(Column.START_TIME),
+        pl.col(Column.START_TIME_DIFF),
         pl.col(Column.END_TIME),
         pl.len().cast(pl.Int64).alias(Column.SEQUENCE_LENGTH),
     )
     transformer = td.Sequential(
         [
             td.Sort(columns=[Column.VIDEO]),
             td.SortColumns(),
@@ -645,14 +653,15 @@
     ...             "video_validation_1",
     ...             "video_validation_2",
     ...             "video_validation_2",
     ...             "video_validation_2",
     ...             "video_validation_2",
     ...         ],
     ...         Column.START_TIME: [1.0, 17.0, 79.0, 2.0, 4.0, 20.0, 27.0],
+    ...         Column.START_TIME_DIFF: [0.0, 16.07, 61.73, 0.0, 1.57, 15.68, 7.20],
     ...         Column.END_TIME: [5.0, 18.0, 83.0, 3.0, 5.0, 20.0, 30.0],
     ...         Column.ACTION: [
     ...             "dribble",
     ...             "guard",
     ...             "dribble",
     ...             "guard",
     ...             "guard",
@@ -695,14 +704,20 @@
       'sequence_length': array([3, 4]),
       'split': array(['validation', 'validation'], dtype='<U10'),
       'start_time': masked_array(
       data=[[1.0, 17.0, 79.0, --],
             [2.0, 4.0, 20.0, 27.0]],
       mask=[[False, False, False,  True],
             [False, False, False, False]],
+      fill_value=1e+20),
+      'start_time_diff': masked_array(
+      data=[[0.0, 16.07, 61.73, --],
+            [0.0, 1.57, 15.68, 7.2]],
+      mask=[[False, False, False,  True],
+            [False, False, False, False]],
       fill_value=1e+20)}
 
     ```
     """
     groups = group_by_sequence(frame)
     lengths = groups.get_column(Column.SEQUENCE_LENGTH).to_numpy()
     mask = generate_mask_from_lengths(lengths)
@@ -741,14 +756,23 @@
                 groups.get_column(Column.START_TIME).to_list(),
                 dtype=np.float64,
                 max_len=mask.shape[1],
                 padded_value=-1.0,
             ),
             mask=mask,
         ),
+        Column.START_TIME_DIFF: np.ma.masked_array(
+            data=convert_sequences_to_array(
+                groups.get_column(Column.START_TIME_DIFF).to_list(),
+                dtype=np.float64,
+                max_len=mask.shape[1],
+                padded_value=-1.0,
+            ),
+            mask=mask,
+        ),
     }
 
 
 def to_list(frame: pl.DataFrame) -> dict[str, list]:
     r"""Convert a DataFrame to a dictionary of lists.
 
     Args:
@@ -771,14 +795,15 @@
     ...             "video_validation_1",
     ...             "video_validation_2",
     ...             "video_validation_2",
     ...             "video_validation_2",
     ...             "video_validation_2",
     ...         ],
     ...         Column.START_TIME: [1.0, 17.0, 79.0, 2.0, 4.0, 20.0, 27.0],
+    ...         Column.START_TIME_DIFF: [0.0, 16.07, 61.73, 0.0, 1.57, 15.68, 7.20],
     ...         Column.END_TIME: [5.0, 18.0, 83.0, 3.0, 5.0, 20.0, 30.0],
     ...         Column.ACTION: [
     ...             "dribble",
     ...             "guard",
     ...             "dribble",
     ...             "guard",
     ...             "guard",
@@ -798,16 +823,18 @@
     ...     },
     ... )
     >>> data_list = to_list(frame)
     >>> data_list
     {'action': [['dribble', 'guard', 'dribble'], ['guard', 'guard', 'guard', 'shoot']],
      'action_id': [[1, 0, 1], [0, 0, 0, 2]],
      'end_time': [[5.0, 18.0, 83.0], [3.0, 5.0, 20.0, 30.0]],
-     'sequence_length': [3, 4], 'split': ['validation', 'validation'],
+     'sequence_length': [3, 4],
+     'split': ['validation', 'validation'],
      'start_time': [[1.0, 17.0, 79.0], [2.0, 4.0, 20.0, 27.0]],
+     'start_time_diff': [[0.0, 16.07, 61.73], [0.0, 1.57, 15.68, 7.2]],
      'video': ['video_validation_1', 'video_validation_2']}
 
     ```
     """
     return group_by_sequence(frame).to_dict(as_series=False)
```

### Comparing `arctix-0.0.5/src/arctix/testing/fixtures.py` & `arctix-0.0.6/src/arctix/testing/fixtures.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/transformer/dataframe/__init__.py` & `arctix-0.0.6/src/arctix/transformer/dataframe/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 
 from __future__ import annotations
 
 __all__ = [
     "BaseDataFrameTransformer",
     "Cast",
     "CastDataFrameTransformer",
+    "Diff",
+    "DiffDataFrameTransformer",
     "Function",
     "FunctionDataFrameTransformer",
     "IndexToToken",
     "IndexToTokenDataFrameTransformer",
     "JsonDecode",
     "JsonDecodeDataFrameTransformer",
     "Replace",
@@ -18,14 +20,16 @@
     "SequentialDataFrameTransformer",
     "Sort",
     "SortColumns",
     "SortColumnsDataFrameTransformer",
     "SortDataFrameTransformer",
     "StripChars",
     "StripCharsDataFrameTransformer",
+    "TimeDiff",
+    "TimeDiffDataFrameTransformer",
     "TimeToSecond",
     "TimeToSecondDataFrameTransformer",
     "ToTime",
     "ToTimeDataFrameTransformer",
     "TokenToIndex",
     "TokenToIndexDataFrameTransformer",
     "is_dataframe_transformer_config",
@@ -37,14 +41,18 @@
     is_dataframe_transformer_config,
     setup_dataframe_transformer,
 )
 from arctix.transformer.dataframe.casting import CastDataFrameTransformer
 from arctix.transformer.dataframe.casting import CastDataFrameTransformer as Cast
 from arctix.transformer.dataframe.casting import ToTimeDataFrameTransformer
 from arctix.transformer.dataframe.casting import ToTimeDataFrameTransformer as ToTime
+from arctix.transformer.dataframe.diff import DiffDataFrameTransformer
+from arctix.transformer.dataframe.diff import DiffDataFrameTransformer as Diff
+from arctix.transformer.dataframe.diff import TimeDiffDataFrameTransformer
+from arctix.transformer.dataframe.diff import TimeDiffDataFrameTransformer as TimeDiff
 from arctix.transformer.dataframe.function import FunctionDataFrameTransformer
 from arctix.transformer.dataframe.function import (
     FunctionDataFrameTransformer as Function,
 )
 from arctix.transformer.dataframe.json import JsonDecodeDataFrameTransformer
 from arctix.transformer.dataframe.json import (
     JsonDecodeDataFrameTransformer as JsonDecode,
```

### Comparing `arctix-0.0.5/src/arctix/transformer/dataframe/base.py` & `arctix-0.0.6/src/arctix/transformer/dataframe/base.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/transformer/dataframe/casting.py` & `arctix-0.0.6/src/arctix/transformer/dataframe/casting.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/transformer/dataframe/function.py` & `arctix-0.0.6/src/arctix/transformer/dataframe/function.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/transformer/dataframe/json.py` & `arctix-0.0.6/src/arctix/transformer/dataframe/json.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/transformer/dataframe/replace.py` & `arctix-0.0.6/src/arctix/transformer/dataframe/replace.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/transformer/dataframe/sequential.py` & `arctix-0.0.6/src/arctix/transformer/dataframe/sequential.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/transformer/dataframe/sorting.py` & `arctix-0.0.6/src/arctix/transformer/dataframe/sorting.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/transformer/dataframe/string.py` & `arctix-0.0.6/src/arctix/transformer/dataframe/string.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/transformer/dataframe/time.py` & `arctix-0.0.6/src/arctix/transformer/dataframe/time.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/transformer/dataframe/vocab.py` & `arctix-0.0.6/src/arctix/transformer/dataframe/vocab.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/utils/dataframe/removing.py` & `arctix-0.0.6/src/arctix/utils/dataframe/removing.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/utils/dataframe/vocab.py` & `arctix-0.0.6/src/arctix/utils/dataframe/vocab.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/utils/download.py` & `arctix-0.0.6/src/arctix/utils/download.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/utils/imports.py` & `arctix-0.0.6/src/arctix/utils/imports.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/utils/iter/path.py` & `arctix-0.0.6/src/arctix/utils/iter/path.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/utils/mapping.py` & `arctix-0.0.6/src/arctix/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/utils/masking.py` & `arctix-0.0.6/src/arctix/utils/masking.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/utils/noop.py` & `arctix-0.0.6/src/arctix/utils/noop.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/src/arctix/utils/vocab.py` & `arctix-0.0.6/src/arctix/utils/vocab.py`

 * *Files identical despite different names*

### Comparing `arctix-0.0.5/PKG-INFO` & `arctix-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arctix
-Version: 0.0.5
+Version: 0.0.6
 Summary: 
 Home-page: https://github.com/durandtibo/arctix
 License: BSD-3-Clause
 Keywords: asynchronous time-series,dataset,preprocessing
 Author: Thibaut Durand
 Author-email: durand.tibo+gh@gmail.com
 Requires-Python: >=3.9,<3.13
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: arctix Version: 0.0.5 Summary: Home-page: https://
+Metadata-Version: 2.1 Name: arctix Version: 0.0.6 Summary: Home-page: https://
 github.com/durandtibo/arctix License: BSD-3-Clause Keywords: asynchronous time-
 series,dataset,preprocessing Author: Thibaut Durand Author-email:
 durand.tibo+gh@gmail.com Requires-Python: >=3.9,<3.13 Classifier: Development
 Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers Classifier:
 Intended Audience :: Science/Research Classifier: License :: OSI Approved ::
 BSD License Classifier: Operating System :: POSIX :: Linux Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

