# Comparing `tmp/great_tables-0.5.2.tar.gz` & `tmp/great_tables-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "great_tables-0.5.2.tar", last modified: Mon May 13 17:52:50 2024, max compression
+gzip compressed data, was "great_tables-0.6.0.tar", last modified: Thu May 16 20:30:47 2024, max compression
```

## Comparing `great_tables-0.5.2.tar` & `great_tables-0.6.0.tar`

### file list

```diff
@@ -1,262 +1,280 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.086212 great_tables-0.5.2/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/.github/
--rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/CODE_OF_CONDUCT.md
--rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/CONTRIBUTING.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/.github/ISSUE_TEMPLATE/
--rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/ISSUE_TEMPLATE/bug.md
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/ISSUE_TEMPLATE/feature.md
--rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/PULL_REQUEST_TEMPLATE.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/scripts/no_pandas.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/workflows/ci-docs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2002 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/workflows/ci-tests.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-13 17:52:45.000000 great_tables-0.5.2/.github/workflows/code-checks.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-13 17:52:45.000000 great_tables-0.5.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-13 17:52:45.000000 great_tables-0.5.2/.pre-commit-config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/.vscode/
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-13 17:52:45.000000 great_tables-0.5.2/.vscode/launch.json
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-13 17:52:45.000000 great_tables-0.5.2/.vscode/settings.json
--rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-13 17:52:45.000000 great_tables-0.5.2/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-13 17:52:45.000000 great_tables-0.5.2/CHANGELOG.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     5243 2024-05-13 17:52:45.000000 great_tables-0.5.2/CODE_OF_CONDUCT.md
--rwxr-xr-x   0 runner    (1001) docker     (127)     2259 2024-05-13 17:52:45.000000 great_tables-0.5.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-13 17:52:45.000000 great_tables-0.5.2/HISTORY.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     1081 2024-05-13 17:52:45.000000 great_tables-0.5.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 17:52:45.000000 great_tables-0.5.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-13 17:52:45.000000 great_tables-0.5.2/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-05-13 17:52:50.086212 great_tables-0.5.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-13 17:52:45.000000 great_tables-0.5.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.014210 great_tables-0.5.2/docs/_extensions/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.014210 great_tables-0.5.2/docs/_extensions/machow/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/docs/_extensions/machow/interlinks/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/_extensions/machow/interlinks/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/_extensions/machow/interlinks/_extension.yml
--rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/_extensions/machow/interlinks/interlinks.lua
--rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/_quarto.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.022211 great_tables-0.5.2/docs/articles/
--rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/articles/intro.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.030211 great_tables-0.5.2/docs/assets/
--rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/assets/GT_logo.svg
--rw-r--r--   0 runner    (1001) docker     (127)  2325288 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/assets/datasets.png
--rw-r--r--   0 runner    (1001) docker     (127)   136430 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/assets/gt_parts_of_a_table.svg
--rw-r--r--   0 runner    (1001) docker     (127)   342328 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/assets/gt_sp500_table.svg
--rw-r--r--   0 runner    (1001) docker     (127)    74998 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/assets/gt_workflow_diagram.svg
--rw-r--r--   0 runner    (1001) docker     (127)   209904 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/assets/tables_from_the_web.png
--rw-r--r--   0 runner    (1001) docker     (127)   139817 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/assets/the_components_of_a_table.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.030211 great_tables-0.5.2/docs/blog/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.030211 great_tables-0.5.2/docs/blog/bring-your-own-df/
--rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/bring-your-own-df/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.038211 great_tables-0.5.2/docs/blog/design-philosophy/
--rw-r--r--   0 runner    (1001) docker     (127)   241842 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/a_simple_table.png
--rw-r--r--   0 runner    (1001) docker     (127)   195558 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/cave_grids.png
--rw-r--r--   0 runner    (1001) docker     (127)   656631 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/composition_of_a_table_in_GT.png
--rw-r--r--   0 runner    (1001) docker     (127)   801735 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/computer_tables.png
--rw-r--r--   0 runner    (1001) docker     (127)    22595 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)  1486510 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/nippur_cuneiform_tablet.png
--rw-r--r--   0 runner    (1001) docker     (127)  1629638 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png
--rw-r--r--   0 runner    (1001) docker     (127)   458471 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/uruk_tablet_with_annotations.png
--rw-r--r--   0 runner    (1001) docker     (127)   812542 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/design-philosophy/visicalc.png
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.038211 great_tables-0.5.2/docs/blog/introduction-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/introduction-0.2.0/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.038211 great_tables-0.5.2/docs/blog/introduction-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/introduction-0.3.0/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.038211 great_tables-0.5.2/docs/blog/introduction-0.4.0/
--rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/introduction-0.4.0/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/introduction_great_tables.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.038211 great_tables-0.5.2/docs/blog/polars-styling/
--rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/polars-styling/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)   132380 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/polars-styling/table-preview.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.042211 great_tables-0.5.2/docs/blog/superbowl-squares/
--rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/superbowl-squares/_code.py
--rw-r--r--   0 runner    (1001) docker     (127)  1949299 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/superbowl-squares/games.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/blog/superbowl-squares/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.042211 great_tables-0.5.2/docs/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.042211 great_tables-0.5.2/docs/examples/_data/
--rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/_data/power_cie_prepared_tbl.csv
--rw-r--r--   0 runner    (1001) docker     (127)     9028 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/index.qmd
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.046211 great_tables-0.5.2/docs/examples/sports-earnings/
--rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/sports-earnings/basketball.png
--rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/sports-earnings/boxing.png
--rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/sports-earnings/golf.png
--rw-r--r--   0 runner    (1001) docker     (127)    76604 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/sports-earnings/index.ipynb
--rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/sports-earnings/soccer.png
--rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/sports-earnings/sports_earnings.csv
--rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/examples/sports-earnings/tennis.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.046211 great_tables-0.5.2/docs/get-started/
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/basic-column-labels.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/basic-formatting.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/basic-header.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/basic-stub.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/basic-styling.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/colorizing-with-data.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/column-selection.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/index.qmd
--rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/nanoplots.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/overview.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/row-selection.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/table-theme-options.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/get-started/table-theme-premade.qmd
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-13 17:52:45.000000 great_tables-0.5.2/docs/styles.css
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.054211 great_tables-0.5.2/great_tables/
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_body.py
--rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_boxhead.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.058211 great_tables-0.5.2/great_tables/_data_color/
--rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_data_color/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_data_color/base.py
--rw-r--r--   0 runner    (1001) docker     (127)    27133 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_data_color/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_data_color/palettes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_databackend.py
--rw-r--r--   0 runner    (1001) docker     (127)     9275 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_export.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_footnotes.py
--rw-r--r--   0 runner    (1001) docker     (127)   151729 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)    40689 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_formats_vals.py
--rw-r--r--   0 runner    (1001) docker     (127)    43858 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_gt_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_heading.py
--rw-r--r--   0 runner    (1001) docker     (127)    32944 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_locale.py
--rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    74939 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_render.py
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_row_groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_scss.py
--rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_source_notes.py
--rw-r--r--   0 runner    (1001) docker     (127)    25402 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_spanners.py
--rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_stub.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_stubhead.py
--rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_substitution.py
--rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_tab_create_modify.py
--rw-r--r--   0 runner    (1001) docker     (127)    16622 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_tbl_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_text.py
--rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_types.py
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    55726 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_utils_nanoplots.py
--rw-r--r--   0 runner    (1001) docker     (127)    27299 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/_utils_render_html.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.058211 great_tables-0.5.2/great_tables/css/
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/css/gt_colors.scss
--rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/css/gt_styles_default.scss
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.066212 great_tables-0.5.2/great_tables/data/
--rw-r--r--   0 runner    (1001) docker     (127)   412361 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/01-countrypops.csv
--rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/02-sza.csv
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/03-gtcars.csv
--rw-r--r--   0 runner    (1001) docker     (127)   906055 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/04-sp500.csv
--rw-r--r--   0 runner    (1001) docker     (127)  2848391 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/05-pizzaplace.csv
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/06-exibble.csv
--rw-r--r--   0 runner    (1001) docker     (127)    81025 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/07-towny.csv
--rw-r--r--   0 runner    (1001) docker     (127)    20916 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/08-metro.csv
--rw-r--r--   0 runner    (1001) docker     (127)    21007 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/09-constants.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/10-illness.csv
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/11-islands.csv
--rw-r--r--   0 runner    (1001) docker     (127)    28127 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.074212 great_tables-0.5.2/great_tables/data/metro_images/
--rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_1.svg
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_10.svg
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_11.svg
--rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_12.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_13.svg
--rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_14.svg
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_2.svg
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_3.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_3bis.svg
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_4.svg
--rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_5.svg
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_6.svg
--rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_7.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_7bis.svg
--rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_8.svg
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/metro_9.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/rer_A.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/rer_B.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/rer_C.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/rer_D.svg
--rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/rer_E.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T1.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T11.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T13.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T2.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T3a.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T3b.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T4.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T5.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T6.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T7.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T8.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/tram_T9.svg
--rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_H.svg
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_J.svg
--rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_K.svg
--rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_L.svg
--rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_N.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_P.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_R.svg
--rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/metro_images/transilien_U.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/x-airquality.csv
--rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/x_currencies.csv
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/x_currency_symbols.csv
--rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/x_default_locales.csv
--rw-r--r--   0 runner    (1001) docker     (127)   255709 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/data/x_locales.csv
--rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/gt.py
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/loc.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/shiny.py
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/style.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/utils_render_common.py
--rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-13 17:52:45.000000 great_tables-0.5.2/great_tables/vals.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.082212 great_tables-0.5.2/great_tables.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-05-13 17:52:49.000000 great_tables-0.5.2/great_tables.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     7525 2024-05-13 17:52:50.000000 great_tables-0.5.2/great_tables.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:52:49.000000 great_tables-0.5.2/great_tables.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-13 17:52:49.000000 great_tables-0.5.2/great_tables.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-13 17:52:49.000000 great_tables-0.5.2/great_tables.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-13 17:52:45.000000 great_tables-0.5.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-13 17:52:45.000000 great_tables-0.5.2/pyrightconfig.json
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:52:50.086212 great_tables-0.5.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.078212 great_tables-0.5.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.082212 great_tables-0.5.2/tests/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)    10002 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_export.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    14024 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_formats.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_locations.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_options.ambr
--rw-r--r--   0 runner    (1001) docker     (127)    31704 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_repr.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_scss.ambr
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_tbl_data.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     7441 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/__snapshots__/test_utils_render_html.ambr
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.082212 great_tables-0.5.2/tests/data_color/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:52:50.082212 great_tables-0.5.2/tests/data_color/__snapshots__/
--rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/data_color/__snapshots__/test_data_color.ambr
--rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/data_color/test_data_color.py
--rw-r--r--   0 runner    (1001) docker     (127)    18147 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/data_color/test_data_color_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test__boxhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test__formats_vals.py
--rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test__stubhead.py
--rw-r--r--   0 runner    (1001) docker     (127)    54571 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test__utils_nanoplots.py
--rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_body.py
--rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_boxhead.py
--rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (127)    55851 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_formats_nanoplots.py
--rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_gt.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_gt_data.py
--rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_heading.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_repr.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_scss.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_shiny.py
--rw-r--r--   0 runner    (1001) docker     (127)     9587 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_spanners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_styles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_substitutions.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_tab_create_modify.py
--rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_tbl_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_utils_render_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     4123 2024-05-13 17:52:45.000000 great_tables-0.5.2/tests/test_utils_render_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.106188 great_tables-0.6.0/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.046188 great_tables-0.6.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)     5246 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/CODE_OF_CONDUCT.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2847 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/CONTRIBUTING.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.046188 great_tables-0.6.0/.github/ISSUE_TEMPLATE/
+-rw-r--r--   0 runner    (1001) docker     (127)     1370 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/ISSUE_TEMPLATE/bug.md
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/ISSUE_TEMPLATE/feature.md
+-rw-r--r--   0 runner    (1001) docker     (127)      545 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0 runner    (1001) docker     (127)      628 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/PULL_REQUEST_TEMPLATE.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.050188 great_tables-0.6.0/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)     2095 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/scripts/no_pandas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/scripts/save_browser_table.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.050188 great_tables-0.6.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/workflows/ci-docs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3210 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/workflows/ci-tests.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-05-16 20:30:42.000000 great_tables-0.6.0/.github/workflows/code-checks.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1386 2024-05-16 20:30:42.000000 great_tables-0.6.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-16 20:30:42.000000 great_tables-0.6.0/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.050188 great_tables-0.6.0/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-16 20:30:42.000000 great_tables-0.6.0/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-16 20:30:42.000000 great_tables-0.6.0/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (127)      161 2024-05-16 20:30:42.000000 great_tables-0.6.0/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-05-16 20:30:42.000000 great_tables-0.6.0/CHANGELOG.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5243 2024-05-16 20:30:42.000000 great_tables-0.6.0/CODE_OF_CONDUCT.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)     2259 2024-05-16 20:30:42.000000 great_tables-0.6.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-05-16 20:30:42.000000 great_tables-0.6.0/HISTORY.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1081 2024-05-16 20:30:42.000000 great_tables-0.6.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 20:30:42.000000 great_tables-0.6.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-16 20:30:42.000000 great_tables-0.6.0/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-05-16 20:30:47.106188 great_tables-0.6.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6947 2024-05-16 20:30:42.000000 great_tables-0.6.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.050188 great_tables-0.6.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.042188 great_tables-0.6.0/docs/_extensions/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.042188 great_tables-0.6.0/docs/_extensions/machow/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.050188 great_tables-0.6.0/docs/_extensions/machow/interlinks/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/_extensions/machow/interlinks/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      126 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/_extensions/machow/interlinks/_extension.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     6853 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/_extensions/machow/interlinks/interlinks.lua
+-rw-r--r--   0 runner    (1001) docker     (127)     7161 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/_quarto.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.050188 great_tables-0.6.0/docs/articles/
+-rw-r--r--   0 runner    (1001) docker     (127)     5560 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/articles/intro.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.054188 great_tables-0.6.0/docs/assets/
+-rw-r--r--   0 runner    (1001) docker     (127)     2719 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/assets/GT_logo.svg
+-rw-r--r--   0 runner    (1001) docker     (127)  2325288 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/assets/datasets.png
+-rw-r--r--   0 runner    (1001) docker     (127)   136430 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/assets/gt_parts_of_a_table.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   342328 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/assets/gt_sp500_table.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    74998 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/assets/gt_workflow_diagram.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   209904 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/assets/tables_from_the_web.png
+-rw-r--r--   0 runner    (1001) docker     (127)   139817 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/assets/the_components_of_a_table.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.054188 great_tables-0.6.0/docs/blog/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.054188 great_tables-0.6.0/docs/blog/bring-your-own-df/
+-rw-r--r--   0 runner    (1001) docker     (127)     8617 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/bring-your-own-df/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.062188 great_tables-0.6.0/docs/blog/design-philosophy/
+-rw-r--r--   0 runner    (1001) docker     (127)   241842 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/a_simple_table.png
+-rw-r--r--   0 runner    (1001) docker     (127)   195558 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/cave_grids.png
+-rw-r--r--   0 runner    (1001) docker     (127)   656631 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/composition_of_a_table_in_GT.png
+-rw-r--r--   0 runner    (1001) docker     (127)   801735 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/computer_tables.png
+-rw-r--r--   0 runner    (1001) docker     (127)    22595 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)  1486510 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/nippur_cuneiform_tablet.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1629638 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png
+-rw-r--r--   0 runner    (1001) docker     (127)   458471 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/uruk_tablet_with_annotations.png
+-rw-r--r--   0 runner    (1001) docker     (127)   812542 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/design-philosophy/visicalc.png
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.066188 great_tables-0.6.0/docs/blog/introduction-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     4566 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/introduction-0.2.0/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.066188 great_tables-0.6.0/docs/blog/introduction-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     8361 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/introduction-0.3.0/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.066188 great_tables-0.6.0/docs/blog/introduction-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     7534 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/introduction-0.4.0/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10310 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/introduction_great_tables.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.066188 great_tables-0.6.0/docs/blog/polars-styling/
+-rw-r--r--   0 runner    (1001) docker     (127)     8785 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/polars-styling/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)   132380 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/polars-styling/table-preview.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.070188 great_tables-0.6.0/docs/blog/superbowl-squares/
+-rw-r--r--   0 runner    (1001) docker     (127)     2108 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/superbowl-squares/_code.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1949299 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/superbowl-squares/games.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5005 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/blog/superbowl-squares/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.070188 great_tables-0.6.0/docs/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.070188 great_tables-0.6.0/docs/examples/_data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2843 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-sales.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.070188 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/aeropress.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2524 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/cezve.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2723 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/chemex.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2457 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/cold-brew.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3332 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/drip-machine.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2165 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/espresso-machine.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2538 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/filter.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2642 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/french-press.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/grinder.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2682 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/kettle.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3900 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/moka-pot.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2962 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/noun-drip-machine-6065915.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2458 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/pour-over.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/scale.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/coffee-table-icons/total.png
+-rw-r--r--   0 runner    (1001) docker     (127)     3570 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/_data/power_cie_prepared_tbl.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    10751 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/index.qmd
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.074188 great_tables-0.6.0/docs/examples/sports-earnings/
+-rw-r--r--   0 runner    (1001) docker     (127)     3847 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/sports-earnings/basketball.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1642 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/sports-earnings/boxing.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2710 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/sports-earnings/golf.png
+-rw-r--r--   0 runner    (1001) docker     (127)    76604 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/sports-earnings/index.ipynb
+-rw-r--r--   0 runner    (1001) docker     (127)     3418 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/sports-earnings/soccer.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2675 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/sports-earnings/sports_earnings.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     3024 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/examples/sports-earnings/tennis.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.074188 great_tables-0.6.0/docs/get-started/
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/basic-column-labels.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5218 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/basic-formatting.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2307 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/basic-header.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/basic-stub.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     7558 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/basic-styling.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5713 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/colorizing-with-data.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2450 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/column-selection.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/index.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)    10497 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/nanoplots.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     1205 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/overview.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2586 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/row-selection.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     5562 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/table-theme-options.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2125 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/get-started/table-theme-premade.qmd
+-rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-05-16 20:30:42.000000 great_tables-0.6.0/docs/styles.css
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.082188 great_tables-0.6.0/great_tables/
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      440 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6252 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_boxhead.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.082188 great_tables-0.6.0/great_tables/_data_color/
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_data_color/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23399 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_data_color/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27133 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_data_color/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5966 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_data_color/palettes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_databackend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10685 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_footnotes.py
+-rw-r--r--   0 runner    (1001) docker     (127)   151727 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40689 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_formats_vals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43858 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_gt_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2906 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32945 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2641 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_locale.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14848 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    74939 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_render.py
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_row_groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5847 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_scss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1808 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_source_notes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25728 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_spanners.py
+-rw-r--r--   0 runner    (1001) docker     (127)      618 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_stub.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_stubhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12616 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6289 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_substitution.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5962 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_tab_create_modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16646 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_tbl_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_text.py
+-rw-r--r--   0 runner    (1001) docker     (127)      186 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    55726 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_utils_nanoplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27424 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/_utils_render_html.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.082188 great_tables-0.6.0/great_tables/css/
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/css/gt_colors.scss
+-rw-r--r--   0 runner    (1001) docker     (127)    10079 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/css/gt_styles_default.scss
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.090188 great_tables-0.6.0/great_tables/data/
+-rw-r--r--   0 runner    (1001) docker     (127)   412361 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/01-countrypops.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    12898 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/02-sza.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/03-gtcars.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   906055 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/04-sp500.csv
+-rw-r--r--   0 runner    (1001) docker     (127)  2848391 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/05-pizzaplace.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/06-exibble.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    81025 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/07-towny.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    20916 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/08-metro.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    21007 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/09-constants.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2104 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/10-illness.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/11-islands.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    28139 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.098188 great_tables-0.6.0/great_tables/data/metro_images/
+-rw-r--r--   0 runner    (1001) docker     (127)      475 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_10.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_11.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      839 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_12.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_13.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      657 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_14.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      670 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_3.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1968 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_3bis.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      636 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      448 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_7.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1589 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_7bis.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/metro_9.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1020 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/rer_A.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/rer_B.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/rer_C.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1013 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/rer_D.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      806 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/rer_E.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1174 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T1.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1382 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T11.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T13.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1507 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T2.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T3a.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T3b.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1533 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T5.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T6.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T7.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1948 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T8.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/tram_T9.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      807 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_H.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_J.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      860 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_K.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      727 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_L.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      948 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_N.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_P.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1160 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_R.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/metro_images/transilien_U.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2890 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/x-airquality.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     5313 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/x_currencies.csv
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/x_currency_symbols.csv
+-rw-r--r--   0 runner    (1001) docker     (127)     2543 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/x_default_locales.csv
+-rw-r--r--   0 runner    (1001) docker     (127)   255709 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/data/x_locales.csv
+-rw-r--r--   0 runner    (1001) docker     (127)    15541 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/loc.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)     1630 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/shiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/style.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/utils_render_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)      415 2024-05-16 20:30:42.000000 great_tables-0.6.0/great_tables/vals.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.106188 great_tables-0.6.0/great_tables.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10846 2024-05-16 20:30:46.000000 great_tables-0.6.0/great_tables.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8401 2024-05-16 20:30:47.000000 great_tables-0.6.0/great_tables.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 20:30:46.000000 great_tables-0.6.0/great_tables.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-05-16 20:30:46.000000 great_tables-0.6.0/great_tables.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 20:30:46.000000 great_tables-0.6.0/great_tables.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-16 20:30:42.000000 great_tables-0.6.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-05-16 20:30:42.000000 great_tables-0.6.0/pyrightconfig.json
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 20:30:47.106188 great_tables-0.6.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.102188 great_tables-0.6.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.106188 great_tables-0.6.0/tests/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)    10002 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_export.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    14024 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_formats.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_locations.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    14728 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_options.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    31704 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_repr.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     7516 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_scss.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_tbl_data.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)    10815 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/__snapshots__/test_utils_render_html.ambr
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.106188 great_tables-0.6.0/tests/data_color/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 20:30:47.106188 great_tables-0.6.0/tests/data_color/__snapshots__/
+-rw-r--r--   0 runner    (1001) docker     (127)    22008 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/data_color/__snapshots__/test_data_color.ambr
+-rw-r--r--   0 runner    (1001) docker     (127)     9178 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/data_color/test_data_color.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18147 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/data_color/test_data_color_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3705 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test__boxhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      343 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test__formats_vals.py
+-rw-r--r--   0 runner    (1001) docker     (127)      723 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test__stubhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    54571 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test__utils_nanoplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)      291 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_body.py
+-rw-r--r--   0 runner    (1001) docker     (127)      321 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_boxhead.py
+-rw-r--r--   0 runner    (1001) docker     (127)      417 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1279 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56339 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2094 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_formats_nanoplots.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1761 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_gt.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_gt_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)      280 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3789 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18349 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_repr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_scss.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_shiny.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10528 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_spanners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1620 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_styles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2200 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_substitutions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_tab_create_modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4428 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_tbl_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3159 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      548 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_utils_render_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5049 2024-05-16 20:30:42.000000 great_tables-0.6.0/tests/test_utils_render_html.py
```

### Comparing `great_tables-0.5.2/.github/CODE_OF_CONDUCT.md` & `great_tables-0.6.0/.github/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/.github/CONTRIBUTING.md` & `great_tables-0.6.0/.github/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/.github/ISSUE_TEMPLATE/bug.md` & `great_tables-0.6.0/.github/ISSUE_TEMPLATE/bug.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/.github/ISSUE_TEMPLATE/feature.md` & `great_tables-0.6.0/.github/ISSUE_TEMPLATE/feature.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/.github/ISSUE_TEMPLATE/question.md` & `great_tables-0.6.0/.github/ISSUE_TEMPLATE/question.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/.github/PULL_REQUEST_TEMPLATE.md` & `great_tables-0.6.0/.github/PULL_REQUEST_TEMPLATE.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/.github/scripts/no_pandas.py` & `great_tables-0.6.0/.github/scripts/no_pandas.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/.github/workflows/ci-docs.yaml` & `great_tables-0.6.0/.github/workflows/ci-docs.yaml`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/.github/workflows/ci-tests.yaml` & `great_tables-0.6.0/.github/workflows/ci-tests.yaml`

 * *Files 24% similar despite different names*

