# Comparing `tmp/cumulus_library_data_metrics-0.0.0.tar.gz` & `tmp/cumulus_library_data_metrics-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cumulus_library_data_metrics-0.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "cumulus_library_data_metrics-1.0.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `cumulus_library_data_metrics-0.0.0.tar` & `cumulus_library_data_metrics-1.0.0.tar`

### file list

```diff
@@ -1,278 +1,278 @@
--rw-r--r--   0        0        0    11357 2024-05-10 16:22:00.022863 cumulus_library_data_metrics-0.0.0/LICENSE
--rw-r--r--   0        0        0     4356 2024-05-06 17:32:12.293789 cumulus_library_data_metrics-0.0.0/README.md
--rw-r--r--   0        0        0       68 2024-05-14 17:31:51.185664 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/__init__.py
--rw-r--r--   0        0        0        0 2024-05-13 13:20:32.751383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/__init__.py
--rw-r--r--   0        0        0     3750 2024-05-13 13:20:32.751383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/base.py
--rw-r--r--   0        0        0     1434 2024-05-13 13:20:32.751383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/base.summary.jinja
--rw-r--r--   0        0        0      899 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_pt_count/README.md
--rw-r--r--   0        0        0     1113 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_pt_count/c_pt_count.jinja
--rw-r--r--   0        0        0      922 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_pt_count/c_pt_count.py
--rw-r--r--   0        0        0      308 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_pt_deceased_count/README.md
--rw-r--r--   0        0        0     1861 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_pt_deceased_count/c_pt_deceased_count.jinja
--rw-r--r--   0        0        0      563 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_pt_deceased_count/c_pt_deceased_count.py
--rw-r--r--   0        0        0      265 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_resource_count/README.md
--rw-r--r--   0        0        0     1099 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_resource_count/c_resource_count.jinja
--rw-r--r--   0        0        0     1094 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_resource_count/c_resource_count.py
--rw-r--r--   0        0        0      347 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_resources_per_pt/README.md
--rw-r--r--   0        0        0     2545 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_resources_per_pt/c_resources_per_pt.jinja
--rw-r--r--   0        0        0      955 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_resources_per_pt/c_resources_per_pt.py
--rw-r--r--   0        0        0     1057 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_term_coverage/README.md
--rw-r--r--   0        0        0     2385 2024-05-13 15:17:59.298111 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_term_coverage/c_term_coverage.jinja
--rw-r--r--   0        0        0     2237 2024-05-13 15:17:59.298111 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_term_coverage/c_term_coverage.py
--rw-r--r--   0        0        0     2075 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_us_core_v4_count/README.md
--rw-r--r--   0        0        0     1595 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_us_core_v4_count/c_us_core_v4_count.jinja
--rw-r--r--   0        0        0      446 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_us_core_v4_count/c_us_core_v4_count.py
--rw-r--r--   0        0        0     3647 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/manifest.toml
--rw-r--r--   0        0        0     1078 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/meta/dates.jinja
--rw-r--r--   0        0        0      748 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/meta/meta.py
--rw-r--r--   0        0        0       77 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/meta/version.jinja
--rw-r--r--   0        0        0      904 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_date_recent/README.md
--rw-r--r--   0        0        0     1234 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_date_recent/q_date_recent.jinja
--rw-r--r--   0        0        0      825 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_date_recent/q_date_recent.py
--rw-r--r--   0        0        0     1420 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_ref_target_pop/README.md
--rw-r--r--   0        0        0      374 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_ref_target_pop/q_ref_target_pop.jinja
--rw-r--r--   0        0        0     1544 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_ref_target_pop/q_ref_target_pop.py
--rw-r--r--   0        0        0     1195 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_ref_target_valid/README.md
--rw-r--r--   0        0        0      504 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_ref_target_valid/denominator.jinja
--rw-r--r--   0        0        0      991 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_ref_target_valid/q_ref_target_valid.jinja
--rw-r--r--   0        0        0     2594 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_ref_target_valid/q_ref_target_valid.py
--rw-r--r--   0        0        0      736 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_term_use/README.md
--rw-r--r--   0        0        0      947 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_term_use/q_term_use.jinja
--rw-r--r--   0        0        0     3712 2024-05-13 15:17:59.298111 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_term_use/q_term_use.py
--rw-r--r--   0        0        0     3587 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_valid_us_core_v4/README.md
--rw-r--r--   0        0        0      738 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.jinja
--rw-r--r--   0        0        0      701 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.py
--rw-r--r--   0        0        0     2725 2024-05-13 15:17:59.298111 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/resource_info.py
--rw-r--r--   0        0        0      105 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/t_us_core_v4/README.md
--rw-r--r--   0        0        0      182 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/t_us_core_v4/mandatory.jinja
--rw-r--r--   0        0        0      225 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/t_us_core_v4/must_support.jinja
--rw-r--r--   0        0        0      828 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/t_us_core_v4/t_us_core_v4.py
--rw-r--r--   0        0        0      345 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/README.md
--rw-r--r--   0        0        0       50 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/__init__.py
--rw-r--r--   0        0        0     2453 2024-05-13 15:21:50.405212 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/allergyintolerance_mandatory.jinja
--rw-r--r--   0        0        0     2666 2024-05-14 15:57:36.342009 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/allergyintolerance_must_support.jinja
--rw-r--r--   0        0        0     2603 2024-05-13 15:21:46.029078 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/condition_mandatory.jinja
--rw-r--r--   0        0        0     1414 2024-05-14 15:57:36.342009 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/condition_must_support.jinja
--rw-r--r--   0        0        0     1180 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/diagnosticreport_note_mandatory.jinja
--rw-r--r--   0        0        0      763 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/diagnosticreport_note_must_support.jinja
--rw-r--r--   0        0        0     2129 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/documentreference_mandatory.jinja
--rw-r--r--   0        0        0     2945 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/documentreference_must_support.jinja
--rw-r--r--   0        0        0      834 2024-05-13 13:20:32.755383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/encounter_mandatory.jinja
--rw-r--r--   0        0        0     1503 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/encounter_must_support.jinja
--rw-r--r--   0        0        0      954 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/immunization_mandatory.jinja
--rw-r--r--   0        0        0      570 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/immunization_must_support.jinja
--rw-r--r--   0        0        0      356 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/medication_mandatory.jinja
--rw-r--r--   0        0        0      129 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/medication_must_support.jinja
--rw-r--r--   0        0        0     1322 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/medicationrequest_mandatory.jinja
--rw-r--r--   0        0        0     1018 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/medicationrequest_must_support.jinja
--rw-r--r--   0        0        0      316 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/observation_blood_pressure_mandatory.jinja
--rw-r--r--   0        0        0     2291 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/observation_laboratory_mandatory.jinja
--rw-r--r--   0        0        0     1024 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/observation_laboratory_must_support.jinja
--rw-r--r--   0        0        0     1974 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/observation_smoking_status_mandatory.jinja
--rw-r--r--   0        0        0      190 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/observation_smoking_status_must_support.jinja
--rw-r--r--   0        0        0     3804 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/observation_utils.jinja
--rw-r--r--   0        0        0     4855 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/observation_vital_signs_mandatory.jinja
--rw-r--r--   0        0        0     1032 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/observation_vital_signs_must_support.jinja
--rw-r--r--   0        0        0      619 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/patient_mandatory.jinja
--rw-r--r--   0        0        0     2503 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/patient_must_support.jinja
--rw-r--r--   0        0        0     5242 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/patient_utils.jinja
--rw-r--r--   0        0        0     1004 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/procedure_mandatory.jinja
--rw-r--r--   0        0        0      128 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/procedure_must_support.jinja
--rw-r--r--   0        0        0     3559 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/profiles.py
--rw-r--r--   0        0        0      398 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/slice.jinja
--rw-r--r--   0        0        0     9285 2024-05-13 13:20:32.759383 cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/utils.jinja
--rw-r--r--   0        0        0     1599 2024-05-14 17:23:36.759247 cumulus_library_data_metrics-0.0.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-11-27 19:34:06.223839 cumulus_library_data_metrics-0.0.0/tests/__init__.py
--rw-r--r--   0        0        0     9018 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_pt_count/cubed/expected.csv
--rw-r--r--   0        0        0     3065 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_pt_count/cubed/patient/0.ndjson
--rw-r--r--   0        0        0      679 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_pt_count/general/expected.csv
--rw-r--r--   0        0        0     3065 2024-03-15 16:16:34.311959 cumulus_library_data_metrics-0.0.0/tests/data/c_pt_count/general/patient/0.ndjson
--rw-r--r--   0        0        0      122 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_pt_count/no-ext/expected.csv
--rw-r--r--   0        0        0       33 2024-01-09 18:47:28.423218 cumulus_library_data_metrics-0.0.0/tests/data/c_pt_count/no-ext/patient/0.ndjson
--rw-r--r--   0        0        0      269 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_pt_deceased_count/general/expected.csv
--rw-r--r--   0        0        0      786 2024-01-19 19:10:24.850826 cumulus_library_data_metrics-0.0.0/tests/data/c_pt_deceased_count/general/patient/0.ndjson
--rw-r--r--   0        0        0     1334 2023-12-08 18:29:24.777837 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0     1978 2023-12-05 21:40:19.230358 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/condition/0.ndjson
--rw-r--r--   0        0        0       24 2023-12-05 21:40:19.230358 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/device/0.ndjson
--rw-r--r--   0        0        0      494 2024-05-07 13:43:38.371994 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/diagnosticreport/0.ndjson
--rw-r--r--   0        0        0      593 2024-05-07 13:43:38.371994 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/documentreference/0.ndjson
--rw-r--r--   0        0        0      603 2023-12-05 21:40:19.230358 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/encounter/0.ndjson
--rw-r--r--   0        0        0      417 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_allergyintolerance_month.csv
--rw-r--r--   0        0        0      375 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_allergyintolerance_year.csv
--rw-r--r--   0        0        0      456 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_condition_month.csv
--rw-r--r--   0        0        0      354 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_condition_year.csv
--rw-r--r--   0        0        0       27 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_device_all.csv
--rw-r--r--   0        0        0      200 2024-05-07 13:43:38.371994 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_diagnosticreport_month.csv
--rw-r--r--   0        0        0      190 2024-05-07 13:43:38.371994 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_diagnosticreport_year.csv
--rw-r--r--   0        0        0      225 2024-05-07 13:43:38.371994 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_documentreference_month.csv
--rw-r--r--   0        0        0      215 2024-05-07 13:43:38.371994 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_documentreference_year.csv
--rw-r--r--   0        0        0      203 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_encounter_month.csv
--rw-r--r--   0        0        0      193 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_encounter_year.csv
--rw-r--r--   0        0        0      114 2024-05-07 13:43:38.371994 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_immunization_month.csv
--rw-r--r--   0        0        0      104 2024-05-07 13:43:38.371994 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_immunization_year.csv
--rw-r--r--   0        0        0       27 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_medication_all.csv
--rw-r--r--   0        0        0      144 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_medicationrequest_month.csv
--rw-r--r--   0        0        0      140 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_medicationrequest_year.csv
--rw-r--r--   0        0        0      273 2024-05-07 13:43:38.371994 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_observation_month.csv
--rw-r--r--   0        0        0      257 2024-05-07 13:43:38.371994 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_observation_year.csv
--rw-r--r--   0        0        0       47 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_patient_all.csv
--rw-r--r--   0        0        0      178 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_procedure_month.csv
--rw-r--r--   0        0        0      147 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/expected_procedure_year.csv
--rw-r--r--   0        0        0      203 2024-05-07 13:43:38.371994 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/immunization/0.ndjson
--rw-r--r--   0        0        0       36 2023-12-05 21:40:19.230358 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/medication/0.ndjson
--rw-r--r--   0        0        0      342 2023-12-05 21:40:19.230358 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/medicationrequest/0.ndjson
--rw-r--r--   0        0        0      934 2024-05-07 13:43:38.371994 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/observation/0.ndjson
--rw-r--r--   0        0        0       87 2023-12-08 19:02:04.206381 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/patient/0.ndjson
--rw-r--r--   0        0        0      310 2024-01-26 19:00:15.066781 cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/procedure/0.ndjson
--rw-r--r--   0        0        0      118 2024-05-09 14:45:04.527709 cumulus_library_data_metrics-0.0.0/tests/data/c_resources_per_pt/general/condition/0.ndjson
--rw-r--r--   0        0        0      544 2024-05-09 14:45:04.527709 cumulus_library_data_metrics-0.0.0/tests/data/c_resources_per_pt/general/expected_summary.csv
--rw-r--r--   0        0        0     1264 2024-05-09 14:45:04.527709 cumulus_library_data_metrics-0.0.0/tests/data/c_resources_per_pt/general/medicationrequest/0.ndjson
--rw-r--r--   0        0        0       36 2024-05-08 13:37:46.002085 cumulus_library_data_metrics-0.0.0/tests/data/c_resources_per_pt/general/patient/0.ndjson
--rw-r--r--   0        0        0      993 2024-02-16 14:04:37.999886 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0     1408 2023-12-12 14:40:53.343644 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/condition/0.ndjson
--rw-r--r--   0        0        0      105 2023-12-12 14:46:10.774892 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/device/0.ndjson
--rw-r--r--   0        0        0      105 2024-01-08 20:06:19.758713 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/diagnosticreport/0.ndjson
--rw-r--r--   0        0        0      105 2023-12-12 14:46:10.774892 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/documentreference/0.ndjson
--rw-r--r--   0        0        0      383 2023-12-12 15:33:10.903243 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/encounter/0.ndjson
--rw-r--r--   0        0        0      265 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/expected_allergyintolerance_code.csv
--rw-r--r--   0        0        0      368 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/expected_condition_code.csv
--rw-r--r--   0        0        0       73 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/expected_device_type.csv
--rw-r--r--   0        0        0      106 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/expected_diagnosticreport_code.csv
--rw-r--r--   0        0        0      106 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/expected_documentreference_type.csv
--rw-r--r--   0        0        0      105 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/expected_encounter_class.csv
--rw-r--r--   0        0        0      147 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/expected_encounter_type.csv
--rw-r--r--   0        0        0      106 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/expected_immunization_vaccinecode.csv
--rw-r--r--   0        0        0       73 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/expected_medication_code.csv
--rw-r--r--   0        0        0      106 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/expected_medicationrequest_medicationcodeableconcept.csv
--rw-r--r--   0        0        0      281 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/expected_observation_code.csv
--rw-r--r--   0        0        0      308 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/expected_observation_valuecodeableconcept.csv
--rw-r--r--   0        0        0      106 2024-05-06 17:32:12.297789 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/expected_procedure_code.csv
--rw-r--r--   0        0        0      112 2023-12-12 14:48:08.823415 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/immunization/0.ndjson
--rw-r--r--   0        0        0      105 2023-12-12 14:48:51.748684 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/medication/0.ndjson
--rw-r--r--   0        0        0      126 2023-12-12 14:49:31.353700 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/medicationrequest/0.ndjson
--rw-r--r--   0        0        0     1415 2024-02-14 21:48:33.707568 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/observation/0.ndjson
--rw-r--r--   0        0        0      105 2023-12-12 14:50:08.362526 cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/procedure/0.ndjson
--rw-r--r--   0        0        0      842 2024-04-12 13:09:48.084692 cumulus_library_data_metrics-0.0.0/tests/data/c_us_core_v4_count/general/documentreference/0.ndjson
--rw-r--r--   0        0        0      254 2024-05-07 13:43:38.371994 cumulus_library_data_metrics-0.0.0/tests/data/c_us_core_v4_count/general/expected_documentreference.csv
--rw-r--r--   0        0        0       68 2024-03-18 13:18:48.992629 cumulus_library_data_metrics-0.0.0/tests/data/meta/general/condition/0.ndjson
--rw-r--r--   0        0        0       74 2024-03-18 13:18:48.992629 cumulus_library_data_metrics-0.0.0/tests/data/meta/general/encounter/0.ndjson
--rw-r--r--   0        0        0       40 2024-03-18 13:18:48.992629 cumulus_library_data_metrics-0.0.0/tests/data/meta/general/expected_date.csv
--rw-r--r--   0        0        0       23 2024-03-18 13:18:48.992629 cumulus_library_data_metrics-0.0.0/tests/data/meta/general/expected_version.csv
--rw-r--r--   0        0        0      246 2024-03-18 13:18:48.992629 cumulus_library_data_metrics-0.0.0/tests/data/meta/general/observation/0.ndjson
--rw-r--r--   0        0        0       12 2024-03-18 13:18:48.992629 cumulus_library_data_metrics-0.0.0/tests/data/meta/general/patient/0.ndjson
--rw-r--r--   0        0        0      269 2024-03-18 13:21:06.170254 cumulus_library_data_metrics-0.0.0/tests/data/q_date_recent/general/condition/0.ndjson
--rw-r--r--   0        0        0      221 2024-03-18 13:21:06.170254 cumulus_library_data_metrics-0.0.0/tests/data/q_date_recent/general/encounter/0.ndjson
--rw-r--r--   0        0        0      138 2024-03-18 13:21:06.170254 cumulus_library_data_metrics-0.0.0/tests/data/q_date_recent/general/expected_condition.csv
--rw-r--r--   0        0        0       44 2024-03-18 13:21:06.170254 cumulus_library_data_metrics-0.0.0/tests/data/q_date_recent/general/expected_encounter.csv
--rw-r--r--   0        0        0       76 2024-03-18 13:21:06.170254 cumulus_library_data_metrics-0.0.0/tests/data/q_date_recent/general/expected_procedure.csv
--rw-r--r--   0        0        0      238 2024-03-18 13:21:06.170254 cumulus_library_data_metrics-0.0.0/tests/data/q_date_recent/general/expected_summary.csv
--rw-r--r--   0        0        0      262 2024-03-18 13:21:06.170254 cumulus_library_data_metrics-0.0.0/tests/data/q_date_recent/general/procedure/0.ndjson
--rw-r--r--   0        0        0       55 2023-11-27 16:09:57.472333 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_pop/general/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0       55 2023-11-27 16:12:42.650951 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_pop/general/condition/0.ndjson
--rw-r--r--   0        0        0       55 2023-11-27 15:59:16.453940 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_pop/general/device/0.ndjson
--rw-r--r--   0        0        0       55 2023-11-27 16:12:50.395073 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_pop/general/diagnosticreport/0.ndjson
--rw-r--r--   0        0        0       55 2023-11-27 16:12:50.395073 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_pop/general/documentreference/0.ndjson
--rw-r--r--   0        0        0       55 2024-05-09 14:45:04.527709 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_pop/general/encounter/0.ndjson
--rw-r--r--   0        0        0      451 2024-05-09 14:45:04.527709 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_pop/general/expected_summary.csv
--rw-r--r--   0        0        0       55 2023-11-27 16:09:57.472333 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_pop/general/immunization/0.ndjson
--rw-r--r--   0        0        0       55 2023-11-27 16:13:04.515297 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_pop/general/medicationrequest/0.ndjson
--rw-r--r--   0        0        0       55 2023-11-27 16:13:11.831412 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_pop/general/observation/0.ndjson
--rw-r--r--   0        0        0      198 2023-11-27 20:37:42.221598 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_pop/general/procedure/0.ndjson
--rw-r--r--   0        0        0       98 2023-11-27 19:40:48.088266 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0       98 2023-11-27 19:40:58.224377 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/condition/0.ndjson
--rw-r--r--   0        0        0       98 2023-11-27 19:41:05.780461 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/device/0.ndjson
--rw-r--r--   0        0        0       98 2024-01-08 20:12:29.894941 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/diagnosticreport/0.ndjson
--rw-r--r--   0        0        0      603 2023-11-27 21:04:31.485129 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/documentreference/0.ndjson
--rw-r--r--   0        0        0       51 2024-05-09 14:45:04.527709 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/encounter/0.ndjson
--rw-r--r--   0        0        0      122 2024-01-22 15:57:40.952559 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/expected_documentreference_encounter.csv
--rw-r--r--   0        0        0      107 2024-01-22 15:54:42.137639 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/expected_procedure_encounter.csv
--rw-r--r--   0        0        0      787 2024-05-09 14:45:04.527709 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/expected_summary.csv
--rw-r--r--   0        0        0       98 2023-11-27 19:41:55.821012 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/immunization/0.ndjson
--rw-r--r--   0        0        0       98 2023-11-27 19:42:00.397063 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/medicationrequest/0.ndjson
--rw-r--r--   0        0        0       98 2023-11-27 19:42:04.109104 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/observation/0.ndjson
--rw-r--r--   0        0        0       12 2023-11-27 19:39:52.447652 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/patient/0.ndjson
--rw-r--r--   0        0        0      890 2023-11-27 20:55:41.312899 cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/procedure/0.ndjson
--rw-r--r--   0        0        0       77 2023-12-08 19:45:39.832290 cumulus_library_data_metrics-0.0.0/tests/data/q_term_use/general/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0       77 2023-11-28 14:22:12.264165 cumulus_library_data_metrics-0.0.0/tests/data/q_term_use/general/condition/0.ndjson
--rw-r--r--   0        0        0       77 2023-11-28 14:22:24.044290 cumulus_library_data_metrics-0.0.0/tests/data/q_term_use/general/device/0.ndjson
--rw-r--r--   0        0        0       71 2024-01-08 20:15:08.156746 cumulus_library_data_metrics-0.0.0/tests/data/q_term_use/general/diagnosticreport/0.ndjson
--rw-r--r--   0        0        0       71 2023-11-28 14:22:44.880511 cumulus_library_data_metrics-0.0.0/tests/data/q_term_use/general/documentreference/0.ndjson
--rw-r--r--   0        0        0      498 2024-02-29 12:05:58.504489 cumulus_library_data_metrics-0.0.0/tests/data/q_term_use/general/expected_summary.csv
--rw-r--r--   0        0        0       89 2023-11-28 14:23:11.288791 cumulus_library_data_metrics-0.0.0/tests/data/q_term_use/general/immunization/0.ndjson
--rw-r--r--   0        0        0       98 2023-11-28 14:25:21.506176 cumulus_library_data_metrics-0.0.0/tests/data/q_term_use/general/medication/0.ndjson
--rw-r--r--   0        0        0      119 2023-11-28 14:25:37.254344 cumulus_library_data_metrics-0.0.0/tests/data/q_term_use/general/medicationrequest/0.ndjson
--rw-r--r--   0        0        0      175 2023-11-28 14:26:30.402911 cumulus_library_data_metrics-0.0.0/tests/data/q_term_use/general/observation/0.ndjson
--rw-r--r--   0        0        0      452 2024-02-28 14:28:47.785074 cumulus_library_data_metrics-0.0.0/tests/data/q_term_use/general/procedure/0.ndjson
--rw-r--r--   0        0        0      178 2024-04-12 13:09:48.084692 cumulus_library_data_metrics-0.0.0/tests/data/q_valid_us_core_v4/general/encounter/0.ndjson
--rw-r--r--   0        0        0      155 2024-04-12 13:09:48.088692 cumulus_library_data_metrics-0.0.0/tests/data/q_valid_us_core_v4/general/expected_encounter.csv
--rw-r--r--   0        0        0      344 2024-02-29 12:05:00.591966 cumulus_library_data_metrics-0.0.0/tests/data/q_valid_us_core_v4/general/expected_summary.csv
--rw-r--r--   0        0        0       18 2024-01-29 15:15:10.961103 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/allergy-low-schema/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0      146 2024-04-12 13:09:48.088692 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/allergy-low-schema/expected_allergyintolerance_mandatory.csv
--rw-r--r--   0        0        0       90 2024-02-05 19:51:46.283395 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/allergy-low-schema/expected_allergyintolerance_must_support.csv
--rw-r--r--   0        0        0       18 2024-02-05 19:52:27.928068 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/docref-low-schema/documentreference/0.ndjson
--rw-r--r--   0        0        0      125 2024-02-05 19:52:51.732453 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/docref-low-schema/expected_documentreference_mandatory.csv
--rw-r--r--   0        0        0      119 2024-02-05 21:58:02.063303 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/docref-low-schema/expected_documentreference_must_support.csv
--rw-r--r--   0        0        0       18 2024-02-05 19:52:27.928068 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/encounter-low-schema/encounter/0.ndjson
--rw-r--r--   0        0        0       97 2024-02-15 15:06:47.940666 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/encounter-low-schema/expected_encounter_mandatory.csv
--rw-r--r--   0        0        0      145 2024-02-15 15:06:56.368788 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/encounter-low-schema/expected_encounter_must_support.csv
--rw-r--r--   0        0        0     2788 2024-04-12 13:09:48.088692 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0     2723 2024-04-12 13:09:48.088692 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/condition/0.ndjson
--rw-r--r--   0        0        0     1527 2023-12-15 14:07:00.823562 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/diagnosticreport/0.ndjson
--rw-r--r--   0        0        0     1407 2024-04-12 13:09:48.088692 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/documentreference/0.ndjson
--rw-r--r--   0        0        0      827 2023-12-15 14:15:26.174219 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/encounter/0.ndjson
--rw-r--r--   0        0        0      945 2024-04-12 13:09:48.092692 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_allergyintolerance_mandatory.csv
--rw-r--r--   0        0        0     1048 2024-04-12 13:09:48.092692 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_condition_mandatory.csv
--rw-r--r--   0        0        0      610 2024-02-05 19:24:01.171508 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_diagnosticreport_note_mandatory.csv
--rw-r--r--   0        0        0      763 2024-04-08 20:20:09.627186 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_documentreference_mandatory.csv
--rw-r--r--   0        0        0      395 2024-02-05 19:26:56.574663 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_encounter_mandatory.csv
--rw-r--r--   0        0        0      377 2024-02-05 19:27:34.503331 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_immunization_mandatory.csv
--rw-r--r--   0        0        0       80 2024-02-05 19:28:15.816055 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_medication_mandatory.csv
--rw-r--r--   0        0        0      497 2024-04-12 13:09:48.092692 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_medicationrequest_mandatory.csv
--rw-r--r--   0        0        0     1682 2024-02-05 19:31:50.583748 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_laboratory_mandatory.csv
--rw-r--r--   0        0        0      620 2024-04-12 13:09:48.096692 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_smoking_status_mandatory.csv
--rw-r--r--   0        0        0     1238 2024-02-05 19:32:44.076654 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_vital_signs_mandatory.csv
--rw-r--r--   0        0        0      164 2024-03-18 13:18:48.992629 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_patient_mandatory.csv
--rw-r--r--   0        0        0      510 2024-02-05 19:33:07.505050 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_procedure_mandatory.csv
--rw-r--r--   0        0        0      894 2023-12-15 14:39:26.882868 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/immunization/0.ndjson
--rw-r--r--   0        0        0      109 2023-12-15 14:43:56.834629 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/medication/0.ndjson
--rw-r--r--   0        0        0      937 2024-04-12 13:09:48.096692 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/medicationrequest/0.ndjson
--rw-r--r--   0        0        0     6994 2024-01-08 19:47:31.085636 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/observation/labs.ndjson
--rw-r--r--   0        0        0     1471 2024-04-12 13:09:48.096692 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/observation/smoking.ndjson
--rw-r--r--   0        0        0     3357 2024-01-26 20:13:23.226444 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/observation/vitals.ndjson
--rw-r--r--   0        0        0      191 2024-03-18 13:18:48.992629 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/patient/0.ndjson
--rw-r--r--   0        0        0     1358 2024-01-08 20:49:08.655956 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/procedure/0.ndjson
--rw-r--r--   0        0        0      799 2024-02-05 21:27:17.611578 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/allergyintolerance/0.ndjson
--rw-r--r--   0        0        0      237 2024-02-05 21:30:05.801896 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/condition/0.ndjson
--rw-r--r--   0        0        0      210 2024-02-05 21:36:08.878953 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/diagnosticreport/0.ndjson
--rw-r--r--   0        0        0      714 2024-02-05 21:56:30.041804 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/documentreference/0.ndjson
--rw-r--r--   0        0        0      598 2024-02-15 15:04:41.422840 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/encounter/0.ndjson
--rw-r--r--   0        0        0      371 2024-02-05 21:26:19.386780 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/expected_allergyintolerance_must_support.csv
--rw-r--r--   0        0        0      106 2024-02-05 21:32:33.375944 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/expected_condition_must_support.csv
--rw-r--r--   0        0        0      195 2024-02-05 21:36:25.163181 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/expected_diagnosticreport_note_must_support.csv
--rw-r--r--   0        0        0      441 2024-02-05 21:56:48.986114 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/expected_documentreference_must_support.csv
--rw-r--r--   0        0        0      364 2024-02-15 15:05:41.247704 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/expected_encounter_must_support.csv
--rw-r--r--   0        0        0      207 2024-02-15 15:19:36.103304 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/expected_immunization_must_support.csv
--rw-r--r--   0        0        0       22 2024-02-15 15:24:57.351300 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/expected_medication_must_support.csv
--rw-r--r--   0        0        0      236 2024-04-12 13:09:48.096692 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/expected_medicationrequest_must_support.csv
--rw-r--r--   0        0        0      141 2024-02-06 19:56:17.052559 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/expected_observation_laboratory_must_support.csv
--rw-r--r--   0        0        0       30 2024-02-15 15:43:34.886519 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/expected_observation_smoking_status_must_support.csv
--rw-r--r--   0        0        0      173 2024-02-16 13:51:53.850726 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/expected_observation_vital_signs_must_support.csv
--rw-r--r--   0        0        0      637 2024-02-09 16:15:29.565807 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/expected_patient_must_support.csv
--rw-r--r--   0        0        0       22 2024-02-15 15:24:57.351300 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/expected_procedure_must_support.csv
--rw-r--r--   0        0        0      296 2024-02-15 15:19:56.015541 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/immunization/0.ndjson
--rw-r--r--   0        0        0       18 2024-02-15 15:24:34.283002 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/medication/0.ndjson
--rw-r--r--   0        0        0      313 2024-04-12 13:09:48.100692 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/medicationrequest/0.ndjson
--rw-r--r--   0        0        0      901 2024-02-07 16:24:20.443797 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/observation/labs.ndjson
--rw-r--r--   0        0        0       18 2024-02-06 16:13:58.288869 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/observation/nothing.ndjson
--rw-r--r--   0        0        0       99 2024-02-15 15:42:27.837583 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/observation/smoking.ndjson
--rw-r--r--   0        0        0      773 2024-02-15 16:39:40.839525 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/observation/vitals.ndjson
--rw-r--r--   0        0        0     1652 2024-02-09 16:10:25.617488 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/patient/0.ndjson
--rw-r--r--   0        0        0       18 2024-02-15 15:24:34.283002 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/procedure/0.ndjson
--rw-r--r--   0        0        0      165 2024-02-08 20:47:37.932563 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/obs-low-schema/expected_observation_laboratory_mandatory.csv
--rw-r--r--   0        0        0       50 2024-02-08 20:48:00.885341 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/obs-low-schema/expected_observation_laboratory_must_support.csv
--rw-r--r--   0        0        0      147 2024-02-08 20:47:16.739848 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/obs-low-schema/observation/0.ndjson
--rw-r--r--   0        0        0       57 2024-02-09 16:04:05.483412 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/patient-low-schema/expected_patient_mandatory.csv
--rw-r--r--   0        0        0      152 2024-02-09 16:04:35.482888 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/patient-low-schema/expected_patient_must_support.csv
--rw-r--r--   0        0        0       18 2024-02-05 19:52:27.928068 cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/patient-low-schema/patient/0.ndjson
--rw-r--r--   0        0        0     5816 2024-05-10 16:22:00.022863 cumulus_library_data_metrics-0.0.0/tests/test_metrics.py
--rw-r--r--   0        0        0     5247 1970-01-01 00:00:00.000000 cumulus_library_data_metrics-0.0.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/LICENSE
+-rw-r--r--   0        0        0     3362 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/README.md
+-rw-r--r--   0        0        0       68 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/__init__.py
+-rw-r--r--   0        0        0     3332 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/base.py
+-rw-r--r--   0        0        0     1434 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/base.summary.jinja
+-rw-r--r--   0        0        0      899 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_count/README.md
+-rw-r--r--   0        0        0     1113 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_count/c_pt_count.jinja
+-rw-r--r--   0        0        0      909 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_count/c_pt_count.py
+-rw-r--r--   0        0        0      308 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_deceased_count/README.md
+-rw-r--r--   0        0        0     1861 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_deceased_count/c_pt_deceased_count.jinja
+-rw-r--r--   0        0        0      550 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_deceased_count/c_pt_deceased_count.py
+-rw-r--r--   0        0        0      265 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resource_count/README.md
+-rw-r--r--   0        0        0     1099 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resource_count/c_resource_count.jinja
+-rw-r--r--   0        0        0     1068 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resource_count/c_resource_count.py
+-rw-r--r--   0        0        0      347 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resources_per_pt/README.md
+-rw-r--r--   0        0        0     2545 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resources_per_pt/c_resources_per_pt.jinja
+-rw-r--r--   0        0        0      929 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resources_per_pt/c_resources_per_pt.py
+-rw-r--r--   0        0        0     1057 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_term_coverage/README.md
+-rw-r--r--   0        0        0     2083 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_term_coverage/c_term_coverage.jinja
+-rw-r--r--   0        0        0     2205 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_term_coverage/c_term_coverage.py
+-rw-r--r--   0        0        0     2075 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_us_core_v4_count/README.md
+-rw-r--r--   0        0        0     1595 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_us_core_v4_count/c_us_core_v4_count.jinja
+-rw-r--r--   0        0        0      433 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_us_core_v4_count/c_us_core_v4_count.py
+-rw-r--r--   0        0        0     3647 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/manifest.toml
+-rw-r--r--   0        0        0     1078 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/meta/dates.jinja
+-rw-r--r--   0        0        0      735 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/meta/meta.py
+-rw-r--r--   0        0        0       77 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/meta/version.jinja
+-rw-r--r--   0        0        0      904 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_date_recent/README.md
+-rw-r--r--   0        0        0     1234 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_date_recent/q_date_recent.jinja
+-rw-r--r--   0        0        0      812 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_date_recent/q_date_recent.py
+-rw-r--r--   0        0        0     1420 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_pop/README.md
+-rw-r--r--   0        0        0      374 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_pop/q_ref_target_pop.jinja
+-rw-r--r--   0        0        0     1531 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_pop/q_ref_target_pop.py
+-rw-r--r--   0        0        0     1195 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_valid/README.md
+-rw-r--r--   0        0        0      504 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_valid/denominator.jinja
+-rw-r--r--   0        0        0      991 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_valid/q_ref_target_valid.jinja
+-rw-r--r--   0        0        0     2581 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_valid/q_ref_target_valid.py
+-rw-r--r--   0        0        0      736 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_term_use/README.md
+-rw-r--r--   0        0        0      947 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_term_use/q_term_use.jinja
+-rw-r--r--   0        0        0     3235 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_term_use/q_term_use.py
+-rw-r--r--   0        0        0     3587 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/README.md
+-rw-r--r--   0        0        0      738 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.jinja
+-rw-r--r--   0        0        0      688 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.py
+-rw-r--r--   0        0        0     2509 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/resource_info.py
+-rw-r--r--   0        0        0     2046 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/systems.py
+-rw-r--r--   0        0        0      105 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/t_us_core_v4/README.md
+-rw-r--r--   0        0        0      182 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/t_us_core_v4/mandatory.jinja
+-rw-r--r--   0        0        0      225 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/t_us_core_v4/must_support.jinja
+-rw-r--r--   0        0        0      815 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/t_us_core_v4/t_us_core_v4.py
+-rw-r--r--   0        0        0      345 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/README.md
+-rw-r--r--   0        0        0       50 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/__init__.py
+-rw-r--r--   0        0        0     2453 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/allergyintolerance_mandatory.jinja
+-rw-r--r--   0        0        0     2666 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/allergyintolerance_must_support.jinja
+-rw-r--r--   0        0        0     2603 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/condition_mandatory.jinja
+-rw-r--r--   0        0        0     1414 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/condition_must_support.jinja
+-rw-r--r--   0        0        0     1180 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_note_mandatory.jinja
+-rw-r--r--   0        0        0      763 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_note_must_support.jinja
+-rw-r--r--   0        0        0     2129 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/documentreference_mandatory.jinja
+-rw-r--r--   0        0        0     2945 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/documentreference_must_support.jinja
+-rw-r--r--   0        0        0      834 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/encounter_mandatory.jinja
+-rw-r--r--   0        0        0     1503 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/encounter_must_support.jinja
+-rw-r--r--   0        0        0      954 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/immunization_mandatory.jinja
+-rw-r--r--   0        0        0      570 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/immunization_must_support.jinja
+-rw-r--r--   0        0        0      356 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/medication_mandatory.jinja
+-rw-r--r--   0        0        0      129 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/medication_must_support.jinja
+-rw-r--r--   0        0        0     1322 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/medicationrequest_mandatory.jinja
+-rw-r--r--   0        0        0     1018 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/medicationrequest_must_support.jinja
+-rw-r--r--   0        0        0      316 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_blood_pressure_mandatory.jinja
+-rw-r--r--   0        0        0     2291 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_laboratory_mandatory.jinja
+-rw-r--r--   0        0        0     1024 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_laboratory_must_support.jinja
+-rw-r--r--   0        0        0     1974 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_smoking_status_mandatory.jinja
+-rw-r--r--   0        0        0      190 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_smoking_status_must_support.jinja
+-rw-r--r--   0        0        0     3804 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_utils.jinja
+-rw-r--r--   0        0        0     4855 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_vital_signs_mandatory.jinja
+-rw-r--r--   0        0        0     1032 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_vital_signs_must_support.jinja
+-rw-r--r--   0        0        0      619 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/patient_mandatory.jinja
+-rw-r--r--   0        0        0     2503 2024-05-16 17:48:34.034490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/patient_must_support.jinja
+-rw-r--r--   0        0        0     5242 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/patient_utils.jinja
+-rw-r--r--   0        0        0     1004 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/procedure_mandatory.jinja
+-rw-r--r--   0        0        0      128 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/procedure_must_support.jinja
+-rw-r--r--   0        0        0     3546 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/profiles.py
+-rw-r--r--   0        0        0      398 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/slice.jinja
+-rw-r--r--   0        0        0     9285 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/utils.jinja
+-rw-r--r--   0        0        0     1599 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/__init__.py
+-rw-r--r--   0        0        0     9018 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/cubed/expected.csv
+-rw-r--r--   0        0        0     3065 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/cubed/patient/0.ndjson
+-rw-r--r--   0        0        0      679 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/general/expected.csv
+-rw-r--r--   0        0        0     3065 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/general/patient/0.ndjson
+-rw-r--r--   0        0        0      122 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/no-ext/expected.csv
+-rw-r--r--   0        0        0       33 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/no-ext/patient/0.ndjson
+-rw-r--r--   0        0        0      269 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_deceased_count/general/expected.csv
+-rw-r--r--   0        0        0      786 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_pt_deceased_count/general/patient/0.ndjson
+-rw-r--r--   0        0        0     1334 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0     1978 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/condition/0.ndjson
+-rw-r--r--   0        0        0       24 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/device/0.ndjson
+-rw-r--r--   0        0        0      494 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/diagnosticreport/0.ndjson
+-rw-r--r--   0        0        0      593 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/documentreference/0.ndjson
+-rw-r--r--   0        0        0      603 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/encounter/0.ndjson
+-rw-r--r--   0        0        0      417 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_allergyintolerance_month.csv
+-rw-r--r--   0        0        0      375 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_allergyintolerance_year.csv
+-rw-r--r--   0        0        0      456 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_condition_month.csv
+-rw-r--r--   0        0        0      354 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_condition_year.csv
+-rw-r--r--   0        0        0       27 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_device_all.csv
+-rw-r--r--   0        0        0      200 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_diagnosticreport_month.csv
+-rw-r--r--   0        0        0      190 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_diagnosticreport_year.csv
+-rw-r--r--   0        0        0      225 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_documentreference_month.csv
+-rw-r--r--   0        0        0      215 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_documentreference_year.csv
+-rw-r--r--   0        0        0      203 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_encounter_month.csv
+-rw-r--r--   0        0        0      193 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_encounter_year.csv
+-rw-r--r--   0        0        0      114 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_immunization_month.csv
+-rw-r--r--   0        0        0      104 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_immunization_year.csv
+-rw-r--r--   0        0        0       27 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_medication_all.csv
+-rw-r--r--   0        0        0      144 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_medicationrequest_month.csv
+-rw-r--r--   0        0        0      140 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_medicationrequest_year.csv
+-rw-r--r--   0        0        0      273 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_observation_month.csv
+-rw-r--r--   0        0        0      257 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_observation_year.csv
+-rw-r--r--   0        0        0       47 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_patient_all.csv
+-rw-r--r--   0        0        0      178 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_procedure_month.csv
+-rw-r--r--   0        0        0      147 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/expected_procedure_year.csv
+-rw-r--r--   0        0        0      203 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/immunization/0.ndjson
+-rw-r--r--   0        0        0       36 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/medication/0.ndjson
+-rw-r--r--   0        0        0      342 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0      934 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/observation/0.ndjson
+-rw-r--r--   0        0        0       87 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/patient/0.ndjson
+-rw-r--r--   0        0        0      310 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/procedure/0.ndjson
+-rw-r--r--   0        0        0      118 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resources_per_pt/general/condition/0.ndjson
+-rw-r--r--   0        0        0      544 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resources_per_pt/general/expected_summary.csv
+-rw-r--r--   0        0        0     1264 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resources_per_pt/general/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0       36 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_resources_per_pt/general/patient/0.ndjson
+-rw-r--r--   0        0        0     1082 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0     1408 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/condition/0.ndjson
+-rw-r--r--   0        0        0      105 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/device/0.ndjson
+-rw-r--r--   0        0        0      105 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/diagnosticreport/0.ndjson
+-rw-r--r--   0        0        0      105 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/documentreference/0.ndjson
+-rw-r--r--   0        0        0      383 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/encounter/0.ndjson
+-rw-r--r--   0        0        0      308 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_allergyintolerance_code.csv
+-rw-r--r--   0        0        0      368 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_condition_code.csv
+-rw-r--r--   0        0        0       73 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_device_type.csv
+-rw-r--r--   0        0        0      106 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_diagnosticreport_code.csv
+-rw-r--r--   0        0        0      106 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_documentreference_type.csv
+-rw-r--r--   0        0        0      105 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_encounter_class.csv
+-rw-r--r--   0        0        0      147 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_encounter_type.csv
+-rw-r--r--   0        0        0      106 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_immunization_vaccinecode.csv
+-rw-r--r--   0        0        0       73 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_medication_code.csv
+-rw-r--r--   0        0        0      106 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_medicationrequest_medicationcodeableconcept.csv
+-rw-r--r--   0        0        0      281 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_observation_code.csv
+-rw-r--r--   0        0        0      308 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_observation_valuecodeableconcept.csv
+-rw-r--r--   0        0        0      106 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/expected_procedure_code.csv
+-rw-r--r--   0        0        0      112 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/immunization/0.ndjson
+-rw-r--r--   0        0        0      105 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/medication/0.ndjson
+-rw-r--r--   0        0        0      126 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0     1415 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/observation/0.ndjson
+-rw-r--r--   0        0        0      105 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/procedure/0.ndjson
+-rw-r--r--   0        0        0      842 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_us_core_v4_count/general/documentreference/0.ndjson
+-rw-r--r--   0        0        0      254 2024-05-16 17:48:34.038490 cumulus_library_data_metrics-1.0.0/tests/data/c_us_core_v4_count/general/expected_documentreference.csv
+-rw-r--r--   0        0        0       68 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/meta/general/condition/0.ndjson
+-rw-r--r--   0        0        0       74 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/meta/general/encounter/0.ndjson
+-rw-r--r--   0        0        0       40 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/meta/general/expected_date.csv
+-rw-r--r--   0        0        0       23 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/meta/general/expected_version.csv
+-rw-r--r--   0        0        0      246 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/meta/general/observation/0.ndjson
+-rw-r--r--   0        0        0       12 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/meta/general/patient/0.ndjson
+-rw-r--r--   0        0        0      269 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_date_recent/general/condition/0.ndjson
+-rw-r--r--   0        0        0      221 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_date_recent/general/encounter/0.ndjson
+-rw-r--r--   0        0        0      138 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_date_recent/general/expected_condition.csv
+-rw-r--r--   0        0        0       44 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_date_recent/general/expected_encounter.csv
+-rw-r--r--   0        0        0       76 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_date_recent/general/expected_procedure.csv
+-rw-r--r--   0        0        0      238 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_date_recent/general/expected_summary.csv
+-rw-r--r--   0        0        0      262 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_date_recent/general/procedure/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/condition/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/device/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/diagnosticreport/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/documentreference/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/encounter/0.ndjson
+-rw-r--r--   0        0        0      451 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/expected_summary.csv
+-rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/immunization/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0       55 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/observation/0.ndjson
+-rw-r--r--   0        0        0      198 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_pop/general/procedure/0.ndjson
+-rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/condition/0.ndjson
+-rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/device/0.ndjson
+-rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/diagnosticreport/0.ndjson
+-rw-r--r--   0        0        0      603 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/documentreference/0.ndjson
+-rw-r--r--   0        0        0       51 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/encounter/0.ndjson
+-rw-r--r--   0        0        0      122 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/expected_documentreference_encounter.csv
+-rw-r--r--   0        0        0      107 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/expected_procedure_encounter.csv
+-rw-r--r--   0        0        0      787 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/expected_summary.csv
+-rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/immunization/0.ndjson
+-rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/observation/0.ndjson
+-rw-r--r--   0        0        0       12 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/patient/0.ndjson
+-rw-r--r--   0        0        0      890 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/procedure/0.ndjson
+-rw-r--r--   0        0        0       77 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0       77 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/condition/0.ndjson
+-rw-r--r--   0        0        0       77 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/device/0.ndjson
+-rw-r--r--   0        0        0       71 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/diagnosticreport/0.ndjson
+-rw-r--r--   0        0        0       71 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/documentreference/0.ndjson
+-rw-r--r--   0        0        0      498 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/expected_summary.csv
+-rw-r--r--   0        0        0       89 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/immunization/0.ndjson
+-rw-r--r--   0        0        0       98 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/medication/0.ndjson
+-rw-r--r--   0        0        0      119 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0      175 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/observation/0.ndjson
+-rw-r--r--   0        0        0      452 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_term_use/general/procedure/0.ndjson
+-rw-r--r--   0        0        0      178 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_valid_us_core_v4/general/encounter/0.ndjson
+-rw-r--r--   0        0        0      155 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_valid_us_core_v4/general/expected_encounter.csv
+-rw-r--r--   0        0        0      344 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/q_valid_us_core_v4/general/expected_summary.csv
+-rw-r--r--   0        0        0       18 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/allergy-low-schema/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0      146 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/allergy-low-schema/expected_allergyintolerance_mandatory.csv
+-rw-r--r--   0        0        0       90 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/allergy-low-schema/expected_allergyintolerance_must_support.csv
+-rw-r--r--   0        0        0       18 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/docref-low-schema/documentreference/0.ndjson
+-rw-r--r--   0        0        0      125 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/docref-low-schema/expected_documentreference_mandatory.csv
+-rw-r--r--   0        0        0      119 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/docref-low-schema/expected_documentreference_must_support.csv
+-rw-r--r--   0        0        0       18 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/encounter-low-schema/encounter/0.ndjson
+-rw-r--r--   0        0        0       97 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/encounter-low-schema/expected_encounter_mandatory.csv
+-rw-r--r--   0        0        0      145 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/encounter-low-schema/expected_encounter_must_support.csv
+-rw-r--r--   0        0        0     2788 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0     2723 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/condition/0.ndjson
+-rw-r--r--   0        0        0     1527 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/diagnosticreport/0.ndjson
+-rw-r--r--   0        0        0     1407 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/documentreference/0.ndjson
+-rw-r--r--   0        0        0      827 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/encounter/0.ndjson
+-rw-r--r--   0        0        0      945 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_allergyintolerance_mandatory.csv
+-rw-r--r--   0        0        0     1048 2024-05-16 17:48:34.042490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_condition_mandatory.csv
+-rw-r--r--   0        0        0      610 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_diagnosticreport_note_mandatory.csv
+-rw-r--r--   0        0        0      763 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_documentreference_mandatory.csv
+-rw-r--r--   0        0        0      395 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_encounter_mandatory.csv
+-rw-r--r--   0        0        0      377 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_immunization_mandatory.csv
+-rw-r--r--   0        0        0       80 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_medication_mandatory.csv
+-rw-r--r--   0        0        0      497 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_medicationrequest_mandatory.csv
+-rw-r--r--   0        0        0     1682 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_laboratory_mandatory.csv
+-rw-r--r--   0        0        0      620 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_smoking_status_mandatory.csv
+-rw-r--r--   0        0        0     1238 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_vital_signs_mandatory.csv
+-rw-r--r--   0        0        0      164 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_patient_mandatory.csv
+-rw-r--r--   0        0        0      510 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_procedure_mandatory.csv
+-rw-r--r--   0        0        0      894 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/immunization/0.ndjson
+-rw-r--r--   0        0        0      109 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/medication/0.ndjson
+-rw-r--r--   0        0        0      937 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0     6994 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/observation/labs.ndjson
+-rw-r--r--   0        0        0     1471 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/observation/smoking.ndjson
+-rw-r--r--   0        0        0     3357 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/observation/vitals.ndjson
+-rw-r--r--   0        0        0      191 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/patient/0.ndjson
+-rw-r--r--   0        0        0     1358 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/procedure/0.ndjson
+-rw-r--r--   0        0        0      799 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/allergyintolerance/0.ndjson
+-rw-r--r--   0        0        0      237 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/condition/0.ndjson
+-rw-r--r--   0        0        0      210 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/diagnosticreport/0.ndjson
+-rw-r--r--   0        0        0      714 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/documentreference/0.ndjson
+-rw-r--r--   0        0        0      598 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/encounter/0.ndjson
+-rw-r--r--   0        0        0      371 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_allergyintolerance_must_support.csv
+-rw-r--r--   0        0        0      106 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_condition_must_support.csv
+-rw-r--r--   0        0        0      195 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_diagnosticreport_note_must_support.csv
+-rw-r--r--   0        0        0      441 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_documentreference_must_support.csv
+-rw-r--r--   0        0        0      364 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_encounter_must_support.csv
+-rw-r--r--   0        0        0      207 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_immunization_must_support.csv
+-rw-r--r--   0        0        0       22 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_medication_must_support.csv
+-rw-r--r--   0        0        0      236 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_medicationrequest_must_support.csv
+-rw-r--r--   0        0        0      141 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_observation_laboratory_must_support.csv
+-rw-r--r--   0        0        0       30 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_observation_smoking_status_must_support.csv
+-rw-r--r--   0        0        0      173 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_observation_vital_signs_must_support.csv
+-rw-r--r--   0        0        0      637 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_patient_must_support.csv
+-rw-r--r--   0        0        0       22 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_procedure_must_support.csv
+-rw-r--r--   0        0        0      296 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/immunization/0.ndjson
+-rw-r--r--   0        0        0       18 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/medication/0.ndjson
+-rw-r--r--   0        0        0      313 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/medicationrequest/0.ndjson
+-rw-r--r--   0        0        0      901 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/observation/labs.ndjson
+-rw-r--r--   0        0        0       18 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/observation/nothing.ndjson
+-rw-r--r--   0        0        0       99 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/observation/smoking.ndjson
+-rw-r--r--   0        0        0      773 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/observation/vitals.ndjson
+-rw-r--r--   0        0        0     1652 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/patient/0.ndjson
+-rw-r--r--   0        0        0       18 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/procedure/0.ndjson
+-rw-r--r--   0        0        0      165 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/obs-low-schema/expected_observation_laboratory_mandatory.csv
+-rw-r--r--   0        0        0       50 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/obs-low-schema/expected_observation_laboratory_must_support.csv
+-rw-r--r--   0        0        0      147 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/obs-low-schema/observation/0.ndjson
+-rw-r--r--   0        0        0       57 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/patient-low-schema/expected_patient_mandatory.csv
+-rw-r--r--   0        0        0      152 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/patient-low-schema/expected_patient_must_support.csv
+-rw-r--r--   0        0        0       18 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/patient-low-schema/patient/0.ndjson
+-rw-r--r--   0        0        0     6243 2024-05-16 17:48:34.046490 cumulus_library_data_metrics-1.0.0/tests/test_metrics.py
+-rw-r--r--   0        0        0     4253 1970-01-01 00:00:00.000000 cumulus_library_data_metrics-1.0.0/PKG-INFO
```

