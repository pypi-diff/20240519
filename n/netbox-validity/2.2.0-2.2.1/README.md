# Comparing `tmp/netbox_validity-2.2.0.tar.gz` & `tmp/netbox_validity-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox_validity-2.2.0.tar", last modified: Sun Apr 21 22:23:58 2024, max compression
+gzip compressed data, was "netbox_validity-2.2.1.tar", last modified: Sun May 19 19:10:46 2024, max compression
```

## Comparing `netbox_validity-2.2.0.tar` & `netbox_validity-2.2.1.tar`

### file list

```diff
@@ -1,193 +1,193 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.789053 netbox_validity-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-04-21 22:23:58.789053 netbox_validity-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.789053 netbox_validity-2.2.0/netbox_validity.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-04-21 22:23:58.000000 netbox_validity-2.2.0/netbox_validity.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-04-21 22:23:58.000000 netbox_validity-2.2.0/netbox_validity.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-21 22:23:58.000000 netbox_validity-2.2.0/netbox_validity.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      420 2024-04-21 22:23:58.000000 netbox_validity-2.2.0/netbox_validity.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-21 22:23:58.000000 netbox_validity-2.2.0/netbox_validity.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.765053 netbox_validity-2.2.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (127)      228 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/requirements/base.txt
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (127)       52 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-21 22:23:58.793053 netbox_validity-2.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.769053 netbox_validity-2.2.0/validity/
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/admin.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.769053 netbox_validity-2.2.0/validity/api/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)    12299 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/api/serializers.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/api/urls.py
--rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/api/views.py
--rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.769053 netbox_validity-2.2.0/validity/compliance/
--rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/dynamic_pairs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.769053 netbox_validity-2.2.0/validity/compliance/eval/
--rw-r--r--   0 runner    (1001) docker     (127)      141 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/eval/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/eval/default_nameset.py
--rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/eval/eval.py
--rw-r--r--   0 runner    (1001) docker     (127)      598 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/eval/eval_defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.773053 netbox_validity-2.2.0/validity/compliance/serialization/
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/routeros.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/serializable.py
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/textfsm.py
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/ttp.py
--rw-r--r--   0 runner    (1001) docker     (127)      682 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/xml.py
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/serialization/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/compliance/state.py
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/custom_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     3573 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/data_backends.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.773053 netbox_validity-2.2.0/validity/fields/
--rw-r--r--   0 runner    (1001) docker     (127)       91 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/fields/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/fields/encrypted.py
--rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/filtersets.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.773053 netbox_validity-2.2.0/validity/forms/
--rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/forms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/forms/filterset.py
--rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/forms/general.py
--rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/forms/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/j2_env.py
--rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.773053 netbox_validity-2.2.0/validity/migrations/
--rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0002_custom_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0003_complianceselector_dp_tag_prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)      406 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0004_netbox35_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0005_rename_serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     9900 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0006_datasources.py
--rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0007_polling.py
--rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0008_script_change.py
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/0009_serializer_parameters.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/migrations/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.777053 netbox_validity-2.2.0/validity/models/
--rw-r--r--   0 runner    (1001) docker     (127)      327 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/nameset.py
--rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/polling.py
--rw-r--r--   0 runner    (1001) docker     (127)      559 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/models/test_result.py
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/navigation.py
--rw-r--r--   0 runner    (1001) docker     (127)      611 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/netbox_changes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.777053 netbox_validity-2.2.0/validity/pollers/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3009 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)      485 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/default_credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)      971 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/http.py
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/netconf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/pollers/result.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.777053 netbox_validity-2.2.0/validity/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/scripts/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.777053 netbox_validity-2.2.0/validity/scripts/install/
--rw-r--r--   0 runner    (1001) docker     (127)      168 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/scripts/install/validity_scripts.py
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/scripts/run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/scripts/script_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      350 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/scripts/variables.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.761053 netbox_validity-2.2.0/validity/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.777053 netbox_validity-2.2.0/validity/static/validity/
--rw-r--r--   0 runner    (1001) docker     (127)      798 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/static/validity/connection-type-select.js
--rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/static/validity/prism-dark.css
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/static/validity/prism-light.css
--rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/static/validity/prism.js
--rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/subforms.py
--rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tables.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/template_content.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.761053 netbox_validity-2.2.0/validity/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.781053 netbox_validity-2.2.0/validity/templates/validity/
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/aux_tab_table.html
--rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/command.html
--rw-r--r--   0 runner    (1001) docker     (127)      443 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/compliance_results.html
--rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/compliancereport.html
--rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/complianceselector.html
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/compliancetest.html
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/compliancetestresult.html
--rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/device_state.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.781053 netbox_validity-2.2.0/validity/templates/validity/inc/
--rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/configcontext_format.html
--rw-r--r--   0 runner    (1001) docker     (127)      309 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/datasource_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      546 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/parameters.html
--rw-r--r--   0 runner    (1001) docker     (127)      469 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/path_with_link.html
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/prism.html
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/related_objects.html
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/report_stats_row.html
--rw-r--r--   0 runner    (1001) docker     (127)      227 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/search_form.html
--rw-r--r--   0 runner    (1001) docker     (127)      285 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/inc/yaml_card.html
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/nameset.html
--rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/poller.html
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/poller_edit.html
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/report_devices.html
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templates/validity/serializer.html
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.781053 netbox_validity-2.2.0/validity/templatetags/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/templatetags/validity.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.785053 netbox_validity-2.2.0/validity/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/factories.py
--rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_choices.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.785053 netbox_validity-2.2.0/validity/tests/test_compliance/
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_compliance/test_dynamic_pairs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_compliance/test_eval.py
--rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_compliance/test_serialization.py
--rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_compliance/test_state.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_custom_validators.py
--rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_data_backends.py
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_graphql.py
--rw-r--r--   0 runner    (1001) docker     (127)     2598 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_managers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.785053 netbox_validity-2.2.0/validity/tests/test_models/
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_models/test_clean.py
--rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_models/test_compliancetest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_models/test_git_link.py
--rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_models/test_selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_models/test_vdatasource.py
--rw-r--r--   0 runner    (1001) docker     (127)     2828 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_models/test_vdevice.py
--rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_pollers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.785053 netbox_validity-2.2.0/validity/tests/test_scripts/
--rw-r--r--   0 runner    (1001) docker     (127)      282 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_scripts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_scripts/test_run_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_scripts/test_script_data.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.785053 netbox_validity-2.2.0/validity/tests/test_utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_utils/test_json.py
--rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_utils/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_utils/test_orm.py
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_version.py
--rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/tests/test_views.py
--rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.785053 netbox_validity-2.2.0/validity/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/utils/json.py
--rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/utils/orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-21 22:23:58.789053 netbox_validity-2.2.0/validity/views/
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/command.py
--rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/data_source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/device.py
--rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/nameset.py
--rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/poller.py
--rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/report.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/serializer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-04-21 22:23:46.000000 netbox_validity-2.2.0/validity/views/test_result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.192576 netbox_validity-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-19 19:10:46.188576 netbox_validity-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5183 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.188576 netbox_validity-2.2.1/netbox_validity.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8454 2024-05-19 19:10:46.000000 netbox_validity-2.2.1/netbox_validity.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5565 2024-05-19 19:10:46.000000 netbox_validity-2.2.1/netbox_validity.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:10:46.000000 netbox_validity-2.2.1/netbox_validity.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      420 2024-05-19 19:10:46.000000 netbox_validity-2.2.1/netbox_validity.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-19 19:10:46.000000 netbox_validity-2.2.1/netbox_validity.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2465 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.160576 netbox_validity-2.2.1/requirements/
+-rw-r--r--   0 runner    (1001) docker     (127)      228 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/requirements/base.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       52 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 19:10:46.192576 netbox_validity-2.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.164576 netbox_validity-2.2.1/validity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/admin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.164576 netbox_validity-2.2.1/validity/api/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2952 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12299 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/api/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/api/urls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4164 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/api/views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4709 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.164576 netbox_validity-2.2.1/validity/compliance/
+-rw-r--r--   0 runner    (1001) docker     (127)     2472 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/dynamic_pairs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.168576 netbox_validity-2.2.1/validity/compliance/eval/
+-rw-r--r--   0 runner    (1001) docker     (127)      141 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/eval/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1136 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/eval/default_nameset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3608 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/eval/eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)      598 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/eval/eval_defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.168576 netbox_validity-2.2.1/validity/compliance/serialization/
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5380 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/routeros.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/serializable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/textfsm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/ttp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      682 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/xml.py
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/serialization/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/compliance/state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/custom_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3806 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/data_backends.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.168576 netbox_validity-2.2.1/validity/fields/
+-rw-r--r--   0 runner    (1001) docker     (127)       91 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/fields/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4636 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/fields/encrypted.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5270 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/filtersets.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.168576 netbox_validity-2.2.1/validity/forms/
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/forms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7412 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/forms/filterset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6434 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/forms/general.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4151 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/forms/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3483 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/j2_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10970 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.172576 netbox_validity-2.2.1/validity/migrations/
+-rw-r--r--   0 runner    (1001) docker     (127)    12472 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0002_custom_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0003_complianceselector_dp_tag_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)      406 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0004_netbox35_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1514 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0005_rename_serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9746 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0006_datasources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5988 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0007_polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1790 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0008_script_change.py
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/0009_serializer_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/migrations/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.172576 netbox_validity-2.2.1/validity/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      327 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3330 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4496 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2728 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4958 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/polling.py
+-rw-r--r--   0 runner    (1001) docker     (127)      559 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5138 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3015 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/models/test_result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/navigation.py
+-rw-r--r--   0 runner    (1001) docker     (127)      611 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/netbox_changes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.176576 netbox_validity-2.2.1/validity/pollers/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3183 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/default_credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1280 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2057 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/http.py
+-rw-r--r--   0 runner    (1001) docker     (127)      489 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/netconf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2249 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/pollers/result.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.176576 netbox_validity-2.2.1/validity/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/scripts/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.176576 netbox_validity-2.2.1/validity/scripts/install/
+-rw-r--r--   0 runner    (1001) docker     (127)      168 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/scripts/install/validity_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/scripts/run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3720 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/scripts/script_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      350 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/scripts/variables.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.156576 netbox_validity-2.2.1/validity/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.176576 netbox_validity-2.2.1/validity/static/validity/
+-rw-r--r--   0 runner    (1001) docker     (127)      798 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/static/validity/connection-type-select.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2459 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/static/validity/prism-dark.css
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/static/validity/prism-light.css
+-rw-r--r--   0 runner    (1001) docker     (127)     9622 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/static/validity/prism.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2826 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/subforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10153 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tables.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/template_content.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.156576 netbox_validity-2.2.1/validity/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.180576 netbox_validity-2.2.1/validity/templates/validity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/aux_tab_table.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1454 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/command.html
+-rw-r--r--   0 runner    (1001) docker     (127)      443 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/compliance_results.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2420 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/compliancereport.html
+-rw-r--r--   0 runner    (1001) docker     (127)     3435 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/complianceselector.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/compliancetest.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/compliancetestresult.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2536 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/device_state.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.180576 netbox_validity-2.2.1/validity/templates/validity/inc/
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/configcontext_format.html
+-rw-r--r--   0 runner    (1001) docker     (127)      309 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/datasource_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      546 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/parameters.html
+-rw-r--r--   0 runner    (1001) docker     (127)      469 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/path_with_link.html
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/prism.html
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/related_objects.html
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/report_stats_row.html
+-rw-r--r--   0 runner    (1001) docker     (127)      227 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/search_form.html
+-rw-r--r--   0 runner    (1001) docker     (127)      285 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/inc/yaml_card.html
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/nameset.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2291 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/poller.html
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/poller_edit.html
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/report_devices.html
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templates/validity/serializer.html
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.180576 netbox_validity-2.2.1/validity/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2548 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/templatetags/validity.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.184576 netbox_validity-2.2.1/validity/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3954 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6488 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/factories.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6126 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_choices.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.184576 netbox_validity-2.2.1/validity/tests/test_compliance/
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_compliance/test_dynamic_pairs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4160 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_compliance/test_eval.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5031 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_compliance/test_serialization.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4391 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_compliance/test_state.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_custom_validators.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1525 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_data_backends.py
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2138 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_graphql.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_managers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.184576 netbox_validity-2.2.1/validity/tests/test_models/
+-rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_models/test_clean.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1183 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_models/test_compliancetest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1089 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_models/test_git_link.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2863 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_models/test_selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_models/test_vdatasource.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3393 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_models/test_vdevice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3292 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_pollers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.184576 netbox_validity-2.2.1/validity/tests/test_scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)      282 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_scripts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6795 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_scripts/test_run_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1056 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_scripts/test_script_data.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.184576 netbox_validity-2.2.1/validity/tests/test_utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_utils/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1910 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_utils/test_misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2311 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_utils/test_orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5481 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/tests/test_views.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2848 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.184576 netbox_validity-2.2.1/validity/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     2779 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/utils/json.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2573 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6066 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/utils/orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1043 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:10:46.188576 netbox_validity-2.2.1/validity/views/
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3742 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1120 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1291 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/data_source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1702 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/device.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1124 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/nameset.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1572 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/poller.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4760 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1925 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/serializer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1895 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1951 2024-05-19 19:10:34.000000 netbox_validity-2.2.1/validity/views/test_result.py
```

### Comparing `netbox_validity-2.2.0/LICENSE` & `netbox_validity-2.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/PKG-INFO` & `netbox_validity-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 2.2.0
+Version: 2.2.1
 Summary: NetBox plugin for network devices validation
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netbox-validity Version: 2.2.0 Summary: NetBox
+Metadata-Version: 2.1 Name: netbox-validity Version: 2.2.1 Summary: NetBox
 plugin for network devices validation Author-email: Anton Miasnikov
 gmail.com> License: MIT License Copyright (c) 2023 Anton Miasnikov Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `netbox_validity-2.2.0/README.md` & `netbox_validity-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/netbox_validity.egg-info/PKG-INFO` & `netbox_validity-2.2.1/netbox_validity.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: netbox-validity
-Version: 2.2.0
+Version: 2.2.1
 Summary: NetBox plugin for network devices validation
 Author-email: Anton Miasnikov <anton2008m@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Anton Miasnikov
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: netbox-validity Version: 2.2.0 Summary: NetBox
+Metadata-Version: 2.1 Name: netbox-validity Version: 2.2.1 Summary: NetBox
 plugin for network devices validation Author-email: Anton Miasnikov
 gmail.com> License: MIT License Copyright (c) 2023 Anton Miasnikov Permission
 is hereby granted, free of charge, to any person obtaining a copy of this
 software and associated documentation files (the "Software"), to deal in the
 Software without restriction, including without limitation the rights to use,
 copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the
 Software, and to permit persons to whom the Software is furnished to do so,
```