```diff
@@ -36,14 +36,29 @@
 
       - name: Upload coverage reports to Codecov
         uses: codecov/codecov-action@v4
         with:
           name: "py${{ matrix.python-version }}"
           token: ${{ secrets.CODECOV_TOKEN }}
 
+  test-windows:
+    runs-on: windows-latest
+    steps:
+      - uses: actions/checkout@v4
+      - name: Set up Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: "3.12"
+      - name: Install dependencies
+        run: |
+          pip install -e '.[all]'
+      - name: pytest unit tests
+        run: |
+          make test
+
   test-pandas:
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v4
       - name: Set up Python
         uses: actions/setup-python@v5
         with:
@@ -51,14 +66,44 @@
       - name: Install dependencies
         run: |
           pip install -e '.[dev-no-pandas]'
       - name: pytest unit tests
         run: |
           make test-no-pandas
 
+  browser-save-image-test:
+    name: "Test for saving table image with browser"
+    runs-on: ubuntu-latest
+    steps:
+      # browsers
+      - uses: browser-actions/setup-firefox@v1
+      - run: firefox --version
+      - uses: browser-actions/setup-chrome@v1
+      - run: chrome --version
+      - uses: browser-actions/setup-edge@v1
+
+      #
+      - uses: actions/checkout@v4
+      - name: Set up Python
+        uses: actions/setup-python@v5
+        with:
+          python-version: "3.12"
+      - name: Install dependencies
+        run: |
+          pip install -e '.[extra]'
+          pip install pandas
+      - name: save browser tables
+        run: |
+            make save-browser-table-ci
+      - uses: actions/upload-artifact@v4
+        with:
+          name: browser-save-image
+          path: _browser-tests.html
+          if-no-files-found: error
+
   release-pypi:
     name: "Release to pypi"
     runs-on: ubuntu-latest
     needs: [build, test-pandas]
     if: github.event_name == 'release'
     steps:
       - uses: actions/checkout@v2
```

