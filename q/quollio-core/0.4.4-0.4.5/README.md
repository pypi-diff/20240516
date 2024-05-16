# Comparing `tmp/quollio_core-0.4.4.tar.gz` & `tmp/quollio_core-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quollio_core-0.4.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quollio_core-0.4.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quollio_core-0.4.4.tar` & `quollio_core-0.4.5.tar`

### file list

```diff
@@ -1,63 +1,82 @@
--rw-r--r--   0        0        0    34520 2024-03-15 09:23:26.505416 quollio_core-0.4.4/LICENSE
--rw-r--r--   0        0        0     4770 2024-03-15 09:23:26.505416 quollio_core-0.4.4/README.md
--rw-r--r--   0        0        0     1884 2024-03-15 09:23:26.505416 quollio_core-0.4.4/pyproject.toml
--rw-r--r--   0        0        0       83 2024-03-15 09:23:26.505416 quollio_core-0.4.4/quollio_core/__init__.py
--rw-r--r--   0        0        0      571 2024-03-15 09:23:26.505416 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/README.md
--rw-r--r--   0        0        0        0 2024-03-15 09:23:26.505416 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/analyses/.gitkeep
--rw-r--r--   0        0        0      405 2024-03-15 09:23:26.505416 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/dbt_project.yml
--rw-r--r--   0        0        0        0 2024-03-15 09:23:26.505416 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/macros/.gitkeep
--rw-r--r--   0        0        0     3492 2024-03-15 09:23:26.505416 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/macros/materialization/divided_view.sql
--rw-r--r--   0        0        0     2042 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_lineage_table_level.sql
--rw-r--r--   0        0        0      236 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_lineage_table_level.yml
--rw-r--r--   0        0        0     1289 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_lineage_view_level.sql
--rw-r--r--   0        0        0      235 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_lineage_view_level.yml
--rw-r--r--   0        0        0     1049 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_sqllineage_sources.sql
--rw-r--r--   0        0        0      377 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_sqllineage_sources.yml
--rw-r--r--   0        0        0      302 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_stats_columns.sql
--rw-r--r--   0        0        0       67 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_stats_columns.yml
--rw-r--r--   0        0        0     1592 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.sql
--rw-r--r--   0        0        0      523 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.yml
--rw-r--r--   0        0        0    14646 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/sources.yml
--rw-r--r--   0        0        0      109 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/package-lock.yml
--rw-r--r--   0        0        0       61 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/packages.yml
--rw-r--r--   0        0        0      291 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/profiles/profiles_template.yml
--rw-r--r--   0        0        0        0 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/seeds/.gitkeep
--rw-r--r--   0        0        0        0 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/redshift/snapshots/.gitkeep
--rw-r--r--   0        0        0      571 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/README.md
--rw-r--r--   0        0        0        0 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/analyses/.gitkeep
--rw-r--r--   0        0        0      407 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/dbt_project.yml
--rw-r--r--   0        0        0        0 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/macros/.gitkeep
--rw-r--r--   0        0        0     2782 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/macros/materialization/divided_view.sql
--rw-r--r--   0        0        0     4721 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.sql
--rw-r--r--   0        0        0      711 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.yml
--rw-r--r--   0        0        0     5112 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_lineage_table_level.sql
--rw-r--r--   0        0        0      325 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_lineage_table_level.yml
--rw-r--r--   0        0        0     1520 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_sqllineage_sources.sql
--rw-r--r--   0        0        0      377 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_sqllineage_sources.yml
--rw-r--r--   0        0        0      302 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_stats_columns.sql
--rw-r--r--   0        0        0       67 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_stats_columns.yml
--rw-r--r--   0        0        0     1382 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.sql
--rw-r--r--   0        0        0      538 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.yml
--rw-r--r--   0        0        0    10975 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/sources.yml
--rw-r--r--   0        0        0      109 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/package-lock.yml
--rw-r--r--   0        0        0       61 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/packages.yml
--rw-r--r--   0        0        0      379 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/profiles/profiles_template.yml
--rw-r--r--   0        0        0        0 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/seeds/.gitkeep
--rw-r--r--   0        0        0        0 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/snapshots/.gitkeep
--rw-r--r--   0        0        0        0 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/helper/__init__.py
--rw-r--r--   0        0        0     1127 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/helper/core.py
--rw-r--r--   0        0        0     1074 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/helper/env_default.py
--rw-r--r--   0        0        0        0 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/profilers/__init__.py
--rw-r--r--   0        0        0     5892 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/profilers/lineage.py
--rw-r--r--   0        0        0     7862 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/profilers/redshift.py
--rw-r--r--   0        0        0     9090 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/profilers/snowflake.py
--rw-r--r--   0        0        0     5177 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/profilers/sqllineage.py
--rw-r--r--   0        0        0     4721 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/profilers/stats.py
--rw-r--r--   0        0        0    10234 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/redshift.py
--rw-r--r--   0        0        0        0 2024-03-15 09:23:26.509415 quollio_core-0.4.4/quollio_core/repository/__init__.py
--rw-r--r--   0        0        0      770 2024-03-15 09:23:26.513415 quollio_core-0.4.4/quollio_core/repository/dbt.py
--rw-r--r--   0        0        0     4702 2024-03-15 09:23:26.513415 quollio_core-0.4.4/quollio_core/repository/qdc.py
--rw-r--r--   0        0        0     2991 2024-03-15 09:23:26.513415 quollio_core-0.4.4/quollio_core/repository/redshift.py
--rw-r--r--   0        0        0     1874 2024-03-15 09:23:26.513415 quollio_core-0.4.4/quollio_core/repository/snowflake.py
--rw-r--r--   0        0        0    10333 2024-03-15 09:23:26.513415 quollio_core-0.4.4/quollio_core/snowflake.py
--rw-r--r--   0        0        0     6400 1970-01-01 00:00:00.000000 quollio_core-0.4.4/PKG-INFO
+-rw-r--r--   0        0        0    34520 2024-05-07 08:43:16.812994 quollio_core-0.4.5/LICENSE
+-rw-r--r--   0        0        0     4770 2024-05-07 08:43:16.812994 quollio_core-0.4.5/README.md
+-rw-r--r--   0        0        0     2003 2024-05-07 08:43:16.812994 quollio_core-0.4.5/pyproject.toml
+-rw-r--r--   0        0        0       83 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/__init__.py
+-rw-r--r--   0        0        0     8001 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/bricks.py
+-rw-r--r--   0        0        0       29 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/.gitignore
+-rw-r--r--   0        0        0      440 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/analyses/.gitkeep
+-rw-r--r--   0        0        0      480 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/dbt_project.yml
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/macros/.gitkeep
+-rw-r--r--   0        0        0     2171 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/models/quollio_lineage_column_level.sql
+-rw-r--r--   0        0        0      450 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/models/quollio_lineage_column_level.yml
+-rw-r--r--   0        0        0     1558 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/models/quollio_lineage_table_level.sql
+-rw-r--r--   0        0        0      344 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/models/quollio_lineage_table_level.yml
+-rw-r--r--   0        0        0     2231 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/models/sources.yml
+-rw-r--r--   0        0        0      376 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/package-lock.yml
+-rw-r--r--   0        0        0      443 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/packages.yml
+-rw-r--r--   0        0        0      353 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/profiles/profiles_template.yml
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/seeds/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/snapshots/.gitkeep
+-rw-r--r--   0        0        0      571 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/analyses/.gitkeep
+-rw-r--r--   0        0        0      405 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/dbt_project.yml
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/macros/.gitkeep
+-rw-r--r--   0        0        0     3998 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/macros/materialization/divided_view.sql
+-rw-r--r--   0        0        0     2042 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_lineage_table_level.sql
+-rw-r--r--   0        0        0      236 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_lineage_table_level.yml
+-rw-r--r--   0        0        0     1289 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_lineage_view_level.sql
+-rw-r--r--   0        0        0      235 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_lineage_view_level.yml
+-rw-r--r--   0        0        0     1049 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_sqllineage_sources.sql
+-rw-r--r--   0        0        0      377 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_sqllineage_sources.yml
+-rw-r--r--   0        0        0      302 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_stats_columns.sql
+-rw-r--r--   0        0        0       67 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_stats_columns.yml
+-rw-r--r--   0        0        0     1592 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.sql
+-rw-r--r--   0        0        0      523 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.yml
+-rw-r--r--   0        0        0    14646 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/sources.yml
+-rw-r--r--   0        0        0      109 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/package-lock.yml
+-rw-r--r--   0        0        0       61 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/packages.yml
+-rw-r--r--   0        0        0      291 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/profiles/profiles_template.yml
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/seeds/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/snapshots/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/seeds/.gitkeep
+-rw-r--r--   0        0        0      571 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/analyses/.gitkeep
+-rw-r--r--   0        0        0      407 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/dbt_project.yml
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/macros/.gitkeep
+-rw-r--r--   0        0        0     2782 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/macros/materialization/divided_view.sql
+-rw-r--r--   0        0        0     4721 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.sql
+-rw-r--r--   0        0        0      711 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.yml
+-rw-r--r--   0        0        0     5112 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_lineage_table_level.sql
+-rw-r--r--   0        0        0      325 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_lineage_table_level.yml
+-rw-r--r--   0        0        0     1520 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_sqllineage_sources.sql
+-rw-r--r--   0        0        0      377 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_sqllineage_sources.yml
+-rw-r--r--   0        0        0      302 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_stats_columns.sql
+-rw-r--r--   0        0        0       67 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_stats_columns.yml
+-rw-r--r--   0        0        0     1382 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.sql
+-rw-r--r--   0        0        0      538 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.yml
+-rw-r--r--   0        0        0    10975 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/sources.yml
+-rw-r--r--   0        0        0      109 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/package-lock.yml
+-rw-r--r--   0        0        0       61 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/packages.yml
+-rw-r--r--   0        0        0      379 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/profiles/profiles_template.yml
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/seeds/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/snapshots/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/helper/__init__.py
+-rw-r--r--   0        0        0     1127 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/helper/core.py
+-rw-r--r--   0        0        0     1202 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/helper/env_default.py
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/profilers/__init__.py
+-rw-r--r--   0        0        0     7501 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/profilers/databricks.py
+-rw-r--r--   0        0        0     6379 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/profilers/lineage.py
+-rw-r--r--   0        0        0     7862 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/profilers/redshift.py
+-rw-r--r--   0        0        0     9090 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/profilers/snowflake.py
+-rw-r--r--   0        0        0     5177 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/profilers/sqllineage.py
+-rw-r--r--   0        0        0     4720 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/profilers/stats.py
+-rw-r--r--   0        0        0    10167 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/redshift.py
+-rw-r--r--   0        0        0        0 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/repository/__init__.py
+-rw-r--r--   0        0        0     1945 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/repository/databricks.py
+-rw-r--r--   0        0        0      770 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/repository/dbt.py
+-rw-r--r--   0        0        0     4702 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/repository/qdc.py
+-rw-r--r--   0        0        0     2991 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/repository/redshift.py
+-rw-r--r--   0        0        0     1874 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/repository/snowflake.py
+-rw-r--r--   0        0        0    10266 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/snowflake.py
+-rw-r--r--   0        0        0     6571 1970-01-01 00:00:00.000000 quollio_core-0.4.5/PKG-INFO
```

