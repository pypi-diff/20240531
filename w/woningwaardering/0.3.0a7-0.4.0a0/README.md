# Comparing `tmp/woningwaardering-0.3.0a7.tar.gz` & `tmp/woningwaardering-0.4.0a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woningwaardering-0.3.0a7.tar", last modified: Fri May 24 09:56:50 2024, max compression
+gzip compressed data, was "woningwaardering-0.4.0a0.tar", last modified: Fri May 31 10:34:48 2024, max compression
```

## Comparing `woningwaardering-0.3.0a7.tar` & `woningwaardering-0.4.0a0.tar`

### file list

```diff
@@ -1,483 +1,506 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.704161 woningwaardering-0.3.0a7/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.632161 woningwaardering-0.3.0a7/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/.github/labeler.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.636160 woningwaardering-0.3.0a7/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/.github/workflows/labeler.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    26709 2024-05-24 09:56:50.700161 woningwaardering-0.3.0a7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    24886 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.624160 woningwaardering-0.3.0a7/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.636160 woningwaardering-0.3.0a7/docs/afbeeldingen/
--rw-r--r--   0 runner    (1001) docker     (127)    34043 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/docs/afbeeldingen/excel_viewer.png
--rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw
--rw-r--r--   0 runner    (1001) docker     (127)   132221 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/docs/afbeeldingen/oppervlakte_van_vertrekken.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.624160 woningwaardering-0.3.0a7/docs/implementatietoelichting-beleidsboeken/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.636160 woningwaardering-0.3.0a7/docs/implementatietoelichting-beleidsboeken/2024/
--rw-r--r--   0 runner    (1001) docker     (127)    39279 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.636160 woningwaardering-0.3.0a7/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/scripts/genereer_opzet_woningwaarderinggroep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/scripts/genereer_test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/scripts/genereer_vera_referentiedata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/scripts/uitbreiden_vera_modellen.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-24 09:56:50.704161 woningwaardering-0.3.0a7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/taskfile.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.636160 woningwaardering-0.3.0a7/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.624160 woningwaardering-0.3.0a7/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.624160 woningwaardering-0.3.0a7/tests/data/input/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.636160 woningwaardering-0.3.0a7/tests/data/input/generiek/
--rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/generiek/37101000032.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.640160 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/
--rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/12006000004.json
--rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/12006000004.md
--rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/23003000050.json
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/23003000050.md
--rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/25048000007.json
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/25048000007.md
--rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/28018000044.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/28018000044.md
--rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/37101000032.json
--rw-r--r--   0 runner    (1001) docker     (127)    14864 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/41027000003.json
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/41027000003.md
--rw-r--r--   0 runner    (1001) docker     (127)    16792 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/41123000005.json
--rw-r--r--   0 runner    (1001) docker     (127)    17301 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/41162000015.json
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/41162000015.md
--rw-r--r--   0 runner    (1001) docker     (127)    12899 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/41164000002.json
--rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/51011000042.json
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/51011000042.md
--rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/71211000027.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/71211000027.md
--rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/77795000000.json
--rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/81020000003.json
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/81020000003.md
--rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/81065000089.json
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/81065000089.md
--rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/85651000021.json
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/85651000021.md
--rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/87402000003.json
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/87402000003.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.644160 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)     3953 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json
--rw-r--r--   0 runner    (1001) docker     (127)     4165 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json
--rw-r--r--   0 runner    (1001) docker     (127)     4519 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json
--rw-r--r--   0 runner    (1001) docker     (127)     4892 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json
--rw-r--r--   0 runner    (1001) docker     (127)     3963 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json
--rw-r--r--   0 runner    (1001) docker     (127)     6489 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json
--rw-r--r--   0 runner    (1001) docker     (127)     4792 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json
--rw-r--r--   0 runner    (1001) docker     (127)     4655 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json
--rw-r--r--   0 runner    (1001) docker     (127)     4751 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json
--rw-r--r--   0 runner    (1001) docker     (127)     4629 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json
--rw-r--r--   0 runner    (1001) docker     (127)     4525 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json
--rw-r--r--   0 runner    (1001) docker     (127)     4232 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json
--rw-r--r--   0 runner    (1001) docker     (127)     3932 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json
--rw-r--r--   0 runner    (1001) docker     (127)     3739 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.644160 woningwaardering-0.3.0a7/tests/stelsels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.644160 woningwaardering-0.3.0a7/tests/stelsels/config/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/config/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.644160 woningwaardering-0.3.0a7/tests/stelsels/stelsel/
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.644160 woningwaardering-0.3.0a7/tests/stelsels/stelselgroep/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/test_ZelfstandigeWoonruimten.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.644160 woningwaardering-0.3.0a7/tests/stelsels/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/utils/test_import_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/utils/test_is_geldig.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/utils/test_vind_yaml_bestanden.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.644160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.648161 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.json
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.md
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json
--rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.md
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.648161 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_A++++_egw.json
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_egw.json
--rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_mgw.json
--rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/test_Energieprestatie.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.648161 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.648161 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.648161 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.648161 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.648161 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.648161 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/gedeelde_berging.md
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.md
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.md
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.648161 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.652161 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/bad.json
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/bad_en_douche.json
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/bidet.json
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/douche.json
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/geen_sanitair.json
--rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/lavet.json
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/toilet.json
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/twee_bad_en_douche.json
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/wastafel.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.652161 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/bad.json
--rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/bad_en_douche.json
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/bidet.json
--rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/douche.json
--rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/geen_sanitair.json
--rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/lavet.json
--rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/toilet.json
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/twee_bad_en_douche.json
--rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/wastafel.json
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/test_Sanitair.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.652161 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.656160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten_individueel.md
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.md
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten_individueel.md
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.628160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.656160 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.656160 woningwaardering-0.3.0a7/wettelijke-documenten/
--rw-r--r--   0 runner    (1001) docker     (127)   116885 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.656160 woningwaardering-0.3.0a7/woningwaardering/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-24 09:56:50.000000 woningwaardering-0.3.0a7/woningwaardering/_version.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.656160 woningwaardering-0.3.0a7/woningwaardering/stelsels/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.660161 woningwaardering-0.3.0a7/woningwaardering/stelsels/config/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/stelsel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/stelselgroep.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/stelselgroepversie.py
--rw-r--r--   0 runner    (1001) docker     (127)     8737 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.660161 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.660161 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py
--rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.660161 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/
--rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/bouwjaar_punten.csv
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_0-25m2_energielabel_punten.csv
--rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_25-40m2_energielabel_punten.csv
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_40m2+_energielabel_punten.csv
--rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oud_energielabel_punten.csv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.660161 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py
--rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.660161 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.660161 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/sanitair.py
--rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/sanitair_2024.py
--rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.664161 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py
--rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.632161 woningwaardering-0.3.0a7/woningwaardering/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.632161 woningwaardering-0.3.0a7/woningwaardering/templates/stelsels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.664161 woningwaardering-0.3.0a7/woningwaardering/templates/stelsels/stelsel/
--rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/templates/stelsels/stelsel/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.664161 woningwaardering-0.3.0a7/woningwaardering/templates/stelsels/stelsel/stelselgroep/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/templates/stelsels/stelsel/stelselgroep/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.664161 woningwaardering-0.3.0a7/woningwaardering/vera/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.664161 woningwaardering-0.3.0a7/woningwaardering/vera/bvg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/bvg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   137423 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/bvg/generated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.664161 woningwaardering-0.3.0a7/woningwaardering/vera/bvg/model_uitbreidingen/
--rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_energieprestatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/bvg/model_uitbreidingen/referentiedata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.700161 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/
--rw-r--r--   0 runner    (1001) docker     (127)    15108 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/aanbiedingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/accountstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/adressoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/afletterstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/afrekenwijzesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/afspraakstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/afwezigheidsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/aktesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/authentiekgegevenbron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/authentiekgegevensoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/bedrijfsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/begrotingversie.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/bestemming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/betaalgegevensoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/betaalwijzesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/betalingsregelingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/boekingdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/boekingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/boekingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/boekjaarstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    28284 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/brandwerendheidscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/btw.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/btwaangiftestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/burgerlijkestaat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/clustersoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/collectiefobjectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/communicatiekanaal.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/communicatierichting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/conditiescore.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/contactgegevensoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/contactgegevenstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/crediteursoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/crediteurstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/dagdeel.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/debiteursoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/debiteurstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/defectlocatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/defectoorzaak.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/defectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/defectstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/doelgroep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.700161 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/dossier/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/dossier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheiddetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheiddetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidinterieur.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidisolatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidligging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidmonument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidprijsconditie.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidsanitair.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eindedetailreden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eindereden.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.700161 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/energie/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/energie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/energielabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/energieprestatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/energieprestatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/externeincassosoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/externeincassostatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/factuurbetaalwijze.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/factuursoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.700161 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/financien/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/financien/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/gebeurtenissoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/geometriesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/geslacht.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/huurgeschilsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/huurgeschilstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/huurklasse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/huuropzeggingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/incassomoment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inexploitatiereden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/informatieobjectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inkomensbron.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inkomenssoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inschrijvingherkomst.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inspectierapportsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inspectierapportstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/kandidaatstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.700161 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/kwaliteit/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/kwaliteit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/kwaliteitsniveau.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/leningaflosvorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/leningdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/leningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/maatschappelijklabel.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/machtigingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    35393 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/materiaaldetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/materiaalsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/medewerkerrol.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/medewerkersoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/meeteenheid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.700161 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoud/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudslabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudspecialisme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/opleidingsniveau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/oppervlaktesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/opzegtermijn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.700161 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/organisatie/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/organisatie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/organisatievorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.700161 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/overeenkomsten/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/overeenkomstsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/overeenkomststatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/passendheiddetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/passendheidssoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/prestatieafspraak.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/prijscomponentsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.700161 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/projectontwikkeling/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/projectontwikkeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/projectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/projectstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/provincie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/publicatiedetailmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/publicatiedetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/publicatieintakevorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/publicatiemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/publicatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/puntenberekeningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/puntenmutatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/reclamatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/reclamatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/redenontbinding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/redenopzegging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/redenvernietiging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/regiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/relatieadressoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/relatiedetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/relatierolsoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.700161 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/relaties/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/relaties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/relatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/relatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/rentesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13384 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/ruimtedetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/ruimteligging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/ruimtesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/sanctiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/sanctiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/signaleringdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/signaleringsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/signaleringstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/taal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/uitexploitatiereden.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/uitvoerendesoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.700161 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/vastgoed/
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/vastgoed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/verantwoordingregime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/verbijzonderingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/verbijzonderingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/verrekeningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/vertrouwelijkheid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/voorrangdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/voorrangsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py
--rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/woningtype.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py
--rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.700161 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/woonruimteverdeling/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/woonsituatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/woonvorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/zaakobjectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/zaakrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/zaakstatussoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/zaaktypesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata_uitbreiding.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-24 09:56:46.000000 woningwaardering-0.3.0a7/woningwaardering/vera/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-24 09:56:50.700161 woningwaardering-0.3.0a7/woningwaardering.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    26709 2024-05-24 09:56:50.000000 woningwaardering-0.3.0a7/woningwaardering.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    25860 2024-05-24 09:56:50.000000 woningwaardering-0.3.0a7/woningwaardering.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-24 09:56:50.000000 woningwaardering-0.3.0a7/woningwaardering.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-24 09:56:50.000000 woningwaardering-0.3.0a7/woningwaardering.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-24 09:56:50.000000 woningwaardering-0.3.0a7/woningwaardering.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.504763 woningwaardering-0.4.0a0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.428762 woningwaardering-0.4.0a0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      324 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/.github/labeler.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.428762 woningwaardering-0.4.0a0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      211 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/.github/workflows/labeler.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3611 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    27046 2024-05-31 10:34:48.504763 woningwaardering-0.4.0a0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    25223 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.416762 woningwaardering-0.4.0a0/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.428762 woningwaardering-0.4.0a0/docs/afbeeldingen/
+-rw-r--r--   0 runner    (1001) docker     (127)    34043 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/docs/afbeeldingen/excel_viewer.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)   132221 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/docs/afbeeldingen/oppervlakte_van_vertrekken.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.416762 woningwaardering-0.4.0a0/docs/implementatietoelichting-beleidsboeken/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.428762 woningwaardering-0.4.0a0/docs/implementatietoelichting-beleidsboeken/2024/
+-rw-r--r--   0 runner    (1001) docker     (127)    51700 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1833 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.432762 woningwaardering-0.4.0a0/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     6514 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/scripts/genereer_opzet_woningwaarderinggroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2678 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/scripts/genereer_test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/scripts/genereer_vera_referentiedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/scripts/uitbreiden_vera_modellen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-31 10:34:48.504763 woningwaardering-0.4.0a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1349 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/taskfile.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.432762 woningwaardering-0.4.0a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.416762 woningwaardering-0.4.0a0/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.416762 woningwaardering-0.4.0a0/tests/data/input/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.432762 woningwaardering-0.4.0a0/tests/data/input/generiek/
+-rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/generiek/37101000032.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.436762 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/12006000004.json
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/12006000004.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/23003000050.json
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/23003000050.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/25048000007.json
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/25048000007.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/28018000044.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/28018000044.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/37101000032.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14864 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/41027000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/41027000003.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16699 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/41123000005.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17301 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/41162000015.json
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/41162000015.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12899 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/41164000002.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/51011000042.json
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/51011000042.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/71211000027.json
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/71211000027.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10718 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/77795000000.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13187 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/81020000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/81020000003.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/81065000089.json
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/81065000089.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/85651000021.json
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/85651000021.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/87402000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/87402000003.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.416762 woningwaardering-0.4.0a0/tests/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.416762 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.440762 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)     4506 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4719 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4026 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5072 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5445 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4516 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5346 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5208 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5305 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5182 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5078 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4785 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4485 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.440762 woningwaardering-0.4.0a0/tests/stelsels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.440762 woningwaardering-0.4.0a0/tests/stelsels/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/config/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.440762 woningwaardering-0.4.0a0/tests/stelsels/stelsel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.440762 woningwaardering-0.4.0a0/tests/stelsels/stelselgroep/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1108 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/test_ZelfstandigeWoonruimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.440762 woningwaardering-0.4.0a0/tests/stelsels/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      709 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/utils/test_import_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/utils/test_is_geldig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/utils/test_vind_yaml_bestanden.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.424762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.440762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.440762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.md
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.md
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.444762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_A++++_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_mgw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/test_Energieprestatie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.444762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.444762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/input/aanrecht_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/input/aanrecht_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/input/aanrecht_<1.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1102 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/input/aanrecht_en_wandafwerking.json
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/input/aanrecht_zonder_lengte.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/input/woon_slaap_met_aanrecht.json
+-rw-r--r--   0 runner    (1001) docker     (127)      270 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/input/woon_slaap_met_aanrecht.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.444762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/output/peildatum/2024-01-01/aanrecht_1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/output/peildatum/2024-01-01/aanrecht_2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/output/peildatum/2024-01-01/aanrecht_<1.json
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/output/peildatum/2024-01-01/aanrecht_en_wandafwerking.json
+-rw-r--r--   0 runner    (1001) docker     (127)      312 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/output/peildatum/2024-01-01/aanrecht_zonder_lengte.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1347 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/data/output/peildatum/2024-01-01/woon_slaap_met_aanrecht.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1851 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/keuken/test_Keuken.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.444762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.444762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.444762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.444762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.448763 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.448763 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/gedeelde_berging.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.448763 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.448763 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/bad.json
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/bad_en_douche.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/bidet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/douche.json
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/geen_sanitair.json
+-rw-r--r--   0 runner    (1001) docker     (127)      332 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/lavet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/toilet.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/twee_bad_en_douche.json
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/wastafel.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.420762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.452762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      454 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/bad.json
+-rw-r--r--   0 runner    (1001) docker     (127)      481 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/bad_en_douche.json
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/bidet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      457 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/douche.json
+-rw-r--r--   0 runner    (1001) docker     (127)      314 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/geen_sanitair.json
+-rw-r--r--   0 runner    (1001) docker     (127)      456 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/lavet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      467 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/toilet.json
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/twee_bad_en_douche.json
+-rw-r--r--   0 runner    (1001) docker     (127)      459 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/output/peildatum/2024-01-01/wastafel.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/test_Sanitair.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.452762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.424762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.452762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten_individueel.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten_individueel.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.424762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.424762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.452762 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.456762 woningwaardering-0.4.0a0/wettelijke-documenten/
+-rw-r--r--   0 runner    (1001) docker     (127)   116885 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.456762 woningwaardering-0.4.0a0/woningwaardering/
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-31 10:34:48.000000 woningwaardering-0.4.0a0/woningwaardering/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.456762 woningwaardering-0.4.0a0/woningwaardering/stelsels/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.456762 woningwaardering-0.4.0a0/woningwaardering/stelsels/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4692 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/stelsel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/stelselgroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/stelselgroepversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8737 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.456762 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.456762 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.460762 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/bouwjaar_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_0-25m2_energielabel_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_25-40m2_energielabel_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_40m2+_energielabel_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oud_energielabel_punten.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.460762 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/keuken/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/keuken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/keuken/keuken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6235 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/keuken/keuken_2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.460762 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8848 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.460762 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.460762 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/sanitair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6019 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/sanitair_2024.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7010 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.460762 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7474 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.424762 woningwaardering-0.4.0a0/woningwaardering/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.424762 woningwaardering-0.4.0a0/woningwaardering/templates/stelsels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.460762 woningwaardering-0.4.0a0/woningwaardering/templates/stelsels/stelsel/
+-rw-r--r--   0 runner    (1001) docker     (127)      412 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/templates/stelsels/stelsel/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.464763 woningwaardering-0.4.0a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.464763 woningwaardering-0.4.0a0/woningwaardering/vera/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.464763 woningwaardering-0.4.0a0/woningwaardering/vera/bvg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/bvg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137423 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/bvg/generated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.464763 woningwaardering-0.4.0a0/woningwaardering/vera/bvg/model_uitbreidingen/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_energieprestatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/bvg/model_uitbreidingen/referentiedata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.500763 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/
+-rw-r--r--   0 runner    (1001) docker     (127)    15108 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/aanbiedingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/accountstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      910 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/adressoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/afletterstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/afrekenwijzesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/afspraakstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/afwezigheidsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/aktesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/authentiekgegevenbron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/authentiekgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/bedrijfsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/begrotingversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/bestemming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/betaalgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/betaalwijzesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/betalingsregelingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/boekingdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/boekingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/boekingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/boekjaarstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28284 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/brandwerendheidscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/btw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/btwaangiftestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/burgerlijkestaat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/clustersoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/collectiefobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/communicatiekanaal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/communicatierichting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/conditiescore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/contactgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/contactgegevenstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/crediteursoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/crediteurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/dagdeel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/debiteursoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/debiteurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/defectlocatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/defectoorzaak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/defectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/defectstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/doelgroep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.500763 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/dossier/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/dossier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheiddetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheiddetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidinterieur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidisolatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidligging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidmonument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidprijsconditie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidsanitair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eindedetailreden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eindereden.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.500763 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/energie/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/energie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/energielabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/energieprestatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/energieprestatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/externeincassosoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/externeincassostatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/factuurbetaalwijze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/factuursoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.500763 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/financien/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/financien/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/gebeurtenissoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/geometriesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/geslacht.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/huurgeschilsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/huurgeschilstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/huurklasse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/huuropzeggingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/incassomoment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inexploitatiereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/informatieobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inkomensbron.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inkomenssoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inschrijvingherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inspectierapportsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inspectierapportstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/kandidaatstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.500763 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/kwaliteit/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/kwaliteit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/kwaliteitsniveau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/leningaflosvorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/leningdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/leningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/maatschappelijklabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/machtigingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35573 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/materiaaldetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/materiaalsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/medewerkerrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/medewerkersoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1992 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/meeteenheid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.500763 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoud/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudslabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudspecialisme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/opleidingsniveau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/oppervlaktesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/opzegtermijn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.500763 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/organisatie/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/organisatie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/organisatievorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.500763 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/overeenkomsten/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/overeenkomstsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/overeenkomststatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/passendheiddetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/passendheidssoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/prestatieafspraak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/prijscomponentsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.500763 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/projectontwikkeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/projectontwikkeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/projectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/projectstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/provincie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/publicatiedetailmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/publicatiedetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/publicatieintakevorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/publicatiemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/publicatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/puntenberekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/puntenmutatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/reclamatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/reclamatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/redenontbinding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/redenopzegging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/redenvernietiging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/regiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/relatieadressoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/relatiedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/relatierolsoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.500763 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/relaties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/relaties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/relatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/relatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/rentesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13384 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/ruimtedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/ruimteligging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/ruimtesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/sanctiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/sanctiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/signaleringdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/signaleringsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/signaleringstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/taal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/uitexploitatiereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/uitvoerendesoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.500763 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/vastgoed/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/vastgoed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/verantwoordingregime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/verbijzonderingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/verbijzonderingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/verrekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/vertrouwelijkheid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/voorrangdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/voorrangsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/woningtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.500763 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/woonruimteverdeling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/woonsituatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/woonvorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/zaakobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/zaakrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/zaakstatussoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/zaaktypesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata_uitbreiding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3557 2024-05-31 10:34:43.000000 woningwaardering-0.4.0a0/woningwaardering/vera/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-31 10:34:48.500763 woningwaardering-0.4.0a0/woningwaardering.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    27046 2024-05-31 10:34:48.000000 woningwaardering-0.4.0a0/woningwaardering.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27294 2024-05-31 10:34:48.000000 woningwaardering-0.4.0a0/woningwaardering.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-31 10:34:48.000000 woningwaardering-0.4.0a0/woningwaardering.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-31 10:34:48.000000 woningwaardering-0.4.0a0/woningwaardering.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-31 10:34:48.000000 woningwaardering-0.4.0a0/woningwaardering.egg-info/top_level.txt
```

### Comparing `woningwaardering-0.3.0a7/.github/workflows/cicd.yml` & `woningwaardering-0.4.0a0/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/.github/workflows/publish-to-pypi.yml` & `woningwaardering-0.4.0a0/.github/workflows/publish-to-pypi.yml`

 * *Files 10% similar despite different names*

```diff
@@ -85,48 +85,35 @@
     runs-on: ubuntu-latest
 
     permissions:
       contents: write # IMPORTANT: mandatory for making GitHub Releases
       id-token: write # IMPORTANT: mandatory for sigstore
 
     steps:
