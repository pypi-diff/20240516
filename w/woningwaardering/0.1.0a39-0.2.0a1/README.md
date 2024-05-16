# Comparing `tmp/woningwaardering-0.1.0a39.tar.gz` & `tmp/woningwaardering-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "woningwaardering-0.1.0a39.tar", last modified: Thu May 16 09:02:53 2024, max compression
+gzip compressed data, was "woningwaardering-0.2.0a1.tar", last modified: Thu May 16 13:57:38 2024, max compression
```

## Comparing `woningwaardering-0.1.0a39.tar` & `woningwaardering-0.2.0a1.tar`

### file list

```diff
@@ -1,423 +1,451 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.074685 woningwaardering-0.1.0a39/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.014685 woningwaardering-0.1.0a39/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/.github/workflows/cicd.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4152 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)     2661 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/.python-version
--rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    24064 2024-05-16 09:02:53.074685 woningwaardering-0.1.0a39/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22339 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.014685 woningwaardering-0.1.0a39/docs/afbeeldingen/
--rw-r--r--   0 runner    (1001) docker     (127)    34043 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/docs/afbeeldingen/excel_viewer.png
--rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw
--rw-r--r--   0 runner    (1001) docker     (127)   132221 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/docs/afbeeldingen/oppervlakte_van_vertrekken.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/docs/implementatietoelichting-beleidsboeken/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.014685 woningwaardering-0.1.0a39/docs/implementatietoelichting-beleidsboeken/2024/
--rw-r--r--   0 runner    (1001) docker     (127)    22198 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)     1752 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.014685 woningwaardering-0.1.0a39/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/scripts/genereer_opzet_woningwaarderinggroep.py
--rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/scripts/genereer_test_output.py
--rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/scripts/genereer_vera_referentiedata.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/scripts/uitbreiden_vera_modellen.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:02:53.074685 woningwaardering-0.1.0a39/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/taskfile.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.014685 woningwaardering-0.1.0a39/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/data/input/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.014685 woningwaardering-0.1.0a39/tests/data/input/generiek/
--rw-r--r--   0 runner    (1001) docker     (127)    15724 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/generiek/37101000032.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.018685 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/
--rw-r--r--   0 runner    (1001) docker     (127)    13039 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/12006000004.json
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/12006000004.md
--rw-r--r--   0 runner    (1001) docker     (127)     7475 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/23003000050.json
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/23003000050.md
--rw-r--r--   0 runner    (1001) docker     (127)     4849 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/25048000007.json
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/25048000007.md
--rw-r--r--   0 runner    (1001) docker     (127)    10905 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/28018000044.json
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/28018000044.md
--rw-r--r--   0 runner    (1001) docker     (127)    15804 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/37101000032.json
--rw-r--r--   0 runner    (1001) docker     (127)    13973 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/41027000003.json
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/41027000003.md
--rw-r--r--   0 runner    (1001) docker     (127)    15907 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/41123000005.json
--rw-r--r--   0 runner    (1001) docker     (127)    16414 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/41162000015.json
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/41162000015.md
--rw-r--r--   0 runner    (1001) docker     (127)    12030 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/41164000002.json
--rw-r--r--   0 runner    (1001) docker     (127)    12825 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/51011000042.json
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/51011000042.md
--rw-r--r--   0 runner    (1001) docker     (127)    12126 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/71211000027.json
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/71211000027.md
--rw-r--r--   0 runner    (1001) docker     (127)     9941 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/77795000000.json
--rw-r--r--   0 runner    (1001) docker     (127)    12395 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/81020000003.json
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/81020000003.md
--rw-r--r--   0 runner    (1001) docker     (127)     7340 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/81065000089.json
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/81065000089.md
--rw-r--r--   0 runner    (1001) docker     (127)     7594 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/85651000021.json
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/85651000021.md
--rw-r--r--   0 runner    (1001) docker     (127)     5278 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/87402000003.json
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/87402000003.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.022685 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)     2807 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json
--rw-r--r--   0 runner    (1001) docker     (127)     3023 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json
--rw-r--r--   0 runner    (1001) docker     (127)     3725 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json
--rw-r--r--   0 runner    (1001) docker     (127)     5345 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json
--rw-r--r--   0 runner    (1001) docker     (127)     3650 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json
--rw-r--r--   0 runner    (1001) docker     (127)     3512 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json
--rw-r--r--   0 runner    (1001) docker     (127)     3609 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json
--rw-r--r--   0 runner    (1001) docker     (127)     3381 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json
--rw-r--r--   0 runner    (1001) docker     (127)     3371 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json
--rw-r--r--   0 runner    (1001) docker     (127)     3022 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.022685 woningwaardering-0.1.0a39/tests/stelsels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.022685 woningwaardering-0.1.0a39/tests/stelsels/config/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/config/test_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.022685 woningwaardering-0.1.0a39/tests/stelsels/stelsel/
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.022685 woningwaardering-0.1.0a39/tests/stelsels/stelselgroep/
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/test_ZelfstandigeWoonruimten.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.022685 woningwaardering-0.1.0a39/tests/stelsels/utils/
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/utils/test_import_class.py
--rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/utils/test_is_geldig.py
--rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/utils/test_vind_yaml_bestanden.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.022685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.022685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.026685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.026685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.026685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json
--rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json
--rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.026685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json
--rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.md
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/gedeelde_berging.md
--rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.md
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.md
--rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.026685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.026685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten_individueel.md
--rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.md
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten_individueel.md
--rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.006685 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.030686 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json
--rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py
--rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.030686 woningwaardering-0.1.0a39/wettelijke-documenten/
--rw-r--r--   0 runner    (1001) docker     (127)   116885 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.030686 woningwaardering-0.1.0a39/woningwaardering/
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      414 2024-05-16 09:02:52.000000 woningwaardering-0.1.0a39/woningwaardering/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.030686 woningwaardering-0.1.0a39/woningwaardering/stelsels/
--rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.030686 woningwaardering-0.1.0a39/woningwaardering/stelsels/config/
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/config/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml
--rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/stelsel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/stelselgroep.py
--rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/stelselgroepversie.py
--rw-r--r--   0 runner    (1001) docker     (127)     6775 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.030686 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/
--rw-r--r--   0 runner    (1001) docker     (127)      276 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.034685 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
--rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py
--rw-r--r--   0 runner    (1001) docker     (127)     8554 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.034685 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
--rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py
--rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py
--rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.034685 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py
--rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.010686 woningwaardering-0.1.0a39/woningwaardering/templates/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.010686 woningwaardering-0.1.0a39/woningwaardering/templates/stelsels/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.034685 woningwaardering-0.1.0a39/woningwaardering/templates/stelsels/stelsel/
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/templates/stelsels/stelsel/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.034685 woningwaardering-0.1.0a39/woningwaardering/templates/stelsels/stelsel/stelselgroep/
--rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/templates/stelsels/stelsel/stelselgroep/__init__.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.034685 woningwaardering-0.1.0a39/woningwaardering/vera/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.034685 woningwaardering-0.1.0a39/woningwaardering/vera/bvg/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/bvg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   136654 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/bvg/generated.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.034685 woningwaardering-0.1.0a39/woningwaardering/vera/bvg/model_uitbreidingen/
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py
--rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/bvg/model_uitbreidingen/referentiedata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.070685 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/
--rw-r--r--   0 runner    (1001) docker     (127)    15055 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/aanbiedingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py
--rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/accountstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/adressoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/afletterstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/afrekenwijzesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/afspraakstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/afwezigheidsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/aktesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/authentiekgegevenbron.py
--rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/authentiekgegevensoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/bedrijfsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/begrotingversie.py
--rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/bestemming.py
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/betaalgegevensoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/betaalwijzesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/betalingsregelingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/boekingdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/boekingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/boekingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/boekjaarstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)    27844 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/brandwerendheidscore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/btw.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/btwaangiftestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/burgerlijkestaat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/clustersoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/collectiefobjectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/communicatiekanaal.py
--rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/communicatierichting.py
--rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/conditiescore.py
--rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/contactgegevensoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/contactgegevenstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py
--rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/crediteursoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/crediteurstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/dagdeel.py
--rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/debiteursoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/debiteurstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/defectlocatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/defectoorzaak.py
--rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/defectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/defectstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/doelgroep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.070685 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/dossier/
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/dossier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py
--rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheiddetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheiddetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidinterieur.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidisolatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidligging.py
--rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidmonument.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidprijsconditie.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidsanitair.py
--rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eindedetailreden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eindereden.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.070685 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/energie/
--rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/energie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/energielabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/energieprestatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/energieprestatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/externeincassosoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/externeincassostatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/factuurbetaalwijze.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/factuursoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.070685 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/financien/
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/financien/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/gebeurtenissoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/geometriesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/geslacht.py
--rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py
--rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/huurgeschilsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/huurgeschilstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/huurklasse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/huuropzeggingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/incassomoment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inexploitatiereden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/informatieobjectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inkomensbron.py
--rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inkomenssoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inschrijvingherkomst.py
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inspectierapportsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inspectierapportstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/kandidaatstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.070685 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/kwaliteit/
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/kwaliteit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/kwaliteitsniveau.py
--rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/leningaflosvorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/leningdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/leningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/maatschappelijklabel.py
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/machtigingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    35393 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/materiaaldetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/materiaalsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/medewerkerrol.py
--rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/medewerkersoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/meeteenheid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.070685 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoud/
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudslabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudspecialisme.py
--rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/opleidingsniveau.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/oppervlaktesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/opzegtermijn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.070685 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/organisatie/
--rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/organisatie/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/organisatievorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.070685 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/overeenkomsten/
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/overeenkomstsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/overeenkomststatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/passendheiddetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/passendheidssoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/prestatieafspraak.py
--rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/prijscomponentsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py
--rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.070685 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/projectontwikkeling/
--rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/projectontwikkeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/projectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/projectstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/provincie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/publicatiedetailmodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/publicatiedetailstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/publicatieintakevorm.py
--rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/publicatiemodel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/publicatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/puntenberekeningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/puntenmutatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/reclamatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/reclamatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/redenontbinding.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/redenopzegging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/redenvernietiging.py
--rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/regiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/relatieadressoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/relatiedetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/relatierolsoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.070685 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/relaties/
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/relaties/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/relatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/relatiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/rentesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)    13384 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/ruimtedetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/ruimteligging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/ruimtesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/sanctiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/sanctiestatus.py
--rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/signaleringdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/signaleringsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/signaleringstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/taal.py
--rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/uitexploitatiereden.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/uitvoerendesoort.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.070685 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/vastgoed/
--rw-r--r--   0 runner    (1001) docker     (127)     2361 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/vastgoed/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/verantwoordingregime.py
--rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/verbijzonderingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/verbijzonderingstatus.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/verrekeningsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/vertrouwelijkheid.py
--rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/voorrangdetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/voorrangsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py
--rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.070685 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/woonruimteverdeling/
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/woonsituatiesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/woonvorm.py
--rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/zaakobjectsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/zaakrol.py
--rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/zaakstatussoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/zaaktypesoort.py
--rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py
--rw-r--r--   0 runner    (1001) docker     (127)      408 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata_uitbreiding.csv
--rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-16 09:02:48.000000 woningwaardering-0.1.0a39/woningwaardering/vera/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:02:53.070685 woningwaardering-0.1.0a39/woningwaardering.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    24064 2024-05-16 09:02:52.000000 woningwaardering-0.1.0a39/woningwaardering.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22024 2024-05-16 09:02:52.000000 woningwaardering-0.1.0a39/woningwaardering.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:02:52.000000 woningwaardering-0.1.0a39/woningwaardering.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      316 2024-05-16 09:02:52.000000 woningwaardering-0.1.0a39/woningwaardering.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 09:02:52.000000 woningwaardering-0.1.0a39/woningwaardering.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.682373 woningwaardering-0.2.0a1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.618373 woningwaardering-0.2.0a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1203 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/.github/workflows/cicd.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4141 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3122 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)     2701 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/.python-version
+-rw-r--r--   0 runner    (1001) docker     (127)     1075 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    24170 2024-05-16 13:57:38.682373 woningwaardering-0.2.0a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22339 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.618373 woningwaardering-0.2.0a1/docs/afbeeldingen/
+-rw-r--r--   0 runner    (1001) docker     (127)    34043 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/docs/afbeeldingen/excel_viewer.png
+-rw-r--r--   0 runner    (1001) docker     (127)    10340 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw
+-rw-r--r--   0 runner    (1001) docker     (127)   132221 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/docs/afbeeldingen/oppervlakte_van_vertrekken.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/docs/implementatietoelichting-beleidsboeken/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.618373 woningwaardering-0.2.0a1/docs/implementatietoelichting-beleidsboeken/2024/
+-rw-r--r--   0 runner    (1001) docker     (127)    33544 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/docs/implementatietoelichting-beleidsboeken/2024/zelfstandige_woonruimten.md
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.622372 woningwaardering-0.2.0a1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     6459 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/scripts/genereer_opzet_woningwaarderinggroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2703 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/scripts/genereer_test_output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8600 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/scripts/genereer_vera_referentiedata.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5732 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/scripts/uitbreiden_vera_modellen.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 13:57:38.682373 woningwaardering-0.2.0a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/taskfile.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.622372 woningwaardering-0.2.0a1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1965 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/tests/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/tests/data/input/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.622372 woningwaardering-0.2.0a1/tests/data/input/generiek/
+-rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/generiek/37101000032.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.626373 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)    13487 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/12006000004.json
+-rw-r--r--   0 runner    (1001) docker     (127)      146 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/12006000004.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8362 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/23003000050.json
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/23003000050.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5740 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/25048000007.json
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/25048000007.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11362 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/28018000044.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/28018000044.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16677 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/37101000032.json
+-rw-r--r--   0 runner    (1001) docker     (127)    14864 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41027000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41027000003.md
+-rw-r--r--   0 runner    (1001) docker     (127)    16792 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41123000005.json
+-rw-r--r--   0 runner    (1001) docker     (127)    17301 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41162000015.json
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41162000015.md
+-rw-r--r--   0 runner    (1001) docker     (127)    12899 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41164000002.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13711 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/51011000042.json
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/51011000042.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13013 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/71211000027.json
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/71211000027.md
+-rw-r--r--   0 runner    (1001) docker     (127)    10811 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/77795000000.json
+-rw-r--r--   0 runner    (1001) docker     (127)    13280 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/81020000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/81020000003.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8305 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/81065000089.json
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/81065000089.md
+-rw-r--r--   0 runner    (1001) docker     (127)     8051 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/85651000021.json
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/85651000021.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5741 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/87402000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/87402000003.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/tests/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.610372 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)     3232 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3444 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4146 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3242 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)     5766 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4071 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3934 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json
+-rw-r--r--   0 runner    (1001) docker     (127)     4030 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3803 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3797 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3211 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/config/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/config/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/stelsel/
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/stelselgroep/
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1133 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/test_ZelfstandigeWoonruimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/utils/test_import_class.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1067 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/utils/test_is_geldig.py
+-rw-r--r--   0 runner    (1001) docker     (127)      257 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/utils/test_vind_yaml_bestanden.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.md
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)       47 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.md
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      450 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_A++++_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_egw.json
+-rw-r--r--   0 runner    (1001) docker     (127)      455 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_mgw.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2006 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/energieprestatie/test_Energieprestatie.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.630373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2225 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.634373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.634373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)      680 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1248 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json
+-rw-r--r--   0 runner    (1001) docker     (127)     2221 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.634373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json
+-rw-r--r--   0 runner    (1001) docker     (127)      303 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.md
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/gedeelde_berging.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1367 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.md
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2115 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.634373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.634373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      252 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten_individueel.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4648 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten_individueel.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4606 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      320 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.634373 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1352 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)      786 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1919 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2979 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.638373 woningwaardering-0.2.0a1/wettelijke-documenten/
+-rw-r--r--   0 runner    (1001) docker     (127)   116885 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.638373 woningwaardering-0.2.0a1/woningwaardering/
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      413 2024-05-16 13:57:38.000000 woningwaardering-0.2.0a1/woningwaardering/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.638373 woningwaardering-0.2.0a1/woningwaardering/stelsels/
+-rw-r--r--   0 runner    (1001) docker     (127)      180 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.638373 woningwaardering-0.2.0a1/woningwaardering/stelsels/config/
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1867 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     4693 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/stelsel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5156 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/stelselgroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)      540 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/stelselgroepversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8737 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.638373 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)      347 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.638373 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11817 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/
+-rw-r--r--   0 runner    (1001) docker     (127)      292 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/bouwjaar_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_0-25m2_energielabel_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      286 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_25-40m2_energielabel_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_40m2+_energielabel_punten.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      318 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oud_energielabel_punten.csv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/
+-rw-r--r--   0 runner    (1001) docker     (127)      248 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8888 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3933 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7042 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/
+-rw-r--r--   0 runner    (1001) docker     (127)      135 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7479 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1119 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/woningwaardering/templates/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.614372 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1055 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelselgroep/
+-rw-r--r--   0 runner    (1001) docker     (127)      380 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelselgroep/__init__.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1144 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1909 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/vera/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.642373 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   137423 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/generated.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.646373 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/model_uitbreidingen/
+-rw-r--r--   0 runner    (1001) docker     (127)      655 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_energieprestatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py
+-rw-r--r--   0 runner    (1001) docker     (127)      432 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/bvg/model_uitbreidingen/referentiedata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/
+-rw-r--r--   0 runner    (1001) docker     (127)    15108 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8181 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aanbiedingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3830 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1095 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/accountstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/adressoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afletterstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afrekenwijzesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1171 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afspraakstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afwezigheidsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aktesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/authentiekgegevenbron.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1769 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/authentiekgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2602 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bedrijfsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/begrotingversie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      902 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bestemming.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betaalgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      950 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betaalwijzesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1270 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1274 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betalingsregelingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3951 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekingdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2591 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1731 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      800 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekjaarstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27844 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2168 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/brandwerendheidscore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1305 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/btw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/btwaangiftestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/burgerlijkestaat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/clustersoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2961 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/collectiefobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/communicatiekanaal.py
+-rw-r--r--   0 runner    (1001) docker     (127)      658 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/communicatierichting.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1691 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/conditiescore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      765 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1175 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevensoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevenstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      652 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3949 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/crediteursoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      901 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/crediteurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/dagdeel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      877 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/debiteursoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/debiteurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4239 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectlocatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2578 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectoorzaak.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6974 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/doelgroep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/dossier/
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/dossier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6190 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1396 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30772 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheiddetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5661 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheiddetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1419 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidinterieur.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidisolatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7032 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1802 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidligging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3171 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidmonument.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidprijsconditie.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidsanitair.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2341 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2965 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eindedetailreden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1314 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eindereden.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energie/
+-rw-r--r--   0 runner    (1001) docker     (127)      259 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1245 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energielabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3469 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energieprestatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energieprestatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      673 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/externeincassosoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/externeincassostatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/factuurbetaalwijze.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/factuursoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/financien/
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/financien/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3108 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/gebeurtenissoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      781 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/geometriesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      844 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/geslacht.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2818 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)      626 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huurgeschilsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huurgeschilstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huurklasse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huuropzeggingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5737 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/incassomoment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2502 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inexploitatiereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1714 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/informatieobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkomensbron.py
+-rw-r--r--   0 runner    (1001) docker     (127)      921 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkomenssoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2272 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1647 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inschrijvingherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inspectierapportsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      917 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inspectierapportstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3348 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1608 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kandidaatstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kwaliteit/
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kwaliteit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kwaliteitsniveau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1005 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/leningaflosvorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/leningdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/leningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1767 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/maatschappelijklabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/machtigingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35393 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/materiaaldetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1701 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/materiaalsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      756 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/medewerkerrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)      993 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/medewerkersoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1845 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/meeteenheid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoud/
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1002 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudslabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2277 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2899 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8627 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudspecialisme.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2247 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2226 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2114 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2821 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/opleidingsniveau.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/oppervlaktesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/opzegtermijn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/organisatie/
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/organisatie/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4052 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/organisatievorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5569 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomsten/
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2894 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomststatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1383 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/passendheiddetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1355 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/passendheidssoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prestatieafspraak.py
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14827 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1319 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1166 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectontwikkeling/
+-rw-r--r--   0 runner    (1001) docker     (127)      435 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectontwikkeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/provincie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1871 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiedetailmodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3537 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiedetailstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatieintakevorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2522 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiemodel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1121 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/puntenberekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2517 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/puntenmutatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      864 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/reclamatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/reclamatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      871 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/redenontbinding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/redenopzegging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/redenvernietiging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2039 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/regiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1028 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatieadressoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      833 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatiedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13143 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatierolsoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relaties/
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relaties/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1250 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      928 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      640 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/rentesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13384 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/ruimtedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/ruimteligging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/ruimtesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/sanctiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/sanctiestatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3077 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/signaleringdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/signaleringsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/signaleringstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      952 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/taal.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2628 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2990 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/uitexploitatiereden.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/uitvoerendesoort.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/vastgoed/
+-rw-r--r--   0 runner    (1001) docker     (127)     2395 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/vastgoed/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verantwoordingregime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3033 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verbijzonderingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      748 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verbijzonderingstatus.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verrekeningsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1307 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/vertrouwelijkheid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5922 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/voorrangdetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1368 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/voorrangsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1049 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woningtype.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14624 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woonruimteverdeling/
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woonsituatiesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2557 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woonvorm.py
+-rw-r--r--   0 runner    (1001) docker     (127)      942 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaakobjectsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaakrol.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1511 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaakstatussoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5290 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1257 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaaktypesoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1838 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py
+-rw-r--r--   0 runner    (1001) docker     (127)      676 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata_uitbreiding.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     1918 2024-05-16 13:57:33.000000 woningwaardering-0.2.0a1/woningwaardering/vera/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 13:57:38.678373 woningwaardering-0.2.0a1/woningwaardering.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    24170 2024-05-16 13:57:38.000000 woningwaardering-0.2.0a1/woningwaardering.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    23957 2024-05-16 13:57:38.000000 woningwaardering-0.2.0a1/woningwaardering.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 13:57:38.000000 woningwaardering-0.2.0a1/woningwaardering.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      355 2024-05-16 13:57:38.000000 woningwaardering-0.2.0a1/woningwaardering.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 13:57:38.000000 woningwaardering-0.2.0a1/woningwaardering.egg-info/top_level.txt
```

### Comparing `woningwaardering-0.1.0a39/.github/workflows/cicd.yml` & `woningwaardering-0.2.0a1/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/.github/workflows/publish-to-pypi.yml` & `woningwaardering-0.2.0a1/.github/workflows/publish-to-pypi.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Publish Python distribution without PR
+name: Publish Python distribution
 
 on:
   push:
     tags:
       - "v*"
 
 jobs:
```

### Comparing `woningwaardering-0.1.0a39/.gitignore` & `woningwaardering-0.2.0a1/.gitignore`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/.pre-commit-config.yaml` & `woningwaardering-0.2.0a1/.pre-commit-config.yaml`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
           [
             pydantic==2.*,
             types-requests==2.*,
             unidecode==1.*,
             PyYAML==6.*,
             types-pyyaml==6.*,
             libcst==1.*,
+            types-python-dateutil==2.*,
           ]
         description: "Mypy is an optional static type checker for Python."
         args:
           ["--strict", "--ignore-missing-imports", "--allow-untyped-decorators"]
         exclude: "tests"
         stages:
           - "pre-push"
```

### Comparing `woningwaardering-0.1.0a39/LICENSE` & `woningwaardering-0.2.0a1/LICENSE`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/PKG-INFO` & `woningwaardering-0.2.0a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: woningwaardering
-Version: 0.1.0a39
+Version: 0.2.0a1
 Summary: Berekent de punten van een woning op basis van het woningwaarderingsstelsel.
-Author: Woonstad Rotterdam
-Author-email: Ben Verhees <ben.verhees@woonstadrotterdam.nl>, Tiddo Loos <tiddo.loos@woonstadrotterdam.nl>, Tomer Gabay <tomer.gabay@woonstadrotterdam.nl>
+Author-email: Woonstad Rotterdam <info@woonstadrotterdam.nl>, Ben Verhees <ben.verhees@woonstadrotterdam.nl>, Tiddo Loos <tiddo.loos@woonstadrotterdam.nl>, Tomer Gabay <tomer.gabay@woonstadrotterdam.nl>
 Project-URL: Homepage, https://github.com/WoonstadRotterdamTemp/woningwaardering
 Project-URL: Issues, https://github.com/WoonstadRotterdamTemp/woningwaardering/issues
 Keywords: woning,waardering,stelsel,woningwaarderingsstelsel,wws
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -16,19 +15,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.*
 Requires-Dist: loguru==0.7.*
 Requires-Dist: types-pyyaml==6.*
 Requires-Dist: PyYAML==6.*
 Requires-Dist: prettytable==3.*
+Requires-Dist: pandas==2.*
 Provides-Extra: test
 Requires-Dist: pre-commit==3.3.*; extra == "test"
 Requires-Dist: ruff==0.3.*; extra == "test"
 Requires-Dist: pytest==8.0.*; extra == "test"
 Requires-Dist: types-requests==2.*; extra == "test"
+Requires-Dist: types-python-dateutil==2.*; extra == "test"
 Provides-Extra: dev
 Requires-Dist: woningwaardering[test]; extra == "dev"
 Requires-Dist: datamodel-code-generator[http]==0.25.5; extra == "dev"
 Requires-Dist: unidecode==1.*; extra == "dev"
 Requires-Dist: jinja2==3.*; extra == "dev"
 Requires-Dist: types-pyyaml==6.*; extra == "dev"
 Requires-Dist: PyYAML==6.*; extra == "dev"
```