### Comparing `cumulus_library_data_metrics-0.0.0/LICENSE` & `cumulus_library_data_metrics-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/base.py` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 """Module for generating q_ref_target_pop tables"""
 
 import copy
 import os.path
 from typing import ClassVar
 
 import jinja2
-from cumulus_library import databases
-from cumulus_library.template_sql import base_templates
+from cumulus_library import base_utils
+from cumulus_library.template_sql import sql_utils
 
-from cumulus_library_data_metrics.data_metrics import resource_info
+from cumulus_library_data_metrics import resource_info
 
 
 class MetricMixin:
     name = "base"
     uses_fields: ClassVar[dict] = {}
 
     def __init__(self):
@@ -27,55 +27,47 @@
         self.date_fields = copy.deepcopy(resource_info.DATES)
 
     def make_summary(self) -> None:
         """Makes a summary table, from all the individual metric tables"""
         sql = self.render_sql("../base.summary", entries=self.summary_entries, metric=self.name)
         self.queries.append(sql)
 
-    def _query_schema(
-        self, cursor: databases.DatabaseCursor, schema: str, parser: databases.DatabaseParser
-    ) -> None:
+    def _query_schema(self, config: base_utils.StudyConfig) -> None:
         fields_to_check = copy.deepcopy(self.uses_fields)
 
         # Since so many metrics use date data, add a standard date field into the mix
         check_docref_period = "context.period.start" in self.date_fields["DocumentReference"]
         if check_docref_period:
             docref = fields_to_check.setdefault("DocumentReference", {})
             context = docref.setdefault("context", {})
             period = context.setdefault("period", {})
             period["start"] = {}
 
