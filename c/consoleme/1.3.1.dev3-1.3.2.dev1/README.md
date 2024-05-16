# Comparing `tmp/consoleme-1.3.1.dev3.tar.gz` & `tmp/consoleme-1.3.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consoleme-1.3.1.dev3.tar", last modified: Mon May 13 17:19:53 2024, max compression
+gzip compressed data, was "consoleme-1.3.2.dev1.tar", last modified: Thu May 16 17:30:47 2024, max compression
```

## Comparing `consoleme-1.3.1.dev3.tar` & `consoleme-1.3.2.dev1.tar`

### file list

```diff
@@ -1,303 +1,303 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.369191 consoleme-1.3.1.dev3/
--rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-05-13 17:19:53.369191 consoleme-1.3.1.dev3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.301189 consoleme-1.3.1.dev3/cdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/app.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.301189 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.301189 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/consoleme_ecs_service_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/consoleme_spoke_accounts_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.305189 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/alb_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/auth_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/cache_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/compute_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/config_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/db_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/domain_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/iam_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/shared_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/vpc_stack.py
--rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.305189 consoleme-1.3.1.dev3/cdk/tests/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/cdk/tests/test_cdk.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.305189 consoleme-1.3.1.dev3/consoleme/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/babel.config.js
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/celery_tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/celery_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    86894 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/celery_tasks/celery_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/auth/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12702 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/auth/auth.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/aws/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    27051 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/aws/aws.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/celery_tasks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/celery_tasks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/celery_tasks/celery_tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/group_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/group_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/group_mapping/group_mapping.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.309189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/handlers/internal_demo_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/internal_routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.313189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/base_metric.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.313189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/cloudwatch/
--rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/cloudwatch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/default_metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.313189 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/policies/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/policies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/policies/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/default_plugins/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.313189 consoleme-1.3.1.dev3/consoleme/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/exceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/exceptions/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.313189 consoleme-1.3.1.dev3/consoleme/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    26952 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.313189 consoleme-1.3.1.dev3/consoleme/handlers/v1/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v1/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v1/headers.py
--rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v1/health.py
--rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v1/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v1/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v1/saml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.317190 consoleme-1.3.1.dev3/consoleme/handlers/v2/
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/audit.py
--rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/aws_iam_users.py
--rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/challenge.py
--rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/dynamic_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/generate_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/generate_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/index.py
--rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/logout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/managed_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    33629 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/resources.py
--rw-r--r--   0 runner    (1001) docker     (127)    25989 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/self_service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/service_control_policy.py
--rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/templated_resources.py
--rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/typeahead.py
--rw-r--r--   0 runner    (1001) docker     (127)    13172 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/handlers/v2/user_profile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.325190 consoleme-1.3.1.dev3/consoleme/lib/
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.325190 consoleme-1.3.1.dev3/consoleme/lib/account_indexers/
--rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/account_indexers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/account_indexers/aws_organizations.py
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/account_indexers/current_account.py
--rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/account_indexers/local_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/account_indexers/swag.py
--rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/alb_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/asyncio.py
--rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    81605 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/aws.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.325190 consoleme-1.3.1.dev3/consoleme/lib/aws_config/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/aws_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/aws_config/aws_config.py
--rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/aws_secret_manager.py
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/challenge.py
--rw-r--r--   0 runner    (1001) docker     (127)    18225 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/change_request.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.325190 consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/
--rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/dynamic_config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/internal_plugin.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/role_tags.py
--rw-r--r--   0 runner    (1001) docker     (127)    10464 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cloudtrail.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/cookie-py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/credential_auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/defaults.py
--rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/duo.py
--rw-r--r--   0 runner    (1001) docker     (127)    49019 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/dynamo.py
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/elasticsearch.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.325190 consoleme-1.3.1.dev3/consoleme/lib/event_bridge/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/event_bridge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/event_bridge/access_denies.py
--rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/event_bridge/role_updates.py
--rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/generic.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/git.py
--rw-r--r--   0 runner    (1001) docker     (127)    22017 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/google.py
--rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/groups.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/handler_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.325190 consoleme-1.3.1.dev3/consoleme/lib/notifications/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/notifications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/notifications/models.py
--rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/oidc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/password.py
--rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/plugins.py
--rw-r--r--   0 runner    (1001) docker     (127)    35445 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/policies.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/pydantic.py
--rw-r--r--   0 runner    (1001) docker     (127)    15893 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/redis.py
--rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/requests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/lib/role_updater/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/role_updater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/role_updater/cli.py
--rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/role_updater/handler.py
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/role_updater/schemas.py
--rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/s3_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/saml.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/lib/scm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/scm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/lib/scm/git/
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/scm/git/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/scm/git/bitbucket.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/lib/self_service/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/self_service/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/self_service/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/self_service/typeahead.py
--rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/ses.py
--rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/singleton.py
--rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/slack.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/lib/templated_resources/
--rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/templated_resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/templated_resources/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     8861 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/templated_resources/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/timeout.py
--rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/tracing.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/lib/v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/v2/aws_principals.py
--rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/v2/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)   121179 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/v2/requests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/v2/user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/web.py
--rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/lib/yaml.py
--rw-r--r--   0 runner    (1001) docker     (127)    26089 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/consoleme/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/templates/
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/asset-manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.297189 consoleme-1.3.1.dev3/consoleme/templates/images/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.329190 consoleme-1.3.1.dev3/consoleme/templates/images/logos/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.333190 consoleme-1.3.1.dev3/consoleme/templates/images/logos/infrasec/
--rw-r--r--   0 runner    (1001) docker     (127)  1780372 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/infrasec/DifferentGradient.png
--rw-r--r--   0 runner    (1001) docker     (127)   784262 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/infrasec/Honeybee.png
--rw-r--r--   0 runner    (1001) docker     (127)  1401997 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/infrasec/MikeCloudNoGradientWithFace.png
--rw-r--r--   0 runner    (1001) docker     (127)    32211 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/logo192.png
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/netflix-security-dark-bg-tight.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.337190 consoleme-1.3.1.dev3/consoleme/templates/images/logos/nosunglasses/
--rw-r--r--   0 runner    (1001) docker     (127)   353657 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/nosunglasses/1.png
--rw-r--r--   0 runner    (1001) docker     (127)   230322 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/nosunglasses/2.png
--rw-r--r--   0 runner    (1001) docker     (127)   243749 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/nosunglasses/3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.337190 consoleme-1.3.1.dev3/consoleme/templates/images/logos/quarantine/
--rw-r--r--   0 runner    (1001) docker     (127)   374928 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/quarantine/1.png
--rw-r--r--   0 runner    (1001) docker     (127)   387350 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/quarantine/2.png
--rw-r--r--   0 runner    (1001) docker     (127)   359457 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/quarantine/3.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.341190 consoleme-1.3.1.dev3/consoleme/templates/images/logos/sunglasses/
--rw-r--r--   0 runner    (1001) docker     (127)   375501 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/sunglasses/1.png
--rw-r--r--   0 runner    (1001) docker     (127)   347136 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/sunglasses/2.png
--rw-r--r--   0 runner    (1001) docker     (127)   362390 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/images/logos/sunglasses/3.png
--rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/index.html
--rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/manifest.json
--rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-13 17:19:06.000000 consoleme-1.3.1.dev3/consoleme/templates/robots.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.301189 consoleme-1.3.1.dev3/consoleme/templates/static/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.341190 consoleme-1.3.1.dev3/consoleme/templates/static/css/
--rw-r--r--   0 runner    (1001) docker     (127)   609522 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/css/main.463a8800.css
--rw-r--r--   0 runner    (1001) docker     (127)   904718 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/css/main.463a8800.css.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.349190 consoleme-1.3.1.dev3/consoleme/templates/static/js/
--rw-r--r--   0 runner    (1001) docker     (127)  2669634 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/js/main.903555c6.js
--rw-r--r--   0 runner    (1001) docker     (127)    68532 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/js/main.903555c6.js.LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)  8284688 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/js/main.903555c6.js.map
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.365191 consoleme-1.3.1.dev3/consoleme/templates/static/media/
--rw-r--r--   0 runner    (1001) docker     (127)    54488 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.278156e41e0ad908cf7f.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    98404 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.65a2fb6d9aaa164b41a0.ttf
--rw-r--r--   0 runner    (1001) docker     (127)   507628 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.6729d29753e000c17489.svg
--rw-r--r--   0 runner    (1001) docker     (127)    63728 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.cac87dc00c87a5d74711.woff
--rw-r--r--   0 runner    (1001) docker     (127)    98640 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.d68fa3e67dbb653a13ce.eot
--rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/flags.99f63ae7a743f21ab308.png
--rw-r--r--   0 runner    (1001) docker     (127)    40148 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.38c6d8bab26db77d8c80.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    50524 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.425399f81e4ce7cbd967.woff
--rw-r--r--   0 runner    (1001) docker     (127)   390837 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.62d9dae4e0040e81c980.svg
--rw-r--r--   0 runner    (1001) docker     (127)   106004 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.a01e3f2d6c83dc3aee17.eot
--rw-r--r--   0 runner    (1001) docker     (127)   105784 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.c656b8caa454ed19b9a2.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    30928 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.5367103510b27b784827.ttf
--rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.687a4990ea22bb1a49d4.woff2
--rw-r--r--   0 runner    (1001) docker     (127)    31156 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.752905fa5edf21fc52a1.eot
--rw-r--r--   0 runner    (1001) docker     (127)   107201 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.9c4845b4b41ef40a22fa.svg
--rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.ddae9b1ba9b0b42f5880.woff
--rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper1Active.9866ff3a1ea1cc7a93fa.svg
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper1Complete.6222088c914dcaffd0e4.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper2Active.b5befeb514c5ec2f9815.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper2Complete.47bfe6ee0ee7b0da663a.svg
--rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper2Pending.3aac534f4c215708e3eb.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper3Active.45f15c88d73d2a09105e.svg
--rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper3Pending.b72269cdc74f6782c021.svg
--rw-r--r--   0 runner    (1001) docker     (127)    15246 2024-05-13 17:19:48.000000 consoleme-1.3.1.dev3/consoleme/templates/static/media/warning.5b4ee25d2b57cd9f461e.png
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.369191 consoleme-1.3.1.dev3/consoleme.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-05-13 17:19:53.000000 consoleme-1.3.1.dev3/consoleme.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-05-13 17:19:53.000000 consoleme-1.3.1.dev3/consoleme.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:19:53.000000 consoleme-1.3.1.dev3/consoleme.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-13 17:19:53.000000 consoleme-1.3.1.dev3/consoleme.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 17:19:53.000000 consoleme-1.3.1.dev3/consoleme.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-13 17:19:53.000000 consoleme-1.3.1.dev3/consoleme.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 17:19:53.000000 consoleme-1.3.1.dev3/consoleme.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.365191 consoleme-1.3.1.dev3/scripts/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/scripts/initialize_dynamodb_oss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/scripts/initialize_redis_oss.py
--rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/scripts/retrieve_or_decode_configuration.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 17:19:53.369191 consoleme-1.3.1.dev3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.365191 consoleme-1.3.1.dev3/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.365191 consoleme-1.3.1.dev3/tests/celery/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/celery/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/celery/test_celery.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.365191 consoleme-1.3.1.dev3/tests/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/test_accessui.py
--rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/test_base.py
--rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/test_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/test_role_login_api.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/test_users.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 17:19:53.369191 consoleme-1.3.1.dev3/tests/handlers/v2/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_aws_iam_users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_errors.py
--rw-r--r--   0 runner    (1001) docker     (127)    25135 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_generate_changes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_policies.py
--rw-r--r--   0 runner    (1001) docker     (127)    38224 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_roles.py
--rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_typeahead.py
--rw-r--r--   0 runner    (1001) docker     (127)    10131 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/handlers/v2/test_user_profile.py
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-13 17:16:55.000000 consoleme-1.3.1.dev3/tests/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.210606 consoleme-1.3.2.dev1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11343 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-05-16 17:30:47.210606 consoleme-1.3.2.dev1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4527 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.134606 consoleme-1.3.2.dev1/cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/app.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.134606 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.134606 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/consoleme_ecs_service_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2260 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/consoleme_spoke_accounts_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.138605 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/alb_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4343 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/auth_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1302 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/cache_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/compute_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7345 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/config_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3595 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/db_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3748 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/domain_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8910 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/iam_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)      633 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/shared_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/vpc_stack.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1944 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.138605 consoleme-1.3.2.dev1/cdk/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1285 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/cdk/tests/test_cdk.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.138605 consoleme-1.3.2.dev1/consoleme/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/babel.config.js
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.138605 consoleme-1.3.2.dev1/consoleme/celery_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/celery_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    86894 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/celery_tasks/celery_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.142605 consoleme-1.3.2.dev1/consoleme/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14652 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.142605 consoleme-1.3.2.dev1/consoleme/default_plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.142605 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.142605 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12702 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/auth/auth.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.142605 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27051 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/aws/aws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.142605 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/celery_tasks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/celery_tasks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2488 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/celery_tasks/celery_tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.142605 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3421 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.142605 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/group_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/group_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7028 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/group_mapping/group_mapping.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.142605 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/internal_routes/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/internal_routes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.142605 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/internal_routes/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/internal_routes/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1297 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/internal_routes/handlers/internal_demo_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/internal_routes/internal_routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.146605 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/metrics/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/metrics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/metrics/base_metric.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.146605 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/metrics/cloudwatch/
+-rw-r--r--   0 runner    (1001) docker     (127)     2439 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/metrics/cloudwatch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/metrics/default_metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/metrics/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.146605 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/policies/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/policies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/policies/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1932 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/default_plugins/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.146605 consoleme-1.3.2.dev1/consoleme/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/exceptions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10377 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/exceptions/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.146605 consoleme-1.3.2.dev1/consoleme/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26952 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.146605 consoleme-1.3.2.dev1/consoleme/handlers/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23260 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v1/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2315 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v1/headers.py
+-rw-r--r--   0 runner    (1001) docker     (127)      474 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v1/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11978 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v1/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1916 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v1/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3203 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v1/saml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.150606 consoleme-1.3.2.dev1/consoleme/handlers/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4447 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/audit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5260 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/aws_iam_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13422 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4946 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/dynamic_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      809 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/generate_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1326 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/generate_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5986 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/index.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2397 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6005 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/managed_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5944 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33629 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8644 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25989 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/self_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1735 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/service_control_policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)      617 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/templated_resources.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6164 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/typeahead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13172 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5046 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/handlers/v2/user_profile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.162605 consoleme-1.3.2.dev1/consoleme/lib/
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.162605 consoleme-1.3.2.dev1/consoleme/lib/account_indexers/
+-rw-r--r--   0 runner    (1001) docker     (127)     4980 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/account_indexers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9554 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/account_indexers/aws_organizations.py
+-rw-r--r--   0 runner    (1001) docker     (127)      918 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/account_indexers/current_account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      934 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/account_indexers/local_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/account_indexers/swag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6453 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/alb_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1682 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/asyncio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11566 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    81605 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/aws.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.162605 consoleme-1.3.2.dev1/consoleme/lib/aws_config/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/aws_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4204 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/aws_config/aws_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      483 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/aws_secret_manager.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2289 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/challenge.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18225 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/change_request.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.162605 consoleme-1.3.2.dev1/consoleme/lib/cloud_credential_authorization_mapping/
+-rw-r--r--   0 runner    (1001) docker     (127)    11918 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/cloud_credential_authorization_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/cloud_credential_authorization_mapping/dynamic_config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/cloud_credential_authorization_mapping/internal_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/cloud_credential_authorization_mapping/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3833 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/cloud_credential_authorization_mapping/role_tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10464 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/cloudtrail.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/cookie-py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/credential_auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2072 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13539 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/defaults.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2286 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/duo.py
+-rw-r--r--   0 runner    (1001) docker     (127)    49019 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/dynamo.py
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/elasticsearch.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.162605 consoleme-1.3.2.dev1/consoleme/lib/event_bridge/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/event_bridge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9914 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/event_bridge/access_denies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4277 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/event_bridge/role_updates.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11368 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/generic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/git.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22017 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/google.py
+-rw-r--r--   0 runner    (1001) docker     (127)      820 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/groups.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/handler_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      570 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3612 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.162605 consoleme-1.3.2.dev1/consoleme/lib/notifications/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/notifications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4139 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/notifications/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12720 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/oidc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2166 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2031 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/plugins.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35445 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/pydantic.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15893 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/redis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9202 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/requests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.166606 consoleme-1.3.2.dev1/consoleme/lib/role_updater/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/role_updater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1197 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/role_updater/cli.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6381 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/role_updater/handler.py
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/role_updater/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7559 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/s3_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3832 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/saml.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.166606 consoleme-1.3.2.dev1/consoleme/lib/scm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/scm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.166606 consoleme-1.3.2.dev1/consoleme/lib/scm/git/
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/scm/git/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      927 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/scm/git/bitbucket.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.166606 consoleme-1.3.2.dev1/consoleme/lib/self_service/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/self_service/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/self_service/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6221 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/self_service/typeahead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13702 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/ses.py
+-rw-r--r--   0 runner    (1001) docker     (127)      344 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/singleton.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4820 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/slack.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.166606 consoleme-1.3.2.dev1/consoleme/lib/templated_resources/
+-rw-r--r--   0 runner    (1001) docker     (127)     9330 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/templated_resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/templated_resources/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9729 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/templated_resources/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      515 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/timeout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6710 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/tracing.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.166606 consoleme-1.3.2.dev1/consoleme/lib/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9280 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/v2/aws_principals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7490 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/v2/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)   121179 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/v2/requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2123 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/v2/user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1064 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/web.py
+-rw-r--r--   0 runner    (1001) docker     (127)      206 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/lib/yaml.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26089 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9064 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/consoleme/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.170606 consoleme-1.3.2.dev1/consoleme/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/asset-manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)    15086 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.130605 consoleme-1.3.2.dev1/consoleme/templates/images/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.170606 consoleme-1.3.2.dev1/consoleme/templates/images/logos/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.174605 consoleme-1.3.2.dev1/consoleme/templates/images/logos/infrasec/
+-rw-r--r--   0 runner    (1001) docker     (127)  1780372 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/images/logos/infrasec/DifferentGradient.png
+-rw-r--r--   0 runner    (1001) docker     (127)   784262 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/images/logos/infrasec/Honeybee.png
+-rw-r--r--   0 runner    (1001) docker     (127)  1401997 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/images/logos/infrasec/MikeCloudNoGradientWithFace.png
+-rw-r--r--   0 runner    (1001) docker     (127)    32211 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/images/logos/logo192.png
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/images/logos/netflix-security-dark-bg-tight.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.174605 consoleme-1.3.2.dev1/consoleme/templates/images/logos/nosunglasses/
+-rw-r--r--   0 runner    (1001) docker     (127)   353657 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/images/logos/nosunglasses/1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   230322 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/images/logos/nosunglasses/2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   243749 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/images/logos/nosunglasses/3.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.178606 consoleme-1.3.2.dev1/consoleme/templates/images/logos/quarantine/
+-rw-r--r--   0 runner    (1001) docker     (127)   374928 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/images/logos/quarantine/1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   387350 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/images/logos/quarantine/2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   359457 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/images/logos/quarantine/3.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.178606 consoleme-1.3.2.dev1/consoleme/templates/images/logos/sunglasses/
+-rw-r--r--   0 runner    (1001) docker     (127)   375501 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/images/logos/sunglasses/1.png
+-rw-r--r--   0 runner    (1001) docker     (127)   347136 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/images/logos/sunglasses/2.png
+-rw-r--r--   0 runner    (1001) docker     (127)   362390 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/images/logos/sunglasses/3.png
+-rw-r--r--   0 runner    (1001) docker     (127)      674 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/index.html
+-rw-r--r--   0 runner    (1001) docker     (127)      401 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/manifest.json
+-rw-r--r--   0 runner    (1001) docker     (127)       67 2024-05-16 17:30:01.000000 consoleme-1.3.2.dev1/consoleme/templates/robots.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.130605 consoleme-1.3.2.dev1/consoleme/templates/static/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.182606 consoleme-1.3.2.dev1/consoleme/templates/static/css/
+-rw-r--r--   0 runner    (1001) docker     (127)   609522 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/css/main.463a8800.css
+-rw-r--r--   0 runner    (1001) docker     (127)   904718 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/css/main.463a8800.css.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.186606 consoleme-1.3.2.dev1/consoleme/templates/static/js/
+-rw-r--r--   0 runner    (1001) docker     (127)  2669634 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/js/main.903555c6.js
+-rw-r--r--   0 runner    (1001) docker     (127)    68532 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/js/main.903555c6.js.LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)  8284688 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/js/main.903555c6.js.map
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.206606 consoleme-1.3.2.dev1/consoleme/templates/static/media/
+-rw-r--r--   0 runner    (1001) docker     (127)    54488 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/brand-icons.278156e41e0ad908cf7f.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    98404 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/brand-icons.65a2fb6d9aaa164b41a0.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)   507628 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/brand-icons.6729d29753e000c17489.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    63728 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/brand-icons.cac87dc00c87a5d74711.woff
+-rw-r--r--   0 runner    (1001) docker     (127)    98640 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/brand-icons.d68fa3e67dbb653a13ce.eot
+-rw-r--r--   0 runner    (1001) docker     (127)    28123 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/flags.99f63ae7a743f21ab308.png
+-rw-r--r--   0 runner    (1001) docker     (127)    40148 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/icons.38c6d8bab26db77d8c80.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    50524 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/icons.425399f81e4ce7cbd967.woff
+-rw-r--r--   0 runner    (1001) docker     (127)   390837 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/icons.62d9dae4e0040e81c980.svg
+-rw-r--r--   0 runner    (1001) docker     (127)   106004 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/icons.a01e3f2d6c83dc3aee17.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   105784 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/icons.c656b8caa454ed19b9a2.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    30928 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/outline-icons.5367103510b27b784827.ttf
+-rw-r--r--   0 runner    (1001) docker     (127)    12240 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/outline-icons.687a4990ea22bb1a49d4.woff2
+-rw-r--r--   0 runner    (1001) docker     (127)    31156 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/outline-icons.752905fa5edf21fc52a1.eot
+-rw-r--r--   0 runner    (1001) docker     (127)   107201 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/outline-icons.9c4845b4b41ef40a22fa.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    14712 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/outline-icons.ddae9b1ba9b0b42f5880.woff
+-rw-r--r--   0 runner    (1001) docker     (127)      585 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/stepper1Active.9866ff3a1ea1cc7a93fa.svg
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/stepper1Complete.6222088c914dcaffd0e4.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1613 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/stepper2Active.b5befeb514c5ec2f9815.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/stepper2Complete.47bfe6ee0ee7b0da663a.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     1539 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/stepper2Pending.3aac534f4c215708e3eb.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2241 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/stepper3Active.45f15c88d73d2a09105e.svg
+-rw-r--r--   0 runner    (1001) docker     (127)     2167 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/stepper3Pending.b72269cdc74f6782c021.svg
+-rw-r--r--   0 runner    (1001) docker     (127)    15246 2024-05-16 17:30:42.000000 consoleme-1.3.2.dev1/consoleme/templates/static/media/warning.5b4ee25d2b57cd9f461e.png
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.210606 consoleme-1.3.2.dev1/consoleme.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6572 2024-05-16 17:30:47.000000 consoleme-1.3.2.dev1/consoleme.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10238 2024-05-16 17:30:47.000000 consoleme-1.3.2.dev1/consoleme.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 17:30:47.000000 consoleme-1.3.2.dev1/consoleme.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-16 17:30:47.000000 consoleme-1.3.2.dev1/consoleme.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 17:30:47.000000 consoleme-1.3.2.dev1/consoleme.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-05-16 17:30:47.000000 consoleme-1.3.2.dev1/consoleme.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 17:30:47.000000 consoleme-1.3.2.dev1/consoleme.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.206606 consoleme-1.3.2.dev1/scripts/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8776 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/scripts/initialize_dynamodb_oss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3998 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/scripts/initialize_redis_oss.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3158 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/scripts/retrieve_or_decode_configuration.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 17:30:47.210606 consoleme-1.3.2.dev1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2812 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.206606 consoleme-1.3.2.dev1/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.206606 consoleme-1.3.2.dev1/tests/celery/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/celery/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/celery/test_celery.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.206606 consoleme-1.3.2.dev1/tests/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/test_accessui.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3449 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3075 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/test_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3299 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/test_role_login_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/test_users.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 17:30:47.210606 consoleme-1.3.2.dev1/tests/handlers/v2/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4912 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/v2/test_aws_iam_users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2931 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/v2/test_errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25135 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/v2/test_generate_changes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2298 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/v2/test_policies.py
+-rw-r--r--   0 runner    (1001) docker     (127)    38280 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/v2/test_requests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14007 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/v2/test_roles.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8553 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/v2/test_typeahead.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10131 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/v2/test_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3177 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/handlers/v2/test_user_profile.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-05-16 17:27:54.000000 consoleme-1.3.2.dev1/tests/test_main.py
```

### Comparing `consoleme-1.3.1.dev3/LICENSE` & `consoleme-1.3.2.dev1/LICENSE`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/PKG-INFO` & `consoleme-1.3.2.dev1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consoleme
-Version: 1.3.1.dev3
+Version: 1.3.2.dev1
 Summary: A central control plane for AWS permissions and access
 Home-page: https://github.com/Netflix/ConsoleMe
 Author: Netflix Security
 Author-email: consoleme-maintainers@netflix.com
 License: Apache 2.0
 Keywords: consoleme
 Requires-Python: >=3.8
```