### Comparing `netbox_validity-2.2.0/netbox_validity.egg-info/SOURCES.txt` & `netbox_validity-2.2.1/netbox_validity.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/pyproject.toml` & `netbox_validity-2.2.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "netbox-validity"
-version = "2.2.0"
+version = "2.2.1"
 description = "NetBox plugin for network devices validation"
 authors = [
     {name = "Anton Miasnikov", email = "anton2008m@gmail.com"},
 ]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
```

### Comparing `netbox_validity-2.2.0/validity/__init__.py` & `netbox_validity-2.2.1/validity/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 
 class NetBoxValidityConfig(PluginConfig):
     name = "validity"
     verbose_name = "Validity"
     description = "Write and run auto tests for network devices"
     author = "Anton Miasnikov"
     author_email = "anton2008m@gmail.com"
-    version = "2.2.0"
+    version = "2.2.1"
     base_url = "validity"
     django_apps = ["bootstrap5"]
     min_version = "3.5.0"
 
     # custom field
     netbox_version = NetboxVersion(VERSION)
 
@@ -34,11 +34,12 @@
 config = NetBoxValidityConfig
 
 
 class ValiditySettings(BaseModel):
     store_last_results: int = Field(default=5, gt=0, lt=1001)
     store_reports: int = Field(default=5, gt=0, lt=1001)
     sleep_between_tests: float = 0
