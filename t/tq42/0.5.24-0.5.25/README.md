# Comparing `tmp/tq42-0.5.24.tar.gz` & `tmp/tq42-0.5.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tq42-0.5.24.tar", max compression
+gzip compressed data, was "tq42-0.5.25.tar", max compression
```

## Comparing `tq42-0.5.24.tar` & `tq42-0.5.25.tar`

### file list

```diff
@@ -1,83 +1,83 @@
--rw-r--r--   0        0        0    11357 2024-05-03 15:44:22.049384 tq42-0.5.24/LICENSE
--rw-r--r--   0        0        0     5911 2024-05-03 15:44:22.049384 tq42-0.5.24/README.md
--rw-r--r--   0        0        0      750 2024-05-03 15:44:22.073384 tq42-0.5.24/pyproject.toml
--rw-r--r--   0        0        0       76 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/__init__.py
--rwxr-xr-x   0        0        0      977 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/__main__.py
--rw-r--r--   0        0        0     3086 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/algorithm.py
--rw-r--r--   0        0        0        0 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/__init__.py
--rw-r--r--   0        0        0     3133 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/cli_functions.py
--rw-r--r--   0        0        0     1017 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/compute_group.py
--rw-r--r--   0        0        0     1053 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/experiment_group.py
--rw-r--r--   0        0        0     1478 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/experiment_run_group.py
--rw-r--r--   0        0        0      420 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/organization_group.py
--rw-r--r--   0        0        0        0 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/output_format/__init__.py
--rw-r--r--   0        0        0     3243 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/output_format/formatter.py
--rw-r--r--   0        0        0        0 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/parsers/__init__.py
--rw-r--r--   0        0        0     2688 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/parsers/params_checker.py
--rw-r--r--   0        0        0     5891 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/parsers/tq42parser.py
--rw-r--r--   0        0        0      783 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/project_dataset_group.py
--rw-r--r--   0        0        0      719 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/project_group.py
--rw-r--r--   0        0        0     1201 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/tq42_all.py
--rw-r--r--   0        0        0     3500 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/cli/tq42_help.py
--rw-r--r--   0        0        0     9781 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/client.py
--rw-r--r--   0        0        0     2282 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/compute.py
--rw-r--r--   0        0        0     2890 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/dataset.py
--rw-r--r--   0        0        0     2355 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/exception_handling.py
--rw-r--r--   0        0        0     2033 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/exceptions.py
--rw-r--r--   0        0        0     4133 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/experiment.py
--rw-r--r--   0        0        0     6109 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/experiment_run.py
--rw-r--r--   0        0        0        0 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/functional_tests/__init__.py
--rw-r--r--   0        0        0      573 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/functional_tests/conftest.py
--rw-r--r--   0        0        0     3396 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/functional_tests/functional_test_config.py
--rw-r--r--   0        0        0        0 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/functional_tests/invoke_cli/__init__.py
--rw-r--r--   0        0        0     1474 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/functional_tests/invoke_cli/test_functional_cli.py
--rw-r--r--   0        0        0     1523 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/functional_tests/invoke_cli/test_functional_compute_group.py
--rw-r--r--   0        0        0     1190 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/functional_tests/invoke_cli/test_functional_experiment_group.py
--rw-r--r--   0        0        0     2404 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/functional_tests/invoke_cli/test_functional_experiment_run_group.py
--rw-r--r--   0        0        0      678 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/functional_tests/invoke_cli/test_functional_organization_group.py
--rw-r--r--   0        0        0     1222 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/functional_tests/invoke_cli/test_functional_project_group.py
--rw-r--r--   0        0        0      689 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/functional_tests/test_functional_cache_utils.py
--rw-r--r--   0        0        0     5721 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/functional_tests/test_functional_tq42_api.py
--rw-r--r--   0        0        0     1371 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/functional_tests/test_polling_function.py
--rw-r--r--   0        0        0      437 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/functional_tests/test_test_config.py
--rw-r--r--   0        0        0     3199 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/organization.py
--rw-r--r--   0        0        0     5511 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/project.py
--rw-r--r--   0        0        0        0 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/cli/__init__.py
--rw-r--r--   0        0        0     4861 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/cli/test_output_format.py
--rw-r--r--   0        0        0     6185 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/cli/test_tq42_help.py
--rw-r--r--   0        0        0     3787 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/cli/test_tq42_help_flags.py
--rw-r--r--   0        0        0      892 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/test_cache_utils.py
--rw-r--r--   0        0        0      806 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/test_compute.py
--rw-r--r--   0        0        0     2253 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/test_config_environment.py
--rw-r--r--   0        0        0     1890 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/test_dirs.py
--rw-r--r--   0        0        0      825 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/test_example.py
--rw-r--r--   0        0        0     1475 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/test_imports.py
--rw-r--r--   0        0        0      159 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/test_package_version.py
--rw-r--r--   0        0        0     7800 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/test_tq42_api.py
--rw-r--r--   0        0        0     7617 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/test_tq42_error_handling.py
--rw-r--r--   0        0        0    10223 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/test_utils.py
--rwxr-xr-x   0        0        0       48 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/testdata/README.md
--rw-r--r--   0        0        0      147 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/testdata/config.json
--rwxr-xr-x   0        0        0      460 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/testdata/test_convert_colon_separated_string_to_dict.txt
--rwxr-xr-x   0        0        0      210 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/tests/testdata/test_utils_get_id.txt
--rw-r--r--   0        0        0        0 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/utils/__init__.py
--rw-r--r--   0        0        0      547 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/utils/constants.py
--rw-r--r--   0        0        0     1256 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/utils/dirs.py
--rw-r--r--   0        0        0     1828 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/utils/environment_utils.py
--rw-r--r--   0        0        0      365 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/utils/file_handling.py
--rw-r--r--   0        0        0      147 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/utils/text_files/config.json
--rwxr-xr-x   0        0        0      132 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/utils/text_files/cpu_configs.json
--rwxr-xr-x   0        0        0      829 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/utils/text_files/hardware_configs.json
--rw-r--r--   0        0        0    14193 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/utils/text_files/help.json
--rw-r--r--   0        0        0     2342 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/utils/text_files/help_flags.json
--rw-r--r--   0        0        0      491 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/utils/text_files/insufficient_permission_error.txt
--rw-r--r--   0        0        0      130 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/utils/text_files/invalid_arguments_error.txt
--rw-r--r--   0        0        0      191 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/utils/text_files/local_permission_error.txt
--rw-r--r--   0        0        0      470 2024-05-03 15:44:22.073384 tq42-0.5.24/tq42/utils/text_files/no_default_error.txt
--rwxr-xr-x   0        0        0      657 2024-05-03 15:44:22.077384 tq42-0.5.24/tq42/utils/text_files/tq42_commands.txt
--rw-r--r--   0        0        0      329 2024-05-03 15:44:22.077384 tq42-0.5.24/tq42/utils/text_files/unauthenticated_error.txt
--rw-r--r--   0        0        0     2284 2024-05-03 15:44:22.077384 tq42-0.5.24/tq42/utils/token_manager.py
--rw-r--r--   0        0        0     4469 2024-05-03 15:44:22.077384 tq42-0.5.24/tq42/utils/utils.py
--rw-r--r--   0        0        0      966 2024-05-03 15:44:22.077384 tq42-0.5.24/tq42/utils/utils_for_cache.py
--rw-r--r--   0        0        0     6573 1970-01-01 00:00:00.000000 tq42-0.5.24/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-16 14:50:21.905427 tq42-0.5.25/LICENSE
+-rw-r--r--   0        0        0     5911 2024-05-16 14:50:21.905427 tq42-0.5.25/README.md
+-rw-r--r--   0        0        0      750 2024-05-16 14:50:21.929427 tq42-0.5.25/pyproject.toml
+-rw-r--r--   0        0        0       76 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/__init__.py
+-rwxr-xr-x   0        0        0      977 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/__main__.py
+-rw-r--r--   0        0        0     3086 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/algorithm.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/__init__.py
+-rw-r--r--   0        0        0     3133 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/cli_functions.py
+-rw-r--r--   0        0        0     1017 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/compute_group.py
+-rw-r--r--   0        0        0     1053 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/experiment_group.py
+-rw-r--r--   0        0        0     1478 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/experiment_run_group.py
+-rw-r--r--   0        0        0      420 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/organization_group.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/output_format/__init__.py
+-rw-r--r--   0        0        0     3243 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/output_format/formatter.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/parsers/__init__.py
+-rw-r--r--   0        0        0     2688 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/parsers/params_checker.py
+-rw-r--r--   0        0        0     5891 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/parsers/tq42parser.py
+-rw-r--r--   0        0        0      783 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/project_dataset_group.py
+-rw-r--r--   0        0        0      719 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/project_group.py
+-rw-r--r--   0        0        0     1201 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/tq42_all.py
+-rw-r--r--   0        0        0     3500 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/cli/tq42_help.py
+-rw-r--r--   0        0        0     9781 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/client.py
+-rw-r--r--   0        0        0     2282 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/compute.py
+-rw-r--r--   0        0        0     2890 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/dataset.py
+-rw-r--r--   0        0        0     2355 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/exception_handling.py
+-rw-r--r--   0        0        0     2033 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/exceptions.py
+-rw-r--r--   0        0        0     4133 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/experiment.py
+-rw-r--r--   0        0        0     6109 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/experiment_run.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/functional_tests/__init__.py
+-rw-r--r--   0        0        0      573 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/functional_tests/conftest.py
+-rw-r--r--   0        0        0     3396 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/functional_tests/functional_test_config.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/functional_tests/invoke_cli/__init__.py
+-rw-r--r--   0        0        0     1474 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/functional_tests/invoke_cli/test_functional_cli.py
+-rw-r--r--   0        0        0     1523 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/functional_tests/invoke_cli/test_functional_compute_group.py
+-rw-r--r--   0        0        0     1190 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/functional_tests/invoke_cli/test_functional_experiment_group.py
+-rw-r--r--   0        0        0     2404 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/functional_tests/invoke_cli/test_functional_experiment_run_group.py
+-rw-r--r--   0        0        0      678 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/functional_tests/invoke_cli/test_functional_organization_group.py
+-rw-r--r--   0        0        0     1222 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/functional_tests/invoke_cli/test_functional_project_group.py
+-rw-r--r--   0        0        0      689 2024-05-16 14:50:21.929427 tq42-0.5.25/tq42/functional_tests/test_functional_cache_utils.py
+-rw-r--r--   0        0        0     5721 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/functional_tests/test_functional_tq42_api.py
+-rw-r--r--   0        0        0     1371 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/functional_tests/test_polling_function.py
+-rw-r--r--   0        0        0      437 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/functional_tests/test_test_config.py
+-rw-r--r--   0        0        0     3199 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/organization.py
+-rw-r--r--   0        0        0     5511 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/project.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/cli/__init__.py
+-rw-r--r--   0        0        0     4861 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/cli/test_output_format.py
+-rw-r--r--   0        0        0     6185 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/cli/test_tq42_help.py
+-rw-r--r--   0        0        0     3787 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/cli/test_tq42_help_flags.py
+-rw-r--r--   0        0        0      892 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/test_cache_utils.py
+-rw-r--r--   0        0        0      806 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/test_compute.py
+-rw-r--r--   0        0        0     2253 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/test_config_environment.py
+-rw-r--r--   0        0        0     1890 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/test_dirs.py
+-rw-r--r--   0        0        0      825 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/test_example.py
+-rw-r--r--   0        0        0     1475 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/test_imports.py
+-rw-r--r--   0        0        0      159 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/test_package_version.py
+-rw-r--r--   0        0        0     7800 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/test_tq42_api.py
+-rw-r--r--   0        0        0     7617 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/test_tq42_error_handling.py
+-rw-r--r--   0        0        0    10223 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/test_utils.py
+-rwxr-xr-x   0        0        0       48 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/testdata/README.md
+-rw-r--r--   0        0        0      147 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/testdata/config.json
+-rwxr-xr-x   0        0        0      460 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/testdata/test_convert_colon_separated_string_to_dict.txt
+-rwxr-xr-x   0        0        0      210 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/tests/testdata/test_utils_get_id.txt
+-rw-r--r--   0        0        0        0 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/__init__.py
+-rw-r--r--   0        0        0      547 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/constants.py
+-rw-r--r--   0        0        0     1256 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/dirs.py
+-rw-r--r--   0        0        0     1828 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/environment_utils.py
+-rw-r--r--   0        0        0      365 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/file_handling.py
+-rw-r--r--   0        0        0      147 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/text_files/config.json
+-rwxr-xr-x   0        0        0      132 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/text_files/cpu_configs.json
+-rwxr-xr-x   0        0        0      829 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/text_files/hardware_configs.json
+-rw-r--r--   0        0        0    14193 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/text_files/help.json
+-rw-r--r--   0        0        0     2342 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/text_files/help_flags.json
+-rw-r--r--   0        0        0      491 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/text_files/insufficient_permission_error.txt
+-rw-r--r--   0        0        0      130 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/text_files/invalid_arguments_error.txt
+-rw-r--r--   0        0        0      191 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/text_files/local_permission_error.txt
+-rw-r--r--   0        0        0      470 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/text_files/no_default_error.txt
+-rwxr-xr-x   0        0        0      657 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/text_files/tq42_commands.txt
+-rw-r--r--   0        0        0      329 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/text_files/unauthenticated_error.txt
+-rw-r--r--   0        0        0     2284 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/token_manager.py
+-rw-r--r--   0        0        0     4469 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/utils.py
+-rw-r--r--   0        0        0      966 2024-05-16 14:50:21.933427 tq42-0.5.25/tq42/utils/utils_for_cache.py
+-rw-r--r--   0        0        0     6573 1970-01-01 00:00:00.000000 tq42-0.5.25/PKG-INFO
```

### Comparing `tq42-0.5.24/LICENSE` & `tq42-0.5.25/LICENSE`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/README.md` & `tq42-0.5.25/README.md`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/pyproject.toml` & `tq42-0.5.25/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 include = ["utils/text_files/*.txt", "utils/text_files/config.json", "tests/testdata/*.txt"]
 
 [tool.poetry]
 name = "tq42"