### Comparing `great_tables-0.5.2/.github/workflows/code-checks.yaml` & `great_tables-0.6.0/.github/workflows/code-checks.yaml`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/.gitignore` & `great_tables-0.6.0/.gitignore`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/CODE_OF_CONDUCT.md` & `great_tables-0.6.0/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/CONTRIBUTING.md` & `great_tables-0.6.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/LICENSE` & `great_tables-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/Makefile` & `great_tables-0.6.0/Makefile`

 * *Files 22% similar despite different names*

```diff
@@ -44,7 +44,13 @@
 docs-build:
 	cd docs \
 	  && quartodoc build --verbose \
 	  && quarto render
 
 install: dist ## install the package to the active Python's site-packages
 	python3 -m pip install --force-reinstall dist/gt*.whl
+
+save-browser-table:
+	python .github/scripts/save_browser_table.py _browser-tests.html chrome firefox
+
+save-browser-table-ci:
+	python .github/scripts/save_browser_table.py _browser-tests.html chrome firefox edge
```

### Comparing `great_tables-0.5.2/PKG-INFO` & `great_tables-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great-tables
-Version: 0.5.2
+Version: 0.6.0
 Summary: Easily generate information-rich, publication-quality tables from Python.
 Author-email: Richard Iannone <rich@posit.co>, Michael Chow <michael.chow@posit.co>
 License: MIT License
         
         Copyright (c) 2022-2024 Posit Software, PBC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: great-tables Version: 0.5.2 Summary: Easily
+Metadata-Version: 2.1 Name: great-tables Version: 0.6.0 Summary: Easily
 generate information-rich, publication-quality tables from Python. Author-
 email: Richard Iannone
 posit.co>, Michael Chow
 posit.co> License: MIT License Copyright (c) 2022-2024 Posit Software, PBC
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
```

### Comparing `great_tables-0.5.2/README.md` & `great_tables-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/_extensions/machow/interlinks/interlinks.lua` & `great_tables-0.6.0/docs/_extensions/machow/interlinks/interlinks.lua`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/_quarto.yml` & `great_tables-0.6.0/docs/_quarto.yml`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/articles/intro.qmd` & `great_tables-0.6.0/docs/articles/intro.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/assets/GT_logo.svg` & `great_tables-0.6.0/docs/assets/GT_logo.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/assets/datasets.png` & `great_tables-0.6.0/docs/assets/datasets.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/assets/gt_parts_of_a_table.svg` & `great_tables-0.6.0/docs/assets/gt_parts_of_a_table.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/assets/gt_sp500_table.svg` & `great_tables-0.6.0/docs/assets/gt_sp500_table.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/assets/gt_workflow_diagram.svg` & `great_tables-0.6.0/docs/assets/gt_workflow_diagram.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/assets/tables_from_the_web.png` & `great_tables-0.6.0/docs/assets/tables_from_the_web.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/assets/the_components_of_a_table.svg` & `great_tables-0.6.0/docs/assets/the_components_of_a_table.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/bring-your-own-df/index.qmd` & `great_tables-0.6.0/docs/blog/bring-your-own-df/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/design-philosophy/a_simple_table.png` & `great_tables-0.6.0/docs/blog/design-philosophy/a_simple_table.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/design-philosophy/cave_grids.png` & `great_tables-0.6.0/docs/blog/design-philosophy/cave_grids.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/design-philosophy/composition_of_a_table_in_GT.png` & `great_tables-0.6.0/docs/blog/design-philosophy/composition_of_a_table_in_GT.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/design-philosophy/computer_tables.png` & `great_tables-0.6.0/docs/blog/design-philosophy/computer_tables.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/design-philosophy/index.qmd` & `great_tables-0.6.0/docs/blog/design-philosophy/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/design-philosophy/nippur_cuneiform_tablet.png` & `great_tables-0.6.0/docs/blog/design-philosophy/nippur_cuneiform_tablet.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png` & `great_tables-0.6.0/docs/blog/design-philosophy/snippets_from_manual_tablular_presentation.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/design-philosophy/uruk_tablet_with_annotations.png` & `great_tables-0.6.0/docs/blog/design-philosophy/uruk_tablet_with_annotations.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/design-philosophy/visicalc.png` & `great_tables-0.6.0/docs/blog/design-philosophy/visicalc.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/introduction-0.2.0/index.qmd` & `great_tables-0.6.0/docs/blog/introduction-0.2.0/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/introduction-0.3.0/index.qmd` & `great_tables-0.6.0/docs/blog/introduction-0.3.0/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/introduction-0.4.0/index.qmd` & `great_tables-0.6.0/docs/blog/introduction-0.4.0/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/introduction_great_tables.qmd` & `great_tables-0.6.0/docs/blog/introduction_great_tables.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/polars-styling/index.qmd` & `great_tables-0.6.0/docs/blog/polars-styling/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/polars-styling/table-preview.png` & `great_tables-0.6.0/docs/blog/polars-styling/table-preview.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/superbowl-squares/_code.py` & `great_tables-0.6.0/docs/blog/superbowl-squares/_code.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/superbowl-squares/games.csv` & `great_tables-0.6.0/docs/blog/superbowl-squares/games.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/blog/superbowl-squares/index.qmd` & `great_tables-0.6.0/docs/blog/superbowl-squares/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/examples/_data/power_cie_prepared_tbl.csv` & `great_tables-0.6.0/docs/examples/_data/power_cie_prepared_tbl.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/examples/index.qmd` & `great_tables-0.6.0/docs/examples/index.qmd`

 * *Files 7% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         Temp = html("Temp,<br>&deg;F")
     )
 )
 ```
 
 :::
 
-:::{.g-col-lg-6 .g-col-12}
+:::{.g-col-lg-6 .g-col-12 .shrink-example}
 
 ```{python}
 from great_tables import GT
 from great_tables.data import countrypops
 import polars as pl
 import polars.selectors as cs
 
@@ -336,10 +336,82 @@
 )
 
 gt_tbl
 ```
 
 :::
 