### Comparing `woningwaardering-0.1.0a39/README.md` & `woningwaardering-0.2.0a1/README.md`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/docs/afbeeldingen/excel_viewer.png` & `woningwaardering-0.2.0a1/docs/afbeeldingen/excel_viewer.png`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw` & `woningwaardering-0.2.0a1/docs/afbeeldingen/oppervlakte_van_vertrekken.excalidraw`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/docs/afbeeldingen/oppervlakte_van_vertrekken.png` & `woningwaardering-0.2.0a1/docs/afbeeldingen/oppervlakte_van_vertrekken.png`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/pyproject.toml` & `woningwaardering-0.2.0a1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "woningwaardering"
 dynamic = ["version"]
 description = "Berekent de punten van een woning op basis van het woningwaarderingsstelsel."
 authors = [
-    { name = "Woonstad Rotterdam" },
+    { name = "Woonstad Rotterdam", email = "info@woonstadrotterdam.nl"},
     { name = "Ben Verhees", email = "ben.verhees@woonstadrotterdam.nl" },
     { name = "Tiddo Loos", email = "tiddo.loos@woonstadrotterdam.nl" },
     { name = "Tomer Gabay", email = "tomer.gabay@woonstadrotterdam.nl" }
 ]
 keywords = ["woning", "waardering", "stelsel", "woningwaarderingsstelsel", "wws"]
 classifiers = [
     "Programming Language :: Python :: 3.10",
@@ -23,15 +23,16 @@
 readme = {file = "README.md", content-type = "text/markdown"}
 requires-python = ">=3.10"
 dependencies = [
     "pydantic==2.*",
     "loguru==0.7.*",
     "types-pyyaml==6.*",
     "PyYAML==6.*",
-    "prettytable==3.*"
+    "prettytable==3.*",
+    "pandas==2.*"
 ]
 
 [project.urls]
 Homepage = "https://github.com/WoonstadRotterdamTemp/woningwaardering"
 Issues = "https://github.com/WoonstadRotterdamTemp/woningwaardering/issues"
 
 [tool.setuptools.packages.find]
@@ -42,14 +43,15 @@
 
 [project.optional-dependencies]
 test = [
     "pre-commit==3.3.*",
     "ruff==0.3.*",
     "pytest==8.0.*",
     "types-requests==2.*",
+    "types-python-dateutil==2.*",
 ]
 dev = [
     "woningwaardering[test]",
     "datamodel-code-generator[http]==0.25.5",
     "unidecode==1.*",
     "jinja2==3.*",
     "types-pyyaml==6.*",
```

### Comparing `woningwaardering-0.1.0a39/scripts/genereer_opzet_woningwaarderinggroep.py` & `woningwaardering-0.2.0a1/scripts/genereer_opzet_woningwaarderinggroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/scripts/genereer_test_output.py` & `woningwaardering-0.2.0a1/scripts/genereer_test_output.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/scripts/genereer_vera_referentiedata.py` & `woningwaardering-0.2.0a1/scripts/genereer_vera_referentiedata.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/scripts/uitbreiden_vera_modellen.py` & `woningwaardering-0.2.0a1/scripts/uitbreiden_vera_modellen.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,40 +88,40 @@
         )
 
         generated_visitor = GatherClassesVisitor()
         updated_module.visit(generated_visitor)
 
         for module in import_visitor.module_imports:
             if module in generated_visitor.classes.keys():
-                logger.warning(
+                logger.debug(
                     f"`import {module}` wordt niet toegevoegd. Een class met deze naam bestaat al."
                 )
             else:
                 AddImportsVisitor.add_needed_import(
                     codemod_context,
                     module,
                 )
 
         for module, objects in import_visitor.object_mapping.items():
             for obj in objects:
                 if obj in generated_visitor.classes.keys():
-                    logger.warning(
+                    logger.debug(
                         f"`from {module} import {obj}` wordt niet toegevoegd. Een class met deze naam bestaat al."
                     )
                 else:
                     AddImportsVisitor.add_needed_import(
                         codemod_context,
                         module=module,
                         obj=obj,
                     )
 
         for module, import_aliases in import_visitor.alias_mapping.items():
             for obj, asname in import_aliases:
                 if asname in generated_visitor.classes.keys():
-                    logger.info(
+                    logger.debug(
                         f"`from {module} import {obj} as {asname}` wordt niet toegevoegd. Een class met deze naam bestaat al."
                     )
                 else:
                     AddImportsVisitor.add_needed_import(
                         codemod_context,
                         module=module,
                         obj=obj,
```

### Comparing `woningwaardering-0.1.0a39/taskfile.yml` & `woningwaardering-0.2.0a1/taskfile.yml`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/conftest.py` & `woningwaardering-0.2.0a1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/data/input/generiek/37101000032.json` & `woningwaardering-0.2.0a1/tests/data/input/generiek/37101000032.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Nieuwe Boezemstraat'), ('huisnummer', '27'), "*

 * *            "('huisnummer_toevoeging', ''), ('postcode', '3034PH'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000485697'), "*

 * *                                          "('bagIdentificatie', '0599010000485697')])",*

 * * "'energieprestaties'": "[OrderedDict([('soort', OrderedDict([('code', 'EI'), ('naam', "*

 * *                     […]*

```diff
@@ -1,10 +1,49 @@
 {
+    "adres": {
+        "huisnummer": "27",
+        "huisnummer_toevoeging": "",
+        "postcode": "3034PH",
+        "straatnaam": "Nieuwe Boezemstraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000485697",
+        "id": "0599010000485697"
+    },
     "bouwjaar": 1924,
+    "energieprestaties": [
+        {
+            "begindatum": "2019-02-25",
+            "einddatum": "2029-02-25",
+            "energieprestatievergoeding": false,
+            "label": {
+                "code": "C",
+                "naam": "C"
+            },
+            "registratiedatum": "2019-02-26T14:51:38+01:00",
+            "soort": {
+                "code": "EI",
+                "naam": "Energie-index"
+            },
+            "status": {
+                "code": "DEF",
+                "naam": "Definitief"
+            },
+            "waarde": "1.58"
+        }
+    ],
+    "gebruiksoppervlakte": 187,
     "id": "37101000032",
+    "klimaatbeheersingsoort": {
+        "code": "IND",
+        "naam": "Individueel"
+    },
     "ruimten": [
         {
             "detailSoort": {
                 "code": "GAN",
                 "naam": "Gang"
             },
             "gemeenschappelijk": true,
@@ -676,9 +715,13 @@
             "oppervlakte": 0.27936,
             "soort": {
                 "code": "OVR",
                 "naam": "Overige ruimtes"
             },
             "verwarmd": false
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "EGW",
+        "naam": "Eengezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/12006000004.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/12006000004.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Mauritsstraat'), ('huisnummer', '44'), "*

 * *            "('huisnummer_toevoeging', ''), ('postcode', '3012CJ'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000320510'), "*

 * *                                          "('bagIdentificatie', '0599010000320510')])",*

 * * "'bouwjaar'": '1981',*

 * * "'energieprestaties'": '[]',*

 * * "'gebruiksoppervlakte'": '71',*

 * * "'woningtype'": "OrderedDict( […]*

```diff
@@ -1,8 +1,24 @@
 {
+    "adres": {
+        "huisnummer": "44",
+        "huisnummer_toevoeging": "",
+        "postcode": "3012CJ",
+        "straatnaam": "Mauritsstraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000320510",
+        "id": "0599010000320510"
+    },
+    "bouwjaar": 1981,
+    "energieprestaties": [],
+    "gebruiksoppervlakte": 71,
     "id": "12006000004",
     "klimaatbeheersingsoort": {
         "code": "IND",
         "naam": "Individueel"
     },
     "ruimten": [
         {
@@ -546,9 +562,13 @@
             "oppervlakte": 0.3575,
             "soort": {
                 "code": "OVR",
                 "naam": "Overige ruimtes"
             },
             "verwarmd": false
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "MGW",
+        "naam": "Meergezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/23003000050.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/23003000050.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.25%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Vosmaerstraat'), ('huisnummer', '54'), "*

 * *            "('huisnummer_toevoeging', ''), ('postcode', '3027KM'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000090716'), "*

 * *                                          "('bagIdentificatie', '0599010000090716')])",*

 * * "'bouwjaar'": '1921',*

 * * "'energieprestaties'": "[OrderedDict([('soort', OrderedDict([('code', 'EI'), ('naam', "*

 * *    […]*

```diff
@@ -1,8 +1,44 @@
 {
+    "adres": {
+        "huisnummer": "54",
+        "huisnummer_toevoeging": "",
+        "postcode": "3027KM",
+        "straatnaam": "Vosmaerstraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000090716",
+        "id": "0599010000090716"
+    },
+    "bouwjaar": 1921,
+    "energieprestaties": [
+        {
+            "begindatum": "2017-02-23",
+            "einddatum": "2027-02-23",
+            "energieprestatievergoeding": false,
+            "label": {
+                "code": "C",
+                "naam": "C"
+            },
+            "registratiedatum": "2017-02-23T09:55:37+01:00",
+            "soort": {
+                "code": "EI",
+                "naam": "Energie-index"
+            },
+            "status": {
+                "code": "DEF",
+                "naam": "Definitief"
+            },
+            "waarde": "1.48"
+        }
+    ],
+    "gebruiksoppervlakte": 72,
     "id": "23003000050",
     "ruimten": [
         {
             "bouwlaag": {
                 "nummer": "00",
                 "omschrijving": "begane grond"
             },
@@ -318,9 +354,13 @@
             "oppervlakte": 12.219,
             "soort": {
                 "code": "VTK",
                 "naam": "Vertrek"
             },
             "verwarmd": true
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "MGW",
+        "naam": "Meergezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/25048000007.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/25048000007.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Rochussenstraat'), ('huisnummer', '251'), "*

 * *            "('huisnummer_toevoeging', 'c'), ('postcode', '3021NW'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000349626'), "*

 * *                                          "('bagIdentificatie', '0599010000349626')])",*

 * * "'bouwjaar'": '1997',*

 * * "'energieprestaties'": "[OrderedDict([('soort', OrderedDict([('code', 'EI'), ('naam', " […]*

```diff
@@ -1,8 +1,44 @@
 {
+    "adres": {
+        "huisnummer": "251",
+        "huisnummer_toevoeging": "c",
+        "postcode": "3021NW",
+        "straatnaam": "Rochussenstraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000349626",
+        "id": "0599010000349626"
+    },
+    "bouwjaar": 1997,
+    "energieprestaties": [
+        {
+            "begindatum": "2019-07-03",
+            "einddatum": "2029-07-03",
+            "energieprestatievergoeding": false,
+            "label": {
+                "code": "B",
+                "naam": "B"
+            },
+            "registratiedatum": "2019-12-03T16:44:12+01:00",
+            "soort": {
+                "code": "EI",
+                "naam": "Energie-index"
+            },
+            "status": {
+                "code": "DEF",
+                "naam": "Definitief"
+            },
+            "waarde": "1.24"
+        }
+    ],
+    "gebruiksoppervlakte": 79,
     "id": "25048000007",
     "klimaatbeheersingsoort": {
         "code": "IND",
         "naam": "Individueel"
     },
     "ruimten": [
         {
@@ -220,9 +256,13 @@
             "oppervlakte": 1.28113,
             "soort": {
                 "code": "OVR",
                 "naam": "Overige ruimtes"
             },
             "verwarmd": false
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "MGW",
+        "naam": "Meergezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/28018000044.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/28018000044.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Baardsestraat'), ('huisnummer', '14'), "*

 * *            "('huisnummer_toevoeging', ''), ('postcode', '3028RC'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000094913'), "*

 * *                                          "('bagIdentificatie', '0599010000094913')])",*

 * * "'bouwjaar'": '1992',*

 * * "'energieprestaties'": '[]',*

 * * "'gebruiksoppervlakte'": '87',*

 * * "'woningtype'": "OrderedDict( […]*

```diff
@@ -1,8 +1,24 @@
 {
+    "adres": {
+        "huisnummer": "14",
+        "huisnummer_toevoeging": "",
+        "postcode": "3028RC",
+        "straatnaam": "Baardsestraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000094913",
+        "id": "0599010000094913"
+    },
+    "bouwjaar": 1992,
+    "energieprestaties": [],
+    "gebruiksoppervlakte": 87,
     "id": "28018000044",
     "klimaatbeheersingsoort": {
         "code": "IND",
         "naam": "Individueel"
     },
     "ruimten": [
         {
@@ -467,9 +483,13 @@
             "oppervlakte": 13.3481,
             "soort": {
                 "code": "VTK",
                 "naam": "Vertrek"
             },
             "verwarmd": true
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "EGW",
+        "naam": "Eengezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/37101000032.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/37101000032.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4444444444444444%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Nieuwe Boezemstraat'), ('huisnummer', '27'), "*

 * *            "('huisnummer_toevoeging', ''), ('postcode', '3034PH'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000485697'), "*

 * *                                          "('bagIdentificatie', '0599010000485697')])",*

 * * "'energieprestaties'": "[OrderedDict([('soort', OrderedDict([('code', 'EI'), ('naam', "*

 * *                     […]*

```diff
@@ -1,9 +1,44 @@
 {
+    "adres": {
+        "huisnummer": "27",
+        "huisnummer_toevoeging": "",
+        "postcode": "3034PH",
+        "straatnaam": "Nieuwe Boezemstraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000485697",
+        "id": "0599010000485697"
+    },
     "bouwjaar": 1924,
+    "energieprestaties": [
+        {
+            "begindatum": "2019-02-25",
+            "einddatum": "2029-02-25",
+            "energieprestatievergoeding": false,
+            "label": {
+                "code": "C",
+                "naam": "C"
+            },
+            "registratiedatum": "2019-02-26T14:51:38+01:00",
+            "soort": {
+                "code": "EI",
+                "naam": "Energie-index"
+            },
+            "status": {
+                "code": "DEF",
+                "naam": "Definitief"
+            },
+            "waarde": "1.58"
+        }
+    ],
+    "gebruiksoppervlakte": 187,
     "id": "37101000032",
     "klimaatbeheersingsoort": {
         "code": "IND",
         "naam": "Individueel"
     },
     "ruimten": [
         {
@@ -680,9 +715,13 @@
             "oppervlakte": 0.27936,
             "soort": {
                 "code": "OVR",
                 "naam": "Overige ruimtes"
             },
             "verwarmd": false
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "EGW",
+        "naam": "Eengezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/41027000003.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41027000003.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Frits Ruysstraat'), ('huisnummer', '16'), "*

 * *            "('huisnummer_toevoeging', 'd'), ('postcode', '3061ME'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000302054'), "*

 * *                                          "('bagIdentificatie', '0599010000302054')])",*

 * * "'bouwjaar'": '1948',*

 * * "'energieprestaties'": "[OrderedDict([('soort', OrderedDict([('code', 'EI'), ('naam', " […]*

```diff
@@ -1,8 +1,44 @@
 {
+    "adres": {
+        "huisnummer": "16",
+        "huisnummer_toevoeging": "d",
+        "postcode": "3061ME",
+        "straatnaam": "Frits Ruysstraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000302054",
+        "id": "0599010000302054"
+    },
+    "bouwjaar": 1948,
+    "energieprestaties": [
+        {
+            "begindatum": "2019-09-19",
+            "einddatum": "2029-09-19",
+            "energieprestatievergoeding": false,
+            "label": {
+                "code": "E",
+                "naam": "E"
+            },
+            "registratiedatum": "2020-01-31T12:13:24+01:00",
+            "soort": {
+                "code": "EI",
+                "naam": "Energie-index"
+            },
+            "status": {
+                "code": "DEF",
+                "naam": "Definitief"
+            },
+            "waarde": "2.26"
+        }
+    ],
+    "gebruiksoppervlakte": 53,
     "id": "41027000003",
     "klimaatbeheersingsoort": {
         "code": "IND",
         "naam": "Individueel"
     },
     "ruimten": [
         {
@@ -589,9 +625,13 @@
                         "naam": "Overige ruimtes"
                     },
                     "verwarmd": false
                 }
             ],
             "verwarmd": true
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "MGW",
+        "naam": "Meergezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/41123000005.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41123000005.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Plantageweg'), ('huisnummer', '17'), "*

 * *            "('huisnummer_toevoeging', ''), ('postcode', '3061PJ'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000295253'), "*

 * *                                          "('bagIdentificatie', '0599010000295253')])",*

 * * "'bouwjaar'": '1896',*

 * * "'energieprestaties'": "[OrderedDict([('soort', OrderedDict([('code', 'EI'), ('naam', "*

 * *      […]*

```diff
@@ -1,8 +1,44 @@
 {
+    "adres": {
+        "huisnummer": "17",
+        "huisnummer_toevoeging": "",
+        "postcode": "3061PJ",
+        "straatnaam": "Plantageweg",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000295253",
+        "id": "0599010000295253"
+    },
+    "bouwjaar": 1896,
+    "energieprestaties": [
+        {
+            "begindatum": "2019-05-13",
+            "einddatum": "2029-05-13",
+            "energieprestatievergoeding": false,
+            "label": {
+                "code": "B",
+                "naam": "B"
+            },
+            "registratiedatum": "2019-11-21T10:55:31+01:00",
+            "soort": {
+                "code": "EI",
+                "naam": "Energie-index"
+            },
+            "status": {
+                "code": "DEF",
+                "naam": "Definitief"
+            },
+            "waarde": "1.39"
+        }
+    ],
+    "gebruiksoppervlakte": 170,
     "id": "41123000005",
     "klimaatbeheersingsoort": {
         "code": "IND",
         "naam": "Individueel"
     },
     "ruimten": [
         {
@@ -691,9 +727,13 @@
             "oppervlakte": 3.62953,
             "soort": {
                 "code": "OVR",
                 "naam": "Overige ruimtes"
             },
             "verwarmd": false
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "EGW",
+        "naam": "Eengezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/41162000015.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41162000015.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Rubensstraat'), ('huisnummer', '10'), "*

 * *            "('huisnummer_toevoeging', 'c'), ('postcode', '3061ZX'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000302221'), "*

 * *                                          "('bagIdentificatie', '0599010000302221')])",*

 * * "'bouwjaar'": '1949',*

 * * "'energieprestaties'": "[OrderedDict([('soort', OrderedDict([('code', 'EI'), ('naam', "*

 * *    […]*

```diff
@@ -1,8 +1,44 @@
 {
+    "adres": {
+        "huisnummer": "10",
+        "huisnummer_toevoeging": "c",
+        "postcode": "3061ZX",
+        "straatnaam": "Rubensstraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000302221",
+        "id": "0599010000302221"
+    },
+    "bouwjaar": 1949,
+    "energieprestaties": [
+        {
+            "begindatum": "2019-10-11",
+            "einddatum": "2029-10-11",
+            "energieprestatievergoeding": false,
+            "label": {
+                "code": "C",
+                "naam": "C"
+            },
+            "registratiedatum": "2020-01-15T08:58:42+01:00",
+            "soort": {
+                "code": "EI",
+                "naam": "Energie-index"
+            },
+            "status": {
+                "code": "DEF",
+                "naam": "Definitief"
+            },
+            "waarde": "1.62"
+        }
+    ],
+    "gebruiksoppervlakte": 66,
     "id": "41162000015",
     "klimaatbeheersingsoort": {
         "code": "IND",
         "naam": "Individueel"
     },
     "ruimten": [
         {
@@ -700,9 +736,13 @@
             "oppervlakte": 0.4125,
             "soort": {
                 "code": "OVR",
                 "naam": "Overige ruimtes"
             },
             "verwarmd": false
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "MGW",
+        "naam": "Meergezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/41164000002.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/41164000002.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4444444444444444%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Aegidiusstraat'), ('huisnummer', '122'), "*

 * *            "('huisnummer_toevoeging', ''), ('postcode', '3061XR'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000316161'), "*

 * *                                          "('bagIdentificatie', '0599010000316161')])",*

 * * "'energieprestaties'": "[OrderedDict([('soort', OrderedDict([('code', 'EI'), ('naam', "*

 * *                         […]*

```diff
@@ -1,9 +1,44 @@
 {
+    "adres": {
+        "huisnummer": "122",
+        "huisnummer_toevoeging": "",
+        "postcode": "3061XR",
+        "straatnaam": "Aegidiusstraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000316161",
+        "id": "0599010000316161"
+    },
     "bouwjaar": 1904,
+    "energieprestaties": [
+        {
+            "begindatum": "2018-01-18",
+            "einddatum": "2028-01-18",
+            "energieprestatievergoeding": false,
+            "label": {
+                "code": "B",
+                "naam": "B"
+            },
+            "registratiedatum": "2018-03-12T12:17:19+01:00",
+            "soort": {
+                "code": "EI",
+                "naam": "Energie-index"
+            },
+            "status": {
+                "code": "DEF",
+                "naam": "Definitief"
+            },
+            "waarde": "1.36"
+        }
+    ],
+    "gebruiksoppervlakte": 151,
     "id": "41164000002",
     "klimaatbeheersingsoort": {
         "code": "IND",
         "naam": "Individueel"
     },
     "ruimten": [
         {
@@ -527,9 +562,13 @@
             "oppervlakte": 1.87661,
             "soort": {
                 "code": "OVR",
                 "naam": "Overige ruimtes"
             },
             "verwarmd": false
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "EGW",
+        "naam": "Eengezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/51011000042.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/51011000042.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Eskampstraat'), ('huisnummer', '1'), "*

 * *            "('huisnummer_toevoeging', 'b'), ('postcode', '3042SJ'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000312130'), "*

 * *                                          "('bagIdentificatie', '0599010000312130')])",*

 * * "'bouwjaar'": '1952',*

 * * "'energieprestaties'": "[OrderedDict([('soort', OrderedDict([('code', 'EI'), ('naam', "*

 * *     […]*

```diff
@@ -1,8 +1,44 @@
 {
+    "adres": {
+        "huisnummer": "1",
+        "huisnummer_toevoeging": "b",
+        "postcode": "3042SJ",
+        "straatnaam": "Eskampstraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000312130",
+        "id": "0599010000312130"
+    },
+    "bouwjaar": 1952,
+    "energieprestaties": [
+        {
+            "begindatum": "2018-11-14",
+            "einddatum": "2028-11-14",
+            "energieprestatievergoeding": false,
+            "label": {
+                "code": "A",
+                "naam": "A"
+            },
+            "registratiedatum": "2019-03-28T13:39:08+01:00",
+            "soort": {
+                "code": "EI",
+                "naam": "Energie-index"
+            },
+            "status": {
+                "code": "DEF",
+                "naam": "Definitief"
+            },
+            "waarde": "1.09"
+        }
+    ],
+    "gebruiksoppervlakte": 74,
     "id": "51011000042",
     "klimaatbeheersingsoort": {
         "code": "IND",
         "naam": "Individueel"
     },
     "ruimten": [
         {
@@ -548,9 +584,13 @@
             "oppervlakte": 6.92162,
             "soort": {
                 "code": "VTK",
                 "naam": "Vertrek"
             },
             "verwarmd": true
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "MGW",
+        "naam": "Meergezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/71211000027.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/71211000027.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Polslandstraat'), ('huisnummer', '37'), "*

 * *            "('huisnummer_toevoeging', ''), ('postcode', '3081TK'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000307252'), "*

 * *                                          "('bagIdentificatie', '0599010000307252')])",*

 * * "'bouwjaar'": '1919',*

 * * "'energieprestaties'": "[OrderedDict([('soort', OrderedDict([('code', 'EI'), ('naam', "*

 * *   […]*

```diff
@@ -1,8 +1,44 @@
 {
+    "adres": {
+        "huisnummer": "37",
+        "huisnummer_toevoeging": "",
+        "postcode": "3081TK",
+        "straatnaam": "Polslandstraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000307252",
+        "id": "0599010000307252"
+    },
+    "bouwjaar": 1919,
+    "energieprestaties": [
+        {
+            "begindatum": "2018-10-29",
+            "einddatum": "2028-10-29",
+            "energieprestatievergoeding": false,
+            "label": {
+                "code": "D",
+                "naam": "D"
+            },
+            "registratiedatum": "2019-02-13T11:48:42+01:00",
+            "soort": {
+                "code": "EI",
+                "naam": "Energie-index"
+            },
+            "status": {
+                "code": "DEF",
+                "naam": "Definitief"
+            },
+            "waarde": "1.85"
+        }
+    ],
+    "gebruiksoppervlakte": 53,
     "id": "71211000027",
     "klimaatbeheersingsoort": {
         "code": "IND",
         "naam": "Individueel"
     },
     "ruimten": [
         {
@@ -521,9 +557,13 @@
             "oppervlakte": 0.07375,
             "soort": {
                 "code": "OVR",
                 "naam": "Overige ruimtes"
             },
             "verwarmd": false
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "EGW",
+        "naam": "Eengezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/77795000000.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/77795000000.json`

 * *Files 2% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4444444444444444%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Sliedrechtstraat'), ('huisnummer', '22'), "*

 * *            "('huisnummer_toevoeging', ''), ('postcode', '3086JM'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010400005761'), "*

 * *                                          "('bagIdentificatie', '0599010400005761')])",*

 * * "'energieprestaties'": "[OrderedDict([('soort', OrderedDict([('code', 'EI'), ('naam', "*

 * *                        […]*

```diff
@@ -1,9 +1,44 @@
 {
+    "adres": {
+        "huisnummer": "22",
+        "huisnummer_toevoeging": "",
+        "postcode": "3086JM",
+        "straatnaam": "Sliedrechtstraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010400005761",
+        "id": "0599010400005761"
+    },
     "bouwjaar": 2011,
+    "energieprestaties": [
+        {
+            "begindatum": "2017-12-29",
+            "einddatum": "2027-12-29",
+            "energieprestatievergoeding": false,
+            "label": {
+                "code": "A",
+                "naam": "A"
+            },
+            "registratiedatum": "2017-12-29T15:45:50+01:00",
+            "soort": {
+                "code": "EI",
+                "naam": "Energie-index"
+            },
+            "status": {
+                "code": "DEF",
+                "naam": "Definitief"
+            },
+            "waarde": "0.97"
+        }
+    ],
+    "gebruiksoppervlakte": 106,
     "id": "77795000000",
     "klimaatbeheersingsoort": {
         "code": "COL",
         "naam": "Collectief"
     },
     "ruimten": [
         {
@@ -424,9 +459,13 @@
             "oppervlakte": 3.02,
             "soort": {
                 "code": "OVR",
                 "naam": "Overige ruimtes"
             },
             "verwarmd": false
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "EGW",
+        "naam": "Eengezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/81020000003.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/81020000003.json`

 * *Files 5% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Putsebocht'), ('huisnummer', '18'), "*

 * *            "('huisnummer_toevoeging', 'b'), ('postcode', '3073HK'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010400029477'), "*

 * *                                          "('bagIdentificatie', '0599010400029477')])",*

 * * "'bouwjaar'": '1923',*

 * * "'energieprestaties'": "[OrderedDict([('soort', OrderedDict([('code', 'EI'), ('naam', "*

 * *      […]*

```diff
@@ -1,8 +1,44 @@
 {
+    "adres": {
+        "huisnummer": "18",
+        "huisnummer_toevoeging": "b",
+        "postcode": "3073HK",
+        "straatnaam": "Putsebocht",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010400029477",
+        "id": "0599010400029477"
+    },
+    "bouwjaar": 1923,
+    "energieprestaties": [
+        {
+            "begindatum": "2017-09-29",
+            "einddatum": "2027-09-29",
+            "energieprestatievergoeding": false,
+            "label": {
+                "code": "A",
+                "naam": "A"
+            },
+            "registratiedatum": "2017-10-01T10:55:54+02:00",
+            "soort": {
+                "code": "EI",
+                "naam": "Energie-index"
+            },
+            "status": {
+                "code": "DEF",
+                "naam": "Definitief"
+            },
+            "waarde": "0.14"
+        }
+    ],
+    "gebruiksoppervlakte": 100,
     "id": "81020000003",
     "klimaatbeheersingsoort": {
         "code": "COL",
         "naam": "Collectief"
     },
     "ruimten": [
         {
@@ -544,9 +580,13 @@
             "oppervlakte": 1.61275,
             "soort": {
                 "code": "OVR",
                 "naam": "Overige ruimtes"
             },
             "verwarmd": false
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "EGW",
+        "naam": "Eengezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/81065000089.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/81065000089.json`

 * *Files 9% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.25%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Oostendamstraat'), ('huisnummer', '145'), "*

 * *            "('huisnummer_toevoeging', ''), ('postcode', '3073NE'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000310211'), "*

 * *                                          "('bagIdentificatie', '0599010000310211')])",*

 * * "'bouwjaar'": '1921',*

 * * "'energieprestaties'": "[OrderedDict([('soort', OrderedDict([('code', 'EP2'), ('naam', ' […]*

```diff
@@ -1,8 +1,45 @@
 {
+    "adres": {
+        "huisnummer": "145",
+        "huisnummer_toevoeging": "",
+        "postcode": "3073NE",
+        "straatnaam": "Oostendamstraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000310211",
+        "id": "0599010000310211"
+    },
+    "bouwjaar": 1921,
+    "energieprestaties": [
+        {
+            "begindatum": "2024-02-13",
+            "einddatum": "2034-02-13",
+            "energieprestatievergoeding": false,
+            "gebruiksoppervlakteThermischeZone": 78.84,
+            "label": {
+                "code": "B",
+                "naam": "B"
+            },
+            "registratiedatum": "2024-02-21T11:09:37+01:00",
+            "soort": {
+                "code": "EP2",
+                "naam": "Primair energieverbruik - woningbouw"
+            },
+            "status": {
+                "code": "DEF",
+                "naam": "Definitief"
+            },
+            "waarde": "173.08"
+        }
+    ],
+    "gebruiksoppervlakte": 82,
     "id": "81065000089",
     "ruimten": [
         {
             "bouwlaag": {
                 "nummer": "00",
                 "omschrijving": "begane grond"
             },
@@ -330,9 +367,13 @@
             "oppervlakte": 0.173034,
             "soort": {
                 "code": "OVR",
                 "naam": "Overige ruimtes"
             },
             "verwarmd": false
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "EGW",
+        "naam": "Eengezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/85651000021.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/85651000021.json`

 * *Files 3% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Atjehstraat'), ('huisnummer', '47'), "*

 * *            "('huisnummer_toevoeging', 'd'), ('postcode', '3072ZB'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000078889'), "*

 * *                                          "('bagIdentificatie', '0599010000078889')])",*

 * * "'bouwjaar'": '1897',*

 * * "'energieprestaties'": '[]',*

 * * "'gebruiksoppervlakte'": '72',*

 * * "'woningtype'": "OrderedDict([ […]*

```diff
@@ -1,8 +1,24 @@
 {
+    "adres": {
+        "huisnummer": "47",
+        "huisnummer_toevoeging": "d",
+        "postcode": "3072ZB",
+        "straatnaam": "Atjehstraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000078889",
+        "id": "0599010000078889"
+    },
+    "bouwjaar": 1897,
+    "energieprestaties": [],
+    "gebruiksoppervlakte": 72,
     "id": "85651000021",
     "klimaatbeheersingsoort": {
         "code": "IND",
         "naam": "Individueel"
     },
     "ruimten": [
         {
@@ -322,9 +338,13 @@
             "oppervlakte": 0.438,
             "soort": {
                 "code": "OVR",
                 "naam": "Overige ruimtes"
             },
             "verwarmd": false
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "MGW",
+        "naam": "Meergezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/input/zelfstandige_woonruimten/87402000003.json` & `woningwaardering-0.2.0a1/tests/data/input/zelfstandige_woonruimten/87402000003.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3333333333333333%*

 * *Differences: {"'adres'": "OrderedDict([('straatnaam', 'Oranjeboomstraat'), ('huisnummer', '355'), "*

 * *            "('huisnummer_toevoeging', 'c'), ('postcode', '3071SV'), ('woonplaats', "*

 * *            "OrderedDict([('naam', 'ROTTERDAM')]))])",*

 * * "'adresseerbaarObjectBasisregistratie'": "OrderedDict([('id', '0599010000040514'), "*

 * *                                          "('bagIdentificatie', '0599010000040514')])",*

 * * "'bouwjaar'": '1898',*

 * * "'energieprestaties'": '[]',*

 * * "'gebruiksoppervlakte'": '50',*

 * * "'woningtype'": "Ordered […]*

```diff
@@ -1,8 +1,24 @@
 {
+    "adres": {
+        "huisnummer": "355",
+        "huisnummer_toevoeging": "c",
+        "postcode": "3071SV",
+        "straatnaam": "Oranjeboomstraat",
+        "woonplaats": {
+            "naam": "ROTTERDAM"
+        }
+    },
+    "adresseerbaarObjectBasisregistratie": {
+        "bagIdentificatie": "0599010000040514",
+        "id": "0599010000040514"
+    },
+    "bouwjaar": 1898,
+    "energieprestaties": [],
+    "gebruiksoppervlakte": 50,
     "id": "87402000003",
     "klimaatbeheersingsoort": {
         "code": "IND",
         "naam": "Individueel"
     },
     "ruimten": [
         {
@@ -240,9 +256,13 @@
             "oppervlakte": 8.352,
             "soort": {
                 "code": "VTK",
                 "naam": "Vertrek"
             },
             "verwarmd": true
         }
-    ]
+    ],
+    "woningtype": {
+        "code": "MGW",
+        "naam": "Meergezinswoning"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json` & `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7680555555555556%*

 * *Differences: {"'groepen'": "{0: {'punten': 61.0, 'woningwaarderingen': {0: {'aantal': 30.12, 'criterium': "*

 * *              "{'naam': 'Woonkamer'}}, 1: {'aantal': 11.72, 'criterium': {'naam': 'Slaapkamer'}}, "*

 * *              "2: {'aantal': 4.64, 'criterium': {'naam': 'Badruimte'}}, 3: {'aantal': 9.21}, 4: "*

 * *              "{'aantal': 5.76, 'criterium': {'naam': 'Keuken'}}}}, 1: {'punten': 3.75, "*

 * *              "'woningwaarderingen': [OrderedDict([('aantal', 5.1), ('criterium', "*

 * *              "OrderedDict([('naam', 'Berging […]*

```diff
@@ -7,64 +7,64 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 60.0,
+            "punten": 61.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 3.58,
+                    "aantal": 30.12,
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
-                    "aantal": 10.18,
+                    "aantal": 11.72,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken + 2 kasten"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 26.82,
+                    "aantal": 4.64,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer + 1 kast"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 6.49,
+                    "aantal": 9.21,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 12.98,
+                    "aantal": 5.76,
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
@@ -72,16 +72,27 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 0.0,
-            "woningwaarderingen": []
+            "punten": 3.75,
+            "woningwaarderingen": [
+                {
+                    "aantal": 5.1,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Berging"
+                    }
+                }
+            ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
@@ -90,44 +101,65 @@
                     "naam": "Verwarming"
                 }
             },
             "punten": 10.0,
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
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
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
                         "naam": "Slaapkamer"
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
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 28.0,
+            "woningwaarderingen": [
+                {
+                    "criterium": {
+                        "naam": "B (oud)"
+                    },
+                    "punten": 28.0
+                }
+            ]
         }
     ],
-    "punten": 70.0,
+    "punten": 103.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json` & `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/87402000003.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7732638888888889%*

 * *Differences: {"'groepen'": "{0: {'punten': 53.0, 'woningwaarderingen': {0: {'aantal': 11.65}, 1: {'aantal': "*

 * *              "3.12, 'criterium': {'naam': 'Badruimte'}}, 2: {'aantal': 6.37, 'criterium': "*

 * *              "{'naam': 'Keuken'}}, 3: {'aantal': 23.1, 'criterium': {'naam': 'Woonkamer'}}, 4: "*

 * *              "{'aantal': 8.35, 'criterium': {'naam': 'Slaapkamer'}}}}, 1: {'punten': 3.75, "*

 * *              "'woningwaarderingen': {0: {'aantal': 5.25}}}, 2: {'woningwaarderingen': {1: "*

 * *              "{'criterium': {'naam': […]*

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
-                    "aantal": 11.88,
+                    "aantal": 11.65,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 9.73,
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
-                    "aantal": 22.85,
+                    "aantal": 6.37,
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
-                    "aantal": 3.94,
+                    "aantal": 23.1,
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
-                    "aantal": 12.22,
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
+                    "aantal": 5.25,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Berging"
                     }
@@ -107,38 +107,59 @@
                     "criterium": {
                         "naam": "Slaapkamer"
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
-                        "naam": "Badruimte"
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
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 0.0,
+            "woningwaarderingen": [
+                {
+                    "criterium": {
+                        "naam": "Bouwjaar 1898"
+                    },
+                    "punten": 0.0
+                }
+            ]
         }
     ],
-    "punten": 74.0,
+    "punten": 67.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/25048000007.json` & `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7628968253968255%*

 * *Differences: {"'groepen'": "{0: {'punten': 138.0, 'woningwaarderingen': {1: {'aantal': 23.42, 'criterium': "*

 * *              "{'naam': 'Slaapkamer + 1 kast'}}, 2: {'aantal': 22.66}, 3: {'aantal': 14.71, "*

 * *              "'criterium': {'naam': 'Keuken'}}, 4: {'aantal': 17.63}, 6: {'aantal': 20.45, "*

 * *              "'criterium': {'naam': 'Slaapkamer + 1 kast'}}, insert: [(0, OrderedDict([('aantal', "*

 * *              "6.33), ('criterium', OrderedDict([('naam', 'Badruimte'), ('meeteenheid', "*

 * *              "OrderedDict([('code',  […]*

```diff
@@ -7,64 +7,84 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 61.0,
+            "punten": 138.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 30.12,
+                    "aantal": 6.33,
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
+                    "aantal": 23.42,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Slaapkamer + 1 kast"
                     }
                 },
                 {
-                    "aantal": 11.72,
+                    "aantal": 22.66,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 4.64,
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
-                    "aantal": 9.21,
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
-                    "aantal": 5.76,
+                    "aantal": 32.95,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken"
+                        "naam": "Woonkamer"
+                    }
+                },
+                {
+                    "aantal": 20.45,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Slaapkamer + 1 kast"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -72,24 +92,24 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 3.75,
+            "punten": 3.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 5.1,
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
@@ -97,48 +117,81 @@
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
-                        "naam": "Woonkamer"
+                        "naam": "Badruimte"
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
-                        "naam": "Badruimte"
+                        "naam": "Slaapkamer"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "criterium": {
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
-                        "naam": "Keuken"
+                        "naam": "Woonkamer"
+                    },
+                    "punten": 2.0
+                },
+                {
+                    "criterium": {
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
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
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 32.0,
+            "woningwaarderingen": [
+                {
+                    "criterium": {
+                        "naam": "B (oud)"
+                    },
+                    "punten": 32.0
+                }
+            ]
         }
     ],
-    "punten": 75.0,
+    "punten": 187.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json` & `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7628761574074074%*

 * *Differences: {"'groepen'": "{0: {'punten': 58.0, 'woningwaarderingen': {0: {'aantal': 11.63}, 1: {'aantal': "*

 * *              "7.62}, 2: {'aantal': 17.77}, 3: {'aantal': 12.72, 'criterium': {'naam': 'Keuken'}}, "*

 * *              "4: {'aantal': 8.34}, delete: [2]}}, 1: {'punten': 4.5, 'woningwaarderingen': {1: "*

 * *              "{'aantal': 2.86, 'criterium': {'naam': 'Wasruimte'}}, insert: [(0, "*

 * *              "OrderedDict([('aantal', 3.56), ('criterium', OrderedDict([('naam', 'Zolder'), "*

 * *              "('meeteenheid', Ordere […]*

```diff
@@ -7,68 +7,58 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 67.0,
+            "punten": 58.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 10.0,
+                    "aantal": 11.63,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 7.02,
+                    "aantal": 7.62,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 7.64,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Keuken"
-                    }
-                },
-                {
-                    "aantal": 23.62,
+                    "aantal": 17.77,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 5.18,
+                    "aantal": 12.72,
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
-                    "aantal": 13.35,
+                    "aantal": 8.34,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
@@ -82,24 +72,34 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 3.0,
+            "punten": 4.5,
             "woningwaarderingen": [
                 {
-                    "aantal": 4.1,
+                    "aantal": 3.56,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Berging"
+                        "naam": "Zolder"
+                    }
+                },
+                {
+                    "aantal": 2.86,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Wasruimte"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -107,15 +107,15 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 12.0,
+            "punten": 11.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
@@ -123,38 +123,59 @@
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Keuken"
+                        "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Wasruimte"
                     },
-                    "punten": 2.0
+                    "punten": 1.0
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
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 32.0,
+            "woningwaarderingen": [
+                {
+                    "criterium": {
+                        "naam": "B + 78.84m2"
+                    },
+                    "punten": 32.0
+                }
+            ]
         }
     ],
-    "punten": 82.0,
+    "punten": 106.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json` & `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/37101000032.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7916666666666666%*

 * *Differences: {"'groepen'": "{insert: [(3, OrderedDict([('criteriumGroep', OrderedDict([('stelsel', "*

 * *              "OrderedDict([('code', 'ZEL'), ('naam', 'Zelfstandige woonruimten')])), "*

 * *              "('stelselgroep', OrderedDict([('code', 'ENE'), ('naam', 'Energieprestatie')]))])), "*

 * *              "('punten', 22.0), ('woningwaarderingen', [OrderedDict([('criterium', "*

 * *              "OrderedDict([('naam', 'C (oud)')])), ('punten', 22.0)])])]))]}",*

 * * "'punten'": '181.0'}*

```diff
@@ -162,15 +162,36 @@
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
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
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 22.0,
+            "woningwaarderingen": [
+                {
+                    "criterium": {
+                        "naam": "C (oud)"
+                    },
+                    "punten": 22.0
+                }
+            ]
         }
     ],
-    "punten": 159.0,
+    "punten": 181.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41027000003.json` & `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/23003000050.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7681423611111112%*

 * *Differences: {"'groepen'": "{0: {'punten': 61.0, 'woningwaarderingen': {0: {'aantal': 11.88, 'criterium': "*

 * *              "{'naam': 'Slaapkamer'}}, 1: {'aantal': 9.73, 'criterium': {'naam': 'Slaapkamer'}}, "*

 * *              "2: {'aantal': 22.85, 'criterium': {'naam': 'Woonkamer'}}, 3: {'aantal': 3.94, "*

 * *              "'criterium': {'naam': 'Badruimte'}}, 4: {'aantal': 12.22, 'criterium': {'naam': "*

 * *              "'Keuken'}}}}, 1: {'punten': 3.0, 'woningwaarderingen': [OrderedDict([('aantal', "*

 * *              "4.41), ('crit […]*

```diff
@@ -7,64 +7,64 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 43.0,
+            "punten": 61.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 2.18,
+                    "aantal": 11.88,
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
-                    "aantal": 12.1,
+                    "aantal": 9.73,
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
-                    "aantal": 16.65,
+                    "aantal": 22.85,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer + 1 kast"
+                        "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 4.84,
+                    "aantal": 3.94,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken + 1 kast"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 6.84,
+                    "aantal": 12.22,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer + 2 kasten"
+                        "naam": "Keuken"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -72,16 +72,27 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 0.0,
-            "woningwaarderingen": []
+            "punten": 3.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 4.41,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Berging"
+                    }
+                }
+            ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
@@ -90,15 +101,15 @@
                     "naam": "Verwarming"
                 }
             },
             "punten": 10.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
@@ -108,26 +119,47 @@
                     "criterium": {
                         "naam": "Woonkamer"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
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
+        },
+        {
+            "criteriumGroep": {
+                "stelsel": {
+                    "code": "ZEL",
+                    "naam": "Zelfstandige woonruimten"
+                },
+                "stelselgroep": {
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 15.0,
+            "woningwaarderingen": [
+                {
+                    "criterium": {
+                        "naam": "C (oud)"
+                    },
+                    "punten": 15.0
+                }
+            ]
         }
     ],
-    "punten": 53.0,
+    "punten": 89.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json` & `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41123000005.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7916666666666666%*

 * *Differences: {"'groepen'": "{insert: [(3, OrderedDict([('criteriumGroep', OrderedDict([('stelsel', "*

 * *              "OrderedDict([('code', 'ZEL'), ('naam', 'Zelfstandige woonruimten')])), "*

 * *              "('stelselgroep', OrderedDict([('code', 'ENE'), ('naam', 'Energieprestatie')]))])), "*

 * *              "('punten', 32.0), ('woningwaarderingen', [OrderedDict([('criterium', "*

 * *              "OrderedDict([('naam', 'B (oud)')])), ('punten', 32.0)])])]))]}",*

 * * "'punten'": '173.0'}*

```diff
@@ -236,15 +236,36 @@
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
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
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 32.0,
+            "woningwaarderingen": [
+                {
+                    "criterium": {
+                        "naam": "B (oud)"
+                    },
+                    "punten": 32.0
+                }
+            ]
         }
     ],
-    "punten": 141.0,
+    "punten": 173.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json` & `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7730758101851851%*

 * *Differences: {"'groepen'": "{0: {'punten': 54.0, 'woningwaarderingen': {0: {'aantal': 15.89, 'criterium': "*

 * *              "{'naam': 'Woonkamer + 1 kast'}}, 1: {'aantal': 10.63, 'criterium': {'naam': "*

 * *              "'Keuken'}}, 2: {'aantal': 9.08, 'criterium': {'naam': 'Slaapkamer'}}, 3: {'aantal': "*

 * *              "4.73, 'criterium': {'naam': 'Slaapkamer'}}, 4: {'aantal': 8.72, 'criterium': "*

 * *              "{'naam': 'Slaapkamer'}}, 5: {'aantal': 4.94, 'criterium': {'naam': 'Badruimte'}}}}, "*

 * *              "1: {'punten': […]*

```diff
@@ -7,74 +7,74 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 53.0,
+            "punten": 54.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 1.89,
+                    "aantal": 15.89,
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
-                    "aantal": 18.79,
+                    "aantal": 10.63,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer + 1 kast"
+                        "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 5.94,
+                    "aantal": 9.08,
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
-                    "aantal": 12.74,
+                    "aantal": 4.73,
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
-                    "aantal": 5.39,
+                    "aantal": 8.72,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken + 2 kasten"
+                        "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 8.56,
+                    "aantal": 4.94,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer + 2 kasten"
+                        "naam": "Badruimte"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -82,28 +82,28 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 9.0,
+            "punten": 6.75,
             "woningwaarderingen": [
                 {
-                    "aantal": 7.78,
+                    "aantal": 4.4,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Berging"
+                        "naam": "Zolder"
                     }
                 },
                 {
-                    "aantal": 4.03,
+                    "aantal": 5.05,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Berging"
                     }
@@ -121,21 +121,21 @@
                     "naam": "Verwarming"
                 }
             },
             "punten": 12.0,
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
-                        "naam": "Woonkamer"
+                        "naam": "Keuken"
                     },
                     "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
@@ -145,26 +145,47 @@
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
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 14.0,
+            "woningwaarderingen": [
+                {
+                    "criterium": {
+                        "naam": "D (oud)"
+                    },
+                    "punten": 14.0
+                }
+            ]
         }
     ],
-    "punten": 74.0,
+    "punten": 87.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41164000002.json` & `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json`

 * *Files 8% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7635788690476191%*

 * *Differences: {"'groepen'": "{0: {'punten': 79.0, 'woningwaarderingen': {0: {'aantal': 3.8}, 1: {'aantal': "*

 * *              "15.74}, 2: {'aantal': 5.92}, 3: {'aantal': 15.15}, 4: {'aantal': 26.54, "*

 * *              "'criterium': {'naam': 'Woonkamer + 1 kast'}}, 5: {'aantal': 12.23, 'criterium': "*

 * *              "{'naam': 'Slaapkamer'}}, delete: [1]}}, 1: {'punten': 3.75, 'woningwaarderingen': "*

 * *              "{0: {'aantal': 5.19, 'criterium': {'naam': 'Berging'}}}}, 2: {'punten': 9.0, "*

 * *              "'woningwaarderingen': { […]*

```diff
@@ -7,84 +7,74 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 138.0,
+            "punten": 79.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 6.33,
+                    "aantal": 3.8,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 23.42,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Slaapkamer + 1 kast"
-                    }
-                },
-                {
-                    "aantal": 22.66,
+                    "aantal": 15.74,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 14.71,
+                    "aantal": 5.92,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 17.63,
+                    "aantal": 15.15,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 32.95,
+                    "aantal": 26.54,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer"
+                        "naam": "Woonkamer + 1 kast"
                     }
                 },
                 {
-                    "aantal": 20.45,
+                    "aantal": 12.23,
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
@@ -92,24 +82,24 @@
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
-                    "aantal": 4.31,
+                    "aantal": 5.19,
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
@@ -117,60 +107,75 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 14.0,
+            "punten": 9.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
                         "naam": "Badruimte"
                     },
-                    "punten": 2.0
-                },
-                {
-                    "criterium": {
-                        "naam": "Slaapkamer"
-                    },
-                    "punten": 2.0
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
                         "naam": "Keuken"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
                         "naam": "Woonkamer"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
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
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 36.0,
+            "woningwaarderingen": [
+                {
+                    "criterium": {
+                        "naam": "A (oud)"
+                    },
+                    "punten": 36.0
                 }
             ]
         }
     ],
-    "punten": 155.0,
+    "punten": 128.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/51011000042.json` & `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/41162000015.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.759796626984127%*

 * *Differences: {"'groepen'": "{0: {'punten': 53.0, 'woningwaarderingen': {0: {'aantal': 1.89, 'criterium': "*

 * *              "{'naam': 'Badruimte'}}, 1: {'aantal': 18.79, 'criterium': {'naam': 'Woonkamer + 1 "*

 * *              "kast'}}, 2: {'aantal': 5.94, 'criterium': {'naam': 'Slaapkamer + 1 kast'}}, 3: "*

 * *              "{'aantal': 12.74, 'criterium': {'naam': 'Slaapkamer + 1 kast'}}, 4: {'aantal': "*

 * *              "5.39, 'criterium': {'naam': 'Keuken + 2 kasten'}}, 5: {'aantal': 8.56, 'criterium': "*

 * *              "{'naam': 'S […]*

```diff
@@ -7,84 +7,74 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 60.0,
+            "punten": 53.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 17.56,
+                    "aantal": 1.89,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer + 1 kast"
-                    }
-                },
-                {
-                    "aantal": 11.8,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Slaapkamer + 1 kast"
+                        "naam": "Badruimte"
                     }
                 },
                 {
-                    "aantal": 6.99,
+                    "aantal": 18.79,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer + 2 kasten"
+                        "naam": "Woonkamer + 1 kast"
                     }
                 },
                 {
-                    "aantal": 8.15,
+                    "aantal": 5.94,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Slaapkamer + 1 kast"
                     }
                 },
                 {
-                    "aantal": 1.92,
+                    "aantal": 12.74,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Slaapkamer + 1 kast"
                     }
                 },
                 {
-                    "aantal": 7.06,
+                    "aantal": 5.39,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken"
+                        "naam": "Keuken + 2 kasten"
                     }
                 },
                 {
-                    "aantal": 6.92,
+                    "aantal": 8.56,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Slaapkamer + 2 kasten"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -92,39 +82,60 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 0.0,
-            "woningwaarderingen": []
+            "punten": 9.0,
+            "woningwaarderingen": [
+                {
+                    "aantal": 7.78,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Berging"
+                    }
+                },
+                {
+                    "aantal": 4.03,
+                    "criterium": {
+                        "meeteenheid": {
+                            "code": "M2",
+                            "naam": "Vierkante meter, m2"
+                        },
+                        "naam": "Berging"
+                    }
+                }
+            ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 14.0,
+            "punten": 12.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Badruimte"
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
@@ -134,32 +145,47 @@
                     "criterium": {
                         "naam": "Slaapkamer"
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
-                        "naam": "Keuken"
+                        "naam": "Slaapkamer"
                     },
                     "punten": 2.0
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
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 15.0,
+            "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "C (oud)"
                     },
-                    "punten": 2.0
+                    "punten": 15.0
                 }
             ]
         }
     ],
-    "punten": 74.0,
+    "punten": 89.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/71211000027.json` & `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json`

 * *Files 11% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7612950562169312%*

 * *Differences: {"'groepen'": "{0: {'punten': 65.0, 'woningwaarderingen': {0: {'aantal': 9.6, 'criterium': "*

 * *              "{'naam': 'Slaapkamer'}}, 1: {'aantal': 4.71, 'criterium': {'naam': 'Badruimte'}}, "*

 * *              "2: {'aantal': 9.37, 'criterium': {'naam': 'Keuken'}}, 3: {'aantal': 13.41}, 4: "*

 * *              "{'aantal': 21.84, 'criterium': {'naam': 'Woonkamer'}}, 5: {'aantal': 6.06, "*

 * *              "'criterium': {'naam': 'Slaapkamer'}}}}, 1: {'punten': 20.25, 'woningwaarderingen': "*

 * *              "{0: {'aantal': 26 […]*

```diff
@@ -7,74 +7,74 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 54.0,
+            "punten": 65.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 15.89,
+                    "aantal": 9.6,
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
-                    "aantal": 10.63,
+                    "aantal": 4.71,
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
-                    "aantal": 9.08,
+                    "aantal": 9.37,
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
-                    "aantal": 4.73,
+                    "aantal": 13.41,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 8.72,
+                    "aantal": 21.84,
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
-                    "aantal": 4.94,
+                    "aantal": 6.06,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Slaapkamer"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -82,89 +82,106 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 6.75,
+            "punten": 20.25,
             "woningwaarderingen": [
                 {
-                    "aantal": 4.4,
+                    "aantal": 26.96,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Zolder"
                     }
-                },
-                {
-                    "aantal": 5.05,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Berging"
-                    }
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
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 12.0,
+            "punten": 9.75,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Slaapkamer"
+                    },
+                    "punten": 1.5
+                },
+                {
+                    "criterium": {
+                        "naam": "Badruimte"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
+                },
+                {
+                    "criterium": {
+                        "naam": "Zolder"
+                    },
+                    "punten": 0.75
                 },
                 {
                     "criterium": {
                         "naam": "Keuken"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Woonkamer"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
-                    "punten": 2.0
+                    "punten": 1.5
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
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 36.0,
+            "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "A (oud)"
                     },
-                    "punten": 2.0
+                    "punten": 36.0
                 }
             ]
         }
     ],
-    "punten": 73.0,
+    "punten": 131.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/77795000000.json` & `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/28018000044.json`

 * *Files 10% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7638578869047619%*

 * *Differences: {"'groepen'": "{0: {'punten': 67.0, 'woningwaarderingen': {0: {'aantal': 10.0}, 1: {'aantal': "*

 * *              "7.02, 'criterium': {'naam': 'Slaapkamer'}}, 2: {'aantal': 7.64}, 3: {'aantal': "*

 * *              "23.62, 'criterium': {'naam': 'Woonkamer'}}, 4: {'aantal': 5.18, 'criterium': "*

 * *              "{'naam': 'Badruimte'}}, 5: {'aantal': 13.35}}}, 1: {'punten': 3.0, "*

 * *              "'woningwaarderingen': {0: {'aantal': 4.1, 'criterium': {'naam': 'Berging'}}}}, 2: "*

 * *              "{'punten': 12.0, 'woningwaar […]*

```diff
@@ -7,68 +7,68 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 65.0,
+            "punten": 67.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 9.6,
+                    "aantal": 10.0,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 4.71,
+                    "aantal": 7.02,
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
-                    "aantal": 9.37,
+                    "aantal": 7.64,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Keuken"
                     }
                 },
                 {
-                    "aantal": 13.41,
+                    "aantal": 23.62,
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
-                    "aantal": 21.84,
+                    "aantal": 5.18,
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
-                    "aantal": 6.06,
+                    "aantal": 13.35,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
@@ -82,24 +82,24 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 20.25,
+            "punten": 3.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 26.96,
+                    "aantal": 4.1,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Zolder"
+                        "naam": "Berging"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -107,60 +107,75 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 9.75,
+            "punten": 12.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Slaapkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Zolder"
+                        "naam": "Keuken"
                     },
-                    "punten": 0.75
+                    "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Keuken"
+                        "naam": "Woonkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Slaapkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
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
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 22.0,
+            "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Bouwjaar 1992"
                     },
-                    "punten": 1.5
+                    "punten": 22.0
                 }
             ]
         }
     ],
