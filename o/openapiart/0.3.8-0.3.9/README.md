# Comparing `tmp/openapiart-0.3.8.tar.gz` & `tmp/openapiart-0.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openapiart-0.3.8.tar", last modified: Mon Jan  8 10:35:48 2024, max compression
+gzip compressed data, was "openapiart-0.3.9.tar", last modified: Tue Jan 16 10:42:24 2024, max compression
```

## Comparing `openapiart-0.3.8.tar` & `openapiart-0.3.9.tar`

### file list

```diff
@@ -1,119 +1,120 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.975118 openapiart-0.3.8/
--rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-01-08 10:35:00.000000 openapiart-0.3.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-08 10:35:00.000000 openapiart-0.3.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-01-08 10:35:48.975118 openapiart-0.3.8/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.959118 openapiart-0.3.8/openapiart/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    52578 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)    11786 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/common.go
--rw-r--r--   0 runner    (1001) docker     (127)    39920 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/common_test.go
--rw-r--r--   0 runner    (1001) docker     (127)    81902 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.959118 openapiart-0.3.8/openapiart/goserver/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.963118 openapiart-0.3.8/openapiart/goserver/api/
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/api/api.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/api/common.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/api/service_a.api.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/api/service_a.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/api/service_b.api.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      614 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/api/service_b.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/generator_context.py
--rw-r--r--   0 runner    (1001) docker     (127)    16226 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/go_controller_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/go_interface_generator.py
--rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/goserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/http_setup.go
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/response.go
--rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/string_util.py
--rw-r--r--   0 runner    (1001) docker     (127)      568 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/goserver/writer.py
--rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/gotidy.py
--rw-r--r--   0 runner    (1001) docker     (127)    13444 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/openapiart.py
--rw-r--r--   0 runner    (1001) docker     (127)   130817 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/openapiartgo.py
--rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/openapiartplugin.py
--rw-r--r--   0 runner    (1001) docker     (127)    18724 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/openapiartprotobuf.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/openapiartpython.py
--rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/requirements.py
--rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/test_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.967118 openapiart-0.3.8/openapiart/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.967118 openapiart-0.3.8/openapiart/tests/api/
--rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/api/api.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/api/info.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.967118 openapiart-0.3.8/openapiart/tests/check_type/
--rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/check_type/invalid_integer_type.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.967118 openapiart-0.3.8/openapiart/tests/common/
--rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/common/common.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.967118 openapiart-0.3.8/openapiart/tests/config/
--rw-r--r--   0 runner    (1001) docker     (127)    18298 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/config/config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/config/negative_nested_config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.971118 openapiart-0.3.8/openapiart/tests/field_uid/
--rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/field_uid/fielduid.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      761 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/field_uid/property_name_camel_case.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/field_uid/property_name_pascal_case.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/field_uid/property_name_upper_case.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/field_uid/xenum.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/field_uid/xinclude.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/grpcserver.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.971118 openapiart-0.3.8/openapiart/tests/multilevel/
--rw-r--r--   0 runner    (1001) docker     (127)      959 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/multilevel/multi.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.971118 openapiart-0.3.8/openapiart/tests/pattern/
--rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/pattern/invalid-pattern.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1531 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/pattern/pattern.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.971118 openapiart-0.3.8/openapiart/tests/response/
--rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/response/response_200_error.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/response/response_default_error.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/response/response_missing_required_in_error.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/response/response_required_error.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/server.py
--rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      558 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_auto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_bundle.py
--rw-r--r--   0 runner    (1001) docker     (127)      933 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_bundler.py
--rw-r--r--   0 runner    (1001) docker     (127)     3646 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_choice_with_no_property.py
--rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_constraints.py
--rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_enum_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_error_schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_fielduid.py
--rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_formats.py
--rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_func.py
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_grpc_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_http_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_integer_format.py
--rw-r--r--   0 runner    (1001) docker     (127)      290 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_license.py
--rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_perf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_protobuf.py
--rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_py_go_diff.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_required_choices.py
--rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_secure_grpc_response.py
--rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_unique.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_validate_integer_format.py
--rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_validate_property_name.py
--rw-r--r--   0 runner    (1001) docker     (127)     1758 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_validate_x_field_pattern.py
--rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_validate_xenum.py
--rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_validate_xinclude.py
--rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_validation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_warnings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/test_x_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.971118 openapiart-0.3.8/openapiart/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      677 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/utils/common.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.971118 openapiart-0.3.8/openapiart/tests/x-status/
--rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/x-status/invalid_x_status.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      822 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/tests/x-status/x_status_with_required.yaml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.971118 openapiart-0.3.8/openapiart/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-01-08 10:35:00.000000 openapiart-0.3.8/openapiart/utils/autofielduid.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-08 10:35:48.971118 openapiart-0.3.8/openapiart.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-01-08 10:35:48.000000 openapiart-0.3.8/openapiart.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3556 2024-01-08 10:35:48.000000 openapiart-0.3.8/openapiart.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-08 10:35:48.000000 openapiart-0.3.8/openapiart.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-08 10:35:48.000000 openapiart-0.3.8/openapiart.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-08 10:35:48.000000 openapiart-0.3.8/openapiart.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-08 10:35:00.000000 openapiart-0.3.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-01-08 10:35:00.000000 openapiart-0.3.8/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-08 10:35:48.975118 openapiart-0.3.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-01-08 10:35:00.000000 openapiart-0.3.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.106117 openapiart-0.3.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     1109 2024-01-16 10:41:42.000000 openapiart-0.3.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      156 2024-01-16 10:41:42.000000 openapiart-0.3.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-01-16 10:42:24.106117 openapiart-0.3.9/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.090117 openapiart-0.3.9/openapiart/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52599 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12349 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/common.go
+-rw-r--r--   0 runner    (1001) docker     (127)    40405 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1452 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/common_test.go
+-rw-r--r--   0 runner    (1001) docker     (127)    81902 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.090117 openapiart-0.3.9/openapiart/goserver/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.090117 openapiart-0.3.9/openapiart/goserver/api/
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/api/api.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1243 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/api/common.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2170 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/api/service_a.api.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      223 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/api/service_a.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2269 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/api/service_b.api.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      614 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/api/service_b.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     6228 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/generator_context.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16226 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/go_controller_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4216 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/go_interface_generator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3566 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/goserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/http_setup.go
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/response.go
+-rw-r--r--   0 runner    (1001) docker     (127)      289 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/string_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/goserver/writer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1672 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/gotidy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13444 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/openapiart.py
+-rw-r--r--   0 runner    (1001) docker     (127)   130847 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/openapiartgo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5236 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/openapiartplugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18724 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/openapiartprotobuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/openapiartpython.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1881 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (127)      569 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      136 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/test_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.098117 openapiart-0.3.9/openapiart/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.098117 openapiart-0.3.9/openapiart/tests/api/
+-rw-r--r--   0 runner    (1001) docker     (127)     3251 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/api/api.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/api/info.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.098117 openapiart-0.3.9/openapiart/tests/check_type/
+-rw-r--r--   0 runner    (1001) docker     (127)     1654 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/check_type/invalid_integer_type.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.098117 openapiart-0.3.9/openapiart/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (127)     2365 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/common/common.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.098117 openapiart-0.3.9/openapiart/tests/config/
+-rw-r--r--   0 runner    (1001) docker     (127)    18603 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/config/config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/config/negative_nested_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3798 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.102117 openapiart-0.3.9/openapiart/tests/field_uid/
+-rw-r--r--   0 runner    (1001) docker     (127)     4199 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/field_uid/fielduid.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      761 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/field_uid/property_name_camel_case.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/field_uid/property_name_pascal_case.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/field_uid/property_name_upper_case.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/field_uid/xenum.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2811 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/field_uid/xinclude.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     3952 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/grpcserver.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.102117 openapiart-0.3.9/openapiart/tests/multilevel/
+-rw-r--r--   0 runner    (1001) docker     (127)      959 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/multilevel/multi.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.102117 openapiart-0.3.9/openapiart/tests/pattern/
+-rw-r--r--   0 runner    (1001) docker     (127)     2083 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/pattern/invalid-pattern.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1736 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/pattern/pattern.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.102117 openapiart-0.3.9/openapiart/tests/response/
+-rw-r--r--   0 runner    (1001) docker     (127)     1724 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/response/response_200_error.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      762 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/response/response_default_error.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/response/response_missing_required_in_error.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1945 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/response/response_required_error.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     2754 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1263 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      558 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_auto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1006 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (127)      933 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_bundler.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4540 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_choice_with_no_property.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2046 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2430 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_enum_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2372 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_error_schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3124 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_fielduid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4603 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_formats.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6819 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_func.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_grpc_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3477 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_http_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8049 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_integer_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)      290 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_license.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3921 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_oid_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3260 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_perf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1029 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_protobuf.py
+-rw-r--r--   0 runner    (1001) docker     (127)      630 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_py_go_diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_required_choices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3626 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_secure_grpc_response.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6623 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3808 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_unique.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_validate_integer_format.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2076 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_validate_property_name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1765 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_validate_x_field_pattern.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1240 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_validate_xenum.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_validate_xinclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)      678 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_validation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5981 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_warnings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1523 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/test_x_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.102117 openapiart-0.3.9/openapiart/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      677 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/utils/common.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.102117 openapiart-0.3.9/openapiart/tests/x-status/
+-rw-r--r--   0 runner    (1001) docker     (127)      799 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/x-status/invalid_x_status.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      822 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/tests/x-status/x_status_with_required.yaml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.102117 openapiart-0.3.9/openapiart/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9031 2024-01-16 10:41:42.000000 openapiart-0.3.9/openapiart/utils/autofielduid.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-16 10:42:24.102117 openapiart-0.3.9/openapiart.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4756 2024-01-16 10:42:23.000000 openapiart-0.3.9/openapiart.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-01-16 10:42:23.000000 openapiart-0.3.9/openapiart.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-16 10:42:23.000000 openapiart-0.3.9/openapiart.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-01-16 10:42:23.000000 openapiart-0.3.9/openapiart.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-01-16 10:42:23.000000 openapiart-0.3.9/openapiart.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-01-16 10:41:42.000000 openapiart-0.3.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     2795 2024-01-16 10:41:42.000000 openapiart-0.3.9/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-16 10:42:24.106117 openapiart-0.3.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-01-16 10:41:42.000000 openapiart-0.3.9/setup.py
```

### Comparing `openapiart-0.3.8/LICENSE` & `openapiart-0.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/PKG-INFO` & `openapiart-0.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapiart
-Version: 0.3.8
+Version: 0.3.9
 Summary: The OpenAPI Artifact Generator Python Package
 Home-page: https://github.com/open-traffic-generator/openapiart
 Author: https://github.com/open-traffic-generator/openapiart
 Author-email: andy.balogh@keysight.com
 License: MIT
 Keywords: testing openapi artifact generator
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `openapiart-0.3.8/openapiart/bundler.py` & `openapiart-0.3.9/openapiart/bundler.py`

 * *Files 0% similar despite different names*

