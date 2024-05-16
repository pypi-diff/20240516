# Comparing `tmp/dagster-cloud-cli-1.7.5.tar.gz` & `tmp/dagster-cloud-cli-1.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-cloud-cli-1.7.5.tar", last modified: Thu May  9 17:58:34 2024, max compression
+gzip compressed data, was "dagster-cloud-cli-1.7.6.tar", last modified: Thu May 16 20:18:34 2024, max compression
```

## Comparing `dagster-cloud-cli-1.7.5.tar` & `dagster-cloud-cli-1.7.6.tar`

### file list

```diff
@@ -1,94 +1,94 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.728206 dagster-cloud-cli-1.7.5/
--rw-r--r--   0 root         (0) root         (0)      132 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      314 2024-05-09 17:58:34.728206 dagster-cloud-cli-1.7.5/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.688206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/
--rw-r--r--   0 root         (0) root         (0)      160 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.688206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.688206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/branch_deployment/
--rw-r--r--   0 root         (0) root         (0)     5173 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/branch_deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.692206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/
--rw-r--r--   0 root         (0) root         (0)    30031 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4124 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/checks.py
--rw-r--r--   0 root         (0) root         (0)     1872 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/report.py
--rw-r--r--   0 root         (0) root         (0)     4121 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/state.py
--rw-r--r--   0 root         (0) root         (0)      550 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/utils.py
--rw-r--r--   0 root         (0) root         (0)     8651 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.700206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/
--rw-r--r--   0 root         (0) root         (0)     3098 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.700206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/alert_policies/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1803 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
--rw-r--r--   0 root         (0) root         (0)    17101 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.700206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/job/
--rw-r--r--   0 root         (0) root         (0)     1985 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/job/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4425 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/metrics.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.700206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/organization/
--rw-r--r--   0 root         (0) root         (0)     4001 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.700206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/organization/saml/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/organization/saml/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2691 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/organization/saml/commands.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.700206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/run/
--rw-r--r--   0 root         (0) root         (0)      757 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/run/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.704206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/serverless/
--rw-r--r--   0 root         (0) root         (0)     1499 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/serverless/Dockerfile
--rw-r--r--   0 root         (0) root         (0)      628 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
--rw-r--r--   0 root         (0) root         (0)    18458 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/serverless/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.704206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/workspace/
--rw-r--r--   0 root         (0) root         (0)    12788 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/workspace/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18301 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/config_utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.712206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/__init__.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/agent_queue.py
--rw-r--r--   0 root         (0) root         (0)      901 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/alert_types.py
--rw-r--r--   0 root         (0) root         (0)     4801 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/artifacts.py
--rw-r--r--   0 root         (0) root         (0)     1744 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/docker_runner.py
--rw-r--r--   0 root         (0) root         (0)     1131 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/errors.py
--rw-r--r--   0 root         (0) root         (0)    13801 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/graphql_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.712206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/__init__.py
--rw-r--r--   0 root         (0) root         (0)      376 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/auth.py
--rw-r--r--   0 root         (0) root         (0)      924 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/impl.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.716206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/versioning/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/versioning/__init__.py
--rw-r--r--   0 root         (0) root         (0)       96 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/versioning/constants.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.720206 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/
--rw-r--r--   0 root         (0) root         (0)      172 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1680 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/code_location.py
--rw-r--r--   0 root         (0) root         (0)     9423 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/deploy.py
--rw-r--r--   0 root         (0) root         (0)    14436 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/deps.py
--rw-r--r--   0 root         (0) root         (0)      949 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/git_context.py
--rw-r--r--   0 root         (0) root         (0)     6992 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/github_context.py
--rw-r--r--   0 root         (0) root         (0)     1063 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/gitlab_context.py
--rw-r--r--   0 root         (0) root         (0)     1232 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/parse_workspace.py
--rw-r--r--   0 root         (0) root         (0)     4655 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/pex_registry.py
--rw-r--r--   0 root         (0) root         (0)      709 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/selftest.py
--rw-r--r--   0 root         (0) root         (0)     5407 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/source.py
--rw-r--r--   0 root         (0) root         (0)     6220 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/util.py
--rw-r--r--   0 root         (0) root         (0)     2106 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pydantic_yaml.py
--rw-r--r--   0 root         (0) root         (0)     8034 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/workspace.py
--rw-r--r--   0 root         (0) root         (0)     2463 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/docker_utils.py
--rw-r--r--   0 root         (0) root         (0)     6708 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/entrypoint.py
--rw-r--r--   0 root         (0) root         (0)    20800 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/gql.py
--rw-r--r--   0 root         (0) root         (0)     5859 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/pex_utils.py
--rw-r--r--   0 root         (0) root         (0)     1845 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/types.py
--rw-r--r--   0 root         (0) root         (0)     2804 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/ui.py
--rw-r--r--   0 root         (0) root         (0)     3488 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/utils.py
--rw-r--r--   0 root         (0) root         (0)       22 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.688206 dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/
--rw-r--r--   0 root         (0) root         (0)      314 2024-05-09 17:58:34.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3066 2024-05-09 17:58:34.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-09 17:58:34.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       67 2024-05-09 17:58:34.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      112 2024-05-09 17:58:34.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       42 2024-05-09 17:58:34.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-09 17:58:34.728206 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/
--rw-r--r--   0 root         (0) root         (0)        0 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/__init__.py
--rw-r--r--   0 root         (0) root         (0)      189 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/conftest.py
--rw-r--r--   0 root         (0) root         (0)     4130 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_check.py
--rw-r--r--   0 root         (0) root         (0)    16177 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_ci_commands.py
--rw-r--r--   0 root         (0) root         (0)     1095 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_deps.py
--rw-r--r--   0 root         (0) root         (0)      683 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_gql.py
--rw-r--r--   0 root         (0) root         (0)     8872 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_metrics.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-09 17:58:34.728206 dagster-cloud-cli-1.7.5/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1288 2024-05-09 17:47:54.000000 dagster-cloud-cli-1.7.5/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.080917 dagster-cloud-cli-1.7.6/
+-rw-r--r--   0 root         (0) root         (0)      132 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-16 20:18:34.080917 dagster-cloud-cli-1.7.6/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.040917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/
+-rw-r--r--   0 root         (0) root         (0)      160 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.040917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.040917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/branch_deployment/
+-rw-r--r--   0 root         (0) root         (0)     5173 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/branch_deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.044917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/ci/
+-rw-r--r--   0 root         (0) root         (0)    30031 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/ci/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4124 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/ci/checks.py
+-rw-r--r--   0 root         (0) root         (0)     1872 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/ci/report.py
+-rw-r--r--   0 root         (0) root         (0)     4121 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/ci/state.py
+-rw-r--r--   0 root         (0) root         (0)      550 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/ci/utils.py
+-rw-r--r--   0 root         (0) root         (0)     8651 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.044917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/deployment/
+-rw-r--r--   0 root         (0) root         (0)     3098 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/deployment/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.048917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/deployment/alert_policies/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/deployment/alert_policies/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1803 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/deployment/alert_policies/commands.py
+-rw-r--r--   0 root         (0) root         (0)    17101 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.048917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/job/
+-rw-r--r--   0 root         (0) root         (0)     1985 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/job/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4425 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/metrics.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.048917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/organization/
+-rw-r--r--   0 root         (0) root         (0)     4001 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.052917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/organization/saml/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/organization/saml/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2691 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/organization/saml/commands.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.052917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/run/
+-rw-r--r--   0 root         (0) root         (0)      757 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/run/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.052917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/serverless/
+-rw-r--r--   0 root         (0) root         (0)     1499 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/serverless/Dockerfile
+-rw-r--r--   0 root         (0) root         (0)      628 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli
+-rw-r--r--   0 root         (0) root         (0)    18458 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/serverless/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.052917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/workspace/
+-rw-r--r--   0 root         (0) root         (0)    12788 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/workspace/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18301 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/config_utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.060917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/agent_queue.py
+-rw-r--r--   0 root         (0) root         (0)      901 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/alert_types.py
+-rw-r--r--   0 root         (0) root         (0)     4801 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/artifacts.py
+-rw-r--r--   0 root         (0) root         (0)     1744 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/docker_runner.py
+-rw-r--r--   0 root         (0) root         (0)     1131 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/errors.py
+-rw-r--r--   0 root         (0) root         (0)    13801 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/graphql_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.064917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/headers/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/headers/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      376 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/headers/auth.py
+-rw-r--r--   0 root         (0) root         (0)      924 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/headers/impl.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.064917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/headers/versioning/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/headers/versioning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       96 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/headers/versioning/constants.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.072917 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/
+-rw-r--r--   0 root         (0) root         (0)      172 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1680 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/code_location.py
+-rw-r--r--   0 root         (0) root         (0)     9423 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/deploy.py
+-rw-r--r--   0 root         (0) root         (0)    14436 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/deps.py
+-rw-r--r--   0 root         (0) root         (0)      949 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/git_context.py
+-rw-r--r--   0 root         (0) root         (0)     6992 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/github_context.py
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/gitlab_context.py
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/parse_workspace.py
+-rw-r--r--   0 root         (0) root         (0)     4655 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/pex_registry.py
+-rw-r--r--   0 root         (0) root         (0)      709 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/selftest.py
+-rw-r--r--   0 root         (0) root         (0)     5407 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/source.py
+-rw-r--r--   0 root         (0) root         (0)     6220 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/util.py
+-rw-r--r--   0 root         (0) root         (0)     2106 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pydantic_yaml.py
+-rw-r--r--   0 root         (0) root         (0)     8382 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/workspace.py
+-rw-r--r--   0 root         (0) root         (0)     2463 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/docker_utils.py
+-rw-r--r--   0 root         (0) root         (0)     6708 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/entrypoint.py
+-rw-r--r--   0 root         (0) root         (0)    20800 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/gql.py
+-rw-r--r--   0 root         (0) root         (0)     5859 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/pex_utils.py
+-rw-r--r--   0 root         (0) root         (0)     1845 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/types.py
+-rw-r--r--   0 root         (0) root         (0)     2804 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/ui.py
+-rw-r--r--   0 root         (0) root         (0)     3488 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/utils.py
+-rw-r--r--   0 root         (0) root         (0)       22 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.040917 dagster-cloud-cli-1.7.6/dagster_cloud_cli.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      314 2024-05-16 20:18:33.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3066 2024-05-16 20:18:33.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-16 20:18:33.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       67 2024-05-16 20:18:33.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2024-05-16 20:18:33.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       42 2024-05-16 20:18:33.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-16 20:18:34.076917 dagster-cloud-cli-1.7.6/dagster_cloud_cli_tests/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli_tests/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      189 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli_tests/conftest.py
+-rw-r--r--   0 root         (0) root         (0)     4130 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli_tests/test_check.py
+-rw-r--r--   0 root         (0) root         (0)    16177 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli_tests/test_ci_commands.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli_tests/test_deps.py
+-rw-r--r--   0 root         (0) root         (0)      683 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli_tests/test_gql.py
+-rw-r--r--   0 root         (0) root         (0)     8872 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/dagster_cloud_cli_tests/test_metrics.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-16 20:18:34.080917 dagster-cloud-cli-1.7.6/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1283 2024-05-16 20:06:42.000000 dagster-cloud-cli-1.7.6/setup.py
```

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/branch_deployment/__init__.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/branch_deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/__init__.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/ci/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/checks.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/ci/checks.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/report.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/ci/report.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/state.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/ci/state.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/ci/utils.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/ci/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/config.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/config.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/__init__.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/alert_policies/commands.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/deployment/alert_policies/commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/deployment/alert_policies/config_schema.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/job/__init__.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/job/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/metrics.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/metrics.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/organization/__init__.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/organization/saml/commands.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/organization/saml/commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/run/__init__.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/run/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/serverless/Dockerfile` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/serverless/Dockerfile`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/serverless/Dockerfile.dagster-cloud-cli`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/serverless/__init__.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/serverless/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/commands/workspace/__init__.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/commands/workspace/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/config_utils.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/config_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/alert_types.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/alert_types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/artifacts.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/artifacts.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/docker_runner.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/docker_runner.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/errors.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/errors.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/graphql_client.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/graphql_client.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/headers/impl.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/headers/impl.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/code_location.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/code_location.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/deploy.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/deploy.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/deps.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/deps.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/git_context.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/git_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/github_context.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/github_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/gitlab_context.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/gitlab_context.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/parse_workspace.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/parse_workspace.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/pex_registry.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/pex_registry.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/selftest.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/selftest.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/source.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/source.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pex_builder/util.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pex_builder/util.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/pydantic_yaml.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/pydantic_yaml.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/core/workspace.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/core/workspace.py`

 * *Files 6% similar despite different names*

```diff
@@ -66,14 +66,22 @@
     custom_instance_class_data = instance_ref.custom_instance_class_data
     if custom_instance_class_data:
         config_dict = custom_instance_class_data.config_dict
         new_config_dict = {
             key: val for key, val in config_dict.items() if key not in {"agent_queues"}
         }
 