### Comparing `consoleme-1.3.1.dev3/README.md` & `consoleme-1.3.2.dev1/README.md`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/app.py` & `consoleme-1.3.2.dev1/cdk/app.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/consoleme_ecs_service_stack.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/consoleme_ecs_service_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/consoleme_spoke_accounts_stack.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/consoleme_spoke_accounts_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/constants.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/constants.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/helpers.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/helpers.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/alb_stack.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/alb_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/auth_stack.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/auth_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/cache_stack.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/cache_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/compute_stack.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/compute_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/config_stack.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/config_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/db_stack.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/db_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/domain_stack.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/domain_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/iam_stack.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/iam_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/shared_stack.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/shared_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/service/nested_stacks/vpc_stack.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/service/nested_stacks/vpc_stack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/consoleme_ecs_cdk/setup.py` & `consoleme-1.3.2.dev1/cdk/consoleme_ecs_cdk/setup.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/cdk/tests/test_cdk.py` & `consoleme-1.3.2.dev1/cdk/tests/test_cdk.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/__main__.py` & `consoleme-1.3.2.dev1/consoleme/__main__.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/celery_tasks/celery_tasks.py` & `consoleme-1.3.2.dev1/consoleme/celery_tasks/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/config/config.py` & `consoleme-1.3.2.dev1/consoleme/config/config.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/auth/auth.py` & `consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/auth/auth.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/aws/aws.py` & `consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/aws/aws.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/celery_tasks/celery_tasks.py` & `consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/celery_tasks/celery_tasks.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/config/config.py` & `consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/config/config.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/group_mapping/group_mapping.py` & `consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/group_mapping/group_mapping.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/handlers/internal_demo_route.py` & `consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/internal_routes/handlers/internal_demo_route.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/internal_routes/internal_routes.py` & `consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/internal_routes/internal_routes.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/cloudwatch/__init__.py` & `consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/metrics/cloudwatch/__init__.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/metrics/default_metrics.py` & `consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/metrics/default_metrics.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/default_plugins/plugins/policies/policies.py` & `consoleme-1.3.2.dev1/consoleme/default_plugins/plugins/policies/policies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/default_plugins/setup.py` & `consoleme-1.3.2.dev1/consoleme/default_plugins/setup.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/exceptions/exceptions.py` & `consoleme-1.3.2.dev1/consoleme/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/auth.py` & `consoleme-1.3.2.dev1/consoleme/handlers/auth.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/base.py` & `consoleme-1.3.2.dev1/consoleme/handlers/base.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v1/credentials.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v1/credentials.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v1/headers.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v1/headers.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v1/policies.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v1/policies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v1/roles.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v1/roles.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v1/saml.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v1/saml.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/audit.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/audit.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/aws_iam_users.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/aws_iam_users.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/challenge.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/challenge.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/dynamic_config.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/errors.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/errors.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/generate_changes.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/generate_changes.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/generate_policy.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/generate_policy.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/index.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/index.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/logout.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/logout.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/managed_policies.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/managed_policies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/notifications.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/notifications.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/policies.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/policies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/requests.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/requests.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/resources.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/resources.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/roles.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/roles.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/self_service.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/self_service.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/service_control_policy.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/service_control_policy.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/templated_resources.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/templated_resources.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/typeahead.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/typeahead.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/user.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/user.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/handlers/v2/user_profile.py` & `consoleme-1.3.2.dev1/consoleme/handlers/v2/user_profile.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/account_indexers/__init__.py` & `consoleme-1.3.2.dev1/consoleme/lib/account_indexers/__init__.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/account_indexers/aws_organizations.py` & `consoleme-1.3.2.dev1/consoleme/lib/account_indexers/aws_organizations.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/account_indexers/current_account.py` & `consoleme-1.3.2.dev1/consoleme/lib/account_indexers/current_account.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/account_indexers/local_config.py` & `consoleme-1.3.2.dev1/consoleme/lib/account_indexers/local_config.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/account_indexers/swag.py` & `consoleme-1.3.2.dev1/consoleme/lib/account_indexers/swag.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/alb_auth.py` & `consoleme-1.3.2.dev1/consoleme/lib/alb_auth.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/asyncio.py` & `consoleme-1.3.2.dev1/consoleme/lib/asyncio.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/auth.py` & `consoleme-1.3.2.dev1/consoleme/lib/auth.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/aws.py` & `consoleme-1.3.2.dev1/consoleme/lib/aws.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/aws_config/aws_config.py` & `consoleme-1.3.2.dev1/consoleme/lib/aws_config/aws_config.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/cache.py` & `consoleme-1.3.2.dev1/consoleme/lib/cache.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/challenge.py` & `consoleme-1.3.2.dev1/consoleme/lib/challenge.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/change_request.py` & `consoleme-1.3.2.dev1/consoleme/lib/change_request.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/__init__.py` & `consoleme-1.3.2.dev1/consoleme/lib/cloud_credential_authorization_mapping/__init__.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/dynamic_config.py` & `consoleme-1.3.2.dev1/consoleme/lib/cloud_credential_authorization_mapping/dynamic_config.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/internal_plugin.py` & `consoleme-1.3.2.dev1/consoleme/lib/cloud_credential_authorization_mapping/internal_plugin.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/models.py` & `consoleme-1.3.2.dev1/consoleme/lib/cloud_credential_authorization_mapping/models.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/cloud_credential_authorization_mapping/role_tags.py` & `consoleme-1.3.2.dev1/consoleme/lib/cloud_credential_authorization_mapping/role_tags.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/cloudtrail.py` & `consoleme-1.3.2.dev1/consoleme/lib/cloudtrail.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/credential_auth.py` & `consoleme-1.3.2.dev1/consoleme/lib/credential_auth.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/crypto.py` & `consoleme-1.3.2.dev1/consoleme/lib/crypto.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/defaults.py` & `consoleme-1.3.2.dev1/consoleme/lib/defaults.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/duo.py` & `consoleme-1.3.2.dev1/consoleme/lib/duo.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/dynamo.py` & `consoleme-1.3.2.dev1/consoleme/lib/dynamo.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/elasticsearch.py` & `consoleme-1.3.2.dev1/consoleme/lib/elasticsearch.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/event_bridge/access_denies.py` & `consoleme-1.3.2.dev1/consoleme/lib/event_bridge/access_denies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/event_bridge/role_updates.py` & `consoleme-1.3.2.dev1/consoleme/lib/event_bridge/role_updates.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/generic.py` & `consoleme-1.3.2.dev1/consoleme/lib/generic.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/git.py` & `consoleme-1.3.2.dev1/consoleme/lib/git.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/google.py` & `consoleme-1.3.2.dev1/consoleme/lib/google.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/groups.py` & `consoleme-1.3.2.dev1/consoleme/lib/groups.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/handler_utils.py` & `consoleme-1.3.2.dev1/consoleme/lib/handler_utils.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/json_encoder.py` & `consoleme-1.3.2.dev1/consoleme/lib/json_encoder.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/jwt.py` & `consoleme-1.3.2.dev1/consoleme/lib/jwt.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/loader.py` & `consoleme-1.3.2.dev1/consoleme/lib/loader.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/notifications/models.py` & `consoleme-1.3.2.dev1/consoleme/lib/notifications/models.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/oidc.py` & `consoleme-1.3.2.dev1/consoleme/lib/oidc.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/password.py` & `consoleme-1.3.2.dev1/consoleme/lib/password.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/plugins.py` & `consoleme-1.3.2.dev1/consoleme/lib/plugins.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/policies.py` & `consoleme-1.3.2.dev1/consoleme/lib/policies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/redis.py` & `consoleme-1.3.2.dev1/consoleme/lib/redis.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/requests.py` & `consoleme-1.3.2.dev1/consoleme/lib/requests.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/role_updater/cli.py` & `consoleme-1.3.2.dev1/consoleme/lib/role_updater/cli.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/role_updater/handler.py` & `consoleme-1.3.2.dev1/consoleme/lib/role_updater/handler.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/role_updater/schemas.py` & `consoleme-1.3.2.dev1/consoleme/lib/role_updater/schemas.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/s3_helpers.py` & `consoleme-1.3.2.dev1/consoleme/lib/s3_helpers.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/saml.py` & `consoleme-1.3.2.dev1/consoleme/lib/saml.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/scm/git/__init__.py` & `consoleme-1.3.2.dev1/consoleme/lib/scm/git/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -23,14 +23,15 @@
             args.append("-n")
         args.append(self.repo_url)
         if depth:
             kwargs["depth"] = depth
         await sync_to_async(git.Git(self.tempdir).clone)(*args, **kwargs)
         self.repo = git.Repo(os.path.join(self.tempdir, self.repo_name))
         self.repo.config_writer().set_value("user", "name", "ConsoleMe").release()
