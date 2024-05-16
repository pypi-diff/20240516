# Comparing `tmp/cumulus_library-2.1.0.tar.gz` & `tmp/cumulus_library-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library-2.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library-2.2.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library-2.1.0.tar` & `cumulus_library-2.2.0.tar`

### file list

```diff
@@ -1,109 +1,109 @@
-lrwxr-xr-x   0        0        0        0 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/.sqlfluff -> cumulus_library/.sqlfluff
--rw-r--r--   0        0        0      689 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/README.md
--rw-r--r--   0        0        0     7061 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/.sqlfluff
--rw-r--r--   0        0        0       46 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/__init__.py
--rw-r--r--   0        0        0        0 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/apis/__init__.py
--rw-r--r--   0        0        0     6322 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/apis/umls.py
--rw-r--r--   0        0        0     4837 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/base_table_builder.py
--rw-r--r--   0        0        0     3892 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/base_utils.py
--rwxr-xr-x   0        0        0    18237 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/cli.py
--rw-r--r--   0        0        0     8187 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/cli_parser.py
--rw-r--r--   0        0        0    20782 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/databases.py
--rw-r--r--   0        0        0      249 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/db_config.py
--rw-r--r--   0        0        0      422 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/enums.py
--rw-r--r--   0        0        0      665 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/errors.py
--rw-r--r--   0        0        0      205 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/module_allowlist.json
--rw-r--r--   0        0        0     2311 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/parsers/fhir_valueset.py
--rw-r--r--   0        0        0     1716 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/protected_table_builder.py
--rw-r--r--   0        0        0        0 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/schema/__init__.py
--rw-r--r--   0        0        0     4731 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/schema/columns.py
--rw-r--r--   0        0        0     3364 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/schema/typesystem.py
--rw-r--r--   0        0        0     6024 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/schema/valueset.py
--rw-r--r--   0        0        0    10732 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/counts.py
--rw-r--r--   0        0        0    14453 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/psm.py
--rw-r--r--   0        0        0     5136 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/psm.sql
--rw-r--r--   0        0        0     7541 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/count.sql.jinja
--rw-r--r--   0        0        0     2311 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/counts_templates.py
--rw-r--r--   0        0        0     1606 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/psm_create_covariate_table.sql.jinja
--rw-r--r--   0        0        0      363 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/psm_distinct_ids.sql.jinja
--rw-r--r--   0        0        0     3272 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/psm_templates.py
--rw-r--r--   0        0        0     3603 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_condition.py
--rw-r--r--   0        0        0     2789 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_documentreference.py
--rw-r--r--   0        0        0     4676 2024-05-09 13:20:56.629008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_encounter.py
--rw-r--r--   0        0        0     2422 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_medication.py
--rw-r--r--   0        0        0     1853 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_medicationrequest.py
--rw-r--r--   0        0        0     3772 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_observation.py
--rw-r--r--   0        0        0     3098 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_patient.py
--rw-r--r--   0        0        0      867 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/builder_prereq_tables.py
--rw-r--r--   0        0        0     2555 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/completion_utils.jinja
--rw-r--r--   0        0        0     2400 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/condition.sql.jinja
--rw-r--r--   0        0        0      418 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/core_templates.py
--rw-r--r--   0        0        0     4999 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/core_utils.jinja
--rw-r--r--   0        0        0     2829 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/documentreference.sql.jinja
--rw-r--r--   0        0        0     4804 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/encounter.sql.jinja
--rw-r--r--   0        0        0      274 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/incomplete_encounter.sql.jinja
--rw-r--r--   0        0        0     2841 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/medication.sql.jinja
--rw-r--r--   0        0        0     2422 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/medicationrequest.sql.jinja
--rw-r--r--   0        0        0     3324 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/observation.sql.jinja
--rw-r--r--   0        0        0     2081 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/observation_component_valuequantity.sql.jinja
--rw-r--r--   0        0        0     1854 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/patient.sql.jinja
--rw-r--r--   0        0        0     5350 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/count_core.py
--rw-r--r--   0        0        0      948 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/fhir_lookup_tables.sql
--rw-r--r--   0        0        0     4879 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/fhir_mapping_tables.sql
--rw-r--r--   0        0        0      971 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/manifest.toml
--rw-r--r--   0        0        0     1744 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/observation_type.sql
--rw-r--r--   0        0        0    12183 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_condition.sql
--rw-r--r--   0        0        0     5610 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_documentreference.sql
--rw-r--r--   0        0        0    21826 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_encounter.sql
--rw-r--r--   0        0        0     3949 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_medication.sql
--rw-r--r--   0        0        0     3017 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_medicationrequest.sql
--rw-r--r--   0        0        0    11183 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_observation.sql
--rw-r--r--   0        0        0     7061 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_patient.sql
--rw-r--r--   0        0        0     8008 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_prereq_tables.sql
--rw-r--r--   0        0        0    29070 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/count_core.sql
--rw-r--r--   0        0        0     1440 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/setup.sql
--rw-r--r--   0        0        0     2058 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/study_period.sql
--rw-r--r--   0        0        0       69 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/core/version.sql
--rw-r--r--   0        0        0     2743 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/discovery/code_definitions.py
--rw-r--r--   0        0        0     2762 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/discovery/code_detection.py
--rw-r--r--   0        0        0     1978 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/discovery/discovery_templates/code_system_pairs.sql.jinja
--rw-r--r--   0        0        0     1618 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/discovery/discovery_templates/discovery_templates.py
--rw-r--r--   0        0        0      160 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/discovery/manifest.toml
--rw-r--r--   0        0        0     4622 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/discovery/reference_sql/code_detection.sql
--rw-r--r--   0        0        0      863 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/template/counts.sql
--rw-r--r--   0        0        0      187 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/template/date_range.sql
--rw-r--r--   0        0        0      566 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/template/lab_observations.sql
--rw-r--r--   0        0        0     2312 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/template/manifest.toml
--rw-r--r--   0        0        0     1142 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/template/setup.sql
--rw-r--r--   0        0        0       14 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/vocab/.gitignore
--rw-r--r--   0        0        0      253 2024-05-09 13:20:56.633008 cumulus_library-2.1.0/cumulus_library/studies/vocab/README.MD
--rw-r--r--   0        0        0 10584966 2024-05-09 13:20:56.661008 cumulus_library-2.1.0/cumulus_library/studies/vocab/icd/ICD10CM_2023AA.bsv
--rw-r--r--   0        0        0 35303095 2024-05-09 13:20:56.745009 cumulus_library-2.1.0/cumulus_library/studies/vocab/icd/ICD10PCS_2023AA.bsv
--rw-r--r--   0        0        0  1708185 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/studies/vocab/icd/ICD9CM_2023AA.bsv
--rw-r--r--   0        0        0      410 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/studies/vocab/icd_legend.sql
--rw-r--r--   0        0        0      269 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/studies/vocab/manifest.toml
--rw-r--r--   0        0        0      681 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/studies/vocab/reference_sql/vocab_icd_builder.sql
--rw-r--r--   0        0        0     2366 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/studies/vocab/vocab_icd_builder.py
--rw-r--r--   0        0        0    32529 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/study_parser.py
--rw-r--r--   0        0        0       79 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/alias_table.sql.jinja
--rw-r--r--   0        0        0    13075 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/base_templates.py
--rw-r--r--   0        0        0     4423 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
--rw-r--r--   0        0        0     1893 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/coding_denormalize.sql.jinja
--rw-r--r--   0        0        0      385 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/column_datatype.sql.jinja
--rw-r--r--   0        0        0      563 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/create_view_as.sql.jinja
--rw-r--r--   0        0        0      586 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/ctas.sql.jinja
--rw-r--r--   0        0        0      544 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/ctas_empty.sql.jinja
--rw-r--r--   0        0        0      954 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/ctas_from_parquet.sql.jinja
--rw-r--r--   0        0        0       61 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/drop_view_table.sql.jinja
--rw-r--r--   0        0        0     2528 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/extension_denormalize.sql.jinja
--rw-r--r--   0        0        0      535 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/insert_into.sql.jinja
--rw-r--r--   0        0        0      439 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/is_table_not_empty.sql.jinja
--rw-r--r--   0        0        0       34 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/select_all.sql.jinja
--rw-r--r--   0        0        0      370 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/shared_macros/syntax.sql.jinja
--rw-r--r--   0        0        0     1108 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/shared_macros/unnest_utils.jinja
--rw-r--r--   0        0        0      169 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/show_tables.sql.jinja
--rw-r--r--   0        0        0      163 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/show_views.sql.jinja
--rw-r--r--   0        0        0    12401 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/template_sql/sql_utils.py
--rw-r--r--   0        0        0     3261 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/cumulus_library/upload.py
--rw-r--r--   0        0        0     2313 2024-05-09 13:20:56.753009 cumulus_library-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     2142 1970-01-01 00:00:00.000000 cumulus_library-2.1.0/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2024-05-16 17:25:51.340991 cumulus_library-2.2.0/.sqlfluff -> cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0      689 2024-05-16 17:25:51.340991 cumulus_library-2.2.0/README.md
+-rw-r--r--   0        0        0     7061 2024-05-16 17:25:51.340991 cumulus_library-2.2.0/cumulus_library/.sqlfluff
+-rw-r--r--   0        0        0       46 2024-05-16 17:25:51.340991 cumulus_library-2.2.0/cumulus_library/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 17:25:51.340991 cumulus_library-2.2.0/cumulus_library/apis/__init__.py
+-rw-r--r--   0        0        0     6323 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/apis/umls.py
+-rw-r--r--   0        0        0     4835 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/base_table_builder.py
+-rw-r--r--   0        0        0     3890 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/base_utils.py
+-rwxr-xr-x   0        0        0    18530 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/cli.py
+-rw-r--r--   0        0        0     8187 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/cli_parser.py
+-rw-r--r--   0        0        0    21845 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/databases.py
+-rw-r--r--   0        0        0      249 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/db_config.py
+-rw-r--r--   0        0        0      420 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/enums.py
+-rw-r--r--   0        0        0      665 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/errors.py
+-rw-r--r--   0        0        0      300 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/module_allowlist.json
+-rw-r--r--   0        0        0     2311 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/parsers/fhir_valueset.py
+-rw-r--r--   0        0        0     1715 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/protected_table_builder.py
+-rw-r--r--   0        0        0        0 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/schema/__init__.py
+-rw-r--r--   0        0        0     4731 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/schema/columns.py
+-rw-r--r--   0        0        0     3364 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/schema/typesystem.py
+-rw-r--r--   0        0        0     6024 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/schema/valueset.py
+-rw-r--r--   0        0        0    10732 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/statistics/counts.py
+-rw-r--r--   0        0        0    14453 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/statistics/psm.py
+-rw-r--r--   0        0        0     5136 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/statistics/psm.sql
+-rw-r--r--   0        0        0     7541 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/statistics/statistics_templates/count.sql.jinja
+-rw-r--r--   0        0        0     2311 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/statistics/statistics_templates/counts_templates.py
+-rw-r--r--   0        0        0     1606 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/statistics/statistics_templates/psm_create_covariate_table.sql.jinja
+-rw-r--r--   0        0        0      363 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/statistics/statistics_templates/psm_distinct_ids.sql.jinja
+-rw-r--r--   0        0        0     3270 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/statistics/statistics_templates/psm_templates.py
+-rw-r--r--   0        0        0     3515 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/builder_condition.py
+-rw-r--r--   0        0        0     2664 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/builder_documentreference.py
+-rw-r--r--   0        0        0     4478 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/builder_encounter.py
+-rw-r--r--   0        0        0     2173 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/builder_medication.py
+-rw-r--r--   0        0        0     1663 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/builder_medicationrequest.py
+-rw-r--r--   0        0        0     3582 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/builder_observation.py
+-rw-r--r--   0        0        0     2827 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/builder_patient.py
+-rw-r--r--   0        0        0      865 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/builder_prereq_tables.py
+-rw-r--r--   0        0        0     2555 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/completion_utils.jinja
+-rw-r--r--   0        0        0     2400 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/condition.sql.jinja
+-rw-r--r--   0        0        0      418 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/core_templates.py
+-rw-r--r--   0        0        0     4999 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/core_utils.jinja
+-rw-r--r--   0        0        0     2829 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/documentreference.sql.jinja
+-rw-r--r--   0        0        0     4804 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/encounter.sql.jinja
+-rw-r--r--   0        0        0      274 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/incomplete_encounter.sql.jinja
+-rw-r--r--   0        0        0     2918 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/medication.sql.jinja
+-rw-r--r--   0        0        0     2422 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/medicationrequest.sql.jinja
+-rw-r--r--   0        0        0     3324 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/observation.sql.jinja
+-rw-r--r--   0        0        0     2080 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/observation_component_valuequantity.sql.jinja
+-rw-r--r--   0        0        0     1854 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/patient.sql.jinja
+-rw-r--r--   0        0        0     5350 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/count_core.py
+-rw-r--r--   0        0        0      948 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/fhir_lookup_tables.sql
+-rw-r--r--   0        0        0     4879 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/fhir_mapping_tables.sql
+-rw-r--r--   0        0        0      971 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/manifest.toml
+-rw-r--r--   0        0        0     1744 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/observation_type.sql
+-rw-r--r--   0        0        0    12295 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_condition.sql
+-rw-r--r--   0        0        0     5620 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_documentreference.sql
+-rw-r--r--   0        0        0    22038 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_encounter.sql
+-rw-r--r--   0        0        0     3989 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_medication.sql
+-rw-r--r--   0        0        0     3017 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_medicationrequest.sql
+-rw-r--r--   0        0        0    11183 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_observation.sql
+-rw-r--r--   0        0        0     7061 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_patient.sql
+-rw-r--r--   0        0        0     8008 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_prereq_tables.sql
+-rw-r--r--   0        0        0    29070 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/count_core.sql
+-rw-r--r--   0        0        0     1440 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/setup.sql
+-rw-r--r--   0        0        0     2058 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/study_period.sql
+-rw-r--r--   0        0        0       69 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/core/version.sql
+-rw-r--r--   0        0        0     2743 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/discovery/code_definitions.py
+-rw-r--r--   0        0        0     2492 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/discovery/code_detection.py
+-rw-r--r--   0        0        0     1978 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/discovery/discovery_templates/code_system_pairs.sql.jinja
+-rw-r--r--   0        0        0     1618 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/discovery/discovery_templates/discovery_templates.py
+-rw-r--r--   0        0        0      160 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/discovery/manifest.toml
+-rw-r--r--   0        0        0     4622 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/discovery/reference_sql/code_detection.sql
+-rw-r--r--   0        0        0      863 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/template/counts.sql
+-rw-r--r--   0        0        0      187 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/template/date_range.sql
+-rw-r--r--   0        0        0      566 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/template/lab_observations.sql
+-rw-r--r--   0        0        0     2312 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/template/manifest.toml
+-rw-r--r--   0        0        0     1142 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/template/setup.sql
+-rw-r--r--   0        0        0       14 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/vocab/.gitignore
+-rw-r--r--   0        0        0      253 2024-05-16 17:25:51.344991 cumulus_library-2.2.0/cumulus_library/studies/vocab/README.MD
+-rw-r--r--   0        0        0 10584966 2024-05-16 17:25:51.376991 cumulus_library-2.2.0/cumulus_library/studies/vocab/icd/ICD10CM_2023AA.bsv
+-rw-r--r--   0        0        0 35303095 2024-05-16 17:25:51.460991 cumulus_library-2.2.0/cumulus_library/studies/vocab/icd/ICD10PCS_2023AA.bsv
+-rw-r--r--   0        0        0  1708185 2024-05-16 17:25:51.464991 cumulus_library-2.2.0/cumulus_library/studies/vocab/icd/ICD9CM_2023AA.bsv
+-rw-r--r--   0        0        0      410 2024-05-16 17:25:51.464991 cumulus_library-2.2.0/cumulus_library/studies/vocab/icd_legend.sql
+-rw-r--r--   0        0        0      269 2024-05-16 17:25:51.464991 cumulus_library-2.2.0/cumulus_library/studies/vocab/manifest.toml
+-rw-r--r--   0        0        0      681 2024-05-16 17:25:51.464991 cumulus_library-2.2.0/cumulus_library/studies/vocab/reference_sql/vocab_icd_builder.sql
+-rw-r--r--   0        0        0     2364 2024-05-16 17:25:51.464991 cumulus_library-2.2.0/cumulus_library/studies/vocab/vocab_icd_builder.py
+-rw-r--r--   0        0        0    33198 2024-05-16 17:25:51.464991 cumulus_library-2.2.0/cumulus_library/study_parser.py
+-rw-r--r--   0        0        0       79 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/alias_table.sql.jinja
+-rw-r--r--   0        0        0    13073 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/base_templates.py
+-rw-r--r--   0        0        0     4432 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja
+-rw-r--r--   0        0        0     1904 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/coding_denormalize.sql.jinja
+-rw-r--r--   0        0        0      385 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/column_datatype.sql.jinja
+-rw-r--r--   0        0        0      563 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/create_view_as.sql.jinja
+-rw-r--r--   0        0        0      586 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/ctas.sql.jinja
+-rw-r--r--   0        0        0      544 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/ctas_empty.sql.jinja
+-rw-r--r--   0        0        0      954 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/ctas_from_parquet.sql.jinja
+-rw-r--r--   0        0        0       61 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/drop_view_table.sql.jinja
+-rw-r--r--   0        0        0     2528 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/extension_denormalize.sql.jinja
+-rw-r--r--   0        0        0      535 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/insert_into.sql.jinja
+-rw-r--r--   0        0        0      439 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/is_table_not_empty.sql.jinja
+-rw-r--r--   0        0        0       34 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/select_all.sql.jinja
+-rw-r--r--   0        0        0     1400 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/shared_macros/syntax.sql.jinja
+-rw-r--r--   0        0        0     1108 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/shared_macros/unnest_utils.jinja
+-rw-r--r--   0        0        0      225 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/show_tables.sql.jinja
+-rw-r--r--   0        0        0      220 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/show_views.sql.jinja
+-rw-r--r--   0        0        0    12166 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/template_sql/sql_utils.py
+-rw-r--r--   0        0        0     3260 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/cumulus_library/upload.py
+-rw-r--r--   0        0        0     2298 2024-05-16 17:25:51.468991 cumulus_library-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2091 1970-01-01 00:00:00.000000 cumulus_library-2.2.0/PKG-INFO
```

