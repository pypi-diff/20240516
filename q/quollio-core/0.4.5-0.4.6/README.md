# Comparing `tmp/quollio_core-0.4.5.tar.gz` & `tmp/quollio_core-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "quollio_core-0.4.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "quollio_core-0.4.6.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `quollio_core-0.4.5.tar` & `quollio_core-0.4.6.tar`

### file list

```diff
@@ -1,82 +1,82 @@
--rw-r--r--   0        0        0    34520 2024-05-07 08:43:16.812994 quollio_core-0.4.5/LICENSE
--rw-r--r--   0        0        0     4770 2024-05-07 08:43:16.812994 quollio_core-0.4.5/README.md
--rw-r--r--   0        0        0     2003 2024-05-07 08:43:16.812994 quollio_core-0.4.5/pyproject.toml
--rw-r--r--   0        0        0       83 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/__init__.py
--rw-r--r--   0        0        0     8001 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/bricks.py
--rw-r--r--   0        0        0       29 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/.gitignore
--rw-r--r--   0        0        0      440 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/README.md
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/analyses/.gitkeep
--rw-r--r--   0        0        0      480 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/dbt_project.yml
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/macros/.gitkeep
--rw-r--r--   0        0        0     2171 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/models/quollio_lineage_column_level.sql
--rw-r--r--   0        0        0      450 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/models/quollio_lineage_column_level.yml
--rw-r--r--   0        0        0     1558 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/models/quollio_lineage_table_level.sql
--rw-r--r--   0        0        0      344 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/models/quollio_lineage_table_level.yml
--rw-r--r--   0        0        0     2231 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/models/sources.yml
--rw-r--r--   0        0        0      376 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/package-lock.yml
--rw-r--r--   0        0        0      443 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/packages.yml
--rw-r--r--   0        0        0      353 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/profiles/profiles_template.yml
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/seeds/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/databricks/snapshots/.gitkeep
--rw-r--r--   0        0        0      571 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/README.md
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/analyses/.gitkeep
--rw-r--r--   0        0        0      405 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/dbt_project.yml
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/macros/.gitkeep
--rw-r--r--   0        0        0     3998 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/macros/materialization/divided_view.sql
--rw-r--r--   0        0        0     2042 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_lineage_table_level.sql
--rw-r--r--   0        0        0      236 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_lineage_table_level.yml
--rw-r--r--   0        0        0     1289 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_lineage_view_level.sql
--rw-r--r--   0        0        0      235 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_lineage_view_level.yml
--rw-r--r--   0        0        0     1049 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_sqllineage_sources.sql
--rw-r--r--   0        0        0      377 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_sqllineage_sources.yml
--rw-r--r--   0        0        0      302 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_stats_columns.sql
--rw-r--r--   0        0        0       67 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_stats_columns.yml
--rw-r--r--   0        0        0     1592 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.sql
--rw-r--r--   0        0        0      523 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.yml
--rw-r--r--   0        0        0    14646 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/sources.yml
--rw-r--r--   0        0        0      109 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/package-lock.yml
--rw-r--r--   0        0        0       61 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/packages.yml
--rw-r--r--   0        0        0      291 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/profiles/profiles_template.yml
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/seeds/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/redshift/snapshots/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/seeds/.gitkeep
--rw-r--r--   0        0        0      571 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/README.md
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/analyses/.gitkeep
--rw-r--r--   0        0        0      407 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/dbt_project.yml
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/macros/.gitkeep
--rw-r--r--   0        0        0     2782 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/macros/materialization/divided_view.sql
--rw-r--r--   0        0        0     4721 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.sql
--rw-r--r--   0        0        0      711 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.yml
--rw-r--r--   0        0        0     5112 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_lineage_table_level.sql
--rw-r--r--   0        0        0      325 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_lineage_table_level.yml
--rw-r--r--   0        0        0     1520 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_sqllineage_sources.sql
--rw-r--r--   0        0        0      377 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_sqllineage_sources.yml
--rw-r--r--   0        0        0      302 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_stats_columns.sql
--rw-r--r--   0        0        0       67 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_stats_columns.yml
--rw-r--r--   0        0        0     1382 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.sql
--rw-r--r--   0        0        0      538 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.yml
--rw-r--r--   0        0        0    10975 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/sources.yml
--rw-r--r--   0        0        0      109 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/package-lock.yml
--rw-r--r--   0        0        0       61 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/packages.yml
--rw-r--r--   0        0        0      379 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/profiles/profiles_template.yml
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/seeds/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/snapshots/.gitkeep
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/helper/__init__.py
--rw-r--r--   0        0        0     1127 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/helper/core.py
--rw-r--r--   0        0        0     1202 2024-05-07 08:43:16.812994 quollio_core-0.4.5/quollio_core/helper/env_default.py
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/profilers/__init__.py
--rw-r--r--   0        0        0     7501 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/profilers/databricks.py
--rw-r--r--   0        0        0     6379 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/profilers/lineage.py
--rw-r--r--   0        0        0     7862 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/profilers/redshift.py
--rw-r--r--   0        0        0     9090 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/profilers/snowflake.py
--rw-r--r--   0        0        0     5177 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/profilers/sqllineage.py
--rw-r--r--   0        0        0     4720 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/profilers/stats.py
--rw-r--r--   0        0        0    10167 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/redshift.py
--rw-r--r--   0        0        0        0 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/repository/__init__.py
--rw-r--r--   0        0        0     1945 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/repository/databricks.py
--rw-r--r--   0        0        0      770 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/repository/dbt.py
--rw-r--r--   0        0        0     4702 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/repository/qdc.py
--rw-r--r--   0        0        0     2991 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/repository/redshift.py
--rw-r--r--   0        0        0     1874 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/repository/snowflake.py
--rw-r--r--   0        0        0    10266 2024-05-07 08:43:16.816994 quollio_core-0.4.5/quollio_core/snowflake.py
--rw-r--r--   0        0        0     6571 1970-01-01 00:00:00.000000 quollio_core-0.4.5/PKG-INFO
+-rw-r--r--   0        0        0    34520 2024-05-16 06:58:43.671600 quollio_core-0.4.6/LICENSE
+-rw-r--r--   0        0        0     4770 2024-05-16 06:58:43.671600 quollio_core-0.4.6/README.md
+-rw-r--r--   0        0        0     2003 2024-05-16 06:58:43.671600 quollio_core-0.4.6/pyproject.toml
+-rw-r--r--   0        0        0       83 2024-05-16 06:58:43.671600 quollio_core-0.4.6/quollio_core/__init__.py
+-rw-r--r--   0        0        0     8001 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/bricks.py
+-rw-r--r--   0        0        0       29 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/.gitignore
+-rw-r--r--   0        0        0      440 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/analyses/.gitkeep
+-rw-r--r--   0        0        0      480 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/dbt_project.yml
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/macros/.gitkeep
+-rw-r--r--   0        0        0     2171 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/models/quollio_lineage_column_level.sql
+-rw-r--r--   0        0        0      450 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/models/quollio_lineage_column_level.yml
+-rw-r--r--   0        0        0     1558 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/models/quollio_lineage_table_level.sql
+-rw-r--r--   0        0        0      344 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/models/quollio_lineage_table_level.yml
+-rw-r--r--   0        0        0     2231 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/models/sources.yml
+-rw-r--r--   0        0        0      376 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/package-lock.yml
+-rw-r--r--   0        0        0      443 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/packages.yml
+-rw-r--r--   0        0        0      353 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/profiles/profiles_template.yml
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/seeds/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/databricks/snapshots/.gitkeep
+-rw-r--r--   0        0        0      571 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/analyses/.gitkeep
+-rw-r--r--   0        0        0      405 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/dbt_project.yml
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/macros/.gitkeep
+-rw-r--r--   0        0        0     3998 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/macros/materialization/divided_view.sql
+-rw-r--r--   0        0        0     2042 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_lineage_table_level.sql
+-rw-r--r--   0        0        0      236 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_lineage_table_level.yml
+-rw-r--r--   0        0        0     1289 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_lineage_view_level.sql
+-rw-r--r--   0        0        0      235 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_lineage_view_level.yml
+-rw-r--r--   0        0        0     1049 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_sqllineage_sources.sql
+-rw-r--r--   0        0        0      377 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_sqllineage_sources.yml
+-rw-r--r--   0        0        0      302 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_stats_columns.sql
+-rw-r--r--   0        0        0       67 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_stats_columns.yml
+-rw-r--r--   0        0        0     1592 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.sql
+-rw-r--r--   0        0        0      523 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.yml
+-rw-r--r--   0        0        0    14646 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/sources.yml
+-rw-r--r--   0        0        0      109 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/package-lock.yml
+-rw-r--r--   0        0        0       61 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/packages.yml
+-rw-r--r--   0        0        0      291 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/profiles/profiles_template.yml
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/seeds/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/redshift/snapshots/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/seeds/.gitkeep
+-rw-r--r--   0        0        0      571 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/analyses/.gitkeep
+-rw-r--r--   0        0        0      407 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/dbt_project.yml
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/macros/.gitkeep
+-rw-r--r--   0        0        0     2782 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/macros/materialization/divided_view.sql
+-rw-r--r--   0        0        0     4721 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.sql
+-rw-r--r--   0        0        0      711 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.yml
+-rw-r--r--   0        0        0     5112 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_lineage_table_level.sql
+-rw-r--r--   0        0        0      325 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_lineage_table_level.yml
+-rw-r--r--   0        0        0     1520 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_sqllineage_sources.sql
+-rw-r--r--   0        0        0      377 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_sqllineage_sources.yml
+-rw-r--r--   0        0        0      302 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_stats_columns.sql
+-rw-r--r--   0        0        0       67 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_stats_columns.yml
+-rw-r--r--   0        0        0     1382 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.sql
+-rw-r--r--   0        0        0      538 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.yml
+-rw-r--r--   0        0        0    10975 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/sources.yml
+-rw-r--r--   0        0        0      109 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/package-lock.yml
+-rw-r--r--   0        0        0       61 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/packages.yml
+-rw-r--r--   0        0        0      379 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/profiles/profiles_template.yml
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/seeds/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/snapshots/.gitkeep
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/helper/__init__.py
+-rw-r--r--   0        0        0     1127 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/helper/core.py
+-rw-r--r--   0        0        0     1202 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/helper/env_default.py
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/profilers/__init__.py
+-rw-r--r--   0        0        0     7257 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/profilers/databricks.py
+-rw-r--r--   0        0        0     6379 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/profilers/lineage.py
+-rw-r--r--   0        0        0     7862 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/profilers/redshift.py
+-rw-r--r--   0        0        0     9090 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/profilers/snowflake.py
+-rw-r--r--   0        0        0     5177 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/profilers/sqllineage.py
+-rw-r--r--   0        0        0     4720 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/profilers/stats.py
+-rw-r--r--   0        0        0    10167 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/redshift.py
+-rw-r--r--   0        0        0        0 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/repository/__init__.py
+-rw-r--r--   0        0        0     1945 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/repository/databricks.py
+-rw-r--r--   0        0        0      770 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/repository/dbt.py
+-rw-r--r--   0        0        0     4702 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/repository/qdc.py
+-rw-r--r--   0        0        0     2991 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/repository/redshift.py
+-rw-r--r--   0        0        0     1874 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/repository/snowflake.py
+-rw-r--r--   0        0        0    10266 2024-05-16 06:58:43.675600 quollio_core-0.4.6/quollio_core/snowflake.py
+-rw-r--r--   0        0        0     6571 1970-01-01 00:00:00.000000 quollio_core-0.4.6/PKG-INFO
```

