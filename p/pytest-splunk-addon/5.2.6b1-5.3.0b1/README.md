# Comparing `tmp/pytest_splunk_addon-5.2.6b1.tar.gz` & `tmp/pytest_splunk_addon-5.3.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest_splunk_addon-5.2.6b1.tar", max compression
+gzip compressed data, was "pytest_splunk_addon-5.3.0b1.tar", max compression
```

## Comparing `pytest_splunk_addon-5.2.6b1.tar` & `pytest_splunk_addon-5.3.0b1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
--rw-r--r--   0        0        0    11341 2024-04-19 15:14:44.549955 pytest_splunk_addon-5.2.6b1/LICENSE
--rw-r--r--   0        0        0     2322 2024-04-19 15:15:27.394245 pytest_splunk_addon-5.2.6b1/pyproject.toml
--rw-r--r--   0        0        0     1886 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/.ignore_splunk_internal_errors
--rw-r--r--   0        0        0      751 2024-04-19 15:15:27.394245 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/__init__.py
--rw-r--r--   0        0        0     5364 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/docker_class.py
--rw-r--r--   0        0        0     8543 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/plugin.py
--rw-r--r--   0        0        0    34048 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/splunk.py
--rw-r--r--   0        0        0      579 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py
--rw-r--r--   0        0        0    46781 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py
--rw-r--r--   0        0        0     1220 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/__init__.py
--rw-r--r--   0        0        0     2791 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_basic.py
--rw-r--r--   0        0        0     3312 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/__init__.py
--rw-r--r--   0        0        0     2082 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py
--rw-r--r--   0        0        0     3136 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/fields.py
--rw-r--r--   0        0        0    13284 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py
--rw-r--r--   0        0        0     2760 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py
--rw-r--r--   0        0        0     2447 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py
--rw-r--r--   0        0        0     5391 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py
--rw-r--r--   0        0        0     6168 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/app_test_generator.py
--rw-r--r--   0        0        0      754 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py
--rw-r--r--   0        0        0     1251 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py
--rw-r--r--   0        0        0     1130 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py
--rw-r--r--   0        0        0     9586 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py
--rw-r--r--   0        0        0     2351 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py
--rw-r--r--   0        0        0     2801 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py
--rw-r--r--   0        0        0     2442 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py
--rw-r--r--   0        0        0     3553 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json
--rw-r--r--   0        0        0     3699 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json
--rw-r--r--   0        0        0      970 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/__init__.py
--rw-r--r--   0        0        0     2024 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py
--rw-r--r--   0        0        0     2386 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_model.py
--rw-r--r--   0        0        0     3937 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py
--rw-r--r--   0        0        0     3267 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_set.py
--rw-r--r--   0        0        0     4226 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py
--rw-r--r--   0        0        0     9218 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py
--rw-r--r--   0        0        0     2965 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py
--rw-r--r--   0        0        0    11204 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py
--rw-r--r--   0        0        0    20768 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py
--rw-r--r--   0        0        0     2390 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Alerts.json
--rw-r--r--   0        0        0     5281 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Authentication.json
--rw-r--r--   0        0        0     9626 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Certificates.json
--rw-r--r--   0        0        0     8173 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Change.json
--rw-r--r--   0        0        0     2814 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/DLP.json
--rw-r--r--   0        0        0     8598 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Email.json
--rw-r--r--   0        0        0    18855 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Endpoint.json
--rw-r--r--   0        0        0     9400 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json
--rw-r--r--   0        0        0     4255 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Malware.json
--rw-r--r--   0        0        0     6608 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json
--rw-r--r--   0        0        0     5599 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json
--rw-r--r--   0        0        0    17483 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json
--rw-r--r--   0        0        0     3862 2024-04-19 15:14:44.553955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Updates.json
--rw-r--r--   0        0        0     5184 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json
--rw-r--r--   0        0        0     7178 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Web.json
--rw-r--r--   0        0        0      889 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py
--rw-r--r--   0        0        0      862 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py
--rw-r--r--   0        0        0     7339 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py
--rw-r--r--   0        0        0     5002 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py
--rw-r--r--   0        0        0     4418 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py
--rw-r--r--   0        0        0     4995 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py
--rw-r--r--   0        0        0     3615 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py
--rw-r--r--   0        0        0     3015 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py
--rw-r--r--   0        0        0      812 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/__init__.py
--rw-r--r--   0        0        0     3305 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py
--rw-r--r--   0        0        0     5420 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py
--rw-r--r--   0        0        0    11040 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py
--rw-r--r--   0        0        0    10360 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py
--rw-r--r--   0        0        0    21984 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py
--rw-r--r--   0        0        0      766 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/__init__.py
--rw-r--r--   0        0        0      711 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/key_fields.py
--rw-r--r--   0        0        0    11987 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/test_generator.py
--rw-r--r--   0        0        0    11457 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/test_templates.py
--rw-r--r--   0        0        0      909 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/__init__.py
--rw-r--r--   0        0        0     7291 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py
--rw-r--r--   0        0        0    46400 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/rule.py
--rw-r--r--   0        0        0    15413 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py
--rw-r--r--   0        0        0     2290 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py
--rw-r--r--   0        0        0    16792 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py
--rw-r--r--   0        0        0     6032 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py
--rw-r--r--   0        0        0     9990 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd
--rw-r--r--   0        0        0     6217 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py
--rw-r--r--   0        0        0      834 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/__init__.py
--rw-r--r--   0        0        0     4634 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/junit_parser.py
--rw-r--r--   0        0        0     1627 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/log_helper.py
--rw-r--r--   0        0        0     3034 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py
--rw-r--r--   0        0        0     3414 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py
--rw-r--r--   0        0        0    17585 2024-04-19 15:14:44.557955 pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/tools/cim_field_report.py
--rw-r--r--   0        0        0     1410 1970-01-01 00:00:00.000000 pytest_splunk_addon-5.2.6b1/PKG-INFO
+-rw-r--r--   0        0        0    11341 2024-05-16 10:02:01.376977 pytest_splunk_addon-5.3.0b1/LICENSE
+-rw-r--r--   0        0        0     2160 2024-05-16 10:02:56.605110 pytest_splunk_addon-5.3.0b1/pyproject.toml
+-rw-r--r--   0        0        0     1886 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/.ignore_splunk_internal_errors
+-rw-r--r--   0        0        0      751 2024-05-16 10:02:56.601110 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/__init__.py
+-rw-r--r--   0        0        0     5364 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/docker_class.py
+-rw-r--r--   0        0        0     8543 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/plugin.py
+-rw-r--r--   0        0        0    34181 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/splunk.py
+-rw-r--r--   0        0        0      579 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py
+-rw-r--r--   0        0        0    46781 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py
+-rw-r--r--   0        0        0     1220 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/__init__.py
+-rw-r--r--   0        0        0     2791 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_basic.py
+-rw-r--r--   0        0        0     3312 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/__init__.py
+-rw-r--r--   0        0        0     2082 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py
+-rw-r--r--   0        0        0     3136 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/fields.py
+-rw-r--r--   0        0        0    13284 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py
+-rw-r--r--   0        0        0     2760 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py
+-rw-r--r--   0        0        0     2447 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py
+-rw-r--r--   0        0        0     5391 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py
+-rw-r--r--   0        0        0     6168 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/app_test_generator.py
+-rw-r--r--   0        0        0      754 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py
+-rw-r--r--   0        0        0     1251 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py
+-rw-r--r--   0        0        0     1130 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py
+-rw-r--r--   0        0        0     9586 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py
+-rw-r--r--   0        0        0     2351 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py
+-rw-r--r--   0        0        0     2801 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py
+-rw-r--r--   0        0        0     2442 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py
+-rw-r--r--   0        0        0     3553 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json
+-rw-r--r--   0        0        0     3699 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json
+-rw-r--r--   0        0        0      970 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/__init__.py
+-rw-r--r--   0        0        0     2024 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py
+-rw-r--r--   0        0        0     2386 2024-05-16 10:02:01.380977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_model.py
+-rw-r--r--   0        0        0     3937 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py
+-rw-r--r--   0        0        0     3267 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_set.py
+-rw-r--r--   0        0        0     4226 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py
+-rw-r--r--   0        0        0     9218 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py
+-rw-r--r--   0        0        0     2965 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py
+-rw-r--r--   0        0        0    11204 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py
+-rw-r--r--   0        0        0    20768 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py
+-rw-r--r--   0        0        0     2390 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Alerts.json
+-rw-r--r--   0        0        0     5281 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Authentication.json
+-rw-r--r--   0        0        0     9626 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Certificates.json
+-rw-r--r--   0        0        0     8173 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Change.json
+-rw-r--r--   0        0        0     2814 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/DLP.json
+-rw-r--r--   0        0        0     8598 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Email.json
+-rw-r--r--   0        0        0    18855 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Endpoint.json
+-rw-r--r--   0        0        0     9890 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json
+-rw-r--r--   0        0        0     4255 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Malware.json
+-rw-r--r--   0        0        0     8746 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json
+-rw-r--r--   0        0        0     5599 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json
+-rw-r--r--   0        0        0    18953 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json
+-rw-r--r--   0        0        0     3862 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Updates.json
+-rw-r--r--   0        0        0     5184 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json
+-rw-r--r--   0        0        0     7178 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Web.json
+-rw-r--r--   0        0        0      889 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py
+-rw-r--r--   0        0        0      862 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py
+-rw-r--r--   0        0        0     7339 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py
+-rw-r--r--   0        0        0     5002 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py
+-rw-r--r--   0        0        0     4418 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py
+-rw-r--r--   0        0        0     4995 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py
+-rw-r--r--   0        0        0     3615 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py
+-rw-r--r--   0        0        0     3015 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py
+-rw-r--r--   0        0        0      812 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/__init__.py
+-rw-r--r--   0        0        0     3305 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py
+-rw-r--r--   0        0        0     5420 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py
+-rw-r--r--   0        0        0    11040 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py
+-rw-r--r--   0        0        0    10360 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py
+-rw-r--r--   0        0        0    21984 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py
+-rw-r--r--   0        0        0      766 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/__init__.py
+-rw-r--r--   0        0        0      711 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/key_fields.py
+-rw-r--r--   0        0        0    11987 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/test_generator.py
+-rw-r--r--   0        0        0    11457 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/test_templates.py
+-rw-r--r--   0        0        0      909 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/__init__.py
+-rw-r--r--   0        0        0     7291 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py
+-rw-r--r--   0        0        0    46400 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/rule.py
+-rw-r--r--   0        0        0    15413 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py
+-rw-r--r--   0        0        0     2290 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py
+-rw-r--r--   0        0        0    16792 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py
+-rw-r--r--   0        0        0     6032 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py
+-rw-r--r--   0        0        0     9990 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd
+-rw-r--r--   0        0        0     6217 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py
+-rw-r--r--   0        0        0      834 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/__init__.py
+-rw-r--r--   0        0        0     4634 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/junit_parser.py
+-rw-r--r--   0        0        0     1627 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/log_helper.py
+-rw-r--r--   0        0        0     3034 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py
+-rw-r--r--   0        0        0     3414 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py
+-rw-r--r--   0        0        0    17585 2024-05-16 10:02:01.384977 pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/tools/cim_field_report.py
+-rw-r--r--   0        0        0     1427 1970-01-01 00:00:00.000000 pytest_splunk_addon-5.3.0b1/PKG-INFO
```

### Comparing `pytest_splunk_addon-5.2.6b1/LICENSE` & `pytest_splunk_addon-5.3.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pyproject.toml` & `pytest_splunk_addon-5.3.0b1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -12,15 +12,15 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 #
 
 [tool.poetry]
 name = "pytest-splunk-addon"