-    result_batch_size: int = 500
+    result_batch_size: int = Field(default=500, ge=1)
+    polling_threads: int = Field(default=500, ge=1)
 
 
 settings = ValiditySettings.model_validate(django_settings.PLUGINS_CONFIG.get("validity", {}))
```

### Comparing `netbox_validity-2.2.0/validity/api/helpers.py` & `netbox_validity-2.2.1/validity/api/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/api/serializers.py` & `netbox_validity-2.2.1/validity/api/serializers.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/api/urls.py` & `netbox_validity-2.2.1/validity/api/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/api/views.py` & `netbox_validity-2.2.1/validity/api/views.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/choices.py` & `netbox_validity-2.2.1/validity/choices.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/compliance/dynamic_pairs.py` & `netbox_validity-2.2.1/validity/compliance/dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/compliance/eval/default_nameset.py` & `netbox_validity-2.2.1/validity/compliance/eval/default_nameset.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/compliance/eval/eval.py` & `netbox_validity-2.2.1/validity/compliance/eval/eval.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/compliance/eval/eval_defaults.py` & `netbox_validity-2.2.1/validity/compliance/eval/eval_defaults.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/compliance/exceptions.py` & `netbox_validity-2.2.1/validity/compliance/exceptions.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/compliance/serialization/backend.py` & `netbox_validity-2.2.1/validity/compliance/serialization/backend.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/compliance/serialization/routeros.py` & `netbox_validity-2.2.1/validity/compliance/serialization/routeros.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/compliance/serialization/serializable.py` & `netbox_validity-2.2.1/validity/compliance/serialization/serializable.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/compliance/serialization/xml.py` & `netbox_validity-2.2.1/validity/compliance/serialization/xml.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/compliance/state.py` & `netbox_validity-2.2.1/validity/compliance/state.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/custom_validators.py` & `netbox_validity-2.2.1/validity/custom_validators.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/data_backends.py` & `netbox_validity-2.2.1/validity/data_backends.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 from tempfile import TemporaryDirectory
 from typing import Generator
 
 import yaml
 from django import forms
 from django.db.models import Q
 from django.utils.translation import gettext_lazy as _