### Comparing `cumulus_library-2.1.0/README.md` & `cumulus_library-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/.sqlfluff` & `cumulus_library-2.2.0/cumulus_library/.sqlfluff`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/apis/umls.py` & `cumulus_library-2.2.0/cumulus_library/apis/umls.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Class for communicating with the umls API"""
+
 import os
 import pathlib
 
 import requests
 
 from cumulus_library import base_utils, errors
```

### Comparing `cumulus_library-2.1.0/cumulus_library/base_table_builder.py` & `cumulus_library-2.2.0/cumulus_library/base_table_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" abstract base for python-based study executors """
+"""abstract base for python-based study executors"""
 
 import pathlib
 import re
 import sys
 from abc import ABC, abstractmethod
 from typing import final
```

### Comparing `cumulus_library-2.1.0/cumulus_library/base_utils.py` & `cumulus_library-2.2.0/cumulus_library/base_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Collection of small commonly used utility functions """
+"""Collection of small commonly used utility functions"""
 
 import dataclasses
 import datetime
 import json
 import pathlib
 import shutil
 import zipfile
```

### Comparing `cumulus_library-2.1.0/cumulus_library/cli.py` & `cumulus_library-2.2.0/cumulus_library/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,15 +176,15 @@
         :param config: A StudyConfig object containing optional params
         """
         studyparser = study_parser.StudyManifestParser(target)
         studyparser.run_matching_table_builder(
             self.cursor,
             self.schema_name,
             table_builder_name,
-            self.verbose,
+            verbose=self.verbose,
             parser=self.db.parser(),
             config=config,
         )
 
     def clean_and_build_all(
         self, study_dict: dict, config: base_utils.StudyConfig
     ) -> None:
@@ -314,22 +314,26 @@
         paths = paths + alt_dir_paths
     for path in paths:
         found_studies = get_studies_by_manifest_path(path)
         manifest_studies.update(found_studies)
     return manifest_studies
 
 
-def get_studies_by_manifest_path(path: pathlib.Path) -> dict:
+def get_studies_by_manifest_path(path: pathlib.Path) -> dict[str, pathlib.Path]:
     """Recursively search for manifest.toml files from a given path"""
     manifest_paths = {}
     for child_path in path.iterdir():
         if child_path.is_dir():
             manifest_paths.update(get_studies_by_manifest_path(child_path))
         elif child_path.name == "manifest.toml":
-            manifest_paths[path.name] = path
+            try:
+                manifest = study_parser.StudyManifestParser(path)
+                manifest_paths[manifest.get_study_prefix()] = path
+            except errors.StudyManifestParsingError as exc:
+                rich.print(f"[bold red] Ignoring study in '{path}': {exc}")
     return manifest_paths
 
 
 def run_cli(args: dict):
     """Controls which library tasks are run based on CLI arguments"""
     console = rich.console.Console()
     if args["action"] == "create":
@@ -344,15 +348,15 @@
 
     # all other actions require connecting to the database
     else:
         config = base_utils.StudyConfig(
             db=databases.create_db_backend(args),
             force_upload=args.get("replace_existing", False),
             stats_build=args.get("stats_build", False),
-            umls_key=args.get("umls"),
+            umls_key=args.get("umls_key"),
         )
         try:
             runner = StudyRunner(config.db, data_path=args.get("data_path"))
             if args.get("verbose"):
                 runner.verbose = True
             console.print("[italic] Connecting to database...")
             runner.cursor.execute("SHOW DATABASES")
@@ -361,15 +365,15 @@
                 if args["target"]:
                     for target in args["target"]:
                         if target not in study_dict:
                             sys.exit(
                                 f"{target} was not found in available studies: "
                                 f"{list(study_dict.keys())}.\n\n"
                                 "If you are trying to run a custom study, make sure "
-                                "you include `-s path/to/study/dir` as an arugment."
+                                "you include `-s path/to/study/dir` as an argument."
                             )
             if args["action"] == "clean":
                 runner.clean_study(
                     args["target"],
                     study_dict,
                     stats_clean=args["stats_clean"],
                     prefix=args["prefix"],
@@ -377,15 +381,15 @@
             elif args["action"] == "build":
                 if "all" in args["target"]:
                     runner.clean_and_build_all(study_dict, config=config)
                 else:
                     for target in args["target"]:
                         if args["builder"]:
                             runner.run_matching_table_builder(
-                                study_dict[target], config=config
+                                study_dict[target], args["builder"], config=config
                             )
                         else:
                             runner.clean_and_build_study(
                                 study_dict[target],
                                 config=config,
                             )
 
@@ -448,15 +452,15 @@
         ("db_type", "CUMULUS_LIBRARY_DB_TYPE"),
         ("id", "CUMULUS_AGGREGATOR_ID"),
         ("load_ndjson_dir", "CUMULUS_LIBRARY_LOAD_NDJSON_DIR"),
         ("profile", "CUMULUS_LIBRARY_PROFILE"),
         ("region", "CUMULUS_LIBRARY_REGION"),
         ("schema_name", "CUMULUS_LIBRARY_DATABASE"),
         ("study_dir", "CUMULUS_LIBRARY_STUDY_DIR"),
-        ("umls", "UMLS_API_KEY"),
+        ("umls_key", "UMLS_API_KEY"),
         ("url", "CUMULUS_AGGREGATOR_URL"),
         ("user", "CUMULUS_AGGREGATOR_USER"),
         ("workgroup", "CUMULUS_LIBRARY_WORKGROUP"),
     )
     read_env_vars = []
     for pair in arg_env_pairs:
         if env_val := os.environ.get(pair[1]):
```

### Comparing `cumulus_library-2.1.0/cumulus_library/cli_parser.py` & `cumulus_library-2.2.0/cumulus_library/cli_parser.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/databases.py` & `cumulus_library-2.2.0/cumulus_library/databases.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 """
 
 import abc
 import datetime
 import json
 import os
 import pathlib
+import re
 import sys
 from pathlib import Path
 from typing import Any, Protocol
 
 import boto3
 import cumulus_fhir_support
 import duckdb
@@ -152,14 +153,25 @@
     def execute_as_pandas(self, sql: str) -> pandas.DataFrame:
         """Returns a pandas.DataFrame version of the results from the provided SQL"""
 
     @abc.abstractmethod
     def parser(self) -> DatabaseParser:
         """Returns parser object for interrogating DB schemas"""
 
+    def operational_errors(self) -> tuple[Exception]:
+        """Returns a tuple of operational exception classes
+
+        An operational error is something that went wrong while performing a database
+        query. So something like "table doesn't exist" but not like a network or
+        syntax error.
+
+        This is designed to be used in an `except` clause.
+        """
+        return ()
+
     def upload_file(
         self,
         *,
         file: pathlib.Path,
         study: str,
         topic: str,
         remote_filename: str | None = None,
@@ -215,14 +227,17 @@
 
     def execute_as_pandas(self, sql: str) -> pandas.DataFrame:
         return self.pandas_cursor().execute(sql).as_pandas()
 
     def parser(self) -> DatabaseParser:
         return AthenaParser()
 
+    def operational_errors(self) -> tuple[Exception]:
+        return (pyathena.OperationalError,)
+
     def upload_file(
         self,
         *,
         file: pathlib.Path,
         study: str,
         topic: str,
         remote_filename: str | None = None,
@@ -338,14 +353,21 @@
             # DuckDB's version is array_to_string -- seems there is no standard here.
             "array_join",
             self._compat_array_join,
             None,
             duckdb.typing.VARCHAR,
         )
         self.connection.create_function(
+            # DuckDB's version is regexp_matches.
+            "regexp_like",
+            self._compat_regexp_like,
+            None,
+            duckdb.typing.BOOLEAN,
+        )
+        self.connection.create_function(
             # We frequently use Athena's date() function because it's easier than
             # the more widely-supported way of CAST(x AS DATE).
             # Rather than convert all of our SQL to the longer version,
             # we'll just make our own version of date().
             "date",
             self._compat_date,
             None,
@@ -390,14 +412,21 @@
         value: list[str | None] | None, delimiter: str
     ) -> str | None:
         if value is None:
             return None
         return delimiter.join(v for v in value if v is not None)
 
     @staticmethod
+    def _compat_regexp_like(string: str | None, pattern: str | None) -> bool:
+        if string is None or pattern is None:
+            return None
+        match = re.search(pattern, string)
+        return match is not None
+
+    @staticmethod
     def _compat_date(
         value: str | datetime.datetime | datetime.date | None,
     ) -> datetime.date | None:
         if value is None:
             return None
         elif isinstance(value, str):
             return datetime.date.fromisoformat(value)
@@ -450,14 +479,17 @@
         # we call this to convert to its nullable int column type.
         # PyAthena seems to do this correctly for us, but not DuckDB.
         return self.connection.execute(sql).df().convert_dtypes()
 
     def parser(self) -> DatabaseParser:
         return DuckDbParser()
 
+    def operational_errors(self) -> tuple[Exception]:
+        return (duckdb.OperationalError,)
+
     def close(self) -> None:
         self.connection.close()
 
 
 class DuckDbParser(DatabaseParser):
     """Table parser for DuckDB schemas"""
```

### Comparing `cumulus_library-2.1.0/cumulus_library/errors.py` & `cumulus_library-2.2.0/cumulus_library/errors.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/parsers/fhir_valueset.py` & `cumulus_library-2.2.0/cumulus_library/parsers/fhir_valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/protected_table_builder.py` & `cumulus_library-2.2.0/cumulus_library/protected_table_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Builder for creating tables for tracking state/logging changes"""
+"""Builder for creating tables for tracking state/logging changes"""
 
 from cumulus_library import base_table_builder, enums
 from cumulus_library.template_sql import base_templates
 
 TRANSACTIONS_COLS = ["study_name", "library_version", "status", "event_time"]
 TRANSACTION_COLS_TYPES = ["varchar", "varchar", "varchar", "timestamp"]
 # while it may seem redundant, study_name and view_name are included as a column for
