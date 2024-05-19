# Comparing `tmp/woningwaardering-0.2.0a1.tar.gz` & `tmp/woningwaardering-0.2.14a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woningwaardering-0.2.0a1.tar", last modified: Thu May 16 13:57:38 2024, max compression
+gzip compressed data, was "woningwaardering-0.2.14a0.tar", last modified: Sun May 19 19:31:34 2024, max compression
```

## Comparing `woningwaardering-0.2.0a1.tar` & `woningwaardering-0.2.14a0.tar`

### file list

```diff
@@ -1,451 +1,451 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.682373 woningwaardering-0.2.0a1/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.618373 woningwaardering-0.2.0a1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24170 2024-05-16 13:57:38.682373 woningwaardering-0.2.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22339 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.618373 woningwaardering-0.2.0a1/docs/afbeeldingen/
--rw-r--r--   0 runner    (1001) docker     (127)    34043 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/docs/afbeeldingen/excel_viewer.png
--rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw
--rw-r--r--   0 runner    (1001) docker     (127)   132221 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/docs/afbeeldingen/oppervlakte_van_vertrekken.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/docs/implementatietoelichting-beleidsboeken/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.618373 woningwaardering-0.2.0a1/docs/implementatietoelichting-beleidsboeken/2024/
--rw-r--r--   0 runner    (1001) docker     (127)    33544 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.622372 woningwaardering-0.2.0a1/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/scripts/genereer_opzet_woningwaarderinggroep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/scripts/genereer_test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/scripts/genereer_vera_referentiedata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/scripts/uitbreiden_vera_modellen.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:57:38.682373 woningwaardering-0.2.0a1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/taskfile.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.622372 woningwaardering-0.2.0a1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/tests/data/input/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.622372 woningwaardering-0.2.0a1/tests/data/input/generiek/
--rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/generiek/37101000032.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.626373 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/
--rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/12006000004.json
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/12006000004.md
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/23003000050.json
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/23003000050.md
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/25048000007.json
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/25048000007.md
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/28018000044.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/28018000044.md
--rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/37101000032.json
--rw-r--r--   0 runner    (1001) docker     (127)    14864 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41027000003.json
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41027000003.md
--rw-r--r--   0 runner    (1001) docker     (127)    16792 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41123000005.json
--rw-r--r--   0 runner    (1001) docker     (127)    17301 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41162000015.json
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41162000015.md
--rw-r--r--   0 runner    (1001) docker     (127)    12899 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41164000002.json
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/51011000042.json
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/51011000042.md
--rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/71211000027.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/71211000027.md
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/77795000000.json
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/81020000003.json
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/81020000003.md
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/81065000089.json
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/81065000089.md
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/85651000021.json
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/85651000021.md
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/87402000003.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/87402000003.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/tests/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json
--rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json
--rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json
--rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json
--rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json
--rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json
--rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json
--rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json
--rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json
--rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json
--rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/config/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/config/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/stelsel/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/stelselgroep/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/test_ZelfstandigeWoonruimten.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/utils/test_import_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/utils/test_is_geldig.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/utils/test_vind_yaml_bestanden.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.json
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.md
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.md
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_A++++_egw.json
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_egw.json
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_mgw.json
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/test_Energieprestatie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.634373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.634373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.634373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/gedeelde_berging.md
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.md
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.md
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.634373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.634373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten_individueel.md
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.md
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten_individueel.md
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.634373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.638373 woningwaardering-0.2.0a1/wettelijke-documenten/
--rw-r--r--   0 runner    (1001) docker     (127)   116885 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.638373 woningwaardering-0.2.0a1/woningwaardering/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-16 13:57:38.000000 woningwaardering-0.2.0a1/woningwaardering/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.638373 woningwaardering-0.2.0a1/woningwaardering/stelsels/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.638373 woningwaardering-0.2.0a1/woningwaardering/stelsels/config/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/stelsel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/stelselgroep.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/stelselgroepversie.py
--rw-r--r--   0 runner    (1001) docker     (127)     8737 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.638373 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/
--rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.638373 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py
--rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/bouwjaar_punten.csv
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_0-25m2_energielabel_punten.csv
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_25-40m2_energielabel_punten.csv
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_40m2+_energielabel_punten.csv
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oud_energielabel_punten.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py
--rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py
--rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/woningwaardering/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelselgroep/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelselgroep/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/vera/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   137423 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/generated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.646373 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/model_uitbreidingen/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_energieprestatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/model_uitbreidingen/referentiedata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/
--rw-r--r--   0 runner    (1001) docker     (127)    15108 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aanbiedingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/accountstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/adressoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afletterstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afrekenwijzesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afspraakstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afwezigheidsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aktesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/authentiekgegevenbron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/authentiekgegevensoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bedrijfsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/begrotingversie.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bestemming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betaalgegevensoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betaalwijzesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betalingsregelingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekingdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekjaarstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    27844 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/brandwerendheidscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/btw.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/btwaangiftestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/burgerlijkestaat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/clustersoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/collectiefobjectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/communicatiekanaal.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/communicatierichting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/conditiescore.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevensoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevenstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/crediteursoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/crediteurstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/dagdeel.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/debiteursoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/debiteurstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectlocatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectoorzaak.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/doelgroep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/dossier/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/dossier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheiddetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheiddetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidinterieur.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidisolatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidligging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidmonument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidprijsconditie.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidsanitair.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eindedetailreden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eindereden.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energie/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energielabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energieprestatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energieprestatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/externeincassosoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/externeincassostatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/factuurbetaalwijze.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/factuursoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/financien/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/financien/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/gebeurtenissoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/geometriesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/geslacht.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huurgeschilsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huurgeschilstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huurklasse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huuropzeggingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/incassomoment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inexploitatiereden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/informatieobjectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkomensbron.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkomenssoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inschrijvingherkomst.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inspectierapportsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inspectierapportstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kandidaatstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kwaliteit/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kwaliteit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kwaliteitsniveau.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/leningaflosvorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/leningdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/leningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/maatschappelijklabel.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/machtigingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    35393 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/materiaaldetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/materiaalsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/medewerkerrol.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/medewerkersoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/meeteenheid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoud/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudslabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudspecialisme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/opleidingsniveau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/oppervlaktesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/opzegtermijn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/organisatie/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/organisatie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/organisatievorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomsten/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomststatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/passendheiddetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/passendheidssoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prestatieafspraak.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectontwikkeling/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectontwikkeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/provincie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiedetailmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiedetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatieintakevorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/puntenberekeningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/puntenmutatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/reclamatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/reclamatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/redenontbinding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/redenopzegging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/redenvernietiging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/regiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatieadressoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatiedetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatierolsoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relaties/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relaties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/rentesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13384 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/ruimtedetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/ruimteligging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/ruimtesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/sanctiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/sanctiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/signaleringdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/signaleringsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/signaleringstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/taal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/uitexploitatiereden.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/uitvoerendesoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/vastgoed/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/vastgoed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verantwoordingregime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verbijzonderingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verbijzonderingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verrekeningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/vertrouwelijkheid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/voorrangdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/voorrangsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woningtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py
--rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woonruimteverdeling/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woonsituatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woonvorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaakobjectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaakrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaakstatussoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaaktypesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata_uitbreiding.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24170 2024-05-16 13:57:38.000000 woningwaardering-0.2.0a1/woningwaardering.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    23957 2024-05-16 13:57:38.000000 woningwaardering-0.2.0a1/woningwaardering.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:57:38.000000 woningwaardering-0.2.0a1/woningwaardering.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-16 13:57:38.000000 woningwaardering-0.2.0a1/woningwaardering.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 13:57:38.000000 woningwaardering-0.2.0a1/woningwaardering.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.914697 woningwaardering-0.2.14a0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.838697 woningwaardering-0.2.14a0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.846697 woningwaardering-0.2.14a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3565 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    26722 2024-05-19 19:31:34.910697 woningwaardering-0.2.14a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    24890 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.838697 woningwaardering-0.2.14a0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.846697 woningwaardering-0.2.14a0/docs/afbeeldingen/
+-rw-r--r--   0 runner    (1001) docker     (127)    34043 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/docs/afbeeldingen/excel_viewer.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)   132221 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/docs/afbeeldingen/oppervlakte_van_vertrekken.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.838697 woningwaardering-0.2.14a0/docs/implementatietoelichting-beleidsboeken/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.850697 woningwaardering-0.2.14a0/docs/implementatietoelichting-beleidsboeken/2024/
+-rw-r--r--   0 runner    (1001) docker     (127)    33544 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.850697 woningwaardering-0.2.14a0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/scripts/genereer_opzet_woningwaarderinggroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/scripts/genereer_test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/scripts/genereer_vera_referentiedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/scripts/uitbreiden_vera_modellen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-19 19:31:34.914697 woningwaardering-0.2.14a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/taskfile.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.850697 woningwaardering-0.2.14a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.838697 woningwaardering-0.2.14a0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.838697 woningwaardering-0.2.14a0/tests/data/input/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.850697 woningwaardering-0.2.14a0/tests/data/input/generiek/
+-rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/generiek/37101000032.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.854697 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/12006000004.json
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/12006000004.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/23003000050.json
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/23003000050.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/25048000007.json
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/25048000007.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/28018000044.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/28018000044.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/37101000032.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14864 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/41027000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/41027000003.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16792 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/41123000005.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17301 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/41162000015.json
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/41162000015.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12899 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/41164000002.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/51011000042.json
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/51011000042.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/71211000027.json
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/71211000027.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/77795000000.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/81020000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/81020000003.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/81065000089.json
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/81065000089.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/85651000021.json
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/85651000021.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/87402000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/87402000003.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.838697 woningwaardering-0.2.14a0/tests/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.838697 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.838697 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.858697 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.858697 woningwaardering-0.2.14a0/tests/stelsels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.858697 woningwaardering-0.2.14a0/tests/stelsels/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/config/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.858697 woningwaardering-0.2.14a0/tests/stelsels/stelsel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.858697 woningwaardering-0.2.14a0/tests/stelsels/stelselgroep/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/test_ZelfstandigeWoonruimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.858697 woningwaardering-0.2.14a0/tests/stelsels/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/utils/test_import_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/utils/test_is_geldig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/utils/test_vind_yaml_bestanden.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.842697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.858697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.838697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.858697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.md
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.md
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.838697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.838697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.858697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_A++++_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_mgw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/test_Energieprestatie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.858697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.838697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.862697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.838697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.838697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.862697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.862697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.842697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.862697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.842697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.842697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.862697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/gedeelde_berging.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.862697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.842697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.866697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten_individueel.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten_individueel.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.842697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.842697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.866697 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.866697 woningwaardering-0.2.14a0/wettelijke-documenten/
+-rw-r--r--   0 runner    (1001) docker     (127)   116885 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.866697 woningwaardering-0.2.14a0/woningwaardering/
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-19 19:31:34.000000 woningwaardering-0.2.14a0/woningwaardering/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.866697 woningwaardering-0.2.14a0/woningwaardering/stelsels/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.866697 woningwaardering-0.2.14a0/woningwaardering/stelsels/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/stelsel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/stelselgroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/stelselgroepversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8737 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.866697 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.870697 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.870697 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/bouwjaar_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_0-25m2_energielabel_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_25-40m2_energielabel_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_40m2+_energielabel_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oud_energielabel_punten.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.870697 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.870697 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.870697 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.842697 woningwaardering-0.2.14a0/woningwaardering/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.842697 woningwaardering-0.2.14a0/woningwaardering/templates/stelsels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.870697 woningwaardering-0.2.14a0/woningwaardering/templates/stelsels/stelsel/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/templates/stelsels/stelsel/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.870697 woningwaardering-0.2.14a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.870697 woningwaardering-0.2.14a0/woningwaardering/vera/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.870697 woningwaardering-0.2.14a0/woningwaardering/vera/bvg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/bvg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137423 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/bvg/generated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.874697 woningwaardering-0.2.14a0/woningwaardering/vera/bvg/model_uitbreidingen/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_energieprestatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/bvg/model_uitbreidingen/referentiedata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.906697 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/
+-rw-r--r--   0 runner    (1001) docker     (127)    15108 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/aanbiedingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/accountstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/adressoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/afletterstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/afrekenwijzesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/afspraakstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/afwezigheidsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/aktesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/authentiekgegevenbron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/authentiekgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/bedrijfsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/begrotingversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/bestemming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/betaalgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/betaalwijzesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/betalingsregelingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/boekingdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/boekingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/boekingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/boekjaarstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27844 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/brandwerendheidscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/btw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/btwaangiftestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/burgerlijkestaat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/clustersoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/collectiefobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/communicatiekanaal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/communicatierichting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/conditiescore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/contactgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/contactgegevenstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/crediteursoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/crediteurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/dagdeel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/debiteursoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/debiteurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/defectlocatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/defectoorzaak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/defectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/defectstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/doelgroep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.910697 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/dossier/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/dossier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheiddetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheiddetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidinterieur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidisolatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidligging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidmonument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidprijsconditie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidsanitair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eindedetailreden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eindereden.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.910697 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/energie/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/energie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/energielabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/energieprestatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/energieprestatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/externeincassosoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/externeincassostatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/factuurbetaalwijze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/factuursoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.910697 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/financien/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/financien/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/gebeurtenissoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/geometriesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/geslacht.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/huurgeschilsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/huurgeschilstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/huurklasse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/huuropzeggingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/incassomoment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inexploitatiereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/informatieobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inkomensbron.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inkomenssoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inschrijvingherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inspectierapportsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inspectierapportstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/kandidaatstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.910697 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/kwaliteit/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/kwaliteit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/kwaliteitsniveau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/leningaflosvorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/leningdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/leningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/maatschappelijklabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/machtigingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35393 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/materiaaldetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/materiaalsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/medewerkerrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/medewerkersoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/meeteenheid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.910697 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoud/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudslabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudspecialisme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/opleidingsniveau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/oppervlaktesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/opzegtermijn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.910697 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/organisatie/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/organisatie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/organisatievorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.910697 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/overeenkomsten/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/overeenkomstsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/overeenkomststatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/passendheiddetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/passendheidssoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/prestatieafspraak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/prijscomponentsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.910697 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/projectontwikkeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/projectontwikkeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/projectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/projectstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/provincie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/publicatiedetailmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/publicatiedetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/publicatieintakevorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/publicatiemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/publicatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/puntenberekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/puntenmutatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/reclamatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/reclamatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/redenontbinding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/redenopzegging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/redenvernietiging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/regiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/relatieadressoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/relatiedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/relatierolsoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.910697 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/relaties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/relaties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/relatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/relatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/rentesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13384 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/ruimtedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/ruimteligging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/ruimtesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/sanctiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/sanctiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/signaleringdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/signaleringsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/signaleringstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/taal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/uitexploitatiereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/uitvoerendesoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.910697 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/vastgoed/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/vastgoed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/verantwoordingregime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/verbijzonderingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/verbijzonderingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/verrekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/vertrouwelijkheid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/voorrangdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/voorrangsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/woningtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.910697 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/woonruimteverdeling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/woonsituatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/woonvorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/zaakobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/zaakrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/zaakstatussoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/zaaktypesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata_uitbreiding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-19 19:31:30.000000 woningwaardering-0.2.14a0/woningwaardering/vera/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-19 19:31:34.910697 woningwaardering-0.2.14a0/woningwaardering.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    26722 2024-05-19 19:31:34.000000 woningwaardering-0.2.14a0/woningwaardering.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23957 2024-05-19 19:31:34.000000 woningwaardering-0.2.14a0/woningwaardering.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-19 19:31:34.000000 woningwaardering-0.2.14a0/woningwaardering.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-19 19:31:34.000000 woningwaardering-0.2.14a0/woningwaardering.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-19 19:31:34.000000 woningwaardering-0.2.14a0/woningwaardering.egg-info/top_level.txt
```

### Comparing `woningwaardering-0.2.0a1/.github/workflows/cicd.yml` & `woningwaardering-0.2.14a0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/.github/workflows/publish-to-pypi.yml` & `woningwaardering-0.2.14a0/.github/workflows/publish-to-pypi.yml`

 * *Files 18% similar despite different names*

```diff
@@ -1,52 +1,25 @@
 name: Publish Python distribution