### Comparing `quollio_core-0.4.4/LICENSE` & `quollio_core-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/README.md` & `quollio_core-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/pyproject.toml` & `quollio_core-0.4.5/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -29,31 +29,35 @@
 ]
 
 dependencies = [
     "blake3==0.3.3"
     ,"dbt-core==1.7.10"
     ,"dbt-snowflake==1.7.0"
     ,"dbt-redshift==1.7.1"
+    ,"dbt-databricks==1.7.1"
     ,"jinja2==3.1.3"
     ,"PyYAML==6.0.1"
     ,"requests==2.31.0"
     ,"pyjwt==2.8.0"
     ,"redshift-connector==2.0.915"
     ,"snowflake-connector-python==3.5.0"
+    ,"databricks-sdk==0.17.0"
+    ,"databricks-sql-connector==2.9.5"
     ,"sqlglot==20.8.0"
 ]
 dynamic = ["version", "description"]
 
 [project.urls]
 Source = "https://github.com/QuollioLabs/quollio-core"
 Home = "https://quollio.com"
 
 [project.optional-dependencies]
 test = [
   "black>=22.3.0"
+  ,"coverage>=7.3.2"
   ,"isort>=5.10.1"
   ,"pyproject-flake8>=0.0.1-alpha.2"
   ,"pytest>=5.2"
   ,"dbt-osmosis==0.12.5"
 ]
 
 [tool.flit.module]