### Comparing `quollio_core-0.4.5/LICENSE` & `quollio_core-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/README.md` & `quollio_core-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/pyproject.toml` & `quollio_core-0.4.6/pyproject.toml`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/bricks.py` & `quollio_core-0.4.6/quollio_core/bricks.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/databricks/models/quollio_lineage_column_level.sql` & `quollio_core-0.4.6/quollio_core/dbt_projects/databricks/models/quollio_lineage_column_level.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/databricks/models/quollio_lineage_table_level.sql` & `quollio_core-0.4.6/quollio_core/dbt_projects/databricks/models/quollio_lineage_table_level.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/databricks/models/sources.yml` & `quollio_core-0.4.6/quollio_core/dbt_projects/databricks/models/sources.yml`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/README.md` & `quollio_core-0.4.6/quollio_core/dbt_projects/redshift/README.md`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/macros/materialization/divided_view.sql` & `quollio_core-0.4.6/quollio_core/dbt_projects/redshift/macros/materialization/divided_view.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_lineage_table_level.sql` & `quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_lineage_table_level.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_lineage_view_level.sql` & `quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_lineage_view_level.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_sqllineage_sources.sql` & `quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_sqllineage_sources.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.sql` & `quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.yml` & `quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/quollio_stats_profiling_columns.yml`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/redshift/models/sources.yml` & `quollio_core-0.4.6/quollio_core/dbt_projects/redshift/models/sources.yml`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/README.md` & `quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/README.md`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/macros/materialization/divided_view.sql` & `quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/macros/materialization/divided_view.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.sql` & `quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.yml` & `quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_lineage_column_level.yml`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_lineage_table_level.sql` & `quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_lineage_table_level.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_sqllineage_sources.sql` & `quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_sqllineage_sources.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.sql` & `quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.sql`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.yml` & `quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/quollio_stats_profiling_columns.yml`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/dbt_projects/snowflake/models/sources.yml` & `quollio_core-0.4.6/quollio_core/dbt_projects/snowflake/models/sources.yml`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/helper/core.py` & `quollio_core-0.4.6/quollio_core/helper/core.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/helper/env_default.py` & `quollio_core-0.4.6/quollio_core/helper/env_default.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/profilers/databricks.py` & `quollio_core-0.4.6/quollio_core/profilers/databricks.py`

 * *Files 6% similar despite different names*