+from netbox.config import ConfigItem
 from netbox.registry import registry
 
 from validity import config
 from validity.models import VDevice
 from .pollers.result import DescriptiveError, PollingInfo
 
 
@@ -32,21 +33,30 @@
     parameters = {
         "datasource_id": forms.IntegerField(
             label=_("Data Source ID"),
             widget=forms.TextInput(attrs={"class": "form-control"}),
         )
     }
 
-    devices_qs = VDevice.objects.prefetch_poller(with_commands=True).annotate_datasource_id().order_by("poller_id")
+    devices_qs = (
+        VDevice.objects.select_related("primary_ip4", "primary_ip6")
+        .prefetch_poller(with_commands=True)
+        .annotate_datasource_id()
+        .order_by("poller_id")
+    )
     metainfo_file = Path("polling_info.yaml")
 
     def bound_devices_qs(self, device_filter: Q):
         datasource_id = self.params.get("datasource_id")
         assert datasource_id, 'Data Source parameters must contain "datasource_id"'
-        return self.devices_qs.filter(data_source_id=datasource_id).filter(device_filter)
+        return (
+            self.devices_qs.filter(data_source_id=datasource_id)
+            .filter(device_filter)
+            .set_attribute("prefer_ipv4", ConfigItem("PREFER_IPV4")())
+        )
 
     def write_metainfo(self, dir_name: str, polling_info: PollingInfo) -> None:
         # NetBox does not provide an opportunity for a backend to return any info/errors to the user
         # Hence, it will be written into "polling_info.yaml" file
         path = dir_name / self.metainfo_file
         path.write_text(yaml.safe_dump(polling_info.model_dump(exclude_defaults=True), sort_keys=False))