+
+:::{.g-col-lg-6 .g-col-12 .shrink-example}
+
+<a
+  href="https://github.com/machow/coffee-sales-data/"
+  target="_blank"
+  >View source ⬀</a>
+  &nbsp;&nbsp;&nbsp;&nbsp;<a
+  href="https://github.com/machow/coffee-sales-data/blob/main/example_notebook.ipynb"
+  target="_blank"
+  >Notebook ⬀</a>
+
+
+
+```{python}
+import polars as pl
+import polars.selectors as cs
+from great_tables import GT, loc, style
+
+coffee_sales = pl.read_json("./_data/coffee-sales.json")
+
+sel_rev = cs.starts_with("revenue")
+sel_prof = cs.starts_with("profit")
+
+# yo
+
+coffee_table = (
+    GT(coffee_sales)
+    .tab_header("Sales of Coffee Equipment")
+    .tab_spanner(label="Revenue", columns=sel_rev)
+    .tab_spanner(label="Profit", columns=sel_prof)
+    .cols_label(
+        revenue_dollars="Amount",
+        profit_dollars="Amount",
+        revenue_pct="Percent",
+        profit_pct="Percent",
+        monthly_sales="Monthly Sales",
+        icon="",
+        product="Product",
+    )
+    # formatting ----
+    .fmt_number(
+        columns=cs.ends_with("dollars"),
+        compact=True,
+        pattern="${x}",
+        n_sigfig=3,
+    )
+    .fmt_percent(columns=cs.ends_with("pct"), decimals=0)
+    # style ----
+    .tab_style(
+        style=style.fill(color="aliceblue"),
+        locations=loc.body(columns=sel_rev),
+    )
+    .tab_style(
+        style=style.fill(color="papayawhip"),
+        locations=loc.body(columns=sel_prof),
+    )
+    .tab_style(
+        style=style.text(weight="bold"),
+        locations=loc.body(rows=pl.col("product") == "Total"),
+    )
+    .fmt_nanoplot("monthly_sales", plot_type="bar")
+    .fmt_image("icon", path="_data/coffee-table-icons/")
+    .sub_missing(missing_text="")
+)
+
+coffee_table
+```
+
+:::
+
+
 :::::
 ::::::
```

### Comparing `great_tables-0.5.2/docs/examples/sports-earnings/basketball.png` & `great_tables-0.6.0/docs/examples/sports-earnings/basketball.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/examples/sports-earnings/boxing.png` & `great_tables-0.6.0/docs/examples/sports-earnings/boxing.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/examples/sports-earnings/golf.png` & `great_tables-0.6.0/docs/examples/sports-earnings/golf.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/examples/sports-earnings/index.ipynb` & `great_tables-0.6.0/docs/examples/sports-earnings/index.ipynb`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/examples/sports-earnings/soccer.png` & `great_tables-0.6.0/docs/examples/sports-earnings/soccer.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/examples/sports-earnings/sports_earnings.csv` & `great_tables-0.6.0/docs/examples/sports-earnings/sports_earnings.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/examples/sports-earnings/tennis.png` & `great_tables-0.6.0/docs/examples/sports-earnings/tennis.png`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/get-started/basic-column-labels.qmd` & `great_tables-0.6.0/docs/get-started/basic-column-labels.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/get-started/basic-formatting.qmd` & `great_tables-0.6.0/docs/get-started/basic-formatting.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/get-started/basic-header.qmd` & `great_tables-0.6.0/docs/get-started/basic-header.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/get-started/basic-stub.qmd` & `great_tables-0.6.0/docs/get-started/basic-stub.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/get-started/basic-styling.qmd` & `great_tables-0.6.0/docs/get-started/basic-styling.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/get-started/colorizing-with-data.qmd` & `great_tables-0.6.0/docs/get-started/colorizing-with-data.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/get-started/column-selection.qmd` & `great_tables-0.6.0/docs/get-started/column-selection.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/get-started/index.qmd` & `great_tables-0.6.0/docs/get-started/index.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/get-started/nanoplots.qmd` & `great_tables-0.6.0/docs/get-started/nanoplots.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/get-started/overview.qmd` & `great_tables-0.6.0/docs/get-started/overview.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/get-started/row-selection.qmd` & `great_tables-0.6.0/docs/get-started/row-selection.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/get-started/table-theme-options.qmd` & `great_tables-0.6.0/docs/get-started/table-theme-options.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/get-started/table-theme-premade.qmd` & `great_tables-0.6.0/docs/get-started/table-theme-premade.qmd`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/docs/styles.css` & `great_tables-0.6.0/docs/styles.css`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/__init__.py` & `great_tables-0.6.0/great_tables/__init__.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_boxhead.py` & `great_tables-0.6.0/great_tables/_boxhead.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_data_color/base.py` & `great_tables-0.6.0/great_tables/_data_color/base.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_data_color/constants.py` & `great_tables-0.6.0/great_tables/_data_color/constants.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_data_color/palettes.py` & `great_tables-0.6.0/great_tables/_data_color/palettes.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_databackend.py` & `great_tables-0.6.0/great_tables/_databackend.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_export.py` & `great_tables-0.6.0/great_tables/_export.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 from __future__ import annotations
 
 import tempfile
-from typing import TYPE_CHECKING, Literal
+import time
+import warnings
 
+from typing import TYPE_CHECKING, Literal
 from typing_extensions import TypeAlias
 
 from ._utils import _try_import
 
 if TYPE_CHECKING:
     # Note that as_raw_html uses methods on the GT class, not just data
     from .gt import GT
 
+    from selenium import webdriver
+
 
 def as_raw_html(
     self: GT,
     make_page: bool = False,
     all_important: bool = False,
 ) -> str:
     """
@@ -59,68 +63,60 @@
 WebDrivers: TypeAlias = Literal[
     "chrome",
     "firefox",
     "safari",
     "edge",
 ]
 
+DebugDumpOptions: TypeAlias = Literal["zoom", "width_resize", "final_resize"]
+
 
 def save(
     self: GT,
     file: str,
     selector: str = "table",
     scale: float = 1.0,
     expand: int = 5,
     web_driver: WebDrivers = "chrome",
     window_size: tuple[int, int] = (6000, 6000),
+    debug_port: None | int = None,
+    _debug_dump: DebugDumpOptions | None = None,
 ) -> None:
     """
-    Save a table as an image file or a PDF document.
+    Produce a high-resolution image file or PDF of the table.
 