```

### Comparing `cumulus_library-2.1.0/cumulus_library/schema/columns.py` & `cumulus_library-2.2.0/cumulus_library/schema/columns.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/schema/typesystem.py` & `cumulus_library-2.2.0/cumulus_library/schema/typesystem.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/schema/valueset.py` & `cumulus_library-2.2.0/cumulus_library/schema/valueset.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/statistics/counts.py` & `cumulus_library-2.2.0/cumulus_library/statistics/counts.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/statistics/psm.py` & `cumulus_library-2.2.0/cumulus_library/statistics/psm.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/statistics/psm.sql` & `cumulus_library-2.2.0/cumulus_library/statistics/psm.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/count.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/statistics/statistics_templates/count.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/counts_templates.py` & `cumulus_library-2.2.0/cumulus_library/statistics/statistics_templates/counts_templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/psm_create_covariate_table.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/statistics/statistics_templates/psm_create_covariate_table.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/statistics/statistics_templates/psm_templates.py` & `cumulus_library-2.2.0/cumulus_library/statistics/statistics_templates/psm_templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Collection of jinja template getters for common SQL queries """
+"""Collection of jinja template getters for common SQL queries"""
 
 from pathlib import Path
 
 from cumulus_library.errors import CumulusLibraryError
 from cumulus_library.template_sql import base_templates
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/builder_condition.py` & `cumulus_library-2.2.0/cumulus_library/studies/core/builder_condition.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cumulus_library import base_table_builder, databases
+from cumulus_library import base_table_builder, base_utils
 from cumulus_library.studies.core.core_templates import core_templates
 from cumulus_library.template_sql import base_templates, sql_utils
 
 expected_table_cols = {
     "condition": {
         "id": [],
         "recordedDate": [],
@@ -71,20 +71,16 @@
         self.queries += [
             base_templates.get_codeable_concept_denormalize_query(config)
             for config in configs
         ]
 
     def prepare_queries(
         self,
-        cursor: object,
-        schema: str,
         *args,
-        parser: databases.DatabaseParser = None,
+        config: base_utils.StudyConfig,
         **kwargs,
     ):
         self.denormalize_codes()
-        validated_schema = sql_utils.validate_schema(
-            cursor, schema, expected_table_cols, parser
-        )
+        validated_schema = sql_utils.validate_schema(config.db, expected_table_cols)
         self.queries.append(
             core_templates.get_core_template("condition", validated_schema)
         )
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/builder_documentreference.py` & `cumulus_library-2.2.0/cumulus_library/studies/core/builder_documentreference.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from cumulus_library import base_table_builder, databases
+from cumulus_library import base_table_builder, base_utils
 from cumulus_library.studies.core.core_templates import core_templates
 from cumulus_library.template_sql import sql_utils
 
 expected_table_cols = {
     "documentreference": {
         "id": [],
         "status": [],
@@ -15,24 +15,20 @@
 
 
 class CoreDocumentreferenceBuilder(base_table_builder.BaseTableBuilder):
     display_text = "Creating DocumentReference tables..."
 
     def prepare_queries(
         self,
-        cursor: object,
-        schema: str,
         *args,
-        parser: databases.DatabaseParser = None,
+        config: base_utils.StudyConfig,
         **kwargs,
     ):
         self.queries = sql_utils.denormalize_complex_objects(
-            schema,
-            cursor,
-            parser,
+            config.db,
             [
                 sql_utils.CodeableConceptConfig(
                     source_table="documentreference",
                     source_id="id",
                     column_hierarchy=[("type", dict)],
                     target_table="core__documentreference_dn_type",
                 ),
@@ -58,13 +54,11 @@
                     source_id="id",
                     column_hierarchy=[("content", list), ("format", dict)],
                     target_table="core__documentreference_dn_format",
                     expected={"format": sql_utils.CODING},
                 ),
             ],
         )
-        validated_schema = sql_utils.validate_schema(
-            cursor, schema, expected_table_cols, parser
-        )
+        validated_schema = sql_utils.validate_schema(config.db, expected_table_cols)
         self.queries.append(
             core_templates.get_core_template("documentreference", validated_schema)
         )
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/builder_encounter.py` & `cumulus_library-2.2.0/cumulus_library/studies/core/builder_encounter.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from dataclasses import dataclass
 
-from cumulus_library import base_table_builder, databases
+from cumulus_library import base_table_builder, base_utils
 from cumulus_library.studies.core.core_templates import core_templates
 from cumulus_library.template_sql import sql_utils
 
 expected_table_cols = {
     "encounter": {
         "id": [],
         "status": [],
@@ -33,15 +33,15 @@
     def __post_init__(self):
         self.target_table = f"core__encounter_dn_{self.column_hierarchy[-1][0]}"
 
 
 class CoreEncounterBuilder(base_table_builder.BaseTableBuilder):
     display_text = "Creating Encounter tables..."
 
-    def denormalize_codes(self, schema, cursor, parser):
+    def denormalize_codes(self, database):
         code_configs = [
             EncConfig(
                 column_hierarchy=[("type", list)],
                 filter_priority=True,
                 code_systems=[
                     "http://terminology.hl7.org/CodeSystem/encounter-type",
                     "http://terminology.hl7.org/CodeSystem/v2-0004",
@@ -99,31 +99,21 @@
                 column_hierarchy=[
                     ("hospitalization", dict),
                     ("dischargedisposition", dict),
                 ],
                 expected={"dischargedisposition": sql_utils.CODEABLE_CONCEPT},
             ),
         ]
-        self.queries += sql_utils.denormalize_complex_objects(
-            schema, cursor, parser, code_configs
-        )
+        self.queries += sql_utils.denormalize_complex_objects(database, code_configs)
 
     def prepare_queries(
         self,
-        cursor: object,
-        schema: str,
         *args,
-        parser: databases.DatabaseParser = None,
+        config: base_utils.StudyConfig,
         **kwargs,
     ):
-        self.denormalize_codes(
-            schema,
-            cursor,
-            parser,
-        )
-        validated_schema = sql_utils.validate_schema(
-            cursor, schema, expected_table_cols, parser
-        )
+        self.denormalize_codes(config.db)
+        validated_schema = sql_utils.validate_schema(config.db, expected_table_cols)
         self.queries += [
             core_templates.get_core_template("encounter", validated_schema),
             core_templates.get_core_template("incomplete_encounter", validated_schema),
         ]
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/builder_medication.py` & `cumulus_library-2.2.0/cumulus_library/studies/core/builder_medication.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-""" Module for generating core medication table"""
+"""Module for generating core medication table"""
 
-from cumulus_library import base_table_builder, databases
+from cumulus_library import base_table_builder, base_utils
 from cumulus_library.studies.core.core_templates import core_templates
 from cumulus_library.template_sql import sql_utils
 
 expected_table_cols = {
     "medicationrequest": {
         "id": [],
         "subject": sql_utils.REFERENCE,
@@ -15,25 +15,21 @@
 
 
 class MedicationBuilder(base_table_builder.BaseTableBuilder):
     display_text = "Creating Medication table..."
 
     def prepare_queries(
         self,
-        cursor: databases.DatabaseCursor,
-        schema: str,
-        parser: databases.DatabaseParser = None,
         *args,
+        config: base_utils.StudyConfig,
         **kwargs,
     ) -> None:
         """Constructs queries related to condition codeableConcept
 
-        :param cursor: A database cursor object
-        :param schema: the schema/db name, matching the cursor
-        :param parser: A database parser
+        :param config: A study config object
         """
         code_sources = [
             sql_utils.CodeableConceptConfig(
                 source_table="medication",
                 column_hierarchy=[("code", dict)],
                 target_table="core__medication_dn_code",
             ),
@@ -53,16 +49,12 @@
                 },
                 extra_fields=[
                     ("id", "contained_id"),
                     ("resourceType", "resource_type"),
                 ],
             ),
         ]
-        self.queries += sql_utils.denormalize_complex_objects(
-            schema, cursor, parser, code_sources
-        )
-        validated_schema = sql_utils.validate_schema(
-            cursor, schema, expected_table_cols, parser
-        )
+        self.queries += sql_utils.denormalize_complex_objects(config.db, code_sources)
+        validated_schema = sql_utils.validate_schema(config.db, expected_table_cols)
         self.queries += [
             core_templates.get_core_template("medication", validated_schema),
         ]
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/builder_medicationrequest.py` & `cumulus_library-2.2.0/cumulus_library/studies/core/builder_medicationrequest.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,13 +1,13 @@
-""" Module for extracting US core extensions from medicationrequests
+"""Module for extracting US core extensions from medicationrequests
 
 Note: This module assumes that you have already run builder_medication,
 as it leverages the core__medication table for data population"""
 