```diff
@@ -614,15 +614,15 @@
             "maxLength",
         }
         if isinstance(value, dict):
             intersect_keys = restricted_keys.intersection(set(value.keys()))
             if (
                 len(intersect_keys) > 0
                 and "format" in value.keys()
-                and value["format"] in ["ipv4", "ipv6", "mac"]
+                and value["format"] in ["ipv4", "ipv6", "mac", "oid"]
             ):
                 stacks = inspect.stack()
                 property = "{}/{}/{}".format(
                     stacks[3].frame.f_locals["key"]
                     if "key" in stacks[3].frame.f_locals
                     else "",
                     stacks[2].frame.f_locals["key"]
@@ -692,15 +692,15 @@
                 )
             if not isinstance(xpattern["signed"], bool):
                 self._errors.append(
                     "invalid value {} in {}, signed property can either be true or false".format(
                         str(xpattern["signed"]), str(xpattern_path.full_path)
                     )
                 )
-        valid_formats = ["integer", "ipv4", "ipv6", "mac", "checksum"]
+        valid_formats = ["integer", "ipv4", "ipv6", "mac", "checksum", "oid"]
         if xpattern["format"] not in valid_formats:
             self._errors.append(
                 "%s has unspported format %s , valid formats are %s"
                 % (
                     str(xpattern_path.full_path),
                     xpattern["format"],
                     str(valid_formats),
@@ -742,15 +742,15 @@
                         piece[0].upper() + piece[1:]
                         for piece in property_name.split("_")
                     ]
                 ),
             )
             fmt = None
             type_name = xpattern["format"]
-            if type_name in ["ipv4", "ipv6", "mac", "x-enum"]:
+            if type_name in ["ipv4", "ipv6", "mac", "x-enum", "oid"]:
                 fmt = type_name
                 type_name = "string"
             description = "TBD"
             if "description" in xpattern:
                 description = xpattern["description"]
             elif "description" in property_schema:
                 description = property_schema["description"]
```

