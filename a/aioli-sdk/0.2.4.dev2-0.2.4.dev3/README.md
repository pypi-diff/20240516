# Comparing `tmp/aioli_sdk-0.2.4.dev2.tar.gz` & `tmp/aioli_sdk-0.2.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aioli_sdk-0.2.4.dev2.tar", last modified: Tue May  7 09:58:17 2024, max compression
+gzip compressed data, was "aioli_sdk-0.2.4.dev3.tar", last modified: Thu May 16 10:38:47 2024, max compression
```

## Comparing `aioli_sdk-0.2.4.dev2.tar` & `aioli_sdk-0.2.4.dev3.tar`

### file list

```diff
@@ -1,98 +1,98 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-07 09:58:17.931867 aioli_sdk-0.2.4.dev2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-07 09:58:17.931867 aioli_sdk-0.2.4.dev2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-07 09:58:17.927867 aioli_sdk-0.2.4.dev2/aioli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/__version__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-07 09:58:17.927867 aioli_sdk-0.2.4.dev2/aioli/cli/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/__main__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8270 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    13159 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14935 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7705 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/render.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/sso.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-07 09:58:17.927867 aioli_sdk-0.2.4.dev2/aioli/cli/test/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/test/conftest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    29032 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/test/test_cli.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/cli/version.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-07 09:58:17.927867 aioli_sdk-0.2.4.dev2/aioli/common/
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/common/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-07 09:58:17.927867 aioli_sdk-0.2.4.dev2/aioli/common/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/common/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/common/api/_util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/common/api/authentication.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/common/api/certs.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/common/api/errors.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/common/api/request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/common/check.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/common/constants.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/common/declarative_argparse.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/common/requests.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4706 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/common/util.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/aioli/util.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-07 09:58:17.931867 aioli_sdk-0.2.4.dev2/aioli_sdk.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-07 09:58:17.000000 aioli_sdk-0.2.4.dev2/aioli_sdk.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2482 2024-05-07 09:58:17.000000 aioli_sdk-0.2.4.dev2/aioli_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-07 09:58:17.000000 aioli_sdk-0.2.4.dev2/aioli_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-05-07 09:58:17.000000 aioli_sdk-0.2.4.dev2/aioli_sdk.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-07 09:58:15.000000 aioli_sdk-0.2.4.dev2/aioli_sdk.egg-info/not-zip-safe
--rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-05-07 09:58:17.000000 aioli_sdk-0.2.4.dev2/aioli_sdk.egg-info/requires.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-07 09:58:17.000000 aioli_sdk-0.2.4.dev2/aioli_sdk.egg-info/top_level.txt
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-07 09:58:17.927867 aioli_sdk-0.2.4.dev2/aiolirest/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3218 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/__init__.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-07 09:58:17.931867 aioli_sdk-0.2.4.dev2/aiolirest/api/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/api/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    22813 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/api/authentication_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    84659 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/api/deployments_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    10515 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/api/information_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    91193 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/api/packaged_models_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    64597 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/api/registries_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    43082 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/api/roles_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)   105944 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/api/templates_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    61885 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/api/users_api.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    25050 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/api_client.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/api_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14926 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/configuration.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5597 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/exceptions.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-07 09:58:17.931867 aioli_sdk-0.2.4.dev2/aiolirest/models/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2280 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/auto_scaling_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3986 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/autoscaling.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3662 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/configuration_resources.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     7356 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/deployment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4309 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/deployment_model_version.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5068 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/deployment_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     4884 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/deployment_state.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/error_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/event_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3261 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/failure_info.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2642 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/login_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/login_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2820 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/model_auth_token.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3950 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/model_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/observability.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     6065 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/packaged_model.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5499 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/packaged_model_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2940 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/resource_profile.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3366 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/resources_template.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2747 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/role.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2836 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/role_assignment.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2024-05-07 09:58:13.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/role_assignments.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/security.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2649 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/success_response.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5202 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/trained_model_registry.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     5028 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/trained_model_registry_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/user.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2663 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/user_patch_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     3387 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/models/user_request.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/py.typed
--rw-r--r--   0 circleci  (1001) circleci  (1002)     8440 2024-05-07 09:58:14.000000 aioli_sdk-0.2.4.dev2/aiolirest/rest.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-07 09:58:17.931867 aioli_sdk-0.2.4.dev2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2024-05-07 09:52:48.000000 aioli_sdk-0.2.4.dev2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.370155 aioli_sdk-0.2.4.dev3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-16 10:38:47.366155 aioli_sdk-0.2.4.dev3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      176 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.362155 aioli_sdk-0.2.4.dev3/aioli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      109 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       89 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/__version__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.362155 aioli_sdk-0.2.4.dev3/aioli/cli/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      132 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      147 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/__main__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1644 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8270 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    13159 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      689 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14935 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7705 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7221 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/render.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3558 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5304 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/sso.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.362155 aioli_sdk-0.2.4.dev3/aioli/cli/test/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      728 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/test/conftest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    29096 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/test/test_cli.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6629 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3103 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/cli/version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.362155 aioli_sdk-0.2.4.dev3/aioli/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.362155 aioli_sdk-0.2.4.dev3/aioli/common/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      336 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      348 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/api/_util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    18000 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/api/authentication.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8098 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/api/certs.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3671 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/api/errors.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10969 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/api/request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8655 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/check.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      650 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/constants.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8480 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/declarative_argparse.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1724 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/requests.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4706 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/common/util.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2272 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/aioli/util.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.366155 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1420 2024-05-16 10:38:47.000000 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2482 2024-05-16 10:38:47.000000 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-16 10:38:47.000000 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       50 2024-05-16 10:38:47.000000 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2024-05-16 10:38:45.000000 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/not-zip-safe
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      474 2024-05-16 10:38:47.000000 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       16 2024-05-16 10:38:47.000000 aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.362155 aioli_sdk-0.2.4.dev3/aiolirest/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3218 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/__init__.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.366155 aioli_sdk-0.2.4.dev3/aiolirest/api/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      487 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    22813 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/authentication_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    84659 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/deployments_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    10515 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/information_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    91193 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/packaged_models_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    66586 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/registries_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    43082 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/roles_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   105944 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/templates_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    61885 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api/users_api.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    25050 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api_client.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      674 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/api_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14926 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/configuration.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5597 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/exceptions.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:47.366155 aioli_sdk-0.2.4.dev3/aiolirest/models/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2280 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3384 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/auto_scaling_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3986 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/autoscaling.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3662 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/configuration_resources.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     7356 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/deployment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4309 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/deployment_model_version.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5068 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/deployment_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5091 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/deployment_state.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2788 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/error_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3775 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/event_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3261 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/failure_info.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2642 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/login_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/login_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2820 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/model_auth_token.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4130 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/model_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2970 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/observability.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     6263 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/packaged_model.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5740 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/packaged_model_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2940 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/resource_profile.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3366 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/resources_template.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2747 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/role.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2836 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/role_assignment.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3296 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/role_assignments.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2905 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/security.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2649 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/success_response.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5202 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/trained_model_registry.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     5028 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/trained_model_registry_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3932 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/user.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2663 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/user_patch_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3387 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/models/user_request.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/py.typed
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     8440 2024-05-16 10:38:43.000000 aioli_sdk-0.2.4.dev3/aiolirest/rest.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      113 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2024-05-16 10:38:47.370155 aioli_sdk-0.2.4.dev3/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2404 2024-05-16 10:33:30.000000 aioli_sdk-0.2.4.dev3/setup.py
```

### Comparing `aioli_sdk-0.2.4.dev2/PKG-INFO` & `aioli_sdk-0.2.4.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.4.dev2
+Version: 0.2.4.dev3
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli_sdk-0.2.4.dev2/aioli/cli/_util.py` & `aioli_sdk-0.2.4.dev3/aioli/cli/_util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/cli/cli.py` & `aioli_sdk-0.2.4.dev3/aioli/cli/cli.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/cli/deployment.py` & `aioli_sdk-0.2.4.dev3/aioli/cli/deployment.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/cli/errors.py` & `aioli_sdk-0.2.4.dev3/aioli/cli/errors.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/cli/model.py` & `aioli_sdk-0.2.4.dev3/aioli/cli/model.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/cli/registry.py` & `aioli_sdk-0.2.4.dev3/aioli/cli/registry.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/cli/render.py` & `aioli_sdk-0.2.4.dev3/aioli/cli/render.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/cli/role.py` & `aioli_sdk-0.2.4.dev3/aioli/cli/role.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/cli/sso.py` & `aioli_sdk-0.2.4.dev3/aioli/cli/sso.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/cli/test/conftest.py` & `aioli_sdk-0.2.4.dev3/aioli/cli/test/conftest.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/cli/test/test_cli.py` & `aioli_sdk-0.2.4.dev3/aioli/cli/test/test_cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,22 +338,22 @@
 
     def test_model_create_no_image(self, setup_login: None) -> None:
         # The image is optional; verify...
         assert (
             os.system(
                 "aioli model create openllm --registry bento-registry1 "
                 "--format openllm "
-                "--url openllm://demo-bento-registry/iris-tf-keras "
+                "--url s3://demo-bento-registry/iris-tf-keras "
                 '--description "the model description"'
             )
             == 0
         )
         expected = (
             "openllm       | the model description |         1 | "
-            "openllm://demo-bento-registry/iris-tf-keras |"
+            "s3://demo-bento-registry/iris-tf-keras |"
             "                                      | bento-registry1"
         )
         actual = subprocess.check_output(["aioli", "model", "list"]).decode("utf-8")
 
         assert (actual.find(expected)) > 0
         assert os.system("aioli model delete openllm 1") == 0
 
