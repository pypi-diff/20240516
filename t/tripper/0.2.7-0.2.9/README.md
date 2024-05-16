# Comparing `tmp/tripper-0.2.7.tar.gz` & `tmp/tripper-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tripper-0.2.7.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "tripper-0.2.9.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `tripper-0.2.7.tar` & `tripper-0.2.9.tar`

### file list

```diff
@@ -1,80 +1,80 @@
--rw-r--r--   0        0        0      205 2023-08-29 12:28:01.230424 tripper-0.2.7/.github/dependabot.yml
--rw-r--r--   0        0        0      652 2023-08-29 12:28:01.230424 tripper-0.2.7/.github/pull_request_template.md
--rw-r--r--   0        0        0      918 2023-08-29 12:28:01.230424 tripper-0.2.7/.github/workflows/cd_release.yml
--rw-r--r--   0        0        0      545 2023-08-29 12:28:01.230424 tripper-0.2.7/.github/workflows/ci_automerge_dependency_prs.yml
--rw-r--r--   0        0        0      662 2023-08-29 12:28:01.230424 tripper-0.2.7/.github/workflows/ci_cd_updated_main.yml
--rw-r--r--   0        0        0      602 2023-08-29 12:28:01.230424 tripper-0.2.7/.github/workflows/ci_check_dependencies.yml
--rw-r--r--   0        0        0     2430 2023-08-29 12:28:01.230424 tripper-0.2.7/.github/workflows/ci_tests.yml
--rw-r--r--   0        0        0      840 2023-08-29 12:28:01.230424 tripper-0.2.7/.github/workflows/ci_update_dependencies.yml
--rw-r--r--   0        0        0      137 2023-08-29 12:28:01.230424 tripper-0.2.7/.gitignore
--rw-r--r--   0        0        0     1819 2023-08-29 12:28:01.230424 tripper-0.2.7/.pre-commit-config.yaml
--rw-r--r--   0        0        0    12143 2023-08-29 12:29:08.311543 tripper-0.2.7/CHANGELOG.md
--rw-r--r--   0        0        0     1063 2023-08-29 12:28:01.234424 tripper-0.2.7/LICENSE
--rw-r--r--   0        0        0     2593 2023-08-29 12:28:01.234424 tripper-0.2.7/README.md
-lrwxr-xr-x   0        0        0        0 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/CHANGELOG.md -> ../CHANGELOG.md
-lrwxr-xr-x   0        0        0        0 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/LICENSE.md -> ../LICENSE
--rw-r--r--   0        0        0       23 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/.pages
--rw-r--r--   0        0        0       18 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/backends/.pages
--rw-r--r--   0        0        0       46 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/backends/collection.md
--rw-r--r--   0        0        0       38 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/backends/ontopy.md
--rw-r--r--   0        0        0       38 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/backends/rdflib.md
--rw-r--r--   0        0        0       52 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/backends/sparqlwrapper.md
--rw-r--r--   0        0        0       17 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/convert/.pages
--rw-r--r--   0        0        0       39 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/convert/convert.md
--rw-r--r--   0        0        0       29 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/errors.md
--rw-r--r--   0        0        0       35 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/interface.md
--rw-r--r--   0        0        0       31 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/literal.md
--rw-r--r--   0        0        0       18 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/mappings/.pages
--rw-r--r--   0        0        0       42 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/mappings/mappings.md
--rw-r--r--   0        0        0       35 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/namespace.md
--rw-r--r--   0        0        0       39 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/triplestore.md
--rw-r--r--   0        0        0       31 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/tripper.md
--rw-r--r--   0        0        0       27 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/api_reference/utils.md
--rw-r--r--   0        0        0     2909 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/backend_discovery.md
--rw-r--r--   0        0        0      183 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/css/reference.css
--rw-r--r--   0        0        0     2586 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/index.md
--rw-r--r--   0        0        0    12710 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/mappings/figs/function_emmo.svg
--rw-r--r--   0        0        0      228 2023-08-29 12:28:01.234424 tripper-0.2.7/docs/planned-backends.md
--rw-r--r--   0        0        0     3963 2023-08-29 12:28:01.238424 tripper-0.2.7/docs/tutorial.md
--rw-r--r--   0        0        0     1190 2023-08-29 12:28:01.238424 tripper-0.2.7/examples/workflow-mappings/README.md
--rw-r--r--   0        0        0    18333 2023-08-29 12:28:01.238424 tripper-0.2.7/examples/workflow-mappings/knowledge-base.svg
--rw-r--r--   0        0        0     8546 2023-08-29 12:28:01.238424 tripper-0.2.7/examples/workflow-mappings/route.svg
--rw-r--r--   0        0        0     7117 2023-08-29 12:28:01.238424 tripper-0.2.7/examples/workflow-mappings/workflow.svg
--rw-r--r--   0        0        0      894 2023-08-29 12:28:01.238424 tripper-0.2.7/examples/workflow-mappings/workflow_mappings.py
--rw-r--r--   0        0        0    14169 2023-08-29 12:28:01.238424 tripper-0.2.7/examples/workflow-mappings/workflow_w_pipes.svg
--rw-r--r--   0        0        0     1943 2023-08-29 12:28:01.238424 tripper-0.2.7/mkdocs.yml
--rw-r--r--   0        0        0     2887 2023-08-29 12:28:01.238424 tripper-0.2.7/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/backends/__init__.py
--rw-r--r--   0        0        0      542 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/backends/dummy.py
--rw-r--r--   0        0        0     3480 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/conftest.py
--rw-r--r--   0        0        0     1393 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/convert/test_convert.py
--rw-r--r--   0        0        0      951 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/mappings/test_function.py
--rw-r--r--   0        0        0     1461 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/mappings/test_mappings.py
--rw-r--r--   0        0        0     5701 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/ontologies/family.ttl
--rw-r--r--   0        0        0     6753 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/ontologies/food.ttl
--rw-r--r--   0        0        0     3166 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/test_add_function.py
--rw-r--r--   0        0        0      880 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/test_collection.py
--rw-r--r--   0        0        0      241 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/test_custom_backend.py
--rw-r--r--   0        0        0     2455 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/test_get_data.py
--rw-r--r--   0        0        0     4494 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/test_literals.py
--rw-r--r--   0        0        0     1993 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/test_namespace.py
--rw-r--r--   0        0        0     7895 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/test_triplestore.py
--rw-r--r--   0        0        0     6168 2023-08-29 12:28:01.238424 tripper-0.2.7/tests/test_utils.py
--rw-r--r--   0        0        0      796 2023-08-29 12:29:08.867552 tripper-0.2.7/tripper/__init__.py
--rw-r--r--   0        0        0     1330 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/backends/__init__.py
--rw-r--r--   0        0        0     2523 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/backends/collection.py
--rw-r--r--   0        0        0     9177 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/backends/ontopy.py
--rw-r--r--   0        0        0     7381 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/backends/rdflib.py
--rw-r--r--   0        0        0     4144 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/backends/sparqlwrapper.py
--rw-r--r--   0        0        0      195 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/convert/__init__.py
--rw-r--r--   0        0        0     7078 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/convert/convert.py
--rw-r--r--   0        0        0      362 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/errors.py
--rw-r--r--   0        0        0     5401 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/interface.py
--rw-r--r--   0        0        0     5671 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/literal.py
--rw-r--r--   0        0        0      102 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/mappings/__init__.py
--rw-r--r--   0        0        0    35786 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/mappings/mappings.py
--rw-r--r--   0        0        0     6995 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/namespace.py
--rw-r--r--   0        0        0    32618 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/triplestore.py
--rw-r--r--   0        0        0    10977 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/tripper.py
--rw-r--r--   0        0        0     8553 2023-08-29 12:28:01.238424 tripper-0.2.7/tripper/utils.py
--rw-r--r--   0        0        0     5506 1970-01-01 00:00:00.000000 tripper-0.2.7/PKG-INFO
+-rw-r--r--   0        0        0      205 2023-09-29 17:37:35.931714 tripper-0.2.9/.github/dependabot.yml
+-rw-r--r--   0        0        0      652 2023-09-29 17:37:35.931714 tripper-0.2.9/.github/pull_request_template.md
+-rw-r--r--   0        0        0      918 2023-09-29 17:37:35.931714 tripper-0.2.9/.github/workflows/cd_release.yml
+-rw-r--r--   0        0        0      545 2023-09-29 17:37:35.931714 tripper-0.2.9/.github/workflows/ci_automerge_dependency_prs.yml
+-rw-r--r--   0        0        0      662 2023-09-29 17:37:35.931714 tripper-0.2.9/.github/workflows/ci_cd_updated_main.yml
+-rw-r--r--   0        0        0      602 2023-09-29 17:37:35.931714 tripper-0.2.9/.github/workflows/ci_check_dependencies.yml
+-rw-r--r--   0        0        0     2430 2023-09-29 17:37:35.931714 tripper-0.2.9/.github/workflows/ci_tests.yml
+-rw-r--r--   0        0        0      840 2023-09-29 17:37:35.931714 tripper-0.2.9/.github/workflows/ci_update_dependencies.yml
+-rw-r--r--   0        0        0      137 2023-09-29 17:37:35.931714 tripper-0.2.9/.gitignore
+-rw-r--r--   0        0        0     1819 2023-09-29 17:37:35.931714 tripper-0.2.9/.pre-commit-config.yaml
+-rw-r--r--   0        0        0    12633 2023-09-29 17:38:30.831743 tripper-0.2.9/CHANGELOG.md
+-rw-r--r--   0        0        0     1063 2023-09-29 17:37:35.935714 tripper-0.2.9/LICENSE
+-rw-r--r--   0        0        0     2593 2023-09-29 17:37:35.935714 tripper-0.2.9/README.md
+lrwxr-xr-x   0        0        0        0 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/CHANGELOG.md -> ../CHANGELOG.md
+lrwxr-xr-x   0        0        0        0 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/LICENSE.md -> ../LICENSE
+-rw-r--r--   0        0        0       23 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/.pages
+-rw-r--r--   0        0        0       18 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/backends/.pages
+-rw-r--r--   0        0        0       46 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/backends/collection.md
+-rw-r--r--   0        0        0       38 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/backends/ontopy.md
+-rw-r--r--   0        0        0       38 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/backends/rdflib.md
+-rw-r--r--   0        0        0       52 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/backends/sparqlwrapper.md
+-rw-r--r--   0        0        0       17 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/convert/.pages
+-rw-r--r--   0        0        0       39 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/convert/convert.md
+-rw-r--r--   0        0        0       29 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/errors.md
+-rw-r--r--   0        0        0       35 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/interface.md
+-rw-r--r--   0        0        0       31 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/literal.md
+-rw-r--r--   0        0        0       18 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/mappings/.pages
+-rw-r--r--   0        0        0       42 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/mappings/mappings.md
+-rw-r--r--   0        0        0       35 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/namespace.md
+-rw-r--r--   0        0        0       39 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/triplestore.md
+-rw-r--r--   0        0        0       31 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/tripper.md
+-rw-r--r--   0        0        0       27 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/api_reference/utils.md
+-rw-r--r--   0        0        0     2909 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/backend_discovery.md
+-rw-r--r--   0        0        0      183 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/css/reference.css
+-rw-r--r--   0        0        0     2586 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/index.md
+-rw-r--r--   0        0        0    12710 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/mappings/figs/function_emmo.svg
+-rw-r--r--   0        0        0      228 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/planned-backends.md
+-rw-r--r--   0        0        0     3963 2023-09-29 17:37:35.935714 tripper-0.2.9/docs/tutorial.md
+-rw-r--r--   0        0        0     1190 2023-09-29 17:37:35.935714 tripper-0.2.9/examples/workflow-mappings/README.md
+-rw-r--r--   0        0        0    18333 2023-09-29 17:37:35.935714 tripper-0.2.9/examples/workflow-mappings/knowledge-base.svg
+-rw-r--r--   0        0        0     8546 2023-09-29 17:37:35.935714 tripper-0.2.9/examples/workflow-mappings/route.svg
+-rw-r--r--   0        0        0     7117 2023-09-29 17:37:35.935714 tripper-0.2.9/examples/workflow-mappings/workflow.svg
+-rw-r--r--   0        0        0      894 2023-09-29 17:37:35.935714 tripper-0.2.9/examples/workflow-mappings/workflow_mappings.py
+-rw-r--r--   0        0        0    14169 2023-09-29 17:37:35.935714 tripper-0.2.9/examples/workflow-mappings/workflow_w_pipes.svg
+-rw-r--r--   0        0        0     1943 2023-09-29 17:37:35.935714 tripper-0.2.9/mkdocs.yml
+-rw-r--r--   0        0        0     2909 2023-09-29 17:37:35.935714 tripper-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/backends/__init__.py
+-rw-r--r--   0        0        0      542 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/backends/dummy.py
+-rw-r--r--   0        0        0     3480 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/conftest.py
+-rw-r--r--   0        0        0     1436 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/convert/test_convert.py
+-rw-r--r--   0        0        0      951 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/mappings/test_function.py
+-rw-r--r--   0        0        0     1461 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/mappings/test_mappings.py
+-rw-r--r--   0        0        0     5701 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/ontologies/family.ttl
+-rw-r--r--   0        0        0     6753 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/ontologies/food.ttl
+-rw-r--r--   0        0        0     3166 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/test_add_function.py
+-rw-r--r--   0        0        0      880 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/test_collection.py
+-rw-r--r--   0        0        0      241 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/test_custom_backend.py
+-rw-r--r--   0        0        0     2455 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/test_get_data.py
+-rw-r--r--   0        0        0     4653 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/test_literals.py
+-rw-r--r--   0        0        0     1993 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/test_namespace.py
+-rw-r--r--   0        0        0     7891 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/test_triplestore.py
+-rw-r--r--   0        0        0     6168 2023-09-29 17:37:35.935714 tripper-0.2.9/tests/test_utils.py
+-rw-r--r--   0        0        0      796 2023-09-29 17:38:31.335743 tripper-0.2.9/tripper/__init__.py
+-rw-r--r--   0        0        0     1330 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/backends/__init__.py
+-rw-r--r--   0        0        0     2523 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/backends/collection.py
+-rw-r--r--   0        0        0     9177 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/backends/ontopy.py
+-rw-r--r--   0        0        0     7381 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/backends/rdflib.py
+-rw-r--r--   0        0        0     4144 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/backends/sparqlwrapper.py
+-rw-r--r--   0        0        0      287 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/convert/__init__.py
+-rw-r--r--   0        0        0    13078 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/convert/convert.py
+-rw-r--r--   0        0        0      362 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/errors.py
+-rw-r--r--   0        0        0     5401 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/interface.py
+-rw-r--r--   0        0        0     5671 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/literal.py
+-rw-r--r--   0        0        0      102 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/mappings/__init__.py
+-rw-r--r--   0        0        0    35786 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/mappings/mappings.py
+-rw-r--r--   0        0        0     6995 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/namespace.py
+-rw-r--r--   0        0        0    32618 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/triplestore.py
+-rw-r--r--   0        0        0    10977 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/tripper.py
+-rw-r--r--   0        0        0     8894 2023-09-29 17:37:35.939714 tripper-0.2.9/tripper/utils.py
+-rw-r--r--   0        0        0     5557 1970-01-01 00:00:00.000000 tripper-0.2.9/PKG-INFO
```