### Comparing `openapiart-0.3.8/openapiart/common.go` & `openapiart-0.3.9/openapiart/common.go`

 * *Files 9% similar despite different names*

```diff
@@ -326,27 +326,44 @@
 	matched, err := regexp.MatchString(`^[0-9a-fA-F]+$|^0[x|X][0-9a-fA-F]+$`, hex)
 	if err != nil || !matched {
 		return fmt.Errorf(fmt.Sprintf("Invalid hex value %s", hex))
 	}
 	return nil
 }
 
+func (obj *validation) validateOid(oid string) error {
+	segments := strings.Split(oid, ".")
+	if len(segments) < 2 {
+		return fmt.Errorf(fmt.Sprintf("Invalid oid value %s", oid))
+	}
+
+	for _, segment := range segments {
+		number, err := strconv.Atoi(segment)
+		if err != nil || 0 > number || number > 4294967295 {
+			return fmt.Errorf(fmt.Sprintf("Invalid oid value %s", oid))
+		}
+	}
+	return nil
+}
+
 func (obj *validation) validateSlice(valSlice []string, sliceType string) error {
 	indices := []string{}
 	var err error
 	for i, val := range valSlice {
 		if sliceType == "mac" {
 			err = obj.validateMac(val)
 		} else if sliceType == "ipv4" {
 			err = obj.validateIpv4(val)
 
 		} else if sliceType == "ipv6" {
 			err = obj.validateIpv6(val)
 		} else if sliceType == "hex" {
 			err = obj.validateHex(val)
+		} else if sliceType == "oid" {
+			err = obj.validateOid(val)
 		} else {
 			return fmt.Errorf(fmt.Sprintf("Invalid slice type received <%s>", sliceType))
 		}
 
 		if err != nil {
 			indices = append(indices, fmt.Sprintf("%d", i))
 		}
@@ -371,14 +388,18 @@
 	return obj.validateSlice(ip, "ipv6")
 }
 
 func (obj *validation) validateHexSlice(hex []string) error {
 	return obj.validateSlice(hex, "hex")
 }
 
+func (obj *validation) validateOidSlice(oid []string) error {
+	return obj.validateSlice(oid, "oid")
+}
+
 // TODO: restore behavior
 // func (obj *validation) createMap(objName string) {
 // 	if obj.constraints == nil {
 // 		obj.constraints = make(map[string]map[string]Constraints)
 // 	}
 // 	_, ok := obj.constraints[objName]
 // 	if !ok {
```