-version = "5.2.6-beta.1"
+version = "5.3.0-beta.1"
 description = "A Dynamic test tool for Splunk Apps and Add-ons"
 authors = ["Splunk <addonfactory@splunk.com>"]
 license = "APACHE-2.0"
 classifiers = [
         "Framework :: Pytest",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Testing",
@@ -32,41 +32,32 @@
 include = ["pytest_splunk_addon/**/*.json", "pytest_splunk_addon/**/*.txt"]
 
 [tool.poetry.dependencies]
 python = "^3.7"
 pytest = ">5.4.0,<8"
 splunk-sdk = ">=1.6"
 requests = "^2.31.0"
-jsonschema = ">=4,<5"
-pytest-xdist = ">=2.3.0"
+jsonschema = "^v4.17.3"
+pytest-xdist = "^3.5.0"
 filelock = "^3.0"
 pytest-ordering = "~0.6"
 junitparser = "^2.2.0"
 addonfactory-splunk-conf-parser-lib = "*"
 defusedxml = "^0.7.1"
-Faker = ">=13.12,<19.0.0"
+Faker = "^18.0.0"
 xmltodict = "^0.13.0"
-xmlschema = "^1.11.3"
+xmlschema = "^2.5.1"
 splunksplwrapper = "^1.1.1"
 urllib3 = "<2"
 
-
 [tool.poetry.group.dev.dependencies]
-pytest-cov = "^3.0.0"
+pytest-cov = "^4"
 requests-mock = "^1.8.0"
-freezegun = "^1.2.1"
-pytz = "^2022.1"
-
-[tool.poetry.group.docs]
-optional = true
-
-[tool.poetry.group.docs.dependencies]
-jinja2 = "3.1.3"
-sphinx-rtd-theme = "1.1.1"
-sphinx-panels = "0.6.0"
+freezegun = "^1.5.1"
+pytz = "^2024.1"
 
 [tool.poetry.plugins]
 pytest11 = { plugin = "pytest_splunk_addon.plugin", "splunk" = "pytest_splunk_addon.splunk" }
 
 [tool.poetry.scripts]
 cim-report = 'pytest_splunk_addon.standard_lib.utilities.junit_parser:main'
 cim-field-report = 'pytest_splunk_addon.tools.cim_field_report:main'
```

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/.ignore_splunk_internal_errors` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/.ignore_splunk_internal_errors`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/__init__.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,8 +14,8 @@
 # limitations under the License.
 #
 # -*- coding: utf-8 -*-
 """Top-level package for splunk-app-test-lib."""
 
 __author__ = """Splunk Inc."""
 __email__ = "addonfactory@splunk.com"
-__version__ = "5.2.6-beta.1"
+__version__ = "5.3.0-beta.1"
```

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/docker_class.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/docker_class.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/plugin.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/splunk.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/splunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -1015,7 +1015,9 @@
 
 def pytest_unconfigure(config):
     if PYTEST_XDIST_TESTRUNUID:
         if os.path.exists(PYTEST_XDIST_TESTRUNUID + "_wait"):
             os.remove(PYTEST_XDIST_TESTRUNUID + "_wait")
         if os.path.exists(PYTEST_XDIST_TESTRUNUID + "_events"):
             os.remove(PYTEST_XDIST_TESTRUNUID + "_events")
+        if os.path.exists(PYTEST_XDIST_TESTRUNUID + "_events.lock"):
+            os.remove(PYTEST_XDIST_TESTRUNUID + "_events.lock")
```

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/CIM_Models/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/CIM_Models/datamodel_definition.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/__init__.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_basic.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_basic.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/__init__.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/eventtype_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/fields.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/fields.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/props_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/savedsearches_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/tags_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/addon_parser/transforms_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/app_test_generator.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/app_test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/base_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/base_table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/cim_report_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/markdown_table.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_compliance/plugin.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/CommonFields.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/DatamodelSchema.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/__init__.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/base_schema.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_model.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_model.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_model_handler.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/data_set.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/data_set.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_adapter.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/field_test_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/json_schema.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/cim_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Alerts.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Alerts.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Authentication.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Authentication.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Certificates.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Certificates.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Change.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Change.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/DLP.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/DLP.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Email.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Email.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Endpoint.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Endpoint.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Intrusion_Detection.json`

 * *Files 6% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998263888888889%*

 * *Differences: {"'objects'": '{0: {\'fields\': {2: {\'validity\': \'case(in(upper(transport), "HOPOPT", "ICMP", '*

 * *              '"IGMP", "GGP", "IP-IN-IP", "ST", "TCP", "CBT", "EGP", "IGP", "BBN-RCC-MON", '*

 * *              '"NVP-II", "PUP", "ARGUS", "EMCON", "XNET", "CHAOS", "UDP", "MUX", "DCN-MEAS", '*

 * *              '"HMP", "PRM", "XNS-ID", "TRUNK-1", "TRUNK-2", "LEAF-1", "LEAF-2", "RDP", "IRTP", '*

 * *              '"ISO-TP4", "NETBLT", "MFE-NSP", "MERIT-INP", "DCCP", "3CP", "IDPR", "XTP", "DDP", '*

 * *              '"IDPR-CMTP",  […]*

```diff
@@ -59,15 +59,15 @@
                     "type": "required"
                 },
                 {
                     "comment": "The destination of the attack detected by the intrusion detection system (IDS). You can alias this from more specific fields not included in this data model, such as dest_host, dest_ip, or dest_name.",
                     "condition": "ids_type=\"network\"",
                     "name": "dest",
                     "type": "conditional",
-                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(dest,\"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"), dest, null()), match(dest,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), dest, true(), null())"
+                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(dest,\"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"), dest, null()), match(dest,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), dest, true(), null())"
                 },
                 {
                     "comment": "The device that detected the intrusion event. You can alias this from more specific fields not included in this data model, such as dvc_host, dvc_ip, or dvc_name.",
                     "name": "dvc",
                     "type": "required"
                 },
                 {
@@ -115,15 +115,15 @@
                     "type": "required"
                 },
                 {
                     "comment": "The source involved in the attack detected by the IDS. You can alias this from more specific fields not included in this data model, such as src_host, src_ip, or src_name.",
                     "condition": "ids_type=\"network\"",
                     "name": "src",
                     "type": "conditional",
-                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(src,\"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"), src, null()), match(src,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), src, true(), null())"
+                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(src,\"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"), src, null()), match(src,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), src, true(), null())"
                 },
                 {
                     "comment": "The OSI layer 4 (transport) protocol of the intrusion, in lower case.",
                     "condition": "ids_type=\"network\"",
                     "name": "transport",
                     "type": "conditional"
                 },
```

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Malware.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Malware.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Resolution.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Sessions.json`

 * *Files 18% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.7714699074074073%*

 * *Differences: {"'model_name'": "'Network_Sessions'",*

 * * "'objects'": "{0: {'name': 'All_Sessions', 'tags': {0: {insert: [(1, 'session')], delete: [2, "*

 * *              "1]}}, 'fields': {0: {'name': 'action', 'expected_values': ['added', 'blocked'], "*

 * *              "'comment': 'The action taken by the reporting device.'}, 1: {'name': 'dest_ip', "*

 * *              "'comment': 'The internal IP address allocated to the client initializing a network "*

 * *              "session. For DHCP and VPN events, this is the IP address leased to  […]*

```diff
@@ -1,197 +1,168 @@
 {
-    "model_name": "Network_Resolution",
+    "model_name": "Network_Sessions",
     "objects": [
         {
-            "child_dataset": [],
-            "fields": [
-                {
-                    "comment": "Number of entries in the 'additional' section of the DNS message.",
-                    "name": "additional_answer_count",
-                    "type": "required",
-                    "validity": "if(isnum(additional_answer_count),additional_answer_count,null())"
-                },
-                {
-                    "comment": "Resolved address for the query.",
-                    "multi_value": true,
-                    "name": "answer",
-                    "type": "required"
-                },
+            "child_dataset": [
                 {
-                    "comment": "Number of entries in the answer section of the DNS message.",
-                    "name": "answer_count",
-                    "type": "required",
-                    "validity": "if(isnum(answer_count) and answer_count == mvcount(answer),answer_count,null())"
-                },
-                {
-                    "comment": "Number of entries in the 'authority' section of the DNS message.",
-                    "name": "authority_answer_count",
-                    "type": "required",
-                    "validity": "if(isnum(authority_answer_count),authority_answer_count,null())"
-                },
-                {
-                    "comment": "The destination of the network resolution event. You can alias this from more specific fields, such as dest_host, dest_ip, or dest_name.",
-                    "name": "dest",
-                    "type": "required",
-                    "validity": "case(in(upper(transport), \"TCP\", \"UDP\"), if(match(dest,\"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"), dest, null()), match(dest,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), dest, true(), null())"
-                },
+                    "child_dataset": [],
+                    "fields": [],
+                    "fields_cluster": [],
+                    "name": "Session_Start",
+                    "search_constraints": "tag=start",
+                    "tags": [
+                        [
+                            "network",
+                            "session",
+                            "start"
+                        ]
+                    ]
+                },
+                {
+                    "child_dataset": [],
+                    "fields": [],
+                    "fields_cluster": [],
+                    "name": "Session_End",
+                    "search_constraints": "tag=end",
+                    "tags": [
+                        [
+                            "network",
+                            "session",
+                            "end"
+                        ]
+                    ]
+                },
+                {
+                    "child_dataset": [],
+                    "fields": [
+                        {
+                            "comment": "The duration of the Dynamic Host Configuration Protocol (DHCP) lease, in seconds.",
+                            "condition": "lease_duration=*",
+                            "name": "lease_duration",
+                            "type": "conditional",
+                            "validity": "if(isnum(lease_duration),lease_duration,null())"
+                        },
+                        {
+                            "comment": "The consecutive range of possible IP addresses that the Dynamic Host Configuration Protocol (DHCP) server can lease to clients on a subnet. A lease_scope typically defines a single physical subnet on your network to which DHCP services are offered.",
+                            "name": "lease_scope",
+                            "type": "required"
+                        },
+                        {
+                            "comment": "The IP address of the client initializing a network session. Not applicable for DHCP events.",
+                            "name": "src_ip",
+                            "type": "not_allowed_in_search"
+                        },
+                        {
+                            "comment": "The MAC address of the client initializing a network session. Not applicable for DHCP events.Note: Always force lower case on this field.Note: Always use colons instead of dashes, spaces, or no separator.",
+                            "name": "src_mac",
+                            "type": "not_allowed_in_search"
+                        }
+                    ],
+                    "fields_cluster": [],
+                    "name": "DHCP",
+                    "search_constraints": "tag=dhcp",
+                    "tags": [
+                        [
+                            "network",
+                            "session",
+                            "dhcp"
+                        ]
+                    ]
+                },
+                {
+                    "child_dataset": [],
+                    "fields": [],
+                    "fields_cluster": [],
+                    "name": "VPN",
+                    "search_constraints": "tag=vpn",
+                    "tags": [
+                        [
+                            "network",
+                            "session",
+                            "vpn"
+                        ]
+                    ]
+                }
+            ],
+            "fields": [
                 {
-                    "comment": "Type of DNS message.",
+                    "comment": "The action taken by the reporting device.",
                     "expected_values": [
-                        "Query",
-                        "Response"
+                        "added",
+                        "blocked"
                     ],
-                    "name": "message_type",
+                    "name": "action",
                     "type": "required"
                 },
                 {
-                    "comment": "The domain which needs to be resolved. Applies to messages of type 'Query'.",
-                    "multi_value": true,
-                    "name": "query",
+                    "comment": "The internal IP address allocated to the client initializing a network session. For DHCP and VPN events, this is the IP address leased to the client.",
+                    "name": "dest_ip",
                     "type": "required"
                 },
                 {
-                    "comment": "Number of entries that appear in the 'Questions' section of the DNS query.",
-                    "name": "query_count",
-                    "type": "required",
-                    "validity": "if(isnum(query_count) and query_count == mvcount(query),query_count,null())"
-                },
-                {
-                    "comment": "The field may contain DNS OpCodes or Resource Record Type codes. For details, see the Domain Name System Parameters on the Internet Assigned Numbers Authority (IANA) web site. If a value is not set, the DNS.record_type field is referenced.",
-                    "expected_values": [
-                        "Query",
-                        "IQuery",
-                        "Status",
-                        "Notify",
-                        "Update",
-                        "A",
-                        "MX",
-                        "NS",
-                        "PTR"
-                    ],
-                    "name": "query_type",
+                    "comment": "The internal MAC address of the network session client. For DHCP events, this is the MAC address of the client acquiring an IP address lease. For VPN events, this is the MAC address of the client initializing a network session.Note: Always force lower case on this field.Note: Always use colons instead of dashes, spaces, or no separator.",
+                    "name": "dest_mac",
                     "type": "required"
                 },
                 {
-                    "comment": "The DNS resource record type. For details, see the List of DNS record types on Wikipedia.",
-                    "expected_values": [
-                        "A",
-                        "DNAME",
-                        "MX",
-                        "NS",
-                        "PTR"
-                    ],
-                    "name": "record_type",
+                    "comment": "An indication of the type of network session event.",
+                    "name": "signature",
                     "type": "required"
                 },
                 {
-                    "comment": "The return code for the response. For details, see the Domain Name System Parameters on the Internet Assigned Numbers Authority (IANA) web site.",
-                    "expected_values": [
-                        "No Error",
-                        "Format Error",
-                        "Server Failure",
-                        "Non-Existent Domain",
-                        "NotImp",
-                        "Refused",
-                        "YXDomain",
-                        "YXRRSet",
-                        "NotAuth",
-                        "NotZone",
-                        "BADVERS",
-                        "BADSIG",
-                        "BADKEY",
-                        "BADTIME",
-                        "BADMODE",
-                        "BADNAME",
-                        "BADALG"
-                    ],
-                    "name": "reply_code",
-                    "type": "required"
+                    "comment": "The priority of the destination.",
+                    "name": "dest_priority",
+                    "type": "optional"
                 },
                 {
-                    "comment": "The numerical id or name of a return code. For details, see the Domain Name System Parameters on the Internet Assigned Numbers Authority (IANA) web site.",
-                    "expected_values": [
-                        "No Error",
-                        "Format Error",
-                        "Server Failure",
-                        "Non-Existent Domain",
-                        "NotImp",
-                        "Refused",
-                        "YXDomain",
-                        "YXRRSet",
-                        "NotAuth",
-                        "NotZone",
-                        "BADVERS",
-                        "BADSIG",
-                        "BADKEY",
-                        "BADTIME",
-                        "BADMODE",
-                        "BADNAME",
-                        "BADALG",
-                        "0",
-                        "1",
-                        "2",
-                        "3"
-                    ],
-                    "name": "reply_code_id",
-                    "type": "required"
+                    "comment": "The amount of time for the completion of the network session event, in seconds.",
+                    "name": "duration",
+                    "type": "optional",
+                    "validity": "if(isnum(duration),duration,null())"
                 },
                 {
-                    "comment": "The amount of time it took to receive a response in the network resolution event, in seconds.",
+                    "comment": "The amount of time it took to receive a response in the network session event, in seconds.",
                     "name": "response_time",
-                    "type": "required",
+                    "type": "optional",
                     "validity": "if(isnum(response_time),response_time,null())"
                 },
                 {
-                    "comment": "The source of the network resolution event. You can alias this from more specific fields, such as src_host, src_ip, or src_name.",
-                    "name": "src",
-                    "type": "required",
-                    "validity": "case(in(upper(transport), \"TCP\", \"UDP\"), if(match(src,\"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"), src, null()), match(src,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), src, true(), null())"
-                },
-                {
-                    "comment": "The unique numerical transaction id of the network resolution event",
-                    "name": "transaction_id",
-                    "type": "required",
-                    "validity": "if(isnum(transaction_id),transaction_id,null())"
-                },
-                {
-                    "comment": "The transport protocol used by the network resolution event.",
-                    "name": "transport",
-                    "type": "required"
+                    "comment": "The external domain name of the client initializing a network session. Not applicable for DHCP events.",
+                    "name": "src_dns",
+                    "type": "optional"
                 },
                 {
-                    "comment": "The time taken by the network resolution event, in seconds.",
-                    "name": "duration",
-                    "type": "optional",
-                    "validity": "if(isnum(duration),duration,null())"
+                    "comment": "The MAC address of the client initializing a network session. Not applicable for DHCP events.Note: Always force lower case on this field.Note: Always use colons instead of dashes, spaces, or no separator.",
+                    "condition": "tag != dhcp",
+                    "name": "src_mac",
+                    "type": "optional"
                 },
                 {
-                    "comment": "The name of the DNS event.",
-                    "name": "name",
+                    "comment": "The full name of the Dynamic Host Configuration Protocol (DHCP) or DNS server involved in this event including vendor and product name, such as Microsoft DHCP or ISC BIND. This field is generated by combining the values of the vendor and product fields.",
+                    "name": "vendor_product",
                     "type": "optional"
                 },
                 {
-                    "comment": "The time-to-live of the network resolution event, in seconds.",
-                    "name": "ttl",
-                    "type": "optional",
-                    "validity": "if(isnum(ttl),ttl,null())"
+                    "comment": "The IP address of the client initializing a network session. Not applicable for DHCP events.",
+                    "condition": "tag != dhcp",
+                    "name": "src_ip",
+                    "type": "conditional"
                 },
                 {
-                    "comment": "The vendor product name of the DNS server. The Splunk platform can derive this field from the fields vendor and product in the raw data, if they exist.",
-                    "name": "vendor_product",
-                    "type": "optional"
+                    "comment": "The user in a network session event, where applicable. For example, a VPN session or an authenticated DHCP event.",
+                    "name": "user",
+                    "type": "required"
                 }
             ],
             "fields_cluster": [],