-        for table, cols in fields_to_check.items():
-            query = base_templates.get_column_datatype_query(schema, table.lower(), cols.keys())
-            cursor.execute(query)
-            table_schema = cursor.fetchall()
-            self.schemas[table] = parser.validate_table_schema(cols, table_schema)
+        self.schemas = sql_utils.validate_schema(config.db, fields_to_check)
 
         if (
             check_docref_period
             and not self.schemas["DocumentReference"]["context"]["period"]["start"]
         ):
             self.date_fields["DocumentReference"].remove("context.period.start")
 
-    def extra_schema_checks(self, cursor: databases.DatabaseCursor, schema: str) -> None:
+    def extra_schema_checks(self, config: base_utils.StudyConfig) -> None:
         pass
 
     def add_metric_queries(self) -> None:
         pass
 
     def prepare_queries(
         self,
-        cursor: databases.DatabaseCursor,
-        schema: str,
         *args,
-        parser: databases.DatabaseParser,
+        config: base_utils.StudyConfig,
         **kwargs,
     ) -> None:
-        self._query_schema(cursor, schema, parser)
-        self.extra_schema_checks(cursor, schema)
+        self._query_schema(config)
+        self.extra_schema_checks(config)
         self.add_metric_queries()
 
     def render_sql(self, template: str, **kwargs) -> str:
         path = os.path.dirname(__file__)
 
         if src := kwargs.get("src"):
             kwargs["dates"] = self.date_fields.get(src)
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/base.summary.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/base.summary.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_pt_count/README.md` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_count/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_pt_count/c_pt_count.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_count/c_pt_count.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_pt_count/c_pt_count.py` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_count/c_pt_count.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module for generating c_pt_count tables"""
 
 from typing import ClassVar
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
-from cumulus_library_data_metrics.data_metrics.base import MetricMixin
+from cumulus_library_data_metrics.base import MetricMixin
 
 
 class PatientCountBuilder(MetricMixin, BaseTableBuilder):
     name = "c_pt_count"
     uses_fields: ClassVar[dict] = {
         "Patient": {
             "extension": {
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_pt_deceased_count/c_pt_deceased_count.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_deceased_count/c_pt_deceased_count.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_pt_deceased_count/c_pt_deceased_count.py` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_pt_deceased_count/c_pt_deceased_count.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module for generating c_pt_deceased_count tables"""
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
-from cumulus_library_data_metrics.data_metrics.base import MetricMixin
+from cumulus_library_data_metrics.base import MetricMixin
 
 
 class DeceasedCountBuilder(MetricMixin, BaseTableBuilder):
     name = "c_pt_deceased_count"
 
     def add_metric_queries(self, *args, **kwargs) -> None:
         # https://github.com/sync-for-science/qualifier/blob/master/metrics.md#c_pt_deceased_count-demographics-count-of-deceased-patients-by-gender-by-age-at-death
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_resource_count/c_resource_count.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resource_count/c_resource_count.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_resource_count/c_resource_count.py` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resource_count/c_resource_count.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module for generating c_resource_count tables"""
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
-from cumulus_library_data_metrics.data_metrics import resource_info
-from cumulus_library_data_metrics.data_metrics.base import MetricMixin
+from cumulus_library_data_metrics import resource_info
+from cumulus_library_data_metrics.base import MetricMixin
 
 
 class ResourceCountBuilder(MetricMixin, BaseTableBuilder):
     name = "c_resource_count"
 
     def make_tables(self, src: str) -> None:
         """Make metric tables"""
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_resources_per_pt/c_resources_per_pt.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resources_per_pt/c_resources_per_pt.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_resources_per_pt/c_resources_per_pt.py` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_resources_per_pt/c_resources_per_pt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Module for generating c_resources_per_pt tables"""
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
-from cumulus_library_data_metrics.data_metrics import resource_info
-from cumulus_library_data_metrics.data_metrics.base import MetricMixin
+from cumulus_library_data_metrics import resource_info
+from cumulus_library_data_metrics.base import MetricMixin
 
 
 class ResourcesPerPatientBuilder(MetricMixin, BaseTableBuilder):
     name = "c_resources_per_pt"
 
     def add_metric_queries(self) -> None:
         # https://github.com/sync-for-science/qualifier/blob/master/metrics.md#c_resources_per_pt-volume-distribution-of-unique-resources-per-patient-by-resource-type-by-category
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_term_coverage/README.md` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_term_coverage/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_term_coverage/c_term_coverage.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_term_coverage/c_term_coverage.jinja`

 * *Files 16% similar despite different names*

```diff
@@ -28,29 +28,21 @@
     FROM {{ src }},
         UNNEST({{ field }}.coding) AS c (coding)
     {% endif %}
 ),
 src_systems_readable AS (
     SELECT
         id,
-        (
-            CASE
-            WHEN system = 'http://hl7.org/fhir/sid/cvx'
-            THEN 'CVX'
-            WHEN system = 'http://hl7.org/fhir/sid/ndc'
-            THEN 'NDC'
-            WHEN system = 'http://loinc.org'
-            THEN 'LOINC'
-            WHEN system = 'http://snomed.info/sct'
-            THEN 'SNOMED'
-            WHEN system = 'http://www.nlm.nih.gov/research/umls/rxnorm'
-            THEN 'RxNorm'
-            ELSE system
-            END
-        ) AS system
+        CASE
+        {% for url, name in system_names.items() %}
+        WHEN system = '{{ url }}'
+        THEN '{{ name }}'
+        {% endfor %}
+        ELSE system
+        END AS system
     FROM src_systems_flat
 ),
 src_systems AS (
     SELECT
         id,
         ARRAY_AGG(system) AS systems
     FROM src_systems_readable
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_term_coverage/c_term_coverage.py` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_term_coverage/c_term_coverage.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,47 +1,48 @@
 """Module for generating c_term_coverage tables"""
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
-from cumulus_library_data_metrics.data_metrics.base import MetricMixin
+from cumulus_library_data_metrics import systems
+from cumulus_library_data_metrics.base import MetricMixin
 
 # Note that this CUBE is already very large / slow.
 # Please do not add new columns to it.
 # We already had to drop one planned column (has_text) from it due to performance.
 
 
 class TermCoverageBuilder(MetricMixin, BaseTableBuilder):
     name = "c_term_coverage"
 
     def make_table(self, **kwargs) -> None:
         """Make a single metric table"""
-        self.queries.append(self.render_sql(self.name, **kwargs))
+        self.queries.append(self.render_sql(self.name, system_names=systems.NAMES, **kwargs))
 
     def add_metric_queries(self) -> None:
         # https://github.com/sync-for-science/qualifier/blob/master/metrics.md#c_term_coverage-terminology-count-of-resources-by-terminology-system-by-resource-type-by-category
         # With some tweaks:
         # - Also stratify by year
         # - Don't stratify by has_text -- CUBE was too big, had to drop something
         # - added Encounter.class
         # - added Medication.code
         self.make_table(
             src="Observation",
             field="code",
-            category_system="http://terminology.hl7.org/CodeSystem/observation-category",
+            category_system=systems.OBSERVATION_CATEGORY,
         )
         self.make_table(
             src="Observation",
             field="valueCodeableConcept",
-            category_system="http://terminology.hl7.org/CodeSystem/observation-category",
+            category_system=systems.OBSERVATION_CATEGORY,
         )
         self.make_table(src="AllergyIntolerance", field="code")
         self.make_table(
             src="Condition",
             field="code",
-            category_system="http://terminology.hl7.org/CodeSystem/condition-category",
+            category_system=systems.CONDITION_CATEGORY,
         )
         self.make_table(src="Device", field="type")
         self.make_table(src="DiagnosticReport", field="code")
         self.make_table(src="DocumentReference", field="type")
         self.make_table(src="Encounter", field="class", is_coding=True)
         self.make_table(src="Encounter", field="type", is_array=True)
         self.make_table(src="Immunization", field="vaccineCode")
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_us_core_v4_count/README.md` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_us_core_v4_count/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/c_us_core_v4_count/c_us_core_v4_count.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/c_us_core_v4_count/c_us_core_v4_count.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/manifest.toml` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/manifest.toml`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/meta/dates.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/meta/dates.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/meta/meta.py` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/meta/meta.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Sets study metadata"""
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
-from cumulus_library_data_metrics.data_metrics.base import MetricMixin
+from cumulus_library_data_metrics.base import MetricMixin
 
 
 class MetadataBuilder(MetricMixin, BaseTableBuilder):
     name = "meta"
 
     def add_date_query(self) -> None:
         # This is just a mapping of *START* dates - no mechanism for looking up end dates in
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_date_recent/README.md` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_date_recent/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_date_recent/q_date_recent.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_date_recent/q_date_recent.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_date_recent/q_date_recent.py` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_date_recent/q_date_recent.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Module for generating q_date_recent tables
 
 https://github.com/sync-for-science/qualifier/blob/master/metrics.md#q_date_recent-plausibility-expect-date-to-be-in-recent-past
 """
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
-from cumulus_library_data_metrics.data_metrics.base import MetricMixin
+from cumulus_library_data_metrics.base import MetricMixin
 
 
 class DateRecentBuilder(MetricMixin, BaseTableBuilder):
     name = "q_date_recent"
 
     def make_table(self, **kwargs) -> None:
         """Make a single metric table"""
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_ref_target_pop/README.md` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_pop/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_ref_target_pop/q_ref_target_pop.py` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_pop/q_ref_target_pop.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module for generating q_ref_target_pop tables"""
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
-from cumulus_library_data_metrics.data_metrics.base import MetricMixin
+from cumulus_library_data_metrics.base import MetricMixin
 
 
 class TargetPopBuilder(MetricMixin, BaseTableBuilder):
     name = "q_ref_target_pop"
 
     def make_table(self, **kwargs) -> str:
         """Make a single metric table"""
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_ref_target_valid/README.md` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_valid/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_ref_target_valid/q_ref_target_valid.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_valid/q_ref_target_valid.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_ref_target_valid/q_ref_target_valid.py` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_ref_target_valid/q_ref_target_valid.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Module for generating q_ref_target_valid tables"""
 
 from typing import ClassVar
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
-from cumulus_library_data_metrics.data_metrics.base import MetricMixin
+from cumulus_library_data_metrics.base import MetricMixin
 
 
 class TargetValidBuilder(MetricMixin, BaseTableBuilder):
     name = "q_ref_target_valid"
 
     uses_fields: ClassVar[dict] = {
         "DocumentReference": {
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_term_use/README.md` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_term_use/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_term_use/q_term_use.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_term_use/q_term_use.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_valid_us_core_v4/README.md` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/README.md`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.py` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/q_valid_us_core_v4/q_valid_us_core_v4.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module for generating q_valid_us_core_v4 tables"""
 
 from cumulus_library.base_table_builder import BaseTableBuilder
 