-    The `save()` method makes it easy to save a table object as an image file. The function produces
-    a high-resolution image file or PDF of the table. The output file is create by first taking a
-    screenshot of the table using a headless Chrome browser (other browser options are possible if
-    Chrome isn't present). The screenshot is then cropped to only include the table element, with
-    some additional pixels added around the table (controlled by the `expand=` parameter). Finally,
-    the resulting image is saved to the specified file path in the format specified (via the file
-    extension).
+    The output file is created by taking a screenshot of the table using a headless browser.
 
     Parameters
     ----------
     file
         The name of the file to save the image to. Accepts names ending with .png, .bmp, and other
         image extensions. Also accepts the extension .pdf.
     selector
-        The HTML element selector to use to select the table. By default, this is set to "table",
-        which selects the first table element in the HTML content.
+        (NOT IMPLEMENTED) The HTML element name used to select table. Defaults to the whole table.
     scale
-        The scaling factor that will be used when generating the image. By default, this is set to a
-        value of `1.0`. Lowering this will result in a smaller image, whereas increasing it will
-        result in a much higher-resolution image. This can be considered a quality setting, yet it
-        also affects the file size. The default value of `1.0` is a good balance between file size
-        and quality.
+        The scaling factor that will be used when generating the image.  Lower values decrease
+        resolution. A scale of 2 is equivalent to doubling the width of the table in pixels. Note
+        that higher resolution results in larger file sizes.
     expand
-        The number of pixels to expand the screenshot by. By default, this is set to 5. This can be
+        (NOT IMPLEMENTED) The number of pixels to expand the screenshot by.  This can be
         increased to capture more of the surrounding area, or decreased to capture less.
     web_driver
-        The webdriver to use when taking the screenshot. By default, this is set to `"chrome"` which
-        uses Google Chrome in headless mode. If that browser isn't available on the host system,
-        there are other options available: `"firefox"` (Mozilla Firefox), `"safari"` (Apple Safari),
-        and `"edge"` (Microsoft Edge). Ensure that at least one of these browsers is installed on
-        the system and choose the appropriate option based on that.
+        The webdriver to use when taking the screenshot. By default, uses Google Chrome. Supports
+        `"firefox"` (Mozilla Firefox), `"safari"` (Apple Safari), and `"edge"` (Microsoft Edge).
+        Specified browser must be installed.
     window_size
-        The size of the window to use when taking the screenshot. This is a tuple of two integers,
-        representing the width and height of the window. By default, this is set to `(6000, 6000)`,
-        a large size that should be sufficient for most tables. If the table is larger than this
-        (and this will be obvious once inspecting the image file) you can increase the appropriate
-        values of the tuple. If the table is very small, then a reduction in these these values will
-        result in a speed gain during image capture. Please note that the window size is *not* the
-        same as the final image size. The table will be captured at the same size as it is displayed
-        in the headless browser, and the window size is used to ensure that the entire table is
-        visible in the screen capture before the cropping process occurs.
+        The size of the browser window to use when laying out the table. This shouldn't be necessary
+        to capture a table, but may affect the tables appearance.
+    debug_port
+        Port number to use for debugging. By default no debugging port is opened.
+    _debug_dump
+        Whether the saved image should be a big browser window, with key elements outlined. This is
+        helpful for debugging this function's resizing, cropping heuristics. This is an internal
+        parameter and subject to change.
 
     Returns
     -------
     None
         This function does not return anything; it simply saves the image to the specified file
         path.
 
@@ -143,101 +139,173 @@
     pip install great_tables[extra]
     ```
 
     """
 
     # Import the required packages
     _try_import(name="selenium", pip_install_line="pip install selenium")
-    _try_import(name="PIL", pip_install_line="pip install pillow")
 
     from selenium import webdriver
-    from selenium.webdriver.common.by import By
-    from PIL import Image
-    from io import BytesIO
 
-    Image.MAX_IMAGE_PIXELS = None
+    if selector != "table":
+        raise NotImplementedError("Currently, only selector='table' is supported.")
 
     # Get the file extension from the file name
     file_extension = file.split(".")[-1]
 
     # If there is no file extension, add the .png extension
     if len(file_extension) == len(file):
         file += ".png"
 
     # Get the HTML content from the displayed output
     html_content = as_raw_html(self)
 
-    # Create a temp directory to store the HTML file
-    temp_dir = tempfile.mkdtemp()
-
     # Set the webdriver and options based on the chosen browser (`web_driver=` argument)
     if web_driver == "chrome":
         wdriver = webdriver.Chrome
         wd_options = webdriver.ChromeOptions()
     elif web_driver == "safari":
         wdriver = webdriver.Safari
         wd_options = webdriver.SafariOptions()
     elif web_driver == "firefox":
         wdriver = webdriver.Firefox
         wd_options = webdriver.FirefoxOptions()
     elif web_driver == "edge":
         wdriver = webdriver.Edge
         wd_options = webdriver.EdgeOptions()
 
-    # All webdrivers except for 'Firefox' can operate in headless mode; they all accept window size
-    # options are separate width and height arguments
-    if web_driver != "firefox":
-        wd_options.add_argument(str("--headless"))
-
-    wd_options.add_argument(f"--width={window_size[0]}")
-    wd_options.add_argument(f"--height={window_size[1]}")
+    # specify headless flag ----
+    if web_driver in {"firefox", "edge"}:
+        wd_options.add_argument("--headless")
+    elif web_driver == "chrome":
+        # Operate all webdrivers in headless mode
+        wd_options.add_argument("--headless=new")
+    else:
+        # note that safari currently doesn't support headless browsing
+        pass
+
+    if debug_port:
+        if web_driver == "chrome":
+            wd_options.add_argument(f"--remote-debugging-port={debug_port}")
+        elif web_driver == "firefox":
+            # TODO: not sure how to connect to this session on firefox?
+            wd_options.add_argument(f"--start-debugger-server {debug_port}")
+        else:
+            warnings.warn("debug_port argument only supported on chrome and firefox")
+            debug_port = None
 
+    # run browser ----
     with (
-        tempfile.NamedTemporaryFile(suffix=".html", dir=temp_dir) as temp_file,
+        tempfile.TemporaryDirectory() as tmp_dir,
         wdriver(options=wd_options) as headless_browser,
     ):
 
         # Write the HTML content to the temp file
-        with open(temp_file.name, "w") as fp:
-            fp.write(html_content)
+        with open(f"{tmp_dir}/table.html", "w") as temp_file:
+            temp_file.write(html_content)
 
-        # Convert the scale value to a percentage string used by the
-        # Chrome browser for zooming
-        zoom_level = str(scale * 100) + "%"
+        # Open the HTML file in the headless browser
+        headless_browser.set_window_size(window_size[0], window_size[1])
+        headless_browser.get("file://" + temp_file.name)
 
-        # Get the scaling factor by multiplying `scale` by 2
-        scaling_factor = scale * 2
+        _save_screenshot(headless_browser, scale, file, debug=_debug_dump)
 
-        # Adjust the expand value by the scaling factor
-        expansion_amount = expand * scaling_factor
+        if debug_port:
+            input(
+                f"Currently debugging on port {debug_port}.\n\n"
+                "If you are using Chrome, enter chrome://inspect to preview the headless browser."
+                "Other browsers may have different ways to preview headless browser sessions.\n\n"
+                "Press enter to continue."
+            )
 
-        # Open the HTML file in the headless browser
-        headless_browser.get("file://" + temp_file.name)
-        headless_browser.execute_script(f"document.body.style.zoom = '{zoom_level}'")
 
-        # Get only the chosen element from the page; by default, this is the table element
-        element = headless_browser.find_element(by=By.TAG_NAME, value=selector)
+def _save_screenshot(
+    driver: webdriver.Chrome, scale, path: str, debug: DebugDumpOptions | None
+) -> None:
+    from io import BytesIO
+    from selenium.webdriver.common.by import By
+
+    # Based on: https://stackoverflow.com/a/52572919/
+    # In some headless browsers, element position and width do not always reflect
+    # css transforms like zoom.
+    #
+    # This approach works on the following assumptions:
+    #   * Zoomed table width cannot always be obtained directly, but is its clientWidth * scale
+    #   * Zoomed table height is obtained by the height of the div wrapping it
+    #   * A sleep may be necessary before the final screen capture
+    #
+    # I can't say for sure whether the final sleep is needed. Only that it seems like
+    # on CI with firefox sometimes the final screencapture is wider than necessary.
+
+    original_size = driver.get_window_size()
+
+    # set table zoom ----
+    driver.execute_script(
+        "var el = document.getElementsByTagName('table')[0]; "
+        f"el.style.zoom = '{scale}'; "
+        "el.parentNode.style.display='none'; "
+        "el.parentNode.style.display='';"
+    )
+
+    if debug == "zoom":
+        return _dump_debug_screenshot(driver, path)
+
+    # get table width and height, resizing window as we go ----
+
+    # the window can be bigger than the table, but smaller risks pushing text
+    # onto new lines. this pads width and height for a little slack.
+    # note that this is mostly to account for body, div padding, and table borders.
+    crud_factor = 100
+
+    offset_left, offset_top = driver.execute_script(
+        "var div = document.body.childNodes[0]; return [div.offsetLeft, div.offsetTop];"
+    )
+    reported_width = driver.execute_script(
+        "var el = document.getElementsByTagName('table')[0]; return el.clientWidth;"
+    )
+    required_width = (reported_width + offset_left * 2 + crud_factor) * scale
+
+    # set to our required_width first, in case it changes the height of the table
+    driver.set_window_size(required_width, original_size["height"])
+
+    if debug == "width_resize":
+        return _dump_debug_screenshot(driver, path)
+
+    # height accounts for top-padding supplied by the browser (doubled to pad top and bottom)
+    div_height = driver.execute_script(
+        "var div = document.body.childNodes[0]; return div.scrollHeight;"
+    )
+    required_height = div_height + crud_factor + offset_top * 2
+
+    # final resize window and capture image ----
+    driver.set_window_size(required_width, required_height)
+
+    if debug == "final_resize":
+        return _dump_debug_screenshot(driver, path)
+
+    el = driver.find_element(by=By.TAG_NAME, value="body")
+
+    time.sleep(0.05)
 
-        # Get the location and size of the table element; this will be used
-        # to crop the screenshot later
-        location = element.location
-        size = element.size
-
-        # Get a screenshot of the entire page as a PNG image
-        png = headless_browser.get_screenshot_as_png()
-
-    # Open the screenshot as an image with the PIL library; since the screenshot will be large
-    # (due to the large window size), we use the BytesIO class to handle the large image data
-    image = Image.open(fp=BytesIO(png))
-
-    # Crop the image to only include the table element; the scaling factor
-    # of 6 is used to account for the zoom level of 300% set earlier
-    left = (location["x"] * scaling_factor) - expansion_amount
-    top = (location["y"] * scaling_factor) - expansion_amount
-    right = ((location["x"] + size["width"]) * scaling_factor) + expansion_amount
-    bottom = ((location["y"] + size["height"]) * scaling_factor) + expansion_amount
+    if path.endswith(".png"):
+        el.screenshot(path)
+    else:
+        _try_import(name="PIL", pip_install_line="pip install pillow")
 
-    # Save the cropped image to the output path
-    image = image.crop((left, top, right, bottom))
+        from PIL import Image
 
-    # Save the image to the output path in the specified format
-    image.save(fp=file)
+        # convert to other formats (e.g. pdf, bmp) using PIL
+        with tempfile.TemporaryDirectory() as tmp_dir:
+            fname = f"{tmp_dir}/image.png"
+            el.screenshot(fname)
+
+            with open(fname, "rb") as f:
+                Image.open(fp=BytesIO(f)).save(fp=path)
+
+
+def _dump_debug_screenshot(driver, path):
+    driver.execute_script(
+        "document.body.style.border = '5px solid blue'; "
+        "document.body.childNodes[0].style.border = '5px solid orange'; "
+        "document.getElementsByTagName('table')[0].style.border = '5px solid green'; "
+    )
+    driver.save_screenshot(path)
```

### Comparing `great_tables-0.5.2/great_tables/_formats.py` & `great_tables-0.6.0/great_tables/_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -3403,15 +3403,15 @@
         import base64
 
         with open(filename, "rb") as f:
             encoded = base64.b64encode(f.read()).decode()
 
         mime_type = cls._get_mime_type(filename)
 
-        return f"data: {mime_type}; base64,{encoded}"
+        return f"data:{mime_type};base64,{encoded}"
 
     @staticmethod
     def _get_mime_type(filename: str) -> str:
         from pathlib import Path
 
         # note that we strip off the leading "."
         suffix = Path(filename).suffix[1:]
```

### Comparing `great_tables-0.5.2/great_tables/_formats_vals.py` & `great_tables-0.6.0/great_tables/_formats_vals.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_gt_data.py` & `great_tables-0.6.0/great_tables/_gt_data.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_heading.py` & `great_tables-0.6.0/great_tables/_heading.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_helpers.py` & `great_tables-0.6.0/great_tables/_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -694,15 +694,15 @@
     currency
         If the values are to be displayed as currency values, supply either: (1) a 3-letter currency
         code (e.g., `"USD"` for U.S. Dollars, `"EUR"` for the Euro currency), or (2) a common
         currency name (e.g., `"dollar"`, `"pound"`, `"yen"`, etc.).
 
     Examples
     --------
-    See [`fmt_nanoplot()`](`great_tables.GT.fmt_nanoplot`)
+    See [`fmt_nanoplot()`](`great_tables.GT.fmt_nanoplot`).
     """
 
     data_point_radius = _normalize_listable_nanoplot_options(
         nano_opt=data_point_radius, option_type=int
     )
     data_point_stroke_color = _normalize_listable_nanoplot_options(
         nano_opt=data_point_stroke_color, option_type=str
```

### Comparing `great_tables-0.5.2/great_tables/_locale.py` & `great_tables-0.6.0/great_tables/_locale.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 from importlib_resources import files
 
 DATA_MOD = files("great_tables") / "data"
 
 
 def read_csv(fname: str) -> list[dict[str, Any]]:
-    with open(fname) as f:
+    with open(fname, encoding="utf8") as f:
         return list(DictReader(f))
 
 
 class Locale:
     locale: str | None
 
     def __init__(self, locale: str | None = ""):
```

### Comparing `great_tables-0.5.2/great_tables/_locations.py` & `great_tables-0.6.0/great_tables/_locations.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_options.py` & `great_tables-0.6.0/great_tables/_options.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_render.py` & `great_tables-0.6.0/great_tables/_render.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_scss.py` & `great_tables-0.6.0/great_tables/_scss.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_source_notes.py` & `great_tables-0.6.0/great_tables/_source_notes.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_spanners.py` & `great_tables-0.6.0/great_tables/_spanners.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,50 +119,57 @@
             label=md("*Performance*"),
             columns=["hp", "hp_rpm", "trq", "trq_rpm", "mpg_c", "mpg_h"]
         )
     )
     ```
     """
 
-    crnt_spanner_ids = [span.spanner_id for span in data._spanners]
+    crnt_spanner_ids = set([span.spanner_id for span in data._spanners])
 
     if id is None:
-        id = label
+        # The label may contain HTML or Markdown, so we need to extract
+        # it from the Text object
+        if hasattr(label, "text"):
+            id = label.text
+        else:
+            id = label
 
     if isinstance(columns, (str, int)):
         columns = [columns]
+    elif columns is None:
+        columns = []
 
     if isinstance(spanners, (str, int)):
         spanners = [spanners]
+    elif spanners is None:
+        spanners = []
 
     # validations ----
     if level is not None and level < 0:
         raise ValueError(f"Level may not be negative. Received {level}.")
     if id in crnt_spanner_ids:
         raise ValueError(f"Spanner id {id} already exists.")
 
     # select columns ----
 
-    if columns is None:
-        # TODO: null_means is unimplemented
-        raise NotImplementedError("columns must be specified")
-
-    selected_column_names = resolve_cols_c(data=data, expr=columns, null_means="nothing")
+    selected_column_names = resolve_cols_c(data=data, expr=columns, null_means="nothing") or []
 
     # select spanner ids ----
     # TODO: this supports tidyselect
     # TODO: could we use something like resolve_vector_l
     if spanners is not None:
         assert set(spanners).issubset(set(crnt_spanner_ids))
         spanner_ids = spanners
     else:
         spanner_ids = []
 
+    # Check that we've selected something explicitly
     if not len(selected_column_names) and not len(spanner_ids):
-        return data
+        # TODO: null_means is unimplemented
+        raise NotImplementedError("columns/spanners must be specified")
 
     # get column names associated with selected spanners ----
     _vars = [span.vars for span in data._spanners if span.spanner_id in spanner_ids]
     spanner_column_names = list({k: True for k in itertools.chain(*_vars)})
 
     column_names = list({k: True for k in [*selected_column_names, *spanner_column_names]})
 
@@ -183,18 +190,17 @@
         vars=column_names,
         spanner_units=spanner_units,
         spanner_pattern=spanner_pattern,
         spanner_label=label,
     )
 
     spanners = data._spanners.append_entry(new_span)