-    "punten": 95.0,
+    "punten": 104.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81020000003.json` & `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7580295138888888%*

 * *Differences: {"'groepen'": "{0: {'punten': 60.0, 'woningwaarderingen': {0: {'aantal': 8.05, 'criterium': "*

 * *              "{'naam': 'Keuken'}}, 1: {'aantal': 5.78, 'criterium': {'naam': 'Badruimte'}}, 2: "*

 * *              "{'aantal': 25.54, 'criterium': {'naam': 'Woonkamer'}}, 3: {'aantal': 12.06}, 4: "*

 * *              "{'aantal': 8.11}, delete: [4]}}, 1: {'punten': 0.0, 'woningwaarderingen': []}, 2: "*

 * *              "{'punten': 10.0, 'woningwaarderingen': {0: {'punten': 2.0, 'criterium': {'naam': "*

 * *              "'Keuken'}}, […]*

```diff
@@ -7,68 +7,58 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 79.0,
+            "punten": 60.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 3.8,
+                    "aantal": 8.05,
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
-                    "aantal": 15.74,
+                    "aantal": 5.78,
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
-                    "aantal": 5.92,
+                    "aantal": 25.54,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Keuken"
+                        "naam": "Woonkamer"
                     }
                 },
                 {
-                    "aantal": 15.15,
+                    "aantal": 12.06,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 26.54,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Woonkamer + 1 kast"
-                    }
-                },
-                {
-                    "aantal": 12.23,
+                    "aantal": 8.11,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
@@ -82,79 +72,83 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 3.75,
-            "woningwaarderingen": [
-                {
-                    "aantal": 5.19,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Berging"
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
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 9.0,
+            "punten": 10.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Badruimte"
+                        "naam": "Keuken"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Badruimte"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Keuken"
+                        "naam": "Woonkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
                 },
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer"
+                        "naam": "Slaapkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2.0
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
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 0.0,
+            "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Slaapkamer"
+                        "naam": "Bouwjaar 1897"
                     },
-                    "punten": 1.5
+                    "punten": 0.0
                 }
             ]
         }
     ],
-    "punten": 92.0,
+    "punten": 70.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/81065000089.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json`

 * *Files 27% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.4113425925925926%*

 * *Differences: {"'groepen'": "{0: {'punten': 7.0, 'woningwaarderingen': {0: {'aantal': 2.0, 'criterium': {'naam': "*

 * *              "'Keuken'}}, 1: {'aantal': 4.0}, 2: {'aantal': 1.0, 'criterium': {'naam': "*

 * *              "'Badkamer/toilet'}}, delete: [3, 2]}}, 1: {'punten': 0.0, 'woningwaarderingen': "*

 * *              '[]}, delete: [2]}',*

 * * "'punten'": '7.0',*

 * * 'delete': "['stelsel']"}*

```diff
@@ -7,64 +7,44 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
-            "punten": 58.0,
+            "punten": 7.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 11.63,
+                    "aantal": 2.0,
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
-                    "aantal": 7.62,
+                    "aantal": 4.0,
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
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Woonkamer"
-                    }
-                },
-                {
-                    "aantal": 12.72,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Keuken"
-                    }
-                },
-                {
-                    "aantal": 8.34,
+                    "aantal": 1.0,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Slaapkamer"
+                        "naam": "Badkamer/toilet"
                     }
                 }
             ]
         },
         {
             "criteriumGroep": {
                 "stelsel": {
@@ -72,89 +52,13 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "OOZ",
                     "naam": "Oppervlakte van overige ruimten"
                 }
             },
-            "punten": 4.5,
-            "woningwaarderingen": [
-                {
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
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Wasruimte"
-                    }
-                }
-            ]
-        },
-        {
-            "criteriumGroep": {
-                "stelsel": {
-                    "code": "ZEL",
-                    "naam": "Zelfstandige woonruimten"
-                },
-                "stelselgroep": {
-                    "code": "VZE",
-                    "naam": "Verwarming"
-                }
-            },
-            "punten": 11.0,
-            "woningwaarderingen": [
-                {
-                    "criterium": {
-                        "naam": "Slaapkamer"
-                    },
-                    "punten": 2.0
-                },
-                {
-                    "criterium": {
-                        "naam": "Slaapkamer"
-                    },
-                    "punten": 2.0
-                },
-                {
-                    "criterium": {
-                        "naam": "Woonkamer"
-                    },
-                    "punten": 2.0
-                },
-                {
-                    "criterium": {
-                        "naam": "Wasruimte"
-                    },
-                    "punten": 1.0
-                },
-                {
-                    "criterium": {
-                        "naam": "Keuken"
-                    },
-                    "punten": 2.0
-                },
-                {
-                    "criterium": {
-                        "naam": "Slaapkamer"
-                    },
-                    "punten": 2.0
-                }
-            ]
+            "punten": 0.0,
+            "woningwaarderingen": []
         }
     ],
-    "punten": 74.0,
-    "stelsel": {
-        "code": "ZEL",
-        "naam": "Zelfstandige woonruimten"
-    }
+    "punten": 7.0
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/85651000021.json` & `woningwaardering-0.2.0a1/tests/data/output/zelfstandige_woonruimten/peildatum/2024-01-01/12006000004.json`

 * *Files 23% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7893229166666668%*

 * *Differences: {"'groepen'": "{0: {'woningwaarderingen': {0: {'aantal': 3.58, 'criterium': {'naam': "*

 * *              "'Badruimte'}}, 1: {'aantal': 10.18, 'criterium': {'naam': 'Keuken + 2 kasten'}}, 2: "*

 * *              "{'aantal': 26.82, 'criterium': {'naam': 'Woonkamer + 1 kast'}}, 3: {'aantal': "*

 * *              "6.49}, 4: {'aantal': 12.98}}}, 2: {'woningwaarderingen': {0: {'criterium': {'naam': "*

 * *              "'Badruimte'}}, 1: {'criterium': {'naam': 'Keuken'}}}}, insert: [(3, "*

 * *              "OrderedDict([('criteriumGroe […]*

```diff
@@ -10,55 +10,55 @@
                     "code": "OVZ",
                     "naam": "Oppervlakte van vertrekken"
                 }
             },
             "punten": 60.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 8.05,
+                    "aantal": 3.58,
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
-                    "aantal": 5.78,
+                    "aantal": 10.18,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Badruimte"
+                        "naam": "Keuken + 2 kasten"
                     }
                 },
                 {
-                    "aantal": 25.54,
+                    "aantal": 26.82,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
-                        "naam": "Woonkamer"
+                        "naam": "Woonkamer + 1 kast"
                     }
                 },
                 {
-                    "aantal": 12.06,
+                    "aantal": 6.49,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
                 },
                 {
-                    "aantal": 8.11,
+                    "aantal": 12.98,
                     "criterium": {
                         "meeteenheid": {
                             "code": "M2",
                             "naam": "Vierkante meter, m2"
                         },
                         "naam": "Slaapkamer"
                     }
@@ -90,21 +90,21 @@
                     "naam": "Verwarming"
                 }
             },
             "punten": 10.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Keuken"
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
                         "naam": "Woonkamer"
                     },
@@ -119,15 +119,36 @@
                 {
                     "criterium": {
                         "naam": "Slaapkamer"
                     },
                     "punten": 2.0
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
+                    "code": "ENE",
+                    "naam": "Energieprestatie"
+                }
+            },
+            "punten": 5.0,
+            "woningwaarderingen": [
+                {
+                    "criterium": {
+                        "naam": "Bouwjaar 1981"
+                    },
+                    "punten": 5.0
+                }
+            ]
         }
     ],
-    "punten": 70.0,
+    "punten": 75.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/config/test_config.py` & `woningwaardering-0.2.0a1/tests/stelsels/config/test_config.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py` & `woningwaardering-0.2.0a1/tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 @pytest.mark.parametrize(
     "peildatum, stelsel, aantal_geldige_stelselgroepen",
     [
         (
             date(2025, 1, 1),
             Woningwaarderingstelsel.zelfstandige_woonruimten,
-            3,
+            4,
         )
     ],
 )
 def test_select_geldige_stelselgroepen(
     peildatum, stelsel, aantal_geldige_stelselgroepen
 ):
     geldigige_stelselgroepen = Stelsel.select_geldige_stelselgroepen(
```

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py` & `woningwaardering-0.2.0a1/tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/test_ZelfstandigeWoonruimten.py` & `woningwaardering-0.2.0a1/tests/stelsels/test_ZelfstandigeWoonruimten.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/utils/test_import_class.py` & `woningwaardering-0.2.0a1/tests/stelsels/utils/test_import_class.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/utils/test_is_geldig.py` & `woningwaardering-0.2.0a1/tests/stelsels/utils/test_is_geldig.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/ruimte_meer_of_minder_dan_4m2.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/zolder_vertrek.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/badkamer_en_of_toilet_boven_en_onder_0.64.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/ruimte_meer_of_minder_dan_4m2.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json`

 * *Files 14% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.3328993055555556%*

 * *Differences: {"'groepen'": "{0: {'criteriumGroep': {'stelselgroep': {'code': 'VZE', 'naam': 'Verwarming'}}, "*

 * *              "'punten': 4.0, 'woningwaarderingen': {3: {'criterium': {'naam': 'Woonkamer4', "*

 * *              "delete: ['meeteenheid']}, 'punten': 0.75, delete: ['aantal']}, 4: {'criterium': "*

 * *              "{'naam': 'Woonkamer5', delete: ['meeteenheid']}, 'punten': 0.75, delete: "*

 * *              "['aantal']}, 5: {'criterium': {'naam': 'Woonkamer6', delete: ['meeteenheid']}, "*

 * *              "'punten': 0.25, delete […]*

```diff
@@ -3,62 +3,53 @@
         {
             "criteriumGroep": {
                 "stelsel": {
                     "code": "ZEL",
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
-                    "code": "OVZ",
-                    "naam": "Oppervlakte van vertrekken"
+                    "code": "VZE",
+                    "naam": "Verwarming"
                 }
             },
-            "punten": 7.0,
+            "punten": 4.0,
             "woningwaarderingen": [
                 {
-                    "aantal": 2.0,
                     "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Keuken"
-                    }
-                },
-                {
-                    "aantal": 4.0,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Slaapkamer"
-                    }
-                },
-                {
-                    "aantal": 1.0,
-                    "criterium": {
-                        "meeteenheid": {
-                            "code": "M2",
-                            "naam": "Vierkante meter, m2"
-                        },
-                        "naam": "Badkamer/toilet"
-                    }
-                }
-            ]
-        },
-        {
-            "criteriumGroep": {
-                "stelsel": {
-                    "code": "ZEL",
-                    "naam": "Zelfstandige woonruimten"
+                        "naam": "Woonkamer1"
+                    },
+                    "punten": 0.75
                 },
-                "stelselgroep": {
-                    "code": "OOZ",
-                    "naam": "Oppervlakte van overige ruimten"
+                {
+                    "criterium": {
+                        "naam": "Woonkamer2"
+                    },
+                    "punten": 0.75
+                },
+                {
+                    "criterium": {
+                        "naam": "Woonkamer3"
+                    },
+                    "punten": 0.75
+                },
+                {
+                    "criterium": {
+                        "naam": "Woonkamer4"
+                    },
+                    "punten": 0.75
+                },
+                {
+                    "criterium": {
+                        "naam": "Woonkamer5"
+                    },
+                    "punten": 0.75
+                },
+                {
+                    "criterium": {
+                        "naam": "Woonkamer6"
+                    },
+                    "punten": 0.25
                 }
-            },
-            "punten": 0.0,
-            "woningwaarderingen": []
+            ]
         }
