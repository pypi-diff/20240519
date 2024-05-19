# Comparing `tmp/wetlab-0.28.0.tar.gz` & `tmp/wetlab-0.29.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "wetlab-0.28.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "wetlab-0.29.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `wetlab-0.28.0.tar` & `wetlab-0.29.0.tar`

### file list

```diff
@@ -1,39 +1,23 @@
--rw-r--r--   0        0        0     1988 2024-03-08 12:26:27.957200 wetlab-0.28.0/.github/workflows/build.yml
--rw-r--r--   0        0        0      482 2024-03-08 12:26:27.957327 wetlab-0.28.0/.github/workflows/deploy-instance-apis.yml
--rw-r--r--   0        0        0      133 2024-03-08 12:26:27.957503 wetlab-0.28.0/.github/workflows/latest-changes.jinja2
--rw-r--r--   0        0        0      597 2024-03-08 12:26:27.957680 wetlab-0.28.0/.github/workflows/latest-changes.yml
--rw-r--r--   0        0        0     1309 2024-03-08 12:53:13.133702 wetlab-0.28.0/.gitignore
--rw-r--r--   0        0        0     1800 2024-03-08 12:26:27.957903 wetlab-0.28.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       95 2024-03-08 12:53:13.134572 wetlab-0.28.0/README.md
--rw-r--r--   0        0        0     6598 2024-04-25 14:55:02.631764 wetlab-0.28.0/docs/changelog.md
--rw-r--r--   0        0        0     1975 2024-03-08 12:53:13.135290 wetlab-0.28.0/docs/guide/01-get-started.ipynb
--rw-r--r--   0        0        0       65 2024-03-08 12:26:27.958461 wetlab-0.28.0/docs/guide/index.md
--rw-r--r--   0        0        0      122 2024-03-08 12:26:27.958539 wetlab-0.28.0/docs/index.md
--rw-r--r--   0        0        0       54 2024-03-08 12:53:13.135435 wetlab-0.28.0/docs/reference.md
--rw-r--r--   0        0        0      509 2024-03-08 12:26:27.961959 wetlab-0.28.0/noxfile.py
--rw-r--r--   0        0        0      610 2024-03-08 12:53:13.135998 wetlab-0.28.0/pyproject.toml
--rw-r--r--   0        0        0      279 2024-03-08 12:53:13.137380 wetlab-0.28.0/tests/test_integrity.py
--rw-r--r--   0        0        0      401 2024-03-08 12:26:27.962604 wetlab-0.28.0/tests/test_notebooks.py
--rw-r--r--   0        0        0      772 2024-04-25 14:55:06.379561 wetlab-0.28.0/wetlab/__init__.py
--rw-r--r--   0        0        0    12114 2024-03-08 12:53:13.140111 wetlab-0.28.0/wetlab/migrations/0001_initial.py
--rw-r--r--   0        0        0    14581 2024-03-08 12:53:13.140965 wetlab-0.28.0/wetlab/migrations/0001_initial_squashed_0012.py
--rw-r--r--   0        0        0     1176 2024-03-08 12:53:13.141152 wetlab-0.28.0/wetlab/migrations/0002_alter_biosample_options_alter_experiment_options_and_more.py
--rw-r--r--   0        0        0     2325 2024-03-08 12:53:13.141263 wetlab-0.28.0/wetlab/migrations/0003_alter_biosample_created_by_and_more.py
--rw-r--r--   0        0        0     2597 2024-03-08 12:53:13.141657 wetlab-0.28.0/wetlab/migrations/0004_remove_treatment_target_genes_treatmenttarget_and_more.py
--rw-r--r--   0        0        0     1043 2024-03-08 12:53:13.142250 wetlab-0.28.0/wetlab/migrations/0005_alter_treatmenttarget_created_by_and_more.py
--rw-r--r--   0        0        0      562 2024-03-08 12:53:13.142408 wetlab-0.28.0/wetlab/migrations/0006_remove_treatment_target_treatment_targets.py
--rw-r--r--   0        0        0     3001 2024-03-08 12:53:13.142865 wetlab-0.28.0/wetlab/migrations/0007_rename_batch_name_biosample_batch_and_more.py
--rw-r--r--   0        0        0     1231 2024-03-08 12:53:13.143458 wetlab-0.28.0/wetlab/migrations/0008_platewell_delete_well.py
--rw-r--r--   0        0        0      560 2024-03-08 12:53:13.143688 wetlab-0.28.0/wetlab/migrations/0009_alter_platewell_id.py
--rw-r--r--   0        0        0     1980 2024-03-08 12:53:13.144138 wetlab-0.28.0/wetlab/migrations/0010_rename_platewell_well.py
--rw-r--r--   0        0        0     4347 2024-03-08 12:53:13.144343 wetlab-0.28.0/wetlab/migrations/0011_migrate_to_integer_pks.py
--rw-r--r--   0        0        0     1485 2024-04-25 14:12:48.980909 wetlab-0.28.0/wetlab/migrations/0012_export_legacy_data.py
--rw-r--r--   0        0        0     1721 2024-04-25 14:12:48.981143 wetlab-0.28.0/wetlab/migrations/0013_import_legacy_data.py
--rw-r--r--   0        0        0      367 2024-03-08 12:53:13.144699 wetlab-0.28.0/wetlab/migrations/0014_rename_species_biosample_organism.py
--rw-r--r--   0        0        0     1014 2024-03-08 12:53:13.144873 wetlab-0.28.0/wetlab/migrations/0015_rename_files_biosample_artifacts_and_more.py
--rw-r--r--   0        0        0      834 2024-03-08 12:53:13.145223 wetlab-0.28.0/wetlab/migrations/0016_rename_datasets_biosample_collections_and_more.py
--rw-r--r--   0        0        0      578 2024-03-08 12:53:13.145348 wetlab-0.28.0/wetlab/migrations/0017_remove_biosample_artifacts.py
--rw-r--r--   0        0        0     1245 2024-04-25 14:54:41.237054 wetlab-0.28.0/wetlab/migrations/0018_well_created_at_well_created_by_well_updated_at.py
--rw-r--r--   0        0        0        0 2024-03-08 12:53:13.145388 wetlab-0.28.0/wetlab/migrations/__init__.py
--rw-r--r--   0        0        0    10668 2024-04-25 14:54:41.238397 wetlab-0.28.0/wetlab/models.py
--rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 wetlab-0.28.0/PKG-INFO
+-rw-r--r--   0        0        0     1988 2024-05-16 08:59:09.813602 wetlab-0.29.0/.github/workflows/build.yml
+-rw-r--r--   0        0        0      482 2024-05-16 08:59:09.813714 wetlab-0.29.0/.github/workflows/deploy-instance-apis.yml
+-rw-r--r--   0        0        0      133 2024-05-16 08:59:09.813806 wetlab-0.29.0/.github/workflows/latest-changes.jinja2
+-rw-r--r--   0        0        0      597 2024-05-16 08:59:09.813896 wetlab-0.29.0/.github/workflows/latest-changes.yml
+-rw-r--r--   0        0        0     1309 2024-05-16 08:59:09.813993 wetlab-0.29.0/.gitignore
+-rw-r--r--   0        0        0     1800 2024-05-16 08:59:09.814093 wetlab-0.29.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       95 2024-05-16 08:59:09.814228 wetlab-0.29.0/README.md
+-rw-r--r--   0        0        0     6921 2024-05-19 17:02:29.362985 wetlab-0.29.0/docs/changelog.md
+-rw-r--r--   0        0        0     1975 2024-05-16 08:59:09.814594 wetlab-0.29.0/docs/guide/01-get-started.ipynb
+-rw-r--r--   0        0        0       65 2024-05-16 08:59:09.814677 wetlab-0.29.0/docs/guide/index.md
+-rw-r--r--   0        0        0      122 2024-05-16 08:59:09.814761 wetlab-0.29.0/docs/index.md
+-rw-r--r--   0        0        0       54 2024-05-16 08:59:09.814837 wetlab-0.29.0/docs/reference.md
+-rw-r--r--   0        0        0      509 2024-05-16 08:59:09.814925 wetlab-0.29.0/noxfile.py
+-rw-r--r--   0        0        0      610 2024-05-16 08:59:09.815023 wetlab-0.29.0/pyproject.toml
+-rw-r--r--   0        0        0      279 2024-05-16 08:59:09.815173 wetlab-0.29.0/tests/test_integrity.py
+-rw-r--r--   0        0        0      401 2024-05-16 08:59:09.815261 wetlab-0.29.0/tests/test_notebooks.py
+-rw-r--r--   0        0        0      772 2024-05-19 17:01:59.577340 wetlab-0.29.0/wetlab/__init__.py
+-rw-r--r--   0        0        0    13420 2024-05-16 18:54:02.888355 wetlab-0.29.0/wetlab/migrations/0017_remove_biosample_artifacts.py
+-rw-r--r--   0        0        0    14641 2024-05-19 14:53:26.158247 wetlab-0.29.0/wetlab/migrations/0018_squashed.py
+-rw-r--r--   0        0        0     1108 2024-05-16 18:52:52.319326 wetlab-0.29.0/wetlab/migrations/0018_well_created_at_well_created_by_well_updated_at.py
+-rw-r--r--   0        0        0        0 2024-05-16 08:59:09.817223 wetlab-0.29.0/wetlab/migrations/__init__.py
+-rw-r--r--   0        0        0    10668 2024-05-19 14:59:01.833816 wetlab-0.29.0/wetlab/models.py
+-rw-r--r--   0        0        0      607 1970-01-01 00:00:00.000000 wetlab-0.29.0/PKG-INFO
```