### Comparing `openapiart-0.3.8/openapiart/common.py` & `openapiart-0.3.9/openapiart/common.py`

 * *Files 1% similar despite different names*

```diff
@@ -483,14 +483,25 @@
         return all(
             [
                 True if int(bin) == 0 or int(bin) == 1 else False
                 for bin in value
             ]
         )
 
+    def validate_oid(self, value):
+        segments = value.split(".")
+        if len(segments) < 2:
+            return False
+        for segment in segments:
+            if not segment.isnumeric():
+                return False
+            if not (0 <= int(segment) <= 4294967295):
+                return False
+        return True
+
     def types_validation(
         self,
         value,
         type_,
         err_msg,
         itemtype=None,
         min=None,
@@ -694,18 +705,21 @@
                 )
             else:
                 self._properties[name] = default_value(parent=parent)
             if (
                 "_DEFAULTS" in dir(self._properties[name])
                 and "choice" in self._properties[name]._DEFAULTS
             ):
-                getattr(
-                    self._properties[name],
-                    self._properties[name]._DEFAULTS["choice"],
-                )
+                choice_str = self._properties[name]._DEFAULTS["choice"]
+
+                if choice_str in self._properties[name]._TYPES:
+                    getattr(
+                        self._properties[name],
+                        self._properties[name]._DEFAULTS["choice"],
+                    )
         else:
             if default_value is None and name in self._DEFAULTS:
                 self._set_choice(name)
                 self._properties[name] = self._DEFAULTS[name]
             else:
                 self._properties[name] = default_value
         return self._properties[name]
```

