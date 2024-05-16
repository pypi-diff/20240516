# Comparing `tmp/collate_sqllineage-1.3.2.tar.gz` & `tmp/collate_sqllineage-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "collate_sqllineage-1.3.2.tar", last modified: Tue Apr 16 13:57:11 2024, max compression
+gzip compressed data, was "collate_sqllineage-1.4.0.tar", last modified: Thu May 16 07:17:51 2024, max compression
```

## Comparing `collate_sqllineage-1.3.2.tar` & `collate_sqllineage-1.4.0.tar`

### file list

```diff
@@ -1,245 +1,245 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.237843 collate_sqllineage-1.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-16 13:57:11.237843 collate_sqllineage-1.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6611 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.173843 collate_sqllineage-1.3.2/collate_sqllineage/
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.177843 collate_sqllineage-1.3.2/collate_sqllineage/build/
--rw-r--r--   0 runner    (1001) docker     (127)      644 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)   146541 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/editor.worker.js
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/editor.worker.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)   622794 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/editor.worker.js.map
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-16 13:56:00.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-16 13:56:00.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/logo192.png
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-16 13:56:00.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/logo512.png
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-16 13:56:00.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-16 13:56:00.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.169843 collate_sqllineage-1.3.2/collate_sqllineage/build/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.177843 collate_sqllineage-1.3.2/collate_sqllineage/build/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)    69444 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/static/css/main.c1b86fee.css
--rw-r--r--   0 runner    (1001) docker     (127)   146886 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/static/css/main.c1b86fee.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.181843 collate_sqllineage-1.3.2/collate_sqllineage/build/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)    18303 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/static/js/333.97bcedbd.chunk.js
--rw-r--r--   0 runner    (1001) docker     (127)    45386 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/static/js/333.97bcedbd.chunk.js.map
--rw-r--r--   0 runner    (1001) docker     (127)  3567481 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/static/js/main.a8b33e0c.js
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/static/js/main.a8b33e0c.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127) 12937453 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/static/js/main.a8b33e0c.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.201843 collate_sqllineage-1.3.2/collate_sqllineage/build/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    62792 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf
--rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.201843 collate_sqllineage-1.3.2/collate_sqllineage/core/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/analyzer.py
--rw-r--r--   0 runner    (1001) docker     (127)    12953 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/holders.py
--rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/models.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.201843 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/
--rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.201843 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.201843 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/
--rw-r--r--   0 runner    (1001) docker     (127)      245 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/cte_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/ddl_alter_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/ddl_drop_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5510 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/dml_insert_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/dml_merge_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/dml_select_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/lineage_holder_extractor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/noop_extractor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.205843 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     6814 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/handlers/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/handlers/swap_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/handlers/target.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/holder_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9273 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    16781 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.205843 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/analyzer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.205843 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)      349 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/handlers/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/handlers/cte.py
--rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/handlers/source.py
--rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/handlers/swap_partition.py
--rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/handlers/target.py
--rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/holder_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.169843 collate_sqllineage-1.3.2/collate_sqllineage/data/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.221843 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query01.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query02.sql
--rw-r--r--   0 runner    (1001) docker     (127)      479 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query03.sql
--rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query04.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query05.sql
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query06.sql
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query07.sql
--rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query08.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query09.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query10.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query11.sql
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query12.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query13.sql
--rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query14.sql
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query15.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query16.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query17.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query18.sql
--rw-r--r--   0 runner    (1001) docker     (127)      750 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query19.sql
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query20.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query21.sql
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query22.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query23.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query24.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query25.sql
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query26.sql
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query27.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query28.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query29.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query30.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query31.sql
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query32.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query33.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query34.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query35.sql
--rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query36.sql
--rw-r--r--   0 runner    (1001) docker     (127)      537 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query37.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query38.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query39.sql
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query40.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query41.sql
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query42.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query43.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query44.sql
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query45.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query46.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query47.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query48.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query49.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query50.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query51.sql
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query52.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query53.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query54.sql
--rw-r--r--   0 runner    (1001) docker     (127)      383 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query55.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query56.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query57.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query58.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query59.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query60.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query61.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query62.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query63.sql
--rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query64.sql
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query65.sql
--rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query66.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query67.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query68.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query69.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query70.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query71.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query72.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query73.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query74.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query75.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query76.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query77.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query78.sql
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query79.sql
--rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query80.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query81.sql
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query82.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query83.sql
--rw-r--r--   0 runner    (1001) docker     (127)      620 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query84.sql
--rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query85.sql
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query86.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query87.sql
--rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query88.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query89.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query90.sql
--rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query91.sql
--rw-r--r--   0 runner    (1001) docker     (127)      659 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query92.sql
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query93.sql
--rw-r--r--   0 runner    (1001) docker     (127)      898 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query94.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query95.sql
--rw-r--r--   0 runner    (1001) docker     (127)      399 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query96.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query97.sql
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query98.sql
--rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query99.sql
--rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/drawing.py
--rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/io.py
--rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.221843 collate_sqllineage-1.3.2/collate_sqllineage/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      410 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/utils/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      213 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/utils/entities.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/collate_sqllineage/utils/wildcard_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.233842 collate_sqllineage-1.3.2/collate_sqllineage.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-04-16 13:57:11.000000 collate_sqllineage-1.3.2/collate_sqllineage.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      240 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-04-16 13:57:09.000000 collate_sqllineage-1.3.2/collate_sqllineage.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:57:11.237843 collate_sqllineage-1.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.225843 collate_sqllineage-1.3.2/sqllineagejs/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/config-overrides.js
--rw-r--r--   0 runner    (1001) docker     (127)  1248521 2024-04-16 13:55:58.000000 collate_sqllineage-1.3.2/sqllineagejs/package-lock.json
--rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/package.json
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.225843 collate_sqllineage-1.3.2/sqllineagejs/public/
--rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/public/favicon.ico
--rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/public/index.html
--rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/public/logo192.png
--rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/public/logo512.png
--rw-r--r--   0 runner    (1001) docker     (127)      494 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/public/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/public/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.229843 collate_sqllineage-1.3.2/sqllineagejs/src/
--rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/src/App.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.229843 collate_sqllineage-1.3.2/sqllineagejs/src/api/
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/src/api/client.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.229843 collate_sqllineage-1.3.2/sqllineagejs/src/app/
--rw-r--r--   0 runner    (1001) docker     (127)      293 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/src/app/store.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.169843 collate_sqllineage-1.3.2/sqllineagejs/src/features/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.229843 collate_sqllineage-1.3.2/sqllineagejs/src/features/directory/
--rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/src/features/directory/Directory.js
--rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/src/features/directory/DirectoryTreeItem.js
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/src/features/directory/directorySlice.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.229843 collate_sqllineage-1.3.2/sqllineagejs/src/features/editor/
--rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/src/features/editor/DAG.js
--rw-r--r--   0 runner    (1001) docker     (127)      930 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/src/features/editor/DAGDesc.js
--rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/src/features/editor/Editor.js
--rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/src/features/editor/editorSlice.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.229843 collate_sqllineage-1.3.2/sqllineagejs/src/features/widget/
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/src/features/widget/LoadError.js
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/src/features/widget/Loading.js
--rw-r--r--   0 runner    (1001) docker     (127)      641 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/src/index.css
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/sqllineagejs/src/index.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:57:11.233842 collate_sqllineage-1.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_benchmark.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (127)    35744 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_columns.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_cte.py
--rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_cte_dialect_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_drawing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_exception.py
--rw-r--r--   0 runner    (1001) docker     (127)      311 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_insert.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_insert_dialect_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_others.py
--rw-r--r--   0 runner    (1001) docker     (127)     8108 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_others_dialect_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)      929 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_path_dialect_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_runner.py
--rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_select_dialect_specific.py
--rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_sqlfluff.py
--rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-04-16 13:55:22.000000 collate_sqllineage-1.3.2/tests/test_wildcard_columns.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.647693 collate_sqllineage-1.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-05-16 07:17:51.647693 collate_sqllineage-1.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6611 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.583693 collate_sqllineage-1.4.0/collate_sqllineage/
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.587693 collate_sqllineage-1.4.0/collate_sqllineage/build/
+-rw-r--r--   0 runner    (1001) docker     (127)      644 2024-05-16 07:17:49.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)   146541 2024-05-16 07:17:49.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/editor.worker.js
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-05-16 07:17:49.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/editor.worker.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)   622794 2024-05-16 07:17:49.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/editor.worker.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-16 07:16:40.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-16 07:17:49.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-05-16 07:16:40.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-16 07:16:40.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-16 07:16:40.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 07:16:40.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.579693 collate_sqllineage-1.4.0/collate_sqllineage/build/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.587693 collate_sqllineage-1.4.0/collate_sqllineage/build/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)    69444 2024-05-16 07:17:49.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/static/css/main.c1b86fee.css
+-rw-r--r--   0 runner    (1001) docker     (127)   146886 2024-05-16 07:17:49.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/static/css/main.c1b86fee.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.595693 collate_sqllineage-1.4.0/collate_sqllineage/build/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)    18303 2024-05-16 07:17:49.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/static/js/333.97bcedbd.chunk.js
+-rw-r--r--   0 runner    (1001) docker     (127)    45386 2024-05-16 07:17:49.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/static/js/333.97bcedbd.chunk.js.map
+-rw-r--r--   0 runner    (1001) docker     (127)  3567481 2024-05-16 07:17:49.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/static/js/main.a8b33e0c.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-16 07:17:49.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/static/js/main.a8b33e0c.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127) 12937453 2024-05-16 07:17:49.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/static/js/main.a8b33e0c.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.607693 collate_sqllineage-1.4.0/collate_sqllineage/build/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    62792 2024-05-16 07:17:49.000000 collate_sqllineage-1.4.0/collate_sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)     3508 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.611693 collate_sqllineage-1.4.0/collate_sqllineage/core/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/analyzer.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12953 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/holders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7148 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/models.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.611693 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/
+-rw-r--r--   0 runner    (1001) docker     (127)     3090 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.611693 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2895 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.611693 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/
+-rw-r--r--   0 runner    (1001) docker     (127)      245 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3395 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/cte_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1911 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/ddl_alter_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1344 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/ddl_drop_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5556 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/dml_insert_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5663 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/dml_merge_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2626 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/dml_select_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5133 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/lineage_holder_extractor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/noop_extractor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.615693 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1445 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6927 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/handlers/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1553 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/handlers/swap_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6071 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/handlers/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1847 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/holder_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9273 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16781 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.615693 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11204 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/analyzer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.615693 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)      349 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1578 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/handlers/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/handlers/cte.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4839 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/handlers/source.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1139 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/handlers/swap_partition.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2777 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/handlers/target.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2154 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/holder_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7483 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7527 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.579693 collate_sqllineage-1.4.0/collate_sqllineage/data/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.635693 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query01.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2556 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query02.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      479 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query03.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     6685 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query04.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5211 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query05.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query06.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query07.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     8175 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query08.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2222 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query09.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1897 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query10.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3407 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query11.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query12.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1658 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query13.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     9010 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query14.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query15.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1041 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query16.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1964 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query17.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query18.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      750 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query19.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query20.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query21.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query22.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4338 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query23.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3037 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query24.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query25.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query26.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query27.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2324 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query28.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query29.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1425 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query30.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1809 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query31.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query32.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2010 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query33.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1534 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query34.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1756 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query35.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query36.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      537 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query37.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query38.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3127 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query39.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query40.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2243 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query41.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query42.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1026 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query43.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1688 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query44.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query45.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query46.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2133 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query47.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1789 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query48.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4775 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query49.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query50.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query51.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query52.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query53.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1784 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query54.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      383 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query55.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query56.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1872 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query57.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2769 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query58.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2547 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query59.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1937 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query60.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1360 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query61.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query62.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query63.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     4418 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query64.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query65.sql
+-rw-r--r--   0 runner    (1001) docker     (127)    13194 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query66.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1210 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query67.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query68.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query69.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1220 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query70.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1399 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query71.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1330 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query72.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1295 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query73.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2092 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query74.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3089 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query75.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query76.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3844 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query77.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3067 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query78.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query79.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     3652 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query80.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1497 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query81.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query82.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query83.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      620 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query84.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     2574 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query85.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query86.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query87.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     5794 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query88.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1278 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query89.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query90.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query91.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      659 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query92.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query93.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      898 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query94.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query95.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      399 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query96.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1088 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query97.sql
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query98.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     1464 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query99.sql
+-rw-r--r--   0 runner    (1001) docker     (127)     7443 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/drawing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/io.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6188 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/runner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.635693 collate_sqllineage-1.4.0/collate_sqllineage/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      410 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/utils/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      213 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/utils/entities.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2825 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/collate_sqllineage/utils/wildcard_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.643693 collate_sqllineage-1.4.0/collate_sqllineage.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8154 2024-05-16 07:17:50.000000 collate_sqllineage-1.4.0/collate_sqllineage.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9061 2024-05-16 07:17:51.000000 collate_sqllineage-1.4.0/collate_sqllineage.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 07:17:50.000000 collate_sqllineage-1.4.0/collate_sqllineage.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-05-16 07:17:50.000000 collate_sqllineage-1.4.0/collate_sqllineage.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      240 2024-05-16 07:17:50.000000 collate_sqllineage-1.4.0/collate_sqllineage.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 07:17:50.000000 collate_sqllineage-1.4.0/collate_sqllineage.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 07:17:51.647693 collate_sqllineage-1.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3206 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.635693 collate_sqllineage-1.4.0/sqllineagejs/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/config-overrides.js
+-rw-r--r--   0 runner    (1001) docker     (127)  1248521 2024-05-16 07:16:38.000000 collate_sqllineage-1.4.0/sqllineagejs/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/package.json
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.639693 collate_sqllineage-1.4.0/sqllineagejs/public/
+-rw-r--r--   0 runner    (1001) docker     (127)     3870 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/public/favicon.ico
+-rw-r--r--   0 runner    (1001) docker     (127)     1813 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/public/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)     5347 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/public/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     9664 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/public/logo512.png
+-rw-r--r--   0 runner    (1001) docker     (127)      494 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/public/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/public/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.639693 collate_sqllineage-1.4.0/sqllineagejs/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/src/App.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.639693 collate_sqllineage-1.4.0/sqllineagejs/src/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/src/api/client.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.639693 collate_sqllineage-1.4.0/sqllineagejs/src/app/
+-rw-r--r--   0 runner    (1001) docker     (127)      293 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/src/app/store.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.579693 collate_sqllineage-1.4.0/sqllineagejs/src/features/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.639693 collate_sqllineage-1.4.0/sqllineagejs/src/features/directory/
+-rw-r--r--   0 runner    (1001) docker     (127)     1443 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/src/features/directory/Directory.js
+-rw-r--r--   0 runner    (1001) docker     (127)     3300 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/src/features/directory/DirectoryTreeItem.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/src/features/directory/directorySlice.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.639693 collate_sqllineage-1.4.0/sqllineagejs/src/features/editor/
+-rw-r--r--   0 runner    (1001) docker     (127)    12152 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/src/features/editor/DAG.js
+-rw-r--r--   0 runner    (1001) docker     (127)      930 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/src/features/editor/DAGDesc.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2762 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/src/features/editor/Editor.js
+-rw-r--r--   0 runner    (1001) docker     (127)     2357 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/src/features/editor/editorSlice.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.639693 collate_sqllineage-1.4.0/sqllineagejs/src/features/widget/
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/src/features/widget/LoadError.js
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/src/features/widget/Loading.js
+-rw-r--r--   0 runner    (1001) docker     (127)      641 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/src/index.css
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/sqllineagejs/src/index.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 07:17:51.643693 collate_sqllineage-1.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1645 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35744 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1837 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_cte.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1617 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_cte_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3083 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_drawing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1232 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)      311 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_insert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3858 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_insert_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5801 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_others.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8742 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_others_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)      929 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_path_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_runner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6822 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2090 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_select_dialect_specific.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8456 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_sqlfluff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4640 2024-05-16 07:15:59.000000 collate_sqllineage-1.4.0/tests/test_wildcard_columns.py
```

### Comparing `collate_sqllineage-1.3.2/PKG-INFO` & `collate_sqllineage-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collate-sqllineage
-Version: 1.3.2
+Version: 1.4.0
 Summary: Collate SQL Lineage for Analysis Tool powered by Python and sqlfluff based on sqllineage.
 Author: Collate Committers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `collate_sqllineage-1.3.2/README.md` & `collate_sqllineage-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/__init__.py` & `collate_sqllineage-1.4.0/collate_sqllineage/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
 
 NAME = "collate-sqllineage"
-VERSION = "1.3.2"
+VERSION = "1.4.0"
 DEFAULT_LOGGING = {
     "version": 1,
     "disable_existing_loggers": False,
     "formatters": {"default": {"format": "%(levelname)s: %(message)s"}},
     "handlers": {
         "console": {
             "level": "WARNING",
```

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/asset-manifest.json` & `collate_sqllineage-1.4.0/collate_sqllineage/build/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/editor.worker.js` & `collate_sqllineage-1.4.0/collate_sqllineage/build/editor.worker.js`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/editor.worker.js.map` & `collate_sqllineage-1.4.0/collate_sqllineage/build/editor.worker.js.map`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/favicon.ico` & `collate_sqllineage-1.4.0/collate_sqllineage/build/favicon.ico`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/index.html` & `collate_sqllineage-1.4.0/collate_sqllineage/build/index.html`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/logo192.png` & `collate_sqllineage-1.4.0/collate_sqllineage/build/logo192.png`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/logo512.png` & `collate_sqllineage-1.4.0/collate_sqllineage/build/logo512.png`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/static/css/main.c1b86fee.css` & `collate_sqllineage-1.4.0/collate_sqllineage/build/static/css/main.c1b86fee.css`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/static/css/main.c1b86fee.css.map` & `collate_sqllineage-1.4.0/collate_sqllineage/build/static/css/main.c1b86fee.css.map`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/static/js/333.97bcedbd.chunk.js` & `collate_sqllineage-1.4.0/collate_sqllineage/build/static/js/333.97bcedbd.chunk.js`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/static/js/333.97bcedbd.chunk.js.map` & `collate_sqllineage-1.4.0/collate_sqllineage/build/static/js/333.97bcedbd.chunk.js.map`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/static/js/main.a8b33e0c.js` & `collate_sqllineage-1.4.0/collate_sqllineage/build/static/js/main.a8b33e0c.js`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/static/js/main.a8b33e0c.js.LICENSE.txt` & `collate_sqllineage-1.4.0/collate_sqllineage/build/static/js/main.a8b33e0c.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/static/js/main.a8b33e0c.js.map` & `collate_sqllineage-1.4.0/collate_sqllineage/build/static/js/main.a8b33e0c.js.map`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf` & `collate_sqllineage-1.4.0/collate_sqllineage/build/static/media/codicon.4168b9c11e5075e9cfe6.ttf`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/cli.py` & `collate_sqllineage-1.4.0/collate_sqllineage/cli.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/holders.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/holders.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/models.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/models.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/__init__.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/__init__.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/analyzer.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/analyzer.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/cte_extractor.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/cte_extractor.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/ddl_alter_extractor.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/ddl_alter_extractor.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/ddl_drop_extractor.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/ddl_drop_extractor.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/dml_insert_extractor.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/dml_insert_extractor.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
     """
 
     SUPPORTED_STMT_TYPES = [
         "insert_statement",
         "create_table_statement",
         "create_table_as_statement",
         "create_view_statement",
+        "create_materialized_view_statement",
         "update_statement",
         "copy_statement",
         "insert_overwrite_directory_hive_fmt_statement",
         "copy_into_statement",
         "copy_into_table_statement",
     ]
```

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/dml_merge_extractor.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/dml_merge_extractor.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/dml_select_extractor.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/dml_select_extractor.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/lineage_holder_extractor.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/lineage_holder_extractor.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/extractors/noop_extractor.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/extractors/noop_extractor.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/handlers/base.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/handlers/base.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/handlers/source.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/handlers/source.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 )
 from collate_sqllineage.core.parser.sqlfluff.holder_utils import (
     retrieve_holder_data_from,
 )
 from collate_sqllineage.core.parser.sqlfluff.models import (
     SqlFluffColumn,
     SqlFluffSubQuery,
-    SqlFluffTable,
 )
 from collate_sqllineage.core.parser.sqlfluff.utils import (
     find_table_identifier,
     get_grandchild,
     get_inner_from_expression,
     get_multiple_identifiers,
     get_subqueries,
@@ -60,15 +59,15 @@
         Handle the segment, and update the lineage result accordingly in the holder
         :param segment: segment to be handled
         :param holder: 'SubQueryLineageHolder' to hold lineage
         """
         if self._indicate_table(segment):
             self._handle_table(segment, holder)
         elif is_union(segment):
-            self._handle_union(segment)
+            self._handle_union(segment, holder)
         if self._indicate_column(segment):
             self._handle_column(segment)
 
     def _handle_table(
         self, segment: BaseSegment, holder: SubQueryLineageHolder
     ) -> None:
         """
@@ -98,33 +97,37 @@
                     self.columns.append(SqlFluffColumn.of(sub_segment))
                 except Exception as err:
                     logger.warning(
                         f"Failed to parse column {str(sub_segment)} due to {err}"
                     )
                     logger.debug(traceback.format_exc())
 
-    def _handle_union(self, segment: BaseSegment) -> None:
+    def _handle_union(
+        self, segment: BaseSegment, holder: SubQueryLineageHolder
+    ) -> None:
         """
         Union handler method
         :param segment: segment to be handled
         """
         subqueries = get_subqueries(segment)
         if subqueries:
             for idx, sq in enumerate(subqueries):
                 if idx != 0:
                     self.union_barriers.append((len(self.columns), len(self.tables)))
                 subquery, alias = sq
                 table_identifier = find_table_identifier(subquery)
                 if table_identifier:
-                    read_sq = SqlFluffTable.of(table_identifier, alias)
                     segments = retrieve_segments(subquery)
                     for seg in segments:
                         if seg.type == "select_clause":
                             self._handle_column(seg)
-                    self.tables.append(read_sq)
+                    dataset = retrieve_holder_data_from(
+                        segments, holder, table_identifier, alias=alias
+                    )
+                    self.tables.append(dataset)
 
     def _add_dataset_from_expression_element(
         self, segment: BaseSegment, holder: SubQueryLineageHolder
     ) -> None:
         """
         Append tables and subqueries identified in the 'from_expression_element' type segment to the table and
         holder extra subqueries sets
```

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/handlers/swap_partition.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/handlers/swap_partition.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/handlers/target.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/handlers/target.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/holder_utils.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/holder_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Union
+from typing import List, Optional, Union
 
 from sqlfluff.core.parser import BaseSegment
 
 from collate_sqllineage.core.holders import SubQueryLineageHolder
 from collate_sqllineage.core.models import Path, SubQuery, Table
 from collate_sqllineage.core.parser.sqlfluff.models import (
     SqlFluffSubQuery,
@@ -12,33 +12,34 @@
 from collate_sqllineage.utils.helpers import escape_identifier_name
 
 
 def retrieve_holder_data_from(
     segments: List[BaseSegment],
     holder: SubQueryLineageHolder,
     table_identifier: BaseSegment,
+    alias: Optional[str] = None,
 ) -> Union[Path, SubQuery, Table]:
     """
     Build a 'SqlFluffSubquery' or 'SqlFluffTable' for a given list of segments and a table identifier segment.
     It will use the list of segments to find an alias and the holder CTE set of 'SqlFluffSubQuery'.
     :param segments: list of segments to search for an alias
     :param holder: 'SqlFluffSubQueryLineageHolder' to use the CTE set of 'SqlFluffSubQuery'
     :param table_identifier: a table identifier segment
     :return: 'Path' or 'SqlFluffSubQuery' or 'SqlFluffTable' object
     """
     data = None
-    alias = get_table_alias(segments)
+    alias_ = alias or get_table_alias(segments)
     if "." not in table_identifier.raw:
         cte_dict = {s.alias: s for s in holder.cte}
         cte = cte_dict.get(table_identifier.raw)
         if cte is not None:
             # could reference CTE with or without alias
             data = SqlFluffSubQuery.of(
                 cte.query,
-                alias or table_identifier.raw,
+                alias_ or table_identifier.raw,
             )
     if data is None:
         if table_identifier.type == "file_reference":
             return Path(escape_identifier_name(table_identifier.segments[-1].raw))
         else:
-            return SqlFluffTable.of(table_identifier, alias=alias)
+            return SqlFluffTable.of(table_identifier, alias=alias_)
     return data
```

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/models.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/models.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlfluff/utils.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlfluff/utils.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/__init__.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/__init__.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/analyzer.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/analyzer.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/handlers/base.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/handlers/base.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/handlers/cte.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/handlers/cte.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/handlers/source.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/handlers/source.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/handlers/swap_partition.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/handlers/swap_partition.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/handlers/target.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/handlers/target.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/holder_utils.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/holder_utils.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/models.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/models.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/core/parser/sqlparse/utils.py` & `collate_sqllineage-1.4.0/collate_sqllineage/core/parser/sqlparse/utils.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query01.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query01.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query02.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query02.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query04.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query04.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query05.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query05.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query06.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query06.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query07.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query07.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query08.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query08.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query09.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query09.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query10.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query10.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query11.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query11.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query12.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query12.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query13.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query13.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query14.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query14.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query15.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query15.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query16.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query16.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query17.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query17.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query18.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query18.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query19.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query19.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query20.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query20.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query21.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query21.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query23.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query23.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query24.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query24.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query25.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query25.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query26.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query26.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query27.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query27.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query28.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query28.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query29.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query29.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query30.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query30.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query31.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query31.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query32.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query32.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query33.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query33.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query34.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query34.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query35.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query35.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query36.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query36.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query37.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query37.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query38.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query38.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query39.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query39.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query40.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query40.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query41.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query41.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query42.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query42.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query43.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query43.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query44.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query44.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query45.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query45.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query46.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query46.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query47.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query47.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query48.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query48.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query49.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query49.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query50.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query50.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query51.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query51.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query53.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query53.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query54.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query54.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query56.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query56.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query57.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query57.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query58.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query58.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query59.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query59.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query60.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query60.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query61.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query61.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query62.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query62.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query63.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query63.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query64.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query64.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query65.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query65.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query66.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query66.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query67.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query67.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query68.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query68.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query69.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query69.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query70.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query70.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query71.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query71.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query72.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query72.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query73.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query73.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query74.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query74.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query75.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query75.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query76.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query76.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query77.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query77.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query78.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query78.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query79.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query79.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query80.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query80.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query81.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query81.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query82.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query82.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query83.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query83.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query84.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query84.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query85.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query85.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query86.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query86.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query87.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query87.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query88.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query88.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query89.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query89.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query90.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query90.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query91.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query91.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query92.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query92.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query93.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query93.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query94.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query94.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query95.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query95.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query97.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query97.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query98.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query98.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/data/tpcds/query99.sql` & `collate_sqllineage-1.4.0/collate_sqllineage/data/tpcds/query99.sql`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/drawing.py` & `collate_sqllineage-1.4.0/collate_sqllineage/drawing.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/io.py` & `collate_sqllineage-1.4.0/collate_sqllineage/io.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/runner.py` & `collate_sqllineage-1.4.0/collate_sqllineage/runner.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/utils/helpers.py` & `collate_sqllineage-1.4.0/collate_sqllineage/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage/utils/wildcard_handler.py` & `collate_sqllineage-1.4.0/collate_sqllineage/utils/wildcard_handler.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage.egg-info/PKG-INFO` & `collate_sqllineage-1.4.0/collate_sqllineage.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: collate-sqllineage
-Version: 1.3.2
+Version: 1.4.0
 Summary: Collate SQL Lineage for Analysis Tool powered by Python and sqlfluff based on sqllineage.
 Author: Collate Committers
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `collate_sqllineage-1.3.2/collate_sqllineage.egg-info/SOURCES.txt` & `collate_sqllineage-1.4.0/collate_sqllineage.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/setup.py` & `collate_sqllineage-1.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/package-lock.json` & `collate_sqllineage-1.4.0/sqllineagejs/package-lock.json`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/package.json` & `collate_sqllineage-1.4.0/sqllineagejs/package.json`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/public/favicon.ico` & `collate_sqllineage-1.4.0/sqllineagejs/public/favicon.ico`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/public/index.html` & `collate_sqllineage-1.4.0/sqllineagejs/public/index.html`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/public/logo192.png` & `collate_sqllineage-1.4.0/sqllineagejs/public/logo192.png`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/public/logo512.png` & `collate_sqllineage-1.4.0/sqllineagejs/public/logo512.png`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/src/App.js` & `collate_sqllineage-1.4.0/sqllineagejs/src/App.js`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/src/api/client.js` & `collate_sqllineage-1.4.0/sqllineagejs/src/api/client.js`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/src/features/directory/Directory.js` & `collate_sqllineage-1.4.0/sqllineagejs/src/features/directory/Directory.js`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/src/features/directory/DirectoryTreeItem.js` & `collate_sqllineage-1.4.0/sqllineagejs/src/features/directory/DirectoryTreeItem.js`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/src/features/directory/directorySlice.js` & `collate_sqllineage-1.4.0/sqllineagejs/src/features/directory/directorySlice.js`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/src/features/editor/DAG.js` & `collate_sqllineage-1.4.0/sqllineagejs/src/features/editor/DAG.js`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/src/features/editor/DAGDesc.js` & `collate_sqllineage-1.4.0/sqllineagejs/src/features/editor/DAGDesc.js`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/src/features/editor/Editor.js` & `collate_sqllineage-1.4.0/sqllineagejs/src/features/editor/Editor.js`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/src/features/editor/editorSlice.js` & `collate_sqllineage-1.4.0/sqllineagejs/src/features/editor/editorSlice.js`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/src/features/widget/LoadError.js` & `collate_sqllineage-1.4.0/sqllineagejs/src/features/widget/LoadError.js`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/src/features/widget/Loading.js` & `collate_sqllineage-1.4.0/sqllineagejs/src/features/widget/Loading.js`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/sqllineagejs/src/index.css` & `collate_sqllineage-1.4.0/sqllineagejs/src/index.css`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_benchmark.py` & `collate_sqllineage-1.4.0/tests/test_benchmark.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_cli.py` & `collate_sqllineage-1.4.0/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_columns.py` & `collate_sqllineage-1.4.0/tests/test_columns.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_cte.py` & `collate_sqllineage-1.4.0/tests/test_cte.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_cte_dialect_specific.py` & `collate_sqllineage-1.4.0/tests/test_cte_dialect_specific.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_drawing.py` & `collate_sqllineage-1.4.0/tests/test_drawing.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_exception.py` & `collate_sqllineage-1.4.0/tests/test_exception.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_models.py` & `collate_sqllineage-1.4.0/tests/test_models.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_others.py` & `collate_sqllineage-1.4.0/tests/test_others.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_others_dialect_specific.py` & `collate_sqllineage-1.4.0/tests/test_others_dialect_specific.py`

 * *Files 2% similar despite different names*

```diff
@@ -262,7 +262,26 @@
                 TestColumnQualifierTuple("c2", "my_table"),
                 TestColumnQualifierTuple("col2", "view_with_rls"),
             ),
         ],
         dialect=dialect,
         test_sqlparse=False,
     )
+
+
+@pytest.mark.parametrize("dialect", ["redshift"])
+def test_redshift_materialize_view(dialect: str):
+    sql = """create materialized view test_schema.sales_current2 as (
+    WITH current_or_previous AS (
+        SELECT
+            MAX(data_release_version) AS data_release_version
+        FROM metadata_schema.datamart_run
+        WHERE dag_id = 'test_id'
+    ) select eventid, listid, salesrow from test_schema.sales);
+"""
+    assert_table_lineage_equal(
+        sql,
+        {"test_schema.sales", "metadata_schema.datamart_run"},
+        {"test_schema.sales_current2"},
+        dialect=dialect,
+        test_sqlparse=False,
+    )
```

### Comparing `collate_sqllineage-1.3.2/tests/test_parser.py` & `collate_sqllineage-1.4.0/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_path_dialect_specific.py` & `collate_sqllineage-1.4.0/tests/test_path_dialect_specific.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_select.py` & `collate_sqllineage-1.4.0/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_select_dialect_specific.py` & `collate_sqllineage-1.4.0/tests/test_select_dialect_specific.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_sqlfluff.py` & `collate_sqllineage-1.4.0/tests/test_sqlfluff.py`

 * *Files identical despite different names*

### Comparing `collate_sqllineage-1.3.2/tests/test_wildcard_columns.py` & `collate_sqllineage-1.4.0/tests/test_wildcard_columns.py`

 * *Files identical despite different names*