-
+run-name: Publish release ${{ github.ref_name }}
 on:
   push:
     tags:
       - "v*"
 
 jobs:
-  dump_contexts_to_log:
-    runs-on: ubuntu-latest
-    steps:
-      - name: Dump GitHub context
-        env:
-          GITHUB_CONTEXT: ${{ toJson(github) }}
-        run: echo "$GITHUB_CONTEXT"
-      - name: Dump job context
-        env:
-          JOB_CONTEXT: ${{ toJson(job) }}
-        run: echo "$JOB_CONTEXT"
-      - name: Dump steps context
-        env:
-          STEPS_CONTEXT: ${{ toJson(steps) }}
-        run: echo "$STEPS_CONTEXT"
-      - name: Dump runner context
-        env:
-          RUNNER_CONTEXT: ${{ toJson(runner) }}
-        run: echo "$RUNNER_CONTEXT"
-      - name: Dump strategy context
-        env:
-          STRATEGY_CONTEXT: ${{ toJson(strategy) }}
-        run: echo "$STRATEGY_CONTEXT"
-      - name: Dump matrix context
-        env:
-          MATRIX_CONTEXT: ${{ toJson(matrix) }}
-        run: echo "$MATRIX_CONTEXT"
   build:
     name: Build distribution 📦
     runs-on: ubuntu-latest
 
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
-          python-version: "3.x"
+          python-version: ">=3.10"
       - name: Install pypa/build
         run: >-
           python3 -m
           pip install
           build
           --user
       - name: Build a binary wheel and a source tarball