-      - name: Get latest release
-        shell: bash {0}
-        env:
-          GITHUB_TOKEN: ${{ github.token }}
-        id: latest-release
-        run: |
-          latestTagName=$(gh release view --repo '${{ github.repository }}' --jq .tagName --json tagName)
-          if [ "$latestTagName" == "" ]; then
-            echo "getting prerelease"
-            latestTagName=$(gh release list -L1 --repo '${{ github.repository }}' --json tagName --jq .[].tagName)
-          fi
-          echo "LATEST_TAG_NAME=$latestTagName" >> "$GITHUB_OUTPUT"
       - name: Download all the dists
         uses: actions/download-artifact@v4
         with:
           name: python-package-distributions
           path: dist/
       - name: Sign the dists with Sigstore
         uses: sigstore/gh-action-sigstore-python@v2.1.1
         with:
           inputs: >-
             ./dist/*.tar.gz
             ./dist/*.whl
       - name: Create GitHub Release
         env:
           GITHUB_TOKEN: ${{ github.token }}
-          LATEST_TAG_NAME: ${{ steps.latest-release.outputs.LATEST_TAG_NAME }}
         run: >-
           gh release create
           '${{ github.ref_name }}'
           --repo '${{ github.repository }}'
           ${{ (contains(github.ref_name, 'alpha') || contains(github.ref_name, 'beta') || contains(github.ref_name, 'rc')) && '--prerelease' || ''}}
           --generate-notes
-          --notes-start-tag $LATEST_TAG_NAME
+          --notes-start-tag $(gh release view --repo '${{ github.repository }}' --jq .tagName --json tagName)
       - name: Upload artifact signatures to GitHub Release
         env:
           GITHUB_TOKEN: ${{ github.token }}
         # Upload to GitHub Release using the `gh` CLI.
         # `dist/` contains the built packages, and the
         # sigstore-produced signatures and certificates.
         run: >-
```

### Comparing `woningwaardering-0.3.0a7/.gitignore` & `woningwaardering-0.4.0a0/.gitignore`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/.pre-commit-config.yaml` & `woningwaardering-0.4.0a0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/LICENSE` & `woningwaardering-0.4.0a0/LICENSE`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/PKG-INFO` & `woningwaardering-0.4.0a0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woningwaardering
-Version: 0.3.0a7
+Version: 0.4.0a0
 Summary: Berekent de punten van een woning op basis van het woningwaarderingsstelsel.
 Author-email: Woonstad Rotterdam <info@woonstadrotterdam.nl>, Ben Verhees <ben.verhees@woonstadrotterdam.nl>, Tiddo Loos <tiddo.loos@woonstadrotterdam.nl>, Tomer Gabay <tomer.gabay@woonstadrotterdam.nl>
 Project-URL: Homepage, https://github.com/woonstadrotterdam/woningwaardering
 Project-URL: Issues, https://github.com/woonstadrotterdam/woningwaardering/issues
 Keywords: woning,waardering,stelsel,woningwaarderingsstelsel,wws
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -348,13 +348,17 @@
 
 ### Eenheidklimaatbeheersingsoort
 
 Om te bepalen of de ruimten van een eenheid als individueel of collectief verwarmd gewaardeerd dienen te worden, mist de VERA standaard een veld voor de `Eenheidklimaatbeheersingsoort` referentiedata. Dit attribuut is toegevoegd aan `EenhedenEenheid`.  
 Om dit attribuut ook aan de VERA standaard toe te voegen is
 https://github.com/Aedes-datastandaarden/vera-openapi/issues/54 aangemaakt.
 
+### Bidet en Lavet
+
+In het beleidshandboek van de huurcomissie voor het woningwaardeeringstelsel wordt voor zowel een bidet als een lavet één punt toegekend. In de huidige referentiedata ontbreken deze twee type `bouwkundigelementdetailsoort`. Zie [dit issue](https://github.com/Aedes-datastandaarden/vera-referentiedata/issues/104).
+
 ### Verwarmd
 
 In de VERA standaard is nog geen mogelijkheid om aan te geven of een ruimte verwarmd is. Het attribuut `verwarmde_vertrekken_aantal` bestaat wel, maar dit bestaat op niveau van de eenheid en daarin bestaat geen onderscheid tussen vertrekken en overige ruimten. Dit is aangekaart in deze twee issues:
 
 - https://github.com/Aedes-datastandaarden/vera-openapi/issues/41
 - https://github.com/Aedes-datastandaarden/vera-referentiedata/issues/100
```

### Comparing `woningwaardering-0.3.0a7/README.md` & `woningwaardering-0.4.0a0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -309,13 +309,17 @@
 
 ### Eenheidklimaatbeheersingsoort
 
 Om te bepalen of de ruimten van een eenheid als individueel of collectief verwarmd gewaardeerd dienen te worden, mist de VERA standaard een veld voor de `Eenheidklimaatbeheersingsoort` referentiedata. Dit attribuut is toegevoegd aan `EenhedenEenheid`.  
 Om dit attribuut ook aan de VERA standaard toe te voegen is
 https://github.com/Aedes-datastandaarden/vera-openapi/issues/54 aangemaakt.
 
+### Bidet en Lavet
+
+In het beleidshandboek van de huurcomissie voor het woningwaardeeringstelsel wordt voor zowel een bidet als een lavet één punt toegekend. In de huidige referentiedata ontbreken deze twee type `bouwkundigelementdetailsoort`. Zie [dit issue](https://github.com/Aedes-datastandaarden/vera-referentiedata/issues/104).
+
 ### Verwarmd
 
 In de VERA standaard is nog geen mogelijkheid om aan te geven of een ruimte verwarmd is. Het attribuut `verwarmde_vertrekken_aantal` bestaat wel, maar dit bestaat op niveau van de eenheid en daarin bestaat geen onderscheid tussen vertrekken en overige ruimten. Dit is aangekaart in deze twee issues:
 
 - https://github.com/Aedes-datastandaarden/vera-openapi/issues/41
 - https://github.com/Aedes-datastandaarden/vera-referentiedata/issues/100
```

### Comparing `woningwaardering-0.3.0a7/docs/afbeeldingen/excel_viewer.png` & `woningwaardering-0.4.0a0/docs/afbeeldingen/excel_viewer.png`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw` & `woningwaardering-0.4.0a0/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/docs/afbeeldingen/oppervlakte_van_vertrekken.png` & `woningwaardering-0.4.0a0/docs/afbeeldingen/oppervlakte_van_vertrekken.png`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md` & `woningwaardering-0.4.0a0/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,254 +1,185 @@
 # 2024. Zelfstandige Woonruimten
 
 ## 4.2 Oppervlakte van Vertrekken
 
 ### 4.2.1 Wat zijn vertrekken?
 
-Het eerste onderdeel van de woningwaardering is de oppervlakte van vertrekken. Onder vertrek-
-ken worden woonkamer, andere kamers (hobbykamer, studeerkamer, slaapkamer en eetkamer),
-keuken, badkamer of doucheruimte verstaan. De waardering van vertrekken is 1 punt per m2.
-
-Geen vertrekken zijn: schuren, zolderberging, kelders, wasruimten, bijkeukens, garages en bergingen,
-gang, (speel)hal en zogenoemde verkeersruimten (bijvoorbeeld overlopen). De oppervlakte van
-deze ruimten tellen dus niet mee als vertrekken.
-De Huurcommissie geeft op een aantal punten nadere invulling aan de hierboven genoemde
-wettelijke begrippen. Dat wordt hierna beschreven.
+Het eerste onderdeel van de woningwaardering is de oppervlakte van vertrekken. Onder vertrekken worden woonkamer, andere kamers (hobbykamer, studeerkamer, slaapkamer en eetkamer), keuken, badkamer of doucheruimte verstaan. De waardering van vertrekken is 1 punt per m2.
 
-**Woonkamer of andere kamer**
+Geen vertrekken zijn: schuren, zolderberging, kelders, wasruimten, bijkeukens, garages en bergingen, gang, (speel)hal en zogenoemde verkeersruimten (bijvoorbeeld overlopen). De oppervlakte van deze ruimten tellen dus niet mee als vertrekken.  
 
-Een woonkamer of een andere kamer is dus een vertrek in de zin van het
-woningwaarderingsstelsel.
+De Huurcommissie geeft op een aantal punten nadere invulling aan de hierboven genoemde wettelijke begrippen. Dat wordt hierna beschreven.
+
+**Woonkamer of andere kamer**  
+Een woonkamer of een andere kamer is dus een vertrek in de zin van het woningwaarderingsstelsel.
 
 Hiervan is alleen sprake als:
 
 - ~~De vloer begaanbaar is.~~
 - ~~De muren en wanden uit vast materiaal bestaan.~~
 - ~~En de daglichttoetreding, de ventilatiemogelijkheid en het aantal elektrische lichtpunten in overeenstemming zijn met de geldende verkeersopvattingen.~~
 - De ruimte een oppervlakte heeft van minimaal 4 m2.
 - ~~De ruimte over de volle lengte ten minste 1,50 m breed is.~~
-- ~~De ruimte over ten minste 50% van de oppervlakte een vrije hoogte heeft van 2.10 m (gemeten
-  vanaf de vloer tot het zichtbare plafond).~~
-
-Alleen als aan al deze eisen is voldaan, wordt de (oppervlakte van de) woonruimte of andere
-kamer meegeteld als “vertrek”. Zo niet, dan wordt de oppervlakte meegeteld als “overige ruimte”
-(zie paragraaf 4.3.).
-Uitzondering hierop geldt voor de keuken: de eisen van minimaal 4 m2 en ~~minimaal 1,50 m
-breedte~~ gelden niet voor de keuken en verzetten zich er dus niet tegen om een keuken als “vertrek” aan te merken en overeenkomstig te waarderen.
+- ~~De ruimte over ten minste 50% van de oppervlakte een vrije hoogte heeft van 2.10 m (gemeten vanaf de vloer tot het zichtbare plafond).~~
 
-**Badkamer of doucheruimte**
+Alleen als aan al deze eisen is voldaan, wordt de (oppervlakte van de) woonruimte of andere kamer meegeteld als “vertrek”. Zo niet, dan wordt de oppervlakte meegeteld als “overige ruimte” (zie [paragraaf 4.3](#43-oppervlakte-van-overige-ruimten).).  
+Uitzondering hierop geldt voor de keuken: de eisen van minimaal 4 m2 en ~~minimaal 1,50 m breedte~~ gelden niet voor de keuken en verzetten zich er dus niet tegen om een keuken als “vertrek” aan te merken en overeenkomstig te waarderen.
 
+**Badkamer of doucheruimte**  
 Een badkamer of doucheruimte is dus een vertrek in de zin van het woningwaarderingsstelsel.
 
 Hiervan is alleen sprake als:
 
 - ~~De vloer begaanbaar is.~~
 - ~~De muren en wanden uit vast materiaal bestaan.~~
-- ~~En de ventilatiemogelijkheid en het aantal elektrische lichtpunten in overeenstemming zijn met
-  de geldende verkeersopvattingen.~~
+- ~~En de ventilatiemogelijkheid en het aantal elektrische lichtpunten in overeenstemming zijn met de geldende verkeersopvattingen.~~
 - ~~De ruimte over ten minste 50% van de oppervlakte een vrije hoogte heeft van 2,00 m. (gemeten vanaf de vloer tot het zichtbare plafond).~~
 
-~~Alleen als aan al deze eisen is voldaan, wordt de (oppervlakte van de) badkamer of doucheruimte
-meegeteld als “vertrek”. Zo niet, dan wordt de oppervlakte meegeteld als “overige ruimte” (zie
-verderop).~~
+~~Alleen als aan al deze eisen is voldaan, wordt de (oppervlakte van de) badkamer of doucheruimte meegeteld als “vertrek”. Zo niet, dan wordt de oppervlakte meegeteld als “overige ruimte” (zie verderop).~~
 
 > Hoewel de VERA-standaard een onderscheid maakt tussen badkamer, doucheruimte en badkamer/toilet (badkamer met toilet) beschouwen wij ieder van deze ruimtes indien zij een toilet bevatten als een badkamer met toilet, conform hoe de huurcommissie omgaat met deze ruimtes.. Zie ook [dit Github issue](https://github.com/Aedes-datastandaarden/vera-referentiedata/issues/96).
 
 Voor gecombineerde bad-/doucheruimte met toilet geldt een minimale oppervlakte van 0,64 m².
 
-> Elke Badkamer, Badkamer/toilet of Doucheruimte die als vertrek is aangemerkt wordt meegeteld als vertrek, tenzij onder aftrek van 1 m2 voor een in de ruimte geplaatst toilet de oppervlakte kleiner is dan 0,64 m². (Zie punt 5 in 4.2.2).
-
-**Zolderruimte**
+> Elke Badkamer, Badkamer/toilet of Doucheruimte die als vertrek is aangemerkt wordt meegeteld als vertrek, tenzij onder aftrek van 1 m2 voor een in de ruimte geplaatst toilet de oppervlakte kleiner is dan 0,64 m². (Zie punt 5 in [4.2.2](#422-hoe-wordt-de-oppervlakte-van-vertrekken-gemeten)).
 
-Zolderruimten zijn in het algemeen “overige ruimte”. Echter, in geval een zolderruimte een functie
-heeft als “vertrek” (dus woonkamer, andere kamers, badkamer of doucheruimte), en ook voldoet
-aan de eisen die daarvoor gelden (zie hierboven), dan mag de zolderruimte meetellen als “vertrek”,
-mits deze ruimte bereikbaar is via een vaste trap ~~en het dak beschoten is~~.
+**Zolderruimte**  
+Zolderruimten zijn in het algemeen “overige ruimte”. Echter, in geval een zolderruimte een functie heeft als “vertrek” (dus woonkamer, andere kamers, badkamer of doucheruimte), en ook voldoet aan de eisen die daarvoor gelden (zie hierboven), dan mag de zolderruimte meetellen als “vertrek”, mits deze ruimte bereikbaar is via een vaste trap ~~en het dak beschoten is~~.
 
 > In het beleidsboek wordt er onderscheid gemaakt tussen een zolder vertrek met een vaste trap of zolder met een ander soort trap. Wanneer een zolder als vertrek wordt aangemerkt moet deze te bereiken zijn via een vaste trap. Daarom wordt er voor een zolder gekeken of er een vaste trap in de `bouwkundige_elementen` zit. Als dit het geval is dan telt de gehele oppervlakte van de zolder mee voor de punten van Oppervlakte van Vertrekken.
 
 ### 4.2.2 Hoe wordt de oppervlakte van vertrekken gemeten?
 
-De wetgever heeft in de toelichting op het woningwaarderingsstelsel een aantal meetinstructies
-meegegeven:
+De wetgever heeft in de toelichting op het woningwaarderingsstelsel een aantal meetinstructies meegegeven:
 
-1. Meting van de oppervlakte van vertrekken vindt plaats ~~van muur tot muur, op een hoogte van
-   1,50 m boven de vloer,~~ inclusief de oppervlakte van alle tot de woning behorende losse en
-   vaste kasten (kleiner dan 2m²). ~~Deze meethoogte geldt ook als de oppervlakte afwijkt van die
-   op vloerniveau.~~
+1. Meting van de oppervlakte van vertrekken vindt plaats ~~van muur tot muur, op een hoogte van 1,50 m boven de vloer,~~ inclusief de oppervlakte van alle tot de woning behorende losse en vaste kasten (kleiner dan 2m²). ~~Deze meethoogte geldt ook als de oppervlakte afwijkt van die op vloerniveau.~~
 
 De Huurcommissie hanteert hierbij de volgende uitgangspunten.
 
-~~Als er sprake is van een pui wordt de binnenzijde van die pui (het kozijn) genomen. Een erker
-wordt meegerekend indien deze inwendig een vrije hoogte heeft van ten minste 1,50 m. Indien er
-sprake is van een zgn. entresol (tussenverdieping) dan dient de oppervlakte onder en/of boven
-deze entresol te worden meegerekend, indien de vrije hoogte ten minste 1,50m bedraagt.~~ Voor
-het meten van vertrekken die met elkaar in open verbinding staan, zie verderop.
-“Alle tot de woning behorende losse en vaste kasten” lees de Huurcommissie als: “alle tot de
-vertrekken behorende kasten”. De plaats van de deur van de kast bepaalt bij welk vertrek de kast
-behoort. Dus een kast die in een vertrek uitkomt wordt, ongeacht de afmeting, bij dat vertrek
-geteld. Dat geldt ook voor het waarderen van een kastenwand tussen twee vertrekken.
-
-- Van vaste kasten (kleiner dan 2m²) wordt de netto oppervlakte bepaald en bij de oppervlakte
-  van het betreffende vertrek opgeteld;
-- Een kast, (kleiner dan 2m²) waarvan de deur uitkomt op een verkeersruimte, wordt niet
-  gewaardeerd;
-- Losse kasten zijn niet van belang bij het meten. De oppervlakte van het vertrek wordt bepaald,
-  incl. de oppervlakte die wordt ingenomen door een losse kast;
+~~Als er sprake is van een pui wordt de binnenzijde van die pui (het kozijn) genomen. Een erker wordt meegerekend indien deze inwendig een vrije hoogte heeft van ten minste 1,50 m. Indien er sprake is van een zgn. entresol (tussenverdieping) dan dient de oppervlakte onder en/of boven deze entresol te worden meegerekend, indien de vrije hoogte ten minste 1,50m bedraagt.~~ Voor het meten van vertrekken die met elkaar in open verbinding staan, zie verderop.  
+“Alle tot de woning behorende losse en vaste kasten” lees de Huurcommissie als: “alle tot de vertrekken behorende kasten”. De plaats van de deur van de kast bepaalt bij welk vertrek de kast behoort. Dus een kast die in een vertrek uitkomt wordt, ongeacht de afmeting, bij dat vertrek geteld. Dat geldt ook voor het waarderen van een kastenwand tussen twee vertrekken.
+
+- Van vaste kasten (kleiner dan 2m²) wordt de netto oppervlakte bepaald en bij de oppervlakte van het betreffende vertrek opgeteld;
+- Een kast, (kleiner dan 2m²) waarvan de deur uitkomt op een verkeersruimte, wordt niet gewaardeerd;
+- Losse kasten zijn niet van belang bij het meten. De oppervlakte van het vertrek wordt bepaald, incl. de oppervlakte die wordt ingenomen door een losse kast;
 
 > Binnen het woningwaarderingsstelsel mag onder bepaalde voorwaarden de oppervlakte van vaste kasten worden opgeteld bij de ruimte waar de deur van de kast zich bevindt. Als hier bij het inmeten geen rekening mee gehouden is, kan het attribuut `verbonden_ruimten` gebruikt worden om de met een ruimte verbonden vaste kasten mee te laten nemen in de waardering. Hiervoor is de VERA referentiedata binnen deze repository uitgebreid met ruimtedetailsoort Kast, code KAS.
 
-2. ~~Als oppervlakte van een vertrek met een (ten dele) hellend of verlaagd plafond geldt dat
-   alleen het gedeelte waarboven het plafond ten minste 1,50m hoog is wordt meegeteld bij de
-   berekening van de oppervlakte.~~
-
-~~De Huurcommissie eist in geval van een (ten dele) hellend plafond dat de 1,50m-hoogte loopt tot
-het dakbeschot of tot het zichtbare dakvlak of plafond. Met gordingen en balken wordt bij de
-meting geen rekening gehouden.~~
-
-3. ~~De vloeroppervlakte onder aanrechten, toestellen in de keuken, badkuip, lavet of douchebak,
-   moederhaard, c.v.-ketel en boilerinstallatie, wordt meegeteld.~~
-
-~~De Huurcommissie gaat hier als volgt mee om. Indien zich in een vertrek, of in een kast in een
-vertrek, een gas- en/of elektrameter bevindt, dan wordt de oppervlakte gewaardeerd onder aftrek
-van 30 x 60 cm (minimale afmeting meterkast bestaande bouw).
-De vloeroppervlakte onder radiatoren wordt meegeteld.~~
-
-4. ~~De oppervlakte die wordt ingenomen door schoorsteenkanalen, ventilatiekanalen of stand- of
-   grondleidingen (tenzij horizontale leidingen, zie hierna) wordt niet meegeteld.~~
-
-~~Bij een schoorsteenmantel en/of rookkanaal (die naar boven of beneden breed kan uitlopen) is de
-oppervlakte op 1,50m-hoogte bepalend. De oppervlakte die wordt ingenomen door standleidin-
-gen (verticale leidingen) wordt niet meegeteld.
-De oppervlakte die wordt ingenomen door grondleidingen (horizontale leidingen), wordt wel
-meegeteld.~~
-
-5. Indien een toilet in een badruimte of doucheruimte is geplaatst, wordt de oppervlakte van die
-   ruimte met één vierkante meter verminderd.
-
-6. ~~Van de oppervlakte onder een open dan wel gesloten vaste trap geldt dat gedeelte waar de
-   ruimte tussen vloer en onderkant trap ten minste 1,50m hoog is.~~
-
-7. Afronding van de oppervlakte op hele vierkante meters vindt plaats na saldering van de
-   oppervlakte van alle vertrekken; bij 0,5m² of meer wordt afgerond naar boven, bij minder dan
-   0,5m² naar beneden. Waardering in punten vindt na saldering en afronding plaats.
-
-De Huurcommissie licht dit als volgt toe:
-Afronding: eerst de oppervlakte per vertrek op 2 decimalen afronden en pas daarna de oppervlak-
-te van alle vertrekken salderen en afronden op hele vierkante meters.
-
-**Voorbeeld:**  
-kamer : lengte 3,76m x breedte 4,12m = 15,4912 m², afgerond : 15,49 m²  
-keuken: lengte 2,95m x breedte 3,81m = 11,2395 m², afgerond : 11,24 m²  
-Totaal : 26,73 m² Afronding op hele m² : 27 m².
-
-8. ~~Twee vertrekken die met elkaar in verbinding staan, worden in een bepaald geval als één
-   vertrek gewaardeerd. Dit is het geval als zich tussen die twee vertrekken een opening bevindt,
-   die breder is dan 50% van de muur, waarin deze opening zich bevindt (zie schets hieronder).
-   Het moet hierbij gaan om een niet afsluitbare opening, die doorloopt tot aan de vloer. De muur
-   wordt gemeten in het vertrek, waarin de tussenwand het smalst is.~~
+2. ~~Als oppervlakte van een vertrek met een (ten dele hellend of verlaagd plafond geldt dat alleen het gedeelte waarboven het plafond ten minste 1,50m hoog is wordt meegeteld bij de berekening van de oppervlakte.~~
+
+~~De Huurcommissie eist in geval van een (ten dele) hellend plafond dat de 1,50m-hoogte loopt tot het dakbeschot of tot het zichtbare dakvlak of plafond. Met gordingen en balken wordt bij de meting geen rekening gehouden.~~
+
+3. ~~De vloeroppervlakte onder aanrechten, toestellen in de keuken, badkuip, lavet of douchebak, moederhaard, c.v.-ketel en boilerinstallatie, wordt meegeteld.~~
+
+~~De Huurcommissie gaat hier als volgt mee om. Indien zich in een vertrek, of in een kast in een vertrek, een gas- en/of elektrameter bevindt, dan wordt de oppervlakte gewaardeerd onder aftrek van 30 x 60 cm (minimale afmeting meterkast bestaande bouw). De vloeroppervlakte onder radiatoren wordt meegeteld.~~
+
+4. ~~De oppervlakte die wordt ingenomen door schoorsteenkanalen, ventilatiekanalen of stand- of grondleidingen (tenzij horizontale leidingen, zie hierna) wordt niet meegeteld.~~
+
+~~Bij een schoorsteenmantel en/of rookkanaal (die naar boven of beneden breed kan uitlopen) is de oppervlakte op 1,50m-hoogte bepalend. De oppervlakte die wordt ingenomen door standleidingen (verticale leidingen) wordt niet meegeteld. De oppervlakte die wordt ingenomen door grondleidingen (horizontale leidingen), wordt wel meegeteld.~~
+
+5. Indien een toilet in een badruimte of doucheruimte is geplaatst, wordt de oppervlakte van die ruimte met één vierkante meter verminderd.
+
+6. ~~Van de oppervlakte onder een open dan wel gesloten vaste trap geldt dat gedeelte waar de ruimte tussen vloer en onderkant trap ten minste 1,50m hoog is.~~
+
+7. Afronding van de oppervlakte op hele vierkante meters vindt plaats na saldering van de oppervlakte van alle vertrekken; bij 0,5m² of meer wordt afgerond naar boven, bij minder dan 0,5m² naar beneden. Waardering in punten vindt na saldering en afronding plaats.
+
+De Huurcommissie licht dit als volgt toe:  
+
+Afronding: eerst de oppervlakte per vertrek op 2 decimalen afronden en pas daarna de oppervlakte van alle vertrekken salderen en afronden op hele vierkante meters.
+
+**_Voorbeeld:_**  
+_kamer : lengte 3,76m x breedte 4,12m = 15,4912 m², afgerond : 15,49 m²_  
+_keuken: lengte 2,95m x breedte 3,81m = 11,2395 m², afgerond : 11,24 m²_  
+_Totaal : 26,73 m² Afronding op hele m² : 27 m²._
+
+8. ~~Twee vertrekken die met elkaar in verbinding staan, worden in een bepaald geval als één vertrek gewaardeerd. Dit is het geval als zich tussen die twee vertrekken een opening bevindt, die breder is dan 50% van de muur, waarin deze opening zich bevindt (zie schets hieronder). Het moet hierbij gaan om een niet afsluitbare opening, die doorloopt tot aan de vloer. De muur wordt gemeten in het vertrek, waarin de tussenwand het smalst is.~~
+
+## 4.3 Oppervlakte van overige ruimten
+
+### 4.3.1 Wat zijn overige ruimten?
+
+“Overige ruimten” die voor een puntenwaardering in aanmerking komen zijn:  
+
+a. bijkeukens  
+b. bergingen  
+c. wasruimte  
+d. schuren  
+e. garages  
+f. zolderbergingen  
+g. kelders  
+~~h. parkeerplaats (zie paragraaf 4.9.6)~~
+
+> parkeerplaats wordt geïmplementeerd bij het implementeren van 4.9 (privé-buitenruimten).
+
+Deze ruimten tellen alleen mee als de oppervlakte van een ruimte afzonderlijk gelijk is aan of groter dan twee vierkante meter, ~~voor zover de plafondhoogte ten minste 1,50 meter is boven de vloer.~~  
+
+Verkeersruimten zoals hallen, gangen, en overlopen worden sowieso niet afzonderlijk gewaardeerd, dus krijgen geen punten op basis van dit onderdeel van het woningwaarderingsstelsel.
 
+Tot bergingen worden de volgende ruimten gerekend: vaste kasten, bergingen in, achter, voor, dan wel onder de woning, bergingen onder de kap van etagewoningen, bergingen in flatgebouwen en dergelijke, mits deze een afzonderlijke ruimte vormen.
 
 ### 4.3.2 Hoe wordt de oppervlakte van overige ruimte gemeten?
+
 De wetgever heeft een aantal eisen en meetinstructies meegegeven:
+
 1. ~~De ruimten worden slechts als “overige oppervlakte” gewaardeerd, als de vloer begaanbaar is.~~
-   
-2. ~~Van de overige ruimten wordt de gehele oppervlakte gemeten, dus zonder aftrek van loop- of
-verkeersruimte. De oppervlakte van een trapgat wordt wel in mindering gebracht. De oppervlakte die een uitschuifbare of opvouwbare trap in gesloten toestand inneemt, wordt van de
-oppervlakte van de ruimte afgetrokken.~~
-
-3. ~~Meting van de oppervlakte vindt plaats van muur tot muur, op een hoogte van 1,50m boven
-de vloer. En ook inclusief de oppervlakte van de moederhaard, CV-ketel en boilerinstallatie.
-Maar niet: de oppervlakte die wordt ingenomen door schoorsteenkanalen, ventilatiekanalen of
-stand- of grondleidingen.~~
-
-~~De Huurcommissie meet als er sprake is van een pui, vanaf de binnenzijde van die pui (het kozijn).
-Ook een erker, die inwendig een vrije hoogte heeft van ten minste 1,50m, telt mee. De oppervlakte
-onder en/of boven een zogenaamde entresol (tussenverdieping) wordt meegerekend, indien de
-hoogte minstens 1,50m bedraagt.~~
-
-~~De Huurcommissie berekent de hoogte van 1,50 meter door te meten tot het dakbeschot, het
-zichtbare dakvlak of plafond (gordingen en balken blijven buiten de meting).~~
-
-4. Ook de oppervlakte van alle tot de woning behorende losse en vaste kasten (kleiner dan 2m²)
-wordt meegerekend.
-
-Losse kasten zijn niet van belang bij het meten. De oppervlakte van de overige ruimte wordt
-bepaald, incl. de oppervlakte die wordt ingenomen door een losse kast.
-Van vaste kasten (kleiner dan 2m²) die uitkomen in een wel gewaardeerde overige ruimte wordt
-de netto oppervlakte bepaald en bij de oppervlakte opgeteld.
-Een kast, (kleiner dan 2m²) waarvan de deur uitkomt op een verkeersruimte, wordt niet
-gewaardeerd.
-
-~~Indien zich in een overige ruimte, of een kast in een overige ruimte, een gas- en/of elektrameter
-bevindt, dan wordt de oppervlakte gewaardeerd onder aftrek van 30 x 60 cm (minimale afmeting
-meterkast bestaande bouw).~~
+
+2. ~~Van de overige ruimten wordt de gehele oppervlakte gemeten, dus zonder aftrek van loop- of verkeersruimte. De oppervlakte van een trapgat wordt wel in mindering gebracht. De oppervlakte die een uitschuifbare of opvouwbare trap in gesloten toestand inneemt, wordt van de oppervlakte van de ruimte afgetrokken.~~
+
+3. ~~Meting van de oppervlakte vindt plaats van muur tot muur, op een hoogte van 1,50m boven de vloer. En ook inclusief de oppervlakte van de moederhaard, CV-ketel en boilerinstallatie. Maar niet: de oppervlakte die wordt ingenomen door schoorsteenkanalen, ventilatiekanalen of stand- of grondleidingen.~~
+
+~~De Huurcommissie meet als er sprake is van een pui, vanaf de binnenzijde van die pui (het kozijn). Ook een erker, die inwendig een vrije hoogte heeft van ten minste 1,50m, telt mee. De oppervlakte onder en/of boven een zogenaamde entresol (tussenverdieping) wordt meegerekend, indien de hoogte minstens 1,50m bedraagt.~~
+
+~~De Huurcommissie berekent de hoogte van 1,50 meter door te meten tot het dakbeschot, het zichtbare dakvlak of plafond (gordingen en balken blijven buiten de meting).~~
+
+4. Ook de oppervlakte van alle tot de woning behorende losse en vaste kasten (kleiner dan 2m²) wordt meegerekend.
+
+Losse kasten zijn niet van belang bij het meten. De oppervlakte van de overige ruimte wordt bepaald, incl. de oppervlakte die wordt ingenomen door een losse kast.  
+Van vaste kasten (kleiner dan 2m²) die uitkomen in een wel gewaardeerde overige ruimte wordt de netto oppervlakte bepaald en bij de oppervlakte opgeteld.  
+Een kast, (kleiner dan 2m²) waarvan de deur uitkomt op een verkeersruimte, wordt niet gewaardeerd.
+
+~~Indien zich in een overige ruimte, of een kast in een overige ruimte, een gas- en/of elektrameter bevindt, dan wordt de oppervlakte gewaardeerd onder aftrek van 30 x 60 cm (minimale afmeting meterkast bestaande bouw).~~
 
 5. ~~De Huurcommissie telt de vloeroppervlakte onder radiatoren ook mee.~~  
 
-~~Voor een schoorsteenmantel en/of rookkanaal (die naar boven of beneden breed kan uitlopen)
-vindt de Huurcommissie de oppervlakte op 1,50m-hoogte bepalend.~~
+~~Voor een schoorsteenmantel en/of rookkanaal (die naar boven of beneden breed kan uitlopen) vindt de Huurcommissie de oppervlakte op 1,50m-hoogte bepalend.~~
+
+6. ~~Van de oppervlakte onder een vaste (open of gesloten) trap, telt mee dat gedeelte waar de ruimte tussen vloer en onderkant trap ten minste 1,50m hoog is.~~
+
+7. ~~De oppervlakte die door een in ingeschoven toestand liggende inschuifbare of opvouwbare trap wordt ingenomen, wordt niet meegeteld.~~
+
+8. Betreft het een zolderberging dan wordt ~~, naast de eis van een begaanbare vloer,~~ als voorwaarde gesteld, ~~dat het dak beschoten is en~~ dat de zolderruimte via een tot de woning behorende trap bereikbaar is. Indien aan deze voorwaarden niet is voldaan, tellen zolderber gingen bij de woningwaardering niet mee.
 
-6. ~~Van de oppervlakte onder een vaste (open of gesloten) trap, telt mee dat gedeelte waar de
-ruimte tussen vloer en onderkant trap ten minste 1,50m hoog is.~~
+Indien geen vaste trap aanwezig is, wordt het aantal punten van de vloeroppervlakte van de zolderruimte met 5 verminderd, doch niet met meer punten dan voor de oppervlakte van de zolderruimten wordt gegeven.
 
-7. ~~De oppervlakte die door een in ingeschoven toestand liggende inschuifbare of opvouwbare
-trap wordt ingenomen, wordt niet meegeteld.~~
+~~Is er op de zolderverdieping ook nog een vertrek aanwezig dat alleen bereikbaar is via het zoldergedeelte dan wordt de oppervlakte van het zoldergedeelte verminderd met de loopruimte om het vertrek te bereiken. De dan resterende zolderoppervlakte dient minimaal 2 m2 te bedragen en wordt dan gewaardeerd als overige ruimte.~~
 
-8. Betreft het een zolderberging dan wordt ~~, naast de eis van een begaanbare vloer,~~ als voor-
-waarde gesteld, ~~dat het dak beschoten is en~~ dat de zolderruimte via een tot de woning
-behorende trap bereikbaar is. Indien aan deze voorwaarden niet is voldaan, tellen zolderber-
-gingen bij de woningwaardering niet mee.
-
-Indien geen vaste trap aanwezig is, wordt het aantal punten van de vloeroppervlakte van de
-zolderruimte met 5 verminderd, doch niet met meer punten dan voor de oppervlakte van de
-zolderruimten wordt gegeven.
-
-~~Is er op de zolderverdieping ook nog een vertrek aanwezig dat alleen bereikbaar is via het zolder-
-gedeelte dan wordt de oppervlakte van het zoldergedeelte verminderd met de loopruimte om het
-vertrek te bereiken. De dan resterende zolderoppervlakte dient minimaal 2 m2 te bedragen en
-wordt dan gewaardeerd als overige ruimte.~~
-
-> Wanneer een zolder als overige ruimte wordt beschouwd, kijken we in de `bouwkundige_elementen` van de zolder of de zolder bereikbaar is via een trap. Wanneer deze bereikbaar is via een vaste trap telt de volledige oppervlakte mee voor de punten berekening van Oppervlakte van Overige ruimten.
-Wanneer deze wel bereikbaar is, maar niet via een vaste trap, moeten er 5 punten in mindering worden gebracht omdat de ruimte niet bereikt kan worden met een vaste trap. In onze implementatie hebben wij er voor gekozen om te checken of er dan wel een vlizotrap aanwezig is in de `bouwkundige_elementen`, aangezien dit de enige andere soort trap in het VERA model is waarmee een zolder ruimte bereikt zou kunnen worden.
-Daarnaast is het onze keuze om de 5 punten in mindering te brengen door de oppervlakte van de zolder te corrigeren. Het beleidsboek
-geeft aan dat de punten in mindering gebracht moeten worden
-op de punten berekend voor deze ruimte. Maar ook dat punten
-pas berekend moeten worden wanneer de totale oppervlakte van een eenheid bekend is en afgerond is.
-Dit is tegenstrijdig en daarom kiezen wij de implementatie die volgens ons het beleidsboek zo goed mogelijk benadert.
-Let op, door de afronding komt deze berekening niet helemaal juist
-uit, maar dit is de benadering waar wij nu voor kiezen.
-
-9. Een overloop is een verkeersruimte en wordt dus niet gewaardeerd. ~~Als er met aftrek van de
-verkeersruimte en trap voldoende ruimte overblijft en deze (zolder)overloop kennelijk ook
-bedoeld is als bergruimte, dan wordt deze ruimte wel gewaardeerd.~~
+> Wanneer een zolder als overige ruimte wordt beschouwd, kijken we in de `bouwkundige_elementen` van de zolder of de zolder bereikbaar is via een trap. Wanneer deze bereikbaar is via een vaste trap telt de volledige oppervlakte mee voor de punten berekening van Oppervlakte van Overige ruimten. Wanneer deze wel bereikbaar is, maar niet via een vaste trap, moeten er 5 punten in mindering worden gebracht omdat de ruimte niet bereikt kan worden met een vaste trap. In onze implementatie hebben wij er voor gekozen om te checken of er dan wel een vlizotrap aanwezig is in de `bouwkundige_elementen`, aangezien dit de enige andere soort trap in het VERA model is waarmee een zolder ruimte bereikt zou kunnen worden. Daarnaast is het onze keuze om de 5 punten in mindering te brengen door de oppervlakte van de zolder te corrigeren. Het beleidsboek geeft aan dat de punten in mindering gebracht moeten worden op de punten berekend voor deze ruimte. Maar ook dat punten pas berekend moeten worden wanneer de totale oppervlakte van een eenheid bekend is en afgerond is. Dit is tegenstrijdig en daarom kiezen wij de implementatie die volgens ons het beleidsboek zo goed mogelijk benadert. Let op, door de afronding komt deze berekening niet helemaal juist uit, maar dit is de benadering waar wij nu voor kiezen.
+
+9. Een overloop is een verkeersruimte en wordt dus niet gewaardeerd. ~~Als er met aftrek van de verkeersruimte en trap voldoende ruimte overblijft en deze (zolder)overloop kennelijk ook bedoeld is als bergruimte, dan wordt deze ruimte wel gewaardeerd.~~
 
 10. Gemeenschappelijke bergingen worden gewaardeerd als overige ruimte als:
+
 - ~~zij binnen het woongebouw liggen of tot de onroerende aanhorigheden behoren;~~
 - ~~de vergoeding daarvoor in de huurprijs van de woning is begrepen;~~
 - de oppervlakte, na deling door het aantal woningen, per woning minstens 2m2 bedraagt.
 
 > Hiervoor is het `EenhedenRuimte` model uitgebreid met het attribuut `gedeeldMetAantalEenheden` of `gedeeld_met_aantal_eenheden` voor de Python representatie. Om deze berekening correct uit te voeren dient deze waarde gevuld te zijn. Zonder deze waarde wordt de volledige oppervlakte van een ruimte meegeteld.
 
-De toekenning van punten bij een gemeenschappelijke berging is als volgt: totale oppervlakte,
-afronden in m2, delen door het aantal woningen en waarderen als “overige ruimte”. Kasten <2m2
-en uitkomend in een verkeersruimte worden niet meegeteld.
-
-11.  Afronding van de oppervlakte op hele vierkante meters vindt plaats na saldering van de
-oppervlakte van alle afzonderlijke ruimten; bij 0,5m² of meer wordt afgerond naar boven, bij
-minder dan 0,5m² naar beneden. Waardering in punten vindt na saldering en afronding plaats.
-
-De Huurcommissie licht dit als volgt toe:
-Afronding: eerst de oppervlakte per overige ruimte op 2 decimalen afronden en pas daarna de
-oppervlakte van alle overige ruimten salderen en afronden op hele vierkante meters.
-
-**Voorbeeld:**  
-Garage : lengte 3,16m x breedte 6,12m = 19,3392 m², afgerond : 19,34 m²  
-Bijkeuken: lengte 2,11m x breedte 2,87m = 6,0557 m², afgerond : 6,06 m²  
-Totaal : 25,40 m² Afronding op hele m² : 25 m².  
+De toekenning van punten bij een gemeenschappelijke berging is als volgt: totale oppervlakte, afronden in m2, delen door het aantal woningen en waarderen als “overige ruimte”. Kasten <2m2 en uitkomend in een verkeersruimte worden niet meegeteld.
+
+1. Afronding van de oppervlakte op hele vierkante meters vindt plaats na saldering van de oppervlakte van alle afzonderlijke ruimten; bij 0,5m² of meer wordt afgerond naar boven, bij minder dan 0,5m² naar beneden. Waardering in punten vindt na saldering en afronding plaats.
+
+De Huurcommissie licht dit als volgt toe:  
+Afronding: eerst de oppervlakte per overige ruimte op 2 decimalen afronden en pas daarna de oppervlakte van alle overige ruimten salderen en afronden op hele vierkante meters.
+
+**_Voorbeeld:_**  
+_Garage : lengte 3,16m x breedte 6,12m = 19,3392 m², afgerond : 19,34 m²_  
+_Bijkeuken: lengte 2,11m x breedte 2,87m = 6,0557 m², afgerond : 6,06 m²_  
+_Totaal : 25,40 m² Afronding op hele m² : 25 m²._  
 
 ## 4.4 Verwarming
 
 Het waarderingsstelsel kent punten toe voor verwarming. Hierbij gelden de volgende regels.
 
 ### 4.4.1 Punten voor verwarmde vertrekken en overige ruimtes
 
@@ -295,34 +226,29 @@
 
 Ook een aanrecht dat is geplaatst in een woon- of slaapvertrek is een open keuken, ook als er geen duidelijke afscheiding tussen keukengedeelte en de rest van het vertrek aanwezig is.
 
 > Om een aanrecht in een woon- of slaapvertrek te waarderen als open keuken, moet de ruimte gespecificeerd worden met detailsoortcode `WOK` voor Woonkamer/keuken. Alternatief kan er in de bouwkundige elementen van een `Woonkamer`, `Slaapkamer` of `Woon-/slaapkamer` een bouwkundig element worden gespecificeerd met detailsoortcode `AAN` voor Aanrecht.
 
 ## 4.5 Energieprestatie
 
-Een (groot) deel van het totale puntenaantal wordt bepaald door de energieprestatie van de
-woonruimte. Sinds 2011 speelt het energielabel een rol in het puntenstelsel, waarbi een energielabel of energie-index maximaal 10 jaar geldig is. De energieprestatie kan sinds 1 januari 2021 op
-drie manieren zin bepaald.
-1. Een oud energielabel: registratie heeft plaatsgevonden vóór 1 januari 2015. In 2021 en later
-lopen veel sinds 1 juli 2011 verstrekte energielabels af, want de geldigheidsduur is tien jaar.
-2. De energie-index: registratie op of na 1 januari 2015 tot 1 januari 2021. In 2025 en later lopen
-veel sinds 1 januari 2015 verstrekte energie-indexen af, want de geldigheidsduur is tien jaar.
+Een (groot) deel van het totale puntenaantal wordt bepaald door de energieprestatie van de woonruimte. Sinds 2011 speelt het energielabel een rol in het puntenstelsel, waarbi een energielabel of energie-index maximaal 10 jaar geldig is. De energieprestatie kan sinds 1 januari 2021 op drie manieren zin bepaald.
+
+1. Een oud energielabel: registratie heeft plaatsgevonden vóór 1 januari 2015. In 2021 en later lopen veel sinds 1 juli 2011 verstrekte energielabels af, want de geldigheidsduur is tien jaar.
+2. De energie-index: registratie op of na 1 januari 2015 tot 1 januari 2021. In 2025 en later lopen veel sinds 1 januari 2015 verstrekte energie-indexen af, want de geldigheidsduur is tien jaar.
 3. Het energielabel op basis van primair fossiel energiegebruik: registratie op of na 1 januari 2021.
 
 In [EP-online](https://www.ep-online.nl/) is te vinden wat de energieprestatie van een woning is.
 
 > In de implemenatie is de combinatie `Energieprestatiesoort` met registratiedatum leidend om te beslissen welke lookup tabellen er worden gebruikt om na te gaan hoeveel punten er gegeven moeten worden voor het stelselgroep energieprestatie.
 
 > In de tabellen ter ondersteuning van de tekst van het beleidsboek over de punten toekenning bij een nieuw energielabel is er voor gekozen om de implementatie van regel [4.5.3 Afwijkingsbevoegdheid hogere energielabelklasse dan A++](#453-afwijkingsbevoegdheid-hogere-energielabelklasse-dan-a) al toe te voegen aan de tabellen.
 
 ### 4.5.1 Puntentoekenning oud energielabel en energie-index
-Bij een oud energielabel bepaalt de labelklasse (A t/m G) het aantal punten dat de verhuurder
-mag doorrekenen in de maximale huur. Een energielabel dat is geregistreerd vóór 2015 en dat niet
-ouder is dan tien jaar, is nog bruikbaar.
-~~Bij een energie-index is de indeling in letters vervangen door een cijfer. De energie-index wordt meegenomen indien in EP-online staat aangegeven dat de energie-index geldig is voor het woningwaarderingsstelsel.~~
+
+Bij een oud energielabel bepaalt de labelklasse (A t/m G) het aantal punten dat de verhuurder mag doorrekenen in de maximale huur. Een energielabel dat is geregistreerd vóór 2015 en dat niet ouder is dan tien jaar, is nog bruikbaar. ~~Bij een energie-index is de indeling in letters vervangen door een cijfer. De energie-index wordt meegenomen indien in EP-online staat aangegeven dat de energie-index geldig is voor het woningwaarderingsstelsel.~~
 
 > De energie-index van een energieprestatie wordt niet gebruikt. In EP-Online hebben alle op energie-index gebaseerde energieprestaties ook een labelklasse. Deze labelklasse dient gebruikt te worden voor de waardering.
 
 Zie hieronder de puntentoekenning van de energieprestatie bij een oud energielabel en een energie-index.
 
 | (oude) Energielabel (afgegeven voor 1-1-2025)| Energie-index (afgegeven na 1-1-2025)| Eengezinswoning | Meergezinswoning |
 | ----- | ------------- | --------------- | ----------------- |
@@ -334,21 +260,18 @@
 | D     | 1.8-2.1       | 14             | 11               |
 | E     | 2.1-2.4       | 8              | 5                |
 | F     | 2.4-2.7       | 4              | 1                |
 | G     | 2.7-          | 0              | 0                |
 
 ### 4.5.2 Puntentoekenning nieuw energielabel
 
-Per 1 januari 2021 geldt een nieuwe manier om de energieprestatie van een woonruimte te
-bepalen met een vernieuwd energielabel.
-Hierbij wordt gewerkt met een bepalingsmethode (NTA 8800) die een nieuwe indicator heeft voor de energieprestatie (in kWh/m2 per jaar).
-De uitkomst van de bepalingsmethode (NTA 8800) wordt gereduceerd tot een energielabel (van A++ tot G).
-Dit label wordt herleid tot punten voor het waarderingsstelsel.
-Aangezien de nieuwe bepalingsmethode tot structurele onderwaardering van de energieprestatie van kleine woningen leidt, wordt er in het kader van het nieuwe energielabel gewerkt met drie klassen met WWS-punten voor de energieprestatie.
-Dit is afhankelijk van de woninggrootte:
+Per 1 januari 2021 geldt een nieuwe manier om de energieprestatie van een woonruimte te bepalen met een vernieuwd energielabel. Hierbij wordt gewerkt met een bepalingsmethode (NTA 8800) die een nieuwe indicator heeft voor de energieprestatie (in kWh/m2 per jaar). De uitkomst van de bepalingsmethode (NTA 8800) wordt gereduceerd tot een energielabel (van A++ tot G). Dit label wordt herleid tot punten voor het waarderingsstelsel.  
+
+Aangezien de nieuwe bepalingsmethode tot structurele onderwaardering van de energieprestatie van kleine woningen leidt, wordt er in het kader van het nieuwe energielabel gewerkt met drie klassen met WWS-punten voor de energieprestatie. Dit is afhankelijk van de woninggrootte:
+
 - \< 25 m2
 - \> 25 m2 en < 40 m2
 - \> 40 m2
 
 > De hier gehanteerde woninggrootte wordt op een andere wijze bepaald dan de gebruiksoppervlakte. Hiervoor is het `EenhedenEnergieprestatie` model uitgebreid met het attribuut `gebruiksoppervlakteThermischeZone` of `gebruiksoppervlakte_thermische_zone` voor de Python representatie. In dit attribuut dient de gebruiksoppervlakte van de thermische zone die gebruikt is bij de registratie van de energieprestatie opgegeven worden.
 
 Voor woningen met een oppervlakte  >= 40 m2 geldt het volgende puntenaantal:
@@ -396,138 +319,204 @@
 | C     | 36              | 32                |
 | D     | 32              | 28                |
 | E     | 22              | 15                |
 | F     | 4               | 1                 |
 | G     | 0               | 0                 |
 
 ### 4.5.3 Afwijkingsbevoegdheid hogere energielabelklasse dan A++
-De hierboven vermelde tabellen met de puntentoekenning voor de labelklasse gaan tot A++. Het
-is mogelijk dat, bij een nieuw energielabel, een betere energielabelklasse dan A++ wordt afgegeven. Een energielabel voor de woonruimte kan tot maximaal A++++ gaan. De Huurcommissie
-heeft de bevoegdheid gekregen om af te wijken van de hierboven aangegeven puntenwaardering
-indien de energieprestatie hoort bij een betere energielabelklasse dan A++. Een dergelijke
-afwijking is uitsluitend mogelijk indien de gemaakte kosten om deze energieprestatie te bereiken,
-aanmerkelijk afwijken van hetgeen als gangbaar wordt beschouwd, of indien de energieprestatie
-aanmerkelijk beter is dan hetgeen als gangbaar bij een energielabelklasse A++ wordt beschouwd.
-De Huurcommissie vult deze bevoegdheid als volgt in. Indien sprake is van een A+++ label dan
-kent de Huurcommissie, 4 extra punten toe, boven op de punten die aan het label A++ worden
-toegekend. Indien sprake is van een A++++ label dan wordt 8 extra punten toegekend, boven op
-de punten die worden gegeven voor een label A++. 
+
+De hierboven vermelde tabellen met de puntentoekenning voor de labelklasse gaan tot A++. Het is mogelijk dat, bij een nieuw energielabel, een betere energielabelklasse dan A++ wordt afgegeven. Een energielabel voor de woonruimte kan tot maximaal A++++ gaan. De Huurcommissie heeft de bevoegdheid gekregen om af te wijken van de hierboven aangegeven puntenwaardering indien de energieprestatie hoort bij een betere energielabelklasse dan A++. Een dergelijke afwijking is uitsluitend mogelijk indien de gemaakte kosten om deze energieprestatie te bereiken, aanmerkelijk afwijken van hetgeen als gangbaar wordt beschouwd, of indien de energieprestatie aanmerkelijk beter is dan hetgeen als gangbaar bij een energielabelklasse A++ wordt beschouwd.  
+
+De Huurcommissie vult deze bevoegdheid als volgt in. Indien sprake is van een A+++ label dan kent de Huurcommissie, 4 extra punten toe, boven op de punten die aan het label A++ worden toegekend. Indien sprake is van een A++++ label dan wordt 8 extra punten toegekend, boven op de punten die worden gegeven voor een label A++. 
 
 ### 4.5.4 Bouwjaar bepalend bij geen geldig energielabel of Energie-Index
 
-Indien de energieprestatie van een woonruimte (in de vorm van een energielabel of een energieindex) niet tijdig is vastgesteld, of als de geldigheidsduur van het energielabel is verstreken, dan
-bepaalt het bouwjaar van de woning het aantal WWS-punten. Een (geldig) energielabel of EnergieIndex wordt door de Huurcommissie in de puntentelling betrokken als deze tijdig beschikbaar is om
-daarmee rekening te houden in de uitspraak. In geval de opnamedatum van het energielabel of de
-Energie-Index is gelegen na de relevante peildatum, geldt hierbij als voorwaarde dat de feitelijke
-toestand (wat energieprestatie betreft) op opnamedatum niet verschilt van de feitelijke toestand op
-de desbetreffende peildatum. Alleen als er geen verschil is zal de Huurcommissie het energielabel of
-Energie-Index bij de woningwaardering betrekken. De bewislast ligt bij de verhuurder.
+Indien de energieprestatie van een woonruimte (in de vorm van een energielabel of een energieindex) niet tijdig is vastgesteld, of als de geldigheidsduur van het energielabel is verstreken, dan bepaalt het bouwjaar van de woning het aantal WWS-punten. Een (geldig) energielabel of EnergieIndex wordt door de Huurcommissie in de puntentelling betrokken als deze tijdig beschikbaar is om daarmee rekening te houden in de uitspraak. In geval de opnamedatum van het energielabel of de Energie-Index is gelegen na de relevante peildatum, geldt hierbij als voorwaarde dat de feitelijke toestand (wat energieprestatie betreft) op opnamedatum niet verschilt van de feitelijke toestand op de desbetreffende peildatum. Alleen als er geen verschil is zal de Huurcommissie het energielabel of Energie-Index bij de woningwaardering betrekken. De bewislast ligt bij de verhuurder.  
+
 De puntentelling is in geval het bouwjaar geldt als volgt: 
 
 | Bouwjaar     | Eengezinswoning | Meergezinswoning |
 | ------------ | --------------- | ---------------- |
 | 2002 en ouder | 36              | 32               |
 | 2000 t/m 2001 | 32              | 28               |
 | 1998 t/m 1999 | 22              | 15               |
 | 1992 t/m 1997 | 22              | 11               |
 | 1984 t/m 1991 | 14              | 11               |
 | 1979 t/m 1983 | 8               | 5                |
 | 1977 t/m 1978 | 4               | 1                |
 | 1976 en ouder | 0               | 0                |
 
 ### ~~4.5.5 Gerede twijfel energielabel~~
+
 ~~Als huurder twijfelt aan de juistheid van het toepasselijke energielabel dan heeft de Huurcommissie de bevoegdheid om een ‘eigen oordeel’ uit te spreken bij gerede twijfel van het energielabel. Een Huurcommissie eigen oordeel (HEO) kan worden uitgesproken indien de huurder met bewijsstukken gemotiveerd aantoont dat sprake is van een verkeerd energielabel/energie-index en dat het gewijzigde energielabel/energie-index van invloed is op de huurprijs. Indien de Huurcommissie tot een eigen oordeel wil komen dan laat de Huurcommissie onderzoeken wat de energieprestatie van de woning is.~~
 
 ~~Het eigen oordeel is uitsluitend in de voorliggende zaak van kracht, wordt niet geregistreerd in het register van de Rijksdienst voor Ondernemend Nederland en komt te vervallen na ontbinding van de huurovereenkomst.~~
 
 > Wanneer een eigen oordeel van kracht is, en de waardering daarop gebaseerd moet worden, dient de gewijzigde energieprestatie opgegeven te worden in plaats van de geregistreerde energieprestatie.
 
 ### 4.5.6 Energieprestatievergoeding
+
 Voor woningen die zelf (gedeeltelijk) in hun energieverbruik voorzien, door bijvoorbeeld zonnepanelen, kan bij het verhuren een energieprestatievergoeding (EPV) worden afgesproken. De woning zal dan moeten voldoen aan de eisen voor een EPV. Als dit het geval is dan is het aantal punten op basis van het puntenstelsel voor energieprestatie lager. Om te voorkomen dat in de gevallen waarin een energieprestatievergoeding is overeengekomen, de opwekking van energie voor de huurder tevens wordt verdisconteerd in de huurprijs, wordt voor deze woningen een correctiefactor toegepast op het aantal punten voor de energieprestatie. In die gevallen wordt de energieprestatie gewaardeerd met een aantal punten gelijk aan de waardering voor een Energie-Index 1,2 < EI ≤ 1,4 (of Energielabel B), met 32 punten voor een ééngezinswoning en 28 punten voor meergezins- en duplexwoningen.
 
 > Hiervoor is het `EenhedenEnergieprestatie` model uitgebreid met het attribuut `energieprestatievergoeding`. Dit attribuut dient gevuld te zijn met een boolean die aangeeft of er bij het verhuren een energieprestatievergoeding (EPV) is overeengekomen.
 
+## 4.6 Keuken
+
+Het woningwaarderingsstelsel kent aan een zelfstandige woonruimte punten toe voor het onderdeel keukeninstallatie. Het woningwaarderingsstelsel geeft dus, naast punten voor de oppervlakte van de keuken (zijnde een vertrek, zie hiervoor onder [4.2.1](#421-wat-zijn-vertrekken)) ook punten voor de keukeninstallatie. Er zijn door de wetgever wel eisen gesteld om aan zo’n keukeninstallatie punten te mogen toekennen. En ook heeft de wetgever bepaald aan de hand waarvan je tot puntentoekenning komt. Hieronder wordt uiteengezet aan welke eisen moet zijn voldaan om punten aan een keukeninstallatie toe te kennen en op welke manier je de punten moet berekenen ([4.6.1](#461-voorzieningen-keuken)). Ook wordt besproken wanneer er extra kwaliteitspunten worden toegekend, welke keukenvoorzieningen daarvoor in aanmerking komen ([4.6.2](#462-voorzieningen-die-extra-kwaliteitspunten-opleveren)).
+
+### 4.6.1 Voorzieningen keuken
+
+Het woningwaarderingsstelsel geeft, naast punten voor de oppervlakte van het vertrek, ook punten voor de keukeninstallatie van zo’n vertrek.
+
+**Keukeninstallatie?**  
+Om punten vanwege de keukeninstallatie toe te kennen, moet het wel gaan om een inrichting van het vertrek dat als keukeninstallatie moet worden beschouwd. Daarvoor is in ieder geval vereist dat er een aanrecht aanwezig is. Zonder aanrecht spreken we niet van een keukeninstallatie. Aanvullend geldt nog dat de keuken voorzien moet zijn van een aan- en afvoer van water. Verder moet de keuken tenminste één aansluitpunt voor koken op gas of elektriciteit hebben. En het aanrecht moet zijn voorzien van minimaal twee onderkasten (met laden, deuren of schuiven).  
+
+In geval aan deze eisen niet wordt voldaan, is er geen sprake van een keukeninstallatie in de zin van het woningwaarderingsstelsel en worden er dus geen punten voor keukeninstallatie gerekend, ongeacht de lengte van het aanrecht (zie hierna). Ook kom je dan niet toe aan extra punten vanwege de kwaliteit van de voorzieningen als bedoeld in paragraaf [4.6.2](#462-voorzieningen-die-extra-kwaliteitspunten-opleveren).
+
+#### Punten: lengte van het aanrecht
+
+Uitgangspunt voor de waardering van de keukeninstallatie is de lengte van het aanrecht:
+
+- Is de lengte van het aanrecht minder dan 1 meter, dan worden er geen punten toegekend.
+- Is de lengte van het aanrecht tussen de 1 en 2 meter, dan worden er 4 punten toegekend.
+- Is de lengte van het aanrecht 2 meter of langer, dan worden er 7 punten toegekend.
+
+De lengte van het aanrecht moet over midden van het bovenblad worden gemeten. Daarbij moeten de ingebouwde spoelbakken worden meegeteld. Ingebouwde kookplaten worden niet meegeteld.  
+
+Een aanrecht met spoelbak, waarvan de lengte minder bedraagt dan 1 meter, voldoet dus niet aan de eis van 1 meter en wordt daarom niet als aanrecht gewaardeerd, maar als wastafel. Een aanrecht zonder onderkasten wordt gewaardeerd als een wastafel.  
+
+Indien een aanrechtblad langer is dan de aanwezige onderkasten met de bedoeling dat er onder het langere gedeelte van het aanrechtblad een losstaande koelkast, vaatwasser, wasmachine e.d., kan worden geplaatst, dan wordt dit gedeelte van het aanrechtblad mee gemeten mits er onder het blad aansluitmogelijkheden aanwezig zijn voor genoemde apparatuur.  
+
+Een ingebouwde (onroerende) koelkast, vaatwasser en/of oven beschouwen we als onderkast, mits daarnaast voldoende vervangende (andere) kastruimte aanwezig is.
+
+Indien er sprake is van onderbouwapparatuur (roerend), dan kan dit niet in de plaats van een onderkast worden gesteld en dient er voldoende vervangende (andere) kastruimte aanwezig te zijn. Een kastruimte in de vorm van een plank kan niet als zodanig worden aangemerkt.
+
+### ~~4.6.2 Voorzieningen die extra kwaliteitspunten opleveren~~
+
+> Er is gekozen om de extra kwaliteitspunten niet te implementeren aangezien veel elemeten niet gemodelleerd zijn in het huidige VERA model.
+
+~~Het woningwaarderingsstelsel kent de mogelijkheid om extra kwaliteitspunten te rekenen in geval de afwerking van de keuken daartoe aanleiding geeft. De extra kwaliteitspunten zijn een gestandaardiseerde invulling van de bevoegdheid van de Huurcommissie om investeringen ten behoeve van extra kwaliteit met extra punten te waarderen, tot maximaal het aantal punten dat reeds op grond van de aanrechtlengte is bepaald.~~
+
+~~De Huurcommissie kent extra kwaliteitspunten toe als de keukenuitrusting uitstijgt boven het minimale niveau, te weten:~~
+~~- een aanrechtblad met een lengte van minimaal 1 m (lengte incl. spoelbakken, exclusief afzuig installaties en inbouwkookplaten (tenzij 2-pits));~~
+~~- én 2 kasten (onder of boven of staande);~~
+~~- én wandtegelwerk of andersoortige waterdichte afwerking boven het aanrechtblad en in de kookhoek vanaf de vloer tot een hoogte van minimaal 1,5 m.~~
+
+~~Indien de keukenuitrusting en/of -afwerking boven het minimale niveau uitstijgt, is de waardering als volgt. Hierna wordt de voorziening genoemd met aansluitend het aantal extra punten.~~
+
+| Voorziening                                               | Aantal punten |
+|-----------------------------------------------------------|---------------|
+| inbouw kookplaat (gas/elektrisch)                         | 0,5           |
+| inbouw kookplaat 5 of 6 pits luxe uitvoering (RVS e.d.)   | 0,75          |
+| inbouw keramische kookplaat                               | 1,25          |
+| inbouw inductiekookplaat                                  | 1,50          |
+| inbouw oven (gas/elektrisch) of magnetron                 | 0,75          |
+| inbouw combi oven/magnetron                               | 1,5           |
+| inbouw oven inclusief kookplaat (gas/elektrisch)          | 1,25          |
+| inbouw magnetron                                          | 0,75          |
+| (inbouw) afzuigkap                                        | 0,5           |
+| (inbouw) luxe uitgevoerde afzuigkap of wasemkap           | 0,75          |
+| inbouw koelkast                                           | 0,75          |
+| inbouw vrieskist of -kast                                 | 0,5           |
+| inbouw vries/koelcombinatie                               | 1,25          |
+| inbouw vaatwasmachine                                     | 1,25          |
+| luxe mengkraan (bv. éénhandsbediening)                    | 0,25          |
+| thermostatische watermengkraan                            | 0,5           |
+| dubbele spoelbak                                          | 0,25          |
+| extra wandbetegeling per 2 m2                             | 0,25          |
+| vloertegels per 2 m2                                      | 0,25          |
+| extra enkele kast *                                       | 0,25          |
+| extra dubbele kast *                                      | 0,5           |
+
+~~*Als er meer dan 6 kasten aanwezig zijn (enkele kasten van min. 50-60 cm breed) dan wordt per extra kastruimte 0,25 punt extra toegekend, tenzij het om vervangende kastruimte gaat voor de door inbouwapparatuur in beslag genomen ruimte.~~
+
+~~Algehele luxe uitvoering (hardhouten of natuurstenen aanrechtblad, massief houten frontjes, ingebouwde verlichting, luxe wand, vloer en of plafondafwerking: ten hoogste 2 punten).~~
+
+~~NB.: Een luxe uitvoering of ingebouwde voorziening/ apparatuur komt voor extra punten in aanmerking, ongeacht de onderhoudstoestand daarvan. Als de kosten van desbetreffende voorziening/ apparatuur aanzienlijk hoger zijn dan de kosten, die als basis voor bovengenoemde normering zijn gehanteerd, dan blijft een afwijkende puntentelling mogelijk. In beginsel wordt altijd uitgegaan van de waardering conform bovenstaande lijst.~~
+
+~~Onder extra kastruimte wordt verstaan: elk gefixeerd element behorende tot de keuken/ het keukenblok, voorzien van een kastdeur, klep of lade én ongeacht de hoogte en breedte. Een element met twee deuren (bv. een hoekcarrousel) wordt als dubbele kast aangemerkt. Een element voorzien van laden wordt gewaardeerd als kast. Kastruimte boven een afzuigkap, waardoor het (lucht)afvoerkanaal verloopt, wordt meegeteld als volwaardige kastruimte.~~
+
 ## 4.7 Sanitair
-Het woningwaarderingsstelsel kent aan een zelfstandige woonruimte punten toe voor het
-onderdeel sanitair. De waardering van het sanitair wordt bepaald op grond van de aanwezigheid
-van bepaalde voorzieningen binnen de woning. Hieronder wordt uiteengezet aan welke sanitaire
-voorzieningen punten worden toegekend en hoeveel punten die voorzieningen krijgen. Ook wordt
-besproken wanneer er extra kwaliteitspunten worden toegekend aan deze sanitaire
-voorzieningen.
+
+Het woningwaarderingsstelsel kent aan een zelfstandige woonruimte punten toe voor het onderdeel sanitair. De waardering van het sanitair wordt bepaald op grond van de aanwezigheid van bepaalde voorzieningen binnen de woning. Hieronder wordt uiteengezet aan welke sanitaire voorzieningen punten worden toegekend en hoeveel punten die voorzieningen krijgen. Ook wordt besproken wanneer er extra kwaliteitspunten worden toegekend aan deze sanitaire voorzieningen.
+
+
 ### 4.7.1 Sanitaire voorzieningen
-Het woningwaarderingsstelsel geeft punten aan de sanitaire voorzieningen toilet, wastafel, bad
-en douche. De puntentoekenning is als volgt:
+
+Het woningwaarderingsstelsel geeft punten aan de sanitaire voorzieningen toilet, wastafel, bad en douche. De puntentoekenning is als volgt:  
 | Voorziening | Punten |
 | -------- | -------- |
 | toilet   | 3   |
 | wastafel  | 1  |
 | bidet    | 1  |
 | lavet*   | 1  |
 | douche   | 4  |
 | bad      | 6  |
 | bad en douche | 7  |
 
 > De punten hierboven in de tabel zijn het aantal punten dat wordt toegekend aan de sanitaire voorziening. De gedetailleerde voorwaarden die hieronder volgen in het beleidsboek worden niet getoetst in de implementatie. Het is aan de gebruiker om alleen voorzieningen op te geven die voldoen aan de voorwaarden.
 
-~~_*Een lavet wordt met vier punten gewaardeerd, als deze is voorzien van aansluitpunten voor warm en koud
-water én van douchegarnituur._~~
+~~_*Een lavet wordt met vier punten gewaardeerd, als deze is voorzien van aansluitpunten voor warm en koud water én van douchegarnituur._~~
 
 **Toilet**  
-Drie punten worden toegekend aan een toilet ~~met waterspoeling als het toilet is geplaatst in een
-daartoe bestemde ruimte en als het toilet binnen het woongebouw is gelegen. Wanneer sprake is
-van een toilet dat buiten de woning maar binnen het woongebouw is gelegen, dan geldt dat het
-toilet in de waardering wordt meegenomen als het gebruik van het toilet door derden is uit te
-sluiten.~~  
+Drie punten worden toegekend aan een toilet ~~met waterspoeling als het toilet is geplaatst in een daartoe bestemde ruimte en als het toilet binnen het woongebouw is gelegen. Wanneer sprake is van een toilet dat buiten de woning maar binnen het woongebouw is gelegen, dan geldt dat het toilet in de waardering wordt meegenomen als het gebruik van het toilet door derden is uit te sluiten.~~  
 
 **Wastafel**  
-Wastafels worden met één punt gewaardeerd. ~~Als wastafels worden alle bakken geteld voor
-wassen en spoelen die op de waterleiding én op het huisriool zijn aangesloten. Een dergelijke bak
-wordt niet als wastafel gewaardeerd indien boven de bak een douche is aangebracht. Een bad en
-spoelbakken in een keukenaanrecht worden niet als wastafels gewaardeerd.
-Als wastafel waardeert de Huurcommissie een fonteintje en een aanrecht dat niet voor punten in
-aanmerking komt, waarvan de aanrechtlengte korter is dan één meter.~~
+Wastafels worden met één punt gewaardeerd. ~~Als wastafels worden alle bakken geteld voor wassen en spoelen die op de waterleiding én op het huisriool zijn aangesloten. Een dergelijke bak wordt niet als wastafel gewaardeerd indien boven de bak een douche is aangebracht. Een bad en spoelbakken in een keukenaanrecht worden niet als wastafels gewaardeerd.~~ 
+
+~~Als wastafel waardeert de Huurcommissie een fonteintje en een aanrecht dat niet voor punten in aanmerking komt, waarvan de aanrechtlengte korter is dan één meter.~~
 
 **Bad en douche**  
-Douches worden gewaardeerd met vier punten. ~~Als douche wordt meegeteld iedere door de
-verhuurder aangebrachte installatie voor het nemen van een stortbad. Hieronder valt eveneens
-een zogenaamde douchecabine, die voldoet aan bovengenoemde voorwaarden, als de douchecabine
-in een vertrek (anders dan bad- of doucheruimte) of overige ruimte is geplaatst. De oppervlakte van dat vertrek of van die overige ruimte wordt in dat geval niet verminderd met de door de
-douchecabine ingenomen oppervlakte.~~
-Aan baden worden zes punten toegekend, ~~ongeacht de lengte van het bad. Indien een bad is
-voorzien van een (hand)douche, dan wordt het douchegarnituur niet afzonderlijk geteld.~~
-Indien in de badruimte behalve het bad tevens een afzonderlijke douche is aangebracht, geldt een
-waardering van zeven punten.  
+Douches worden gewaardeerd met vier punten. ~~Als douche wordt meegeteld iedere door de verhuurder aangebrachte installatie voor het nemen van een stortbad. Hieronder valt eveneens een zogenaamde douchecabine, die voldoet aan bovengenoemde voorwaarden, als de douchecabine in een vertrek (anders dan bad- of doucheruimte) of overige ruimte is geplaatst. De oppervlakte van dat vertrek of van die overige ruimte wordt in dat geval niet verminderd met de door de douchecabine ingenomen oppervlakte.~~  
+
+Aan baden worden zes punten toegekend, ~~ongeacht de lengte van het bad. Indien een bad is voorzien van een (hand)douche, dan wordt het douchegarnituur niet afzonderlijk geteld.~~  
+
+Indien in de badruimte behalve het bad tevens een afzonderlijke douche is aangebracht, geldt een waardering van zeven punten.  
 
 > Het is ambigu hoeveel punten er zouden moeten worden toegekend indien een badruimte meer dan één douche bevat en één bad of vice versa. I.v.m. de onwaarschijnlijkheid van het voortkomen van deze situatie is er gekozen om deze situatie niet te ondersteunen in de implementatie. Indien er een bad en een douche in dezelfde ruimte aanwezig zijn worden er 7 punten toegekend per combinatie van bad en douche.  
 >
 > Oftewel:
 >
 > - één bad en één douche in dezelfde ruimte: 7 punten  
 > - één bad en twee douches in dezelfde ruimte: 7 punten
 > - twee baden en één douche in dezelfde ruimte: 7 punten
 > - twee baden en twee douches in dezelfde ruimte: 14 punten
 
 ~~**Voorzieningen in een bad- en doucheruimte**~~  
-~~Indien sprake is van sanitaire voorzieningen in een bad- of doucheruimte*, dan worden alleen
-punten toegekend aan die voorzieningen indien de bad -of doucheruimte voldoet aan drie
-voorwaarden.
-Ten eerste moet de wand- en vloerafwerking van de bad- of douchruimte voldoende waterdicht
-zijn. Een bad in een vertrek met een niet-waterdichte vloer wordt door de Huurcommissie wel
-gewaardeerd, omdat het bad zelf als een waterdichte afwerking wordt gezien. Ten tweede moet
-de bad- en doucheruimte zijn voorzien van aansluitingspunten voor warm en koud water. Met
-aansluitingspunten voor warm en koud water wordt niet een warmwater apparaat bedoeld. Als
-sprake is van een geiser of boiler dan hoeven deze niet door de verhuurder te zijn verstrekt. Ten
-derde moet het bad of de douche zijn voorzien van douchegarnituur. Met douchegarnituur bedoelt
-de Huurcommissie een warm- en koudwaterkraan of een mengkraan.
-Indien het aansluitpunt voor warm en koud water bedoeld is voor gecombineerd gebruik van
-zowel een wastafel als de naastgelegen douche of bad (bijvoorbeeld door middel van een
-zogenaamde zwenkarm), dan wordt uitsluitend de douche of het bad gewaardeerd. Dus niet én 1
-punt voor wastafel én 4 of 6 punten voor douche of lavet, respectievelijk bad.
-Indien in de bad- of doucheruimte een toilet is geplaatst wordt dit toilet volledig gewaardeerd met
-drie punten.~~
-
-~~_*De Huurcommissie verstaat onder een bad-/doucheruimte een (afzonderlijke) ruimte met een vrije hoogte van ten
-minste 2 meter, gemeten vanaf de vloer tot aan het zichtbare plafond. Daarin dient tenminste aanwezig te zijn een
-wastafel of een douche of een bad. Voor een gecombineerde bad-/douche- en toiletruimte geldt, vanwege de
-oppervlakte-eis voor toilet- ruimten, een minimale oppervlakte van 0,64 m2 . Indien een douche- of badruimte,
-eventueel gecombineerd met een toilet, niet een vrije hoogte heeft van 2,00 m, dan wordt de ruimte gewaardeerd
-als overige ruimte._~~
+~~Indien sprake is van sanitaire voorzieningen in een bad- of doucheruimte[^24], dan worden alleen punten toegekend aan die voorzieningen indien de bad -of doucheruimte voldoet aan drie voorwaarden. Ten eerste moet de wand- en vloerafwerking van de bad- of douchruimte voldoende waterdicht zijn. Een bad in een vertrek met een niet-waterdichte vloer wordt door de Huurcommissie wel gewaardeerd, omdat het bad zelf als een waterdichte afwerking wordt gezien. Ten tweede moet de bad- en doucheruimte zijn voorzien van aansluitingspunten voor warm en koud water. Met aansluitingspunten voor warm en koud water wordt niet een warmwater apparaat bedoeld. Als sprake is van een geiser of boiler dan hoeven deze niet door de verhuurder te zijn verstrekt. Ten derde moet het bad of de douche zijn voorzien van douchegarnituur. Met douchegarnituur bedoelt de Huurcommissie een warm- en koudwaterkraan of een mengkraan. Indien het aansluitpunt voor warm en koud water bedoeld is voor gecombineerd gebruik van zowel een wastafel als de naastgelegen douche of bad (bijvoorbeeld door middel van een zogenaamde zwenkarm), dan wordt uitsluitend de douche of het bad gewaardeerd. Dus niet én 1 punt voor wastafel én 4 of 6 punten voor douche of lavet, respectievelijk bad. Indien in de bad- of doucheruimte een toilet is geplaatst wordt dit toilet volledig gewaardeerd met drie punten.~~
+
+### ~~4.7.2	 Voorzieningen die extra kwaliteitspunten opleveren~~
+
+> Er is gekozen om de extra kwaliteitspunten niet te implementeren aangezien veel elemeten niet gemodelleerd zijn in het huidige VERA model.
+
+~~Extra kwaliteitspunten kunnen worden toegekend indien het sanitair en/of de afwerking van de bad- of doucheruimte een kwaliteitsniveau heeft dat, op het moment van de woningwaardering[^25], het gangbare kwaliteitsniveau van sociale huurwoningen overschrijdt. Met het gangbare kwaliteitsniveau bedoelt de Huurcommissie het kwaliteit-/uitrustingsniveau van nieuwe socialehuurwoningen (niet ouder dan vijf jaar). In dit verband In dit verband heeft de bad- en/of doucheruimte van een nieuwe sociale huurwoning de volgende kenmerken:~~
+
+- ~~een waterdichte vloerafwerking;~~
+- ~~betegeling rondom tot resp. 1,50 m hoogte voor badruimte en 1,80 m voor doucheruimte;~~
+- ~~en wastafel inclusief mengkraan met spiegel en planchet én;~~
+- ~~een douche of bad met aansluitpunten voor warm en koud water en voorzien van douchegarnituur.~~
+
+[^24]: De Huurcommissie verstaat onder een bad-/doucheruimte een (afzonderlijke) ruimte met een vrije hoogte van ten minste 2 meter, gemeten vanaf de vloer tot aan het zichtbare plafond. Daarin dient tenminste aanwezig te zijn een wastafel of een douche of een bad. Voor een gecombineerde bad-/douche- en toiletruimte geldt, vanwege de oppervlakteeis voor toilet- ruimten, een minimale oppervlakte van 0,64 m2 . Indien een douche- of badruimte, eventueel gecombineerd met een toilet, niet een vrije hoogte heeft van 2,00 m, dan wordt de ruimte gewaardeerd als overige ruimte.  
+
+~~[^25]: Zie hoofdstuk 3 van dit beleidsboek voor de peildatum per procedure ten aanzien van de woningwaardering.~~
+
+~~Er kunnen extra kwaliteitspunten worden toegekend tot maximaal het aantal punten dat reeds voor de douche en/of bad is bepaald. Anders gezegd: maximaal een verdubbeling van de toegekende kwaliteitspunten voor douche en/of bad kan plaatsvinden.~~
+
+#### ~~Voorzieningen die extra kwaliteitspunten opleveren~~
+
+~~De Huurcommissie heeft een aantal voorzieningen aangewezen die extra kwaliteitspunten opleveren, aangezien hiermee het kwaliteitsniveau van het sanitair en/of de afwerking van de bad- of doucheruimte het gangbare bij sociale huurwoningen overstijgt. De onderhoudstoestand van de desbetreffende voorziening of apparatuur is niet relevant of extra kwaliteitspunten worden toegekend.~~
+
+| Voorziening                                               | Aantal punten           |
+|-----------------------------------------------------------|-------------------------|
+| extra wandbetegeling                                      | 0,25 (per 2 m2)         |
+| kastje, waarin ingebouwd een wastafel                     | 0,25                    |
+| toiletkastje met ingebouwde verlichting                   | 0,25                    |
+| extra voor een bubbelbad (whirlpool)                      | 2                       |
+| luxe mengkraan (bv. éénhandsbediening)                    | 0,25                    |
+| thermostatische watermengkraan                            | 0,5                     |
+| douchewand of douchecabine (glas of kunststof)            | 1                       |
+| wandcloset/ zwevend toilet (met inbouwreservoir)          | 0,5                     |
+| design-/handdoekradiator                                  | 0,25                    |
+
+~~Een algehele luxe uitvoering van de bad- of doucheruimte (luxe plafondafwerking, vloer- of wandafwerking van reliëf- of natuursteen, ingebouwde verlichting, etc.) levert ten hoogste twee punten op.~~
+
+~~Indien een (pantry) keukenblok van <1 m, met inbouwapparatuur, als wastafel is gewaardeerd dan levert dit maximaal vier extra kwaliteitspunten op.~~
```

### Comparing `woningwaardering-0.3.0a7/pyproject.toml` & `woningwaardering-0.4.0a0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/scripts/genereer_opzet_woningwaarderinggroep.py` & `woningwaardering-0.4.0a0/scripts/genereer_opzet_woningwaarderinggroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/scripts/genereer_test_output.py` & `woningwaardering-0.4.0a0/scripts/genereer_test_output.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/scripts/genereer_vera_referentiedata.py` & `woningwaardering-0.4.0a0/scripts/genereer_vera_referentiedata.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/scripts/uitbreiden_vera_modellen.py` & `woningwaardering-0.4.0a0/scripts/uitbreiden_vera_modellen.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/taskfile.yml` & `woningwaardering-0.4.0a0/taskfile.yml`

 * *Files 4% similar despite different names*

```diff
@@ -28,7 +28,11 @@
     desc: Genereer VERA referentiedata
     cmds:
       - python scripts/genereer_vera_referentiedata.py
   genereer-opzet-woningwaarderinggroep:
     desc: Genereer de opzet voor de code van een woningwaarderinggroep
     cmds:
       - python scripts/genereer_opzet_woningwaarderinggroep.py
+  genereer-test-output:
+    desc: Genereer test output
+    cmds:
+      - python scripts/genereer_test_output.py
```

### Comparing `woningwaardering-0.3.0a7/tests/conftest.py` & `woningwaardering-0.4.0a0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/input/generiek/37101000032.json` & `woningwaardering-0.4.0a0/tests/data/input/generiek/37101000032.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/12006000004.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/12006000004.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/23003000050.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/23003000050.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/25048000007.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/25048000007.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/28018000044.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/28018000044.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/37101000032.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/37101000032.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/41027000003.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/41027000003.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/41123000005.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/41123000005.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.999969135802469%*

 * *Differences: {"'ruimten'": "{12: {'bouwkundigeElementen': {0: {'lengte': 1875, delete: ['extraAttributen']}}}}"}*

```diff
@@ -342,20 +342,17 @@
         {
             "bouwkundigeElementen": [
                 {
                     "detailSoort": {
                         "code": "AAN",
                         "naam": "Aanrecht"
                     },
-                    "extraAttributen": {
-                        "ifcSoort": "IfcFurniture",
-                        "lengteAanrecht": 1875
-                    },
                     "id": "Aanrecht_72739118",
                     "id_bimmodel": "0ZTYhATwr0BOPGb6sgAY$F",
+                    "lengte": 1875,
                     "naam": "Aanrecht",
                     "omschrijving": "Aanrecht in Keuken",
                     "soort": {
                         "code": "KEU",
                         "naam": "Keuken voorziening"
                     }
                 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/41162000015.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/41162000015.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/41164000002.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/41164000002.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/51011000042.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/51011000042.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/71211000027.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/71211000027.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/77795000000.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/77795000000.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999485596707819%*

 * *Differences: {"'ruimten'": "{7: {'bouwkundigeElementen': {0: {'lengte': 3600, delete: ['extraAttributen']}}}}"}*

```diff
@@ -260,20 +260,17 @@
         {
             "bouwkundigeElementen": [
                 {
                     "detailSoort": {
                         "code": "AAN",
                         "naam": "Aanrecht"
                     },
-                    "extraAttributen": {
-                        "ifcSoort": "IfcFurniture",
-                        "lengteAanrecht": 3600
-                    },
                     "id": "Aanrecht_9944878",
                     "id_bimmodel": "1CjCgpyVjFRfJZqbPvo4Cz",
+                    "lengte": 3600,
                     "naam": "Aanrecht",
                     "omschrijving": "Aanrecht in Keuken",
                     "soort": {
                         "code": "KEU",
                         "naam": "Keuken voorziening"
                     }
                 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/81020000003.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/81020000003.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9999649270482602%*

 * *Differences: {"'ruimten'": "{9: {'bouwkundigeElementen': {0: {'lengte': 1800, delete: ['extraAttributen']}}}}"}*

```diff
@@ -298,20 +298,17 @@
         {
             "bouwkundigeElementen": [
                 {
                     "detailSoort": {
                         "code": "AAN",
                         "naam": "Aanrecht"
                     },
-                    "extraAttributen": {
-                        "ifcSoort": "IfcFurniture",
-                        "lengteAanrecht": 1800
-                    },
                     "id": "Aanrecht_57349829",
                     "id_bimmodel": "02Huynkxr6cxvV0_9wJ2PZ",
+                    "lengte": 1800,
                     "naam": "Aanrecht",
                     "omschrijving": "Aanrecht in Keuken",
                     "soort": {
                         "code": "KEU",
                         "naam": "Keuken voorziening"
                     }
                 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/81065000089.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/81065000089.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/85651000021.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/85651000021.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/input/zelfstandige_woonruimten/87402000003.json` & `woningwaardering-0.4.0a0/tests/data/input/zelfstandige_woonruimten/87402000003.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8055555555555557%*

 * *Differences: {"'groepen'": "{insert: [(5, OrderedDict([('criteriumGroep', OrderedDict([('stelsel', "*

 * *              "OrderedDict([('code', 'ZEL'), ('naam', 'Zelfstandige woonruimten')])), "*

 * *              "('stelselgroep', OrderedDict([('code', 'KEU'), ('naam', 'Keuken')]))])), ('punten', "*

 * *              "7.0), ('woningwaarderingen', [OrderedDict([('aantal', 2100.0), ('criterium', "*

 * *              "OrderedDict([('naam', 'Lengte aanrecht'), ('meeteenheid', OrderedDict([('code', "*

 * *              "'MLM'), ('naam', 'Millimeter' […]*

```diff
@@ -176,15 +176,41 @@
                     "aantal": 1.0,
                     "criterium": {
                         "naam": "Closetcombinatie"
                     },
                     "punten": 3.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 7.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 2100.0,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "MLM",
+                            "naam": "Millimeter"
+                        },
+                        "naam": "Lengte aanrecht"
+                    },
+                    "punten": 7.0
+                }
+            ]
         }
     ],
-    "punten": 84.0,
+    "punten": 91.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7824652777777779%*

 * *Differences: {"'groepen'": "{0: {'woningwaarderingen': {0: {'aantal': 30.12, 'criterium': {'naam': "*

 * *              "'Woonkamer'}}, 1: {'aantal': 11.72}, 2: {'aantal': 4.64, 'criterium': {'naam': "*

 * *              "'Badruimte'}}, 3: {'aantal': 9.21, 'criterium': {'naam': 'Slaapkamer'}}, 4: "*

 * *              "{'aantal': 5.76}}}, 1: {'punten': 3.75, 'woningwaarderingen': {0: {'aantal': "*

 * *              "5.1}}}, 2: {'woningwaarderingen': {0: {'criterium': {'naam': 'Woonkamer'}}, 2: "*

 * *              "{'criterium': {'naam': 'Badrui […]*

```diff
@@ -10,55 +10,55 @@
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
             "punten": 61.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 11.88,
+                    "aantal": 30.12,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 9.73,
+                    "aantal": 11.72,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 22.85,
+                    "aantal": 4.64,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 3.94,
+                    "aantal": 9.21,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 12.22,
+                    "aantal": 5.76,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Keuken"
                     }
@@ -72,18 +72,18 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 3.0,
+            "punten": 3.75,
             "woningwaarderingen": [
                 {
-                    "aantal": 4.41,
+                    "aantal": 5.1,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Berging"
                     }
@@ -101,33 +101,33 @@
                     "naam": "Verwarming"
                 }
             },
             "punten": 10.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Badruimte"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Keuken"
                     },
@@ -142,60 +142,52 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "ENE",
                     "naam": "Energieprestatie"
                 }
             },
-            "punten": 15.0,
+            "punten": 28.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "C (oud)"
+                        "naam": "B (oud)"
                     },
-                    "punten": 15.0
+                    "punten": 28.0
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "SAN",
                     "naam": "Sanitair"
                 }
             },
-            "punten": 9.0,
-            "woningwaarderingen": [
-                {
-                    "aantal": 1.0,
-                    "criterium": {
-                        "naam": "Closetcombinatie"
-                    },
-                    "punten": 3.0
-                },
-                {
-                    "aantal": 2.0,
-                    "criterium": {
-                        "naam": "Wastafel"
-                    },
-                    "punten": 2.0
+            "punten": 0.0,
+            "woningwaarderingen": []
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
                 },
-                {
-                    "aantal": 1.0,
-                    "criterium": {
-                        "naam": "Douche"
-                    },
-                    "punten": 4.0
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
                 }
-            ]
+            },
+            "punten": 0.0,
+            "woningwaarderingen": []
         }
     ],
-    "punten": 98.0,
+    "punten": 103.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7913773148148149%*

 * *Differences: {"'groepen'": "{0: {'punten': 53.0, 'woningwaarderingen': {0: {'aantal': 11.65, 'criterium': "*

 * *              "{'naam': 'Slaapkamer'}}, 1: {'aantal': 3.12, 'criterium': {'naam': 'Badruimte'}}, "*

 * *              "2: {'aantal': 6.37, 'criterium': {'naam': 'Keuken'}}, 3: {'aantal': 23.1, "*

 * *              "'criterium': {'naam': 'Woonkamer'}}, 4: {'aantal': 8.35, 'criterium': {'naam': "*

 * *              "'Slaapkamer'}}}}, 1: {'woningwaarderingen': {0: {'aantal': 5.25}}}, 2: "*

 * *              "{'woningwaarderingen': {0: { […]*

```diff
@@ -7,64 +7,64 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 61.0,
+            "punten": 53.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 30.12,
+                    "aantal": 11.65,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 11.72,
+                    "aantal": 3.12,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 4.64,
+                    "aantal": 6.37,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 9.21,
+                    "aantal": 23.1,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 5.76,
+                    "aantal": 8.35,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -75,15 +75,15 @@
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
             "punten": 3.75,
             "woningwaarderingen": [
                 {
-                    "aantal": 5.1,
+                    "aantal": 5.25,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Berging"
                     }
@@ -101,39 +101,39 @@
                     "naam": "Verwarming"
                 }
             },
             "punten": 10.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Keuken"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 }
             ]
         },
         {
             "criteriumGroep": {
@@ -142,21 +142,21 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "ENE",
                     "naam": "Energieprestatie"
                 }
             },
-            "punten": 28.0,
+            "punten": 0.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "B (oud)"
+                        "naam": "Bouwjaar 1898"
                     },
-                    "punten": 28.0
+                    "punten": 0.0
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
@@ -165,15 +165,29 @@
                 "stelselgroep": {
                     "code": "SAN",
                     "naam": "Sanitair"
                 }
             },
             "punten": 0.0,
             "woningwaarderingen": []
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 0.0,
+            "woningwaarderingen": []
         }
     ],
-    "punten": 103.0,
+    "punten": 67.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8055555555555557%*

 * *Differences: {"'groepen'": "{insert: [(5, OrderedDict([('criteriumGroep', OrderedDict([('stelsel', "*

 * *              "OrderedDict([('code', 'ZEL'), ('naam', 'Zelfstandige woonruimten')])), "*

 * *              "('stelselgroep', OrderedDict([('code', 'KEU'), ('naam', 'Keuken')]))])), ('punten', "*

 * *              "7.0), ('woningwaarderingen', [OrderedDict([('aantal', 2210.0), ('criterium', "*

 * *              "OrderedDict([('naam', 'Lengte aanrecht'), ('meeteenheid', OrderedDict([('code', "*

 * *              "'MLM'), ('naam', 'Millimeter' […]*

```diff
@@ -203,15 +203,41 @@
                     "aantal": 1.0,
                     "criterium": {
                         "naam": "Douche"
                     },
                     "punten": 4.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 7.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 2210.0,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "MLM",
+                            "naam": "Millimeter"
+                        },
+                        "naam": "Lengte aanrecht"
+                    },
+                    "punten": 7.0
+                }
+            ]
         }
     ],
-    "punten": 113.0,
+    "punten": 120.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7795919679600235%*

 * *Differences: {"'groepen'": "{0: {'punten': 138.0, 'woningwaarderingen': {0: {'aantal': 6.33, 'criterium': "*

 * *              "{'naam': 'Badruimte'}}, 1: {'aantal': 23.42, 'criterium': {'naam': 'Slaapkamer + 1 "*

 * *              "kast'}}, 2: {'aantal': 22.66, 'criterium': {'naam': 'Slaapkamer'}}, 3: {'aantal': "*

 * *              "14.71, 'criterium': {'naam': 'Keuken'}}, 4: {'aantal': 17.63}, 5: {'aantal': 32.95, "*

 * *              "'criterium': {'naam': 'Woonkamer'}}, 6: {'aantal': 20.45, 'criterium': {'naam': "*

 * *              "'Slaa […]*

```diff
@@ -7,84 +7,84 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 140.0,
+            "punten": 138.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 21.05,
+                    "aantal": 6.33,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 41.0,
+                    "aantal": 23.42,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer"
+                        "naam": "Slaapkamer + 1 kast"
                     }
                 },
                 {
-                    "aantal": 20.37,
+                    "aantal": 22.66,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 6.5,
+                    "aantal": 14.71,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 15.98,
+                    "aantal": 17.63,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 19.15,
+                    "aantal": 32.95,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 15.82,
+                    "aantal": 20.45,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Slaapkamer + 1 kast"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -92,24 +92,24 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 5.25,
+            "punten": 3.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 6.65,
+                    "aantal": 4.31,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Berging"
+                        "naam": "Wasruimte"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -121,45 +121,45 @@
                     "naam": "Verwarming"
                 }
             },
             "punten": 14.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Keuken"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
@@ -174,60 +174,67 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "ENE",
                     "naam": "Energieprestatie"
                 }
             },
-            "punten": 22.0,
+            "punten": 32.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "C (oud)"
+                        "naam": "B (oud)"
                     },
-                    "punten": 22.0
+                    "punten": 32.0
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "SAN",
                     "naam": "Sanitair"
                 }
             },
-            "punten": 16.0,
+            "punten": 7.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 2.0,
-                    "criterium": {
-                        "naam": "Closetcombinatie"
-                    },
-                    "punten": 6.0
-                },
-                {
-                    "aantal": 3.0,
+                    "aantal": 4.0,
                     "criterium": {
                         "naam": "Wastafel"
                     },
-                    "punten": 3.0
+                    "punten": 4.0
                 },
                 {
                     "aantal": 1.0,
                     "criterium": {
-                        "naam": "Bad en Douche in zelfde ruimte"
+                        "naam": "Closetcombinatie"
                     },
-                    "punten": 7.0
+                    "punten": 3.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 0.0,
+            "woningwaarderingen": []
         }
     ],
-    "punten": 197.0,
+    "punten": 194.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8055555555555557%*

 * *Differences: {"'groepen'": "{insert: [(5, OrderedDict([('criteriumGroep', OrderedDict([('stelsel', "*

 * *              "OrderedDict([('code', 'ZEL'), ('naam', 'Zelfstandige woonruimten')])), "*

 * *              "('stelselgroep', OrderedDict([('code', 'KEU'), ('naam', 'Keuken')]))])), ('punten', "*

 * *              "4.0), ('woningwaarderingen', [OrderedDict([('aantal', 1833.0), ('criterium', "*

 * *              "OrderedDict([('naam', 'Lengte aanrecht'), ('meeteenheid', OrderedDict([('code', "*

 * *              "'MLM'), ('naam', 'Millimeter' […]*

```diff
@@ -176,15 +176,41 @@
                     "aantal": 1.0,
                     "criterium": {
                         "naam": "Closetcombinatie"
                     },
                     "punten": 3.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 4.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 1833.0,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "MLM",
+                            "naam": "Millimeter"
+                        },
+                        "naam": "Lengte aanrecht"
+                    },
+                    "punten": 4.0
+                }
+            ]
         }
     ],
-    "punten": 67.0,
+    "punten": 71.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8055555555555557%*

 * *Differences: {"'groepen'": "{insert: [(5, OrderedDict([('criteriumGroep', OrderedDict([('stelsel', "*

 * *              "OrderedDict([('code', 'ZEL'), ('naam', 'Zelfstandige woonruimten')])), "*

 * *              "('stelselgroep', OrderedDict([('code', 'KEU'), ('naam', 'Keuken')]))])), ('punten', "*

 * *              "4.0), ('woningwaarderingen', [OrderedDict([('aantal', 1875.0), ('criterium', "*

 * *              "OrderedDict([('naam', 'Lengte aanrecht'), ('meeteenheid', OrderedDict([('code', "*

 * *              "'MLM'), ('naam', 'Millimeter' […]*

```diff
@@ -293,15 +293,41 @@
                     "aantal": 2.0,
                     "criterium": {
                         "naam": "Closetcombinatie"
                     },
                     "punten": 6.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 4.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 1875.0,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "MLM",
+                            "naam": "Millimeter"
+                        },
+                        "naam": "Lengte aanrecht"
+                    },
+                    "punten": 4.0
+                }
+            ]
         }
     ],
-    "punten": 193.0,
+    "punten": 197.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8055555555555557%*

 * *Differences: {"'groepen'": "{insert: [(5, OrderedDict([('criteriumGroep', OrderedDict([('stelsel', "*

 * *              "OrderedDict([('code', 'ZEL'), ('naam', 'Zelfstandige woonruimten')])), "*

 * *              "('stelselgroep', OrderedDict([('code', 'KEU'), ('naam', 'Keuken')]))])), ('punten', "*

 * *              "7.0), ('woningwaarderingen', [OrderedDict([('aantal', 2010.0), ('criterium', "*

 * *              "OrderedDict([('naam', 'Lengte aanrecht'), ('meeteenheid', OrderedDict([('code', "*

 * *              "'MLM'), ('naam', 'Millimeter' […]*

```diff
@@ -213,15 +213,41 @@
                     "aantal": 1.0,
                     "criterium": {
                         "naam": "Closetcombinatie"
                     },
                     "punten": 3.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 7.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 2010.0,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "MLM",
+                            "naam": "Millimeter"
+                        },
+                        "naam": "Lengte aanrecht"
+                    },
+                    "punten": 7.0
+                }
+            ]
         }
     ],
-    "punten": 98.0,
+    "punten": 105.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7822788065843621%*

 * *Differences: {"'groepen'": "{0: {'punten': 60.0, 'woningwaarderingen': {0: {'aantal': 17.56, 'criterium': "*

 * *              "{'naam': 'Woonkamer + 1 kast'}}, 1: {'aantal': 11.8}, 2: {'aantal': 6.99, "*

 * *              "'criterium': {'naam': 'Slaapkamer + 2 kasten'}}, 3: {'aantal': 8.15, 'criterium': "*

 * *              "{'naam': 'Slaapkamer'}}, 4: {'aantal': 1.92, 'criterium': {'naam': 'Badruimte'}}, "*

 * *              "5: {'aantal': 7.06, 'criterium': {'naam': 'Keuken'}}, 6: {'aantal': 6.92, "*

 * *              "'criterium': {'naam':  […]*

```diff
@@ -7,84 +7,84 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 138.0,
+            "punten": 60.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 6.33,
+                    "aantal": 17.56,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Woonkamer + 1 kast"
                     }
                 },
                 {
-                    "aantal": 23.42,
+                    "aantal": 11.8,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer + 1 kast"
                     }
                 },
                 {
-                    "aantal": 22.66,
+                    "aantal": 6.99,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Slaapkamer + 2 kasten"
                     }
                 },
                 {
-                    "aantal": 14.71,
+                    "aantal": 8.15,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 17.63,
+                    "aantal": 1.92,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 32.95,
+                    "aantal": 7.06,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer"
+                        "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 20.45,
+                    "aantal": 6.92,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer + 1 kast"
+                        "naam": "Slaapkamer"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -92,27 +92,16 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 3.0,
-            "woningwaarderingen": [
-                {
-                    "aantal": 4.31,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Wasruimte"
-                    }
-                }
-            ]
+            "punten": 0.0,
+            "woningwaarderingen": []
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
@@ -121,15 +110,15 @@
                     "naam": "Verwarming"
                 }
             },
             "punten": 14.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
@@ -139,27 +128,27 @@
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Keuken"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
@@ -178,15 +167,15 @@
                     "naam": "Energieprestatie"
                 }
             },
             "punten": 32.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "B (oud)"
+                        "naam": "A (oud)"
                     },
                     "punten": 32.0
                 }
             ]
         },
         {
             "criteriumGroep": {
@@ -195,32 +184,65 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "SAN",
                     "naam": "Sanitair"
                 }
             },
-            "punten": 7.0,
+            "punten": 9.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 4.0,
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Closetcombinatie"
+                    },
+                    "punten": 3.0
+                },
+                {
+                    "aantal": 2.0,
                     "criterium": {
                         "naam": "Wastafel"
                     },
-                    "punten": 4.0
+                    "punten": 2.0
                 },
                 {
                     "aantal": 1.0,
                     "criterium": {
-                        "naam": "Closetcombinatie"
+                        "naam": "Douche"
                     },
-                    "punten": 3.0
+                    "punten": 4.0
+                }
+            ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 4.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 1800.0,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "MLM",
+                            "naam": "Millimeter"
+                        },
+                        "naam": "Lengte aanrecht"
+                    },
+                    "punten": 4.0
                 }
             ]
         }
     ],
-    "punten": 194.0,
+    "punten": 119.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7755180776014109%*

 * *Differences: {"'groepen'": "{0: {'punten': 58.0, 'woningwaarderingen': {0: {'aantal': 11.63, 'criterium': "*

 * *              "{'naam': 'Slaapkamer'}}, 1: {'aantal': 7.62}, 2: {'aantal': 17.77, 'criterium': "*

 * *              "{'naam': 'Woonkamer'}}, 3: {'aantal': 12.72}, 4: {'aantal': 8.34}, delete: [1, "*

 * *              "0]}}, 1: {'punten': 4.5, 'woningwaarderingen': [OrderedDict([('aantal', 3.56), "*

 * *              "('criterium', OrderedDict([('naam', 'Zolder'), ('meeteenheid', "*

 * *              "OrderedDict([('code', 'M2'), ('na […]*

```diff
@@ -7,144 +7,139 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 60.0,
+            "punten": 58.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 17.56,
+                    "aantal": 11.63,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer + 1 kast"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 11.8,
+                    "aantal": 7.62,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer + 1 kast"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 6.99,
+                    "aantal": 17.77,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer + 2 kasten"
+                        "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 8.15,
+                    "aantal": 12.72,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 1.92,
+                    "aantal": 8.34,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Slaapkamer"
                     }
+                }
+            ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
                 },
+                "stelselgroep": {
+                    "code": "OOZ",
+                    "naam": "Oppervlakte van overige ruimten"
+                }
+            },
+            "punten": 4.5,
+            "woningwaarderingen": [
                 {
-                    "aantal": 7.06,
+                    "aantal": 3.56,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken"
+                        "naam": "Zolder"
                     }
                 },
                 {
-                    "aantal": 6.92,
+                    "aantal": 2.86,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Wasruimte"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
-                    "code": "OOZ",
-                    "naam": "Oppervlakte van overige ruimten"
-                }
-            },
-            "punten": 0.0,
-            "woningwaarderingen": []
-        },
-        {
-            "criteriumGroep": {
-                "stelsel": {
-                    "code": "ZEL",
-                    "naam": "Zelfstandige woonruimten"
-                },
-                "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 14.0,
+            "punten": 11.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
-                    },
-                    "punten": 2.0
-                },
-                {
-                    "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Wasruimte"
                     },
-                    "punten": 2.0
+                    "punten": 1.0
                 },
                 {
                     "criterium": {
                         "naam": "Keuken"
                     },
                     "punten": 2.0
                 },
@@ -167,15 +162,15 @@
                     "naam": "Energieprestatie"
                 }
             },
             "punten": 32.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "A (oud)"
+                        "naam": "B + 78.84m2"
                     },
                     "punten": 32.0
                 }
             ]
         },
         {
             "criteriumGroep": {
@@ -184,39 +179,51 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "SAN",
                     "naam": "Sanitair"
                 }
             },
-            "punten": 9.0,
+            "punten": 4.0,
             "woningwaarderingen": [
                 {
                     "aantal": 1.0,
                     "criterium": {
-                        "naam": "Closetcombinatie"
-                    },
-                    "punten": 3.0
-                },
-                {
-                    "aantal": 2.0,
-                    "criterium": {
-                        "naam": "Wastafel"
+                        "naam": "Douche"
                     },
-                    "punten": 2.0
+                    "punten": 4.0
+                }
+            ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
                 },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 7.0,
+            "woningwaarderingen": [
                 {
-                    "aantal": 1.0,
+                    "aantal": 2507.0,
                     "criterium": {
-                        "naam": "Douche"
+                        "meeteenheid": {
+                            "code": "MLM",
+                            "naam": "Millimeter"
+                        },
+                        "naam": "Lengte aanrecht"
                     },
-                    "punten": 4.0
+                    "punten": 7.0
                 }
             ]
         }
     ],
-    "punten": 115.0,
+    "punten": 117.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8055555555555557%*

 * *Differences: {"'groepen'": "{insert: [(5, OrderedDict([('criteriumGroep', OrderedDict([('stelsel', "*

 * *              "OrderedDict([('code', 'ZEL'), ('naam', 'Zelfstandige woonruimten')])), "*

 * *              "('stelselgroep', OrderedDict([('code', 'KEU'), ('naam', 'Keuken')]))])), ('punten', "*

 * *              "7.0), ('woningwaarderingen', [OrderedDict([('aantal', 3000.0), ('criterium', "*

 * *              "OrderedDict([('naam', 'Lengte aanrecht'), ('meeteenheid', OrderedDict([('code', "*

 * *              "'MLM'), ('naam', 'Millimeter' […]*

```diff
@@ -213,15 +213,41 @@
                     "aantal": 1.0,
                     "criterium": {
                         "naam": "Douche"
                     },
                     "punten": 4.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 7.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 3000.0,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "MLM",
+                            "naam": "Millimeter"
+                        },
+                        "naam": "Lengte aanrecht"
+                    },
+                    "punten": 7.0
+                }
+            ]
         }
     ],
-    "punten": 96.0,
+    "punten": 103.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8055555555555557%*

 * *Differences: {"'groepen'": "{insert: [(5, OrderedDict([('criteriumGroep', OrderedDict([('stelsel', "*

 * *              "OrderedDict([('code', 'ZEL'), ('naam', 'Zelfstandige woonruimten')])), "*

 * *              "('stelselgroep', OrderedDict([('code', 'KEU'), ('naam', 'Keuken')]))])), ('punten', "*

 * *              "7.0), ('woningwaarderingen', [OrderedDict([('aantal', 3600.0), ('criterium', "*

 * *              "OrderedDict([('naam', 'Lengte aanrecht'), ('meeteenheid', OrderedDict([('code', "*

 * *              "'MLM'), ('naam', 'Millimeter' […]*

```diff
@@ -209,15 +209,41 @@
                     "aantal": 1.0,
                     "criterium": {
                         "naam": "Douche"
                     },
                     "punten": 4.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 7.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 3600.0,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "MLM",
+                            "naam": "Millimeter"
+                        },
+                        "naam": "Lengte aanrecht"
+                    },
+                    "punten": 7.0
+                }
+            ]
         }
     ],
-    "punten": 143.0,
+    "punten": 150.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json`

 * *Files 1% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8055555555555557%*

 * *Differences: {"'groepen'": "{insert: [(5, OrderedDict([('criteriumGroep', OrderedDict([('stelsel', "*

 * *              "OrderedDict([('code', 'ZEL'), ('naam', 'Zelfstandige woonruimten')])), "*

 * *              "('stelselgroep', OrderedDict([('code', 'KEU'), ('naam', 'Keuken')]))])), ('punten', "*

 * *              "4.0), ('woningwaarderingen', [OrderedDict([('aantal', 1800.0), ('criterium', "*

 * *              "OrderedDict([('naam', 'Lengte aanrecht'), ('meeteenheid', OrderedDict([('code', "*

 * *              "'MLM'), ('naam', 'Millimeter' […]*

```diff
@@ -203,15 +203,41 @@
                     "aantal": 1.0,
                     "criterium": {
                         "naam": "Douche"
                     },
                     "punten": 4.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 4.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 1800.0,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "MLM",
+                            "naam": "Millimeter"
+                        },
+                        "naam": "Lengte aanrecht"
+                    },
+                    "punten": 4.0
+                }
+            ]
         }
     ],
-    "punten": 140.0,
+    "punten": 144.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7726948302469135%*

 * *Differences: {"'groepen'": "{0: {'punten': 61.0, 'woningwaarderingen': {0: {'aantal': 11.88}, 1: {'aantal': "*

 * *              "9.73}, 2: {'aantal': 22.85}, 3: {'aantal': 3.94, 'criterium': {'naam': "*

 * *              "'Badruimte'}}, 4: {'aantal': 12.22, 'criterium': {'naam': 'Keuken'}}}}, 1: "*

 * *              "{'punten': 3.0, 'woningwaarderingen': {0: {'aantal': 4.41, 'criterium': {'naam': "*

 * *              "'Berging'}}, delete: [0]}}, 2: {'punten': 10.0, 'woningwaarderingen': {3: "*

 * *              "{'criterium': {'naam': 'Badruim […]*

```diff
@@ -7,64 +7,64 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 58.0,
+            "punten": 61.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 11.63,
+                    "aantal": 11.88,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 7.62,
+                    "aantal": 9.73,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 17.77,
+                    "aantal": 22.85,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 12.72,
+                    "aantal": 3.94,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 8.34,
+                    "aantal": 12.22,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Keuken"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -72,34 +72,24 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 4.5,
+            "punten": 3.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 3.56,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Zolder"
-                    }
-                },
-                {
-                    "aantal": 2.86,
+                    "aantal": 4.41,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Wasruimte"
+                        "naam": "Berging"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -107,15 +97,15 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 11.0,
+            "punten": 10.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
@@ -129,27 +119,21 @@
                     "criterium": {
                         "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Wasruimte"
-                    },
-                    "punten": 1.0
-                },
-                {
-                    "criterium": {
-                        "naam": "Keuken"
+                        "naam": "Badruimte"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Keuken"
                     },
                     "punten": 2.0
                 }
             ]
         },
         {
             "criteriumGroep": {
@@ -158,46 +142,86 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "ENE",
                     "naam": "Energieprestatie"
                 }
             },
-            "punten": 32.0,
+            "punten": 15.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "B + 78.84m2"
+                        "naam": "C (oud)"
                     },
-                    "punten": 32.0
+                    "punten": 15.0
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "SAN",
                     "naam": "Sanitair"
                 }
             },
-            "punten": 4.0,
+            "punten": 9.0,
             "woningwaarderingen": [
                 {
                     "aantal": 1.0,
                     "criterium": {
+                        "naam": "Closetcombinatie"
+                    },
+                    "punten": 3.0
+                },
+                {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Wastafel"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "aantal": 1.0,
+                    "criterium": {
                         "naam": "Douche"
                     },
                     "punten": 4.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 7.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 2100.0,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "MLM",
+                            "naam": "Millimeter"
+                        },
+                        "naam": "Lengte aanrecht"
+                    },
+                    "punten": 7.0
+                }
+            ]
         }
     ],
-    "punten": 110.0,
+    "punten": 105.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8055555555555557%*

 * *Differences: {"'groepen'": "{insert: [(5, OrderedDict([('criteriumGroep', OrderedDict([('stelsel', "*

 * *              "OrderedDict([('code', 'ZEL'), ('naam', 'Zelfstandige woonruimten')])), "*

 * *              "('stelselgroep', OrderedDict([('code', 'KEU'), ('naam', 'Keuken')]))])), ('punten', "*

 * *              "7.0), ('woningwaarderingen', [OrderedDict([('aantal', 2100.0), ('criterium', "*

 * *              "OrderedDict([('naam', 'Lengte aanrecht'), ('meeteenheid', OrderedDict([('code', "*

 * *              "'MLM'), ('naam', 'Millimeter' […]*

```diff
@@ -176,15 +176,41 @@
                     "aantal": 1.0,
                     "criterium": {
                         "naam": "Closetcombinatie"
                     },
                     "punten": 3.0
                 }
             ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 7.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 2100.0,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "MLM",
+                            "naam": "Millimeter"
+                        },
+                        "naam": "Lengte aanrecht"
+                    },
+                    "punten": 7.0
+                }
+            ]
         }
     ],
-    "punten": 79.0,
+    "punten": 86.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json` & `woningwaardering-0.4.0a0/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json`

 * *Files 20% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.771164021164021%*

 * *Differences: {"'groepen'": "{0: {'punten': 140.0, 'woningwaarderingen': {0: {'aantal': 21.05}, 3: {'aantal': "*

 * *              "6.5}, 4: {'aantal': 15.98, 'criterium': {'naam': 'Slaapkamer'}}, 5: {'aantal': "*

 * *              "19.15, 'criterium': {'naam': 'Slaapkamer'}}, 6: {'aantal': 15.82}, insert: [(1, "*

 * *              "OrderedDict([('aantal', 41.0), ('criterium', OrderedDict([('naam', 'Woonkamer'), "*

 * *              "('meeteenheid', OrderedDict([('code', 'M2'), ('naam', 'Vierkante meter, "*

 * *              "m2')]))]))])), (2,  […]*

```diff
@@ -7,58 +7,78 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 53.0,
+            "punten": 140.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 11.65,
+                    "aantal": 21.05,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 3.12,
+                    "aantal": 41.0,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 6.37,
+                    "aantal": 20.37,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 23.1,
+                    "aantal": 6.5,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer"
+                        "naam": "Badruimte"
+                    }
+                },
+                {
+                    "aantal": 15.98,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 8.35,
+                    "aantal": 19.15,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Slaapkamer"
+                    }
+                },
+                {
+                    "aantal": 15.82,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
@@ -72,18 +92,18 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 3.75,
+            "punten": 5.25,
             "woningwaarderingen": [
                 {
-                    "aantal": 5.25,
+                    "aantal": 6.65,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Berging"
                     }
@@ -97,37 +117,49 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 10.0,
+            "punten": 14.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Keuken"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Badruimte"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "criterium": {
+                        "naam": "Slaapkamer"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "criterium": {
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
@@ -142,38 +174,86 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "ENE",
                     "naam": "Energieprestatie"
                 }
             },
-            "punten": 0.0,
+            "punten": 22.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Bouwjaar 1898"
+                        "naam": "C (oud)"
                     },
-                    "punten": 0.0
+                    "punten": 22.0
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "SAN",
                     "naam": "Sanitair"
                 }
             },
-            "punten": 0.0,
-            "woningwaarderingen": []
+            "punten": 16.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 2.0,
+                    "criterium": {
+                        "naam": "Closetcombinatie"
+                    },
+                    "punten": 6.0
+                },
+                {
+                    "aantal": 3.0,
+                    "criterium": {
+                        "naam": "Wastafel"
+                    },
+                    "punten": 3.0
+                },
+                {
+                    "aantal": 1.0,
+                    "criterium": {
+                        "naam": "Bad en Douche in zelfde ruimte"
+                    },
+                    "punten": 7.0
+                }
+            ]
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "KEU",
+                    "naam": "Keuken"
+                }
+            },
+            "punten": 7.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 2700.0,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "MLM",
+                            "naam": "Millimeter"
+                        },
+                        "naam": "Lengte aanrecht"
+                    },
+                    "punten": 7.0
+                }
+            ]
         }
     ],
-    "punten": 67.0,
+    "punten": 204.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/config/test_config.py` & `woningwaardering-0.4.0a0/tests/stelsels/config/test_config.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py` & `woningwaardering-0.4.0a0/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 
 @pytest.mark.parametrize(
     "peildatum, stelsel, aantal_geldige_stelselgroepen",
     [
         (
             date(2025, 1, 1),
             Woningwaarderingstelsel.zelfstandige_woonruimten,
-            5,
+            6,
         )
     ],
 )
 def test_select_geldige_stelselgroepen(
     peildatum, stelsel, aantal_geldige_stelselgroepen
 ):
     geldigige_stelselgroepen = Stelsel.select_geldige_stelselgroepen(
```

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py` & `woningwaardering-0.4.0a0/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/test_ZelfstandigeWoonruimten.py` & `woningwaardering-0.4.0a0/tests/stelsels/test_ZelfstandigeWoonruimten.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/utils/test_import_class.py` & `woningwaardering-0.4.0a0/tests/stelsels/utils/test_import_class.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/utils/test_is_geldig.py` & `woningwaardering-0.4.0a0/tests/stelsels/utils/test_is_geldig.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/energieprestatie/test_Energieprestatie.py` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/energieprestatie/test_Energieprestatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/bad_en_douche.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/bad_en_douche.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/twee_bad_en_douche.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/data/input/twee_bad_en_douche.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/sanitair/test_Sanitair.py` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/sanitair/test_Sanitair.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py` & `woningwaardering-0.4.0a0/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 
 import pytest
 from test_utils import assert_output_model, laad_specifiek_input_en_output_model
 
-from woningwaardering.stelsels.zelfstandige_woonruimten.verwarming.verwarming import (
+from woningwaardering.stelsels.zelfstandige_woonruimten.verwarming import (
     Verwarming,
 )
 from woningwaardering.vera.bvg.generated import (
     WoningwaarderingResultatenWoningwaarderingGroep,
 )
 from woningwaardering.vera.referentiedata import Woningwaarderingstelselgroep
```

### Comparing `woningwaardering-0.3.0a7/tests/test_utils.py` & `woningwaardering-0.4.0a0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt` & `woningwaardering-0.4.0a0/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/__init__.py` & `woningwaardering-0.4.0a0/woningwaardering/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/config/config.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/config/config.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml`

 * *Files 15% similar despite different names*

```diff
@@ -37,7 +37,15 @@
     module: sanitair
     class_naam: Sanitair
     begindatum: 2024-01-01
     versies:
       - module: sanitair_2024
         class_naam: Sanitair2024
         begindatum: 2024-01-01
+  keuken:
+    module: keuken
+    class_naam: Keuken
+    begindatum: 2024-01-01
+    versies:
+      - module: keuken_2024
+        class_naam: Keuken2024
+        begindatum: 2024-01-01
```

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/stelsel.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/stelsel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/stelselgroep.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/stelselgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/stelselgroepversie.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/stelselgroepversie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/utils.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/utils.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/sanitair.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/sanitair.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/sanitair_2024.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/sanitair_2024.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py` & `woningwaardering-0.4.0a0/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2` & `woningwaardering-0.4.0a0/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2` & `woningwaardering-0.4.0a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2` & `woningwaardering-0.4.0a0/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/bvg/generated.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/bvg/generated.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_energieprestatie.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_energieprestatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/__init__.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/aanbiedingstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/aanbiedingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/accountstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/accountstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/adressoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/adressoort.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 class Adressoort(Enum):
     buitenlands_adres = Referentiedata(
         code="BUI",
         naam="Buitenlands adres",
     )
     """
-    Een buitenlands adres
+    Een buitenlands adres.
     """
 
     eenheid_adres = Referentiedata(
         code="EEN",
         naam="Eenheid adres",
     )
     """
```

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/afletterstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/afletterstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/afrekenwijzesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/afrekenwijzesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/afspraakstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/afspraakstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/afwezigheidsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/afwezigheidsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/aktesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/aktesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/authentiekgegevenbron.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/authentiekgegevenbron.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/authentiekgegevensoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/authentiekgegevensoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/bedrijfsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/bedrijfsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/begrotingversie.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/begrotingversie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/bestemming.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/bestemming.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/betaalgegevensoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/betaalgegevensoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/betaalwijzesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/betaalwijzesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/betalingsregelingstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/betalingsregelingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/boekingdetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/boekingdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/boekingsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/boekingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/boekingstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/boekingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/boekjaarstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/boekjaarstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/brandwerendheidscore.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/brandwerendheidscore.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/btw.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/btw.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/btwaangiftestatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/btwaangiftestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/burgerlijkestaat.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/burgerlijkestaat.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/clustersoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/clustersoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/collectiefobjectsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/collectiefobjectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/communicatiekanaal.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/communicatiekanaal.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/communicatierichting.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/communicatierichting.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/conditiescore.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/conditiescore.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/contactgegevensoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/contactgegevensoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/contactgegevenstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/contactgegevenstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/crediteursoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/crediteursoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/crediteurstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/crediteurstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/dagdeel.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/dagdeel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/debiteursoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/debiteursoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/debiteurstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/debiteurstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/defectlocatie.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/defectlocatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/defectoorzaak.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/defectoorzaak.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/defectsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/defectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/defectstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/defectstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/doelgroep.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/doelgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/dossier/__init__.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/dossier/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheiddetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheiddetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheiddetailstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheiddetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidinterieur.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidinterieur.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidisolatie.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidisolatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidligging.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidligging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidmonument.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidmonument.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidprijsconditie.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidprijsconditie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidsanitair.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidsanitair.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eenheidstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eenheidstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eindedetailreden.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eindedetailreden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/eindereden.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/eindereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/energielabel.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/energielabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/energieprestatiesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/energieprestatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/energieprestatiestatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/energieprestatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/externeincassosoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/externeincassosoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/externeincassostatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/externeincassostatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/factuurbetaalwijze.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/factuurbetaalwijze.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/factuursoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/factuursoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/financien/__init__.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/financien/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/gebeurtenissoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/gebeurtenissoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/geometriesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/geometriesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/geslacht.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/signaleringsoort.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,35 +1,31 @@
 from enum import Enum
 from woningwaardering.vera.bvg.generated import Referentiedata
 
 
-class Geslacht(Enum):
-    mannelijk = Referentiedata(
-        code="M",
-        naam="Mannelijk",
+class Signaleringsoort(Enum):
+    agressie = Referentiedata(
+        code="AGR",
+        naam="Agressie",
     )
-    """
-    Mannelijk geslacht
-    """
-
-    neutraal = Referentiedata(
-        code="N",
-        naam="Neutraal",
+
+    oneigenlijk_gebruik_woning = Referentiedata(
+        code="ONE",
+        naam="Oneigenlijk gebruik woning",
+    )
+
+    overlast = Referentiedata(
+        code="OVE",
+        naam="Overlast",
     )
-    """
-    Gender-neutraal
-    """
-
-    vrouwelijk = Referentiedata(
-        code="V",
-        naam="Vrouwelijk",
+
+    huurschuld = Referentiedata(
+        code="SCH",
+        naam="Huurschuld",
     )
-    """
-    Vrouwelijk geslacht
-    """
 
     @property
     def code(self) -> str:
         if self.value.code is None:
             raise TypeError("de code van een Referentiedata object mag niet None zijn")
         return self.value.code
```

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/huurgeschilsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/huurgeschilsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/huurgeschilstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/huurgeschilstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/huurklasse.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/huurklasse.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/huuropzeggingstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/huuropzeggingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/incassomoment.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/incassomoment.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inexploitatiereden.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inexploitatiereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/informatieobjectsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/informatieobjectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inkomensbron.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inkomensbron.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inkomenssoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inkomenssoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inschrijvingherkomst.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inschrijvingherkomst.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inspectierapportsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inspectierapportsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/inspectierapportstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/inspectierapportstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/kandidaatstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/kandidaatstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/kwaliteitsniveau.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/kwaliteitsniveau.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/leningaflosvorm.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/leningaflosvorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/leningdetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/leningdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/leningsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/leningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/maatschappelijklabel.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/maatschappelijklabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/machtigingsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/machtigingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/materiaaldetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/materiaaldetailsoort.py`

 * *Files 4% similar despite different names*

```diff
@@ -1494,142 +1494,142 @@
         ),
     )
 
     plantaardige_vezel = Referentiedata(
         code="PTA",
         naam="Plantaardige-Vezel",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     bamboe = Referentiedata(
         code="BAM",
         naam="Bamboe",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     hennep = Referentiedata(
         code="HEN",
         naam="Hennep",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     jute = Referentiedata(
         code="JUT",
         naam="Jute",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     katoen = Referentiedata(
         code="KAT",
         naam="Katoen",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     kurk = Referentiedata(
         code="KUR",
         naam="Kurk",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     mais = Referentiedata(
         code="MAI",
         naam="Mais",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     papier = Referentiedata(
         code="PAP",
         naam="Papier",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     riet = Referentiedata(
         code="RIE",
         naam="Riet",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     stro = Referentiedata(
         code="STR",
         naam="Stro",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     vegetatie = Referentiedata(
         code="VEG",
         naam="Vegetatie",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     vilt = Referentiedata(
         code="VIL",
         naam="Vilt",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     vlas = Referentiedata(
         code="VLA",
         naam="Vlas",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     wol = Referentiedata(
         code="WOL",
         naam="Wol",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     hard_rubber = Referentiedata(
         code="HRU",
         naam="Hard-Rubber",
         parent=Referentiedata(
-            code="",
-            naam="",
+            code="ORG",
+            naam="Organisch",
         ),
     )
 
     polysulfide = Referentiedata(
         code="PLS",
         naam="Polysulfide",
         parent=Referentiedata(
```

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/materiaalsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/materiaalsoort.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,14 +59,19 @@
     )
 
     ntb = Referentiedata(
         code="NTB",
         naam="Ntb",
     )
 
+    organisch = Referentiedata(
+        code="ORG",
+        naam="Organisch",
+    )
+
     rubber = Referentiedata(
         code="RUB",
         naam="Rubber",
     )
 
     samengesteld = Referentiedata(
         code="SAM",
```

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/medewerkerrol.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/medewerkerrol.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/medewerkersoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/medewerkersoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/meeteenheid.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/meeteenheid.py`

 * *Files 4% similar despite different names*

```diff
@@ -70,14 +70,22 @@
         naam="Uren",
     )
     """
     Aantal uitgedrukt in uren, bijvoorbeeld 2,5 uur werktijd. 15 minuten kan uitgedrukt
     worden in 0,25 uur
     """
 
+    millimeter = Referentiedata(
+        code="MLM",
+        naam="Millimeter",
+    )
+    """
+    De meeteenheid millimeter (UITBREIDING)
+    """
+
     @property
     def code(self) -> str:
         if self.value.code is None:
             raise TypeError("de code van een Referentiedata object mag niet None zijn")
         return self.value.code
 
     @property
```

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoud/__init__.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoud/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudslabel.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudslabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudspecialisme.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudspecialisme.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/opleidingsniveau.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/opleidingsniveau.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/oppervlaktesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/oppervlaktesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/opzegtermijn.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/opzegtermijn.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/organisatievorm.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/organisatievorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/overeenkomstsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/overeenkomstsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/overeenkomststatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/overeenkomststatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/passendheiddetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/passendheiddetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/passendheidssoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/passendheidssoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/prestatieafspraak.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/prestatieafspraak.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/prijscomponentsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/prijscomponentsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/projectsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/projectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/projectstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/projectstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/provincie.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/provincie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/publicatiedetailmodel.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/publicatiedetailmodel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/publicatiedetailstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/publicatiedetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/publicatieintakevorm.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/publicatieintakevorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/publicatiemodel.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/publicatiemodel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/publicatiestatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/publicatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/puntenberekeningsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/puntenberekeningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/puntenmutatiesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/puntenmutatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/reclamatiesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/reclamatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/reclamatiestatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/reclamatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/redenontbinding.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/redenontbinding.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/redenopzegging.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/redenopzegging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/redenvernietiging.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/redenvernietiging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/regiesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/regiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/relatieadressoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/relatieadressoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/relatiedetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/relatiedetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/relatierolsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/relatierolsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/relaties/__init__.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/relaties/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/relatiesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/relatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/relatiestatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/relatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/rentesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/rentesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/ruimtedetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/ruimtedetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/ruimteligging.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/ruimteligging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/ruimtesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/ruimtesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/sanctiesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/sanctiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/sanctiestatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/sanctiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/signaleringdetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/signaleringdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/signaleringsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/signaleringstatus.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,25 @@
 from enum import Enum
 from woningwaardering.vera.bvg.generated import Referentiedata
 
 
-class Signaleringsoort(Enum):
-    agressie = Referentiedata(
-        code="AGR",
-        naam="Agressie",
+class Signaleringstatus(Enum):
+    actief = Referentiedata(
+        code="ACT",
+        naam="Actief",
     )
 
-    oneigenlijk_gebruik_woning = Referentiedata(
-        code="ONE",
-        naam="Oneigenlijk gebruik woning",
+    passief = Referentiedata(
+        code="PAS",
+        naam="Passief",
     )
 
-    overlast = Referentiedata(
-        code="OVE",
-        naam="Overlast",
-    )
-
-    huurschuld = Referentiedata(
-        code="SCH",
-        naam="Huurschuld",
+    vervallen = Referentiedata(
+        code="VER",
+        naam="Vervallen",
     )
 
     @property
     def code(self) -> str:
         if self.value.code is None:
             raise TypeError("de code van een Referentiedata object mag niet None zijn")
         return self.value.code
```

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/signaleringstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/verbijzonderingstatus.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from enum import Enum
 from woningwaardering.vera.bvg.generated import Referentiedata
 
 
-class Signaleringstatus(Enum):
+class Verbijzonderingstatus(Enum):
     actief = Referentiedata(
         code="ACT",
         naam="Actief",
     )
 
-    passief = Referentiedata(
-        code="PAS",
-        naam="Passief",
+    geblokkeerd = Referentiedata(
+        code="BLK",
+        naam="Geblokkeerd",
     )
 
-    vervallen = Referentiedata(
-        code="VER",
-        naam="Vervallen",
+    historisch = Referentiedata(
+        code="HIS",
+        naam="Historisch",
     )
 
     @property
     def code(self) -> str:
         if self.value.code is None:
             raise TypeError("de code van een Referentiedata object mag niet None zijn")
         return self.value.code
```

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/taal.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/taal.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/uitexploitatiereden.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/uitexploitatiereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/uitvoerendesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/uitvoerendesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/vastgoed/__init__.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/vastgoed/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/verantwoordingregime.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/verantwoordingregime.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/verbijzonderingsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/verbijzonderingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/verbijzonderingstatus.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/zaakobjectsoort.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,35 @@
 from enum import Enum
 from woningwaardering.vera.bvg.generated import Referentiedata
 
 
-class Verbijzonderingstatus(Enum):
-    actief = Referentiedata(
-        code="ACT",
-        naam="Actief",
+class Zaakobjectsoort(Enum):
+    cluster = Referentiedata(
+        code="CLU",
+        naam="Cluster",
     )
 
-    geblokkeerd = Referentiedata(
-        code="BLK",
-        naam="Geblokkeerd",
+    collectief_object = Referentiedata(
+        code="COL",
+        naam="Collectief object",
     )
 
-    historisch = Referentiedata(
-        code="HIS",
-        naam="Historisch",
+    eenheid = Referentiedata(
+        code="EEN",
+        naam="Eenheid",
+    )
+
+    onderhoudsverzoek = Referentiedata(
+        code="OND",
+        naam="Onderhoudsverzoek",
+    )
+
+    overeenkomst = Referentiedata(
+        code="OVE",
+        naam="Overeenkomst",
     )
 
     @property
     def code(self) -> str:
         if self.value.code is None:
             raise TypeError("de code van een Referentiedata object mag niet None zijn")
         return self.value.code
```

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/verrekeningsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/verrekeningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/vertrouwelijkheid.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/vertrouwelijkheid.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/voorrangdetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/voorrangdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/voorrangsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/voorrangsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/woningtype.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/woningtype.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/woonsituatiesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/woonsituatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/woonvorm.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/woonvorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/zaakrol.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/zaakrol.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/zaakstatussoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/zaakstatussoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/zaaktypesoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/zaaktypesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/referentiedata_uitbreiding.csv` & `woningwaardering-0.4.0a0/woningwaardering/vera/referentiedata_uitbreiding.csv`

 * *Files 6% similar despite different names*

```diff
@@ -2,7 +2,8 @@
 RUIMTEDETAILSOORT;OVL;Overloop;Verkeersruimte: (UITBREIDING) Gang op een bovenverdieping.;3-4-2024;;RUIMTESOORT.OVR;Vastgoed
 RUIMTEDETAILSOORT;ENT;Entree;Verkeersruimte: (UITBREIDING) Ingang van een gebouw.;3-4-2024;;RUIMTESOORT.OVR;Vastgoed
 RUIMTEDETAILSOORT;KAS;Kast;Overige ruimte: (UITBREIDING);8-4-2024;;RUIMTESOORT.OVR;Vastgoed
 WONINGTYPE;EGW;Eengezinswoning;Een woning die tevens een geheel pand vormt.;6-5-2024;;EENHEIDSOORT.WOO;Vastgoed
 WONINGTYPE;MGW;Meergezinswoning;Een woning die samen met andere woonruimten c.q. bedrijfsruimten een geheel pand vormt.;6-5-2024;;EENHEIDSOORT.WOO;Vastgoed
 BOUWKUNDIGELEMENTDETAILSOORT;BID;Bidet;Een bidet (UITBREIDING).;17-5-2024;;BOUWKUNDIGELEMENTSOORT.VOO;Vastgoed
 BOUWKUNDIGELEMENTDETAILSOORT;LAV;Lavet;Een Lavet (UITBREIDING).;17-5-2024;;BOUWKUNDIGELEMENTSOORT.VOO;Vastgoed
+MEETEENHEID;MLM;Millimeter;De meeteenheid millimeter (UITBREIDING);14-04-2024;;;
```

### Comparing `woningwaardering-0.3.0a7/woningwaardering/vera/utils.py` & `woningwaardering-0.4.0a0/woningwaardering/vera/utils.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.3.0a7/woningwaardering.egg-info/PKG-INFO` & `woningwaardering-0.4.0a0/woningwaardering.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: woningwaardering
-Version: 0.3.0a7
+Version: 0.4.0a0
 Summary: Berekent de punten van een woning op basis van het woningwaarderingsstelsel.
 Author-email: Woonstad Rotterdam <info@woonstadrotterdam.nl>, Ben Verhees <ben.verhees@woonstadrotterdam.nl>, Tiddo Loos <tiddo.loos@woonstadrotterdam.nl>, Tomer Gabay <tomer.gabay@woonstadrotterdam.nl>
 Project-URL: Homepage, https://github.com/woonstadrotterdam/woningwaardering
 Project-URL: Issues, https://github.com/woonstadrotterdam/woningwaardering/issues
 Keywords: woning,waardering,stelsel,woningwaarderingsstelsel,wws
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -348,13 +348,17 @@
 
 ### Eenheidklimaatbeheersingsoort
 
 Om te bepalen of de ruimten van een eenheid als individueel of collectief verwarmd gewaardeerd dienen te worden, mist de VERA standaard een veld voor de `Eenheidklimaatbeheersingsoort` referentiedata. Dit attribuut is toegevoegd aan `EenhedenEenheid`.  
 Om dit attribuut ook aan de VERA standaard toe te voegen is
 https://github.com/Aedes-datastandaarden/vera-openapi/issues/54 aangemaakt.
 
+### Bidet en Lavet
+
+In het beleidshandboek van de huurcomissie voor het woningwaardeeringstelsel wordt voor zowel een bidet als een lavet één punt toegekend. In de huidige referentiedata ontbreken deze twee type `bouwkundigelementdetailsoort`. Zie [dit issue](https://github.com/Aedes-datastandaarden/vera-referentiedata/issues/104).
+
 ### Verwarmd
 
 In de VERA standaard is nog geen mogelijkheid om aan te geven of een ruimte verwarmd is. Het attribuut `verwarmde_vertrekken_aantal` bestaat wel, maar dit bestaat op niveau van de eenheid en daarin bestaat geen onderscheid tussen vertrekken en overige ruimten. Dit is aangekaart in deze twee issues:
 
 - https://github.com/Aedes-datastandaarden/vera-openapi/issues/41
 - https://github.com/Aedes-datastandaarden/vera-referentiedata/issues/100
```

### Comparing `woningwaardering-0.3.0a7/woningwaardering.egg-info/SOURCES.txt` & `woningwaardering-0.4.0a0/woningwaardering.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -78,14 +78,28 @@
 tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json
 tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.md
 tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json
 tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.md
 tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_A++++_egw.json
 tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_egw.json
 tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_mgw.json
+tests/stelsels/zelfstandige_woonruimten/keuken/test_Keuken.py
+tests/stelsels/zelfstandige_woonruimten/keuken/data/input/aanrecht_1.json
+tests/stelsels/zelfstandige_woonruimten/keuken/data/input/aanrecht_2.json
+tests/stelsels/zelfstandige_woonruimten/keuken/data/input/aanrecht_<1.json
+tests/stelsels/zelfstandige_woonruimten/keuken/data/input/aanrecht_en_wandafwerking.json
+tests/stelsels/zelfstandige_woonruimten/keuken/data/input/aanrecht_zonder_lengte.json
+tests/stelsels/zelfstandige_woonruimten/keuken/data/input/woon_slaap_met_aanrecht.json
+tests/stelsels/zelfstandige_woonruimten/keuken/data/input/woon_slaap_met_aanrecht.md
+tests/stelsels/zelfstandige_woonruimten/keuken/data/output/peildatum/2024-01-01/aanrecht_1.json
+tests/stelsels/zelfstandige_woonruimten/keuken/data/output/peildatum/2024-01-01/aanrecht_2.json
+tests/stelsels/zelfstandige_woonruimten/keuken/data/output/peildatum/2024-01-01/aanrecht_<1.json
+tests/stelsels/zelfstandige_woonruimten/keuken/data/output/peildatum/2024-01-01/aanrecht_en_wandafwerking.json
+tests/stelsels/zelfstandige_woonruimten/keuken/data/output/peildatum/2024-01-01/aanrecht_zonder_lengte.json
+tests/stelsels/zelfstandige_woonruimten/keuken/data/output/peildatum/2024-01-01/woon_slaap_met_aanrecht.json
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json
@@ -129,15 +143,14 @@
 tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json
 tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json
 tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json
 tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json
 wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt
 woningwaardering/__init__.py
 woningwaardering/_version.py
-woningwaardering/py.typed
 woningwaardering.egg-info/PKG-INFO
 woningwaardering.egg-info/SOURCES.txt
 woningwaardering.egg-info/dependency_links.txt
 woningwaardering.egg-info/requires.txt
 woningwaardering.egg-info/top_level.txt
 woningwaardering/stelsels/__init__.py
 woningwaardering/stelsels/stelsel.py
@@ -154,14 +167,17 @@
 woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py
 woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py
 woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/bouwjaar_punten.csv
 woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_0-25m2_energielabel_punten.csv
 woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_25-40m2_energielabel_punten.csv
 woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_40m2+_energielabel_punten.csv
 woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oud_energielabel_punten.csv
+woningwaardering/stelsels/zelfstandige_woonruimten/keuken/__init__.py
+woningwaardering/stelsels/zelfstandige_woonruimten/keuken/keuken.py
+woningwaardering/stelsels/zelfstandige_woonruimten/keuken/keuken_2024.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/__init__.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/__init__.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py
 woningwaardering/stelsels/zelfstandige_woonruimten/sanitair/__init__.py
```