```

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/redshift/README.md` & `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/README.md`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/redshift/macros/materialization/divided_view.sql` & `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/macros/materialization/divided_view.sql`

 * *Files 17% similar despite different names*

```diff
@@ -19,37 +19,65 @@
 {%- set records = [] -%}
 {%- endif -%}
 
 -- build sql
 {%- for i in range(0, records|length, chunk) -%}
   {%- set build_sql %}
   {%- for record in records[i: i+chunk] -%}
-    {%- if not loop.first %}UNION{% endif %}
+    {%- if not loop.first -%}UNION{% endif %}
     SELECT
-      DISTINCT
-      '{{record[0]}}'::varchar as db_name
-      , '{{record[1]}}'::varchar as schema_name
-      , '{{record[2]}}'::varchar as table_name
-      , '{{record[3]}}'::varchar as column_name
-      , {% if var("skip_heavy") == false and record[5] == true %}cast(max("{{record[3]}}") as varchar){% else %}null::varchar{% endif %} AS max_value
-      , {% if var("skip_heavy") == false and record[5] == true %}cast(min("{{record[3]}}") as varchar){% else %}null::varchar{% endif %} AS min_value
-      -- requires full table scan
-      , {% if var("skip_heavy") == false %}cast(SUM(NVL2("{{record[3]}}", 0, 1)) as integer){% else %}null::integer{% endif %} AS null_count
-      , APPROXIMATE COUNT(DISTINCT "{{record[3]}}") AS cardinality
-      -- requires full table scan
-      , {% if var("skip_heavy") == false and record[5] == true %}cast(avg("{{record[3]}}")as varchar){% else %}null::varchar{% endif %} AS avg_value
-      , {% if var("skip_heavy") == false and record[5] == true %}(SELECT cast(median("{{record[3]}}") as varchar) FROM {{record[2]}}){% else %}null::varchar{% endif %} AS median_value
-      -- requires full table scan
-      , {% if var("skip_heavy") == false and record[4] == false %}
-          (SELECT cast("{{record[3]}}" as varchar) FROM (
-            SELECT "{{record[3]}}", ROW_NUMBER() OVER (ORDER BY COUNT(*) DESC) AS row_num FROM {{record[2]}} GROUP BY "{{record[3]}}"
-          ) WHERE row_num = 1)
-        {% else %}null::varchar{% endif %} AS mode_value
-      , {% if record[5] == true %}cast(STDDEV_SAMP("{{record[3]}}") as integer){% else %}null::integer{% endif %} AS stddev_value
-    FROM {{ record[0] }}.{{ record[1] }}.{{ record[2] }}
+      main.db_name
+      , main.schema_name
+      , main.table_name
+      , main.column_name
+      , main.max_value
+      , main.min_value
+      , main.null_count
+      , main.cardinality
+      , main.avg_value
+      , main.median_value
+      , mode.mode_value
+      , main.stddev_value
+    FROM
+      (
+      SELECT
+        DISTINCT
+        '{{record[0]}}'::varchar as db_name
+        , '{{record[1]}}'::varchar as schema_name
+        , '{{record[2]}}'::varchar as table_name
+        , '{{record[3]}}'::varchar as column_name
+        , {% if var("skip_heavy") == false and record[5] == true %}cast(max("{{record[3]}}") as varchar){% else %}null::varchar{% endif %} AS max_value
+        , {% if var("skip_heavy") == false and record[5] == true %}cast(min("{{record[3]}}") as varchar){% else %}null::varchar{% endif %} AS min_value
+        -- requires full table scan
+        , {% if var("skip_heavy") == false %}cast(SUM(NVL2("{{record[3]}}", 0, 1)) as integer){% else %}null::integer{% endif %} AS null_count
+        , APPROXIMATE COUNT(DISTINCT "{{record[3]}}") AS cardinality
+        -- requires full table scan
+        , {% if var("skip_heavy") == false and record[5] == true %}cast(avg("{{record[3]}}")as varchar){% else %}null::varchar{% endif %} AS avg_value
+        , {% if var("skip_heavy") == false and record[5] == true %}cast(median("{{record[3]}}") as varchar){% else %}null::varchar{% endif %} AS median_value
+        -- requires full table scan
+        , {% if record[5] == true %}cast(STDDEV_SAMP("{{record[3]}}") as integer){% else %}null::integer{% endif %} AS stddev_value
+      FROM {{ record[0] }}.{{ record[1] }}.{{ record[2] }}
+    ) main, (
+      {%- if var("skip_heavy") == false and record[4] == false %}
+        SELECT
+          cast("{{record[3]}}" as varchar) mode_value
+        FROM (
+           SELECT
+            DISTINCT
+            "{{record[3]}}"
+            , ROW_NUMBER() OVER (ORDER BY COUNT(*) DESC) AS row_num
+          FROM {{ record[0] }}.{{ record[1] }}.{{ record[2] }}
+          GROUP BY
+            "{{record[3]}}"
+        )
+        WHERE
+          row_num = 1
+      {% else %}
+        SELECT null as mode_value {%- endif -%}
+    ) mode
   {% endfor -%}
   {%- endset %}
   -- create a view with a index as suffix
   {%- set target_identifier = "%s_%d"|format(model['name'], loop.index) %}
   {%- set target_relation = api.Relation.create(identifier=target_identifier, schema=schema, database=database, type='view') %}
   -- {{ drop_relation_if_exists(target_relation) }}
   {% call statement("main") %}