-from cumulus_library_data_metrics.data_metrics.us_core_v4 import UsCoreV4Mixin
+from cumulus_library_data_metrics.us_core_v4 import UsCoreV4Mixin
 
 
 class ValidUsCoreV4Builder(UsCoreV4Mixin, BaseTableBuilder):
     name = "q_valid_us_core_v4"
 
     def make_table(self, **kwargs) -> None:
         """Make a single metric table"""
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/resource_info.py` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/resource_info.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,54 +1,51 @@
 """Holds various static info about resources we want to examine."""
 
+from cumulus_library_data_metrics import systems
+
 # Categories to slice on
 CATEGORIES = {
     "AllergyIntolerance": {
         "cat_field": "category",
     },
     "Condition": {
         "cat_field": "category",
-        "cat_systems": ["http://terminology.hl7.org/CodeSystem/condition-category"],
+        "cat_systems": [systems.CONDITION_CATEGORY],
     },
     "DiagnosticReport": {
         "cat_field": "category",
-        "cat_systems": [
-            "http://loinc.org",
-            "http://terminology.hl7.org/CodeSystem/v2-0074",
-        ],
+        "cat_systems": [systems.LOINC, systems.DIAGNOSTIC_SECTION],
     },
     "DocumentReference": {
         "cat_field": "category",
-        "cat_systems": [
-            "http://hl7.org/fhir/us/core/CodeSystem/us-core-documentreference-category"
-        ],
+        "cat_systems": [systems.USCORE_DOCREF_CATEGORY],
     },
     "Encounter": {
         "cat_field": "type",
-        "cat_systems": ["http://www.ama-assn.org/go/cpt", "http://snomed.info/sct"],
+        "cat_systems": [systems.CPT, systems.SNOMED],
     },
     "MedicationRequest": {
         "cat_field": "category",
-        "cat_systems": ["http://terminology.hl7.org/CodeSystem/medicationrequest-category"],
+        "cat_systems": [systems.MEDREQ_CATEGORY],
     },
     "Observation": {
         "cat_field": "category",
-        "cat_systems": ["http://terminology.hl7.org/CodeSystem/observation-category"],
+        "cat_systems": [systems.OBSERVATION_CATEGORY],
     },
 }
 
 # Date fields in preference order.
 # This prefers "interaction with health system" dates, then administrative dates like "issued",
 # then best effort start dates like onsetDateTime.
 # See https://github.com/smart-on-fhir/cumulus-library-data-metrics/issues/16 for more.
 DATES = {
     "AllergyIntolerance": ["recordedDate", "onsetDateTime", "onsetPeriod.start"],
     "Condition": ["recordedDate", "onsetDateTime", "onsetPeriod.start"],
-    "DocumentReference": ["context.period.start", "date"],
     "DiagnosticReport": ["effectiveDateTime", "effectivePeriod.start", "issued"],
+    "DocumentReference": ["context.period.start", "date"],
     "Encounter": ["period.start"],
     "Immunization": ["occurrenceDateTime", "recorded"],
     "MedicationRequest": ["authoredOn"],
     "Observation": [
         "effectiveDateTime",
         "effectivePeriod.start",
         "effectiveInstant",
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/t_us_core_v4/t_us_core_v4.py` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/t_us_core_v4/t_us_core_v4.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 """Fake/test metric for us_core_v4 profiles"""
 
 import jinja2
 from cumulus_library.base_table_builder import BaseTableBuilder
 