-version = "0.5.24"
+version = "0.5.25"
 description = "tq42 sdk"
 readme = "README.md"
 authors = ["Terra Quantum AG"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 requests = "2.31.0"
 PyYAML = "^6.0.1"
-tq42_grpc_client = "1.0.112"
+tq42_grpc_client = "1.0.120"
 pytest = "^7.4.4"
 keyring = "^25.0.0"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
```

### Comparing `tq42-0.5.24/tq42/__main__.py` & `tq42-0.5.25/tq42/__main__.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/algorithm.py` & `tq42-0.5.25/tq42/algorithm.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/cli/cli_functions.py` & `tq42-0.5.25/tq42/cli/cli_functions.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/cli/compute_group.py` & `tq42-0.5.25/tq42/cli/compute_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/cli/experiment_group.py` & `tq42-0.5.25/tq42/cli/experiment_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/cli/experiment_run_group.py` & `tq42-0.5.25/tq42/cli/experiment_run_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/cli/output_format/formatter.py` & `tq42-0.5.25/tq42/cli/output_format/formatter.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/cli/parsers/params_checker.py` & `tq42-0.5.25/tq42/cli/parsers/params_checker.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/cli/parsers/tq42parser.py` & `tq42-0.5.25/tq42/cli/parsers/tq42parser.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/cli/project_dataset_group.py` & `tq42-0.5.25/tq42/cli/project_dataset_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/cli/project_group.py` & `tq42-0.5.25/tq42/cli/project_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/cli/tq42_all.py` & `tq42-0.5.25/tq42/cli/tq42_all.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/cli/tq42_help.py` & `tq42-0.5.25/tq42/cli/tq42_help.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/client.py` & `tq42-0.5.25/tq42/client.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/compute.py` & `tq42-0.5.25/tq42/compute.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/dataset.py` & `tq42-0.5.25/tq42/dataset.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/exception_handling.py` & `tq42-0.5.25/tq42/exception_handling.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/exceptions.py` & `tq42-0.5.25/tq42/exceptions.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/experiment.py` & `tq42-0.5.25/tq42/experiment.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/experiment_run.py` & `tq42-0.5.25/tq42/experiment_run.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/functional_tests/conftest.py` & `tq42-0.5.25/tq42/functional_tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/functional_tests/functional_test_config.py` & `tq42-0.5.25/tq42/functional_tests/functional_test_config.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/functional_tests/invoke_cli/test_functional_cli.py` & `tq42-0.5.25/tq42/functional_tests/invoke_cli/test_functional_cli.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/functional_tests/invoke_cli/test_functional_compute_group.py` & `tq42-0.5.25/tq42/functional_tests/invoke_cli/test_functional_compute_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/functional_tests/invoke_cli/test_functional_experiment_group.py` & `tq42-0.5.25/tq42/functional_tests/invoke_cli/test_functional_experiment_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/functional_tests/invoke_cli/test_functional_experiment_run_group.py` & `tq42-0.5.25/tq42/functional_tests/invoke_cli/test_functional_experiment_run_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/functional_tests/invoke_cli/test_functional_organization_group.py` & `tq42-0.5.25/tq42/functional_tests/invoke_cli/test_functional_organization_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/functional_tests/invoke_cli/test_functional_project_group.py` & `tq42-0.5.25/tq42/functional_tests/invoke_cli/test_functional_project_group.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/functional_tests/test_functional_cache_utils.py` & `tq42-0.5.25/tq42/functional_tests/test_functional_cache_utils.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/functional_tests/test_functional_tq42_api.py` & `tq42-0.5.25/tq42/functional_tests/test_functional_tq42_api.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/functional_tests/test_polling_function.py` & `tq42-0.5.25/tq42/functional_tests/test_polling_function.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/organization.py` & `tq42-0.5.25/tq42/organization.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/project.py` & `tq42-0.5.25/tq42/project.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/tests/cli/test_output_format.py` & `tq42-0.5.25/tq42/tests/cli/test_output_format.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/tests/cli/test_tq42_help.py` & `tq42-0.5.25/tq42/tests/cli/test_tq42_help.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/tests/cli/test_tq42_help_flags.py` & `tq42-0.5.25/tq42/tests/cli/test_tq42_help_flags.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/tests/test_cache_utils.py` & `tq42-0.5.25/tq42/tests/test_cache_utils.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/tests/test_compute.py` & `tq42-0.5.25/tq42/tests/test_compute.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/tests/test_config_environment.py` & `tq42-0.5.25/tq42/tests/test_config_environment.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/tests/test_dirs.py` & `tq42-0.5.25/tq42/tests/test_dirs.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/tests/test_example.py` & `tq42-0.5.25/tq42/tests/test_example.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/tests/test_imports.py` & `tq42-0.5.25/tq42/tests/test_imports.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/tests/test_tq42_api.py` & `tq42-0.5.25/tq42/tests/test_tq42_api.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/tests/test_tq42_error_handling.py` & `tq42-0.5.25/tq42/tests/test_tq42_error_handling.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/tests/test_utils.py` & `tq42-0.5.25/tq42/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/utils/constants.py` & `tq42-0.5.25/tq42/utils/constants.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/utils/dirs.py` & `tq42-0.5.25/tq42/utils/dirs.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/utils/environment_utils.py` & `tq42-0.5.25/tq42/utils/environment_utils.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/utils/text_files/hardware_configs.json` & `tq42-0.5.25/tq42/utils/text_files/hardware_configs.json`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/utils/text_files/help.json` & `tq42-0.5.25/tq42/utils/text_files/help.json`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/utils/text_files/help_flags.json` & `tq42-0.5.25/tq42/utils/text_files/help_flags.json`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/utils/text_files/tq42_commands.txt` & `tq42-0.5.25/tq42/utils/text_files/tq42_commands.txt`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/utils/token_manager.py` & `tq42-0.5.25/tq42/utils/token_manager.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/utils/utils.py` & `tq42-0.5.25/tq42/utils/utils.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/tq42/utils/utils_for_cache.py` & `tq42-0.5.25/tq42/utils/utils_for_cache.py`

 * *Files identical despite different names*

### Comparing `tq42-0.5.24/PKG-INFO` & `tq42-0.5.25/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: tq42
-Version: 0.5.24
+Version: 0.5.25
 Summary: tq42 sdk
 Author: Terra Quantum AG
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: PyYAML (>=6.0.1,<7.0.0)
 Requires-Dist: keyring (>=25.0.0,<26.0.0)
 Requires-Dist: pytest (>=7.4.4,<8.0.0)
 Requires-Dist: requests (==2.31.0)
-Requires-Dist: tq42_grpc_client (==1.0.112)
+Requires-Dist: tq42_grpc_client (==1.0.120)
 Description-Content-Type: text/markdown
 
 ![](images/TQ42_Logo_Black_Teal.svg)
 
 # Introduction to TQ42
 The TQ42 Python SDK puts the power in your hands to accelerate delivery of custom, high-impact solutions. After installing the SDK and authenticating, access algorithms such as TetraOpt – a global optimization library based on tensor train (TT) decomposition.
```