```

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_lineage_table_level.sql` & `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_lineage_table_level.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_lineage_view_level.sql` & `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_lineage_view_level.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_sqllineage_sources.sql` & `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_sqllineage_sources.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.sql` & `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.yml` & `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.yml`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/redshift/models/sources.yml` & `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/sources.yml`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/README.md` & `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/README.md`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/macros/materialization/divided_view.sql` & `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/macros/materialization/divided_view.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.sql` & `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.yml` & `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.yml`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_lineage_table_level.sql` & `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_lineage_table_level.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_sqllineage_sources.sql` & `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_sqllineage_sources.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.sql` & `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.yml` & `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.yml`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/dbt_projects/snowflake/models/sources.yml` & `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/sources.yml`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/helper/core.py` & `quollio_core-0.4.5/quollio_core/helper/core.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/helper/env_default.py` & `quollio_core-0.4.5/quollio_core/helper/env_default.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,18 @@
 class EnvDefault(argparse.Action):
     """An argparse action class that auto-sets missing default values from env
     vars. Defaults to requiring the argument."""
 
     def __init__(self, envvar, required=True, default=None, **kwargs):
         # override values if envvar exists
         if envvar in os.environ:
-            default = os.environ[envvar]
+            if kwargs.get("nargs", None) is None:
+                default = os.environ[envvar]
+            else:
+                default = os.environ[envvar].split(" ")
         if required and default:
             required = False
         super(EnvDefault, self).__init__(default=default, required=required, **kwargs)
 
     def __call__(self, parser, namespace, values, option_string=None):
         setattr(namespace, self.dest, values)
```