### Comparing `wetlab-0.28.0/.github/workflows/build.yml` & `wetlab-0.29.0/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `wetlab-0.28.0/.github/workflows/latest-changes.yml` & `wetlab-0.29.0/.github/workflows/latest-changes.yml`

 * *Files identical despite different names*

### Comparing `wetlab-0.28.0/.gitignore` & `wetlab-0.29.0/.gitignore`

 * *Files identical despite different names*

### Comparing `wetlab-0.28.0/.pre-commit-config.yaml` & `wetlab-0.29.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `wetlab-0.28.0/docs/changelog.md` & `wetlab-0.29.0/docs/changelog.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,14 @@
 # Changelog
 
 <!-- prettier-ignore -->
 Name | PR | Developer | Date | Version
 --- | --- | --- | --- | ---
+🔥 Prune migrations | [51](https://github.com/laminlabs/wetlab/pull/51) | [falexwolf](https://github.com/falexwolf) | 2024-05-16 | 0.28.0
+🔥  Delete old migrations and create a new squashed initial migration | [49](https://github.com/laminlabs/wetlab/pull/49) | [falexwolf](https://github.com/falexwolf) | 2024-05-16 |
 ✨ Updated at for Well | [48](https://github.com/laminlabs/wetlab/pull/48) | [sunnyosun](https://github.com/sunnyosun) | 2024-04-25 |
 🚚 Rename lnschema-lamin1 to wetlab | [47](https://github.com/laminlabs/wetlab/pull/47) | [sunnyosun](https://github.com/sunnyosun) | 2024-03-08 | 0.27.0
 🔥 Temporarily remove a few biosample fields | [45](https://github.com/laminlabs/wetlab/pull/45) | [sunnyosun](https://github.com/sunnyosun) | 2024-02-07 | 0.26.0
 🚚 Rename `Dataset` to `Collection` | [44](https://github.com/laminlabs/wetlab/pull/44) | [falexwolf](https://github.com/falexwolf) | 2024-01-02 | 0.25.0
 🚚 Rename `File` to `Artifact` | [43](https://github.com/laminlabs/wetlab/pull/43) | [falexwolf](https://github.com/falexwolf) | 2023-12-12 | 0.24.0
 📝 Prettify docstrings | [42](https://github.com/laminlabs/wetlab/pull/42) | [falexwolf](https://github.com/falexwolf) | 2023-11-14 |
 ⬆️ Upgrade lamindb | [41](https://github.com/laminlabs/wetlab/pull/41) | [fredericenard](https://github.com/fredericenard) | 2023-11-11 | 0.23.8
```

### Comparing `wetlab-0.28.0/docs/guide/01-get-started.ipynb` & `wetlab-0.29.0/docs/guide/01-get-started.ipynb`

 * *Files identical despite different names*

### Comparing `wetlab-0.28.0/pyproject.toml` & `wetlab-0.29.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `wetlab-0.28.0/wetlab/__init__.py` & `wetlab-0.29.0/wetlab/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,15 +15,15 @@
    Techsample
    Treatment
    TreatmentTarget
    Well
 
 """
 
-__version__ = "0.28.0"
+__version__ = "0.29.0"
 
 from lamindb_setup import _check_instance_setup
 
 
 # trigger instance loading if users
 # want to access attributes
 def __getattr__(name):
```

### Comparing `wetlab-0.28.0/wetlab/migrations/0001_initial.py` & `wetlab-0.29.0/wetlab/migrations/0017_remove_biosample_artifacts.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,297 +1,321 @@
-# Generated by Django 4.2.2 on 2023-06-12 19:01
+# Generated by Django 5.0.6 on 2024-05-16 18:52
 
 import django.db.models.deletion
 import lnschema_core.ids
+import lnschema_core.models
 import lnschema_core.users
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     initial = True
 
     dependencies = [
-        ("lnschema_core", "0001_initial"),
-        ("lnschema_bionty", "0001_initial"),
+        ("lnschema_bionty", "0023_rename_publicsource_encode_uid"),
     ]
 
     operations = [
-        # only necessary for legacy instances
-        # migrations.RunSQL("alter table wetlab_biosample rename to wetlab_legacy_biosample"),
-        # migrations.RunSQL("alter table wetlab_techsample rename to wetlab_legacy_techsample"),
-        # migrations.RunSQL("alter table wetlab_treatment rename to wetlab_legacy_treatment"),
-        # migrations.RunSQL("alter table wetlab_experimenttype rename to wetlab_legacy_experimenttype"),
-        # migrations.RunSQL("alter table wetlab_experiment rename to wetlab_legacy_experiment"),
-        # migrations.RunSQL("alter table wetlab_well rename to wetlab_legacy_well"),
         migrations.CreateModel(
             name="Biosample",
             fields=[
+                ("id", models.AutoField(primary_key=True, serialize=False)),
                 (
-                    "id",
-                    models.CharField(
-                        default=lnschema_core.ids.base62_12,
-                        max_length=12,
-                        primary_key=True,
-                        serialize=False,
-                    ),
+                    "uid",
+                    models.CharField(default=lnschema_core.ids.base62_12, max_length=12, unique=True),
                 ),
                 (
                     "name",
                     models.CharField(db_index=True, default=None, max_length=255, null=True),
                 ),
                 (
-                    "batch_name",
+                    "batch",
                     models.CharField(db_index=True, default=None, max_length=60, null=True),
                 ),
+                ("description", models.TextField(default=None, null=True)),
                 ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
                 ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
                 (
-                    "cell_line",
+                    "cell_lines",
                     models.ManyToManyField(related_name="biosamples", to="lnschema_bionty.cellline"),
                 ),
                 (
-                    "cell_type",
+                    "cell_types",
                     models.ManyToManyField(related_name="biosamples", to="lnschema_bionty.celltype"),
                 ),
                 (
-                    "created_by",
-                    models.ForeignKey(
-                        default=lnschema_core.users.current_user_id,
-                        on_delete=django.db.models.deletion.PROTECT,
-                        related_name="created_storages",
-                        to="lnschema_core.user",
-                    ),
+                    "collections",
+                    models.ManyToManyField(related_name="biosamples", to="lnschema_core.collection"),
                 ),
                 (
-                    "disease",
+                    "diseases",
                     models.ManyToManyField(related_name="biosamples", to="lnschema_bionty.disease"),
                 ),
                 (
-                    "files",
-                    models.ManyToManyField(related_name="biosamples", to="lnschema_core.artifact"),
-                ),
-                (
-                    "species",
-                    models.ForeignKey(
-                        on_delete=django.db.models.deletion.PROTECT,
-                        related_name="biosamples",
-                        to="lnschema_bionty.organism",
-                    ),
-                ),
-                (
-                    "tissue",
+                    "tissues",
                     models.ManyToManyField(related_name="biosamples", to="lnschema_bionty.tissue"),
                 ),
             ],
-            options={},
+            options={
+                "abstract": False,
+            },
+            bases=(models.Model, lnschema_core.models.CanValidate),
         ),
         migrations.CreateModel(
-            name="Treatment",
+            name="ExperimentType",
             fields=[
+                ("id", models.AutoField(primary_key=True, serialize=False)),
                 (
-                    "id",
-                    models.CharField(
-                        default=lnschema_core.ids.base62_12,
-                        max_length=12,
-                        primary_key=True,
-                        serialize=False,
-                    ),
+                    "uid",
+                    models.CharField(default=lnschema_core.ids.base62_4, max_length=4, unique=True),
                 ),
                 ("name", models.CharField(db_index=True, default=None, max_length=255)),
+                ("description", models.TextField(default=None, null=True)),
                 (
-                    "description",
-                    models.CharField(db_index=True, default=None, max_length=255),
-                ),
-                (
-                    "type",
-                    models.CharField(
-                        choices=[("genetic", "genetic"), ("chemical", "chemical")],
-                        db_index=True,
-                        max_length=20,
-                    ),
+                    "ontology_id",
+                    models.CharField(db_index=True, default=None, max_length=32, null=True),
                 ),
+                ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
+                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
                 (
-                    "system",
-                    models.CharField(
-                        choices=[
-                            ("CRISPR Cas9", "CRISPR_Cas9"),
-                            ("CRISPRi", "CRISPRi"),
-                            ("CRISPRa", "CRISPRa"),
-                            ("shRNA", "shRNA"),
-                            ("siRNA", "siRNA"),
-                            ("transgene", "transgene"),
-                            ("transient transfection", "transient_transfection"),
-                        ],
-                        db_index=True,
-                        default=None,
-                        max_length=20,
+                    "created_by",
+                    models.ForeignKey(
+                        default=lnschema_core.users.current_user_id,
+                        on_delete=django.db.models.deletion.PROTECT,
+                        related_name="created_experiment_types",
+                        to="lnschema_core.user",
                     ),
                 ),
+            ],
+            options={
+                "abstract": False,
+            },
+            bases=(models.Model, lnschema_core.models.CanValidate),
+        ),
+        migrations.CreateModel(
+            name="Experiment",
+            fields=[
+                ("id", models.AutoField(primary_key=True, serialize=False)),
                 (
-                    "target",
-                    models.CharField(db_index=True, default=None, max_length=60),
-                ),
-                ("sequence", models.TextField(db_index=True, default=None)),
-                (
-                    "on_target_score",
-                    models.FloatField(db_index=True, default=None, null=True),
-                ),
-                (
-                    "off_target_score",
-                    models.FloatField(db_index=True, default=None, null=True),
+                    "uid",
+                    models.CharField(default=lnschema_core.ids.base62_8, max_length=8, unique=True),
                 ),
+                ("name", models.CharField(db_index=True, default=None, max_length=255)),
+                ("description", models.TextField(default=None, null=True)),
+                ("date", models.DateField(db_index=True, default=None, null=True)),
+                ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
+                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
                 (
-                    "ontology_id",
-                    models.CharField(db_index=True, default=None, max_length=20),
+                    "artifacts",
+                    models.ManyToManyField(related_name="experiments", to="lnschema_core.artifact"),
                 ),
                 (
-                    "pubchem_id",
-                    models.CharField(db_index=True, default=None, max_length=20),
+                    "collections",
+                    models.ManyToManyField(related_name="experiments", to="lnschema_core.collection"),
                 ),
-                ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
-                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
                 (
                     "created_by",
                     models.ForeignKey(
                         default=lnschema_core.users.current_user_id,
                         on_delete=django.db.models.deletion.PROTECT,
-                        related_name="created_storages",
+                        related_name="created_experiments",
                         to="lnschema_core.user",
                     ),
                 ),
                 (
-                    "files",
-                    models.ManyToManyField(related_name="treatments", to="lnschema_core.artifact"),
+                    "experiment_type",
+                    models.ForeignKey(
+                        null=True,
+                        on_delete=django.db.models.deletion.PROTECT,
+                        related_name="experiments",
+                        to="wetlab.experimenttype",
+                    ),
                 ),
             ],
-            options={},
+            options={
+                "abstract": False,
+            },
+            bases=(models.Model, lnschema_core.models.CanValidate),
         ),
         migrations.CreateModel(
             name="Techsample",
             fields=[
+                ("id", models.AutoField(primary_key=True, serialize=False)),
                 (
-                    "id",
-                    models.CharField(
-                        default=lnschema_core.ids.base62_12,
-                        max_length=12,
-                        primary_key=True,
-                        serialize=False,
-                    ),
+                    "uid",
+                    models.CharField(default=lnschema_core.ids.base62_12, max_length=12, unique=True),
                 ),
                 ("name", models.CharField(db_index=True, default=None, max_length=255)),
                 ("batch", models.CharField(db_index=True, default=None, max_length=60)),
+                ("description", models.TextField(default=None, null=True)),
                 ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
                 ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
                 (
                     "biosamples",
                     models.ManyToManyField(related_name="techsamples", to="wetlab.biosample"),
                 ),
                 (
                     "created_by",
                     models.ForeignKey(
                         default=lnschema_core.users.current_user_id,
                         on_delete=django.db.models.deletion.PROTECT,
-                        related_name="created_storages",
+                        related_name="created_techsamples",
                         to="lnschema_core.user",
                     ),
                 ),
             ],
-            options={},
+            options={
+                "abstract": False,
+            },
+            bases=(models.Model, lnschema_core.models.CanValidate),
         ),
         migrations.CreateModel(
-            name="ExperimentType",
+            name="TreatmentTarget",
             fields=[
+                ("id", models.AutoField(primary_key=True, serialize=False)),
                 (
-                    "id",
-                    models.CharField(
-                        default=lnschema_core.ids.base62_4,
-                        max_length=4,
-                        primary_key=True,
-                        serialize=False,
-                    ),
+                    "uid",
+                    models.CharField(default=lnschema_core.ids.base62_8, max_length=8, unique=True),
                 ),
-                ("name", models.CharField(db_index=True, default=None, max_length=255)),
-                ("efo_id", models.CharField(default=None, max_length=30)),
+                ("name", models.CharField(db_index=True, default=None, max_length=60)),
+                ("description", models.TextField(default=None, null=True)),
                 ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
                 ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
                 (
+                    "artifacts",
+                    models.ManyToManyField(related_name="treatment_targets", to="lnschema_core.artifact"),
+                ),
+                (
                     "created_by",
                     models.ForeignKey(
                         default=lnschema_core.users.current_user_id,
                         on_delete=django.db.models.deletion.PROTECT,
-                        related_name="created_experiment_types",
+                        related_name="created_treatment_targets",
                         to="lnschema_core.user",
                     ),
                 ),
+                (
+                    "genes",
+                    models.ManyToManyField(related_name="treatment_targets", to="lnschema_bionty.gene"),
+                ),
             ],
-            options={},
+            options={
+                "abstract": False,
+            },
+            bases=(models.Model, lnschema_core.models.CanValidate),
         ),
         migrations.CreateModel(
-            name="Experiment",
+            name="Treatment",
             fields=[
+                ("id", models.AutoField(primary_key=True, serialize=False)),
+                (
+                    "uid",
+                    models.CharField(default=lnschema_core.ids.base62_12, max_length=12, unique=True),
+                ),
+                ("name", models.CharField(db_index=True, default=None, max_length=255)),
                 (
-                    "id",
+                    "type",
                     models.CharField(
-                        default=lnschema_core.ids.base62_8,
-                        max_length=8,
-                        primary_key=True,
-                        serialize=False,
+                        choices=[("genetic", "genetic"), ("chemical", "chemical")],
+                        db_index=True,
+                        max_length=20,
                     ),
                 ),
-                ("name", models.CharField(db_index=True, default=None, max_length=255)),
-                ("date", models.DateTimeField(db_index=True, default=None, null=True)),
+                (
+                    "system",
+                    models.CharField(
+                        choices=[
+                            ("CRISPR Cas9", "CRISPR_Cas9"),
+                            ("CRISPRi", "CRISPRi"),
+                            ("CRISPRa", "CRISPRa"),
+                            ("shRNA", "shRNA"),
+                            ("siRNA", "siRNA"),
+                            ("transgene", "transgene"),
+                            ("transient transfection", "transient_transfection"),
+                        ],
+                        db_index=True,
+                        default=None,
+                        max_length=20,
+                    ),
+                ),
+                ("description", models.TextField(default=None, null=True)),
+                ("sequence", models.TextField(db_index=True, default=None, null=True)),
+                (
+                    "on_target_score",
+                    models.FloatField(db_index=True, default=None, null=True),
+                ),
+                (
+                    "off_target_score",
+                    models.FloatField(db_index=True, default=None, null=True),
+                ),
+                (
+                    "ontology_id",
+                    models.CharField(db_index=True, default=None, max_length=32, null=True),
+                ),
+                (
+                    "pubchem_id",
+                    models.CharField(db_index=True, default=None, max_length=32, null=True),
+                ),
                 ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
                 ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
                 (
+                    "artifacts",
+                    models.ManyToManyField(related_name="treatments", to="lnschema_core.artifact"),
+                ),
+                (
+                    "collections",
+                    models.ManyToManyField(related_name="treatments", to="lnschema_core.collection"),
+                ),
+                (
                     "created_by",
                     models.ForeignKey(
                         default=lnschema_core.users.current_user_id,
                         on_delete=django.db.models.deletion.PROTECT,
-                        related_name="created_experiments",
+                        related_name="created_treatments",
                         to="lnschema_core.user",
                     ),
                 ),
                 (
-                    "experiment_type",
-                    models.ForeignKey(
-                        on_delete=django.db.models.deletion.PROTECT,
-                        related_name="experiments",
-                        to="wetlab.experimenttype",
-                    ),
-                ),
-                (
-                    "files",
-                    models.ManyToManyField(related_name="experiments", to="lnschema_core.artifact"),
+                    "targets",
+                    models.ManyToManyField(related_name="treatments", to="wetlab.treatmenttarget"),
                 ),
             ],
-            options={},
+            options={
+                "abstract": False,
+            },
+            bases=(models.Model, lnschema_core.models.CanValidate),
         ),
         migrations.CreateModel(
             name="Well",
             fields=[
+                ("id", models.AutoField(primary_key=True, serialize=False)),
                 (
-                    "id",
-                    models.BigAutoField(
-                        auto_created=True,
-                        primary_key=True,
-                        serialize=False,
-                        verbose_name="ID",
+                    "uid",
+                    models.CharField(default=lnschema_core.ids.base62_4, max_length=4, unique=True),
+                ),
+                (
+                    "name",
+                    models.CharField(
+                        db_index=True,
+                        default=None,
+                        max_length=32,
+                        null=True,
+                        unique=True,
                     ),
                 ),
                 ("row", models.CharField(default=None, max_length=4)),
                 ("column", models.IntegerField()),
                 (
-                    "files",
+                    "artifacts",
                     models.ManyToManyField(related_name="wells", to="lnschema_core.artifact"),
                 ),
+                (
+                    "collections",
+                    models.ManyToManyField(related_name="wells", to="lnschema_core.collection"),
+                ),
             ],
             options={
                 "unique_together": {("row", "column")},
             },
+            bases=(models.Model, lnschema_core.models.CanValidate),
         ),
-        migrations.AlterModelOptions(name="biosample", options={"managed": True}),
-        migrations.AlterModelOptions(name="experiment", options={"managed": True}),
-        migrations.AlterModelOptions(name="experimenttype", options={"managed": True}),
-        migrations.AlterModelOptions(name="techsample", options={"managed": True}),
-        migrations.AlterModelOptions(name="treatment", options={"managed": True}),
-        migrations.AlterModelOptions(name="well", options={"managed": True}),
     ]
```

### Comparing `wetlab-0.28.0/wetlab/migrations/0001_initial_squashed_0012.py` & `wetlab-0.29.0/wetlab/migrations/0018_squashed.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,46 +1,45 @@
-# Generated by Django 4.2.5 on 2023-10-12 11:19
+# Generated by Django 5.0.6 on 2024-05-16 09:02
 
+import django.db.migrations.operations.special
 import django.db.models.deletion
+import django.utils.timezone
 import lnschema_core.ids
 import lnschema_core.users
 from django.db import migrations, models
 
+# Functions from the following migrations need manual copying.
+# Move them and any dependencies into this file, then update the
+# RunPython operations to refer to the local versions:
+# wetlab.migrations.0013_
+
 
 class Migration(migrations.Migration):
     replaces = [
-        ("wetlab", "0001_initial"),
-        ("wetlab", "0002_alter_biosample_options_alter_experiment_options_and_more"),
-        ("wetlab", "0003_alter_biosample_created_by_and_more"),
-        ("wetlab", "0004_remove_treatment_target_genes_treatmenttarget_and_more"),
-        ("wetlab", "0005_alter_treatmenttarget_created_by_and_more"),
-        ("wetlab", "0006_remove_treatment_target_treatment_targets"),
-        ("wetlab", "0007_rename_batch_name_biosample_batch_and_more"),
-        ("wetlab", "0008_platewell_delete_well"),
-        ("wetlab", "0009_alter_platewell_id"),
-        ("wetlab", "0010_rename_platewell_well"),
-        ("wetlab", "0011_migrate_to_integer_pks"),
-        ("wetlab", "0012_export_legacy_data"),
+        ("wetlab", "0001_initial_squashed_0012"),
+        ("wetlab", "0013_import_legacy_data"),
+        ("wetlab", "0014_rename_species_biosample_organism"),
+        ("wetlab", "0015_rename_files_biosample_artifacts_and_more"),
+        ("wetlab", "0016_rename_datasets_biosample_collections_and_more"),
+        ("wetlab", "0017_remove_biosample_artifacts"),
+        ("wetlab", "0018_well_created_at_well_created_by_well_updated_at"),
     ]
 
     dependencies = [
-        ("lnschema_core", "0023_export_legacy_data"),
-        ("lnschema_bionty", "0016_export_legacy_data"),
+        ("lnschema_bionty", "0028_squashed"),
     ]
 
-    operations = []  # type: ignore
-
     operations = [
         migrations.CreateModel(
             name="Biosample",
             fields=[
                 ("id", models.AutoField(primary_key=True, serialize=False)),
                 (
                     "uid",
-                    models.CharField(unique=True, default=lnschema_core.ids.base62_12, max_length=12),
+                    models.CharField(default=lnschema_core.ids.base62_12, max_length=12, unique=True),
                 ),
                 (
                     "name",
                     models.CharField(db_index=True, default=None, max_length=255, null=True),
                 ),
                 (
                     "batch",
@@ -54,173 +53,114 @@
                     models.ManyToManyField(related_name="biosamples", to="lnschema_bionty.cellline"),
                 ),
                 (
                     "cell_types",
                     models.ManyToManyField(related_name="biosamples", to="lnschema_bionty.celltype"),
                 ),
                 (
-                    "created_by",
-                    models.ForeignKey(
-                        default=lnschema_core.users.current_user_id,
-                        on_delete=django.db.models.deletion.PROTECT,
-                        related_name="created_biosamples",
-                        to="lnschema_core.user",
-                    ),
-                ),
-                (
-                    "datasets",
+                    "collections",
                     models.ManyToManyField(related_name="biosamples", to="lnschema_core.collection"),
                 ),
                 (
                     "diseases",
                     models.ManyToManyField(related_name="biosamples", to="lnschema_bionty.disease"),
                 ),
                 (
-                    "files",
-                    models.ManyToManyField(related_name="biosamples", to="lnschema_core.artifact"),
-                ),
-                (
-                    "species",
-                    models.ForeignKey(
-                        null=True,
-                        on_delete=django.db.models.deletion.PROTECT,
-                        related_name="biosamples",
-                        to="lnschema_bionty.organism",
-                    ),
-                ),
-                (
                     "tissues",
                     models.ManyToManyField(related_name="biosamples", to="lnschema_bionty.tissue"),
                 ),
             ],
             options={
                 "abstract": False,
             },
+            bases=(models.Model, lnschema_core.models.CanValidate),
         ),
         migrations.CreateModel(
-            name="TreatmentTarget",
+            name="ExperimentType",
             fields=[
                 ("id", models.AutoField(primary_key=True, serialize=False)),
                 (
                     "uid",
-                    models.CharField(unique=True, default=lnschema_core.ids.base62_8, max_length=8),
+                    models.CharField(default=lnschema_core.ids.base62_4, max_length=4, unique=True),
                 ),
-                ("name", models.CharField(db_index=True, default=None, max_length=60)),
+                ("name", models.CharField(db_index=True, default=None, max_length=255)),
                 ("description", models.TextField(default=None, null=True)),
+                (
+                    "ontology_id",
+                    models.CharField(db_index=True, default=None, max_length=32, null=True),
+                ),
                 ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
                 ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
                 (
                     "created_by",
                     models.ForeignKey(
                         default=lnschema_core.users.current_user_id,
                         on_delete=django.db.models.deletion.PROTECT,
-                        related_name="created_treatment_targets",
+                        related_name="created_experiment_types",
                         to="lnschema_core.user",
                     ),
                 ),
-                (
-                    "files",
-                    models.ManyToManyField(related_name="treatment_targets", to="lnschema_core.artifact"),
-                ),
-                (
-                    "genes",
-                    models.ManyToManyField(related_name="treatment_targets", to="lnschema_bionty.gene"),
-                ),
             ],
             options={
                 "abstract": False,
             },
+            bases=(models.Model, lnschema_core.models.CanValidate),
         ),
         migrations.CreateModel(
-            name="Treatment",
+            name="Experiment",
             fields=[
                 ("id", models.AutoField(primary_key=True, serialize=False)),
                 (
                     "uid",
-                    models.CharField(unique=True, default=lnschema_core.ids.base62_12, max_length=12),
+                    models.CharField(default=lnschema_core.ids.base62_8, max_length=8, unique=True),
                 ),
                 ("name", models.CharField(db_index=True, default=None, max_length=255)),
-                (
-                    "type",
-                    models.CharField(
-                        choices=[("genetic", "genetic"), ("chemical", "chemical")],
-                        db_index=True,
-                        max_length=20,
-                    ),
-                ),
-                (
-                    "system",
-                    models.CharField(
-                        choices=[
-                            ("CRISPR Cas9", "CRISPR_Cas9"),
-                            ("CRISPRi", "CRISPRi"),
-                            ("CRISPRa", "CRISPRa"),
-                            ("shRNA", "shRNA"),
-                            ("siRNA", "siRNA"),
-                            ("transgene", "transgene"),
-                            ("transient transfection", "transient_transfection"),
-                        ],
-                        db_index=True,
-                        default=None,
-                        max_length=20,
-                    ),
-                ),
                 ("description", models.TextField(default=None, null=True)),
-                ("sequence", models.TextField(db_index=True, default=None, null=True)),
-                (
-                    "on_target_score",
-                    models.FloatField(db_index=True, default=None, null=True),
-                ),
-                (
-                    "off_target_score",
-                    models.FloatField(db_index=True, default=None, null=True),
-                ),
+                ("date", models.DateField(db_index=True, default=None, null=True)),
+                ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
+                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
                 (
-                    "ontology_id",
-                    models.CharField(db_index=True, default=None, max_length=32, null=True),
+                    "artifacts",
+                    models.ManyToManyField(related_name="experiments", to="lnschema_core.artifact"),
                 ),
                 (
-                    "pubchem_id",
-                    models.CharField(db_index=True, default=None, max_length=32, null=True),
+                    "collections",
+                    models.ManyToManyField(related_name="experiments", to="lnschema_core.collection"),
                 ),
-                ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
-                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
                 (
                     "created_by",
                     models.ForeignKey(
                         default=lnschema_core.users.current_user_id,
                         on_delete=django.db.models.deletion.PROTECT,
-                        related_name="created_treatments",
+                        related_name="created_experiments",
                         to="lnschema_core.user",
                     ),
                 ),
                 (
-                    "datasets",
-                    models.ManyToManyField(related_name="treatments", to="lnschema_core.collection"),
-                ),
-                (
-                    "files",
-                    models.ManyToManyField(related_name="treatments", to="lnschema_core.artifact"),
-                ),
-                (
-                    "targets",
-                    models.ManyToManyField(related_name="treatments", to="wetlab.treatmenttarget"),
+                    "experiment_type",
+                    models.ForeignKey(
+                        null=True,
+                        on_delete=django.db.models.deletion.PROTECT,
+                        related_name="experiments",
+                        to="wetlab.experimenttype",
+                    ),
                 ),
             ],
             options={
                 "abstract": False,
             },
+            bases=(models.Model, lnschema_core.models.CanValidate),
         ),
         migrations.CreateModel(
             name="Techsample",
             fields=[
                 ("id", models.AutoField(primary_key=True, serialize=False)),
                 (
                     "uid",
-                    models.CharField(unique=True, default=lnschema_core.ids.base62_12, max_length=12),
+                    models.CharField(default=lnschema_core.ids.base62_12, max_length=12, unique=True),
                 ),
                 ("name", models.CharField(db_index=True, default=None, max_length=255)),
                 ("batch", models.CharField(db_index=True, default=None, max_length=60)),
                 ("description", models.TextField(default=None, null=True)),
                 ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
                 ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
                 (
@@ -236,116 +176,171 @@
                         to="lnschema_core.user",
                     ),
                 ),
             ],
             options={
                 "abstract": False,
             },
+            bases=(models.Model, lnschema_core.models.CanValidate),
         ),
         migrations.CreateModel(
-            name="ExperimentType",
+            name="TreatmentTarget",
             fields=[
                 ("id", models.AutoField(primary_key=True, serialize=False)),
                 (
                     "uid",
-                    models.CharField(default=lnschema_core.ids.base62_4, max_length=4, unique=True),
+                    models.CharField(default=lnschema_core.ids.base62_8, max_length=8, unique=True),
                 ),
-                ("name", models.CharField(db_index=True, default=None, max_length=255)),
+                ("name", models.CharField(db_index=True, default=None, max_length=60)),
                 ("description", models.TextField(default=None, null=True)),
-                (
-                    "ontology_id",
-                    models.CharField(db_index=True, default=None, max_length=32, null=True),
-                ),
                 ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
                 ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
                 (
+                    "artifacts",
+                    models.ManyToManyField(related_name="treatment_targets", to="lnschema_core.artifact"),
+                ),
+                (
                     "created_by",
                     models.ForeignKey(
                         default=lnschema_core.users.current_user_id,
                         on_delete=django.db.models.deletion.PROTECT,
-                        related_name="created_experiment_types",
+                        related_name="created_treatment_targets",
                         to="lnschema_core.user",
                     ),
                 ),
+                (
+                    "genes",
+                    models.ManyToManyField(related_name="treatment_targets", to="lnschema_bionty.gene"),
+                ),
             ],
             options={
                 "abstract": False,
             },
+            bases=(models.Model, lnschema_core.models.CanValidate),
         ),
         migrations.CreateModel(
-            name="Experiment",
+            name="Treatment",
             fields=[
                 ("id", models.AutoField(primary_key=True, serialize=False)),
                 (
                     "uid",
-                    models.CharField(unique=True, default=lnschema_core.ids.base62_8, max_length=8),
+                    models.CharField(default=lnschema_core.ids.base62_12, max_length=12, unique=True),
                 ),
                 ("name", models.CharField(db_index=True, default=None, max_length=255)),
+                (
+                    "type",
+                    models.CharField(
+                        choices=[("genetic", "genetic"), ("chemical", "chemical")],
+                        db_index=True,
+                        max_length=20,
+                    ),
+                ),
+                (
+                    "system",
+                    models.CharField(
+                        choices=[
+                            ("CRISPR Cas9", "CRISPR_Cas9"),
+                            ("CRISPRi", "CRISPRi"),
+                            ("CRISPRa", "CRISPRa"),
+                            ("shRNA", "shRNA"),
+                            ("siRNA", "siRNA"),
+                            ("transgene", "transgene"),
+                            ("transient transfection", "transient_transfection"),
+                        ],
+                        db_index=True,
+                        default=None,
+                        max_length=20,
+                    ),
+                ),
                 ("description", models.TextField(default=None, null=True)),
-                ("date", models.DateField(db_index=True, default=None, null=True)),
+                ("sequence", models.TextField(db_index=True, default=None, null=True)),
+                (
+                    "on_target_score",
+                    models.FloatField(db_index=True, default=None, null=True),
+                ),
+                (
+                    "off_target_score",
+                    models.FloatField(db_index=True, default=None, null=True),
+                ),
+                (
+                    "ontology_id",
+                    models.CharField(db_index=True, default=None, max_length=32, null=True),
+                ),
+                (
+                    "pubchem_id",
+                    models.CharField(db_index=True, default=None, max_length=32, null=True),
+                ),
                 ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
                 ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
                 (
-                    "created_by",
-                    models.ForeignKey(
-                        default=lnschema_core.users.current_user_id,
-                        on_delete=django.db.models.deletion.PROTECT,
-                        related_name="created_experiments",
-                        to="lnschema_core.user",
-                    ),
+                    "artifacts",
+                    models.ManyToManyField(related_name="treatments", to="lnschema_core.artifact"),
                 ),
                 (
-                    "datasets",
-                    models.ManyToManyField(related_name="experiments", to="lnschema_core.collection"),
+                    "collections",
+                    models.ManyToManyField(related_name="treatments", to="lnschema_core.collection"),
                 ),
                 (
-                    "experiment_type",
+                    "created_by",
                     models.ForeignKey(
-                        null=True,
+                        default=lnschema_core.users.current_user_id,
                         on_delete=django.db.models.deletion.PROTECT,
-                        related_name="experiments",
-                        to="wetlab.experimenttype",
+                        related_name="created_treatments",
+                        to="lnschema_core.user",
                     ),
                 ),
                 (
-                    "files",
-                    models.ManyToManyField(related_name="experiments", to="lnschema_core.artifact"),
+                    "targets",
+                    models.ManyToManyField(related_name="treatments", to="wetlab.treatmenttarget"),
                 ),
             ],
             options={
                 "abstract": False,
             },
+            bases=(models.Model, lnschema_core.models.CanValidate),
         ),
         migrations.CreateModel(
             name="Well",
             fields=[
                 ("id", models.AutoField(primary_key=True, serialize=False)),
                 (
                     "uid",
-                    models.CharField(unique=True, default=lnschema_core.ids.base62_4, max_length=4),
+                    models.CharField(default=lnschema_core.ids.base62_4, max_length=4, unique=True),
                 ),
                 (
                     "name",
                     models.CharField(
                         db_index=True,
                         default=None,
                         max_length=32,
                         null=True,
                         unique=True,
                     ),
                 ),
                 ("row", models.CharField(default=None, max_length=4)),
                 ("column", models.IntegerField()),
+                ("created_at", models.DateTimeField(auto_now_add=True, db_index=True)),
+                ("updated_at", models.DateTimeField(auto_now=True, db_index=True)),
+                (
+                    "artifacts",
+                    models.ManyToManyField(related_name="wells", to="lnschema_core.artifact"),
+                ),
                 (
-                    "datasets",
+                    "collections",
                     models.ManyToManyField(related_name="wells", to="lnschema_core.collection"),
                 ),
                 (
-                    "files",
-                    models.ManyToManyField(related_name="wells", to="lnschema_core.artifact"),
+                    "created_by",
+                    models.ForeignKey(
+                        default=lnschema_core.users.current_user_id,
+                        on_delete=django.db.models.deletion.PROTECT,
+                        related_name="created_wells",
+                        to="lnschema_core.user",
+                    ),
                 ),
             ],
             options={
                 "unique_together": {("row", "column")},
             },
+            bases=(models.Model, lnschema_core.models.CanValidate),
         ),
     ]
```

### Comparing `wetlab-0.28.0/wetlab/migrations/0003_alter_biosample_created_by_and_more.py` & `wetlab-0.29.0/wetlab/migrations/0018_well_created_at_well_created_by_well_updated_at.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,68 +1,36 @@
-# Generated by Django 4.2.1 on 2023-07-03 14:17
+# Generated by Django 5.1 on 2024-04-25 14:41
 
 import django.db.models.deletion
+import django.utils.timezone
 import lnschema_core.users
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
     dependencies = [
-        ("lnschema_core", "0007_feature_synonyms_featureset_field_and_more"),
-        (
-            "wetlab",
-            "0002_alter_biosample_options_alter_experiment_options_and_more",
-        ),
+        ("wetlab", "0017_remove_biosample_artifacts"),
     ]
 
     operations = [
-        migrations.AlterField(
-            model_name="biosample",
-            name="created_by",
-            field=models.ForeignKey(
-                default=lnschema_core.users.current_user_id,
-                on_delete=django.db.models.deletion.PROTECT,
-                related_name="created_biosamples",
-                to="lnschema_core.user",
-            ),
+        migrations.AddField(
+            model_name="well",
+            name="created_at",
+            field=models.DateTimeField(auto_now_add=True, db_index=True, default=django.utils.timezone.now),
+            preserve_default=False,
         ),
-        migrations.AlterField(
-            model_name="techsample",
+        migrations.AddField(
+            model_name="well",
             name="created_by",
             field=models.ForeignKey(
                 default=lnschema_core.users.current_user_id,
                 on_delete=django.db.models.deletion.PROTECT,
-                related_name="created_techsamples",
+                related_name="created_wells",
                 to="lnschema_core.user",
             ),
         ),
-        migrations.AlterField(
-            model_name="treatment",
-            name="created_by",
-            field=models.ForeignKey(
-                default=lnschema_core.users.current_user_id,
-                on_delete=django.db.models.deletion.PROTECT,
-                related_name="created_treatments",
-                to="lnschema_core.user",
-            ),
-        ),
-        migrations.AlterField(
-            model_name="treatment",
-            name="description",
-            field=models.TextField(default=None, null=True),
-        ),
-        migrations.AlterField(
-            model_name="treatment",
-            name="ontology_id",
-            field=models.CharField(db_index=True, default=None, max_length=32, null=True),
-        ),
-        migrations.AlterField(
-            model_name="treatment",
-            name="pubchem_id",
-            field=models.CharField(db_index=True, default=None, max_length=32, null=True),
-        ),
-        migrations.AlterField(
-            model_name="treatment",
-            name="sequence",
-            field=models.TextField(db_index=True, default=None, null=True),
+        migrations.AddField(
+            model_name="well",
+            name="updated_at",
+            field=models.DateTimeField(auto_now=True, db_index=True),
         ),
     ]
```

### Comparing `wetlab-0.28.0/wetlab/models.py` & `wetlab-0.29.0/wetlab/models.py`

 * *Files identical despite different names*

### Comparing `wetlab-0.28.0/PKG-INFO` & `wetlab-0.29.0/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: wetlab
-Version: 0.28.0
+Version: 0.29.0
 Summary: Lamin's default `wetlab` lab schema.
 Author-email: Lamin Labs <laminlabs@gmail.com>
 Description-Content-Type: text/markdown
 Requires-Dist: lamindb[bionty]
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: nox ; extra == "dev"
 Requires-Dist: pytest>=6.0 ; extra == "dev"
```