```diff
@@ -132,45 +132,42 @@
     for table in tables:
         monitored_table = table["table_fqdn"].removesuffix("_profile_metrics")
         monitored_table = monitored_table.split(".")
         if len(monitored_table) != 3:
             raise ValueError(f"Invalid table name: {table['table_fqdn']}")
         with databricks.DatabricksQueryExecutor(config=conn) as databricks_executor:
             query = """
-                WITH MaxCounts AS (
-                    SELECT
-                        t.COLUMN_NAME,
-                        MAX(item.count) AS max_count,
-                        MAX(t.window) AS latest
-                    FROM
-                        {monitoring_table} t
-                    LATERAL VIEW EXPLODE(t.frequent_items) AS item
-                    GROUP BY t.COLUMN_NAME
-                )
                 SELECT
                     "{monitored_table_catalog}" as DB_NAME,
                     "{monitored_table_schema}" as SCHEMA_NAME,
                     "{monitored_table_name}" as TABLE_NAME,
                     t.COLUMN_NAME,
                     t.DATA_TYPE,
                     t.distinct_count as CARDINALITY,
                     t.MAX as MAX_VALUE,
                     t.MIN as MIN_VALUE,
                     t.AVG as AVG_VALUE,
                     t.MEDIAN as MEDIAN_VALUE,
                     t.STDDEV as STDDEV_VALUE,
                     t.NUM_NULLS as NULL_COUNT,
-                    item.item AS MODE_VALUE
+                    t.frequent_items[0].item AS MODE_VALUE,
+                    MAX(t.window) AS LATEST
                 FROM
                     {monitoring_table} t
-                JOIN MaxCounts mc ON t.COLUMN_NAME = mc.COLUMN_NAME
-                LATERAL VIEW EXPLODE(t.frequent_items) AS item
-                WHERE
-                    item.count = mc.max_count
-                    AND t.window = mc.latest
+                GROUP BY
+                    t.COLUMN_NAME,
+                    t.DATA_TYPE,
+                    t.distinct_count,
+                    t.MAX,
+                    t.MIN,
+                    t.AVG,
+                    t.MEDIAN,
+                    t.STDDEV,
+                    t.NUM_NULLS,
+                    t.frequent_items
                 """.format(
                 monitoring_table=table["table_fqdn"],
                 monitored_table_catalog=monitored_table[0],
                 monitored_table_schema=monitored_table[1],
                 monitored_table_name=monitored_table[2],
             )
             stats.append(databricks_executor.get_query_results(query))
```