-from cumulus_library import base_table_builder, databases
+from cumulus_library import base_table_builder, base_utils
 from cumulus_library.studies.core.core_templates import core_templates
 from cumulus_library.template_sql import sql_utils
 
 expected_table_cols = {
     "medicationrequest": {
         "id": [],
         "status": [],
@@ -22,35 +22,28 @@
 
 
 class MedicationRequestBuilder(base_table_builder.BaseTableBuilder):
     display_text = "Creating MedicationRequest tables..."
 
     def prepare_queries(
         self,
-        cursor: object,
-        schema: str,
         *args,
-        parser: databases.DatabaseParser = None,
+        config: base_utils.StudyConfig,
         **kwargs,
     ):
         """constructs queries related to patient extensions of interest
 
-        :param cursor: A database cursor object
-        :param schema: the schema/db name, matching the cursor
+        :param config: A study config object
         """
         code_sources = [
             sql_utils.CodeableConceptConfig(
                 source_table="medicationrequest",
                 source_id="id",
                 column_hierarchy=[("category", list)],
                 target_table="core__medicationrequest_dn_category",
             ),
         ]
-        self.queries += sql_utils.denormalize_complex_objects(
-            schema, cursor, parser, code_sources
-        )
-        validated_schema = sql_utils.validate_schema(
-            cursor, schema, expected_table_cols, parser
-        )
+        self.queries += sql_utils.denormalize_complex_objects(config.db, code_sources)
+        validated_schema = sql_utils.validate_schema(config.db, expected_table_cols)
         self.queries.append(
             core_templates.get_core_template("medicationrequest", validated_schema)
         )
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/builder_observation.py` & `cumulus_library-2.2.0/cumulus_library/studies/core/builder_observation.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-""" Module for extracting US core extensions from patient records"""
+"""Module for extracting US core extensions from patient records"""
 
 from dataclasses import dataclass
 
-from cumulus_library import base_table_builder, databases
+from cumulus_library import base_table_builder, base_utils
 from cumulus_library.studies.core.core_templates import core_templates
 from cumulus_library.template_sql import sql_utils
 
 expected_table_cols = {
     "observation": {
         "id": [],
         "component": {
@@ -37,24 +37,21 @@
 
 
 class ObservationBuilder(base_table_builder.BaseTableBuilder):
     display_text = "Creating Observation tables..."
 
     def prepare_queries(
         self,
-        cursor: object,
-        schema: str,
         *args,
-        parser: databases.DatabaseParser = None,
+        config: base_utils.StudyConfig,
         **kwargs,
     ):
         """constructs queries related to patient extensions of interest
 
-        :param cursor: A database cursor object
-        :param schema: the schema/db name, matching the cursor
+        :param config: A study config object
         """
         code_sources = [
             ObsConfig(column_hierarchy=[("category", list)], filter_priority=False),
             ObsConfig(column_hierarchy=[("code", dict)], filter_priority=False),
             ObsConfig(
                 is_public=True,
                 column_hierarchy=[("component", list), ("code", dict)],
@@ -84,19 +81,15 @@
             ),
             ObsConfig(
                 column_hierarchy=[("dataabsentreason", dict)],
                 filter_priority=False,
             ),
         ]
 
-        self.queries += sql_utils.denormalize_complex_objects(
-            schema, cursor, parser, code_sources
-        )
-        validated_schema = sql_utils.validate_schema(
-            cursor, schema, expected_table_cols, parser
-        )
+        self.queries += sql_utils.denormalize_complex_objects(config.db, code_sources)
+        validated_schema = sql_utils.validate_schema(config.db, expected_table_cols)
         self.queries += [
             core_templates.get_core_template("observation", validated_schema),
             core_templates.get_core_template(
                 "observation_component_valuequantity", validated_schema
             ),
         ]
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/builder_patient.py` & `cumulus_library-2.2.0/cumulus_library/studies/core/builder_patient.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-""" Module for extracting US core extensions from patient records"""
+"""Module for extracting US core extensions from patient records"""
 
-from cumulus_library import databases
+from cumulus_library import base_utils, databases
 from cumulus_library.base_table_builder import BaseTableBuilder
 from cumulus_library.studies.core.core_templates import core_templates
 from cumulus_library.template_sql import base_templates, sql_utils
 
 expected_table_cols = {
     "patient": {
         "id": [],
@@ -16,24 +16,20 @@
 
 
 class PatientBuilder(BaseTableBuilder):
     display_text = "Creating Patient tables..."
 
     @staticmethod
     def make_extension_query(
-        schema: str,
-        cursor: databases.DatabaseCursor,
-        parser: databases.DatabaseParser,
+        database: databases.DatabaseBackend,
         name: str,
         url: str,
     ) -> str:
         has_extensions = sql_utils.is_field_present(
-            schema=schema,
-            cursor=cursor,
-            parser=parser,
+            database=database,
             source_table="patient",
             source_col="extension",
             expected={
                 "extension": {
                     "url": {},
                     "valueCoding": sql_utils.CODING,
                 },
@@ -49,48 +45,43 @@
                 fhir_extension=url,
                 ext_systems=["ombCategory", "detailed"],
                 is_array=True,
             )
             return base_templates.get_extension_denormalize_query(config)
         else:
             return base_templates.get_ctas_empty_query(
-                schema_name=schema,
+                schema_name=database.schema_name,
                 table_name=f"core__patient_ext_{name}",
                 table_cols=["id", "system", f"{name}_code", f"{name}_display"],
             )
 
     def prepare_queries(
         self,
-        cursor: databases.DatabaseCursor,
-        schema: str,
         *args,
-        parser: databases.DatabaseParser = None,
+        config: base_utils.StudyConfig,
         **kwargs,
     ):
         """constructs queries related to patient extensions of interest
 
-        :param cursor: A database cursor object
-        :param schema: the schema/db name, matching the cursor
+        :param config: A study config object
         """
         extension_types = [
             {
                 "name": "race",
                 "fhirpath": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-race",
             },
             {
                 "name": "ethnicity",
                 "fhirpath": "http://hl7.org/fhir/us/core/StructureDefinition/us-core-ethnicity",
             },
         ]
         for extension in extension_types:
             self.queries.append(
                 self.make_extension_query(
-                    schema, cursor, parser, extension["name"], extension["fhirpath"]
+                    config.db, extension["name"], extension["fhirpath"]
                 )
             )
 
-        validated_schema = sql_utils.validate_schema(
-            cursor, schema, expected_table_cols, parser
-        )
+        validated_schema = sql_utils.validate_schema(config.db, expected_table_cols)
         self.queries.append(
             core_templates.get_core_template("patient", validated_schema)
         )
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/builder_prereq_tables.py` & `cumulus_library-2.2.0/cumulus_library/studies/core/builder_prereq_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-""" This builder primarily exists to make sure that the FHIR lookup
+"""This builder primarily exists to make sure that the FHIR lookup
 tables are created before other builders in the core study run, so that
-they are available for joins. """
+they are available for joins."""
 
 import pathlib
 
 import sqlparse
 
 from cumulus_library import base_table_builder
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/completion_utils.jinja` & `cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/completion_utils.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/condition.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/condition.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/core_utils.jinja` & `cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/core_utils.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/documentreference.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/documentreference.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/encounter.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/encounter.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/medication.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/medication.sql.jinja`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 {% import 'core_utils.jinja' as utils -%}
+{% import 'syntax.sql.jinja' as syntax -%}
 
 CREATE TABLE core__medication AS (
     WITH
 
     mr_basics AS (
         SELECT DISTINCT
             {{- utils.basic_cols(
@@ -28,23 +29,23 @@
     ),
 
     contained_refs AS (
         SELECT DISTINCT
             mr.id,
             substring(mr.med_ref, 2) AS medication_id
         FROM mr_basics AS mr
-        WHERE mr.med_ref IS NOT NULL AND mr.med_ref LIKE '#%'
+        WHERE mr.med_ref IS NOT NULL AND {{ syntax.like('mr.med_ref', '#%') }}
     ),
 
     external_refs AS (
         SELECT DISTINCT
             mr.id,
             substring(mr.med_ref, 12) AS medication_id
         FROM mr_basics AS mr
-        WHERE mr.med_ref IS NOT NULL AND mr.med_ref LIKE 'Medication/%'
+        WHERE mr.med_ref IS NOT NULL AND {{ syntax.like('mr.med_ref', 'Medication/%') }}
     )
 
     {# Internal: medication data from inline ETL extraction.
     95% of the time, this dataset is the 'correct' dataset for Cerner.
     It may not be present in EPIC datasets. #}
     SELECT
         mr.id,
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/medicationrequest.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/medicationrequest.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/observation.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/observation.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/observation_component_valuequantity.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/observation_component_valuequantity.sql.jinja`

 * *Files 0% similar despite different names*

```diff
@@ -56,11 +56,11 @@
     SELECT
         'x' AS id,
         CAST(NULL AS BIGINT) AS row,
         CAST(NULL AS DOUBLE) AS value, -- noqa: disable=L029
         'x' AS comparator,
         'x' AS unit,
         'x' AS code_system,
-        'x' AS code,
+        'x' AS code
     WHERE 1=0 -- empty table
     {%- endif %}
 );
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/core_templates/patient.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/studies/core/core_templates/patient.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/count_core.py` & `cumulus_library-2.2.0/cumulus_library/studies/core/count_core.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/fhir_lookup_tables.sql` & `cumulus_library-2.2.0/cumulus_library/studies/core/fhir_lookup_tables.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/fhir_mapping_tables.sql` & `cumulus_library-2.2.0/cumulus_library/studies/core/fhir_mapping_tables.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/manifest.toml` & `cumulus_library-2.2.0/cumulus_library/studies/core/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/observation_type.sql` & `cumulus_library-2.2.0/cumulus_library/studies/core/observation_type.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_condition.sql` & `cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_condition.sql`

 * *Files 7% similar despite different names*

```diff
@@ -68,15 +68,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             condition AS s,
             UNNEST(s.clinicalStatus.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://terminology.hl7.org/CodeSystem/condition-clinical'
+            REGEXP_LIKE(u.coding.system, 'http://terminology\.hl7\.org/CodeSystem/condition-clinical')
     ), --noqa: LT07
 
     union_table AS (
         SELECT
             id,
             row,
             priority,
@@ -133,15 +133,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             condition AS s,
             UNNEST(s.code.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://snomed.info/sct'
+            REGEXP_LIKE(u.coding.system, 'http://snomed\.info/sct')
     ), --noqa: LT07
 
     system_code_1 AS (
         SELECT DISTINCT
             s.id AS id,
             0 AS row,
             '1' AS priority,
@@ -149,15 +149,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             condition AS s,
             UNNEST(s.code.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://hl7.org/fhir/sid/icd-10-cm'
+            REGEXP_LIKE(u.coding.system, 'http://hl7\.org/fhir/sid/icd-10-cm')
     ), --noqa: LT07
 
     system_code_2 AS (
         SELECT DISTINCT
             s.id AS id,
             0 AS row,
             '2' AS priority,
@@ -165,15 +165,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             condition AS s,
             UNNEST(s.code.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://hl7.org/fhir/sid/icd-9-cm'
+            REGEXP_LIKE(u.coding.system, 'http://hl7\.org/fhir/sid/icd-9-cm')
     ), --noqa: LT07
 
     system_code_3 AS (
         SELECT DISTINCT
             s.id AS id,
             0 AS row,
             '3' AS priority,
@@ -181,15 +181,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             condition AS s,
             UNNEST(s.code.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://hl7.org/fhir/sid/icd-9-cm/diagnosis'
+            REGEXP_LIKE(u.coding.system, 'http://hl7\.org/fhir/sid/icd-9-cm/diagnosis')
     ), --noqa: LT07
 
     system_code_4 AS (
         SELECT DISTINCT
             s.id AS id,
             0 AS row,
             '4' AS priority,
@@ -197,15 +197,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             condition AS s,
             UNNEST(s.code.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.2.728286'
+            REGEXP_LIKE(u.coding.system, 'urn:oid:1\.2\.840\.114350\.1\.13\.71\.2\.7\.2\.728286')
     ), --noqa: LT07
 
     system_code_5 AS (
         SELECT DISTINCT
             s.id AS id,
             0 AS row,
             '5' AS priority,
@@ -213,15 +213,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             condition AS s,
             UNNEST(s.code.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.4.698084.10375'
+            REGEXP_LIKE(u.coding.system, 'urn:oid:1\.2\.840\.114350\.1\.13\.71\.2\.7\.4\.698084\.10375')
     ), --noqa: LT07
 
     system_code_6 AS (
         SELECT DISTINCT
             s.id AS id,
             0 AS row,
             '6' AS priority,
@@ -229,15 +229,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             condition AS s,
             UNNEST(s.code.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://terminology.hl7.org/CodeSystem/data-absent-reason'
+            REGEXP_LIKE(u.coding.system, 'http://terminology\.hl7\.org/CodeSystem/data-absent-reason')
     ), --noqa: LT07
 
     union_table AS (
         SELECT
             id,
             row,
             priority,
@@ -393,15 +393,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             condition AS s,
             UNNEST(s.verificationStatus.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://terminology.hl7.org/CodeSystem/condition-ver-status'
+            REGEXP_LIKE(u.coding.system, 'http://terminology\.hl7\.org/CodeSystem/condition-ver-status')
     ), --noqa: LT07
 
     union_table AS (
         SELECT
             id,
             row,
             priority,
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_documentreference.sql` & `cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_documentreference.sql`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.category.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://hl7.org/fhir/us/core/ValueSet/us-core-documentreference-category'
+            REGEXP_LIKE(u.coding.system, 'http://hl7\.org/fhir/us/core/ValueSet/us-core-documentreference-category')
     ), --noqa: LT07
 
     union_table AS (
         SELECT
             id,
             row,
             priority,
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_encounter.sql` & `cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_encounter.sql`

 * *Files 2% similar despite different names*

```diff
@@ -28,15 +28,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://terminology.hl7.org/CodeSystem/encounter-type'
+            REGEXP_LIKE(u.coding.system, 'http://terminology\.hl7\.org/CodeSystem/encounter-type')
     ), --noqa: LT07
 
     system_type_1 AS (
         SELECT DISTINCT
             s.id AS id,
             s.row,
             '1' AS priority,
@@ -44,15 +44,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://terminology.hl7.org/CodeSystem/v2-0004'
+            REGEXP_LIKE(u.coding.system, 'http://terminology\.hl7\.org/CodeSystem/v2-0004')
     ), --noqa: LT07
 
     system_type_2 AS (
         SELECT DISTINCT
             s.id AS id,
             s.row,
             '2' AS priority,
@@ -60,15 +60,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'urn:oid:2.16.840.1.113883.4.642.3.248'
+            REGEXP_LIKE(u.coding.system, 'urn:oid:2\.16\.840\.1\.113883\.4\.642\.3\.248')
     ), --noqa: LT07
 
     system_type_3 AS (
         SELECT DISTINCT
             s.id AS id,
             s.row,
             '3' AS priority,
@@ -76,15 +76,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://snomed.info/sct'
+            REGEXP_LIKE(u.coding.system, 'http://snomed\.info/sct')
     ), --noqa: LT07
 
     system_type_4 AS (
         SELECT DISTINCT
             s.id AS id,
             s.row,
             '4' AS priority,
@@ -92,15 +92,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'https://fhir.cerner.com/%/codeSet/71'
+            REGEXP_LIKE(u.coding.system, 'https://fhir\.cerner\.com/.*/codeSet/71')
     ), --noqa: LT07
 
     system_type_5 AS (
         SELECT DISTINCT
             s.id AS id,
             s.row,
             '5' AS priority,
@@ -108,15 +108,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.10.698084.10110'
+            REGEXP_LIKE(u.coding.system, 'urn:oid:1\.2\.840\.114350\.1\.13\.71\.2\.7\.10\.698084\.10110')
     ), --noqa: LT07
 
     system_type_6 AS (
         SELECT DISTINCT
             s.id AS id,
             s.row,
             '6' AS priority,
@@ -124,15 +124,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.10.698084.18875'
+            REGEXP_LIKE(u.coding.system, 'urn:oid:1\.2\.840\.114350\.1\.13\.71\.2\.7\.10\.698084\.18875')
     ), --noqa: LT07
 
     system_type_7 AS (
         SELECT DISTINCT
             s.id AS id,
             s.row,
             '7' AS priority,
@@ -140,15 +140,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.10.698084.30'
+            REGEXP_LIKE(u.coding.system, 'urn:oid:1\.2\.840\.114350\.1\.13\.71\.2\.7\.10\.698084\.30')
     ), --noqa: LT07
 
     system_type_8 AS (
         SELECT DISTINCT
             s.id AS id,
             s.row,
             '8' AS priority,
@@ -156,15 +156,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.type.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.2.808267'
+            REGEXP_LIKE(u.coding.system, 'urn:oid:1\.2\.840\.114350\.1\.13\.71\.2\.7\.2\.808267')
     ), --noqa: LT07
 
     union_table AS (
         SELECT
             id,
             row,
             priority,
@@ -336,15 +336,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.reasoncode.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://terminology.hl7.org/CodeSystem/v3-ActPriority'
+            REGEXP_LIKE(u.coding.system, 'http://terminology\.hl7\.org/CodeSystem/v3-ActPriority')
     ), --noqa: LT07
 
     system_reasoncode_1 AS (
         SELECT DISTINCT
             s.id AS id,
             s.row,
             '1' AS priority,
@@ -352,15 +352,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.reasoncode.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://snomed.info/sct'
+            REGEXP_LIKE(u.coding.system, 'http://snomed\.info/sct')
     ), --noqa: LT07
 
     system_reasoncode_2 AS (
         SELECT DISTINCT
             s.id AS id,
             s.row,
             '2' AS priority,
@@ -368,15 +368,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.reasoncode.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://hl7.org/fhir/sid/icd-10-cm'
+            REGEXP_LIKE(u.coding.system, 'http://hl7\.org/fhir/sid/icd-10-cm')
     ), --noqa: LT07
 
     system_reasoncode_3 AS (
         SELECT DISTINCT
             s.id AS id,
             s.row,
             '3' AS priority,
@@ -384,15 +384,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.reasoncode.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'http://hl7.org/fhir/sid/icd-9-cm'
+            REGEXP_LIKE(u.coding.system, 'http://hl7\.org/fhir/sid/icd-9-cm')
     ), --noqa: LT07
 
     system_reasoncode_4 AS (
         SELECT DISTINCT
             s.id AS id,
             s.row,
             '4' AS priority,
@@ -400,15 +400,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.reasoncode.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'https://fhir.cerner.com/%/nomenclature'
+            REGEXP_LIKE(u.coding.system, 'https://fhir\.cerner\.com/.*/nomenclature')
     ), --noqa: LT07
 
     system_reasoncode_5 AS (
         SELECT DISTINCT
             s.id AS id,
             s.row,
             '5' AS priority,
@@ -416,15 +416,15 @@
             u.coding.display,
             u.coding.system AS code_system,
             u.coding.userSelected
         FROM
             flattened_rows AS s,
             UNNEST(s.reasoncode.coding) AS u (coding)
         WHERE
-            u.coding.system LIKE 'urn:oid:1.2.840.114350.1.13.71.2.7.2.728286'
+            REGEXP_LIKE(u.coding.system, 'urn:oid:1\.2\.840\.114350\.1\.13\.71\.2\.7\.2\.728286')
     ), --noqa: LT07
 
     union_table AS (
         SELECT
             id,
             row,
             priority,
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_medication.sql` & `cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_medication.sql`

 * *Files 11% similar despite different names*

```diff
@@ -82,23 +82,25 @@
     ),
 
     contained_refs AS (
         SELECT DISTINCT
             mr.id,
             substring(mr.med_ref, 2) AS medication_id
         FROM mr_basics AS mr
-        WHERE mr.med_ref IS NOT NULL AND mr.med_ref LIKE '#%'
+        WHERE mr.med_ref IS NOT NULL AND REGEXP_LIKE(mr.med_ref, '#.*')
+        )
     ),
 
     external_refs AS (
         SELECT DISTINCT
             mr.id,
             substring(mr.med_ref, 12) AS medication_id
         FROM mr_basics AS mr
-        WHERE mr.med_ref IS NOT NULL AND mr.med_ref LIKE 'Medication/%'
+        WHERE mr.med_ref IS NOT NULL AND REGEXP_LIKE(mr.med_ref, 'Medication/.*')
+        )
     )
 
     
     SELECT
         mr.id,
         mr.encounter_ref,
         mr.patient_ref,
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_medicationrequest.sql` & `cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_medicationrequest.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_observation.sql` & `cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_observation.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_patient.sql` & `cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_patient.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/builder_prereq_tables.sql` & `cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/builder_prereq_tables.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/reference_sql/count_core.sql` & `cumulus_library-2.2.0/cumulus_library/studies/core/reference_sql/count_core.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/setup.sql` & `cumulus_library-2.2.0/cumulus_library/studies/core/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/core/study_period.sql` & `cumulus_library-2.2.0/cumulus_library/studies/core/study_period.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/discovery/code_definitions.py` & `cumulus_library-2.2.0/cumulus_library/studies/discovery/code_definitions.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/discovery/code_detection.py` & `cumulus_library-2.2.0/cumulus_library/studies/discovery/code_detection.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,60 +1,52 @@
-""" Module for generating encounter codeableConcept table"""
+"""Module for generating encounter codeableConcept table"""
 
-from cumulus_library import base_table_builder, base_utils, databases
+from cumulus_library import base_table_builder, base_utils
 from cumulus_library.studies.discovery import code_definitions
 from cumulus_library.studies.discovery.discovery_templates import discovery_templates
 from cumulus_library.template_sql import sql_utils
 
 
 class CodeDetectionBuilder(base_table_builder.BaseTableBuilder):
     display_text = "Selecting unique code systems..."
 
-    def _check_coding_against_db(self, code_source, schema, cursor, parser):
+    def _check_coding_against_db(self, code_source, database):
         """selects the appropriate DB query to run"""
 
         return sql_utils.is_field_populated(
-            schema=schema,
+            database=database,
             source_table=code_source["table_name"],
             hierarchy=code_source["column_hierarchy"],
             expected=code_source.get("expected"),
-            cursor=cursor,
-            parser=parser,
         )
 
-    def _check_codes_in_fields(
-        self, code_sources: list[dict], schema, cursor, parser
-    ) -> dict:
+    def _check_codes_in_fields(self, code_sources: list[dict], database) -> dict:
         """checks if Coding/CodeableConcept fields are present and populated"""
 
         with base_utils.get_progress_bar() as progress:
             task = progress.add_task(
                 "Discovering available coding systems...",
                 total=len(code_sources),
             )
             for code_source in code_sources:
                 code_source["has_data"] = self._check_coding_against_db(
-                    code_source, schema, cursor, parser
+                    code_source, database
                 )
                 progress.advance(task)
         return code_sources
 
     def prepare_queries(
         self,
-        cursor: databases.DatabaseCursor,
-        schema: str,
-        parser: databases.DatabaseParser = None,
         *args,
+        config: base_utils.StudyConfig,
         **kwargs,
     ):
         """Constructs queries related to condition codeableConcept
 
-        :param cursor: A database cursor object
-        :param schema: the schema/db name, matching the cursor
-
+        :param config: A study config object
         """
 
         code_sources = []
         required_keys = {"table_name", "column_hierarchy"}
         for code_definition in code_definitions.code_list:
             if not required_keys.issubset(code_definition):
                 raise KeyError(
@@ -63,12 +55,12 @@
                 )
             code_source = {
                 "has_data": False,
             }
             for key in code_definition.keys():
                 code_source[key] = code_definition[key]
             code_sources.append(code_source)
-        code_sources = self._check_codes_in_fields(code_sources, schema, cursor, parser)
+        code_sources = self._check_codes_in_fields(code_sources, config.db)
         query = discovery_templates.get_code_system_pairs(
             "discovery__code_sources", code_sources
         )
         self.queries.append(query)
```

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/discovery/discovery_templates/code_system_pairs.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/studies/discovery/discovery_templates/code_system_pairs.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/discovery/discovery_templates/discovery_templates.py` & `cumulus_library-2.2.0/cumulus_library/studies/discovery/discovery_templates/discovery_templates.py`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/discovery/reference_sql/code_detection.sql` & `cumulus_library-2.2.0/cumulus_library/studies/discovery/reference_sql/code_detection.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/template/counts.sql` & `cumulus_library-2.2.0/cumulus_library/studies/template/counts.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/template/lab_observations.sql` & `cumulus_library-2.2.0/cumulus_library/studies/template/lab_observations.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/template/manifest.toml` & `cumulus_library-2.2.0/cumulus_library/studies/template/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/template/setup.sql` & `cumulus_library-2.2.0/cumulus_library/studies/template/setup.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/vocab/icd/ICD10CM_2023AA.bsv` & `cumulus_library-2.2.0/cumulus_library/studies/vocab/icd/ICD10CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/vocab/icd/ICD10PCS_2023AA.bsv` & `cumulus_library-2.2.0/cumulus_library/studies/vocab/icd/ICD10PCS_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/vocab/icd/ICD9CM_2023AA.bsv` & `cumulus_library-2.2.0/cumulus_library/studies/vocab/icd/ICD9CM_2023AA.bsv`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/vocab/reference_sql/vocab_icd_builder.sql` & `cumulus_library-2.2.0/cumulus_library/studies/vocab/reference_sql/vocab_icd_builder.sql`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/studies/vocab/vocab_icd_builder.py` & `cumulus_library-2.2.0/cumulus_library/studies/vocab/vocab_icd_builder.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Module for directly loading ICD bsvs into athena tables """
+"""Module for directly loading ICD bsvs into athena tables"""
 
 import pathlib
 
 import pandas
 
 from cumulus_library import base_table_builder, base_utils
 from cumulus_library.template_sql import base_templates
```

### Comparing `cumulus_library-2.1.0/cumulus_library/study_parser.py` & `cumulus_library-2.2.0/cumulus_library/study_parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-""" Contains classes for loading study data based on manifest.toml files """
+"""Contains classes for loading study data based on manifest.toml files"""
 
+import contextlib
 import csv
 import importlib.util
 import inspect
 import pathlib
 import sys
 import typing
 
@@ -21,14 +22,24 @@
     errors,
     protected_table_builder,
 )
 from cumulus_library.statistics import psm
 from cumulus_library.template_sql import base_templates
 
 
+@contextlib.contextmanager
+def _temporary_sys_path(add: pathlib.Path) -> None:
+    orig_path = list(sys.path)
+    try:
+        sys.path.insert(0, str(add))
+        yield
+    finally:
+        sys.path = orig_path
+
+
 class StudyManifestParser:
     """Handles loading of study data from manifest files.
 
     The goal of this class is to make it so that a researcher can contribute a study
     definition without touching the main python infrastructure. It provides
     mechanisms for IDing studies/files of interest, and for executing queries, but
     specifically it should never be in charge of instantiation a cursor itself -
@@ -69,17 +80,20 @@
                 ):
                     raise errors.StudyManifestParsingError(
                         f"Invalid prefix in manifest at {study_path}"
                     )
                 self._study_config = config
             self._study_path = study_path
         except FileNotFoundError as e:
-            raise errors.StudyManifestFilesystemError(  # pylint: disable=raise-missing-from
+            raise errors.StudyManifestFilesystemError(
                 f"Missing or invalid manifest found at {study_path}"
             ) from e
+        except toml.TomlDecodeError as e:
+            # just unify the error classes for convenience of catching them
+            raise errors.StudyManifestParsingError(str(e)) from e
 
     def get_study_prefix(self) -> str | None:
         """Reads the name of a study prefix from the in-memory study config
 
         :returns: A string of the prefix in the manifest, or None if not found
         """
         return self._study_config.get("study_prefix")
@@ -349,15 +363,19 @@
 
         """
         spec = importlib.util.spec_from_file_location(
             "table_builder", f"{self._study_path}/{filename}"
         )
         table_builder_module = importlib.util.module_from_spec(spec)
         sys.modules["table_builder"] = table_builder_module
-        spec.loader.exec_module(table_builder_module)
+        # Inject the study dir into sys.path so that builders can import
+        # from surrounding utility code, even if the study isn't installed.
+        # (i.e. you're working from a git checkout and do something like `-s .`)
+        with _temporary_sys_path(self._study_path.parent):
+            spec.loader.exec_module(table_builder_module)
 
         # We're going to find all subclasses of BaseTableBuild in this file.
         # Since BaseTableBuilder itself is a valid subclass of BaseTableBuilder,
         # we'll detect and skip it. If we don't find any subclasses,
         # we'll punt.
         table_builder_subclasses = []
         for _, cls_obj in inspect.getmembers(table_builder_module, inspect.isclass):
```

### Comparing `cumulus_library-2.1.0/cumulus_library/template_sql/base_templates.py` & `cumulus_library-2.2.0/cumulus_library/template_sql/base_templates.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Collection of jinja template getters for common SQL queries """
+"""Collection of jinja template getters for common SQL queries"""
 
 import enum
 import pathlib
 
 import jinja2
 import pandas
```

### Comparing `cumulus_library-2.1.0/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/template_sql/codeable_concept_denormalize.sql.jinja`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
             u.coding.userSelected
         FROM
         {#- Temp workaround - to be reworked by generic DN #}
             {{ source_table }} AS s,
             UNNEST(s.{{ field_alias }}.coding) AS u (coding)
         {%- if filter_priority %}
         WHERE
-            u.coding.system LIKE '{{ system }}'
+            {{ syntax.like('u.coding.system', system) }}
         {%- endif %}
     ), --noqa: LT07
     {%- endfor %}
 
     union_table AS (
         {%- for system in code_systems %}
         SELECT
```

### Comparing `cumulus_library-2.1.0/cumulus_library/template_sql/coding_denormalize.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/template_sql/coding_denormalize.sql.jinja`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
             u.parent_col.{{ column_name }}.display,
             u.parent_col.{{ column_name }}.system AS code_system
         FROM
             {{ source_table }} AS s,
             UNNEST(s.{{ parent_field }}) AS u (parent_col)
         {%- if filter_priority %}
         WHERE
-            u.parent_col.{{ column_name }}.system LIKE '{{ system }}'
+            {{ syntax.like("u.parent_col." + column_name + ".system", system) }}
         {%- endif %}
     ), --noqa: LT07
     {%- endfor %}
 
     union_table AS (
         {%- for system in code_systems %}
         SELECT
```

### Comparing `cumulus_library-2.1.0/cumulus_library/template_sql/create_view_as.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/template_sql/create_view_as.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/template_sql/ctas.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/template_sql/ctas.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/template_sql/ctas_empty.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/template_sql/ctas_empty.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/template_sql/ctas_from_parquet.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/template_sql/ctas_from_parquet.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/template_sql/extension_denormalize.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/template_sql/extension_denormalize.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/template_sql/insert_into.sql.jinja` & `cumulus_library-2.2.0/cumulus_library/template_sql/insert_into.sql.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/template_sql/shared_macros/unnest_utils.jinja` & `cumulus_library-2.2.0/cumulus_library/template_sql/shared_macros/unnest_utils.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library-2.1.0/cumulus_library/template_sql/sql_utils.py` & `cumulus_library-2.2.0/cumulus_library/template_sql/sql_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 and validating them so that the actual generated queries can be constructed more
 simply. This includes, but is not limited, to:
     - Data missing entirely
     - Data present, but 'nullish' - with some structure but no value
     - Data with deep missing elements
     - Data which may or may not be in an array depending on context
 """
-import abc
+
 from dataclasses import dataclass, field
 
 from cumulus_library import base_utils, databases
 from cumulus_library.template_sql import base_templates
 
 # *** Some convenience constants for providing to validate_schema() ***
 # * Only include necessary fields that we actually use.
@@ -22,16 +22,16 @@
 # If you think you need CODEABLE_CONCEPT, you probably need a de-normalization table
 # instead, since CodeableConcepts can contain multiple entries.
 CODEABLE_CONCEPT = {"coding": CODING, "text": {}}
 REFERENCE = ["reference"]
 
 
 @dataclass(kw_only=True)
-class BaseConfig(abc.ABC):
-    """Abstract ase class for handling table detection/denormalization"""
+class BaseConfig:
+    """Base class for handling table detection/denormalization"""
 
     source_table: str = None
     source_id: str = "id"
     target_table: str = None
     has_data: bool = False
 
 
@@ -86,17 +86,15 @@
     target_col_prefix: str
     fhir_extension: str
     ext_systems: list[str]
     is_array: bool = False
 
 
 def _check_data_in_fields(
-    schema: str,
-    cursor: databases.DatabaseCursor,
-    parser: databases.DatabaseParser,
+    database: databases.DatabaseBackend,
     code_sources: list[CodeableConceptConfig],
 ) -> dict:
     """checks if CodeableConcept fields actually have data available
 
     CodeableConcept fields are mostly optional in the FHIR spec, and may be arrays
     or single objects. Additionally, the null representation can be inconsistent,
     depending on how the data is provided from an EHR and how the ETL manages
@@ -112,40 +110,36 @@
     The way we do this is slightly different depending on if the field is an
     array or not (generally requiring one extra level of unnesting).
 
     """
 
     with base_utils.get_progress_bar(transient=True) as progress:
         task = progress.add_task(
-            "Detecting available encounter codeableConcepts...",
+            "Detecting available codeableConcepts...",
             # Each column in code_sources requires at most 3 queries to
             # detect valid data is in the DB
             total=len(code_sources),
         )
         for code_source in code_sources:
             code_source.has_data = is_field_populated(
-                schema=schema,
-                cursor=cursor,
-                parser=parser,
+                database=database,
                 source_table=code_source.source_table,
                 hierarchy=code_source.column_hierarchy,
                 expected=code_source.expected,
             )
             progress.advance(task)
     return code_sources
 
 
 def denormalize_complex_objects(
-    schema: str,
-    cursor: databases.DatabaseCursor,
-    parser: databases.DatabaseParser,
+    database: databases.DatabaseBackend,
     code_sources: list[BaseConfig],
 ):
     queries = []
-    code_sources = _check_data_in_fields(schema, cursor, parser, code_sources)
+    code_sources = _check_data_in_fields(database, code_sources)
     for code_source in code_sources:
         # TODO: This method of pairing classed config objects to
         # specific queries should be considered temporary. This should be
         # replaced at some point by a more generic table schema traversal/
         # generic jinja template approach.
         match code_source:
             case CodeableConceptConfig():
@@ -173,79 +167,83 @@
                         "boolean",
                     ]
                     if code_source.extra_fields:
                         table_cols += [f[1] for f in code_source.extra_fields]
                         col_types += ["varchar"] * len(code_source.extra_fields)
                     queries.append(
                         base_templates.get_ctas_empty_query(
-                            schema_name=schema,
+                            schema_name=database.schema_name,
                             table_name=code_source.target_table,
                             table_cols=table_cols,
                             table_cols_types=col_types,
                         )
                     )
             case CodingConfig():
                 if code_source.has_data:
                     queries.append(
                         base_templates.get_coding_denormalize_query(code_source)
                     )
                 else:
                     queries.append(
                         base_templates.get_ctas_empty_query(
-                            schema_name=schema,
+                            schema_name=database.schema_name,
                             table_name=code_source.target_table,
                             table_cols=["id", "code", "code_system", "display"],
                         )
                     )
 
     return queries
 
 
 def validate_schema(
-    cursor: databases.DatabaseCursor,
-    schema: str,
+    database: databases.DatabaseBackend,
     expected_table_cols: dict,
-    parser: databases.DatabaseParser,
 ) -> dict:
     validated_schema = {}
     for table, cols in expected_table_cols.items():
-        query = base_templates.get_column_datatype_query(schema, table, cols.keys())
-        table_schema = cursor.execute(query).fetchall()
-        validated_schema[table] = parser.validate_table_schema(cols, table_schema)
+        query = base_templates.get_column_datatype_query(
+            database.schema_name, table, cols.keys()
+        )
+
+        try:
+            table_schema = database.cursor().execute(query).fetchall()
+        except database.operational_errors():
+            # A database backend might reasonably raise an exception in cases like
+            # the table not existing (Athena does this).
+            table_schema = []
+
+        validated_schema[table] = database.parser().validate_table_schema(
+            cols, table_schema
+        )
     return validated_schema
 
 
 def is_field_populated(
     *,
-    schema: str,
-    cursor: databases.DatabaseCursor,
-    parser: databases.DatabaseParser,
+    database: databases.DatabaseBackend,
     source_table: str,
     hierarchy: list[tuple],
     expected: list | dict | None = None,
 ) -> bool:
     """Traverses a complex field and determines if it exists and has data
 
     Non-core studies that rely on the core tables shouldn't need this method.
     This is just to examine the weird and wonderful world of the raw FHIR tables.
 
-    :keyword schema: The schema/database name
-    :keyword cursor: a PEP-249 compliant database cursor
+    :keyword database: The database backend
     :keyword source_table: The table to query against
     :keyword hierarchy: a list of tuples defining the FHIR path to the element.
         Each tuple should be of the form ('element_name', dict | list), where
         a dict is a bare nested object and a list is an array object
     :keyword expected: a list of elements that should be present in the field.
         If none, we assume it is a CodeableConcept.
     :returns: a boolean indicating if valid data is present.
     """
     if not is_field_present(
-        schema=schema,
-        cursor=cursor,
-        parser=parser,
+        database=database,
         source_table=source_table,
         source_col=hierarchy[0][0],
         expected=expected,
     ):
         return False
     unnests = []
     source_field = []
@@ -267,45 +265,41 @@
             raise ValueError(
                 "sql_utils.is_field_populated: Unexpected type "
                 f"{element[1]} for field {element[0]}"
             )
     query = base_templates.get_is_table_not_empty_query(
         source_table=source_table, field=".".join(source_field), unnests=unnests
     )
-    res = cursor.execute(query).fetchall()
+    res = database.cursor().execute(query).fetchall()
     if len(res) == 0:
         return False
     return True
 
 
 def is_field_present(
     *,
-    schema: str,
-    cursor: databases.DatabaseCursor,
-    parser: databases.DatabaseParser,
+    database: databases.DatabaseBackend,
     source_table: str,
     source_col: str,
     expected: list | dict | None = None,
 ) -> bool:
     """Validation check for a column existing, and having the expected schema
 
-    :keyword schema: The schema/database name
-    :keyword cursor: a PEP-249 compliant database cursor
-    :keyword parser: a database schema parser
+    :keyword database: The database backend
     :keyword source_table: The table to query against
     :keyword source_col: The column to check the schema against
     :keyword expected: a list of elements that should be present in source_col.
         If none, we assume it is a CodeableConcept.
     :returns: a boolean indicating if the schema was found.
     """
     if expected is None:
         expected = CODEABLE_CONCEPT
 
     table_cols = {source_table: {source_col: expected}}
-    schema = validate_schema(cursor, schema, table_cols, parser)
+    schema = validate_schema(database, table_cols)
 
     def _get_all_values(d: dict) -> list:
         all_values = []
         for value in d.values():
             if isinstance(value, dict):
                 all_values += _get_all_values(value)
             else:
```

### Comparing `cumulus_library-2.1.0/cumulus_library/upload.py` & `cumulus_library-2.2.0/cumulus_library/upload.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-""" Handles pushing data to the aggregator"""
+"""Handles pushing data to the aggregator"""
 
 import sys
 from pathlib import Path
 
 import requests
 from pandas import read_parquet
 from rich.progress import Progress, TaskID
```

### Comparing `cumulus_library-2.1.0/pyproject.toml` & `cumulus_library-2.2.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -27,26 +27,27 @@
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic=["version"]
 [project.optional-dependencies]
 dev = [
-    "ruff == 0.2.1",
+    # if you update the ruff version, also update .pre-commit-config.yaml
+    "ruff == 0.4.4",
     "pre-commit",
 ]
 test = [
     "freezegun",
     "pytest",
     "responses"
 ]
 
 [project.urls]
-Home = "https://smarthealthit.org/cumulus-a-universal-sidecar-for-a-smart-learning-healthcare-system/"
-Documentation = "https://docs.smarthealthit.org/cumulus/"
+Home = "https://smarthealthit.org/cumulus/"
+Documentation = "https://docs.smarthealthit.org/cumulus/library/"
 Source = "https://github.com/smart-on-fhir/cumulus-library"
 
 
 [project.scripts]
 cumulus-library = "cumulus_library.cli:main_cli"
 
 [build-system]
@@ -58,17 +59,14 @@
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 testpaths = [
     "tests",
 ]
 
-[tool.ruff]
-target-version = "py310"
-
 [tool.ruff.lint]
 select = [
     "A",  # prevent using keywords that clobber python builtins
     "B",  # bugbear: security warnings
     "E",  # pycodestyle
     "F",  # pyflakes
     "I",  # isort
```

### Comparing `cumulus_library-2.1.0/PKG-INFO` & `cumulus_library-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cumulus-library
-Version: 2.1.0
+Version: 2.2.0
 Summary: Clinical study SQL generation for data derived from bulk FHIR
 Keywords: FHIR,SQL,Health Informatics
 Requires-Python: >= 3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
@@ -20,21 +20,21 @@
 Requires-Dist: pyathena >= 2.23
 Requires-Dist: pytablewriter >= 1.2
 Requires-Dist: requests >= 2.28
 Requires-Dist: rich >= 13.2
 Requires-Dist: sqlfluff  >= 3
 Requires-Dist: sqlparse >0.4
 Requires-Dist: toml >= 0.10
-Requires-Dist: ruff == 0.2.1 ; extra == "dev"
+Requires-Dist: ruff == 0.4.4 ; extra == "dev"
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: freezegun ; extra == "test"
 Requires-Dist: pytest ; extra == "test"
 Requires-Dist: responses ; extra == "test"
-Project-URL: Documentation, https://docs.smarthealthit.org/cumulus/
-Project-URL: Home, https://smarthealthit.org/cumulus-a-universal-sidecar-for-a-smart-learning-healthcare-system/
+Project-URL: Documentation, https://docs.smarthealthit.org/cumulus/library/
+Project-URL: Home, https://smarthealthit.org/cumulus/
 Project-URL: Source, https://github.com/smart-on-fhir/cumulus-library
 Provides-Extra: dev
 Provides-Extra: test
 
 # Cumulus Library - Core
 
 A framework for designing, executing, and distributing SQL queries packaged as "studies", e.g., for quality monitoring, clinical research, or public health. Part of the [SMART on FHIR Cumulus Project](https://smarthealthit.org/cumulus-a-universal-sidecar-for-a-smart-learning-healthcare-system/)
```