### Comparing `openapiart-0.3.8/openapiart/common_test.go` & `openapiart-0.3.9/openapiart/common_test.go`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/generator.py` & `openapiart-0.3.9/openapiart/generator.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/goserver/api/common.yaml` & `openapiart-0.3.9/openapiart/goserver/api/common.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/goserver/api/service_a.api.yaml` & `openapiart-0.3.9/openapiart/goserver/api/service_a.api.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/goserver/api/service_b.api.yaml` & `openapiart-0.3.9/openapiart/goserver/api/service_b.api.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/goserver/api/service_b.yaml` & `openapiart-0.3.9/openapiart/goserver/api/service_b.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/goserver/generator_context.py` & `openapiart-0.3.9/openapiart/goserver/generator_context.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/goserver/go_controller_generator.py` & `openapiart-0.3.9/openapiart/goserver/go_controller_generator.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/goserver/go_interface_generator.py` & `openapiart-0.3.9/openapiart/goserver/go_interface_generator.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/goserver/goserver.py` & `openapiart-0.3.9/openapiart/goserver/goserver.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/goserver/http_setup.go` & `openapiart-0.3.9/openapiart/goserver/http_setup.go`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/goserver/response.go` & `openapiart-0.3.9/openapiart/goserver/response.go`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/goserver/writer.py` & `openapiart-0.3.9/openapiart/goserver/writer.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/gotidy.py` & `openapiart-0.3.9/openapiart/gotidy.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/openapiart.py` & `openapiart-0.3.9/openapiart/openapiart.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/openapiartgo.py` & `openapiart-0.3.9/openapiart/openapiartgo.py`

 * *Files 0% similar despite different names*

```diff
@@ -2698,15 +2698,16 @@
                         body=inner_body, name=field.name
                     )
             elif field.itemformat in [
                 "mac",
                 "ipv4",
                 "ipv6",
                 "hex",
-            ] or field.format in ["mac", "ipv4", "ipv6", "hex"]:
+                "oid",
+            ] or field.format in ["mac", "ipv4", "ipv6", "hex", "oid"]:
                 if field.format is None:
                     field.format = field.itemformat
                 inner_body = """
                     err := obj.validate{format}(obj.{name}())
                     if err != nil {{
                         vObj.validationErrors = append(vObj.validationErrors, fmt.Sprintf("%s %s", err.Error(), "on {interface}.{name}"))
                     }}
```