@@ -555,23 +555,25 @@
             '    "environment": {},\n'
             '    "goalStatus": "Ready",\n'
             '    "model": "iris-tf-keras",\n'
             '    "name": "iris-tf-keras-deployment",\n'
             '    "namespace": "aioli",\n'
             '    "secondaryState": {\n'
             '      "endpoint": "",\n'
+            '      "modelId": "",\n'
             '      "nativeAppName": "",\n'
             '      "status": "None",\n'
             '      "trafficPercentage": 0\n'
             '    },\n'  # noqa: Q000
             '    "security": {\n'
             '      "authenticationRequired": true\n'
             '    },\n'  # noqa: Q000
             '    "state": {\n'
             '      "endpoint": "",\n'
+            '      "modelId": "",\n'
             '      "nativeAppName": "",\n'
             '      "status": "Deploying",\n'
             '      "trafficPercentage": 0\n'
             '    },\n'  # noqa: Q000
             '    "status": "Deploying"\n'
             '  }\n'  # noqa: Q000
             ']\n'    # noqa: Q000
```

### Comparing `aioli_sdk-0.2.4.dev2/aioli/cli/user.py` & `aioli_sdk-0.2.4.dev3/aioli/cli/user.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/cli/version.py` & `aioli_sdk-0.2.4.dev3/aioli/cli/version.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/common/api/authentication.py` & `aioli_sdk-0.2.4.dev3/aioli/common/api/authentication.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/common/api/certs.py` & `aioli_sdk-0.2.4.dev3/aioli/common/api/certs.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/common/api/errors.py` & `aioli_sdk-0.2.4.dev3/aioli/common/api/errors.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/common/api/request.py` & `aioli_sdk-0.2.4.dev3/aioli/common/api/request.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/common/check.py` & `aioli_sdk-0.2.4.dev3/aioli/common/check.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/common/constants.py` & `aioli_sdk-0.2.4.dev3/aioli/common/constants.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/common/declarative_argparse.py` & `aioli_sdk-0.2.4.dev3/aioli/common/declarative_argparse.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/common/requests.py` & `aioli_sdk-0.2.4.dev3/aioli/common/requests.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/common/util.py` & `aioli_sdk-0.2.4.dev3/aioli/common/util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli/util.py` & `aioli_sdk-0.2.4.dev3/aioli/util.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aioli_sdk.egg-info/PKG-INFO` & `aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioli-sdk
-Version: 0.2.4.dev2
+Version: 0.2.4.dev3
 Summary: Aioli (AI OnLine Inference), a platform for deploying AI models at scale.
 Home-page: https://github.com/determined-ai/aioli
 Author: HPE AI Solutions
 License: Apache License 2.0
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: packaging
```

### Comparing `aioli_sdk-0.2.4.dev2/aioli_sdk.egg-info/SOURCES.txt` & `aioli_sdk-0.2.4.dev3/aioli_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/__init__.py` & `aioli_sdk-0.2.4.dev3/aiolirest/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # flake8: noqa
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/api/authentication_api.py` & `aioli_sdk-0.2.4.dev3/aiolirest/api/authentication_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/api/deployments_api.py` & `aioli_sdk-0.2.4.dev3/aiolirest/api/deployments_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/api/information_api.py` & `aioli_sdk-0.2.4.dev3/aiolirest/api/information_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/api/packaged_models_api.py` & `aioli_sdk-0.2.4.dev3/aiolirest/api/packaged_models_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/api/registries_api.py` & `aioli_sdk-0.2.4.dev3/aiolirest/api/registries_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -24,15 +24,15 @@
 except ImportError:
     from typing_extensions import Annotated
 
 from pydantic import Field
 from typing_extensions import Annotated
 from pydantic import StrictStr
 