-
     new_data = data._replace(_spanners=spanners)
 
-    if gather and not len(spanner_ids) and level == 0:
+    if gather and not len(spanner_ids) and level == 0 and column_names:
         return cols_move(new_data, columns=column_names, after=column_names[0])
 
     return new_data
 
 
 def cols_move(data: GTSelf, columns: SelectExpr, after: str) -> GTSelf:
     """Move one or more columns.
@@ -514,15 +520,14 @@
     # (3) `spanner_level` values have all gaps removed, being compressed
     #     down to start at 1 (e.g., 7, 5, 3, 1 -> 4, 3, 2, 1)
     _vars = [set(span.vars) & set(vars) for span in spanners]
     _lvls = sorted({span.spanner_level for span in spanners})
 
     non_empty_spans = [span for crnt_vars, span in zip(_vars, spanners) if len(crnt_vars)]
     new_levels = [_lvls.index(span.spanner_level) for span in non_empty_spans]
-
     crnt_spans = Spanners(non_empty_spans).relevel(new_levels)
 
     if not crnt_spans:
         return empty_spanner_matrix(vars=vars, omit_columns_row=omit_columns_row)
 
     spanner_height = len(_lvls)
     # TODO: span.built can be None. When does it get set?
```

### Comparing `great_tables-0.5.2/great_tables/_stub.py` & `great_tables-0.6.0/great_tables/_stub.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_stubhead.py` & `great_tables-0.6.0/great_tables/_stubhead.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_styles.py` & `great_tables-0.6.0/great_tables/_styles.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_substitution.py` & `great_tables-0.6.0/great_tables/_substitution.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_tab_create_modify.py` & `great_tables-0.6.0/great_tables/_tab_create_modify.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_tbl_data.py` & `great_tables-0.6.0/great_tables/_tbl_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -408,15 +408,15 @@
     import polars.selectors as cs
 
     list_cols = [
         name for name, dtype in zip(df.columns, df.dtypes) if issubclass(dtype.base_type(), pl.List)
     ]
 
     return df.with_columns(
-        cs.by_name(list_cols).map_elements(lambda x: str(x.to_list())),
+        cs.by_name(list_cols).map_elements(lambda x: str(x.to_list()), return_dtype=pl.String),
         cs.all().exclude(list_cols).cast(pl.Utf8),
     )
 
 
 # replace_null_frame ----
```

### Comparing `great_tables-0.5.2/great_tables/_text.py` & `great_tables-0.6.0/great_tables/_text.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_utils.py` & `great_tables-0.6.0/great_tables/_utils.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_utils_nanoplots.py` & `great_tables-0.6.0/great_tables/_utils_nanoplots.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/_utils_render_html.py` & `great_tables-0.6.0/great_tables/_utils_render_html.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,18 +177,20 @@
 
     if spanner_row_count >= 1:
         spanners, _ = spanners_print_matrix(
             spanners=data._spanners, boxhead=boxhead, include_hidden=False
         )
 
         spanner_ids, spanner_col_names = spanners_print_matrix(
-            spanners=data._spanners, boxhead=boxhead, include_hidden=False, ids=True
+            spanners=data._spanners, boxhead=boxhead, include_hidden=False, ids=False
         )
 
-        level_1_index = 0
+        # Last is column labels
+        # So take second to last
+        level_1_index = -2
 
         # A list of <th> elements that will go in the first level; this
         # includes spanner labels and column labels for solo columns (don't
         # have spanner labels above them)
         level_1_spanners = []
 
         # A list of <th> elements that will go in the second row. This is
@@ -337,42 +339,29 @@
             )
 
         else:
             # Create the `table_col_headings` HTML component
             table_col_headings = tags.tr(level_1_spanners, class_="gt_col_headings gt_spanner_row")
 
     if _get_spanners_matrix_height(data=data) > 2:
-        # TODO: functions like seq_len don't exist
-        higher_spanner_rows_idx = seq_len(nrow(spanner_ids) - 2)  # noqa
-
+        # Spanners are listed top to bottom, so we need to work bottom to top
+        # We can skip the last (column labels) and second to last (first spanner)
+        higher_spanner_rows_idx = range(0, len(spanner_ids) - 2)
         higher_spanner_rows = TagList()
 
         for i in higher_spanner_rows_idx:
-            spanner_ids_row = spanner_ids[i]
             spanners_row = spanners[i]
-            # TODO: shouldn't use np here
-            spanners_vars = list(set(spanner_ids_row[~np.isnan(spanner_ids_row)].tolist()))  # noqa
-
-            # Replace NA values in spanner_ids_row with an empty string
-            # TODO: shouldn't use np here
-            spanner_ids_row[np.isnan(spanner_ids_row)] = ""  # noqa
-
-            spanners_rle = [(k, len(list(g))) for k, g in groupby(list(spanner_ids_row))]
-
-            sig_cells = [1] + [
-                i + 1
-                for i, (k, _) in enumerate(spanners_rle[:-1])
-                if k is None or k != spanners_rle[i - 1][0]
-            ]
-
-            colspans = [
-                spanners_rle[j][1] if (j + 1) in sig_cells else 0
-                for j in range(len(spanner_ids_row))
-            ]
-
+            for k, v in spanners_row.items():
+                if v is None:
+                    spanners_row[k] = ""
+
+            spanner_ids_index = list(spanners_row.values())
+            spanners_rle = list(seq_groups(seq=list(spanner_ids_index)))
+            group_spans = [[x[1]] + [0] * (x[1] - 1) for x in spanners_rle]
+            colspans = list(chain(*group_spans))
             level_i_spanners = []
 
             for colspan, span_label in zip(colspans, spanners_row.values()):
                 if colspan > 0:
                     # Skip styles for now
                     # styles_spanners = styles_tbl[
                     #     (styles_tbl["locname"] == "columns_groups") &
@@ -382,46 +371,59 @@
                     # spanner_style = (
                     #     styles_spanners["html_style"].values[0]
                     #     if len(styles_spanners) > 0
                     #     else None
                     # )
                     spanner_style = None
 
+                    if span_label:
+                        span = tags.span(
+                            HTML(_process_text(span_label)),
+                            class_="gt_column_spanner",
+                        )
+                    else:
+                        span = tags.span(HTML("&nbsp;"))
+
                     level_i_spanners.append(
                         tags.th(
-                            TagList(
-                                tags.span(HTML(span_label)),
-                                tags.span(HTML("&nbsp;"), class_="gt_column_spanner_inner"),
-                            ),
-                            class_="gt_center gt_columns_top_border gt_column_spanner_outer",
+                            span,
+                            class_="gt_center gt_columns_bottom_border gt_columns_top_border gt_column_spanner_outer",
                             rowspan=1,
-                            colspan=colspans[j],
+                            colspan=colspan,
                             style=spanner_style,
-                            scope="colgroup" if colspans[j] > 1 else "col",
+                            scope="colgroup" if colspan > 1 else "col",
                         )
                     )
 
-            if len(stub_layout) > 0 and i == 1:
-                level_i_spanners = tags.th(
-                    TagList(level_i_spanners),
-                    rowspan=max(list(higher_spanner_rows_idx)),
-                    colspan=len(stub_layout),
-                    scope="colgroup" if len(stub_layout) > 1 else "col",
+            if len(stub_layout) > 0:
+                level_i_spanners.insert(
+                    0,
+                    tags.th(
+                        tags.span(HTML("&nbsp")),
+                        class_=f"gt_col_heading gt_columns_bottom_border gt_{str(stubhead_label_alignment)}",
+                        rowspan=1,
+                        colspan=len(stub_layout),
+                        scope="colgroup" if len(stub_layout) > 1 else "col",
+                    ),
                 )
 
             higher_spanner_rows = TagList(
                 higher_spanner_rows,
-                TagList(tags.tr(level_i_spanners, class_="gt_col_headings gt_spanner_row")),
+                TagList(
+                    tags.tr(
+                        level_i_spanners,
+                        class_="gt_col_headings gt_spanner_row",
+                    )
+                ),
             )
 
         table_col_headings = TagList(
             higher_spanner_rows,
             table_col_headings,
         )
-
     return str(table_col_headings)
 
 
 def create_body_component_h(data: GTData) -> str:
     # for now, just coerce everything in the original data to a string
     # so we can fill in the body data with it
     _str_orig_data = cast_frame_to_string(data._tbl_data)
```

### Comparing `great_tables-0.5.2/great_tables/css/gt_colors.scss` & `great_tables-0.6.0/great_tables/css/gt_colors.scss`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/css/gt_styles_default.scss` & `great_tables-0.6.0/great_tables/css/gt_styles_default.scss`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/01-countrypops.csv` & `great_tables-0.6.0/great_tables/data/01-countrypops.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/02-sza.csv` & `great_tables-0.6.0/great_tables/data/02-sza.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/03-gtcars.csv` & `great_tables-0.6.0/great_tables/data/03-gtcars.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/04-sp500.csv` & `great_tables-0.6.0/great_tables/data/04-sp500.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/05-pizzaplace.csv` & `great_tables-0.6.0/great_tables/data/05-pizzaplace.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/06-exibble.csv` & `great_tables-0.6.0/great_tables/data/06-exibble.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/07-towny.csv` & `great_tables-0.6.0/great_tables/data/07-towny.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/08-metro.csv` & `great_tables-0.6.0/great_tables/data/08-metro.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/09-constants.csv` & `great_tables-0.6.0/great_tables/data/09-constants.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/10-illness.csv` & `great_tables-0.6.0/great_tables/data/10-illness.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/11-islands.csv` & `great_tables-0.6.0/great_tables/data/11-islands.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/__init__.py` & `great_tables-0.6.0/great_tables/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -199,18 +199,18 @@
 43.0 degrees.
 
 Details
 -------
 This is a dataset with 816 rows and 4 columns.
 
 - `latitude`: The latitude in decimal degrees for the observations.
-- `month: The measurement month. All calculations where conducted for the first day of each month.
-- `tst: The true solar time at the given `latitude` and date (first of `month`) for which the solar
+- `month`: The measurement month. All calculations where conducted for the first day of each month.
+- `tst`: The true solar time at the given `latitude` and date (first of `month`) for which the solar
 zenith angle is calculated.
-- `sza: The solar zenith angle in degrees, where `NA`s indicate that sunrise hadn't yet occurred by
+- `sza`: The solar zenith angle in degrees, where `NA`s indicate that sunrise hadn't yet occurred by
 the `tst` value.
 
 Source
 ------
 Calculated Actinic Fluxes (290 - 700 nm) for Air Pollution Photochemistry Applications (Peterson,
 1976), available at: <https://nepis.epa.gov/Exe/ZyPURL.cgi?Dockey=9100JA26.txt>.
 """