### Comparing `openapiart-0.3.8/openapiart/openapiartplugin.py` & `openapiart-0.3.9/openapiart/openapiartplugin.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/openapiartprotobuf.py` & `openapiart-0.3.9/openapiart/openapiartprotobuf.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/requirements.py` & `openapiart-0.3.9/openapiart/requirements.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/requirements.txt` & `openapiart-0.3.9/openapiart/requirements.txt`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/api/api.yaml` & `openapiart-0.3.9/openapiart/tests/api/api.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/api/info.yaml` & `openapiart-0.3.9/openapiart/tests/api/info.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/check_type/invalid_integer_type.yaml` & `openapiart-0.3.9/openapiart/tests/check_type/invalid_integer_type.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/common/common.yaml` & `openapiart-0.3.9/openapiart/tests/common/common.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/config/config.yaml` & `openapiart-0.3.9/openapiart/tests/config/config.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -306,14 +306,20 @@
             type: integer
           minimum: 64
           maximum: 9000
           x-field-uid: 52
         signed_integer_pattern:
           $ref: "../pattern/pattern.yaml#/components/schemas/SignedIntegerPattern"
           x-field-uid: 53
+        oid_pattern:
+          $ref: "../pattern/pattern.yaml#/components/schemas/OidPattern"
+          x-field-uid: 54
+        choice_default:
+          $ref: "#/components/schemas/ChoiceObject"
+          x-field-uid: 55
 
     WObject:
       required: [w_name]
       properties:
         w_name:
           type: string
           x-field-uid: 1
@@ -561,14 +567,18 @@
           type: string
           format: ipv6
           x-field-uid: 7
         hex:
           type: string
           format: hex
           x-field-uid: 8
+        oid:
+          type: string
+          format: oid
+          x-field-uid: 9
     Mandate:
       description: "Object to Test required Parameter"
       type: object
       required: ["required_param"]
       properties:
         required_param:
           type: string
```

### Comparing `openapiart-0.3.8/openapiart/tests/config/negative_nested_config.yaml` & `openapiart-0.3.9/openapiart/tests/config/negative_nested_config.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/conftest.py` & `openapiart-0.3.9/openapiart/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/field_uid/fielduid.yaml` & `openapiart-0.3.9/openapiart/tests/field_uid/fielduid.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/field_uid/property_name_camel_case.yaml` & `openapiart-0.3.9/openapiart/tests/field_uid/property_name_camel_case.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/field_uid/property_name_pascal_case.yaml` & `openapiart-0.3.9/openapiart/tests/field_uid/property_name_pascal_case.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/field_uid/property_name_upper_case.yaml` & `openapiart-0.3.9/openapiart/tests/field_uid/property_name_upper_case.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/field_uid/xenum.yaml` & `openapiart-0.3.9/openapiart/tests/field_uid/xenum.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/field_uid/xinclude.yaml` & `openapiart-0.3.9/openapiart/tests/field_uid/xinclude.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/grpcserver.py` & `openapiart-0.3.9/openapiart/tests/grpcserver.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/multilevel/multi.yaml` & `openapiart-0.3.9/openapiart/tests/multilevel/multi.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/pattern/invalid-pattern.yaml` & `openapiart-0.3.9/openapiart/tests/pattern/invalid-pattern.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/pattern/pattern.yaml` & `openapiart-0.3.9/openapiart/tests/pattern/pattern.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -57,7 +57,16 @@
           x-field-pattern:
             format: integer
             default: 0
             signed: true
             length: 8
             features: [count]
           x-field-uid: 1
+    OidPattern:
+      description: Test oid pattern
+      type: object
+      properties:
+        oid:
+          x-field-pattern:
+            format: oid
+            default: "0.1"
+          x-field-uid: 1
```

### Comparing `openapiart-0.3.8/openapiart/tests/response/response_200_error.yaml` & `openapiart-0.3.9/openapiart/tests/response/response_200_error.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/response/response_default_error.yaml` & `openapiart-0.3.9/openapiart/tests/response/response_default_error.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/response/response_missing_required_in_error.yaml` & `openapiart-0.3.9/openapiart/tests/response/response_missing_required_in_error.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/response/response_required_error.yaml` & `openapiart-0.3.9/openapiart/tests/response/response_required_error.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/server.py` & `openapiart-0.3.9/openapiart/tests/server.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_add.py` & `openapiart-0.3.9/openapiart/tests/test_add.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_auto.py` & `openapiart-0.3.9/openapiart/tests/test_auto.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_bundle.py` & `openapiart-0.3.9/openapiart/tests/test_bundle.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_bundler.py` & `openapiart-0.3.9/openapiart/tests/test_bundler.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_choice_with_no_property.py` & `openapiart-0.3.9/openapiart/tests/test_choice_with_no_property.py`

 * *Files 14% similar despite different names*

```diff
@@ -86,14 +86,42 @@
     s_c_obj = c_obj.serialize()
     c_obj.deserialize(s_c_obj)
     assert c_obj.choice == "f_obj"
     assert c_obj._properties.get("f_obj") is not None
     assert c_obj.f_obj.choice == "f_c"
 
 