### Comparing `tripper-0.2.7/.github/pull_request_template.md` & `tripper-0.2.9/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/.github/workflows/cd_release.yml` & `tripper-0.2.9/.github/workflows/cd_release.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/.github/workflows/ci_automerge_dependency_prs.yml` & `tripper-0.2.9/.github/workflows/ci_automerge_dependency_prs.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/.github/workflows/ci_cd_updated_main.yml` & `tripper-0.2.9/.github/workflows/ci_cd_updated_main.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/.github/workflows/ci_check_dependencies.yml` & `tripper-0.2.9/.github/workflows/ci_check_dependencies.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/.github/workflows/ci_tests.yml` & `tripper-0.2.9/.github/workflows/ci_tests.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/.github/workflows/ci_update_dependencies.yml` & `tripper-0.2.9/.github/workflows/ci_update_dependencies.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/.pre-commit-config.yaml` & `tripper-0.2.9/.pre-commit-config.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     - id: mypy
       exclude: ^tests/.*$
       additional_dependencies:
         - "types-requests"
         - "pydantic"
 
   - repo: https://github.com/SINTEF/ci-cd
-    rev: v2.4.0
+    rev: v2.5.1
     hooks:
     - id: docs-api-reference
       args:
       - --package-dir=tripper
     - id: docs-landing-page
 
   - repo: local