+        self.repo.config_writer().set_value("core", "symlinks", "false").release()
         if self.git_email:
             self.repo.config_writer().set_value(
                 "user", "email", self.git_email
             ).release()
         self.git = self.repo.git
         return self.repo
```

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/scm/git/bitbucket.py` & `consoleme-1.3.2.dev1/consoleme/lib/scm/git/bitbucket.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/self_service/models.py` & `consoleme-1.3.2.dev1/consoleme/lib/self_service/models.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/self_service/typeahead.py` & `consoleme-1.3.2.dev1/consoleme/lib/self_service/typeahead.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/ses.py` & `consoleme-1.3.2.dev1/consoleme/lib/ses.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/slack.py` & `consoleme-1.3.2.dev1/consoleme/lib/slack.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/templated_resources/__init__.py` & `consoleme-1.3.2.dev1/consoleme/lib/templated_resources/__init__.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/templated_resources/models.py` & `consoleme-1.3.2.dev1/consoleme/lib/templated_resources/models.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/templated_resources/requests.py` & `consoleme-1.3.2.dev1/consoleme/lib/templated_resources/requests.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,12 @@
 import io
 import json
+import os
+import random
+import string
 import time
 
 from ruamel.yaml.comments import CommentedSeq
 
 from consoleme.config import config
 from consoleme.lib.aws import minimize_iam_policy_statements
 from consoleme.lib.plugins import get_plugin_by_name
@@ -26,15 +29,18 @@
 
 async def generate_honeybee_request_from_change_model_array(
     request_creation: RequestCreationModel, user: str, extended_request_uuid: str
 ) -> ExtendedRequestModel:
     repositories_for_request = {}
     primary_principal = None
     t = int(time.time())
-    generated_branch_name = f"{user}-{t}"
+    suffix = "".join(
+        random.choices(string.ascii_lowercase + string.digits, k=10)  # nosec
+    )
+    generated_branch_name = f"{user}-{t}-{suffix}"
     policy_name = config.get(
         "generate_honeybee_request_from_change_model_array.policy_name",
         "self_service_generated",
     )
     repo_config = None
 
     # Checkout Git Repo and generate a branch name for the user's change
@@ -74,18 +80,34 @@
         git_client = repositories_for_request[change.principal.repository_name][
             "git_client"
         ]
         repo = repositories_for_request[change.principal.repository_name]["repo"].repo
         main_branch_name = repositories_for_request[change.principal.repository_name][
             "main_branch_name"
         ]
-        git_client.checkout(
-            f"origin/{main_branch_name}", change.principal.resource_identifier
+
+        change_file_path = os.path.abspath(
+            f"{repo.working_dir}/{change.principal.resource_identifier}"
         )
-        change_file_path = f"{repo.working_dir}/{change.principal.resource_identifier}"
+        clone_wd_path = os.path.abspath(repo.working_dir)
+        if os.path.commonprefix((clone_wd_path, change_file_path)) != clone_wd_path:
+            log.exception(
+                f"User attempted to reference a file outside of the repository: {change_file_path} is not within {clone_wd_path}"
+            )
+            raise ValueError("Unable to raise change request for this resource")
+
+        try:
+            git_client.checkout(
+                f"origin/{main_branch_name}", "--", change.principal.resource_identifier
+            )
+        except Exception:
+            log.exception(
+                f"Unable to checkout {main_branch_name} for {change.principal.resource_identifier}"
+            )
+            raise ValueError("Unable to raise change request for this resource")
         with open(change_file_path, "r") as f:
             yaml_content = yaml.load(f)
 
         # Original
         buf = io.BytesIO()
         yaml.dump(yaml_content, buf)
         original_text = buf.getvalue()
```

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/timeout.py` & `consoleme-1.3.2.dev1/consoleme/lib/timeout.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/tracing.py` & `consoleme-1.3.2.dev1/consoleme/lib/tracing.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/v2/aws_principals.py` & `consoleme-1.3.2.dev1/consoleme/lib/v2/aws_principals.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/v2/notifications.py` & `consoleme-1.3.2.dev1/consoleme/lib/v2/notifications.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/v2/requests.py` & `consoleme-1.3.2.dev1/consoleme/lib/v2/requests.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/v2/user_profile.py` & `consoleme-1.3.2.dev1/consoleme/lib/v2/user_profile.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/lib/web.py` & `consoleme-1.3.2.dev1/consoleme/lib/web.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/models.py` & `consoleme-1.3.2.dev1/consoleme/models.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/routes.py` & `consoleme-1.3.2.dev1/consoleme/routes.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/asset-manifest.json` & `consoleme-1.3.2.dev1/consoleme/templates/asset-manifest.json`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/favicon.ico` & `consoleme-1.3.2.dev1/consoleme/templates/favicon.ico`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/images/logos/infrasec/DifferentGradient.png` & `consoleme-1.3.2.dev1/consoleme/templates/images/logos/infrasec/DifferentGradient.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/images/logos/infrasec/Honeybee.png` & `consoleme-1.3.2.dev1/consoleme/templates/images/logos/infrasec/Honeybee.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/images/logos/infrasec/MikeCloudNoGradientWithFace.png` & `consoleme-1.3.2.dev1/consoleme/templates/images/logos/infrasec/MikeCloudNoGradientWithFace.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/images/logos/logo192.png` & `consoleme-1.3.2.dev1/consoleme/templates/images/logos/logo192.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/images/logos/netflix-security-dark-bg-tight.svg` & `consoleme-1.3.2.dev1/consoleme/templates/images/logos/netflix-security-dark-bg-tight.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/images/logos/nosunglasses/1.png` & `consoleme-1.3.2.dev1/consoleme/templates/images/logos/nosunglasses/1.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/images/logos/nosunglasses/2.png` & `consoleme-1.3.2.dev1/consoleme/templates/images/logos/nosunglasses/2.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/images/logos/nosunglasses/3.png` & `consoleme-1.3.2.dev1/consoleme/templates/images/logos/nosunglasses/3.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/images/logos/quarantine/1.png` & `consoleme-1.3.2.dev1/consoleme/templates/images/logos/quarantine/1.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/images/logos/quarantine/2.png` & `consoleme-1.3.2.dev1/consoleme/templates/images/logos/quarantine/2.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/images/logos/quarantine/3.png` & `consoleme-1.3.2.dev1/consoleme/templates/images/logos/quarantine/3.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/images/logos/sunglasses/1.png` & `consoleme-1.3.2.dev1/consoleme/templates/images/logos/sunglasses/1.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/images/logos/sunglasses/2.png` & `consoleme-1.3.2.dev1/consoleme/templates/images/logos/sunglasses/2.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/images/logos/sunglasses/3.png` & `consoleme-1.3.2.dev1/consoleme/templates/images/logos/sunglasses/3.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/index.html` & `consoleme-1.3.2.dev1/consoleme/templates/index.html`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/css/main.463a8800.css` & `consoleme-1.3.2.dev1/consoleme/templates/static/css/main.463a8800.css`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/css/main.463a8800.css.map` & `consoleme-1.3.2.dev1/consoleme/templates/static/css/main.463a8800.css.map`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/js/main.903555c6.js` & `consoleme-1.3.2.dev1/consoleme/templates/static/js/main.903555c6.js`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/js/main.903555c6.js.LICENSE.txt` & `consoleme-1.3.2.dev1/consoleme/templates/static/js/main.903555c6.js.LICENSE.txt`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/js/main.903555c6.js.map` & `consoleme-1.3.2.dev1/consoleme/templates/static/js/main.903555c6.js.map`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.278156e41e0ad908cf7f.woff2` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/brand-icons.278156e41e0ad908cf7f.woff2`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.65a2fb6d9aaa164b41a0.ttf` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/brand-icons.65a2fb6d9aaa164b41a0.ttf`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.6729d29753e000c17489.svg` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/brand-icons.6729d29753e000c17489.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.cac87dc00c87a5d74711.woff` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/brand-icons.cac87dc00c87a5d74711.woff`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/brand-icons.d68fa3e67dbb653a13ce.eot` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/brand-icons.d68fa3e67dbb653a13ce.eot`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/flags.99f63ae7a743f21ab308.png` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/flags.99f63ae7a743f21ab308.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.38c6d8bab26db77d8c80.woff2` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/icons.38c6d8bab26db77d8c80.woff2`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.425399f81e4ce7cbd967.woff` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/icons.425399f81e4ce7cbd967.woff`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.62d9dae4e0040e81c980.svg` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/icons.62d9dae4e0040e81c980.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.a01e3f2d6c83dc3aee17.eot` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/icons.a01e3f2d6c83dc3aee17.eot`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/icons.c656b8caa454ed19b9a2.ttf` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/icons.c656b8caa454ed19b9a2.ttf`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.5367103510b27b784827.ttf` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/outline-icons.5367103510b27b784827.ttf`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.687a4990ea22bb1a49d4.woff2` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/outline-icons.687a4990ea22bb1a49d4.woff2`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.752905fa5edf21fc52a1.eot` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/outline-icons.752905fa5edf21fc52a1.eot`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.9c4845b4b41ef40a22fa.svg` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/outline-icons.9c4845b4b41ef40a22fa.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/outline-icons.ddae9b1ba9b0b42f5880.woff` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/outline-icons.ddae9b1ba9b0b42f5880.woff`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper1Active.9866ff3a1ea1cc7a93fa.svg` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/stepper1Active.9866ff3a1ea1cc7a93fa.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper1Complete.6222088c914dcaffd0e4.svg` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/stepper1Complete.6222088c914dcaffd0e4.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper2Active.b5befeb514c5ec2f9815.svg` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/stepper2Active.b5befeb514c5ec2f9815.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper2Complete.47bfe6ee0ee7b0da663a.svg` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/stepper2Complete.47bfe6ee0ee7b0da663a.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper2Pending.3aac534f4c215708e3eb.svg` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/stepper2Pending.3aac534f4c215708e3eb.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper3Active.45f15c88d73d2a09105e.svg` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/stepper3Active.45f15c88d73d2a09105e.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/stepper3Pending.b72269cdc74f6782c021.svg` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/stepper3Pending.b72269cdc74f6782c021.svg`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme/templates/static/media/warning.5b4ee25d2b57cd9f461e.png` & `consoleme-1.3.2.dev1/consoleme/templates/static/media/warning.5b4ee25d2b57cd9f461e.png`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme.egg-info/PKG-INFO` & `consoleme-1.3.2.dev1/consoleme.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consoleme
-Version: 1.3.1.dev3
+Version: 1.3.2.dev1
 Summary: A central control plane for AWS permissions and access
 Home-page: https://github.com/Netflix/ConsoleMe
 Author: Netflix Security
 Author-email: consoleme-maintainers@netflix.com
 License: Apache 2.0
 Keywords: consoleme
 Requires-Python: >=3.8
```