```

### Comparing `netbox_validity-2.2.0/validity/fields/encrypted.py` & `netbox_validity-2.2.1/validity/fields/encrypted.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/filtersets.py` & `netbox_validity-2.2.1/validity/filtersets.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/forms/filterset.py` & `netbox_validity-2.2.1/validity/forms/filterset.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/forms/general.py` & `netbox_validity-2.2.1/validity/forms/general.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/forms/helpers.py` & `netbox_validity-2.2.1/validity/forms/helpers.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/graphql.py` & `netbox_validity-2.2.1/validity/graphql.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/managers.py` & `netbox_validity-2.2.1/validity/managers.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/migrations/0001_initial.py` & `netbox_validity-2.2.1/validity/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/migrations/0002_custom_fields.py` & `netbox_validity-2.2.1/validity/migrations/0002_custom_fields.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/migrations/0005_rename_serializer.py` & `netbox_validity-2.2.1/validity/migrations/0005_rename_serializer.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/migrations/0006_datasources.py` & `netbox_validity-2.2.1/validity/migrations/0006_datasources.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from itertools import chain
 from django.db import migrations
 from django.utils.translation import gettext_lazy as _
 from validity.fields.encrypted import EncryptedString
 from django.db import migrations, models
 import django.db.models.deletion
-from validity.utils.misc import datasource_sync
 
 
 def setup_datasource_cf(apps, schema_editor):
     ContentType = apps.get_model("contenttypes", "ContentType")
     CustomField = apps.get_model("extras", "CustomField")
     DataSource = apps.get_model("core", "DataSource")
     Tenant = apps.get_model("tenancy", "Tenant")
@@ -80,41 +79,40 @@
         if field_value := getattr(model, field_name, None):
             mapped_field_name = fields[field_name] if isinstance(fields, dict) else field_name
             result[mapped_field_name] = field_value
     return result
 
 
 def setup_datasources(apps, schema_editor):
-    from core.models import DataSource
+    from validity.models import VDataSource
 
     db = schema_editor.connection.alias
     GitRepo = apps.get_model("validity", "GitRepo")
     datasources = []
     for repo in GitRepo.objects.using(db).all():
         try:
             cf = get_fields(repo, ["web_url", "device_config_path", "default"])
             parameters = get_fields(repo, ["username", "branch", "encrypted_password"])
             if encrypted_password := parameters.pop("encrypted_password", None):
                 parameters["password"] = EncryptedString.deserialize(encrypted_password).decrypt()