-from cumulus_library_data_metrics.data_metrics.us_core_v4 import UsCoreV4Mixin
+from cumulus_library_data_metrics.us_core_v4 import UsCoreV4Mixin
 
 
 class TestUsCoreV4Builder(UsCoreV4Mixin, BaseTableBuilder):
     name = "t_us_core_v4"
 
     def make_table(self, **kwargs) -> None:
         """Make a table for both mandatory and must_support"""
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/allergyintolerance_mandatory.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/allergyintolerance_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/allergyintolerance_must_support.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/allergyintolerance_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/condition_mandatory.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/condition_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/condition_must_support.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/condition_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/diagnosticreport_note_mandatory.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_note_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/diagnosticreport_note_must_support.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/diagnosticreport_note_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/documentreference_mandatory.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/documentreference_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/documentreference_must_support.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/documentreference_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/encounter_mandatory.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/encounter_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/encounter_must_support.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/encounter_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/immunization_mandatory.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/immunization_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/immunization_must_support.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/immunization_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/medicationrequest_mandatory.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/medicationrequest_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/medicationrequest_must_support.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/medicationrequest_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/observation_laboratory_mandatory.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_laboratory_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/observation_laboratory_must_support.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_laboratory_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/observation_smoking_status_mandatory.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_smoking_status_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/observation_utils.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_utils.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/observation_vital_signs_mandatory.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_vital_signs_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/observation_vital_signs_must_support.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/observation_vital_signs_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/patient_mandatory.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/patient_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/patient_must_support.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/patient_must_support.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/patient_utils.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/patient_utils.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/procedure_mandatory.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/procedure_mandatory.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/us_core_v4/profiles.py` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/us_core_v4/profiles.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Module for generating tables based on US Core v4 profile features"""
 
 from typing import ClassVar
 
-from cumulus_library_data_metrics.data_metrics.base import MetricMixin
+from cumulus_library_data_metrics.base import MetricMixin
 
 
 class UsCoreV4Mixin(MetricMixin):
     # These methods largely deal with inspecting the schema before we fully query the table.
     # Complex column values deeper than the toplevel are not guaranteed to be present in the schema.
     # So we check if they are here.
```