-from typing import List
+from typing import List, Optional
 
 from aiolirest.models.model_response import ModelResponse
 from aiolirest.models.success_response import SuccessResponse
 from aiolirest.models.trained_model_registry import TrainedModelRegistry
 from aiolirest.models.trained_model_registry_request import TrainedModelRegistryRequest
 
 from aiolirest.api_client import ApiClient
@@ -839,14 +839,15 @@
 
 
 
     @validate_call
     def registries_id_models_get(
         self,
         id: Annotated[StrictStr, Field(description="Model Registry ID")],
+        modelformat: Annotated[Optional[StrictStr], Field(description="Model Format Type")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -854,18 +855,20 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> List[ModelResponse]:
         """Get all available models from a registry
 
-        Returns an array of all available models from a registry
+        Returns an array of all available models from a registry When listing from an openllm registry, specify the modelformat (case sensitive) query parameter to filter the responses to a manageable number. The supported format names for openllm are: [baichuan,chatglm,dolly_v2,falcon,flan_t5, gemma,gpt_neox,llama,mistral,mixtral,mpt,opt,phi,qwen,stablelm,starcoder,yi] The list is from https://github.com/bentoml/OpenLLM?tab=readme-ov-file#-supported-models
 
         :param id: Model Registry ID (required)
         :type id: str
+        :param modelformat: Model Format Type
+        :type modelformat: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -882,14 +885,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._registries_id_models_get_serialize(
             id=id,
+            modelformat=modelformat,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -909,14 +913,15 @@
         ).data
 
 
     @validate_call
     def registries_id_models_get_with_http_info(
         self,
         id: Annotated[StrictStr, Field(description="Model Registry ID")],
+        modelformat: Annotated[Optional[StrictStr], Field(description="Model Format Type")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -924,18 +929,20 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[List[ModelResponse]]:
         """Get all available models from a registry
 
-        Returns an array of all available models from a registry
+        Returns an array of all available models from a registry When listing from an openllm registry, specify the modelformat (case sensitive) query parameter to filter the responses to a manageable number. The supported format names for openllm are: [baichuan,chatglm,dolly_v2,falcon,flan_t5, gemma,gpt_neox,llama,mistral,mixtral,mpt,opt,phi,qwen,stablelm,starcoder,yi] The list is from https://github.com/bentoml/OpenLLM?tab=readme-ov-file#-supported-models
 
         :param id: Model Registry ID (required)
         :type id: str
+        :param modelformat: Model Format Type
+        :type modelformat: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -952,14 +959,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._registries_id_models_get_serialize(
             id=id,
+            modelformat=modelformat,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -979,14 +987,15 @@
         )
 
 
     @validate_call
     def registries_id_models_get_without_preload_content(
         self,
         id: Annotated[StrictStr, Field(description="Model Registry ID")],
+        modelformat: Annotated[Optional[StrictStr], Field(description="Model Format Type")] = None,
         _request_timeout: Union[
             None,
             Annotated[StrictFloat, Field(gt=0)],
             Tuple[
                 Annotated[StrictFloat, Field(gt=0)],
                 Annotated[StrictFloat, Field(gt=0)]
             ]
@@ -994,18 +1003,20 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Get all available models from a registry
 
-        Returns an array of all available models from a registry
+        Returns an array of all available models from a registry When listing from an openllm registry, specify the modelformat (case sensitive) query parameter to filter the responses to a manageable number. The supported format names for openllm are: [baichuan,chatglm,dolly_v2,falcon,flan_t5, gemma,gpt_neox,llama,mistral,mixtral,mpt,opt,phi,qwen,stablelm,starcoder,yi] The list is from https://github.com/bentoml/OpenLLM?tab=readme-ov-file#-supported-models
 
         :param id: Model Registry ID (required)
         :type id: str
+        :param modelformat: Model Format Type
+        :type modelformat: str
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
         :type _request_timeout: int, tuple(int, int), optional
         :param _request_auth: set to override the auth_settings for an a single
                               request; this effectively ignores the
@@ -1022,14 +1033,15 @@
                             in the spec for a single request.
         :type _host_index: int, optional
         :return: Returns the result object.
         """ # noqa: E501
 
         _param = self._registries_id_models_get_serialize(
             id=id,
+            modelformat=modelformat,
             _request_auth=_request_auth,
             _content_type=_content_type,
             _headers=_headers,
             _host_index=_host_index
         )
 
         _response_types_map: Dict[str, Optional[str]] = {
@@ -1044,14 +1056,15 @@
         )
         return response_data.response
 
 
     def _registries_id_models_get_serialize(
         self,
         id,
+        modelformat,
         _request_auth,
         _content_type,
         _headers,
         _host_index,
     ) -> Tuple:
 
         _host = None
@@ -1067,14 +1080,18 @@
         _files: Dict[str, str] = {}
         _body_params: Optional[bytes] = None
 
         # process the path parameters
         if id is not None:
             _path_params['id'] = id
         # process the query parameters
+        if modelformat is not None:
+            
+            _query_params.append(('modelformat', modelformat))
+            
         # process the header parameters
         # process the form parameters
         # process the body parameter
 
 
         # set the HTTP header `Accept`
         _header_params['Accept'] = self.api_client.select_header_accept(
@@ -1405,15 +1422,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> TrainedModelRegistry:
         """Create a new model registry.
 
-        A packaged model registry provides the necessary metadata to access and download a model.  Download is suported from S3 storage servers, OpenLLM models from huggingface.co, or NGC models from Nvidia NGC: AI Development Catalog.
+        A packaged model registry provides the necessary metadata to access and download a model.  Download is suported from S3 storage servers, OpenLLM models from huggingface.co, or NGC models from NVIDIA NGC: AI Development Catalog.
 
         :param trained_model_registry: Model Registry Data (required)
         :type trained_model_registry: TrainedModelRegistryRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1475,15 +1492,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> ApiResponse[TrainedModelRegistry]:
         """Create a new model registry.
 
-        A packaged model registry provides the necessary metadata to access and download a model.  Download is suported from S3 storage servers, OpenLLM models from huggingface.co, or NGC models from Nvidia NGC: AI Development Catalog.
+        A packaged model registry provides the necessary metadata to access and download a model.  Download is suported from S3 storage servers, OpenLLM models from huggingface.co, or NGC models from NVIDIA NGC: AI Development Catalog.
 
         :param trained_model_registry: Model Registry Data (required)
         :type trained_model_registry: TrainedModelRegistryRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
@@ -1545,15 +1562,15 @@
         _request_auth: Optional[Dict[StrictStr, Any]] = None,
         _content_type: Optional[StrictStr] = None,
         _headers: Optional[Dict[StrictStr, Any]] = None,
         _host_index: Annotated[StrictInt, Field(ge=0, le=0)] = 0,
     ) -> RESTResponseType:
         """Create a new model registry.
 
-        A packaged model registry provides the necessary metadata to access and download a model.  Download is suported from S3 storage servers, OpenLLM models from huggingface.co, or NGC models from Nvidia NGC: AI Development Catalog.
+        A packaged model registry provides the necessary metadata to access and download a model.  Download is suported from S3 storage servers, OpenLLM models from huggingface.co, or NGC models from NVIDIA NGC: AI Development Catalog.
 
         :param trained_model_registry: Model Registry Data (required)
         :type trained_model_registry: TrainedModelRegistryRequest
         :param _request_timeout: timeout setting for this request. If one
                                  number provided, it will be total request
                                  timeout. It can also be a pair (tuple) of
                                  (connection, read) timeouts.
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/api/roles_api.py` & `aioli_sdk-0.2.4.dev3/aiolirest/api/roles_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/api/templates_api.py` & `aioli_sdk-0.2.4.dev3/aiolirest/api/templates_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/api/users_api.py` & `aioli_sdk-0.2.4.dev3/aiolirest/api/users_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/api_client.py` & `aioli_sdk-0.2.4.dev3/aiolirest/api_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/api_response.py` & `aioli_sdk-0.2.4.dev3/aiolirest/api_response.py`

 * *Files identical despite different names*

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/configuration.py` & `aioli_sdk-0.2.4.dev3/aiolirest/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -385,15 +385,15 @@
         """Gets the essential information for debugging.
 
         :return: The report for debugging.
         """
         return "Python SDK Debug Report:\n"\
                "OS: {env}\n"\
                "Python Version: {pyversion}\n"\
-               "Version of the API: 0.2.4-dev2\n"\
+               "Version of the API: 0.2.4-dev3\n"\
                "SDK Package Version: 1.0.0".\
                format(env=sys.platform, pyversion=sys.version)
 
     def get_host_settings(self):
         """Gets an array of host settings
 
         :return: An array of host settings
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/exceptions.py` & `aioli_sdk-0.2.4.dev3/aiolirest/exceptions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/__init__.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # flake8: noqa
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/auto_scaling_template.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/auto_scaling_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/autoscaling.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/autoscaling.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/configuration_resources.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/configuration_resources.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/deployment.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/deployment.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/deployment_model_version.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/deployment_model_version.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -32,18 +32,18 @@
     The DeploymentModelVersion provides model evolution data that track model deployment changes over time.
     """ # noqa: E501
     canary_traffic_percent: Optional[StrictInt] = Field(default=None, description="Percent traffic to pass to the model.", alias="canaryTrafficPercent")
     deployed: Optional[StrictStr] = Field(default=None, description="The deployment time. This is a read-only field and is automatically assigned on creation.")
     deployment_id: Optional[StrictStr] = Field(default=None, description="The deployment ID", alias="deploymentId")
     deployment_name: Optional[StrictStr] = Field(default=None, description="The deployment name", alias="deploymentName")
     model: Optional[StrictStr] = Field(default=None, description="The name of the model.")
-    mdl_id: Optional[StrictStr] = Field(default=None, description="The ID of the model.", alias="modelID")
+    mdl_id: Optional[StrictStr] = Field(default=None, description="The ID of the model.", alias="modelId")
     mdl_version: Optional[StrictStr] = Field(default=None, description="The version of the model.", alias="modelVersion")
     native_app_name: Optional[StrictStr] = Field(default=None, description="The name of the Kubernetes application for the specific service version. Use this name to match the app value in Grafana/Prometheus to obtain logs and metrics for this deployed service version.", alias="nativeAppName")
-    __properties: ClassVar[List[str]] = ["canaryTrafficPercent", "deployed", "deploymentId", "deploymentName", "model", "modelID", "modelVersion", "nativeAppName"]
+    __properties: ClassVar[List[str]] = ["canaryTrafficPercent", "deployed", "deploymentId", "deploymentName", "model", "modelId", "modelVersion", "nativeAppName"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -90,14 +90,14 @@
 
         _obj = cls.model_validate({
             "canaryTrafficPercent": obj.get("canaryTrafficPercent"),
             "deployed": obj.get("deployed"),
             "deploymentId": obj.get("deploymentId"),
             "deploymentName": obj.get("deploymentName"),
             "model": obj.get("model"),
-            "modelID": obj.get("modelID"),
+            "modelId": obj.get("modelId"),
             "modelVersion": obj.get("modelVersion"),
             "nativeAppName": obj.get("nativeAppName")
         })
         return _obj
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/deployment_request.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/deployment_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/deployment_state.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/deployment_state.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -30,18 +30,19 @@
 
 class DeploymentState(BaseModel):
     """
     Describes the current state of the deployment as managed by KServe
     """ # noqa: E501
     endpoint: Optional[StrictStr] = Field(default=None, description="Endpoint to access inference service.")
     failure_info: Optional[List[FailureInfo]] = Field(default=None, description="List of any failures that have occurred.", alias="failureInfo")
+    mdl_id: Optional[StrictStr] = Field(default=None, description="The ID of the deployed packaged model associcated with this state.", alias="modelId")
     native_app_name: Optional[StrictStr] = Field(default=None, description="The name of the Kubernetes application for the specific service version. Use this name to match the app value in Grafana/Prometheus to obtain logs and metrics for this deployed service version.", alias="nativeAppName")
     status: Optional[StrictStr] = Field(default=None, description="Status of a particular service revision. * `Deploying` - Service configuration is in progress. * `Failed` - The service configuration failed. * `Ready` - The service has been successfully configured and is serving. * `Updating` - A new service revision is being rolledout. * `UpdateFailed` - The current service revision failed to rollout due to an error.   The prior version is still serving requests. * `Deleting` - The deployed service is being removed. * `Paused` - The deployed service has been stopped by the user or an external action. * `Unknown` - Unable to determined the status.  This is a read-only property. Must be one of the values: (Deploying,Ready,Updating,UpdateFailed,Failed,Deleting,Paused,Unknown).")
     traffic_percentage: Optional[StrictInt] = Field(default=None, description="Target percentage of traffic intended for this service version when successfully deployed.", alias="trafficPercentage")
-    __properties: ClassVar[List[str]] = ["endpoint", "failureInfo", "nativeAppName", "status", "trafficPercentage"]
+    __properties: ClassVar[List[str]] = ["endpoint", "failureInfo", "modelId", "nativeAppName", "status", "trafficPercentage"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -92,14 +93,15 @@
 
         if not isinstance(obj, dict):
             return cls.model_validate(obj)
 
         _obj = cls.model_validate({
             "endpoint": obj.get("endpoint"),
             "failureInfo": [FailureInfo.from_dict(_item) for _item in obj.get("failureInfo")] if obj.get("failureInfo") is not None else None,
+            "modelId": obj.get("modelId"),
             "nativeAppName": obj.get("nativeAppName"),
             "status": obj.get("status"),
             "trafficPercentage": obj.get("trafficPercentage")
         })
         return _obj
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/error_response.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/error_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/event_info.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/event_info.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/failure_info.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/failure_info.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/login_request.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/login_request.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/login_response.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/login_response.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/model_auth_token.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/model_auth_token.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/model_response.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/model_response.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -33,16 +33,17 @@
     """ # noqa: E501
     description: Optional[StrictStr] = Field(default=None, description="The description of desribing the model")
     display_name: Optional[StrictStr] = Field(default=None, description="The name displayed that is human readable", alias="displayName")
     image: Optional[StrictStr] = Field(default=None, description="The default container image to execute the model (if available)")
     latest_version_id_str: Optional[StrictStr] = Field(default=None, description="The latest version of the model", alias="latestVersionIdStr")
     latest_version_size_in_bytes: Optional[StrictInt] = Field(default=None, description="The number of bytes for the latest model", alias="latestVersionSizeInBytes")
     metadata: Optional[Dict[str, StrictStr]] = Field(default=None, description="Extra argument in case more variables need to be stored.")
+    format: Optional[StrictStr] = Field(default=None, description="The format of the model", alias="modelFormat")
     name: Optional[StrictStr] = Field(default=None, description="The name used in model specification")
-    __properties: ClassVar[List[str]] = ["description", "displayName", "image", "latestVersionIdStr", "latestVersionSizeInBytes", "metadata", "name"]
+    __properties: ClassVar[List[str]] = ["description", "displayName", "image", "latestVersionIdStr", "latestVersionSizeInBytes", "metadata", "modelFormat", "name"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
 
 
@@ -90,12 +91,13 @@
         _obj = cls.model_validate({
             "description": obj.get("description"),
             "displayName": obj.get("displayName"),
             "image": obj.get("image"),
             "latestVersionIdStr": obj.get("latestVersionIdStr"),
             "latestVersionSizeInBytes": obj.get("latestVersionSizeInBytes"),
             "metadata": obj.get("metadata"),
+            "modelFormat": obj.get("modelFormat"),
             "name": obj.get("name")
         })
         return _obj
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/observability.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/observability.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/packaged_model.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/packaged_model.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -33,20 +33,20 @@
     The PackagedModel describes a specific model that can be loaded. It optionally references a model registry to provide authorization, and other details.
     """ # noqa: E501
     arguments: Optional[List[StrictStr]] = Field(default=None, description="Arguments to be added to the service command line")
     description: Optional[StrictStr] = Field(default=None, description="A description of the model.")
     environment: Optional[Dict[str, StrictStr]] = Field(default=None, description="Environment variables added to the service")
     id: Optional[StrictStr] = Field(default=None, description="The ID of the model.  This is a read-only field and is automatically assigned on creation.")
     image: Optional[StrictStr] = Field(default=None, description="Docker container image servicing the model.")
-    format: Optional[StrictStr] = Field(default='custom', description="Model format for downloaded models (e.g. from s3, http, etc.). Must be one of the values: (bento-archive, openllm, nim, custom). * `custom` - The packaged model is provided in a container image. * `bento-archive` - The packaged model is a bento archive file (.bento).  It will be downloaded,  expanded, and then  will be served using the `bentolm serve` command in a provided bentoml serving container. * `openllm` - The packaged model will be served using the `openllm serve` command in a  provided openllm serving container. * `nim` - The packaged model will be served using an Nvidia NIM microservices container.", alias="modelFormat")
+    format: Optional[StrictStr] = Field(default='custom', description="Model format for downloaded models (e.g. from s3, http, etc.). Must be one of the values: (bento-archive, openllm, nim, custom). * `custom` - The packaged model is provided in a container image. * `bento-archive` - The packaged model is a bento archive file (.bento).  It will be downloaded,  expanded, and then  will be served using the `bentolm serve` command in a provided bentoml serving container. * `openllm` - The packaged model will be served using the `openllm serve` command in a  provided openllm serving container. * `nim` - The packaged model will be served using the specified NVIDIA NIM microservices container image.", alias="modelFormat")
     modified_at: Optional[StrictStr] = Field(default=None, description="Date-time of last modification of the model. This is a read-only field and is automatically updated.", alias="modifiedAt")
     name: StrictStr = Field(description="The name of the model.  Must begin with a letter, but may contain letters, numbers, and hyphen.")
     registry: Optional[StrictStr] = Field(default=None, description="The name or ID of the model registry.")
     resources: Optional[ConfigurationResources] = None
-    url: Optional[StrictStr] = Field(default=None, description="Reference to the bento or model to be served.  Supported schemes are: * `openllm://` - An openllm model name from huggingface.co dynamically loaded and executed with a VLLM backend. * `s3://` - An openllm model path which will be dynamically downloaded from an associated s3  registry bucket and executed with a VLLM backend.")
+    url: Optional[StrictStr] = Field(default=None, description="Reference to the bento or model to be served.  Supported schemes are: * `openllm://` - An openllm model name from huggingface.co dynamically loaded and executed with a VLLM backend. * `s3://` - An openllm model path which will be dynamically downloaded from an associated s3  registry bucket and executed with a VLLM backend. * `ngc://` - An NVIDIA NGC model will be dynamically downloaded from the associated `ngc`  registry bucket and executed with the specified NVIDIA NIM microservices container image.")
     version: Optional[StrictInt] = Field(default=None, description="The version of the model.  This is a read-only field and is automatically assigned on creation.")
     __properties: ClassVar[List[str]] = ["arguments", "description", "environment", "id", "image", "modelFormat", "modifiedAt", "name", "registry", "resources", "url", "version"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/packaged_model_request.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/packaged_model_request.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
 
 
@@ -31,20 +31,20 @@
 class PackagedModelRequest(BaseModel):
     """
     The PackagedModel describes a specific model that can be loaded. It optionally references a model registry to provide authorization, and other details.
     """ # noqa: E501
     arguments: Optional[List[StrictStr]] = Field(default=None, description="Arguments to be added to the service command line")
     description: Optional[StrictStr] = Field(default=None, description="A description of the model.")
     environment: Optional[Dict[str, StrictStr]] = Field(default=None, description="Environment variables added to the service")
-    image: Optional[StrictStr] = Field(default=None, description="Docker container image servicing the model.")
-    format: Optional[StrictStr] = Field(default='custom', description="Model format for downloaded models (e.g. from s3, http, etc.). Must be one of the values: (bento-archive, openllm, nim, custom). * `custom` - The packaged model is provided in a container image. * `bento-archive` - The packaged model is a bento archive file (.bento).  It will be downloaded,  expanded, and then  will be served using the `bentolm serve` command in a provided bentoml serving container. * `openllm` - The packaged model will be served using the `openllm serve` command in a  provided openllm serving container. * `nim` - The packaged model will be servied using an Nvidia NIM microservices container.", alias="modelFormat")
+    image: Optional[StrictStr] = Field(default=None, description="Docker container image servicing the model.  This is required for a 'nim' model format.")
+    format: Optional[StrictStr] = Field(default='custom', description="Model format for downloaded models (e.g. from s3, http, etc.). Must be one of the values: (bento-archive, openllm, nim, custom). * `custom` - The packaged model is provided in a container image. * `bento-archive` - The packaged model is a bento archive file (.bento).  It will be downloaded,  expanded, and then  will be served using the `bentolm serve` command in a provided bentoml serving container. * `openllm` - The packaged model will be served using the `openllm serve` command in a  provided openllm serving container. * `nim` - The packaged model will be served using the specified NVIDIA NIM microservices container image.", alias="modelFormat")
     name: StrictStr = Field(description="The name of the model. Must consist of alphanumeric characters, '-', or '.', and must start and end with an alphanumeric character. The length of the model name must be 63 characters or less.")
     registry: Optional[StrictStr] = Field(default=None, description="The name or ID of the model registry.")
     resources: Optional[ConfigurationResources] = None
-    url: Optional[StrictStr] = Field(default=None, description="Reference to the bento or model to be served.  Supported schemes are: * `openllm://` - An openllm model name from huggingface.co dynamically loaded and executed with a VLLM backend. * `s3://` - An openllm model path which will be dynamically downloaded from an associated s3  registry bucket and executed with a VLLM backend.")
+    url: Optional[StrictStr] = Field(default=None, description="Reference to the bento or model to be served.  Supported schemes are: * `openllm://` - An openllm model name from huggingface.co dynamically loaded and executed with a VLLM backend. * `s3://` - An openllm model path which will be dynamically downloaded from an associated s3  registry bucket and executed with a VLLM backend. * `ngc://` - An NVIDIA NGC model will be dynamically downloaded from the associated `ngc`  registry bucket and executed with the specified NVIDIA NIM microservices container image.")
     __properties: ClassVar[List[str]] = ["arguments", "description", "environment", "image", "modelFormat", "name", "registry", "resources", "url"]
 
     model_config = {
         "populate_by_name": True,
         "validate_assignment": True
     }
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/resource_profile.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/resource_profile.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/resources_template.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/resources_template.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/role.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/role.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/role_assignment.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/role_assignment.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/role_assignments.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/role_assignments.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/security.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/security.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/success_response.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/success_response.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/trained_model_registry.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/trained_model_registry.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/trained_model_registry_request.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/trained_model_registry_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/user.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/user.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/user_patch_request.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/user_patch_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/models/user_request.py` & `aioli_sdk-0.2.4.dev3/aiolirest/models/user_request.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/aiolirest/rest.py` & `aioli_sdk-0.2.4.dev3/aiolirest/rest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # coding: utf-8
 
 """
     HPE Machine Learning Inference Software (MLIS/Aioli)
 
     HPE MLIS is *Aioli* -- The AI On-line Inference Platform that enables easy deployment, tracking, and serving of your packaged models regardless of your preferred AI framework.
 
-    The version of the OpenAPI document: 0.2.4-dev2
+    The version of the OpenAPI document: 0.2.4-dev3
     Contact: community@determined-ai
     Generated by OpenAPI Generator (https://openapi-generator.tech)
 
     Do not edit the class manually.
 """  # noqa: E501
```

### Comparing `aioli_sdk-0.2.4.dev2/setup.py` & `aioli_sdk-0.2.4.dev3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r") as readme:
     markdown_description = "".join(readme.readlines())
 
 setuptools.setup(
     name="aioli-sdk",
-    version="0.2.4-dev2",
+    version="0.2.4-dev3",
     author="HPE AI Solutions",
     # author_email="hello@determined.ai",
     url="https://github.com/determined-ai/aioli",
     description="Aioli (AI OnLine Inference), a platform for deploying AI models at scale.",
     long_description = markdown_description,
     long_description_content_type = "text/markdown",
     license="Apache License 2.0",
```