### Comparing `quollio_core-0.4.5/quollio_core/profilers/lineage.py` & `quollio_core-0.4.6/quollio_core/profilers/lineage.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/profilers/redshift.py` & `quollio_core-0.4.6/quollio_core/profilers/redshift.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/profilers/snowflake.py` & `quollio_core-0.4.6/quollio_core/profilers/snowflake.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/profilers/sqllineage.py` & `quollio_core-0.4.6/quollio_core/profilers/sqllineage.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/profilers/stats.py` & `quollio_core-0.4.6/quollio_core/profilers/stats.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/redshift.py` & `quollio_core-0.4.6/quollio_core/redshift.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/repository/databricks.py` & `quollio_core-0.4.6/quollio_core/repository/databricks.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/repository/dbt.py` & `quollio_core-0.4.6/quollio_core/repository/dbt.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/repository/qdc.py` & `quollio_core-0.4.6/quollio_core/repository/qdc.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/repository/redshift.py` & `quollio_core-0.4.6/quollio_core/repository/redshift.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/repository/snowflake.py` & `quollio_core-0.4.6/quollio_core/repository/snowflake.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/quollio_core/snowflake.py` & `quollio_core-0.4.6/quollio_core/snowflake.py`

 * *Files identical despite different names*

### Comparing `quollio_core-0.4.5/PKG-INFO` & `quollio_core-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: quollio-core
-Version: 0.4.5
+Version: 0.4.6
 Summary: Quollio Core
 Author-email: quollio-dev <qt.dev@quollio.com>
 Maintainer-email: RyoAriyama <ryo.arym@gmail.com>, tharuta <35373297+TakumiHaruta@users.noreply.github.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