@@ -230,15 +230,15 @@
 that, with these cars, comfort is emphasized over all-out performance. Nevertheless, the driving
 experience should also mean motoring at speed, doing so in style and safety.
 
 Details
 -------
 This is a dataset with 47 rows and 15 columns.
 
-- `mfr`: `The name of the car manufacturer.
+- `mfr`: The name of the car manufacturer.
 - `model`: The car's model name.
 - `year`: The car's model year.
 - `trim`: A short description of the car model's trim.
 - `bdy_style`: An identifier of the car's body style, which is either `"coupe"`, `"convertible"`,
 `"sedan"`, or `"hatchback"`.
 - `hp`, `hp_rpm`: The car's horsepower and the associated RPM level.
 - `trq`, `trq_rpm`: The car's torque and the associated RPM level.
@@ -261,19 +261,19 @@
 end of 2015. The index includes 500 leading companies and captures about 80 percent coverage of
 available market capitalization.
 
 Details
 -------
 This is a dataset with 16,607 rows and 7 columns.
 
-`date`: The date expressed as `Date` values.
-`open`, `high`, `low`, `close`: The day's opening, high, low, and closing prices in USD. The `close`
-price is adjusted for splits.
-`volume`: The number of trades for the given `date`.
-`adj_close`: The close price adjusted for both dividends and splits.
+- `date`: The date expressed as `Date` values.
+- `open`, `high`, `low`, `close`: The day's opening, high, low, and closing prices in USD. The
+`close` price is adjusted for splits.
+- `volume`: The number of trades for the given `date`.
+- `adj_close`: The close price adjusted for both dividends and splits.
 """
 
 
 pizzaplace: pd.DataFrame = pd.read_csv(_pizzaplace_fname, dtype=_pizzaplace_dtype)  # type: ignore
 pizzaplace.__doc__ = """
 A year of pizza sales from a pizza place.
 
@@ -359,15 +359,15 @@
 Peppers, Garlic, Pesto Sauce)
 
 Details
 -------
 This is a dataset with 49,574 rows and 7 columns.
 
 - `id`: The ID for the order, which consists of one or more pizzas at a given `date` and `time`.
-`date`: A character representation of the `order` date, expressed in the ISO 8601 date format
+- `date`: A character representation of the `order` date, expressed in the ISO 8601 date format
 ('YYYY-MM-DD').
 - `time`: A character representation of the `order` time, expressed as a 24-hour time the ISO 8601
 extended time format ('hh:mm:ss').
 - `name`: The short name for the pizza.
 - `size`: The size of the pizza, which can either be `"S"`, `"M"`, `"L"`, `"XL"` (rare!), or `"XXL"`
 (even rarer!); most pizzas are available in the `"S"`, `"M"`, and `"L"` sizes but exceptions apply.
 - `type`: The category or type of pizza, which can either be `"classic"`, `"chicken"`, `"supreme"`,
```

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/metro_10.svg` & `great_tables-0.6.0/great_tables/data/metro_images/metro_10.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/metro_11.svg` & `great_tables-0.6.0/great_tables/data/metro_images/metro_11.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/metro_12.svg` & `great_tables-0.6.0/great_tables/data/metro_images/metro_12.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/metro_13.svg` & `great_tables-0.6.0/great_tables/data/metro_images/metro_13.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/metro_14.svg` & `great_tables-0.6.0/great_tables/data/metro_images/metro_14.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/metro_2.svg` & `great_tables-0.6.0/great_tables/data/metro_images/metro_2.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/metro_3.svg` & `great_tables-0.6.0/great_tables/data/metro_images/metro_3.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/metro_3bis.svg` & `great_tables-0.6.0/great_tables/data/metro_images/metro_3bis.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/metro_5.svg` & `great_tables-0.6.0/great_tables/data/metro_images/metro_5.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/metro_6.svg` & `great_tables-0.6.0/great_tables/data/metro_images/metro_6.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/metro_7bis.svg` & `great_tables-0.6.0/great_tables/data/metro_images/metro_7bis.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/metro_8.svg` & `great_tables-0.6.0/great_tables/data/metro_images/metro_8.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/metro_9.svg` & `great_tables-0.6.0/great_tables/data/metro_images/metro_9.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/rer_A.svg` & `great_tables-0.6.0/great_tables/data/metro_images/rer_A.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/rer_B.svg` & `great_tables-0.6.0/great_tables/data/metro_images/rer_B.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/rer_C.svg` & `great_tables-0.6.0/great_tables/data/metro_images/rer_C.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/rer_D.svg` & `great_tables-0.6.0/great_tables/data/metro_images/rer_D.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/rer_E.svg` & `great_tables-0.6.0/great_tables/data/metro_images/rer_E.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/tram_T1.svg` & `great_tables-0.6.0/great_tables/data/metro_images/tram_T1.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/tram_T11.svg` & `great_tables-0.6.0/great_tables/data/metro_images/tram_T11.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/tram_T13.svg` & `great_tables-0.6.0/great_tables/data/metro_images/tram_T13.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/tram_T2.svg` & `great_tables-0.6.0/great_tables/data/metro_images/tram_T2.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/tram_T3a.svg` & `great_tables-0.6.0/great_tables/data/metro_images/tram_T3a.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/tram_T3b.svg` & `great_tables-0.6.0/great_tables/data/metro_images/tram_T3b.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/tram_T4.svg` & `great_tables-0.6.0/great_tables/data/metro_images/tram_T4.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/tram_T5.svg` & `great_tables-0.6.0/great_tables/data/metro_images/tram_T5.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/tram_T6.svg` & `great_tables-0.6.0/great_tables/data/metro_images/tram_T6.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/tram_T7.svg` & `great_tables-0.6.0/great_tables/data/metro_images/tram_T7.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/tram_T8.svg` & `great_tables-0.6.0/great_tables/data/metro_images/tram_T8.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/tram_T9.svg` & `great_tables-0.6.0/great_tables/data/metro_images/tram_T9.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/transilien_H.svg` & `great_tables-0.6.0/great_tables/data/metro_images/transilien_H.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/transilien_J.svg` & `great_tables-0.6.0/great_tables/data/metro_images/transilien_J.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/transilien_K.svg` & `great_tables-0.6.0/great_tables/data/metro_images/transilien_K.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/transilien_L.svg` & `great_tables-0.6.0/great_tables/data/metro_images/transilien_L.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/transilien_N.svg` & `great_tables-0.6.0/great_tables/data/metro_images/transilien_N.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/transilien_P.svg` & `great_tables-0.6.0/great_tables/data/metro_images/transilien_P.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/transilien_R.svg` & `great_tables-0.6.0/great_tables/data/metro_images/transilien_R.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/metro_images/transilien_U.svg` & `great_tables-0.6.0/great_tables/data/metro_images/transilien_U.svg`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/x-airquality.csv` & `great_tables-0.6.0/great_tables/data/x-airquality.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/x_currencies.csv` & `great_tables-0.6.0/great_tables/data/x_currencies.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/x_default_locales.csv` & `great_tables-0.6.0/great_tables/data/x_default_locales.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/data/x_locales.csv` & `great_tables-0.6.0/great_tables/data/x_locales.csv`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/gt.py` & `great_tables-0.6.0/great_tables/gt.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/shiny.py` & `great_tables-0.6.0/great_tables/shiny.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables/utils_render_common.py` & `great_tables-0.6.0/great_tables/utils_render_common.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/great_tables.egg-info/PKG-INFO` & `great_tables-0.6.0/great_tables.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: great-tables
-Version: 0.5.2
+Version: 0.6.0
 Summary: Easily generate information-rich, publication-quality tables from Python.
 Author-email: Richard Iannone <rich@posit.co>, Michael Chow <michael.chow@posit.co>
 License: MIT License
         
         Copyright (c) 2022-2024 Posit Software, PBC
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: great-tables Version: 0.5.2 Summary: Easily
+Metadata-Version: 2.1 Name: great-tables Version: 0.6.0 Summary: Easily
 generate information-rich, publication-quality tables from Python. Author-
 email: Richard Iannone
 posit.co>, Michael Chow
 posit.co> License: MIT License Copyright (c) 2022-2024 Posit Software, PBC
 Permission is hereby granted, free of charge, to any person obtaining a copy of
 this software and associated documentation files (the "Software"), to deal in
 the Software without restriction, including without limitation the rights to
```

### Comparing `great_tables-0.5.2/great_tables.egg-info/SOURCES.txt` & `great_tables-0.6.0/great_tables.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 .github/CODE_OF_CONDUCT.md
 .github/CONTRIBUTING.md
 .github/PULL_REQUEST_TEMPLATE.md
 .github/ISSUE_TEMPLATE/bug.md
 .github/ISSUE_TEMPLATE/feature.md
 .github/ISSUE_TEMPLATE/question.md
 .github/scripts/no_pandas.py
+.github/scripts/save_browser_table.py
 .github/workflows/ci-docs.yaml
 .github/workflows/ci-tests.yaml
 .github/workflows/code-checks.yaml
 .vscode/launch.json
 .vscode/settings.json
 docs/.gitignore
 docs/_quarto.yml
@@ -54,15 +55,31 @@
 docs/blog/introduction-0.4.0/index.qmd
 docs/blog/polars-styling/index.qmd
 docs/blog/polars-styling/table-preview.png
 docs/blog/superbowl-squares/_code.py
 docs/blog/superbowl-squares/games.csv
 docs/blog/superbowl-squares/index.qmd
 docs/examples/index.qmd
+docs/examples/_data/coffee-sales.json
 docs/examples/_data/power_cie_prepared_tbl.csv