### Comparing `cumulus_library_data_metrics-0.0.0/cumulus_library_data_metrics/data_metrics/utils.jinja` & `cumulus_library_data_metrics-1.0.0/cumulus_library_data_metrics/utils.jinja`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/pyproject.toml` & `cumulus_library_data_metrics-1.0.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 name = "cumulus-library-data-metrics"
 requires-python = ">= 3.10"
 dependencies = [
-    "cumulus-library >= 2.1, < 3",
+    "cumulus-library >= 2.2, < 3",
 ]
 description = "Data quality and characterization metrics for Cumulus"
 readme = "README.md"
 license = { text="Apache License 2.0" }
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
```

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_pt_count/cubed/expected.csv` & `cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/cubed/expected.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_pt_count/cubed/patient/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/cubed/patient/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_pt_count/general/expected.csv` & `cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/general/expected.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_pt_count/general/patient/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/c_pt_count/general/patient/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_pt_deceased_count/general/patient/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/c_pt_deceased_count/general/patient/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/allergyintolerance/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/allergyintolerance/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/condition/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/condition/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/documentreference/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/documentreference/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/encounter/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/encounter/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_resource_count/general/observation/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/c_resource_count/general/observation/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_resources_per_pt/general/expected_summary.csv` & `cumulus_library_data_metrics-1.0.0/tests/data/c_resources_per_pt/general/expected_summary.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_resources_per_pt/general/medicationrequest/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/c_resources_per_pt/general/medicationrequest/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/allergyintolerance/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/allergyintolerance/0.ndjson`

 * *Files 9% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 {"id": "snomed", "code": {"coding": [{"system": "http://snomed.info/sct"}]}}
 {"id": "snomed-with-text", "code": {"coding": [{"system": "http://snomed.info/sct"}], "text": "hello"}}