-    ],
-    "punten": 7.0
+    ]
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/output/peildatum/2024-01-01/zolder_vertrek.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_max_4_punten_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/collectief_open_keuken.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_max_4_punten_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/input/individueel_open_keuken.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_max_4_punten_overige_ruimten.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.2926587301587302%*

 * *Differences: {"'groepen'": "{0: {'punten': 10.5, 'woningwaarderingen': {1: {'punten': 1.5, 'criterium': "*

 * *              "{'naam': 'Open keuken in Verwarmde woonkamer'}}, 2: {'punten': 1.5, 'criterium': "*

 * *              "{'naam': 'Verwarmde keuken'}}, 3: {'punten': 1.5, 'criterium': {'naam': 'Verwarmde "*

 * *              "slaapkamer'}}, 4: {'punten': 1.5, 'criterium': {'naam': 'Open keuken in Verwarmde "*

 * *              "slaapkamer'}}, 5: {'punten': 1.5, 'criterium': {'naam': 'Verwarmde "*

 * *              "woonkamer/keuken'}}, 6: […]*

```diff
@@ -7,49 +7,60 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 4.0,
+            "punten": 10.5,
             "woningwaarderingen": [
                 {
                     "criterium": {
-                        "naam": "Woonkamer1"
+                        "naam": "Verwarmde woonkamer"
                     },
-                    "punten": 0.75
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer2"
+                        "naam": "Open keuken in Verwarmde woonkamer"
                     },
-                    "punten": 0.75
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer3"
+                        "naam": "Verwarmde keuken"
                     },
-                    "punten": 0.75
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer4"
+                        "naam": "Verwarmde slaapkamer"
                     },
-                    "punten": 0.75
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer5"
+                        "naam": "Open keuken in Verwarmde slaapkamer"
                     },
-                    "punten": 0.75
+                    "punten": 1.5
                 },
                 {
                     "criterium": {
-                        "naam": "Woonkamer6"
+                        "naam": "Verwarmde woonkamer/keuken"
                     },
-                    "punten": 0.25
+                    "punten": 1.5
+                },
+                {
+                    "criterium": {
+                        "naam": "Open keuken in Verwarmde woonkamer/keuken"
+                    },
+                    "punten": 1.5
                 }
             ]
         }
-    ]
+    ],
+    "punten": 10.5,
+    "stelsel": {
+        "code": "ZEL",
+        "naam": "Zelfstandige woonruimten"
+    }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/collectief_open_keuken.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_open_keuken.json`

 * *Files 4% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.798611111111111%*

 * *Differences: {"'groepen'": "{0: {'punten': 14.0, 'woningwaarderingen': {0: {'punten': 2}, 1: {'punten': 2}, 2: "*

 * *              "{'punten': 2}, 3: {'punten': 2}, 4: {'punten': 2}, 5: {'punten': 2}, 6: {'punten': "*

 * *              '2}}}}',*

 * * "'punten'": '14.0'}*

```diff
@@ -7,60 +7,60 @@
                     "naam": "Zelfstandige woonruimten"
                 },
                 "stelselgroep": {
                     "code": "VZE",
                     "naam": "Verwarming"
                 }
             },
-            "punten": 10.5,
+            "punten": 14.0,
             "woningwaarderingen": [
                 {
                     "criterium": {
                         "naam": "Verwarmde woonkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2
                 },
                 {
                     "criterium": {
                         "naam": "Open keuken in Verwarmde woonkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2
                 },
                 {
                     "criterium": {
                         "naam": "Verwarmde keuken"
                     },
-                    "punten": 1.5
+                    "punten": 2
                 },
                 {
                     "criterium": {
                         "naam": "Verwarmde slaapkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2
                 },
                 {
                     "criterium": {
                         "naam": "Open keuken in Verwarmde slaapkamer"
                     },
-                    "punten": 1.5
+                    "punten": 2
                 },
                 {
                     "criterium": {
                         "naam": "Verwarmde woonkamer/keuken"
                     },
-                    "punten": 1.5
+                    "punten": 2
                 },
                 {
                     "criterium": {
                         "naam": "Open keuken in Verwarmde woonkamer/keuken"
                     },
-                    "punten": 1.5
+                    "punten": 2
                 }
             ]
         }
     ],
-    "punten": 10.5,
+    "punten": 14.0,
     "stelsel": {
         "code": "ZEL",
         "naam": "Zelfstandige woonruimten"
     }
 }
```

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/data/output/peildatum/2024-01-01/individueel_max_4_punten_overige_ruimten.json`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py` & `woningwaardering-0.2.0a1/tests/stelsels/zelfstandige_woonruimten/verwarming/test_Verwarming.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/tests/test_utils.py` & `woningwaardering-0.2.0a1/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt` & `woningwaardering-0.2.0a1/wettelijke-documenten/BWBR0003237-geldend_van_01-01-2024_tm_heden_zichtdatum_06-03-2024.txt`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/__init__.py` & `woningwaardering-0.2.0a1/woningwaardering/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/stelsels/config/config.py` & `woningwaardering-0.2.0a1/woningwaardering/stelsels/config/config.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml` & `woningwaardering-0.2.0a1/woningwaardering/stelsels/config/zelfstandige_woonruimten.yml`

 * *Files 23% similar despite different names*

```diff
@@ -21,7 +21,15 @@
     module: verwarming
     class_naam: Verwarming
     begindatum: 2024-01-01
     versies:
       - module: verwarming_2024
         class_naam: Verwarming2024
         begindatum: 2024-01-01
+  energieprestatie:
+    module: energieprestatie
+    class_naam: Energieprestatie
+    begindatum: 2024-01-01
+    versies:
+      - module: energieprestatie_2024
+        class_naam: Energieprestatie2024
+        begindatum: 2024-01-01
```

### Comparing `woningwaardering-0.1.0a39/woningwaardering/stelsels/stelsel.py` & `woningwaardering-0.2.0a1/woningwaardering/stelsels/stelsel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/stelsels/stelselgroep.py` & `woningwaardering-0.2.0a1/woningwaardering/stelsels/stelselgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/stelsels/stelselgroepversie.py` & `woningwaardering-0.2.0a1/woningwaardering/stelsels/stelselgroepversie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/stelsels/utils.py` & `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,200 +1,214 @@
-from decimal import Decimal
-import importlib
-import os
-from datetime import date
-from typing import Type, TypeVar
+from decimal import ROUND_HALF_UP, Decimal
 
 from loguru import logger
-from prettytable import PrettyTable
 
+from woningwaardering.stelsels import Stelselgroepversie
+from woningwaardering.stelsels.utils import naar_tabel
+from woningwaardering.stelsels.zelfstandige_woonruimten.utils import (
+    classificeer_ruimte,
+    voeg_oppervlakte_kasten_toe_aan_ruimte,
+)
 from woningwaardering.vera.bvg.generated import (
+    EenhedenEenheid,
+    EenhedenRuimte,
+    WoningwaarderingResultatenWoningwaardering,
+    WoningwaarderingResultatenWoningwaarderingCriterium,
+    WoningwaarderingResultatenWoningwaarderingCriteriumGroep,
     WoningwaarderingResultatenWoningwaarderingGroep,
     WoningwaarderingResultatenWoningwaarderingResultaat,
 )
+from woningwaardering.vera.referentiedata import (
+    Meeteenheid,
+    Ruimtedetailsoort,
+    Ruimtesoort,
+    Woningwaarderingstelsel,
+    Woningwaarderingstelselgroep,
+)
+from woningwaardering.vera.referentiedata.bouwkundigelementdetailsoort import (
+    Bouwkundigelementdetailsoort,
+)
+from woningwaardering.vera.utils import heeft_bouwkundig_element
 
-T = TypeVar("T")
 
+class OppervlakteVanOverigeRuimten2024(Stelselgroepversie):
+    @staticmethod
+    def bereken(
+        eenheid: EenhedenEenheid,
+        woningwaardering_resultaat: (
+            WoningwaarderingResultatenWoningwaarderingResultaat | None
+        ) = None,
+    ) -> WoningwaarderingResultatenWoningwaarderingGroep:
+        woningwaardering_groep = WoningwaarderingResultatenWoningwaarderingGroep(
+            criteriumGroep=WoningwaarderingResultatenWoningwaarderingCriteriumGroep(
+                stelsel=Woningwaarderingstelsel.zelfstandige_woonruimten.value,
+                stelselgroep=Woningwaarderingstelselgroep.oppervlakte_van_overige_ruimten.value,
+            ),
+        )
 
-def import_class(module_path: str, class_naam: str, class_type: Type[T]) -> Type[T]:
-    """
-    Importeert een klasse uit een module.
-
-    Parameters:
-        module_path (str): Het pad naar de module waarin de klasse zich bevindt.
-        class_naam (str): De naam van de klasse die geïmporteerd moet worden.
-        class_type (Type[T]): Het verwachtte type van de klasse.
-
-    Returns:
-        Type[T]: De geïmporteerde klasse.
-
-    Raises:
-        ModuleNotFoundError: Als de module niet gevonden kan worden.
-        AttributeError: Als de klasse van het opgegeven type niet gevonden kan worden in de module.
-    """
-    logger.debug(f"Importeer class '{class_naam}' uit '{module_path}'")
-    try:
-        module = importlib.import_module(module_path)
-        class_: Type[T] = getattr(module, class_naam)
-        if not issubclass(class_, class_type):
-            raise TypeError(
-                f"class '{class_.__qualname__}' in '{class_.__module__}' is niet van het type '{class_type.__qualname__}'"
-            )
+        woningwaardering_groep.woningwaarderingen = []
 
-    except ModuleNotFoundError as e:
-        logger.error(f"Module {module_path} niet gevonden.", e)
-        raise
-
-    except AttributeError as e:
-        logger.error(f"Class {class_naam} niet gevonden in: {module_path}.", e)
-        raise
-
-    return class_
-
-
-def is_geldig(
-    begindatum: date = date.min,
-    einddatum: date = date.max,
-    peildatum: date = date.today(),
-) -> bool:
-    """
-    Controleert of de peildatum valt tussen de begindatum en einddatum.
-
-    Parameters:
-        begindatum (date): De begindatum.
-        einddatum (date): De einddatum.
-        peildatum (date): De peildatum.
-
-    Returns:
-        bool: True als de peildatum tussen de begindatum en einddatum valt, anders False.
-    """
-    return begindatum <= peildatum <= einddatum
-
-
-def vind_yaml_bestanden(directory: str) -> list[str]:
-    """
-    Zoekt alle YAML-bestanden in de opgegeven directory en de subdirectories.
-
-    Parameters:
-        directory (str): De hoofddirectory waarin naar YAML-bestanden wordt gezocht.
-
-    Returns:
-        list[str]: Een lijst met paden naar de gevonden YAML-bestanden.
-    """
-    logger.debug(f"Zoek naar YAML-bestanden in: {directory}")
-
-    yaml_files = [
-        os.path.join(root, file)
-        for root, _, files in os.walk(directory)
-        for file in files
-        if file.endswith((".yaml", ".yml"))
-    ]
-
-    if not yaml_files:
-        logger.error(f"Geen YAML-bestanden gevonden in: {directory}")
-    return yaml_files
-
-
-def naar_tabel(
-    woningwaardering_resultaat: (
-        WoningwaarderingResultatenWoningwaarderingResultaat
-        | WoningwaarderingResultatenWoningwaarderingGroep
-    ),
-) -> PrettyTable:
-    """
-    Genereer een tabel met de details van een woningwaarderingresultaat.
-
-    Parameters:
-        woningwaardering_resultaat (WoningwaarderingResultatenWoningwaarderingResultaat | WoningwaarderingResultatenWoningwaarderingGroep): Het object om de gegevens uit te halen
-
-    Returns:
-        PrettyTable: Een tabel met de gegevens van het woningwaarderingresultaat
-    """
-    table = PrettyTable()
-    table.field_names = ["Groep", "Naam", "Aantal", "Meeteenheid", "Punten"]
-    table.align["Groep"] = "l"
-    table.align["Naam"] = "l"
-    table.align["Aantal"] = "r"
-    table.align["Meeteenheid"] = "l"
-    table.align["Punten"] = "r"
-
-    table.float_format = ".2"
-
-    for woningwaardering_groep in (
-        woningwaardering_resultaat.groepen or []
-        if isinstance(
-            woningwaardering_resultaat,
-            WoningwaarderingResultatenWoningwaarderingResultaat,
-        )
-        else [woningwaardering_resultaat]
-    ):
-        woningwaarderingen = woningwaardering_groep.woningwaarderingen or []
-        aantal_waarderingen = len(woningwaarderingen)
-        for index, woningwaardering in enumerate(woningwaarderingen):
-            if (
-                woningwaardering_groep.criterium_groep
-                and woningwaardering_groep.criterium_groep.stelselgroep
-                and woningwaardering.criterium
-            ):
-                table.add_row(
-                    [
-                        woningwaardering_groep.criterium_groep.stelselgroep.naam,
-                        woningwaardering.criterium.naam,
-                        woningwaardering.aantal or "",
-                        woningwaardering.criterium.meeteenheid.naam
-                        if woningwaardering.criterium.meeteenheid is not None
-                        else "",
-                        woningwaardering.punten or "",
-                    ],
-                    divider=index + 1 == aantal_waarderingen,
-                )
-        if (
-            woningwaardering_groep.criterium_groep
-            and woningwaardering_groep.criterium_groep.stelselgroep
-        ):
-            table.add_row(
-                [
-                    woningwaardering_groep.criterium_groep.stelselgroep.naam,
-                    "Subtotaal",
-                    float(
-                        sum(
-                            [
-                                Decimal(woningwaardering.aantal)
-                                for woningwaardering in woningwaarderingen
-                                if woningwaardering.aantal is not None
-                            ]
+        for ruimte in eenheid.ruimten or []:
+            if ruimte.oppervlakte is None:
+                error_msg = f"ruimte {ruimte.id} heeft geen oppervlakte"
+                raise TypeError(error_msg)
+            if ruimte.detail_soort is None:
+                error_msg = f"ruimte {ruimte.id} heeft geen detailsoort"
+                raise TypeError(error_msg)
+
+            criterium_naam = voeg_oppervlakte_kasten_toe_aan_ruimte(ruimte)
+
+            if classificeer_ruimte(ruimte) == Ruimtesoort.overige_ruimtes:
+                if ruimte.oppervlakte < 2:
+                    logger.debug(
+                        f"{ruimte.naam} {ruimte.detail_soort.code} is kleiner dan 2 vierkante meter"
+                    )
+                    continue
+
+                woningwaardering = WoningwaarderingResultatenWoningwaardering()
+
+                woningwaardering.criterium = (
+                    WoningwaarderingResultatenWoningwaarderingCriterium(
+                        meeteenheid=Meeteenheid.vierkante_meter_m2.value,
+                        naam=criterium_naam,
+                    )
+                )
+
+                if (
+                    ruimte.gedeeld_met_aantal_eenheden is not None
+                    and ruimte.gedeeld_met_aantal_eenheden > 1
+                    and ruimte.detail_soort.code == Ruimtedetailsoort.berging.code
+                ):
+                    oppervlakte_per_eenheid = Decimal(
+                        ruimte.oppervlakte / ruimte.gedeeld_met_aantal_eenheden
+                    )
+
+                    if oppervlakte_per_eenheid >= 2:
+                        woningwaardering.aantal = float(
+                            (
+                                Decimal(str(ruimte.oppervlakte)).quantize(
+                                    Decimal("1"), ROUND_HALF_UP
+                                )
+                                / Decimal(str(ruimte.gedeeld_met_aantal_eenheden))
+                            ).quantize(Decimal("0.01"), ROUND_HALF_UP)
+                        )
+                    else:
+                        logger.debug(
+                            f"{ruimte.naam} {ruimte.detail_soort.code} is kleiner dan 2 vierkante meter per eenheid en komt niet in aanmerking voor een puntenwaardering onder {Woningwaarderingstelselgroep.oppervlakte_van_overige_ruimten.naam}"
                         )
+                        continue
+
+                elif ruimte.detail_soort.code == Ruimtedetailsoort.zolder.code:
+                    oppervlakte_aantal = OppervlakteVanOverigeRuimten2024._oppervlakte_zolder_overige_ruimte(
+                        ruimte
                     )
-                    or "",
-                    ", ".join(
-                        list(
-                            {
-                                woningwaardering.criterium.meeteenheid.naam or ""
-                                for woningwaardering in woningwaarderingen
-                                if woningwaardering.criterium is not None
-                                and woningwaardering.criterium.meeteenheid is not None
-                            }
+                    if oppervlakte_aantal > 0.0:
+                        woningwaardering.aantal = oppervlakte_aantal
+                    else:
+                        continue
+
+                else:
+                    woningwaardering.aantal = float(
+                        Decimal(str(ruimte.oppervlakte)).quantize(
+                            Decimal("0.01"), ROUND_HALF_UP
                         )
-                    ),
-                    woningwaardering_groep.punten,
-                ],
-                divider=True,
+                    )
+
+                woningwaardering_groep.woningwaarderingen.append(woningwaardering)
+
+        punten = Decimal(
+            sum(
+                Decimal(str(woningwaardering.aantal))
+                for woningwaardering in (
+                    woningwaardering_groep.woningwaarderingen or []
+                )
+                if woningwaardering.aantal is not None
             )
-    if (
-        isinstance(
-            woningwaardering_resultaat,
-            WoningwaarderingResultatenWoningwaarderingResultaat,
+        ).quantize(Decimal("1"), ROUND_HALF_UP) * Decimal("0.75")
+
+        woningwaardering_groep.punten = float(punten)
+        return woningwaardering_groep
+
+    @staticmethod
+    def _oppervlakte_zolder_overige_ruimte(ruimte: EenhedenRuimte) -> float:
+        """
+        Berekent de oppervlakte voor een zolder van een overige ruimte op basis van een EenhedenRuimte object.
+
+        Args:
+            ruimte (EenhedenRuimte): Het EenhedenRuimte object dat een zolder type is.
+
+        Returns:
+            float: De berekende oppervlakte voor de zolder.
+        """
+        if ruimte.detail_soort is not None and ruimte.oppervlakte is not None:
+            trap = heeft_bouwkundig_element(
+                ruimte, Bouwkundigelementdetailsoort.trap.code
+            )
+
+            if trap:
+                logger.debug(
+                    f"Trap gevonden in {ruimte.naam} ({ruimte.id}): telt mee voor {Woningwaarderingstelselgroep.oppervlakte_van_overige_ruimten.naam}"
+                )
+                return float(
+                    Decimal(str(ruimte.oppervlakte)).quantize(
+                        Decimal("0.01"), ROUND_HALF_UP
+                    )
+                )
+
+            vlizotrap = heeft_bouwkundig_element(
+                ruimte, Bouwkundigelementdetailsoort.vlizotrap.code
+            )
+
+            if vlizotrap:
+                logger.debug(
+                    f"Vlizotrap gevonden in {ruimte.naam} ({ruimte.id}): telt mee voor oppervlakte van overige ruimten"
+                )
+                return max(
+                    0.0,
+                    float(
+                        Decimal(
+                            Decimal(str(ruimte.oppervlakte)).quantize(
+                                Decimal("0.01"), ROUND_HALF_UP
+                            )
+                            # Min 5 punten omdat de ruimte niet bereikt kan worden met een
+                            # vaste trap.
+                            # Let op, hier wordt de oppervlakte gecorrigeerd met de
+                            # hoeveelheid punten per vierkante meter. Onze keuze is om hier
+                            # al de vijf punten in mindering te brengen. Het beleidsboek
+                            # geeft aan dat de punten in mindering gebracht moeten worden
+                            # op de punten berekend voor deze ruimte, maar ook dat punten
+                            # pas berekend moeten worden wanneer de totale oppervlakte
+                            # bekend is en afegerond is.
+                            # Door de afronding komt deze berekening niet helemaal juist
+                            # uit, maar dit is de benadering waar wij nu voor kiezen.
+                            - Decimal("5") / Decimal("0.75")
+                        ).quantize(Decimal("0.01"), ROUND_HALF_UP)
+                    ),
+                )
+
+        logger.warning(
+            f"Geen trap gevonden in {ruimte.naam} ({ruimte.id}): telt niet mee voor {Woningwaarderingstelselgroep.oppervlakte_van_overige_ruimten.naam}"
         )
-        and woningwaardering_resultaat.stelsel
-    ):
-        table.add_row(
-            [
-                woningwaardering_resultaat.stelsel.naam,
-                "Afgerond totaal",
-                "",
-                "",
-                woningwaardering_resultaat.punten,
-            ],
-            divider=True,
+        return 0.0
+
+
+if __name__ == "__main__":
+    logger.enable("woningwaardering")
+
+    oppervlakte_van_overige_ruimten = OppervlakteVanOverigeRuimten2024()
+    with open(
+        "tests/data/input/zelfstandige_woonruimten/85651000021.json",
+        "r+",
+    ) as file:
+        eenheid = EenhedenEenheid.model_validate_json(file.read())
+
+    woningwaardering_resultaat = oppervlakte_van_overige_ruimten.bereken(eenheid)
+
+    print(
+        woningwaardering_resultaat.model_dump_json(
+            by_alias=True, indent=2, exclude_none=True
         )
+    )
+
+    tabel = naar_tabel(woningwaardering_resultaat)
 
-    return table
+    print(tabel)
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py` & `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py` & `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py` & `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py` & `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/utils.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py` & `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py` & `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/verwarming_2024.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py` & `woningwaardering-0.2.0a1/woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py`

 * *Files 8% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 if __name__ == "__main__":
     logger.enable("woningwaardering")
 
     zelfstandige_woonruimten = ZelfstandigeWoonruimten()
     file = open(
-        "./tests/data/input/zelfstandige_woonruimten/41123000005.json",
+        "./tests/data/input/generiek/37101000032.json",
         "r+",
     )
     eenheid = EenhedenEenheid.model_validate_json(file.read())
     woningwaardering_resultaat = zelfstandige_woonruimten.bereken(eenheid)
     print(
         woningwaardering_resultaat.model_dump_json(
             by_alias=True, indent=2, exclude_none=True
```

### Comparing `woningwaardering-0.1.0a39/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2` & `woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelsel.py.j2`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2` & `woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroep.py.j2`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2` & `woningwaardering-0.2.0a1/woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/bvg/generated.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/bvg/generated.py`

 * *Files 0% similar despite different names*

```diff
@@ -946,14 +946,26 @@
     """
     Het energielabel voor woningen geeft met klassen (A**** tot en met G) en kleuren (groen tot en met rood) aan hoe energiezuinig een huis is ten opzichte van andere soortgelijke woningen. Energielabel A (donkergroen) is zuinig, energielabel G (rood) is onzuinig. Het energielabel is meestal een afgeleide van de waarde van de energieprestatie. Referentiedatasoort ENERGIELABEL.
     """
     waarde: Optional[str] = None
     """
     De door een adviseur gemeten waarde die hoort bij de energieprestatie. De energieprestatiesoort bepaalt wat deze waarde representeert. Bijvoorbeeld: Energie-index of EP2 (het energielabel  is daarvan dan afgeleid), compactheid of opgewekte duurzame energie. Bij een voorlopig energielabel is geen waarde van toepassing.
     """
+    # https://github.com/Aedes-datastandaarden/vera-openapi/issues/58
+    gebruiksoppervlakte_thermische_zone: Optional[float] = Field(
+        default=None, alias="gebruiksoppervlakteThermischeZone"
+    )
+    """
+    Gebruiksoppervlakte van de thermische zone, afgebakend volgens NTA 8800
+    """
+    # https://github.com/Aedes-datastandaarden/vera-openapi/issues/59
+    energieprestatievergoeding: Optional[bool] = Field(default=None)
+    """
+    Geeft aan of er bij het verhuren een energieprestatievergoeding (EPV) is overeengekomen
+    """
 
 
 class EenhedenGemeente(BaseModel):
     model_config = ConfigDict(
         populate_by_name=True,
     )
     id: Optional[str] = None
@@ -3241,14 +3253,19 @@
     De omschrijving van de zorgfaciliteit behorende bij de eenheid.
     """
     # https://github.com/Aedes-datastandaarden/vera-openapi/issues/54
     klimaatbeheersingsoort: Optional[Referentiedata] = None
     """
     Het soort klimaatbeheersing. Bijvoorbeeld: individueel of collectief. Referentiedatasoort EENHEIDKLIMAATBEHEERSINGSOORT.
     """
+    # https://github.com/Aedes-datastandaarden/vera-openapi/issues/57
+    woningtype: Optional[Referentiedata] = None
+    """
+    Het type woning: eengezinswoning of meergezinswoning. Referentiedatasoort WONINGTYPE.
+    """
 
 
 class WoningwaarderingResultatenWoningwaarderingResultaatbericht(
     WoningwaarderingResultatenWoningwaarderingResultaat, BerichtBasis
 ):
     pass
     model_config = ConfigDict(
```

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/__init__.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -182,14 +182,15 @@
 from .verbijzonderingsoort import Verbijzonderingsoort
 from .verbijzonderingstatus import Verbijzonderingstatus
 from .verrekeningsoort import Verrekeningsoort
 from .vertrouwelijkheid import Vertrouwelijkheid
 from .voorrangdetailsoort import Voorrangdetailsoort
 from .voorrangsoort import Voorrangsoort
 from .vragenlijstregelherkomst import Vragenlijstregelherkomst
+from .woningtype import Woningtype
 from .woningwaarderingstelsel import Woningwaarderingstelsel
 from .woningwaarderingstelselgroep import Woningwaarderingstelselgroep
 from .woonsituatiesoort import Woonsituatiesoort
 from .woonvorm import Woonvorm
 from .zaakobjectsoort import Zaakobjectsoort
 from .zaakrol import Zaakrol
 from .zaakstatussoort import Zaakstatussoort
@@ -383,14 +384,15 @@
     "Verbijzonderingsoort",
     "Verbijzonderingstatus",
     "Verrekeningsoort",
     "Vertrouwelijkheid",
     "Voorrangdetailsoort",
     "Voorrangsoort",
     "Vragenlijstregelherkomst",
+    "Woningtype",
     "Woningwaarderingstelsel",
     "Woningwaarderingstelselgroep",
     "Woonsituatiesoort",
     "Woonvorm",
     "Zaakobjectsoort",
     "Zaakrol",
     "Zaakstatussoort",
```

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/aanbiedingstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aanbiedingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aanvullendedoelgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/accountstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/accountstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/adressoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/adressoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/afletterstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afletterstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/afrekenwijzesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afrekenwijzesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/afspraakstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afspraakstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afspraakverzoeksoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/afwezigheidsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/afwezigheidsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/aktesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/aktesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/authentiekgegevenbron.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/authentiekgegevenbron.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/authentiekgegevensoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/authentiekgegevensoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/authentiekgegevenstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/bedrijfsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bedrijfsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/begrotingversie.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/begrotingversie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/bestemming.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bestemming.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/betaalgegevensoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betaalgegevensoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betaalwijzedeelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/betaalwijzesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betaalwijzesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betalingsregelingeindereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/betalingsregelingstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/betalingsregelingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/boekingdetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekingdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/boekingsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/boekingstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekjaarperiodesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekjaarperiodestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/boekjaarstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/boekjaarstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bouwkundigelementdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bouwkundigelementplaatsing.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/bouwkundigelementsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/brandwerendheidscore.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/brandwerendheidscore.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/btw.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/btw.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/btwaangiftestatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/btwaangiftestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/burgerlijkestaat.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/burgerlijkestaat.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/clustersoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/clustersoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/collectiefobjectsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/collectiefobjectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/communicatiekanaal.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/communicatiekanaal.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/communicatierichting.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/communicatierichting.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/conditiescore.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/conditiescore.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevendetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/contactgegevensoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevensoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/contactgegevenstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevenstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/contactgegevenvoorkeur.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/crediteursoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/crediteursoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/crediteurstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/crediteurstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/dagdeel.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/dagdeel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/debiteursoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/debiteursoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/debiteurstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/debiteurstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/defectlocatie.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectlocatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/defectoorzaak.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectoorzaak.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/defectsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/defectstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/defectstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/doelgroep.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/doelgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/dossier/__init__.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/dossier/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriasoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriumdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriumsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidcriteriumtoepassing.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheiddetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheiddetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheiddetailstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheiddetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidenergievoorziening.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidinterieur.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidinterieur.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidisolatie.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidisolatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidklimaatbeheersing.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidklimaatbeheersingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidligging.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidligging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidmonument.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidmonument.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidprijsconditie.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidprijsconditie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidsanitair.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidsanitair.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eenheidstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eenheidstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eindedetailreden.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eindedetailreden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/eindereden.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/eindereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/energielabel.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energielabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/energieprestatiesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energieprestatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/energieprestatiestatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energieprestatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/energieprestatievergoedingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/externeincassosoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/externeincassosoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/externeincassostatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/externeincassostatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/factuurbetaalwijze.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/factuurbetaalwijze.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/factuursoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/factuursoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/financien/__init__.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/financien/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/gebeurtenissoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/gebeurtenissoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/geometriesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/geometriesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/geslacht.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/geslacht.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/grootboekmutatieherkomst.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/grootboekrekeningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/grootboekrekeningstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/huurgeschilsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huurgeschilsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/huurgeschilstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huurgeschilstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/huurklasse.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huurklasse.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/huuropzeggingstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/huuropzeggingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/incassomoment.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/incassomoment.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inexploitatiereden.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inexploitatiereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/informatieobjectdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/informatieobjectsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/informatieobjectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inkomensbron.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkomensbron.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inkomenssoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkomenssoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkomensverklaringsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkoopfactuurstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inkoopopdrachtregelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inschrijvingherkomst.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inschrijvingherkomst.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inspectierapportsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inspectierapportsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/inspectierapportstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/inspectierapportstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kandidaatdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/kandidaatstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kandidaatstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/kwaliteitsniveau.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/kwaliteitsniveau.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/leningaflosvorm.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/leningaflosvorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/leningdetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/leningdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/leningsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/leningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/maatschappelijklabel.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/maatschappelijklabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/machtigingsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/machtigingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/materiaaldetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/materiaaldetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/materiaalsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/materiaalsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/medewerkerrol.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/medewerkerrol.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/medewerkersoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/medewerkersoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/meeteenheid.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/meeteenheid.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoud/__init__.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoud/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsbestedingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudslabel.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudslabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsorderstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudspecialisme.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudspecialisme.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudstaakdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudstaakstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/onderhoudsverzoekstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/opleidingsniveau.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/opleidingsniveau.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/oppervlaktesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/oppervlaktesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/opzegtermijn.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/opzegtermijn.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/organisatievorm.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/organisatievorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomsten/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstkoppelingdetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstkoppelingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/overeenkomstsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomstsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/overeenkomststatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/overeenkomststatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/passendheiddetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/passendheiddetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/passendheidssoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/passendheidssoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/prestatieafspraak.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prestatieafspraak.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijsaanpassingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/prijscomponentsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentsubsidiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/prijscomponentwijzigingsreden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectbudgetregelregelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectbudgetregelsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectbudgetregelstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectfasebesluitstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/projectsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/projectstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/projectstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/provincie.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/provincie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/publicatiedetailmodel.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiedetailmodel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/publicatiedetailstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiedetailstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/publicatieintakevorm.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatieintakevorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/publicatiemodel.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiemodel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/publicatiestatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/publicatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/puntenberekeningsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/puntenberekeningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/puntenmutatiesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/puntenmutatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/reclamatiesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/reclamatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/reclamatiestatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/reclamatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/redenontbinding.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/redenontbinding.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/redenopzegging.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/redenopzegging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/redenvernietiging.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/redenvernietiging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/regiesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/regiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/relatieadressoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatieadressoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/relatiedetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatiedetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/relatierolsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatierolsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/relaties/__init__.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relaties/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/relatiesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/relatiestatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/relatiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/rentesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/rentesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/ruimtedetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/ruimtedetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/ruimteligging.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/ruimteligging.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/ruimtesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/ruimtesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/sanctiesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/sanctiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/sanctiestatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/sanctiestatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/signaleringdetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/signaleringdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/signaleringsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/signaleringsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/signaleringstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/signaleringstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/taal.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/taal.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/toegankelijkheidslabel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/uitexploitatiereden.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/uitexploitatiereden.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/uitvoerendesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/uitvoerendesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/vastgoed/__init__.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/vastgoed/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     Prestatieafspraak,
     Provincie,
     Ruimtedetailsoort,
     Ruimteligging,
     Ruimtesoort,
     Toegankelijkheidslabel,
     Uitexploitatiereden,
+    Woningtype,
     Woningwaarderingstelsel,
     Woningwaarderingstelselgroep,
     Woonvorm,
     Zekerheidverpandingsoort,
 )
 
 
@@ -89,12 +90,13 @@
     "Prestatieafspraak",
     "Provincie",
     "Ruimtedetailsoort",
     "Ruimteligging",
     "Ruimtesoort",
     "Toegankelijkheidslabel",
     "Uitexploitatiereden",
+    "Woningtype",
     "Woningwaarderingstelsel",
     "Woningwaarderingstelselgroep",
     "Woonvorm",
     "Zekerheidverpandingsoort",
 ]
```

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verantwoordingconsolidatie.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/verantwoordingregime.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verantwoordingregime.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/verbijzonderingsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verbijzonderingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/verbijzonderingstatus.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verbijzonderingstatus.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/verrekeningsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/verrekeningsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/vertrouwelijkheid.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/vertrouwelijkheid.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/voorrangdetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/voorrangdetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/voorrangsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/voorrangsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woningwaarderingstelsel.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woonruimteverdeling/__init__.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/woonsituatiesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woonsituatiesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/woonvorm.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/woonvorm.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/zaakobjectsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaakobjectsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/zaakrol.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaakrol.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/zaakstatussoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaakstatussoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaaktypedetailsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/zaaktypesoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zaaktypesoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/referentiedata/zekerheidverpandingsoort.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering/vera/utils.py` & `woningwaardering-0.2.0a1/woningwaardering/vera/utils.py`

 * *Files identical despite different names*

### Comparing `woningwaardering-0.1.0a39/woningwaardering.egg-info/PKG-INFO` & `woningwaardering-0.2.0a1/woningwaardering.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 Metadata-Version: 2.1
 Name: woningwaardering
-Version: 0.1.0a39
+Version: 0.2.0a1
 Summary: Berekent de punten van een woning op basis van het woningwaarderingsstelsel.
-Author: Woonstad Rotterdam
-Author-email: Ben Verhees <ben.verhees@woonstadrotterdam.nl>, Tiddo Loos <tiddo.loos@woonstadrotterdam.nl>, Tomer Gabay <tomer.gabay@woonstadrotterdam.nl>
+Author-email: Woonstad Rotterdam <info@woonstadrotterdam.nl>, Ben Verhees <ben.verhees@woonstadrotterdam.nl>, Tiddo Loos <tiddo.loos@woonstadrotterdam.nl>, Tomer Gabay <tomer.gabay@woonstadrotterdam.nl>
 Project-URL: Homepage, https://github.com/WoonstadRotterdamTemp/woningwaardering
 Project-URL: Issues, https://github.com/WoonstadRotterdamTemp/woningwaardering/issues
 Keywords: woning,waardering,stelsel,woningwaarderingsstelsel,wws
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: License :: OSI Approved :: MIT License
@@ -16,19 +15,21 @@
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: pydantic==2.*
 Requires-Dist: loguru==0.7.*
 Requires-Dist: types-pyyaml==6.*
 Requires-Dist: PyYAML==6.*
 Requires-Dist: prettytable==3.*
+Requires-Dist: pandas==2.*
 Provides-Extra: test
 Requires-Dist: pre-commit==3.3.*; extra == "test"
 Requires-Dist: ruff==0.3.*; extra == "test"
 Requires-Dist: pytest==8.0.*; extra == "test"
 Requires-Dist: types-requests==2.*; extra == "test"
+Requires-Dist: types-python-dateutil==2.*; extra == "test"
 Provides-Extra: dev
 Requires-Dist: woningwaardering[test]; extra == "dev"
 Requires-Dist: datamodel-code-generator[http]==0.25.5; extra == "dev"
 Requires-Dist: unidecode==1.*; extra == "dev"
 Requires-Dist: jinja2==3.*; extra == "dev"
 Requires-Dist: types-pyyaml==6.*; extra == "dev"
 Requires-Dist: PyYAML==6.*; extra == "dev"
```

### Comparing `woningwaardering-0.1.0a39/woningwaardering.egg-info/SOURCES.txt` & `woningwaardering-0.2.0a1/woningwaardering.egg-info/SOURCES.txt`

 * *Files 18% similar despite different names*

```diff
@@ -66,14 +66,24 @@
 tests/stelsels/test_ZelfstandigeWoonruimten.py
 tests/stelsels/config/test_config.py
 tests/stelsels/stelsel/test_select_geldige_stelselgroepversies.py
 tests/stelsels/stelselgroep/test_select_geldige_stelselgroepversie.py
 tests/stelsels/utils/test_import_class.py
 tests/stelsels/utils/test_is_geldig.py
 tests/stelsels/utils/test_vind_yaml_bestanden.py
+tests/stelsels/zelfstandige_woonruimten/energieprestatie/test_Energieprestatie.py
+tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.json
+tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_A++++_egw.md
+tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.json
+tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_egw.md
+tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.json
+tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/input/eenheid_epv_mgw.md
+tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_A++++_egw.json
+tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_egw.json
+tests/stelsels/zelfstandige_woonruimten/energieprestatie/data/output/peildatum/2024-01-01/eenheid_epv_mgw.json
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/test_OppervlakteVanOverigeRuimten.py
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.json
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/input/zolder_overige_ruimten.md
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/data/output/peildatum/2024-01-01/zolder_overige_ruimten.json
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/test_OppervlakteVanVertrekken.py
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/badkamer_en_of_toilet_boven_en_onder_0.64.json
 tests/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/data/input/gedeelde_berging.json
@@ -114,14 +124,22 @@
 woningwaardering/stelsels/utils.py
 woningwaardering/stelsels/config/__init__.py
 woningwaardering/stelsels/config/config.py
 woningwaardering/stelsels/config/zelfstandige_woonruimten.yml
 woningwaardering/stelsels/zelfstandige_woonruimten/__init__.py
 woningwaardering/stelsels/zelfstandige_woonruimten/utils.py
 woningwaardering/stelsels/zelfstandige_woonruimten/zelfstandige_woonruimten.py
+woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/__init__.py
+woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie.py
+woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/energieprestatie_2024.py
+woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/bouwjaar_punten.csv
+woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_0-25m2_energielabel_punten.csv
+woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_25-40m2_energielabel_punten.csv
+woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oppervlakte_40m2+_energielabel_punten.csv
+woningwaardering/stelsels/zelfstandige_woonruimten/energieprestatie/lookup_tabellen/oud_energielabel_punten.csv
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/__init__.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_overige_ruimten/oppervlakte_van_overige_ruimten_2024.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/__init__.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken.py
 woningwaardering/stelsels/zelfstandige_woonruimten/oppervlakte_van_vertrekken/oppervlakte_van_vertrekken_2024.py
 woningwaardering/stelsels/zelfstandige_woonruimten/verwarming/__init__.py
@@ -134,14 +152,15 @@
 woningwaardering/templates/stelsels/stelsel/stelselgroep/stelselgroepversie.py.j2
 woningwaardering/vera/__init__.py
 woningwaardering/vera/referentiedata_uitbreiding.csv
 woningwaardering/vera/utils.py
 woningwaardering/vera/bvg/__init__.py
 woningwaardering/vera/bvg/generated.py
 woningwaardering/vera/bvg/model_uitbreidingen/eenheden_eenheid.py
+woningwaardering/vera/bvg/model_uitbreidingen/eenheden_energieprestatie.py
 woningwaardering/vera/bvg/model_uitbreidingen/eenheden_ruimte.py
 woningwaardering/vera/bvg/model_uitbreidingen/referentiedata.py
 woningwaardering/vera/referentiedata/__init__.py
 woningwaardering/vera/referentiedata/aanbiedingdetailstatus.py
 woningwaardering/vera/referentiedata/aanbiedingstatus.py
 woningwaardering/vera/referentiedata/aanvullendedoelgroep.py
 woningwaardering/vera/referentiedata/accountstatus.py
@@ -325,14 +344,15 @@
 woningwaardering/vera/referentiedata/verbijzonderingsoort.py
 woningwaardering/vera/referentiedata/verbijzonderingstatus.py
 woningwaardering/vera/referentiedata/verrekeningsoort.py
 woningwaardering/vera/referentiedata/vertrouwelijkheid.py
 woningwaardering/vera/referentiedata/voorrangdetailsoort.py
 woningwaardering/vera/referentiedata/voorrangsoort.py
 woningwaardering/vera/referentiedata/vragenlijstregelherkomst.py
+woningwaardering/vera/referentiedata/woningtype.py
 woningwaardering/vera/referentiedata/woningwaarderingstelsel.py
 woningwaardering/vera/referentiedata/woningwaarderingstelselgroep.py
 woningwaardering/vera/referentiedata/woonsituatiesoort.py
 woningwaardering/vera/referentiedata/woonvorm.py
 woningwaardering/vera/referentiedata/zaakobjectsoort.py
 woningwaardering/vera/referentiedata/zaakrol.py
 woningwaardering/vera/referentiedata/zaakstatussoort.py
```