+docs/examples/_data/coffee-table-icons/aeropress.png
+docs/examples/_data/coffee-table-icons/cezve.png
+docs/examples/_data/coffee-table-icons/chemex.png
+docs/examples/_data/coffee-table-icons/cold-brew.png
+docs/examples/_data/coffee-table-icons/drip-machine.png
+docs/examples/_data/coffee-table-icons/espresso-machine.png
+docs/examples/_data/coffee-table-icons/filter.png
+docs/examples/_data/coffee-table-icons/french-press.png
+docs/examples/_data/coffee-table-icons/grinder.png
+docs/examples/_data/coffee-table-icons/kettle.png
+docs/examples/_data/coffee-table-icons/moka-pot.png
+docs/examples/_data/coffee-table-icons/noun-drip-machine-6065915.png
+docs/examples/_data/coffee-table-icons/pour-over.png
+docs/examples/_data/coffee-table-icons/scale.png
+docs/examples/_data/coffee-table-icons/total.png
 docs/examples/sports-earnings/basketball.png
 docs/examples/sports-earnings/boxing.png
 docs/examples/sports-earnings/golf.png
 docs/examples/sports-earnings/index.ipynb
 docs/examples/sports-earnings/soccer.png
 docs/examples/sports-earnings/sports_earnings.csv
 docs/examples/sports-earnings/tennis.png
```

### Comparing `great_tables-0.5.2/pyproject.toml` & `great_tables-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/__snapshots__/test_export.ambr` & `great_tables-0.6.0/tests/__snapshots__/test_export.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/__snapshots__/test_formats.ambr` & `great_tables-0.6.0/tests/__snapshots__/test_formats.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/__snapshots__/test_options.ambr` & `great_tables-0.6.0/tests/__snapshots__/test_options.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/__snapshots__/test_repr.ambr` & `great_tables-0.6.0/tests/__snapshots__/test_repr.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/__snapshots__/test_scss.ambr` & `great_tables-0.6.0/tests/__snapshots__/test_scss.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/data_color/__snapshots__/test_data_color.ambr` & `great_tables-0.6.0/tests/data_color/__snapshots__/test_data_color.ambr`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/data_color/test_data_color.py` & `great_tables-0.6.0/tests/data_color/test_data_color.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/data_color/test_data_color_utils.py` & `great_tables-0.6.0/tests/data_color/test_data_color_utils.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test__boxhead.py` & `great_tables-0.6.0/tests/test__boxhead.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test__stubhead.py` & `great_tables-0.6.0/tests/test__stubhead.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test__utils_nanoplots.py` & `great_tables-0.6.0/tests/test__utils_nanoplots.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test_export.py` & `great_tables-0.6.0/tests/test_export.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import sys
 import time
 from pathlib import Path
 
 import pytest
 from great_tables import GT, exibble, md
 
 
@@ -26,14 +27,15 @@
     return gt_tbl
 
 
 def test_html_string_generated(gt_tbl: GT, snapshot: str):
     assert snapshot == gt_tbl.as_raw_html()
 
 
+@pytest.mark.skipif(sys.platform == "win32", reason="chrome might not be installed.")
 @pytest.mark.extra
 def test_save_image_file(gt_tbl: GT):
 
     gt_tbl.save(file="test_image.png")
 
     # Wait for the file to be created before checking; wait up to
     # 5 seconds for the async save to complete
```

### Comparing `great_tables-0.5.2/tests/test_formats.py` & `great_tables-0.6.0/tests/test_formats.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import re
 from typing import Any, Union
 
 import pandas as pd
 import polars as pl
 import pytest
+import sys
 from great_tables import GT, _locale
 from great_tables._data_color.base import _html_color
 from great_tables._formats import (
     FmtImage,
     _expand_exponential_to_full_string,
     _format_number_n_sigfig,
     _format_number_fixed_decimals,
@@ -34,14 +35,21 @@
 def assert_repr_html(snapshot, gt):
     body = gt._repr_html_()
     body = re.sub(r"^.*?<table (.*?)</table>.*$", r"\1", body, flags=re.DOTALL)
 
     assert snapshot == body
 
 
+def strip_windows_drive(x):
+    # this is a hacky approach to ensuring fmt_image path tests succeed
+    # on our windows build. On linux root is just "/". On windows its a
+    # drive name. Assumes our windows runner uses D:\
+    return x.replace('src="D:\\', 'src="/')
+
+
 def test_format_fns():
     df = pd.DataFrame({"x": [1, 2]})
     gt = GT(df)
     new_gt = fmt(gt, fns=lambda x: str(x + 1), columns=["x"])
 
     formats_fn = new_gt._formats[0]
 
@@ -1404,15 +1412,15 @@
 
 
 def test_fmt_image_single():
     formatter = FmtImage(sep=" ", file_pattern="{}.svg", encode=False)
     res = formatter.to_html("/a")
     dst = formatter.SPAN_TEMPLATE.format('<img src="/a.svg" style="vertical-align: middle;">')
 
-    assert res == dst
+    assert strip_windows_drive(res) == dst
 
 
 def test_fmt_image_missing():
     formatter = FmtImage()
     assert formatter.to_html(None) is None
 
     formatter_pd = FmtImage(pd.DataFrame())
@@ -1424,64 +1432,65 @@
     res = formatter.to_html("/a,/b")
     dst = formatter.SPAN_TEMPLATE.format(
         '<img src="/a.svg" style="vertical-align: middle;">'
         "---"
         '<img src="/b.svg" style="vertical-align: middle;">'
     )
 
-    assert res == dst
+    assert strip_windows_drive(res) == dst
 
 
 def test_fmt_image_encode(tmpdir):
     from base64 import b64encode
     from pathlib import Path
 
     content = "abc"
     p_svg = Path(tmpdir) / "some.svg"
     p_svg.write_text(content)
 
     formatter = FmtImage(sep=" ", file_pattern="{}.svg", encode=True)
     res = formatter.to_html(f"{tmpdir}/some")
 
     b64_content = b64encode(content.encode()).decode()
-    img_src = f"data: image/svg+xml; base64,{b64_content}"
+    img_src = f"data:image/svg+xml;base64,{b64_content}"
     dst = formatter.SPAN_TEMPLATE.format(f'<img src="{img_src}" style="vertical-align: middle;">')
 
-    assert res == dst
+    assert strip_windows_drive(res) == dst
 
 
 def test_fmt_image_width_height_str():
     formatter = FmtImage(encode=False, width="20px", height="30px")
     res = formatter.to_html("/a")
     dst_img = '<img src="/a" style="height: 30px;width: 20px;vertical-align: middle;">'
     dst = formatter.SPAN_TEMPLATE.format(dst_img)
 
-    assert res == dst
+    assert strip_windows_drive(res) == dst
 
 
 def test_fmt_image_height_int():
     formatter = FmtImage(encode=False, height=30)
     res = formatter.to_html("/a")
     dst_img = '<img src="/a" style="height: 30px;vertical-align: middle;">'
     dst = formatter.SPAN_TEMPLATE.format(dst_img)
 
-    assert res == dst
+    assert strip_windows_drive(res) == dst
 
 
 def test_fmt_image_width_int():
     formatter = FmtImage(encode=False, width=20)
 
     with pytest.raises(NotImplementedError):
         formatter.to_html("/a")
 
 
+@pytest.mark.skipif(sys.platform == "win32", reason="uses linux specific paths")
 def test_fmt_image_path():
     formatter = FmtImage(encode=False, path="/a/b")
     res = formatter.to_html("c")
-    assert 'src="/a/b/c"' in res
+    assert 'src="/a/b/c"' in strip_windows_drive(res)
 
 
 # ------------------------------------------------------------------------------
 # Test `fmt_nanoplot()`
 # ------------------------------------------------------------------------------
```

### Comparing `great_tables-0.5.2/tests/test_formats_nanoplots.py` & `great_tables-0.6.0/tests/test_formats_nanoplots.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test_gt.py` & `great_tables-0.6.0/tests/test_gt.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test_gt_data.py` & `great_tables-0.6.0/tests/test_gt_data.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test_helpers.py` & `great_tables-0.6.0/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test_locations.py` & `great_tables-0.6.0/tests/test_locations.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test_options.py` & `great_tables-0.6.0/tests/test_options.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test_repr.py` & `great_tables-0.6.0/tests/test_repr.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test_scss.py` & `great_tables-0.6.0/tests/test_scss.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test_spanners.py` & `great_tables-0.6.0/tests/test_spanners.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import pandas as pd
 import polars as pl
 import polars.selectors as cs
 import pytest
-from great_tables import GT
+from great_tables import GT, exibble
 from great_tables._gt_data import Boxhead, ColInfo, ColInfoTypeEnum, SpannerInfo, Spanners
 from great_tables._spanners import (
     cols_hide,
     cols_move,
     cols_move_to_end,
     cols_move_to_start,
     empty_spanner_matrix,
@@ -140,14 +140,37 @@
         "b_spanner", columns=["b"]
     )
 
     assert len(new_gt._spanners) == 2
     assert new_gt._spanners[1] == dst_span
 
 
+def test_multiple_spanners_above_one():
+    from great_tables import GT, exibble
+
+    gt = (
+        GT(exibble, rowname_col="row", groupname_col="group")
+        .tab_spanner("A", ["num", "char", "fctr"])
+        .tab_spanner("B", ["fctr"])
+        .tab_spanner("C", ["num", "char"])
+        .tab_spanner("D", ["fctr", "date", "time"])
+        .tab_spanner("E", spanners=["B", "C"])
+    )
+
+    # Assert that the spanners have been added in the correct
+    # format and in the correct levels
+
+    assert len(gt._spanners) == 5
+    assert gt._spanners[0] == SpannerInfo("A", 0, "A", vars=["num", "char", "fctr"])
+    assert gt._spanners[1] == SpannerInfo("B", 1, "B", vars=["fctr"])
+    assert gt._spanners[2] == SpannerInfo("C", 1, "C", vars=["num", "char"])
+    assert gt._spanners[3] == SpannerInfo("D", 2, "D", vars=["fctr", "date", "time"])
+    assert gt._spanners[4] == SpannerInfo("E", 3, "E", vars=["fctr", "num", "char"])
+
+
 def test_tab_spanners_with_gather():
     df = pd.DataFrame({"a": [1, 2], "b": [3, 4], "c": [5, 6]})
     src_gt = GT(df)
 
     new_gt = tab_spanner(src_gt, "a_spanner", columns=["a", "c"], gather=True)
 
     assert len(new_gt._spanners) == 1
```

### Comparing `great_tables-0.5.2/tests/test_styles.py` & `great_tables-0.6.0/tests/test_styles.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test_substitutions.py` & `great_tables-0.6.0/tests/test_substitutions.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test_tab_create_modify.py` & `great_tables-0.6.0/tests/test_tab_create_modify.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test_tbl_data.py` & `great_tables-0.6.0/tests/test_tbl_data.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test_utils.py` & `great_tables-0.6.0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `great_tables-0.5.2/tests/test_utils_render_common.py` & `great_tables-0.6.0/tests/test_utils_render_common.py`

 * *Files identical despite different names*