```

### Comparing `tripper-0.2.7/CHANGELOG.md` & `tripper-0.2.9/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,22 @@
 # Changelog
 
-## [v0.2.7](https://github.com/EMMC-ASBL/tripper/tree/v0.2.7) (2023-08-28)
+## [v0.2.9](https://github.com/EMMC-ASBL/tripper/tree/v0.2.9) (2023-09-29)
+
+[Full Changelog](https://github.com/EMMC-ASBL/tripper/compare/v0.2.8...v0.2.9)
+
+## [v0.2.8](https://github.com/EMMC-ASBL/tripper/tree/v0.2.8) (2023-09-12)
+
+[Full Changelog](https://github.com/EMMC-ASBL/tripper/compare/v0.2.7...v0.2.8)
+
+**Merged pull requests:**
+
+- Added support for lists in tripper.convert [\#129](https://github.com/EMMC-ASBL/tripper/pull/129) ([jesper-friis](https://github.com/jesper-friis))
+
+## [v0.2.7](https://github.com/EMMC-ASBL/tripper/tree/v0.2.7) (2023-08-29)
 
 [Full Changelog](https://github.com/EMMC-ASBL/tripper/compare/v0.2.6...v0.2.7)
 
 **Fixed bugs:**
 
 - Fix issues related to renaming of the default branch [\#116](https://github.com/EMMC-ASBL/tripper/issues/116)
```

### Comparing `tripper-0.2.7/LICENSE` & `tripper-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/README.md` & `tripper-0.2.9/README.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/docs/backend_discovery.md` & `tripper-0.2.9/docs/backend_discovery.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/docs/index.md` & `tripper-0.2.9/docs/index.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/docs/mappings/figs/function_emmo.svg` & `tripper-0.2.9/docs/mappings/figs/function_emmo.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/docs/tutorial.md` & `tripper-0.2.9/docs/tutorial.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/examples/workflow-mappings/README.md` & `tripper-0.2.9/examples/workflow-mappings/README.md`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/examples/workflow-mappings/knowledge-base.svg` & `tripper-0.2.9/examples/workflow-mappings/knowledge-base.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/examples/workflow-mappings/route.svg` & `tripper-0.2.9/examples/workflow-mappings/route.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/examples/workflow-mappings/workflow.svg` & `tripper-0.2.9/examples/workflow-mappings/workflow.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/examples/workflow-mappings/workflow_mappings.py` & `tripper-0.2.9/examples/workflow-mappings/workflow_mappings.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/examples/workflow-mappings/workflow_w_pipes.svg` & `tripper-0.2.9/examples/workflow-mappings/workflow_w_pipes.svg`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/mkdocs.yml` & `tripper-0.2.9/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/pyproject.toml` & `tripper-0.2.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -25,55 +25,56 @@
 ]
 keywords = ["triplestore", "ontology", "RDF"]
 requires-python = "~=3.7"
 dynamic = ["version"]
 
 dependencies = [
     "typing-extensions ~=4.7; python_version<'3.8'",
-    "pint ~=0.2",
+    "pint ~=0.18",
 ]
 
 [project.optional-dependencies]
 docs = [
     "mike ~=1.1",
     "mkdocs ~=1.5",
     "mkdocs-awesome-pages-plugin ~=2.9",
-    "mkdocs-material ~=9.1",
+    "mkdocs-material ~=9.2",
     "mkdocstrings[python-legacy] ~=0.22.0",
     "EMMOntoPy ~=0.6",
     "rdflib ~=6.3",
     "SPARQLWrapper ~=2.0",
-    "DLite-Python >=0.3.22,<1",
+    "DLite-Python >=0.4.0,<1",
 ]
 pre-commit = [
     "pre-commit ~=2.21",
     "pylint ~=2.13",
 ]
 testing = [
     "pytest ~=7.4",
     "pytest-cov ~=4.1",
     "EMMOntoPy ~=0.6",
     "rdflib ~=6.3",
     "SPARQLWrapper ~=2.0",
-    "DLite-Python >=0.3.22,<1",
+    "DLite-Python >=0.4.0,<1",
+    "graphviz ~= 0.20",
 ]
 dev = [
     "mike ~=1.1",
     "mkdocs ~=1.5",
     "mkdocs-awesome-pages-plugin ~=2.9",
-    "mkdocs-material ~=9.1",
+    "mkdocs-material ~=9.2",
     "mkdocstrings[python-legacy] ~=0.22.0",
     "pre-commit ~=2.21",
     "pylint ~=2.13",
     "pytest ~=7.4",
     "pytest-cov ~=4.1",
     "EMMOntoPy ~=0.6",
     "rdflib ~=6.3",
     "SPARQLWrapper ~=2.0",
-    "DLite-Python >=0.3.22,<1",
+    "DLite-Python >=0.4.0,<1",
 ]
 
 [project.urls]
 Home = "https://github.com/EMMC-ASBL/tripper"
 Documentation = "https://EMMC-ASBL.github.io/tripper"
 Source = "https://github.com/EMMC-ASBL/tripper"
 "Issue Tracker" = "https://github.com/EMMC-ASBL/tripper/issues"
```

### Comparing `tripper-0.2.7/tests/backends/dummy.py` & `tripper-0.2.9/tests/backends/dummy.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tests/conftest.py` & `tripper-0.2.9/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tests/convert/test_convert.py` & `tripper-0.2.9/tests/convert/test_convert.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Test convertions."""
 # pylint: disable=invalid-name
 from tripper import Triplestore
-from tripper.convert import load_dict, save_dict
+from tripper.convert import load_container, save_container
 
 ts = Triplestore(backend="rdflib")
 EX = ts.bind("ex", "http://example.com/ex#")
 
 
 config1 = {
     "downloadUrl": "http://example.com/somedata.txt",
@@ -19,36 +19,37 @@
     "anotherField": "More info...",
     "configurations": {
         "key1": "val1",
         "key2": 2,
         "key3": 3.14,
         "key4": None,
         "key5": True,
-        # "key6": ["a", 1, 2.2, None],  # lists are not supported yet...
+        "key6": False,
+        "key7": ["a", 1, 2.2, True, None],
     },
 }
 
 # Store dictionaries to triplestore
-save_dict(ts, config1, EX.config1)
-save_dict(ts, config2, EX.config2)
+save_container(ts, config1, EX.config1)
+save_container(ts, config2, EX.config2)
 
 # Print content of triplestore
 # print(ts.serialize())
 
 # Load dictionaries from triplestore
-d1 = load_dict(ts, EX.config1)
-d2 = load_dict(ts, EX.config2)
+d1 = load_container(ts, EX.config1)
+d2 = load_container(ts, EX.config2)
 
 # Check that we got back what we stored
 assert d1 == config1
 assert d2 == config2
 
 
 # Now, test serialising using recognised_keys
-save_dict(ts, config1, EX.config1b, recognised_keys="basic")
-save_dict(ts, config2, EX.config2b, recognised_keys="basic")
+save_container(ts, config1, EX.config1b, recognised_keys="basic")
+save_container(ts, config2, EX.config2b, recognised_keys="basic")
 
-d1b = load_dict(ts, EX.config1b, recognised_keys="basic")
-d2b = load_dict(ts, EX.config2b, recognised_keys="basic")
+d1b = load_container(ts, EX.config1b, recognised_keys="basic")
+d2b = load_container(ts, EX.config2b, recognised_keys="basic")
 
 assert d1b == config1
 assert d2b == config2
```

### Comparing `tripper-0.2.7/tests/mappings/test_function.py` & `tripper-0.2.9/tests/mappings/test_function.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tests/mappings/test_mappings.py` & `tripper-0.2.9/tests/mappings/test_mappings.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tests/ontologies/family.ttl` & `tripper-0.2.9/tests/ontologies/family.ttl`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tests/ontologies/food.ttl` & `tripper-0.2.9/tests/ontologies/food.ttl`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tests/test_add_function.py` & `tripper-0.2.9/tests/test_add_function.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tests/test_collection.py` & `tripper-0.2.9/tests/test_collection.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tests/test_get_data.py` & `tripper-0.2.9/tests/test_get_data.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tests/test_literals.py` & `tripper-0.2.9/tests/test_literals.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,14 +99,19 @@
     assert literal.datatype == XSD.double
 
     literal = parse_literal(Literal(True).n3())
     assert literal.value is True
     assert literal.lang is None
     assert literal.datatype == XSD.boolean
 
+    literal = parse_literal(Literal(False).n3())
+    assert literal.value is False
+    assert literal.lang is None
+    assert literal.datatype == XSD.boolean
+
     dt = datetime(2022, 10, 23)
     literal = parse_literal(Literal(dt).n3())
     assert literal.value == dt
     assert literal.lang is None
     assert literal.datatype == XSD.dateTime
 
     literal = parse_literal(dt)
```

### Comparing `tripper-0.2.7/tests/test_namespace.py` & `tripper-0.2.9/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tests/test_triplestore.py` & `tripper-0.2.9/tests/test_triplestore.py`

 * *Files 2% similar despite different names*

```diff
@@ -84,18 +84,17 @@
         assert rows[2] == (
             "http://example.com/onto#Sum",
             "http://www.w3.org/2002/07/owl#Thing",
         )
 
     # Test value() method
     assert ts.value(func_iri, DCTERMS.description) == example_function.__doc__
-    assert (
-        ts.value(func_iri, DCTERMS.description, lang="en")
-        == example_function.__doc__
-    )
+    # assert ts.value(
+    #     func_iri, DCTERMS.description, lang="en"
+    # ) == example_function.__doc__
     assert ts.value(func_iri, DCTERMS.description, lang="de") is None
 
 
 def test_backend_rdflib(expected_function_triplestore: str) -> None:
     """Specifically test the rdflib backend Triplestore.
 
     Parameters:
```

### Comparing `tripper-0.2.7/tests/test_utils.py` & `tripper-0.2.9/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tripper/__init__.py` & `tripper-0.2.9/tripper/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
     XML,
     XSD,
     Namespace,
 )
 from .triplestore import Triplestore, backend_packages
 from .tripper import Tripper
 
-__version__ = "0.2.7"
+__version__ = "0.2.9"
 
 __all__ = (
     "Literal",
     #
     "DCAT",
     "DC",
     "DCTERMS",
```

### Comparing `tripper-0.2.7/tripper/backends/__init__.py` & `tripper-0.2.9/tripper/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tripper/backends/collection.py` & `tripper-0.2.9/tripper/backends/collection.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tripper/backends/ontopy.py` & `tripper-0.2.9/tripper/backends/ontopy.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tripper/backends/rdflib.py` & `tripper-0.2.9/tripper/backends/rdflib.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tripper/backends/sparqlwrapper.py` & `tripper-0.2.9/tripper/backends/sparqlwrapper.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tripper/interface.py` & `tripper-0.2.9/tripper/interface.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tripper/literal.py` & `tripper-0.2.9/tripper/literal.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tripper/mappings/mappings.py` & `tripper-0.2.9/tripper/mappings/mappings.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tripper/namespace.py` & `tripper-0.2.9/tripper/namespace.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tripper/triplestore.py` & `tripper-0.2.9/tripper/triplestore.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tripper/tripper.py` & `tripper-0.2.9/tripper/tripper.py`

 * *Files identical despite different names*

### Comparing `tripper-0.2.7/tripper/utils.py` & `tripper-0.2.9/tripper/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -111,25 +111,30 @@
 
     Equivalent to ``Literal(value, lang="en")``.
     """
     return Literal(value, lang="en")
 
 
 def parse_literal(literal: "Any") -> "Literal":
-    """Parse `literal` and return it as an instance of Literal.
+    """Parse Python object `literal` and return it as an instance of Literal.
 
     The main difference between this function and the Literal constructor,
     is that this function correctly interprets n3-encoded literal strings.
     """
-    # pylint: disable=invalid-name,too-many-branches
+    # pylint: disable=invalid-name,too-many-branches,too-many-return-statements
     lang, datatype = None, None
 
     if isinstance(literal, Literal):
         return literal
 
+    # This will handle rdflib literals correctly and probably most other
+    # literal representations as well.
+    if hasattr(literal, "value"):
+        return Literal(literal.value)
+
     if not isinstance(literal, str):
         if isinstance(literal, tuple(Literal.datatypes)):
             return Literal(
                 literal,
                 lang=lang,
                 datatype=Literal.datatypes.get(type(literal))[
                     0
@@ -166,14 +171,16 @@
 
     if lang or datatype:
         if datatype:
             types = {}
             for pytype, datatypes in Literal.datatypes.items():
                 types.update({t: pytype for t in datatypes})
             type_ = types.get(datatype, str)
+            if type_ is bool and value in ("False", "false", "0", 0, False):
+                return Literal(False)
             try:
                 value = type_(value)
             except TypeError:
                 pass
         return Literal(value, lang=lang, datatype=datatype)
 
     for type_, datatypes in Literal.datatypes.items():
```

### Comparing `tripper-0.2.7/PKG-INFO` & `tripper-0.2.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tripper
-Version: 0.2.7
+Version: 0.2.9
 Summary: A triplestore wrapper for Python.
 Keywords: triplestore,ontology,RDF
 Author-email: SINTEF <TEAM4.0@sintef.no>
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: License :: OSI Approved :: MIT License
@@ -14,45 +14,46 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Environment :: Plugins
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Requires-Dist: typing-extensions ~=4.7; python_version<'3.8'
-Requires-Dist: pint ~=0.2
+Requires-Dist: pint ~=0.18
 Requires-Dist: mike ~=1.1 ; extra == "dev"
 Requires-Dist: mkdocs ~=1.5 ; extra == "dev"
 Requires-Dist: mkdocs-awesome-pages-plugin ~=2.9 ; extra == "dev"
-Requires-Dist: mkdocs-material ~=9.1 ; extra == "dev"
+Requires-Dist: mkdocs-material ~=9.2 ; extra == "dev"
 Requires-Dist: mkdocstrings[python-legacy] ~=0.22.0 ; extra == "dev"
 Requires-Dist: pre-commit ~=2.21 ; extra == "dev"
 Requires-Dist: pylint ~=2.13 ; extra == "dev"
 Requires-Dist: pytest ~=7.4 ; extra == "dev"
 Requires-Dist: pytest-cov ~=4.1 ; extra == "dev"
 Requires-Dist: EMMOntoPy ~=0.6 ; extra == "dev"
 Requires-Dist: rdflib ~=6.3 ; extra == "dev"
 Requires-Dist: SPARQLWrapper ~=2.0 ; extra == "dev"
-Requires-Dist: DLite-Python >=0.3.22,<1 ; extra == "dev"
+Requires-Dist: DLite-Python >=0.4.0,<1 ; extra == "dev"
 Requires-Dist: mike ~=1.1 ; extra == "docs"
 Requires-Dist: mkdocs ~=1.5 ; extra == "docs"
 Requires-Dist: mkdocs-awesome-pages-plugin ~=2.9 ; extra == "docs"
-Requires-Dist: mkdocs-material ~=9.1 ; extra == "docs"
+Requires-Dist: mkdocs-material ~=9.2 ; extra == "docs"
 Requires-Dist: mkdocstrings[python-legacy] ~=0.22.0 ; extra == "docs"
 Requires-Dist: EMMOntoPy ~=0.6 ; extra == "docs"
 Requires-Dist: rdflib ~=6.3 ; extra == "docs"
 Requires-Dist: SPARQLWrapper ~=2.0 ; extra == "docs"
-Requires-Dist: DLite-Python >=0.3.22,<1 ; extra == "docs"
+Requires-Dist: DLite-Python >=0.4.0,<1 ; extra == "docs"
 Requires-Dist: pre-commit ~=2.21 ; extra == "pre-commit"
 Requires-Dist: pylint ~=2.13 ; extra == "pre-commit"
 Requires-Dist: pytest ~=7.4 ; extra == "testing"
 Requires-Dist: pytest-cov ~=4.1 ; extra == "testing"
 Requires-Dist: EMMOntoPy ~=0.6 ; extra == "testing"
 Requires-Dist: rdflib ~=6.3 ; extra == "testing"
 Requires-Dist: SPARQLWrapper ~=2.0 ; extra == "testing"
-Requires-Dist: DLite-Python >=0.3.22,<1 ; extra == "testing"
+Requires-Dist: DLite-Python >=0.4.0,<1 ; extra == "testing"
+Requires-Dist: graphviz ~= 0.20 ; extra == "testing"
 Project-URL: Changelog, https://github.com/EMMC-ASBL/tripper/blob/master/CHANGELOG.md
 Project-URL: Documentation, https://EMMC-ASBL.github.io/tripper
 Project-URL: Home, https://github.com/EMMC-ASBL/tripper
 Project-URL: Issue Tracker, https://github.com/EMMC-ASBL/tripper/issues
 Project-URL: Package, https://pypi.org/project/tripper
 Project-URL: Source, https://github.com/EMMC-ASBL/tripper
 Provides-Extra: dev
```