@@ -130,15 +103,17 @@
       - name: Create GitHub Release
         env:
           GITHUB_TOKEN: ${{ github.token }}
         run: >-
           gh release create
           '${{ github.ref_name }}'
           --repo '${{ github.repository }}'
+          ${{ contains(fromJSON('["alpha", "beta", "rc"]'), github.ref_name) && '--prerelease' || ''}}
           --generate-notes
+          --notes-start-tag $(gh release view --repo '${{ github.repository }}' --jq .tagName --json tagName)
       - name: Upload artifact signatures to GitHub Release
         env:
           GITHUB_TOKEN: ${{ github.token }}
         # Upload to GitHub Release using the `gh` CLI.
         # `dist/` contains the built packages, and the
         # sigstore-produced signatures and certificates.
         run: >-
```

### Comparing `woningwaardering-0.2.0a1/.gitignore` & `woningwaardering-0.2.14a0/.gitignore`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/.pre-commit-config.yaml` & `woningwaardering-0.2.14a0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/LICENSE` & `woningwaardering-0.2.14a0/LICENSE`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/PKG-INFO` & `woningwaardering-0.2.14a0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woningwaardering
-Version: 0.2.0a1
+Version: 0.2.14a0
 Summary: Berekent de punten van een woning op basis van het woningwaarderingsstelsel.
 Author-email: Woonstad Rotterdam <info@woonstadrotterdam.nl>, Ben Verhees <ben.verhees@woonstadrotterdam.nl>, Tiddo Loos <tiddo.loos@woonstadrotterdam.nl>, Tomer Gabay <tomer.gabay@woonstadrotterdam.nl>
 Project-URL: Homepage, https://github.com/WoonstadRotterdamTemp/woningwaardering
 Project-URL: Issues, https://github.com/WoonstadRotterdamTemp/woningwaardering/issues
 Keywords: woning,waardering,stelsel,woningwaarderingsstelsel,wws
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -176,14 +176,54 @@
 De begin- en einddatum van de geldigheid van een stelselgroep wordt vastgelegd in de configuratie `.yml` van het betreffende stelsel.
 
 #### Stelselgroepversies
 
 De daadwerkelijke implementatie van een stelselgroep is een `Stelselgroepversie`. Voor stelselgroepversies wordt de naam van de stelselgroep gevolgd door het jaar waarin de versie van de stelselgroep in gebruik gaat. Bijvoorbeeld: de implementatie van de `Stelselgroepversie` voor oppervlakte van vertrekken die in gaat in het jaar 2024 bevindt zich in [woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py](woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py).
 Omdat het lastig is met terugwerkende kracht te achterhalen in welk jaar een versie van een stelselgroep ingegaan is, gebruiken we voor de eerste versie van een stelselgroep het jaar van de implementatie van de stelselgroep in deze module. Wanneer de berekening van een stelselgroep in een bepaald jaar niet wijzigt, wordt er geen nieuwe stelselgroepversie aangemaakt. De begin- en einddatum van de geldigheid van een stelselgroepversie wordt vastgelegd in de configuratie `.yml` van het betreffende stelsel.
 