-            datasource = DataSource.objects.using(db).create(
+            datasource = VDataSource.objects.using(db).create(
                 type="git",
                 name="validity_" + repo.name,
                 description=f"Auto-created by Validity from Git Repository {repo.name}",
                 source_url=repo.git_url,
                 parameters=parameters,
                 custom_field_data=cf,
             )
             datasources.append(datasource)
         except Exception as e:
             print(
                 f"\nAn error occured while creating Data Source for {repo.name}, skipping...",
                 f"{type(e).__name__}: {e}",
                 sep="\n",
             )  # noqa
-        datasource_sync(datasources, fail_handler=lambda ds, err: print(f"Cannot sync Data Source {ds}:", err))
 
 
 def delete_repo_cf(apps, schema_editor):
     db = schema_editor.connection.alias
     CustomField = apps.get_model("extras", "CustomField")
     CustomField.objects.using(db).filter(name="repo", content_types__model="tenant").delete()
```

### Comparing `netbox_validity-2.2.0/validity/migrations/0007_polling.py` & `netbox_validity-2.2.1/validity/migrations/0007_polling.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/migrations/0008_script_change.py` & `netbox_validity-2.2.1/validity/migrations/0008_script_change.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/models/base.py` & `netbox_validity-2.2.1/validity/models/base.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/models/data.py` & `netbox_validity-2.2.1/validity/models/data.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/models/device.py` & `netbox_validity-2.2.1/validity/models/device.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,14 +13,15 @@
     from .selector import ComplianceSelector
 
 
 class VDevice(Device):
     objects = VDeviceQS.as_manager()
     data_source: VDataSource
     selector: Optional["ComplianceSelector"]
+    prefer_ipv4: bool | None = None
 
     class Meta:
         proxy = True
 
     def _config_item(self) -> Serializable:
         """
         Serializable from  "device_config_path" file
@@ -64,7 +65,20 @@
         if filter_ is None:
             return
         pair = type(self).objects.filter(filter_).first()
         if pair:
             pair.data_source = self.data_source
             pair.poller = self.poller
         return pair
+
+    @property
+    def primary_ip(self):
+        if self.prefer_ipv4 is None:
+            return super().primary_ip
+        if self.prefer_ipv4 and self.primary_ip4:
+            return self.primary_ip4
+        elif self.primary_ip6:
+            return self.primary_ip6
+        elif self.primary_ip4:
+            return self.primary_ip4
+        else:
+            return None
```

### Comparing `netbox_validity-2.2.0/validity/models/nameset.py` & `netbox_validity-2.2.1/validity/models/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/models/polling.py` & `netbox_validity-2.2.1/validity/models/polling.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/models/report.py` & `netbox_validity-2.2.1/validity/models/report.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/models/selector.py` & `netbox_validity-2.2.1/validity/models/selector.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/models/serializer.py` & `netbox_validity-2.2.1/validity/models/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/models/test.py` & `netbox_validity-2.2.1/validity/models/test.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/models/test_result.py` & `netbox_validity-2.2.1/validity/models/test_result.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/navigation.py` & `netbox_validity-2.2.1/validity/navigation.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/netbox_changes.py` & `netbox_validity-2.2.1/validity/netbox_changes.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/pollers/base.py` & `netbox_validity-2.2.1/validity/pollers/base.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,15 +29,17 @@
 
 
 class ThreadPoller(DevicePoller):
     """
     Polls devices one by one using threads
     """
 
-    thread_workers: int = 500
+    def __init__(self, credentials: dict, commands: Collection["Command"], thread_workers: int = 500) -> None:
+        super().__init__(credentials, commands)
+        self.thread_workers = thread_workers
 
     def _poll_one_device(self, device: "VDevice") -> Collection[CommandResult]:
         """
         Handles device-wide errors
         """
         try:
             with reraise(Exception, PollingError):
```

### Comparing `netbox_validity-2.2.0/validity/pollers/default_credentials.py` & `netbox_validity-2.2.1/validity/pollers/default_credentials.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/pollers/factory.py` & `netbox_validity-2.2.1/validity/pollers/factory.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,30 +1,36 @@
+from functools import partial
 from typing import TYPE_CHECKING, Sequence
 
+from validity import settings
 from validity.choices import ConnectionTypeChoices
-from .base import DevicePoller
+from .base import DevicePoller, ThreadPoller
 from .cli import NetmikoPoller
 from .http import RequestsPoller
 from .netconf import ScrapliNetconfPoller
 
 
 if TYPE_CHECKING:
     from validity.models import Command
 
 
 class PollerFactory:
-    def __init__(self, poller_map: dict) -> None:
+    def __init__(self, poller_map: dict, max_threads: int) -> None:
         self.poller_map = poller_map
+        self.max_threads = max_threads
 
     def __call__(self, connection_type: str, credentials: dict, commands: Sequence["Command"]) -> DevicePoller:
         if poller_cls := self.poller_map.get(connection_type):
+            if issubclass(poller_cls, ThreadPoller):
+                poller_cls = partial(poller_cls, thread_workers=self.max_threads)
             return poller_cls(credentials=credentials, commands=commands)
         raise KeyError("No poller exists for this connection type", connection_type)
 
 
 get_poller = PollerFactory(
     poller_map={
         ConnectionTypeChoices.netmiko: NetmikoPoller,
         ConnectionTypeChoices.requests: RequestsPoller,
         ConnectionTypeChoices.scrapli_netconf: ScrapliNetconfPoller,
-    }
+    },
+    max_threads=settings.polling_threads,
 )
```

### Comparing `netbox_validity-2.2.0/validity/pollers/http.py` & `netbox_validity-2.2.1/validity/pollers/http.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/pollers/result.py` & `netbox_validity-2.2.1/validity/pollers/result.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/scripts/run_tests.py` & `netbox_validity-2.2.1/validity/scripts/run_tests.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/scripts/script_data.py` & `netbox_validity-2.2.1/validity/scripts/script_data.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/search.py` & `netbox_validity-2.2.1/validity/search.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/static/validity/connection-type-select.js` & `netbox_validity-2.2.1/validity/static/validity/connection-type-select.js`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/static/validity/prism-dark.css` & `netbox_validity-2.2.1/validity/static/validity/prism-dark.css`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/static/validity/prism-light.css` & `netbox_validity-2.2.1/validity/static/validity/prism-light.css`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/static/validity/prism.js` & `netbox_validity-2.2.1/validity/static/validity/prism.js`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/subforms.py` & `netbox_validity-2.2.1/validity/subforms.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tables.py` & `netbox_validity-2.2.1/validity/tables.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/template_content.py` & `netbox_validity-2.2.1/validity/template_content.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/templates/validity/aux_tab_table.html` & `netbox_validity-2.2.1/validity/templates/validity/aux_tab_table.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/templates/validity/command.html` & `netbox_validity-2.2.1/validity/templates/validity/command.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/templates/validity/compliancereport.html` & `netbox_validity-2.2.1/validity/templates/validity/compliancereport.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/templates/validity/complianceselector.html` & `netbox_validity-2.2.1/validity/templates/validity/complianceselector.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/templates/validity/compliancetest.html` & `netbox_validity-2.2.1/validity/templates/validity/compliancetest.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/templates/validity/compliancetestresult.html` & `netbox_validity-2.2.1/validity/templates/validity/compliancetestresult.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/templates/validity/device_state.html` & `netbox_validity-2.2.1/validity/templates/validity/device_state.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/templates/validity/inc/parameters.html` & `netbox_validity-2.2.1/validity/templates/validity/inc/parameters.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/templates/validity/inc/related_objects.html` & `netbox_validity-2.2.1/validity/templates/validity/inc/related_objects.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/templates/validity/nameset.html` & `netbox_validity-2.2.1/validity/templates/validity/nameset.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/templates/validity/poller.html` & `netbox_validity-2.2.1/validity/templates/validity/poller.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/templates/validity/serializer.html` & `netbox_validity-2.2.1/validity/templates/validity/serializer.html`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/templatetags/validity.py` & `netbox_validity-2.2.1/validity/templatetags/validity.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/base.py` & `netbox_validity-2.2.1/validity/tests/base.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/conftest.py` & `netbox_validity-2.2.1/validity/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/factories.py` & `netbox_validity-2.2.1/validity/tests/factories.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_api.py` & `netbox_validity-2.2.1/validity/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_choices.py` & `netbox_validity-2.2.1/validity/tests/test_choices.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_compliance/test_dynamic_pairs.py` & `netbox_validity-2.2.1/validity/tests/test_compliance/test_dynamic_pairs.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_compliance/test_eval.py` & `netbox_validity-2.2.1/validity/tests/test_compliance/test_eval.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_compliance/test_serialization.py` & `netbox_validity-2.2.1/validity/tests/test_compliance/test_serialization.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_compliance/test_state.py` & `netbox_validity-2.2.1/validity/tests/test_compliance/test_state.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_custom_validators.py` & `netbox_validity-2.2.1/validity/tests/test_custom_validators.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_data_backends.py` & `netbox_validity-2.2.1/validity/tests/test_data_backends.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_fields.py` & `netbox_validity-2.2.1/validity/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_graphql.py` & `netbox_validity-2.2.1/validity/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_managers.py` & `netbox_validity-2.2.1/validity/tests/test_managers.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from itertools import product
 from unittest.mock import Mock
 
 import pytest
 from factories import CommandFactory, CompTestDBFactory, DataSourceFactory, DeviceFactory
 
-from validity.models import Command, ComplianceReport, ComplianceTestResult
+from validity.models import Command, ComplianceReport, ComplianceTestResult, VDevice
 
 
 @pytest.mark.parametrize("store_results", [3, 2, 1])
 @pytest.mark.django_db
 def test_delete_old_results(store_results):
     report = ComplianceReport.objects.create()
     device1 = DeviceFactory()
@@ -51,7 +51,19 @@
     device = DeviceFactory(name="d1")
     ds = DataSourceFactory(
         name="ds1", custom_field_data={"device_command_path": "path/{{device.name}}/{{command.label}}"}
     )
     commands = Command.objects.set_file_paths(device=device, data_source=ds)
     for cmd in commands:
         assert cmd.path == f"path/d1/{cmd.label}"
+
+
+@pytest.mark.django_db
+def test_set_attribute():
+    DeviceFactory(name="d1")
+    DeviceFactory(name="d2")
+    DeviceFactory(name="_d3")
+    device_qs = VDevice.objects.all().set_attribute("attr1", "val1").set_attribute("attr2", "val2")
+    for device in device_qs:
+        assert device.attr1 == "val1" and device.attr2 == "val2"
+    for device in device_qs.filter(name__startswith="d"):
+        assert device.attr1 == "val1" and device.attr2 == "val2"
```

### Comparing `netbox_validity-2.2.0/validity/tests/test_models/test_clean.py` & `netbox_validity-2.2.1/validity/tests/test_models/test_clean.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_models/test_compliancetest.py` & `netbox_validity-2.2.1/validity/tests/test_models/test_compliancetest.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_models/test_git_link.py` & `netbox_validity-2.2.1/validity/tests/test_models/test_git_link.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_models/test_selector.py` & `netbox_validity-2.2.1/validity/tests/test_models/test_selector.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_models/test_vdatasource.py` & `netbox_validity-2.2.1/validity/tests/test_models/test_vdatasource.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_models/test_vdevice.py` & `netbox_validity-2.2.1/validity/tests/test_models/test_vdevice.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 from operator import attrgetter
 
 import pytest
+from dcim.models import Device
 from factories import (
     DataFileFactory,
     DataSourceFactory,
     DeviceFactory,
     SelectorFactory,
     SerializerDBFactory,
     TenantFactory,
 )
+from ipam.models import IPAddress
 
 from validity.compliance.serialization import Serializable
 from validity.models import VDevice
 
 
 @pytest.fixture
 def setup_serializers(create_custom_fields):
@@ -72,7 +74,20 @@
     data_file = DataFileFactory(source=ds, path="path/d1.txt")
     device = DeviceFactory(name="d1")
     device.serializer = SerializerDBFactory()
     device.data_source = ds
     assert device._config_item() == Serializable(device.serializer, data_file)
     device.data_source = None
     assert device._config_item() == Serializable(device.serializer, None)
+
+
+@pytest.mark.django_db
+def test_primary_ip():
+    vdevice = DeviceFactory()
+    device = Device.objects.get(pk=vdevice.pk)
+    vdevice.primary_ip4 = device.primary_ip4 = IPAddress(address="1.1.1.1")
+    vdevice.primary_ip6 = device.primary_ip6 = IPAddress(address="C0CA::BEEF")
+    assert device.primary_ip == vdevice.primary_ip
+    vdevice.prefer_ipv4 = True
+    assert vdevice.primary_ip == vdevice.primary_ip4
+    vdevice.prefer_ipv4 = False
+    assert vdevice.primary_ip == vdevice.primary_ip6
```

### Comparing `netbox_validity-2.2.0/validity/tests/test_pollers.py` & `netbox_validity-2.2.1/validity/tests/test_pollers.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_scripts/test_run_tests.py` & `netbox_validity-2.2.1/validity/tests/test_scripts/test_run_tests.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_scripts/test_script_data.py` & `netbox_validity-2.2.1/validity/tests/test_scripts/test_script_data.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_utils/test_json.py` & `netbox_validity-2.2.1/validity/tests/test_utils/test_json.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_utils/test_misc.py` & `netbox_validity-2.2.1/validity/tests/test_utils/test_misc.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_utils/test_orm.py` & `netbox_validity-2.2.1/validity/tests/test_utils/test_orm.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/tests/test_views.py` & `netbox_validity-2.2.1/validity/tests/test_views.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/urls.py` & `netbox_validity-2.2.1/validity/urls.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/utils/json.py` & `netbox_validity-2.2.1/validity/utils/json.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/utils/misc.py` & `netbox_validity-2.2.1/validity/utils/misc.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/utils/orm.py` & `netbox_validity-2.2.1/validity/utils/orm.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/utils/version.py` & `netbox_validity-2.2.1/validity/utils/version.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/views/__init__.py` & `netbox_validity-2.2.1/validity/views/__init__.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/views/base.py` & `netbox_validity-2.2.1/validity/views/base.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/views/command.py` & `netbox_validity-2.2.1/validity/views/command.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/views/data_source.py` & `netbox_validity-2.2.1/validity/views/data_source.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/views/device.py` & `netbox_validity-2.2.1/validity/views/device.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/views/nameset.py` & `netbox_validity-2.2.1/validity/views/nameset.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/views/poller.py` & `netbox_validity-2.2.1/validity/views/poller.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/views/report.py` & `netbox_validity-2.2.1/validity/views/report.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/views/selector.py` & `netbox_validity-2.2.1/validity/views/selector.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/views/serializer.py` & `netbox_validity-2.2.1/validity/views/serializer.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/views/test.py` & `netbox_validity-2.2.1/validity/views/test.py`

 * *Files identical despite different names*

### Comparing `netbox_validity-2.2.0/validity/views/test_result.py` & `netbox_validity-2.2.1/validity/views/test_result.py`

 * *Files identical despite different names*