### Comparing `quollio_core-0.4.4/quollio_core/profilers/lineage.py` & `quollio_core-0.4.5/quollio_core/profilers/lineage.py`

 * *Files 4% similar despite different names*

```diff
@@ -137,7 +137,19 @@
     for result in results:
         payload = dict()
         payload["DOWNSTREAM_TABLE_NAME"] = result["DOWNSTREAM_TABLE_NAME"]
         payload["DOWNSTREAM_TABLE_DOMAIN"] = result["DOWNSTREAM_TABLE_DOMAIN"]
         payload["UPSTREAM_TABLES"] = json.loads(result["UPSTREAM_TABLES"])
         payloads.append(payload)
     return payloads
+
+
+def parse_databricks_table_lineage(results: List) -> List[Dict[str, Dict]]:
+    # Parses results from Quollio Databricks lineage table
+    # Returns tuple of downstream_table_name (0) and upstream_tables (1)
+    payloads = list()
+    for result in results:
+        payload = dict()
+        payload["DOWNSTREAM_TABLE_NAME"] = result["DOWNSTREAM_TABLE_NAME"]
+        payload["UPSTREAM_TABLES"] = json.loads(result["UPSTREAM_TABLES"])
+        payloads.append(payload)
+    return payloads
```

### Comparing `quollio_core-0.4.4/quollio_core/profilers/redshift.py` & `quollio_core-0.4.5/quollio_core/profilers/redshift.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/profilers/snowflake.py` & `quollio_core-0.4.5/quollio_core/profilers/snowflake.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/profilers/sqllineage.py` & `quollio_core-0.4.5/quollio_core/profilers/sqllineage.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/profilers/stats.py` & `quollio_core-0.4.5/quollio_core/profilers/stats.py`

 * *Files 0% similar despite different names*

```diff
@@ -73,15 +73,14 @@
     for stat in stats:
         global_id_arg = "{db}{schema}{table}{column}".format(
             db=stat["DB_NAME"], schema=stat["SCHEMA_NAME"], table=stat["TABLE_NAME"], column=stat["COLUMN_NAME"]
         )
         table_global_id = new_global_id(
             tenant_id=tenant_id, cluster_id=endpoint, data_id=global_id_arg, data_type="column"
         )
-
         stats_request = StatsRequest(
             global_id=table_global_id,
             db=stat["DB_NAME"],
             schema=stat["SCHEMA_NAME"],
             table=stat["TABLE_NAME"],
             column=stat["COLUMN_NAME"],
             body=StatsInput(
```