### Comparing `consoleme-1.3.1.dev3/consoleme.egg-info/SOURCES.txt` & `consoleme-1.3.2.dev1/consoleme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme.egg-info/entry_points.txt` & `consoleme-1.3.2.dev1/consoleme.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/consoleme.egg-info/requires.txt` & `consoleme-1.3.2.dev1/consoleme.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/scripts/initialize_dynamodb_oss.py` & `consoleme-1.3.2.dev1/scripts/initialize_dynamodb_oss.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/scripts/initialize_redis_oss.py` & `consoleme-1.3.2.dev1/scripts/initialize_redis_oss.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/scripts/retrieve_or_decode_configuration.py` & `consoleme-1.3.2.dev1/scripts/retrieve_or_decode_configuration.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/setup.py` & `consoleme-1.3.2.dev1/setup.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/tests/celery/test_celery.py` & `consoleme-1.3.2.dev1/tests/celery/test_celery.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/tests/handlers/test_base.py` & `consoleme-1.3.2.dev1/tests/handlers/test_base.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/tests/handlers/test_policies.py` & `consoleme-1.3.2.dev1/tests/handlers/test_policies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/tests/handlers/test_role_login_api.py` & `consoleme-1.3.2.dev1/tests/handlers/test_role_login_api.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/tests/handlers/v2/test_aws_iam_users.py` & `consoleme-1.3.2.dev1/tests/handlers/v2/test_aws_iam_users.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/tests/handlers/v2/test_errors.py` & `consoleme-1.3.2.dev1/tests/handlers/v2/test_errors.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/tests/handlers/v2/test_generate_changes.py` & `consoleme-1.3.2.dev1/tests/handlers/v2/test_generate_changes.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/tests/handlers/v2/test_policies.py` & `consoleme-1.3.2.dev1/tests/handlers/v2/test_policies.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/tests/handlers/v2/test_requests.py` & `consoleme-1.3.2.dev1/tests/handlers/v2/test_requests.py`

 * *Files 0% similar despite different names*

```diff
@@ -714,14 +714,15 @@
       - Action:
           - '*'
         Effect: Allow
         Resource:
           - '*'
         Sid: admin"""
         with patch("builtins.open", mock_open(read_data=template_data)):
+            mock_repo.return_value.working_dir = "/tmp"
             response = self.fetch(
                 "/api/v2/request",
                 method="POST",
                 headers=headers,
                 body=json.dumps(input_body),
             )
             result = json.loads(response.body)
```

### Comparing `consoleme-1.3.1.dev3/tests/handlers/v2/test_roles.py` & `consoleme-1.3.2.dev1/tests/handlers/v2/test_roles.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/tests/handlers/v2/test_typeahead.py` & `consoleme-1.3.2.dev1/tests/handlers/v2/test_typeahead.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/tests/handlers/v2/test_user.py` & `consoleme-1.3.2.dev1/tests/handlers/v2/test_user.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/tests/handlers/v2/test_user_profile.py` & `consoleme-1.3.2.dev1/tests/handlers/v2/test_user_profile.py`

 * *Files identical despite different names*

### Comparing `consoleme-1.3.1.dev3/tests/test_main.py` & `consoleme-1.3.2.dev1/tests/test_main.py`

 * *Files identical despite different names*