+### Releasemanagement
+
+#### Versienummering
+
+Voor versienummering maken we gebruik van [SemVer](https://semver.org/lang/nl/):
+
+Bij SemVer wordt een versienummer in de vorm MAJOR.MINOR.PATCH gebruikt, waarbij elk element als volgt wordt verhoogd:
+
+- `MAJOR` wordt verhoogd bij incompatibele API-wijzigingen,
+- `MINOR` wordt verhoogd bij het toevoegen van functionaliteit die compatibel is met de vorige versie, en
+- `PATCH` wordt verhoogd bij compatibele bugfixes.
+
+Er zijn aanvullende labels beschikbaar voor pre-release en build-metadata om toe te voegen aan het `MAJOR.MINOR.PATCH`-formaat.
+
+Bijvoorbeeld: stel dat de huidige versie `0.1.3-alpha` is.
+
+- De suffix `-alpha` wordt gebruikt zolang de software nog niet volledig is, bijvoorbeeld zolang nog niet alle beoogde stelselgroepen geïmplementeerd zijn
+- Wanneer een nieuwe release alleen compatibele bugfixes of updates van dependencies bevat, wordt de nieuwe versie `0.1.4-alpha`
+- Wanneer een nieuwe release ook compatibele nieuwe functionaliteit toevoegt, bijvoorbeeld de implementatie van een nieuwe stelselgroep, dan wordt de nieuwe versie `0.2.0-alpha`.
+- Wanneer alle beoogde stelselgroepen geïmplementeerd zijn, wordt de nieuwe versie `1.0.0-beta`. De publieke api mag vanaf dan enkel nog backwards-compatible wijzigen.
+- Wanneer de software volledig is en in productie genomen wordt, wordt de nieuwe versie `1.0.0`
+- Wanneer er een incompatible wijziging is in de VERA modellen, wordt de nieuwe versie `2.0.0`, eventueel met het `-alpha` of `-beta` label, afhankelijk van de implementatiestatus.
+
+#### Releaseproces
+
+Om een nieuwe release te starten, moet er een Git tag aangemaak worden volgens het format `v<versienummer>`. De prefix `v` geeft aan dat de tag een versiepunt markeert.
+
+Bijvoorbeeld:
+
+```cli
+$ git tag v0.2.3-alpha
+$ git push --tags
+```
+
+Hiermee start het releaseproces, gedefinieerd in een GitHub workflow: [.github/workflows/publish-to-pypi.ymls](.github/workflows/publish-to-pypi.yml)
+
+In dit proces wordt een package aangemaakt met een [Python versienummer](https://packaging.python.org/en/latest/discussions/versioning/), afgeleid van het SemVer nummer in de tag. Bijvoorbeeld: `0.2.3-alpha` wordt `0.2.3a0`
+
+De package wordt eerst gepubliceerd op [TestPyPi](https://test.pypi.org/project/woningwaardering/). Na goedkeuring wordt de package naar [PyPi](https://pypi.org/project/woningwaardering/) gepubliceerd. Daarna wordt er een release aangemaakt in GitHub, met een changelog met de titel en link naar alle pull requests die deel uitmaken van deze release.
+
 ### Testing
 
 Voor het testen van code wordt het [pytest framework](https://docs.pytest.org/en/8.0.x/index.html) gebruikt. Meer informatie is te vinden over het framework.
 Passende tests worden altijd met de nieuw geschreven code opgeleverd.
 Er zijn verschillende "test-scopes" te bedenken, zoals het testen van details en specifieke functies.
 Daarnaast is het testen van een hele keten of stelselgroep-object ook vereist.
 Bij het opleveren van nieuwe code moet aan beide test-scopes gedacht worden.
```

### Comparing `woningwaardering-0.2.0a1/README.md` & `woningwaardering-0.2.14a0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -137,14 +137,54 @@
 De begin- en einddatum van de geldigheid van een stelselgroep wordt vastgelegd in de configuratie `.yml` van het betreffende stelsel.
 
 #### Stelselgroepversies
 
 De daadwerkelijke implementatie van een stelselgroep is een `Stelselgroepversie`. Voor stelselgroepversies wordt de naam van de stelselgroep gevolgd door het jaar waarin de versie van de stelselgroep in gebruik gaat. Bijvoorbeeld: de implementatie van de `Stelselgroepversie` voor oppervlakte van vertrekken die in gaat in het jaar 2024 bevindt zich in [woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py](woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py).
 Omdat het lastig is met terugwerkende kracht te achterhalen in welk jaar een versie van een stelselgroep ingegaan is, gebruiken we voor de eerste versie van een stelselgroep het jaar van de implementatie van de stelselgroep in deze module. Wanneer de berekening van een stelselgroep in een bepaald jaar niet wijzigt, wordt er geen nieuwe stelselgroepversie aangemaakt. De begin- en einddatum van de geldigheid van een stelselgroepversie wordt vastgelegd in de configuratie `.yml` van het betreffende stelsel.
 
+### Releasemanagement
+
+#### Versienummering
+
+Voor versienummering maken we gebruik van [SemVer](https://semver.org/lang/nl/):
+
+Bij SemVer wordt een versienummer in de vorm MAJOR.MINOR.PATCH gebruikt, waarbij elk element als volgt wordt verhoogd:
+
+- `MAJOR` wordt verhoogd bij incompatibele API-wijzigingen,
+- `MINOR` wordt verhoogd bij het toevoegen van functionaliteit die compatibel is met de vorige versie, en
+- `PATCH` wordt verhoogd bij compatibele bugfixes.
+
+Er zijn aanvullende labels beschikbaar voor pre-release en build-metadata om toe te voegen aan het `MAJOR.MINOR.PATCH`-formaat.
+
+Bijvoorbeeld: stel dat de huidige versie `0.1.3-alpha` is.
+
+- De suffix `-alpha` wordt gebruikt zolang de software nog niet volledig is, bijvoorbeeld zolang nog niet alle beoogde stelselgroepen geïmplementeerd zijn
+- Wanneer een nieuwe release alleen compatibele bugfixes of updates van dependencies bevat, wordt de nieuwe versie `0.1.4-alpha`
+- Wanneer een nieuwe release ook compatibele nieuwe functionaliteit toevoegt, bijvoorbeeld de implementatie van een nieuwe stelselgroep, dan wordt de nieuwe versie `0.2.0-alpha`.
+- Wanneer alle beoogde stelselgroepen geïmplementeerd zijn, wordt de nieuwe versie `1.0.0-beta`. De publieke api mag vanaf dan enkel nog backwards-compatible wijzigen.
+- Wanneer de software volledig is en in productie genomen wordt, wordt de nieuwe versie `1.0.0`
+- Wanneer er een incompatible wijziging is in de VERA modellen, wordt de nieuwe versie `2.0.0`, eventueel met het `-alpha` of `-beta` label, afhankelijk van de implementatiestatus.
+
+#### Releaseproces
+
+Om een nieuwe release te starten, moet er een Git tag aangemaak worden volgens het format `v<versienummer>`. De prefix `v` geeft aan dat de tag een versiepunt markeert.
+
+Bijvoorbeeld:
+
+```cli
+$ git tag v0.2.3-alpha
+$ git push --tags
+```
+
+Hiermee start het releaseproces, gedefinieerd in een GitHub workflow: [.github/workflows/publish-to-pypi.ymls](.github/workflows/publish-to-pypi.yml)
+
+In dit proces wordt een package aangemaakt met een [Python versienummer](https://packaging.python.org/en/latest/discussions/versioning/), afgeleid van het SemVer nummer in de tag. Bijvoorbeeld: `0.2.3-alpha` wordt `0.2.3a0`
+
+De package wordt eerst gepubliceerd op [TestPyPi](https://test.pypi.org/project/woningwaardering/). Na goedkeuring wordt de package naar [PyPi](https://pypi.org/project/woningwaardering/) gepubliceerd. Daarna wordt er een release aangemaakt in GitHub, met een changelog met de titel en link naar alle pull requests die deel uitmaken van deze release.
+
 ### Testing
 
 Voor het testen van code wordt het [pytest framework](https://docs.pytest.org/en/8.0.x/index.html) gebruikt. Meer informatie is te vinden over het framework.
 Passende tests worden altijd met de nieuw geschreven code opgeleverd.
 Er zijn verschillende "test-scopes" te bedenken, zoals het testen van details en specifieke functies.
 Daarnaast is het testen van een hele keten of stelselgroep-object ook vereist.
 Bij het opleveren van nieuwe code moet aan beide test-scopes gedacht worden.
```

### Comparing `woningwaardering-0.2.0a1/docs/afbeeldingen/excel_viewer.png` & `woningwaardering-0.2.14a0/docs/afbeeldingen/excel_viewer.png`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw` & `woningwaardering-0.2.14a0/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/docs/afbeeldingen/oppervlakte_van_vertrekken.png` & `woningwaardering-0.2.14a0/docs/afbeeldingen/oppervlakte_van_vertrekken.png`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md` & `woningwaardering-0.2.14a0/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/pyproject.toml` & `woningwaardering-0.2.14a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/scripts/genereer_opzet_woningwaarderinggroep.py` & `woningwaardering-0.2.14a0/scripts/genereer_opzet_woningwaarderinggroep.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,18 +84,20 @@
     woningwaarderingstelselgroep.name, "_"
 ).replace("_", "")
 
 stelsels_folder = Path("woningwaardering") / "stelsels"
 stelsel_folder = stelsels_folder / stelsel
 stelsel_file_path = stelsel_folder / f"{stelsel}.py"
 
+stelsel_class_naam = string.capwords(woningwaarderingstelsel.name, "_").replace("_", "")
+
 if check_write(stelsel_file_path):
     stelsel_template = environment.get_template("stelsels/stelsel/stelsel.py.j2")
     stelsel_result = stelsel_template.render(
-        className=string.capwords(woningwaarderingstelsel.name, "_").replace("_", ""),
+        className=stelsel_class_naam,
         stelsel=woningwaarderingstelsel,
     )
     stelsel_folder.mkdir(parents=True, exist_ok=True)
     stelsel_file = stelsel_file_path.write_text(stelsel_result)
 
 stelselconfig: Stelselconfig
 
@@ -189,11 +191,11 @@
 )
 
 (stelselgroep_folder / "__init__.py").write_text(stelselgroep_init_result)
 
 stelsel_init_template = environment.get_template("stelsels/stelsel/__init__.py.j2")
 
 stelsel_init_result = stelsel_init_template.render(
-    stelselgroepen=stelselconfig.stelselgroepen
+    className=stelsel_class_naam, stelselconfig=stelselconfig
 )
 
 (stelsel_folder / "__init__.py").write_text(stelsel_init_result)
```

### Comparing `woningwaardering-0.2.0a1/scripts/genereer_test_output.py` & `woningwaardering-0.2.14a0/scripts/genereer_test_output.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import sys
 from datetime import date, datetime
 from pathlib import Path
 
 from loguru import logger
 from pydantic import ValidationError
 
-from woningwaardering.stelsels.zelfstandige_woonruimten.zelfstandige_woonruimten import (
+from woningwaardering.stelsels.zelfstandige_woonruimten import (
     ZelfstandigeWoonruimten,
 )
 from woningwaardering.vera.bvg.generated import (
     EenhedenEenheid,
 )
 
 logger.enable("woningwaardering")
```

### Comparing `woningwaardering-0.2.0a1/scripts/genereer_vera_referentiedata.py` & `woningwaardering-0.2.14a0/scripts/genereer_vera_referentiedata.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/scripts/uitbreiden_vera_modellen.py` & `woningwaardering-0.2.14a0/scripts/uitbreiden_vera_modellen.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/taskfile.yml` & `woningwaardering-0.2.14a0/taskfile.yml`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/conftest.py` & `woningwaardering-0.2.14a0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/generiek/37101000032.json` & `woningwaardering-0.2.14a0/tests/data/input/generiek/37101000032.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/12006000004.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/12006000004.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/23003000050.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/23003000050.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/25048000007.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/25048000007.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/28018000044.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/28018000044.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/37101000032.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/37101000032.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41027000003.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/41027000003.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41123000005.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/41123000005.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41162000015.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/41162000015.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41164000002.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/41164000002.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/51011000042.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/51011000042.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/71211000027.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/71211000027.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/77795000000.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/77795000000.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/81020000003.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/81020000003.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/81065000089.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/81065000089.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/85651000021.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/85651000021.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/87402000003.json` & `woningwaardering-0.2.14a0/tests/data/input/zelfstandige_woonruimten/87402000003.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json` & `woningwaardering-0.2.14a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/config/test_config.py` & `woningwaardering-0.2.14a0/tests/stelsels/config/test_config.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py` & `woningwaardering-0.2.14a0/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py` & `woningwaardering-0.2.14a0/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/test_ZelfstandigeWoonruimten.py` & `woningwaardering-0.2.14a0/tests/stelsels/test_ZelfstandigeWoonruimten.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from test_utils import assert_output_model
 
-from woningwaardering.stelsels.zelfstandige_woonruimten.zelfstandige_woonruimten import (
+from woningwaardering.stelsels.zelfstandige_woonruimten import (
     ZelfstandigeWoonruimten,
 )
 from woningwaardering.vera.bvg.generated import (
     WoningwaarderingResultatenWoningwaarderingResultaat,
 )
```

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/utils/test_import_class.py` & `woningwaardering-0.2.14a0/tests/stelsels/utils/test_import_class.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from woningwaardering.stelsels.utils import import_class
 
 
 @pytest.mark.parametrize(
     "module_path, class_naam, class_type",
     [
         (
-            "woningwaardering.stelsels.zelfstandige_woonruimten.zelfstandige_woonruimten",
+            "woningwaardering.stelsels.zelfstandige_woonruimten",
             "ZelfstandigeWoonruimten",
             Stelsel,
         ),
         (
             "woningwaardering.stelsels.zelfstandige_woonruimten.oppervlakte_van_vertrekken",
             "OppervlakteVanVertrekken",
             Stelselgroep,
```

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/utils/test_is_geldig.py` & `woningwaardering-0.2.14a0/tests/stelsels/utils/test_is_geldig.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/test_Energieprestatie.py` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/test_Energieprestatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py` & `woningwaardering-0.2.14a0/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/tests/test_utils.py` & `woningwaardering-0.2.14a0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt` & `woningwaardering-0.2.14a0/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/__init__.py` & `woningwaardering-0.2.14a0/woningwaardering/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/config/config.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/config/config.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/stelsel.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/stelsel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/stelselgroep.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/stelselgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/stelselgroepversie.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/stelselgroepversie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/utils.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/utils.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py` & `woningwaardering-0.2.14a0/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 from datetime import date
 
 from loguru import logger
 
-
 from woningwaardering.stelsels.stelsel import Stelsel
 from woningwaardering.stelsels import utils
 from woningwaardering.vera.bvg.generated import (
     EenhedenEenheid,
 )
 from woningwaardering.vera.referentiedata import (
     Woningwaarderingstelsel,
```

### Comparing `woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2` & `woningwaardering-0.2.14a0/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2` & `woningwaardering-0.2.14a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2` & `woningwaardering-0.2.14a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/bvg/generated.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/bvg/generated.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_energieprestatie.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_energieprestatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/__init__.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aanbiedingstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/aanbiedingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/accountstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/accountstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/adressoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/adressoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afletterstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/afletterstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afrekenwijzesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/afrekenwijzesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afspraakstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/afspraakstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afwezigheidsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/afwezigheidsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aktesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/aktesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/authentiekgegevenbron.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/authentiekgegevenbron.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/authentiekgegevensoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/authentiekgegevensoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bedrijfsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/bedrijfsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/begrotingversie.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/begrotingversie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bestemming.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/bestemming.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betaalgegevensoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/betaalgegevensoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betaalwijzesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/betaalwijzesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betalingsregelingstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/betalingsregelingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekingdetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/boekingdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekingsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/boekingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekingstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/boekingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekjaarstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/boekjaarstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/brandwerendheidscore.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/brandwerendheidscore.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/btw.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/btw.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/btwaangiftestatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/btwaangiftestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/burgerlijkestaat.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/burgerlijkestaat.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/clustersoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/clustersoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/collectiefobjectsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/collectiefobjectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/communicatiekanaal.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/communicatiekanaal.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/communicatierichting.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/communicatierichting.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/conditiescore.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/conditiescore.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevensoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/contactgegevensoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevenstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/contactgegevenstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/crediteursoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/crediteursoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/crediteurstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/crediteurstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/dagdeel.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/dagdeel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/debiteursoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/debiteursoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/debiteurstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/debiteurstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectlocatie.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/defectlocatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectoorzaak.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/defectoorzaak.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/defectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/defectstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/doelgroep.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/doelgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/dossier/__init__.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/dossier/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheiddetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheiddetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheiddetailstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheiddetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidinterieur.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidinterieur.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidisolatie.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidisolatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidligging.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidligging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidmonument.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidmonument.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidprijsconditie.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidprijsconditie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidsanitair.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidsanitair.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eenheidstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eindedetailreden.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eindedetailreden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eindereden.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/eindereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energielabel.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/energielabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energieprestatiesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/energieprestatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energieprestatiestatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/energieprestatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/externeincassosoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/externeincassosoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/externeincassostatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/externeincassostatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/factuurbetaalwijze.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/factuurbetaalwijze.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/factuursoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/factuursoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/financien/__init__.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/financien/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/gebeurtenissoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/gebeurtenissoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/geometriesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/geometriesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/geslacht.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/geslacht.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huurgeschilsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/huurgeschilsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huurgeschilstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/huurgeschilstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huurklasse.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/huurklasse.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huuropzeggingstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/huuropzeggingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/incassomoment.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/incassomoment.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inexploitatiereden.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inexploitatiereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/informatieobjectsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/informatieobjectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkomensbron.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inkomensbron.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkomenssoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inkomenssoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inschrijvingherkomst.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inschrijvingherkomst.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inspectierapportsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inspectierapportsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inspectierapportstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/inspectierapportstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kandidaatstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/kandidaatstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kwaliteitsniveau.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/kwaliteitsniveau.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/leningaflosvorm.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/leningaflosvorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/leningdetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/leningdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/leningsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/leningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/maatschappelijklabel.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/maatschappelijklabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/machtigingsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/machtigingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/materiaaldetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/materiaaldetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/materiaalsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/materiaalsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/medewerkerrol.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/medewerkerrol.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/medewerkersoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/medewerkersoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/meeteenheid.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/meeteenheid.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoud/__init__.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoud/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudslabel.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudslabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudspecialisme.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudspecialisme.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/opleidingsniveau.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/opleidingsniveau.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/oppervlaktesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/oppervlaktesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/opzegtermijn.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/opzegtermijn.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/organisatievorm.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/organisatievorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/overeenkomstsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomststatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/overeenkomststatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/passendheiddetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/passendheiddetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/passendheidssoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/passendheidssoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prestatieafspraak.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/prestatieafspraak.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/prijscomponentsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/projectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/projectstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/provincie.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/provincie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiedetailmodel.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/publicatiedetailmodel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiedetailstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/publicatiedetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatieintakevorm.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/publicatieintakevorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiemodel.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/publicatiemodel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiestatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/publicatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/puntenberekeningsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/puntenberekeningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/puntenmutatiesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/puntenmutatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/reclamatiesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/reclamatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/reclamatiestatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/reclamatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/redenontbinding.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/redenontbinding.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/redenopzegging.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/redenopzegging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/redenvernietiging.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/redenvernietiging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/regiesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/regiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatieadressoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/relatieadressoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatiedetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/relatiedetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatierolsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/relatierolsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relaties/__init__.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/relaties/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatiesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/relatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatiestatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/relatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/rentesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/rentesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/ruimtedetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/ruimtedetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/ruimteligging.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/ruimteligging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/ruimtesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/ruimtesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/sanctiesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/sanctiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/sanctiestatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/sanctiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/signaleringdetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/signaleringdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/signaleringsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/signaleringsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/signaleringstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/signaleringstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/taal.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/taal.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/uitexploitatiereden.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/uitexploitatiereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/uitvoerendesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/uitvoerendesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/vastgoed/__init__.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/vastgoed/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verantwoordingregime.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/verantwoordingregime.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verbijzonderingsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/verbijzonderingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verbijzonderingstatus.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/verbijzonderingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verrekeningsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/verrekeningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/vertrouwelijkheid.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/vertrouwelijkheid.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/voorrangdetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/voorrangdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/voorrangsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/voorrangsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woningtype.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/woningtype.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woonsituatiesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/woonsituatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woonvorm.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/woonvorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaakobjectsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/zaakobjectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaakrol.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/zaakrol.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaakstatussoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/zaakstatussoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaaktypesoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/zaaktypesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata_uitbreiding.csv` & `woningwaardering-0.2.14a0/woningwaardering/vera/referentiedata_uitbreiding.csv`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering/vera/utils.py` & `woningwaardering-0.2.14a0/woningwaardering/vera/utils.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.2.0a1/woningwaardering.egg-info/PKG-INFO` & `woningwaardering-0.2.14a0/woningwaardering.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woningwaardering
-Version: 0.2.0a1
+Version: 0.2.14a0
 Summary: Berekent de punten van een woning op basis van het woningwaarderingsstelsel.
 Author-email: Woonstad Rotterdam <info@woonstadrotterdam.nl>, Ben Verhees <ben.verhees@woonstadrotterdam.nl>, Tiddo Loos <tiddo.loos@woonstadrotterdam.nl>, Tomer Gabay <tomer.gabay@woonstadrotterdam.nl>
 Project-URL: Homepage, https://github.com/WoonstadRotterdamTemp/woningwaardering
 Project-URL: Issues, https://github.com/WoonstadRotterdamTemp/woningwaardering/issues
 Keywords: woning,waardering,stelsel,woningwaarderingsstelsel,wws
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -176,14 +176,54 @@
 De begin- en einddatum van de geldigheid van een stelselgroep wordt vastgelegd in de configuratie `.yml` van het betreffende stelsel.
 
 #### Stelselgroepversies
 
 De daadwerkelijke implementatie van een stelselgroep is een `Stelselgroepversie`. Voor stelselgroepversies wordt de naam van de stelselgroep gevolgd door het jaar waarin de versie van de stelselgroep in gebruik gaat. Bijvoorbeeld: de implementatie van de `Stelselgroepversie` voor oppervlakte van vertrekken die in gaat in het jaar 2024 bevindt zich in [woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py](woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py).
 Omdat het lastig is met terugwerkende kracht te achterhalen in welk jaar een versie van een stelselgroep ingegaan is, gebruiken we voor de eerste versie van een stelselgroep het jaar van de implementatie van de stelselgroep in deze module. Wanneer de berekening van een stelselgroep in een bepaald jaar niet wijzigt, wordt er geen nieuwe stelselgroepversie aangemaakt. De begin- en einddatum van de geldigheid van een stelselgroepversie wordt vastgelegd in de configuratie `.yml` van het betreffende stelsel.
 
+### Releasemanagement
+
+#### Versienummering
+
+Voor versienummering maken we gebruik van [SemVer](https://semver.org/lang/nl/):
+
+Bij SemVer wordt een versienummer in de vorm MAJOR.MINOR.PATCH gebruikt, waarbij elk element als volgt wordt verhoogd:
+
+- `MAJOR` wordt verhoogd bij incompatibele API-wijzigingen,
+- `MINOR` wordt verhoogd bij het toevoegen van functionaliteit die compatibel is met de vorige versie, en
+- `PATCH` wordt verhoogd bij compatibele bugfixes.
+
+Er zijn aanvullende labels beschikbaar voor pre-release en build-metadata om toe te voegen aan het `MAJOR.MINOR.PATCH`-formaat.
+
+Bijvoorbeeld: stel dat de huidige versie `0.1.3-alpha` is.
+
+- De suffix `-alpha` wordt gebruikt zolang de software nog niet volledig is, bijvoorbeeld zolang nog niet alle beoogde stelselgroepen geïmplementeerd zijn
+- Wanneer een nieuwe release alleen compatibele bugfixes of updates van dependencies bevat, wordt de nieuwe versie `0.1.4-alpha`
+- Wanneer een nieuwe release ook compatibele nieuwe functionaliteit toevoegt, bijvoorbeeld de implementatie van een nieuwe stelselgroep, dan wordt de nieuwe versie `0.2.0-alpha`.
+- Wanneer alle beoogde stelselgroepen geïmplementeerd zijn, wordt de nieuwe versie `1.0.0-beta`. De publieke api mag vanaf dan enkel nog backwards-compatible wijzigen.
+- Wanneer de software volledig is en in productie genomen wordt, wordt de nieuwe versie `1.0.0`
+- Wanneer er een incompatible wijziging is in de VERA modellen, wordt de nieuwe versie `2.0.0`, eventueel met het `-alpha` of `-beta` label, afhankelijk van de implementatiestatus.
+
+#### Releaseproces
+
+Om een nieuwe release te starten, moet er een Git tag aangemaak worden volgens het format `v<versienummer>`. De prefix `v` geeft aan dat de tag een versiepunt markeert.
+
+Bijvoorbeeld:
+
+```cli
+$ git tag v0.2.3-alpha
+$ git push --tags
+```
+
+Hiermee start het releaseproces, gedefinieerd in een GitHub workflow: [.github/workflows/publish-to-pypi.ymls](.github/workflows/publish-to-pypi.yml)
+
+In dit proces wordt een package aangemaakt met een [Python versienummer](https://packaging.python.org/en/latest/discussions/versioning/), afgeleid van het SemVer nummer in de tag. Bijvoorbeeld: `0.2.3-alpha` wordt `0.2.3a0`
+
+De package wordt eerst gepubliceerd op [TestPyPi](https://test.pypi.org/project/woningwaardering/). Na goedkeuring wordt de package naar [PyPi](https://pypi.org/project/woningwaardering/) gepubliceerd. Daarna wordt er een release aangemaakt in GitHub, met een changelog met de titel en link naar alle pull requests die deel uitmaken van deze release.
+
 ### Testing
 
 Voor het testen van code wordt het [pytest framework](https://docs.pytest.org/en/8.0.x/index.html) gebruikt. Meer informatie is te vinden over het framework.
 Passende tests worden altijd met de nieuw geschreven code opgeleverd.
 Er zijn verschillende "test-scopes" te bedenken, zoals het testen van details en specifieke functies.
 Daarnaast is het testen van een hele keten of stelselgroep-object ook vereist.
 Bij het opleveren van nieuwe code moet aan beide test-scopes gedacht worden.
```

### Comparing `woningwaardering-0.2.0a1/woningwaardering.egg-info/SOURCES.txt` & `woningwaardering-0.2.14a0/woningwaardering.egg-info/SOURCES.txt`

 * *Files identical despite different names*