+def test_choice_in_choice_default(api):
+    config = api.prefix_config()
+
+    # default choice with no properties should be set properly
+    c_obj = config.choice_default
+    assert c_obj.choice == "no_obj"
+    assert len(c_obj._properties) == 1
+
+    # acesing of objects with choice set to choice with no property should work
+    f_obj = c_obj.f_obj
+
+    # check default in child
+    assert f_obj.choice == "f_a"
+    assert f_obj._properties.get("f_a", None) is not None
+
+    # setting choice with no properties in child as well
+    f_obj.choice = "f_c"
+    assert f_obj._properties.get("choice", None) == "f_c"
+    len(f_obj._properties) == 1
+
+    # serialize and deserialize should have no problem
+    s_c_obj = c_obj.serialize()
+    c_obj.deserialize(s_c_obj)
+    assert c_obj.choice == "f_obj"
+    assert c_obj._properties.get("f_obj") is not None
+    assert c_obj.f_obj.choice == "f_c"
+
+
 def test_choice_with_invalid_enum_and_none_value(api):
     config = api.prefix_config()
     f_obj = config.f
 
     # check default
     assert f_obj.choice == "f_a"
     assert f_obj._properties.get("f_a", None) is not None
```

### Comparing `openapiart-0.3.8/openapiart/tests/test_constraints.py` & `openapiart-0.3.9/openapiart/tests/test_constraints.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_enum_validation.py` & `openapiart-0.3.9/openapiart/tests/test_enum_validation.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_error_schema.py` & `openapiart-0.3.9/openapiart/tests/test_error_schema.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_fielduid.py` & `openapiart-0.3.9/openapiart/tests/test_fielduid.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_formats.py` & `openapiart-0.3.9/openapiart/tests/test_formats.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_func.py` & `openapiart-0.3.9/openapiart/tests/test_func.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_grpc_response.py` & `openapiart-0.3.9/openapiart/tests/test_grpc_response.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_http_response.py` & `openapiart-0.3.9/openapiart/tests/test_http_response.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_integer_format.py` & `openapiart-0.3.9/openapiart/tests/test_integer_format.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_perf.py` & `openapiart-0.3.9/openapiart/tests/test_perf.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_protobuf.py` & `openapiart-0.3.9/openapiart/tests/test_protobuf.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_py_go_diff.py` & `openapiart-0.3.9/openapiart/tests/test_py_go_diff.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_remove.py` & `openapiart-0.3.9/openapiart/tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_required_choices.py` & `openapiart-0.3.9/openapiart/tests/test_required_choices.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_secure_grpc_response.py` & `openapiart-0.3.9/openapiart/tests/test_secure_grpc_response.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_set.py` & `openapiart-0.3.9/openapiart/tests/test_set.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_unique.py` & `openapiart-0.3.9/openapiart/tests/test_unique.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_validate_integer_format.py` & `openapiart-0.3.9/openapiart/tests/test_validate_integer_format.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_validate_property_name.py` & `openapiart-0.3.9/openapiart/tests/test_validate_property_name.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_validate_x_field_pattern.py` & `openapiart-0.3.9/openapiart/tests/test_validate_x_field_pattern.py`

 * *Files 5% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 def str_compare(validte_str, entire_str):
     return validte_str in entire_str
 
 
 def test_validate_pattern():
     error_msgs = [
         "components.schemas.Config.properties.integer.x-field-pattern property using x-field-pattern with format integer must contain length property",
-        "components.schemas.Config.properties.wrong.x-field-pattern has unspported format random , valid formats are ['integer', 'ipv4', 'ipv6', 'mac', 'checksum']",
+        "components.schemas.Config.properties.wrong.x-field-pattern has unspported format random , valid formats are ['integer', 'ipv4', 'ipv6', 'mac', 'checksum', 'oid']",
         "components.schemas.Config.properties.int_128.x-field-pattern property using x-field-pattern with format integer cannot have length greater than 64",
         "signed property can only be used if the format is set to integer in property components.schemas.Config.properties.signed_value_without_int.x-field-pattern",
         "invalid value 45 in components.schemas.Config.properties.wrong_int_signed_value.x-field-pattern, signed property can either be true or false",
     ]
     with pytest.raises(Exception) as execinfo:
         create_openapi_artifacts(
             openapiart_class,
```