-            "name": "DNS",
-            "search_constraints": "tag=network tag=resolution tag=dns",
+            "name": "All_Sessions",
+            "search_constraints": "tag=network tag=session",
             "tags": [
                 [
                     "network",
-                    "resolution",
-                    "dns"
+                    "session"
                 ]
             ]
         }
     ],
     "version": "1.0.0"
 }
```

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Network_Traffic.json`

 * *Files 12% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9998374704491727%*

 * *Differences: {"'objects'": '{0: {\'fields\': {6: {\'validity\': \'case(in(upper(transport), "HOPOPT", "ICMP", '*

 * *              '"IGMP", "GGP", "IP-IN-IP", "ST", "TCP", "CBT", "EGP", "IGP", "BBN-RCC-MON", '*

 * *              '"NVP-II", "PUP", "ARGUS", "EMCON", "XNET", "CHAOS", "UDP", "MUX", "DCN-MEAS", '*

 * *              '"HMP", "PRM", "XNS-ID", "TRUNK-1", "TRUNK-2", "LEAF-1", "LEAF-2", "RDP", "IRTP", '*

 * *              '"ISO-TP4", "NETBLT", "MFE-NSP", "MERIT-INP", "DCCP", "3CP", "IDPR", "XTP", "DDP", '*

 * *              '"IDPR-CMTP",  […]*

```diff
@@ -86,27 +86,27 @@
                     "name": "channel",
                     "type": "not_allowed_in_search"
                 },
                 {
                     "comment": "The destination of the network traffic (the remote host). You can alias this from more specific fields, such as dest_host, dest_ip, or dest_name.",
                     "name": "dest",
                     "type": "required",
-                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(dest,\"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"), dest, null()), match(dest,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), dest, true(), null())"
+                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(dest,\"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"), dest, null()), match(dest,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), dest, true(), null())"
                 },
                 {
                     "comment": "The interface that is listening remotely or receiving packets locally. Can also be referred to as the 'egress interface.'",
                     "name": "dest_interface",
                     "type": "optional"
                 },
                 {
                     "comment": "The IP address of the destination.",
                     "condition": "dest_ip=*",
                     "name": "dest_ip",
                     "type": "conditional",
-                    "validity": "if(match(dest_ip, \"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"),dest_ip,null())"
+                    "validity": "if(match(dest_ip, \"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"),dest_ip,null())"
                 },
                 {
                     "comment": "The destination TCP/IP layer 2 Media Access Control (MAC) address of a packet's destination, such as 06:10:9f:eb:8f:14. Note: Always force lower case on this field and use colons instead of dashes, spaces, or no separator.",
                     "condition": "dest_mac=*",
                     "name": "dest_mac",
                     "type": "conditional",
                     "validity": "if(match(dest_mac,\"^([0-9A-F]{2}[:-]){5}([0-9A-F]{2})$\"),dest_mac,null())"
@@ -202,15 +202,15 @@
                     "comment": "The total count of packets transmitted by this device/interface.",
                     "name": "packets_out",
                     "type": "optional",
                     "validity": "if(isnum(packets_out),packets_out,null())"
                 },
                 {
                     "comment": "The OSI layer 3 (network) protocol of the traffic observed, in lower case. For example, ip, appletalk, ipx.",
-                    "condition": "| where match(src, \"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\") or match(dest, \"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\")",
+                    "condition": "| where match(src, \"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\") or match(dest, \"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\")",
                     "expected_values": [
                         "ip",
                         "icmp"
                     ],
                     "name": "protocol",
                     "type": "conditional"
                 },
@@ -240,15 +240,15 @@
                     "name": "session_id",
                     "type": "optional"
                 },
                 {
                     "comment": "The source of the network traffic (the client requesting the connection). You can alias this from more specific fields, such as src_host, src_ip, or src_name.'",
                     "name": "src",
                     "type": "required",
-                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(src,\"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"), src, null()), match(src,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), src, true(), null())"
+                    "validity": "case(in(upper(transport), \"HOPOPT\", \"ICMP\", \"IGMP\", \"GGP\", \"IP-IN-IP\", \"ST\", \"TCP\", \"CBT\", \"EGP\", \"IGP\", \"BBN-RCC-MON\", \"NVP-II\", \"PUP\", \"ARGUS\", \"EMCON\", \"XNET\", \"CHAOS\", \"UDP\", \"MUX\", \"DCN-MEAS\", \"HMP\", \"PRM\", \"XNS-ID\", \"TRUNK-1\", \"TRUNK-2\", \"LEAF-1\", \"LEAF-2\", \"RDP\", \"IRTP\", \"ISO-TP4\", \"NETBLT\", \"MFE-NSP\", \"MERIT-INP\", \"DCCP\", \"3CP\", \"IDPR\", \"XTP\", \"DDP\", \"IDPR-CMTP\", \"TP++\", \"IL\", \"IPV6\", \"SDRP\", \"IPV6-ROUTE\", \"IPV6-FRAG\", \"IDRP\", \"RSVP\", \"GRES\", \"DSR\", \"BNA\", \"ESP\", \"AH\", \"I-NLSP\", \"SWIPE\", \"NARP\", \"MOBILE\", \"TLSP\", \"SKIP\", \"IPV6-ICMP\", \"IPC6-NONXT\", \"IPV6-OPTS\", \"CFTP\", \"SAT-EXPAK\", \"KRYPTOLAN\", \"RVD\", \"IPPC\", \"SAT-MON\", \"VISA\", \"IPCU\", \"CPNX\", \"CPHB\", \"WSN\", \"PVP\", \"BR-SAT-MON\", \"SUN-ND\", \"WB-MON\", \"WB-EXPAK\", \"ISO-IP\", \"VMTP\", \"SECURE-VMTP\", \"VINES\", \"TTP\", \"IPTM\", \"NSFNET-IGP\", \"DGP\", \"TCF\", \"EIGRP\", \"OSPF\", \"SPRITE-RPC\", \"LARP\", \"MTP\", \"AX.25\", \"OS\", \"MICP\", \"SCC-SP\", \"ETHERIP\", \"ENCAP\", \"GMTP\", \"IFMP\", \"PNNI\", \"PIM\", \"ARIS\", \"SCPS\", \"QNX\", \"A/N\", \"IPCOMP\", \"SNP\", \"COMPAQ-PEER\", \"IPX-IN-IP\", \"VRRP\", \"PGM\", \"L2TP\", \"DDX\", \"IATP\", \"STP\", \"SRP\", \"UTI\", \"SMP\", \"SM\", \"PTP\", \"IS-IS OVER IPV4\", \"FIRE\", \"CRTP\", \"CRUDP\", \"SSCOPMCE\", \"IPLT\", \"SPS\", \"PIPE\", \"SCTP\", \"FC\", \"RSVP-E2E-IGNORE\", \"MOBILITY HEADER\", \"UDPLITE\", \"MPLS-IN-IP\", \"MANET\", \"HIP\", \"SHIM6\", \"WESP\", \"ROHC\", \"ETHERNET\"), if(match(src,\"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"), src, null()), match(src,\"^([0-9A-Fa-f]{2}[:-]){5}([0-9A-Fa-f]{2})$\"), src, true(), null())"
                 },
                 {
                     "comment": "The interface that is listening locally or sending packets remotely. Can also be referred to as the 'ingress interface.'",
                     "name": "src_interface",
                     "type": "optional"
                 },
                 {
@@ -323,15 +323,15 @@
                     "type": "required"
                 },
                 {
                     "comment": "The ip address of the source.",
                     "condition": "src_ip=*",
                     "name": "src_ip",
                     "type": "conditional",
-                    "validity": "if(match(src_ip, \"(?:[0-9A-Fa-f]{1,4}:){7}[0-9A-Fa-f]{1,4}|(?:(?:25[0-5]|2[0-4][0-9]|[01]?[0-9][0-9]?)(?:\\.|$)){4}\"),src_ip,null())"
+                    "validity": "if(match(src_ip, \"(?:(?:::ffff:)|(?:[0-9a-fA-F]{1,4}:){6}ffff:)\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}\\.\\d{1,3}|(?>([a-f0-9]{1,4})(?>:(?1)){7}|(?!(?:.[a-f0-9](?>:|$)){8,})^((?1)(?>:(?1)){0,6})?::(?2)?(?!(?:.*[a-f0-9](?>:|$))))|(?>(?>(?1)(?>:(?1)){5}:|(?!(?:.*[a-f0-9]:){6,})(?3)?::(?>((?1)(?>:(?1)){0,4}):)?)?(25[0-5]|2[0-4][0-9]|1[0-9]{2}|[1-9]?[0-9])(?>\\.(?4)){3})\"),src_ip,null())"
                 },
                 {
                     "comment": "The source TCP/IP layer 2 Media Access Control (MAC) address of a packet's destination, such as 06:10:9f:eb:8f:14. Note: Always force lower case on this field and use colons instead of dashes, spaces, or no separator.",
                     "condition": "src_mac=*",
                     "name": "src_mac",
                     "type": "conditional",
                     "validity": "if(match(src_mac,\"^([0-9A-F]{2}[:-]){5}([0-9A-F]{2})$\"),src_mac,null())"
```

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Updates.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Updates.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Vulnerabilities.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/data_models/Web.json` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/data_models/Web.json`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/base_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/file_monitor_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_metric_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/hec_raw_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/ingestor_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/event_ingestors/sc4s_event_ingestor.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/__init__.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/field_bank.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/requirement_test_datamodel_tag_constants.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/sample_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/fields_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/__init__.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/key_fields.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/key_fields.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/test_generator.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/test_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/index_tests/test_templates.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/index_tests/test_templates.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/__init__.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/pytest_splunk_addon_data_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/rule.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/rule.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_event.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_stanza.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/sample_xdist_generator.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/schema.xsd`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/sample_generation/time_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/__init__.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/__init__.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/junit_parser.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/junit_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/log_helper.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/log_helper.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/sample_splitter.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/standard_lib/utilities/xml_event_parser.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/pytest_splunk_addon/tools/cim_field_report.py` & `pytest_splunk_addon-5.3.0b1/pytest_splunk_addon/tools/cim_field_report.py`

 * *Files identical despite different names*

### Comparing `pytest_splunk_addon-5.2.6b1/PKG-INFO` & `pytest_splunk_addon-5.3.0b1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-splunk-addon
-Version: 5.2.6b1
+Version: 5.3.0b1
 Summary: A Dynamic test tool for Splunk Apps and Add-ons
 License: Apache-2.0
 Author: Splunk
 Author-email: addonfactory@splunk.com
 Requires-Python: >=3.7,<4.0
 Classifier: Framework :: Pytest
 Classifier: Intended Audience :: Developers
@@ -14,22 +14,22 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Testing
-Requires-Dist: Faker (>=13.12,<19.0.0)
+Requires-Dist: Faker (>=18.0.0,<19.0.0)
 Requires-Dist: addonfactory-splunk-conf-parser-lib
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: filelock (>=3.0,<4.0)
-Requires-Dist: jsonschema (>=4,<5)
+Requires-Dist: jsonschema (>=v4.17.3,<5.0.0)
 Requires-Dist: junitparser (>=2.2.0,<3.0.0)
 Requires-Dist: pytest (>5.4.0,<8)
 Requires-Dist: pytest-ordering (>=0.6,<0.7)
-Requires-Dist: pytest-xdist (>=2.3.0)
+Requires-Dist: pytest-xdist (>=3.5.0,<4.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: splunk-sdk (>=1.6)
 Requires-Dist: splunksplwrapper (>=1.1.1,<2.0.0)
 Requires-Dist: urllib3 (<2)
-Requires-Dist: xmlschema (>=1.11.3,<2.0.0)
+Requires-Dist: xmlschema (>=2.5.1,<3.0.0)
 Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
```