+        user_code_launcher_config = config_dict.get("user_code_launcher", {}).get("config")
+        if user_code_launcher_config:
+            new_config_dict["user_code_launcher"]["config"] = {
+                key: val
+                for key, val in user_code_launcher_config.items()
+                if key not in {"agent_metrics"}
+            }
+
         custom_instance_class_data = custom_instance_class_data._replace(
             config_yaml=yaml.dump(new_config_dict)
         )
 
     return instance_ref._replace(custom_instance_class_data=custom_instance_class_data)
```

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/docker_utils.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/docker_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/entrypoint.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/entrypoint.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/gql.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/gql.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/pex_utils.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/pex_utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/types.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/types.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/ui.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/ui.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli/utils.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli.egg-info/SOURCES.txt` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_check.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli_tests/test_check.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_ci_commands.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli_tests/test_ci_commands.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_deps.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli_tests/test_deps.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_gql.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli_tests/test_gql.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/dagster_cloud_cli_tests/test_metrics.py` & `dagster-cloud-cli-1.7.6/dagster_cloud_cli_tests/test_metrics.py`

 * *Files identical despite different names*

### Comparing `dagster-cloud-cli-1.7.5/setup.py` & `dagster-cloud-cli-1.7.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,19 +19,19 @@
 setup(
     name="dagster-cloud-cli",
     version=get_version(),
     author_email="hello@elementl.com",
     packages=find_packages(exclude=["dagster_cloud.cli_tests*"]),
     include_package_data=True,
     install_requires=[
-        "dagster==1.7.5",
+        "dagster==1.7.6",
         "packaging>=20.9",
         "questionary",
         "requests",
-        "typer[all]>=0.4.1",
+        "typer>=0.4.1",
         "PyYAML>=5.1",
         "github3.py",
     ],
     extras_require={
         "tests": [
             "freezegun",
         ],
```