### Comparing `openapiart-0.3.8/openapiart/tests/test_validate_xenum.py` & `openapiart-0.3.9/openapiart/tests/test_validate_xenum.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_validate_xinclude.py` & `openapiart-0.3.9/openapiart/tests/test_validate_xinclude.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_validation.py` & `openapiart-0.3.9/openapiart/tests/test_validation.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_warnings.py` & `openapiart-0.3.9/openapiart/tests/test_warnings.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/test_x_status.py` & `openapiart-0.3.9/openapiart/tests/test_x_status.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/utils/common.py` & `openapiart-0.3.9/openapiart/tests/utils/common.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/x-status/invalid_x_status.yaml` & `openapiart-0.3.9/openapiart/tests/x-status/invalid_x_status.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/tests/x-status/x_status_with_required.yaml` & `openapiart-0.3.9/openapiart/tests/x-status/x_status_with_required.yaml`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart/utils/autofielduid.py` & `openapiart-0.3.9/openapiart/utils/autofielduid.py`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/openapiart.egg-info/PKG-INFO` & `openapiart-0.3.9/openapiart.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: openapiart
-Version: 0.3.8
+Version: 0.3.9
 Summary: The OpenAPI Artifact Generator Python Package
 Home-page: https://github.com/open-traffic-generator/openapiart
 Author: https://github.com/open-traffic-generator/openapiart
 Author-email: andy.balogh@keysight.com
 License: MIT
 Keywords: testing openapi artifact generator
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `openapiart-0.3.8/openapiart.egg-info/SOURCES.txt` & `openapiart-0.3.9/openapiart.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -53,14 +53,15 @@
 openapiart/tests/test_fielduid.py
 openapiart/tests/test_formats.py
 openapiart/tests/test_func.py
 openapiart/tests/test_grpc_response.py
 openapiart/tests/test_http_response.py
 openapiart/tests/test_integer_format.py
 openapiart/tests/test_license.py
+openapiart/tests/test_oid_format.py
 openapiart/tests/test_perf.py
 openapiart/tests/test_protobuf.py
 openapiart/tests/test_py_go_diff.py
 openapiart/tests/test_remove.py
 openapiart/tests/test_required_choices.py
 openapiart/tests/test_secure_grpc_response.py
 openapiart/tests/test_set.py
```

### Comparing `openapiart-0.3.8/readme.md` & `openapiart-0.3.9/readme.md`

 * *Files identical despite different names*

### Comparing `openapiart-0.3.8/setup.py` & `openapiart-0.3.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """
 To build distribution: python setup.py sdist --formats=gztar bdist_wheel --universal
 """
 import os
 import setuptools
 
 pkg_name = "openapiart"
-version = "0.3.8"
+version = "0.3.9"
 
 base_dir = os.path.dirname(os.path.abspath(__file__))
 with open(os.path.join(base_dir, "readme.md")) as fid:
     long_description = fid.read()
 
 requirements_path = os.path.join(base_dir, "openapiart", "requirements.txt")
 test_req_path = os.path.join(base_dir, "openapiart", "test_requirements.txt")
```