+{"id": "snomed-oid", "code": {"coding": [{"system": "urn:oid:2.16.840.1.113883.6.96"}]}}
 {"id": "multiple-systems", "code": {"coding": [{"code": "boo"}, {"system": "http://other"}, {"system": "http://loinc.org"}], "text": "\u0000"}}
 {"id": "repeated-systems", "code": {"coding": [{"system": "http://other"}, {"system": "http://other"}, {"system": "http://www.nlm.nih.gov/research/umls/rxnorm"}]}}
 {"id": "no-system", "code": {"coding": [{"code": "boo"}]}}
 {"id": "only-text", "code": {"text": "Not coded :("}}
 {"id": "empty-text", "code": {"coding": [{"display": "X"}], "text": ""}}
 {"id": "with-date", "recordedDate": "2018-03-02", "code": {"coding": [{"system": "other"}]}}
 {"id": "with-status", "verificationStatus": {"coding": [{"code": "confirmed", "system": "http://terminology.hl7.org/CodeSystem/allergyintolerance-verification"}]}, "code": {"coding": [{"system": "other"}]}}
```

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/condition/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/condition/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_term_coverage/general/observation/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/c_term_coverage/general/observation/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/c_us_core_v4_count/general/documentreference/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/c_us_core_v4_count/general/documentreference/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/documentreference/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/documentreference/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/expected_summary.csv` & `cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/expected_summary.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/q_ref_target_valid/general/procedure/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/q_ref_target_valid/general/procedure/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/allergyintolerance/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/allergyintolerance/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/condition/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/condition/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/diagnosticreport/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/diagnosticreport/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/documentreference/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/documentreference/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/encounter/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/encounter/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_allergyintolerance_mandatory.csv` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_allergyintolerance_mandatory.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_condition_mandatory.csv` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_condition_mandatory.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_diagnosticreport_note_mandatory.csv` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_diagnosticreport_note_mandatory.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_documentreference_mandatory.csv` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_documentreference_mandatory.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_laboratory_mandatory.csv` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_laboratory_mandatory.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_smoking_status_mandatory.csv` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_smoking_status_mandatory.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_vital_signs_mandatory.csv` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/expected_observation_vital_signs_mandatory.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/immunization/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/immunization/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/medicationrequest/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/medicationrequest/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/observation/labs.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/observation/labs.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/observation/smoking.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/observation/smoking.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/observation/vitals.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/observation/vitals.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/mandatory/procedure/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/mandatory/procedure/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/allergyintolerance/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/allergyintolerance/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/documentreference/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/documentreference/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/encounter/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/encounter/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/expected_patient_must_support.csv` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/expected_patient_must_support.csv`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/observation/labs.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/observation/labs.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/observation/vitals.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/observation/vitals.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/data/t_us_core_v4/must-support/patient/0.ndjson` & `cumulus_library_data_metrics-1.0.0/tests/data/t_us_core_v4/must-support/patient/0.ndjson`

 * *Files identical despite different names*

### Comparing `cumulus_library_data_metrics-0.0.0/tests/test_metrics.py` & `cumulus_library_data_metrics-1.0.0/tests/test_metrics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Base class support for unit tests"""
 
 import glob
 import os
 import shutil
+import sys
 import tempfile
 import unittest
 from unittest import mock
 
 import ddt
 import duckdb
 from cumulus_library import cli
@@ -109,16 +110,25 @@
         with tempfile.TemporaryDirectory() as tmpdir:
             # Copy all our study code to this tmpdir
             shutil.copytree(
                 f"{root_dir}/cumulus_library_data_metrics",
                 f"{tmpdir}/cumulus_library_data_metrics",
             )
 
+            # Because we reload the data-metrics study from different paths each time,
+            # python might be keeping the stale imports from previous test builders around.
+            # Manually drop em here.
+            stale_modules = [
+                mod for mod in sys.modules if mod.startswith("cumulus_library_data_metrics")
+            ]
+            for mod in stale_modules:
+                del sys.modules[mod]
+
             # But change the manifest to only run one test metric, for speed reasons
-            manifest_file = f"{tmpdir}/cumulus_library_data_metrics/data_metrics/manifest.toml"
+            manifest_file = f"{tmpdir}/cumulus_library_data_metrics/manifest.toml"
             with open(manifest_file, "w", encoding="utf8") as f:
                 f.write(
                     f"""
 study_prefix = "data_metrics"
 [table_builder_config]
 file_names = [
     "{metric}/{metric}.py",
```

### Comparing `cumulus_library_data_metrics-0.0.0/PKG-INFO` & `cumulus_library_data_metrics-1.0.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: cumulus-library-data-metrics
-Version: 0.0.0
+Version: 1.0.0
 Summary: Data quality and characterization metrics for Cumulus
 Requires-Python: >= 3.10
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
-Requires-Dist: cumulus-library >= 2.1, < 3
+Requires-Dist: cumulus-library >= 2.2, < 3
 Requires-Dist: pre-commit ; extra == "dev"
 Requires-Dist: ruff == 0.4.4 ; extra == "dev"
 Requires-Dist: ddt ; extra == "tests"
 Requires-Dist: pytest ; extra == "tests"
 Project-URL: Documentation, https://docs.smarthealthit.org/cumulus/
 Project-URL: Home, https://smarthealthit.org/cumulus/
 Project-URL: Source, https://github.com/smart-on-fhir/cumulus-library-data-metrics
@@ -20,14 +20,20 @@
 Provides-Extra: tests
 
 # Data Metrics
 
 See [qualifier repo](https://github.com/sync-for-science/qualifier/blob/master/metrics.md)
 for some metric definitions.
 
+## Installing
+
+```sh
+pip install cumulus-library-data-metrics
+```
+
 ## Running the Metrics
 
 These metrics are designed as a
 [Cumulus Library](https://docs.smarthealthit.org/cumulus/library/)
 study and are run using the `cumulus-library` command.
 
 ### Local Ndjson
@@ -42,34 +48,32 @@
   patient/
     Patient.ndjson
 ```
 (This is the same format that Cumulus ETL writes out when using `--output-format=ndjson`.)
 
 Here's a sample command to run against that pile of ndjson data:
 ```sh
-PYTHONPATH=. cumulus-library build \
+cumulus-library build \
   --db-type duckdb \
   --database output-tables.db \
   --load-ndjson-dir path/to/ndjson/root \
-  --target data_metrics \
-  --study-dir .
+  --target data_metrics
 ```
 
 And then you can load `output-tables.db` in a DuckDB session and see the results.
 Or read below to export the counts tables.
 
 ### Athena
 Here's a sample command to run against your Cumulus data in Athena:
 ```sh
-PYTHONPATH=. cumulus-library build \
+cumulus-library build \
   --database your-glue-database \
   --workgroup your-athena-workgroup \
   --profile your-aws-credentials-profile \
-  --target data_metrics \
-  --study-dir .
+  --target data_metrics
 ```
 
 And then you can see the resulting tables in Athena.
 Or read below to export the counts tables.
 
 ### Exporting Counts
 
@@ -79,30 +83,28 @@
 Like so:
 
 ```sh
 cumulus-library export \
   ./output-folder \
   --db-type duckdb \
   --database output-tables.db \
-  --target data_metrics \
-  --study-dir .
+  --target data_metrics
 ```
 
 #### Aggregate counts
 
 This study generates `CUBE` output by default.
 If it's easier to work with simple aggregate counts of every value combination
 (that is, without the partial value combinations that `CUBE()` generates),
 run the build step with `DATA_METRICS_OUTPUT_MODE=aggregate` in your environment.
 
 That is, run it like:
 ```sh
 env \
   DATA_METRICS_OUTPUT_MODE=aggregate \
-  PYTHONPATH=. \
   cumulus-library build ...
 ```
 
 ## SQL Writing Guidelines
 - Don't depend on `core__` tables.
   - Allows folks to build this study even if they can't or haven't built `core`
   - Allows `core` to smooth over data oddities we might be interested in
@@ -118,40 +120,21 @@
 - We drop MedicationAdministration from our metrics - it's not really supported in Cumulus
 - We add support for DiagnosticReport where sensible
 - We consider Observation.effectivePeriod.start and Observation.effectiveInstant in addition
   to Observation.effectiveDateTime
 
 Other specific deltas will be noted in the code for the given metric.
 
-## Metric Prioritization
+## Implemented Metrics
 
-### Table stakes quality:
-- `q_term_use` complies with US Core v1
-- `q_ref_target_pop` complies with US Core v1 (can be run on partial extracts)
-- `q_ref_target_valid` complies with US Core v1 (only on full extracts or data lake)
-- `q_valid_us_core_v4`
-  - numerator: resources that don't have all mandatory bits of any profile
-
-### Table stakes characterization:
-- `c_resource_count` (by category, year, month)
-- `c_pt_count` (by birth year gender, ethnicity, race)
-- `c_pt_deceased_count` (by gender, by age at death)
-- `c_term_coverage` (by resource type, by category)
-- `c_resources_per_pt` (include combinations?)
-- `c_us_core_v4_count`
-  - Tells how many rows match mandatory US Core support
-  - And for each separate must-support requirement, tells which rows have the value
-
-### High value quality:
-- `q_date_sequence`
-- `q_date_in_lifetime`
-- `q_date_recent`
-
-### High value characterization:
-- `c_element_use` for USCDI v1 “must support” elements
-- `c_date_precision` (by resource type, by category, by date element, by precision level)
-- `c_identifier_coverage` (by resource type)
-
-### Useful quality:
-- `q_obs_value_range`
-- `q_obs_comp_value_range`
+- c_pt_count
+- c_pt_deceased_count
+- c_resource_count
+- c_resources_per_pt
+- c_term_coverage
+- c_us_core_v4_count
+- q_date_recent
+- q_ref_target_pop
+- q_ref_target_valid
+- q_term_use
+- q_valid_us_core_v4
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