### Comparing `quollio_core-0.4.4/quollio_core/redshift.py` & `quollio_core-0.4.5/quollio_core/redshift.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,18 @@
     dbt_client.invoke(
         cmd="deps",
         project_dir=project_path,
         profile_dir=template_path,
         options=["--no-use-colors", "--log-level", log_level, "--vars", options],
     )
     run_options = ["--no-use-colors", "--log-level", log_level, "--vars", options]
-    target_tables_list = target_tables.split()
-    if target_tables_list is not None:
-        if "quollio_stats_columns" in target_tables_list:
-            target_tables_list.append("quollio_stats_profiling_columns")
-        target_tables_str = " ".join(target_tables_list)
+    if target_tables is not None:
+        if "quollio_stats_columns" in target_tables:
+            target_tables.append("quollio_stats_profiling_columns")
+        target_tables_str = " ".join(target_tables)
         run_options.append("--select")
         run_options.append(target_tables_str)
 
     dbt_client.invoke(
         cmd="run",
         project_dir=project_path,
         profile_dir=template_path,
```

### Comparing `quollio_core-0.4.4/quollio_core/repository/dbt.py` & `quollio_core-0.4.5/quollio_core/repository/dbt.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/repository/qdc.py` & `quollio_core-0.4.5/quollio_core/repository/qdc.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/repository/redshift.py` & `quollio_core-0.4.5/quollio_core/repository/redshift.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/repository/snowflake.py` & `quollio_core-0.4.5/quollio_core/repository/snowflake.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.4/quollio_core/snowflake.py` & `quollio_core-0.4.5/quollio_core/snowflake.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,19 +46,18 @@
     dbt_client.invoke(
         cmd="deps",
         project_dir=project_path,
         profile_dir=template_path,
         options=["--no-use-colors", "--log-level", log_level, "--vars", options],
     )
     run_options = ["--no-use-colors", "--log-level", log_level, "--vars", options]
-    target_tables_list = target_tables.split()
-    if target_tables_list is not None:
-        if "quollio_stats_columns" in target_tables_list:
-            target_tables_list.append("quollio_stats_profiling_columns")
-        target_tables_str = " ".join(target_tables_list)
+    if target_tables is not None:
+        if "quollio_stats_columns" in target_tables:
+            target_tables.append("quollio_stats_profiling_columns")
+        target_tables_str = " ".join(target_tables)
         run_options.append("--select")
         run_options.append(target_tables_str)
 
     dbt_client.invoke(
         cmd="run",
         project_dir=project_path,
         profile_dir=template_path,
```

### Comparing `quollio_core-0.4.4/PKG-INFO` & `quollio_core-0.4.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quollio-core
-Version: 0.4.4
+Version: 0.4.5
 Summary: Quollio Core
 Author-email: quollio-dev <qt.dev@quollio.com>
 Maintainer-email: RyoAriyama <ryo.arym@gmail.com>, tharuta <35373297+TakumiHaruta@users.noreply.github.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -17,22 +17,26 @@
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: blake3==0.3.3
 Requires-Dist: dbt-core==1.7.10
 Requires-Dist: dbt-snowflake==1.7.0
 Requires-Dist: dbt-redshift==1.7.1
+Requires-Dist: dbt-databricks==1.7.1
 Requires-Dist: jinja2==3.1.3
 Requires-Dist: PyYAML==6.0.1
 Requires-Dist: requests==2.31.0
 Requires-Dist: pyjwt==2.8.0
 Requires-Dist: redshift-connector==2.0.915
 Requires-Dist: snowflake-connector-python==3.5.0
+Requires-Dist: databricks-sdk==0.17.0
+Requires-Dist: databricks-sql-connector==2.9.5
 Requires-Dist: sqlglot==20.8.0
 Requires-Dist: black>=22.3.0 ; extra == "test"
+Requires-Dist: coverage>=7.3.2 ; extra == "test"
 Requires-Dist: isort>=5.10.1 ; extra == "test"
 Requires-Dist: pyproject-flake8>=0.0.1-alpha.2 ; extra == "test"
 Requires-Dist: pytest>=5.2 ; extra == "test"
 Requires-Dist: dbt-osmosis==0.12.5 ; extra == "test"
 Project-URL: Home, https://quollio.com
 Project-URL: Source, https://github.com/QuollioLabs/quollio-core
 Provides-Extra: test
```

