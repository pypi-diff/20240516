# Comparing `tmp/cocnc-0.1.0.tar.gz` & `tmp/cocnc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocnc-0.1.0.tar", max compression
+gzip compressed data, was "cocnc-0.1.1.tar", max compression
```

## Comparing `cocnc-0.1.0.tar` & `cocnc-0.1.1.tar`

### file list

```diff
@@ -1,173 +1,174 @@
--rw-r--r--   0        0        0    35148 2024-04-02 18:10:45.243229 cocnc-0.1.0/LICENSE.txt
--rw-r--r--   0        0        0     5010 2024-05-14 18:02:38.218930 cocnc-0.1.0/README.md
--rw-r--r--   0        0        0      945 2024-05-14 19:41:16.994892 cocnc-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      199 2024-05-12 00:57:28.450735 cocnc-0.1.0/src/cnc/__init__.py
--rw-r--r--   0        0        0      498 2024-05-12 00:57:28.450735 cocnc-0.1.0/src/cnc/check_dependencies.py
--rw-r--r--   0        0        0        0 2024-04-02 18:10:45.243229 cocnc-0.1.0/src/cnc/commands/__init__.py
--rw-r--r--   0        0        0     1312 2024-05-14 18:02:38.222930 cocnc-0.1.0/src/cnc/commands/build.py
--rw-r--r--   0        0        0     1266 2024-05-14 18:02:38.222930 cocnc-0.1.0/src/cnc/commands/deploy.py
--rw-r--r--   0        0        0     1438 2024-05-14 18:02:38.222930 cocnc-0.1.0/src/cnc/commands/info.py
--rw-r--r--   0        0        0     4136 2024-05-12 00:57:28.450735 cocnc-0.1.0/src/cnc/commands/provision.py
--rw-r--r--   0        0        0      753 2024-05-12 00:57:28.450735 cocnc-0.1.0/src/cnc/commands/render.py
--rw-r--r--   0        0        0      663 2024-04-02 18:10:45.243229 cocnc-0.1.0/src/cnc/commands/shell.py
--rw-r--r--   0        0        0      928 2024-05-12 00:57:28.450735 cocnc-0.1.0/src/cnc/commands/telemetry.py
--rw-r--r--   0        0        0        0 2024-04-02 18:10:45.247229 cocnc-0.1.0/src/cnc/commands/template_editor/__init__.py
--rw-r--r--   0        0        0     5650 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/commands/template_editor/inspector.py
--rw-r--r--   0        0        0     2937 2024-05-14 19:09:45.170904 cocnc-0.1.0/src/cnc/commands/toolbox.py
--rw-r--r--   0        0        0      739 2024-04-02 18:10:45.247229 cocnc-0.1.0/src/cnc/constants.py
--rw-r--r--   0        0        0     3780 2024-05-10 01:36:08.673102 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/build/build_functions.sh.j2
--rw-r--r--   0        0        0      789 2024-04-26 14:43:08.886875 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/build/main.sh.j2
--rw-r--r--   0        0        0       43 2024-04-02 18:10:45.247229 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/deploy_functions.sh.j2
--rw-r--r--   0        0        0     2694 2024-05-12 00:57:28.450735 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/ecs_web_task.json.j2
--rw-r--r--   0        0        0     1257 2024-05-01 01:07:56.387004 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/main.sh.j2
--rw-r--r--   0        0        0     1623 2024-05-01 01:07:56.387004 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy.sh.j2
--rw-r--r--   0        0        0     2468 2024-05-01 01:07:56.387004 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy_status_check.sh.j2
--rw-r--r--   0        0        0      766 2024-04-26 14:43:08.898875 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/partials/ecs_wait_with_retries.sh.j2
--rw-r--r--   0        0        0      645 2024-05-01 01:07:56.387004 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/partials/update_task_definition.sh.j2
--rw-r--r--   0        0        0      200 2024-05-01 01:07:56.387004 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy.sh.j2
--rw-r--r--   0        0        0     1047 2024-05-01 01:07:56.387004 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy_functions.sh.j2
--rw-r--r--   0        0        0     1478 2024-05-03 17:48:33.699163 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/base.tf.j2
--rw-r--r--   0        0        0      396 2024-04-02 18:10:45.247229 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/frontend_routing_lambda/index.js
--rw-r--r--   0        0        0      561 2024-04-26 14:43:08.902875 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/main.tf.j2
--rw-r--r--   0        0        0     4651 2024-04-26 14:43:08.902875 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/active_and_paused_envs.tf.j2
--rw-r--r--   0        0        0     5481 2024-04-26 14:43:08.906875 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_backend_deployments.tf.j2
--rw-r--r--   0        0        0     5640 2024-04-26 14:43:08.906875 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_deployments.tf.j2
--rw-r--r--   0        0        0     1759 2024-05-01 01:07:56.387004 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_frontend_deployments.tf.j2
--rw-r--r--   0        0        0    11529 2024-04-26 14:43:08.910875 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_backend_services.tf.j2
--rw-r--r--   0        0        0      813 2024-05-12 00:57:28.450735 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/collection/providers.tf.j2
--rw-r--r--   0        0        0     8800 2024-05-08 16:39:58.931845 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/collection/vpc_configuration.tf.j2
--rw-r--r--   0        0        0     1888 2024-05-12 00:57:28.450735 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/collection_level_resources.tf.j2
--rw-r--r--   0        0        0     1432 2024-04-26 14:43:08.918875 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/environment/efs.tf.j2
--rw-r--r--   0        0        0     1886 2024-04-02 18:10:45.251229 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/environment/msg_queue_and_obj_storage.tf.j2
--rw-r--r--   0        0        0    26090 2024-05-01 01:07:56.391004 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/environment_level_resources.tf.j2
--rw-r--r--   0        0        0     9699 2024-05-01 01:07:56.391004 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_backend.tf.j2
--rw-r--r--   0        0        0     6430 2024-04-26 14:43:08.922875 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_frontend.tf.j2
--rw-r--r--   0        0        0     2382 2024-05-01 01:07:56.391004 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/scheduled_tasks.tf.j2
--rw-r--r--   0        0        0     5446 2024-05-01 01:07:56.391004 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/workers.tf.j2
--rw-r--r--   0        0        0      965 2024-04-26 14:43:08.926875 cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/service_level_resources.tf.j2
--rw-r--r--   0        0        0    11323 2024-05-12 00:57:28.450735 cocnc-0.1.0/src/cnc/flavors/aws/shared/deploy/deploy_functions_base.sh.j2
--rw-r--r--   0        0        0      336 2024-05-10 01:36:08.677103 cocnc-0.1.0/src/cnc/flavors/aws/shared/toolbox/Dockerfile.j2
--rw-r--r--   0        0        0     4184 2024-05-01 01:07:56.391004 cocnc-0.1.0/src/cnc/flavors/aws/shared/toolbox/main.sh.j2
--rw-r--r--   0        0        0      615 2024-04-02 18:10:45.251229 cocnc-0.1.0/src/cnc/flavors/gcp/gke/1/deploy/deploy.sh.j2
--rw-r--r--   0        0        0      290 2024-04-26 14:43:08.930875 cocnc-0.1.0/src/cnc/flavors/gcp/gke/1/deploy/deploy_functions.sh.j2
--rw-r--r--   0        0        0     1953 2024-04-26 14:43:08.930875 cocnc-0.1.0/src/cnc/flavors/gcp/gke/1/provision/base.tf.j2
--rw-r--r--   0        0        0      561 2024-04-26 14:43:08.930875 cocnc-0.1.0/src/cnc/flavors/gcp/gke/1/provision/main.tf.j2
--rw-r--r--   0        0        0     1189 2024-04-26 14:43:08.930875 cocnc-0.1.0/src/cnc/flavors/gcp/gke/1/provision/partials/collection_level_resources.tf.j2
--rw-r--r--   0        0        0     4347 2024-04-26 14:43:08.930875 cocnc-0.1.0/src/cnc/flavors/gcp/gke/1/provision/partials/service_level_resources.tf.j2
--rw-r--r--   0        0        0      299 2024-04-02 18:10:45.251229 cocnc-0.1.0/src/cnc/flavors/gcp/run/1/build/main.sh.j2
--rw-r--r--   0        0        0      104 2024-04-02 18:10:45.251229 cocnc-0.1.0/src/cnc/flavors/gcp/run/1/cnc-flavor.yml
--rw-r--r--   0        0        0      661 2024-04-26 14:43:08.934875 cocnc-0.1.0/src/cnc/flavors/gcp/run/1/deploy/base.sh.j2
--rw-r--r--   0        0        0       43 2024-04-02 18:10:45.255229 cocnc-0.1.0/src/cnc/flavors/gcp/run/1/deploy/deploy_functions.sh.j2
--rw-r--r--   0        0        0      303 2024-04-02 18:10:45.255229 cocnc-0.1.0/src/cnc/flavors/gcp/run/1/deploy/main.sh.j2
--rw-r--r--   0        0        0     2512 2024-05-03 17:48:33.699163 cocnc-0.1.0/src/cnc/flavors/gcp/run/1/provision/base.tf.j2
--rw-r--r--   0        0        0      561 2024-04-26 14:43:08.934875 cocnc-0.1.0/src/cnc/flavors/gcp/run/1/provision/main.tf.j2
--rw-r--r--   0        0        0      299 2024-04-26 14:43:08.930875 cocnc-0.1.0/src/cnc/flavors/gcp/run-lite/1/build/main.sh.j2
--rw-r--r--   0        0        0      493 2024-04-26 14:43:08.934875 cocnc-0.1.0/src/cnc/flavors/gcp/run-lite/1/deploy/base.sh.j2
--rw-r--r--   0        0        0      331 2024-04-26 14:43:08.934875 cocnc-0.1.0/src/cnc/flavors/gcp/run-lite/1/deploy/deploy_functions.sh.j2
--rw-r--r--   0        0        0      303 2024-04-26 14:43:08.934875 cocnc-0.1.0/src/cnc/flavors/gcp/run-lite/1/deploy/main.sh.j2
--rw-r--r--   0        0        0     1778 2024-05-10 01:36:08.677103 cocnc-0.1.0/src/cnc/flavors/gcp/run-lite/1/deploy/run-container.yml.j2
--rw-r--r--   0        0        0     1364 2024-04-26 20:51:50.243437 cocnc-0.1.0/src/cnc/flavors/gcp/run-lite/1/provision/base.tf.j2
--rw-r--r--   0        0        0      561 2024-04-26 14:43:08.934875 cocnc-0.1.0/src/cnc/flavors/gcp/run-lite/1/provision/main.tf.j2
--rw-r--r--   0        0        0     1926 2024-05-01 01:07:56.391004 cocnc-0.1.0/src/cnc/flavors/gcp/run-lite/1/toolbox/main.sh.j2
--rw-r--r--   0        0        0      273 2024-05-01 01:07:56.391004 cocnc-0.1.0/src/cnc/flavors/gcp/shared/build/Dockerfile.run.j2
--rw-r--r--   0        0        0     1017 2024-05-01 01:07:56.391004 cocnc-0.1.0/src/cnc/flavors/gcp/shared/build/base.sh.j2
--rw-r--r--   0        0        0     4441 2024-05-11 13:31:17.231066 cocnc-0.1.0/src/cnc/flavors/gcp/shared/build/build_functions.sh.j2
--rw-r--r--   0        0        0     3555 2024-05-01 01:07:56.391004 cocnc-0.1.0/src/cnc/flavors/gcp/shared/build/nginx.conf.j2
--rw-r--r--   0        0        0       59 2024-04-26 14:43:08.938875 cocnc-0.1.0/src/cnc/flavors/gcp/shared/deploy/all-access-policy.yml.j2
--rw-r--r--   0        0        0     4572 2024-05-10 01:36:08.677103 cocnc-0.1.0/src/cnc/flavors/gcp/shared/deploy/deploy_functions_base.sh.j2
--rw-r--r--   0        0        0     2354 2024-04-02 18:10:45.255229 cocnc-0.1.0/src/cnc/flavors/gcp/shared/deploy/k8s/scheduled_tasks.yml
--rw-r--r--   0        0        0      828 2024-05-10 01:36:08.677103 cocnc-0.1.0/src/cnc/flavors/gcp/shared/deploy/k8s/service_containers/backend-worker.yml
--rw-r--r--   0        0        0     1501 2024-04-02 18:10:45.255229 cocnc-0.1.0/src/cnc/flavors/gcp/shared/deploy/k8s/workers.yml
--rw-r--r--   0        0        0     1973 2024-05-10 01:36:08.677103 cocnc-0.1.0/src/cnc/flavors/gcp/shared/deploy/run-container.yml.j2
--rw-r--r--   0        0        0      191 2024-04-26 20:51:50.247437 cocnc-0.1.0/src/cnc/flavors/gcp/shared/deploy/run-job.yml.j2
--rw-r--r--   0        0        0      278 2024-04-26 14:43:08.942875 cocnc-0.1.0/src/cnc/flavors/gcp/shared/deploy/run-svc.yml.j2
--rw-r--r--   0        0        0     1496 2024-04-26 14:43:08.942875 cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/collection/bastion_instance.tf.j2
--rw-r--r--   0        0        0     3790 2024-05-08 16:39:58.931845 cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/collection/common_setup_resources.tf.j2
--rw-r--r--   0        0        0     2503 2024-05-01 01:07:56.391004 cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/collection/default_service.tf.j2
--rw-r--r--   0        0        0     1704 2024-05-01 01:07:56.391004 cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/collection/gke_cluster.tf.j2
--rw-r--r--   0        0        0      707 2024-04-26 20:51:50.247437 cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/collection/providers.tf.j2
--rw-r--r--   0        0        0     8353 2024-05-01 01:07:56.391004 cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/collection/vpc_networking.tf.j2
--rw-r--r--   0        0        0     3584 2024-05-01 01:07:56.391004 cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/environment/database_resources.tf.j2
--rw-r--r--   0        0        0     1332 2024-04-26 20:51:50.247437 cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/environment/object_storage_resources.tf.j2
--rw-r--r--   0        0        0      463 2024-04-26 14:43:08.942875 cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/environment/resource_managed_secrets.tf.j2
--rw-r--r--   0        0        0     1142 2024-04-26 20:51:50.251437 cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/service/cache.tf.j2
--rw-r--r--   0        0        0     1342 2024-05-10 01:36:08.677103 cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service.tf.j2
--rw-r--r--   0        0        0     1755 2024-04-26 14:43:08.946875 cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service_networking.tf.j2
--rw-r--r--   0        0        0      332 2024-05-10 01:36:08.677103 cocnc-0.1.0/src/cnc/flavors/gcp/shared/toolbox/Dockerfile.j2
--rw-r--r--   0        0        0     4506 2024-05-01 01:07:56.391004 cocnc-0.1.0/src/cnc/flavors/gcp/shared/toolbox/main.sh.j2
--rw-r--r--   0        0        0      913 2024-05-12 00:57:28.450735 cocnc-0.1.0/src/cnc/logger.py
--rw-r--r--   0        0        0     2011 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/main.py
--rw-r--r--   0        0        0      426 2024-04-26 14:43:08.946875 cocnc-0.1.0/src/cnc/models/__init__.py
--rw-r--r--   0        0        0     4488 2024-05-12 00:57:28.450735 cocnc-0.1.0/src/cnc/models/application.py
--rw-r--r--   0        0        0      906 2024-05-12 00:57:28.454735 cocnc-0.1.0/src/cnc/models/base_model.py
--rw-r--r--   0        0        0     2884 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/models/builder.py
--rw-r--r--   0        0        0       30 2024-04-02 18:10:45.255229 cocnc-0.1.0/src/cnc/models/config/__init__.py
--rw-r--r--   0        0        0     7851 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/models/config/config.py
--rw-r--r--   0        0        0      324 2024-05-12 00:57:28.454735 cocnc-0.1.0/src/cnc/models/config/deploy_resource_limits.py
--rw-r--r--   0        0        0    17765 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/models/config/resource.py
--rw-r--r--   0        0        0    11570 2024-05-12 00:57:28.458735 cocnc-0.1.0/src/cnc/models/config/service.py
--rw-r--r--   0        0        0    10437 2024-05-12 00:57:28.458735 cocnc-0.1.0/src/cnc/models/config/settings.py
--rw-r--r--   0        0        0      119 2024-04-02 18:10:45.255229 cocnc-0.1.0/src/cnc/models/config/utils.py
--rw-r--r--   0        0        0      257 2024-04-26 14:43:08.946875 cocnc-0.1.0/src/cnc/models/custom_header.py
--rw-r--r--   0        0        0     8616 2024-05-12 00:57:28.458735 cocnc-0.1.0/src/cnc/models/cycle_stage_base.py
--rw-r--r--   0        0        0     3488 2024-05-12 00:57:28.458735 cocnc-0.1.0/src/cnc/models/deployer.py
--rw-r--r--   0        0        0     8062 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/models/environment.py
--rw-r--r--   0        0        0    10410 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/models/environment_collection.py
--rw-r--r--   0        0        0     3646 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/models/environment_variable.py
--rw-r--r--   0        0        0        0 2024-04-02 18:10:45.259229 cocnc-0.1.0/src/cnc/models/providers/__init__.py
--rw-r--r--   0        0        0      288 2024-04-26 20:51:50.255437 cocnc-0.1.0/src/cnc/models/providers/amazon/__init__.py
--rw-r--r--   0        0        0      485 2024-05-12 00:57:28.458735 cocnc-0.1.0/src/cnc/models/providers/amazon/cache_resource_settings.py
--rw-r--r--   0        0        0     7166 2024-05-12 00:57:28.458735 cocnc-0.1.0/src/cnc/models/providers/amazon/custom_headers.py
--rw-r--r--   0        0        0     3187 2024-05-12 00:57:28.458735 cocnc-0.1.0/src/cnc/models/providers/amazon/database_resource_settings.py
--rw-r--r--   0        0        0     3377 2024-05-12 00:57:28.458735 cocnc-0.1.0/src/cnc/models/providers/amazon/deploy_resource_limits.py
--rw-r--r--   0        0        0     5379 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/models/providers/amazon/environment_collection.py
--rw-r--r--   0        0        0      168 2024-04-02 18:10:45.259229 cocnc-0.1.0/src/cnc/models/providers/amazon/service_account.py
--rw-r--r--   0        0        0      190 2024-04-26 20:51:50.255437 cocnc-0.1.0/src/cnc/models/providers/google/__init__.py
--rw-r--r--   0        0        0      756 2024-04-26 20:51:50.255437 cocnc-0.1.0/src/cnc/models/providers/google/cache_resource_settings.py
--rw-r--r--   0        0        0     2074 2024-05-12 00:57:28.462735 cocnc-0.1.0/src/cnc/models/providers/google/database_resource_settings.py
--rw-r--r--   0        0        0     2837 2024-05-12 00:57:28.462735 cocnc-0.1.0/src/cnc/models/providers/google/deploy_resource_limits.py
--rw-r--r--   0        0        0     9942 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/models/providers/google/environment_collection.py
--rw-r--r--   0        0        0        0 2024-04-02 18:10:45.259229 cocnc-0.1.0/src/cnc/models/providers/google/service_account.py
--rw-r--r--   0        0        0    14427 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/models/provisioner.py
--rw-r--r--   0        0        0      802 2024-04-26 14:43:08.958875 cocnc-0.1.0/src/cnc/models/resource_use_existing.py
--rw-r--r--   0        0        0      779 2024-04-02 18:10:45.259229 cocnc-0.1.0/src/cnc/models/stage.py
--rw-r--r--   0        0        0     4279 2024-05-12 00:57:28.462735 cocnc-0.1.0/src/cnc/models/toolbox.py
--rw-r--r--   0        0        0        0 2024-04-02 18:10:45.259229 cocnc-0.1.0/src/cnc/tests/__init__.py
--rw-r--r--   0        0        0     1071 2024-05-05 23:59:45.934092 cocnc-0.1.0/src/cnc/tests/base_test_class.py
--rw-r--r--   0        0        0       75 2024-05-05 23:59:45.938092 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service/cnc.yml
--rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-1-db/cnc.yml
--rw-r--r--   0        0        0      609 2024-04-26 14:43:08.958875 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_cidrs.yml
--rw-r--r--   0        0        0      673 2024-04-26 14:43:08.958875 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_subnets.yml
--rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-1-db-both-use-existing/cnc.yml
--rw-r--r--   0        0        0      472 2024-04-02 18:10:45.259229 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-1-db-both-use-existing/environments.yml
--rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-1-db-use-existing/cnc.yml
--rw-r--r--   0        0        0      379 2024-04-02 18:10:45.259229 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-1-db-use-existing/environments.yml
--rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/cnc.yml
--rw-r--r--   0        0        0      564 2024-04-02 18:10:45.259229 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/environments.yml
--rw-r--r--   0        0        0      231 2024-05-05 23:59:45.934092 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-2-db/cnc.yml
--rw-r--r--   0        0        0      231 2024-05-05 23:59:45.934092 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/cnc.yml
--rw-r--r--   0        0        0      373 2024-04-02 18:10:45.259229 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments.yml
--rw-r--r--   0        0        0      479 2024-04-02 18:10:45.259229 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments_aws_ecs.yml
--rw-r--r--   0        0        0      392 2024-04-26 14:43:08.962875 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments_gcp_run_region_settings.yml
--rw-r--r--   0        0        0       75 2024-05-05 23:59:45.934092 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-custom/cnc.yml
--rw-r--r--   0        0        0       22 2024-04-26 14:43:08.962875 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-custom/custom/deploy/main.sh.j2
--rw-r--r--   0        0        0      341 2024-04-26 14:43:08.962875 cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-custom/environments.yml
--rw-r--r--   0        0        0      228 2024-05-05 23:59:45.938092 cocnc-0.1.0/src/cnc/tests/fixtures/backend-2-service-1-db/cnc.yml
--rw-r--r--   0        0        0      322 2024-05-05 23:59:45.938092 cocnc-0.1.0/src/cnc/tests/fixtures/backend-2-service-2-db/cnc.yml
--rw-r--r--   0        0        0      153 2024-05-05 23:59:45.938092 cocnc-0.1.0/src/cnc/tests/fixtures/shared/cnc.yml
--rw-r--r--   0        0        0      340 2024-05-05 23:59:45.938092 cocnc-0.1.0/src/cnc/tests/fixtures/shared/environments-custom-provision.yml
--rw-r--r--   0        0        0      294 2024-04-02 18:10:45.259229 cocnc-0.1.0/src/cnc/tests/fixtures/shared/environments.yml
--rw-r--r--   0        0        0      400 2024-04-02 18:10:45.259229 cocnc-0.1.0/src/cnc/tests/fixtures/shared/environments_aws_ecs.yml
--rw-r--r--   0        0        0      474 2024-04-26 14:43:08.962875 cocnc-0.1.0/src/cnc/tests/fixtures/shared/environments_aws_ecs_existing_vpc.yml
--rw-r--r--   0        0        0      299 2024-04-26 14:43:08.962875 cocnc-0.1.0/src/cnc/tests/fixtures/shared/environments_gcp_run_lite.yml
--rw-r--r--   0        0        0     5373 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/tests/test_builder.py
--rw-r--r--   0        0        0     2683 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/tests/test_deployer.py
--rw-r--r--   0        0        0     2445 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/tests/test_environment_collection.py
--rw-r--r--   0        0        0     2287 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/tests/test_environment_variables.py
--rw-r--r--   0        0        0     1872 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/tests/test_environments.py
--rw-r--r--   0        0        0    13574 2024-05-12 00:57:28.462735 cocnc-0.1.0/src/cnc/tests/test_provisioner.py
--rw-r--r--   0        0        0     2898 2024-05-14 18:02:38.226930 cocnc-0.1.0/src/cnc/tests/test_services.py
--rw-r--r--   0        0        0     2224 2024-05-12 00:57:28.462735 cocnc-0.1.0/src/cnc/tests/test_toolbox.py
--rw-r--r--   0        0        0       38 2024-04-26 14:43:08.966875 cocnc-0.1.0/src/cnc/utils/__init__.py
--rw-r--r--   0        0        0      625 2024-04-26 14:43:08.966875 cocnc-0.1.0/src/cnc/utils/string.py
--rw-r--r--   0        0        0     6096 1970-01-01 00:00:00.000000 cocnc-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-02 18:10:45.243229 cocnc-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0     5336 2024-05-16 00:58:59.838603 cocnc-0.1.1/README.md
+-rw-r--r--   0        0        0      945 2024-05-16 01:42:20.554661 cocnc-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      199 2024-05-12 00:57:28.450735 cocnc-0.1.1/src/cnc/__init__.py
+-rw-r--r--   0        0        0      498 2024-05-12 00:57:28.450735 cocnc-0.1.1/src/cnc/check_dependencies.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:10:45.243229 cocnc-0.1.1/src/cnc/commands/__init__.py
+-rw-r--r--   0        0        0     1590 2024-05-16 00:52:25.626595 cocnc-0.1.1/src/cnc/commands/build.py
+-rw-r--r--   0        0        0     1545 2024-05-15 22:32:34.815388 cocnc-0.1.1/src/cnc/commands/deploy.py
+-rw-r--r--   0        0        0     2409 2024-05-16 01:31:54.206647 cocnc-0.1.1/src/cnc/commands/info.py
+-rw-r--r--   0        0        0     4136 2024-05-12 00:57:28.450735 cocnc-0.1.1/src/cnc/commands/provision.py
+-rw-r--r--   0        0        0      753 2024-05-12 00:57:28.450735 cocnc-0.1.1/src/cnc/commands/render.py
+-rw-r--r--   0        0        0      663 2024-04-02 18:10:45.243229 cocnc-0.1.1/src/cnc/commands/shell.py
+-rw-r--r--   0        0        0     1079 2024-05-15 22:12:13.119371 cocnc-0.1.1/src/cnc/commands/telemetry.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:10:45.247229 cocnc-0.1.1/src/cnc/commands/template_editor/__init__.py
+-rw-r--r--   0        0        0     5650 2024-05-14 18:02:38.226930 cocnc-0.1.1/src/cnc/commands/template_editor/inspector.py
+-rw-r--r--   0        0        0     2956 2024-05-15 23:34:56.487440 cocnc-0.1.1/src/cnc/commands/toolbox.py
+-rw-r--r--   0        0        0     1807 2024-05-16 01:03:27.678609 cocnc-0.1.1/src/cnc/commands/update.py
+-rw-r--r--   0        0        0      739 2024-04-02 18:10:45.247229 cocnc-0.1.1/src/cnc/constants.py
+-rw-r--r--   0        0        0     3780 2024-05-10 01:36:08.673102 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/build/build_functions.sh.j2
+-rw-r--r--   0        0        0      789 2024-04-26 14:43:08.886875 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/build/main.sh.j2
+-rw-r--r--   0        0        0       43 2024-04-02 18:10:45.247229 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/deploy_functions.sh.j2
+-rw-r--r--   0        0        0     2694 2024-05-12 00:57:28.450735 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/ecs_web_task.json.j2
+-rw-r--r--   0        0        0     1257 2024-05-01 01:07:56.387004 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/main.sh.j2
+-rw-r--r--   0        0        0     1623 2024-05-01 01:07:56.387004 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy.sh.j2
+-rw-r--r--   0        0        0     2468 2024-05-01 01:07:56.387004 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy_status_check.sh.j2
+-rw-r--r--   0        0        0      766 2024-04-26 14:43:08.898875 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/partials/ecs_wait_with_retries.sh.j2
+-rw-r--r--   0        0        0      645 2024-05-01 01:07:56.387004 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/partials/update_task_definition.sh.j2
+-rw-r--r--   0        0        0      200 2024-05-01 01:07:56.387004 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy.sh.j2
+-rw-r--r--   0        0        0     1047 2024-05-01 01:07:56.387004 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy_functions.sh.j2
+-rw-r--r--   0        0        0     1478 2024-05-03 17:48:33.699163 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/base.tf.j2
+-rw-r--r--   0        0        0      396 2024-04-02 18:10:45.247229 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/frontend_routing_lambda/index.js
+-rw-r--r--   0        0        0      561 2024-04-26 14:43:08.902875 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/main.tf.j2
+-rw-r--r--   0        0        0     4651 2024-04-26 14:43:08.902875 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/active_and_paused_envs.tf.j2
+-rw-r--r--   0        0        0     5481 2024-04-26 14:43:08.906875 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_backend_deployments.tf.j2
+-rw-r--r--   0        0        0     5640 2024-04-26 14:43:08.906875 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_deployments.tf.j2
+-rw-r--r--   0        0        0     1759 2024-05-01 01:07:56.387004 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_frontend_deployments.tf.j2
+-rw-r--r--   0        0        0    11529 2024-04-26 14:43:08.910875 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_backend_services.tf.j2
+-rw-r--r--   0        0        0      813 2024-05-12 00:57:28.450735 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/collection/providers.tf.j2
+-rw-r--r--   0        0        0     8800 2024-05-08 16:39:58.931845 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/collection/vpc_configuration.tf.j2
+-rw-r--r--   0        0        0     1888 2024-05-12 00:57:28.450735 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/collection_level_resources.tf.j2
+-rw-r--r--   0        0        0     1432 2024-04-26 14:43:08.918875 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/environment/efs.tf.j2
+-rw-r--r--   0        0        0     1886 2024-04-02 18:10:45.251229 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/environment/msg_queue_and_obj_storage.tf.j2
+-rw-r--r--   0        0        0    26090 2024-05-01 01:07:56.391004 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/environment_level_resources.tf.j2
+-rw-r--r--   0        0        0     9699 2024-05-01 01:07:56.391004 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_backend.tf.j2
+-rw-r--r--   0        0        0     6430 2024-04-26 14:43:08.922875 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_frontend.tf.j2
+-rw-r--r--   0        0        0     2382 2024-05-01 01:07:56.391004 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/scheduled_tasks.tf.j2
+-rw-r--r--   0        0        0     5446 2024-05-01 01:07:56.391004 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/workers.tf.j2
+-rw-r--r--   0        0        0      965 2024-04-26 14:43:08.926875 cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/service_level_resources.tf.j2
+-rw-r--r--   0        0        0    11323 2024-05-12 00:57:28.450735 cocnc-0.1.1/src/cnc/flavors/aws/shared/deploy/deploy_functions_base.sh.j2
+-rw-r--r--   0        0        0      336 2024-05-10 01:36:08.677103 cocnc-0.1.1/src/cnc/flavors/aws/shared/toolbox/Dockerfile.j2
+-rw-r--r--   0        0        0     4184 2024-05-01 01:07:56.391004 cocnc-0.1.1/src/cnc/flavors/aws/shared/toolbox/main.sh.j2
+-rw-r--r--   0        0        0      615 2024-04-02 18:10:45.251229 cocnc-0.1.1/src/cnc/flavors/gcp/gke/1/deploy/deploy.sh.j2
+-rw-r--r--   0        0        0      290 2024-04-26 14:43:08.930875 cocnc-0.1.1/src/cnc/flavors/gcp/gke/1/deploy/deploy_functions.sh.j2
+-rw-r--r--   0        0        0     1953 2024-04-26 14:43:08.930875 cocnc-0.1.1/src/cnc/flavors/gcp/gke/1/provision/base.tf.j2
+-rw-r--r--   0        0        0      561 2024-04-26 14:43:08.930875 cocnc-0.1.1/src/cnc/flavors/gcp/gke/1/provision/main.tf.j2
+-rw-r--r--   0        0        0     1189 2024-04-26 14:43:08.930875 cocnc-0.1.1/src/cnc/flavors/gcp/gke/1/provision/partials/collection_level_resources.tf.j2
+-rw-r--r--   0        0        0     4347 2024-04-26 14:43:08.930875 cocnc-0.1.1/src/cnc/flavors/gcp/gke/1/provision/partials/service_level_resources.tf.j2
+-rw-r--r--   0        0        0      299 2024-04-02 18:10:45.251229 cocnc-0.1.1/src/cnc/flavors/gcp/run/1/build/main.sh.j2
+-rw-r--r--   0        0        0      104 2024-04-02 18:10:45.251229 cocnc-0.1.1/src/cnc/flavors/gcp/run/1/cnc-flavor.yml
+-rw-r--r--   0        0        0      661 2024-04-26 14:43:08.934875 cocnc-0.1.1/src/cnc/flavors/gcp/run/1/deploy/base.sh.j2
+-rw-r--r--   0        0        0       43 2024-04-02 18:10:45.255229 cocnc-0.1.1/src/cnc/flavors/gcp/run/1/deploy/deploy_functions.sh.j2
+-rw-r--r--   0        0        0      303 2024-04-02 18:10:45.255229 cocnc-0.1.1/src/cnc/flavors/gcp/run/1/deploy/main.sh.j2
+-rw-r--r--   0        0        0     2512 2024-05-03 17:48:33.699163 cocnc-0.1.1/src/cnc/flavors/gcp/run/1/provision/base.tf.j2
+-rw-r--r--   0        0        0      561 2024-04-26 14:43:08.934875 cocnc-0.1.1/src/cnc/flavors/gcp/run/1/provision/main.tf.j2
+-rw-r--r--   0        0        0      299 2024-04-26 14:43:08.930875 cocnc-0.1.1/src/cnc/flavors/gcp/run-lite/1/build/main.sh.j2
+-rw-r--r--   0        0        0      493 2024-04-26 14:43:08.934875 cocnc-0.1.1/src/cnc/flavors/gcp/run-lite/1/deploy/base.sh.j2
+-rw-r--r--   0        0        0      331 2024-04-26 14:43:08.934875 cocnc-0.1.1/src/cnc/flavors/gcp/run-lite/1/deploy/deploy_functions.sh.j2
+-rw-r--r--   0        0        0      303 2024-04-26 14:43:08.934875 cocnc-0.1.1/src/cnc/flavors/gcp/run-lite/1/deploy/main.sh.j2
+-rw-r--r--   0        0        0     1778 2024-05-10 01:36:08.677103 cocnc-0.1.1/src/cnc/flavors/gcp/run-lite/1/deploy/run-container.yml.j2
+-rw-r--r--   0        0        0     1364 2024-04-26 20:51:50.243437 cocnc-0.1.1/src/cnc/flavors/gcp/run-lite/1/provision/base.tf.j2
+-rw-r--r--   0        0        0      561 2024-04-26 14:43:08.934875 cocnc-0.1.1/src/cnc/flavors/gcp/run-lite/1/provision/main.tf.j2
+-rw-r--r--   0        0        0     1926 2024-05-01 01:07:56.391004 cocnc-0.1.1/src/cnc/flavors/gcp/run-lite/1/toolbox/main.sh.j2
+-rw-r--r--   0        0        0      273 2024-05-01 01:07:56.391004 cocnc-0.1.1/src/cnc/flavors/gcp/shared/build/Dockerfile.run.j2
+-rw-r--r--   0        0        0     1017 2024-05-01 01:07:56.391004 cocnc-0.1.1/src/cnc/flavors/gcp/shared/build/base.sh.j2
+-rw-r--r--   0        0        0     4542 2024-05-15 23:31:32.787438 cocnc-0.1.1/src/cnc/flavors/gcp/shared/build/build_functions.sh.j2
+-rw-r--r--   0        0        0     3555 2024-05-01 01:07:56.391004 cocnc-0.1.1/src/cnc/flavors/gcp/shared/build/nginx.conf.j2
+-rw-r--r--   0        0        0       59 2024-04-26 14:43:08.938875 cocnc-0.1.1/src/cnc/flavors/gcp/shared/deploy/all-access-policy.yml.j2
+-rw-r--r--   0        0        0     4572 2024-05-10 01:36:08.677103 cocnc-0.1.1/src/cnc/flavors/gcp/shared/deploy/deploy_functions_base.sh.j2
+-rw-r--r--   0        0        0     2354 2024-04-02 18:10:45.255229 cocnc-0.1.1/src/cnc/flavors/gcp/shared/deploy/k8s/scheduled_tasks.yml
+-rw-r--r--   0        0        0      828 2024-05-10 01:36:08.677103 cocnc-0.1.1/src/cnc/flavors/gcp/shared/deploy/k8s/service_containers/backend-worker.yml
+-rw-r--r--   0        0        0     1501 2024-04-02 18:10:45.255229 cocnc-0.1.1/src/cnc/flavors/gcp/shared/deploy/k8s/workers.yml
+-rw-r--r--   0        0        0     1973 2024-05-10 01:36:08.677103 cocnc-0.1.1/src/cnc/flavors/gcp/shared/deploy/run-container.yml.j2
+-rw-r--r--   0        0        0      191 2024-04-26 20:51:50.247437 cocnc-0.1.1/src/cnc/flavors/gcp/shared/deploy/run-job.yml.j2
+-rw-r--r--   0        0        0      278 2024-04-26 14:43:08.942875 cocnc-0.1.1/src/cnc/flavors/gcp/shared/deploy/run-svc.yml.j2
+-rw-r--r--   0        0        0     1496 2024-04-26 14:43:08.942875 cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/collection/bastion_instance.tf.j2
+-rw-r--r--   0        0        0     3790 2024-05-08 16:39:58.931845 cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/collection/common_setup_resources.tf.j2
+-rw-r--r--   0        0        0     2503 2024-05-01 01:07:56.391004 cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/collection/default_service.tf.j2
+-rw-r--r--   0        0        0     1704 2024-05-01 01:07:56.391004 cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/collection/gke_cluster.tf.j2
+-rw-r--r--   0        0        0      707 2024-04-26 20:51:50.247437 cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/collection/providers.tf.j2
+-rw-r--r--   0        0        0     8353 2024-05-01 01:07:56.391004 cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/collection/vpc_networking.tf.j2
+-rw-r--r--   0        0        0     3584 2024-05-01 01:07:56.391004 cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/environment/database_resources.tf.j2
+-rw-r--r--   0        0        0     1332 2024-04-26 20:51:50.247437 cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/environment/object_storage_resources.tf.j2
+-rw-r--r--   0        0        0      463 2024-04-26 14:43:08.942875 cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/environment/resource_managed_secrets.tf.j2
+-rw-r--r--   0        0        0     1142 2024-04-26 20:51:50.251437 cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/service/cache.tf.j2
+-rw-r--r--   0        0        0     1342 2024-05-10 01:36:08.677103 cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service.tf.j2
+-rw-r--r--   0        0        0     1755 2024-04-26 14:43:08.946875 cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service_networking.tf.j2
+-rw-r--r--   0        0        0      332 2024-05-10 01:36:08.677103 cocnc-0.1.1/src/cnc/flavors/gcp/shared/toolbox/Dockerfile.j2
+-rw-r--r--   0        0        0     4484 2024-05-15 15:08:21.561546 cocnc-0.1.1/src/cnc/flavors/gcp/shared/toolbox/main.sh.j2
+-rw-r--r--   0        0        0      913 2024-05-12 00:57:28.450735 cocnc-0.1.1/src/cnc/logger.py
+-rw-r--r--   0        0        0     2120 2024-05-16 00:59:53.626605 cocnc-0.1.1/src/cnc/main.py
+-rw-r--r--   0        0        0      426 2024-04-26 14:43:08.946875 cocnc-0.1.1/src/cnc/models/__init__.py
+-rw-r--r--   0        0        0     4488 2024-05-12 00:57:28.450735 cocnc-0.1.1/src/cnc/models/application.py
+-rw-r--r--   0        0        0      906 2024-05-12 00:57:28.454735 cocnc-0.1.1/src/cnc/models/base_model.py
+-rw-r--r--   0        0        0     3088 2024-05-15 21:55:12.227357 cocnc-0.1.1/src/cnc/models/builder.py
+-rw-r--r--   0        0        0       30 2024-04-02 18:10:45.255229 cocnc-0.1.1/src/cnc/models/config/__init__.py
+-rw-r--r--   0        0        0     7851 2024-05-14 18:02:38.226930 cocnc-0.1.1/src/cnc/models/config/config.py
+-rw-r--r--   0        0        0      324 2024-05-12 00:57:28.454735 cocnc-0.1.1/src/cnc/models/config/deploy_resource_limits.py
+-rw-r--r--   0        0        0    17833 2024-05-15 22:25:07.115382 cocnc-0.1.1/src/cnc/models/config/resource.py
+-rw-r--r--   0        0        0    11822 2024-05-16 01:33:27.026649 cocnc-0.1.1/src/cnc/models/config/service.py
+-rw-r--r--   0        0        0    10437 2024-05-12 00:57:28.458735 cocnc-0.1.1/src/cnc/models/config/settings.py
+-rw-r--r--   0        0        0      119 2024-04-02 18:10:45.255229 cocnc-0.1.1/src/cnc/models/config/utils.py
+-rw-r--r--   0        0        0      257 2024-04-26 14:43:08.946875 cocnc-0.1.1/src/cnc/models/custom_header.py
+-rw-r--r--   0        0        0     8616 2024-05-12 00:57:28.458735 cocnc-0.1.1/src/cnc/models/cycle_stage_base.py
+-rw-r--r--   0        0        0     3692 2024-05-15 21:55:16.643357 cocnc-0.1.1/src/cnc/models/deployer.py
+-rw-r--r--   0        0        0     8062 2024-05-14 18:02:38.226930 cocnc-0.1.1/src/cnc/models/environment.py
+-rw-r--r--   0        0        0    10410 2024-05-14 18:02:38.226930 cocnc-0.1.1/src/cnc/models/environment_collection.py
+-rw-r--r--   0        0        0     3646 2024-05-14 18:02:38.226930 cocnc-0.1.1/src/cnc/models/environment_variable.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:10:45.259229 cocnc-0.1.1/src/cnc/models/providers/__init__.py
+-rw-r--r--   0        0        0      288 2024-04-26 20:51:50.255437 cocnc-0.1.1/src/cnc/models/providers/amazon/__init__.py
+-rw-r--r--   0        0        0      485 2024-05-12 00:57:28.458735 cocnc-0.1.1/src/cnc/models/providers/amazon/cache_resource_settings.py
+-rw-r--r--   0        0        0     7166 2024-05-12 00:57:28.458735 cocnc-0.1.1/src/cnc/models/providers/amazon/custom_headers.py
+-rw-r--r--   0        0        0     3187 2024-05-12 00:57:28.458735 cocnc-0.1.1/src/cnc/models/providers/amazon/database_resource_settings.py
+-rw-r--r--   0        0        0     3377 2024-05-12 00:57:28.458735 cocnc-0.1.1/src/cnc/models/providers/amazon/deploy_resource_limits.py
+-rw-r--r--   0        0        0     5379 2024-05-14 18:02:38.226930 cocnc-0.1.1/src/cnc/models/providers/amazon/environment_collection.py
+-rw-r--r--   0        0        0      168 2024-04-02 18:10:45.259229 cocnc-0.1.1/src/cnc/models/providers/amazon/service_account.py
+-rw-r--r--   0        0        0      190 2024-04-26 20:51:50.255437 cocnc-0.1.1/src/cnc/models/providers/google/__init__.py
+-rw-r--r--   0        0        0      756 2024-04-26 20:51:50.255437 cocnc-0.1.1/src/cnc/models/providers/google/cache_resource_settings.py
+-rw-r--r--   0        0        0     2074 2024-05-12 00:57:28.462735 cocnc-0.1.1/src/cnc/models/providers/google/database_resource_settings.py
+-rw-r--r--   0        0        0     2837 2024-05-12 00:57:28.462735 cocnc-0.1.1/src/cnc/models/providers/google/deploy_resource_limits.py
+-rw-r--r--   0        0        0     9942 2024-05-14 18:02:38.226930 cocnc-0.1.1/src/cnc/models/providers/google/environment_collection.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:10:45.259229 cocnc-0.1.1/src/cnc/models/providers/google/service_account.py
+-rw-r--r--   0        0        0    14435 2024-05-15 15:50:33.889645 cocnc-0.1.1/src/cnc/models/provisioner.py
+-rw-r--r--   0        0        0      802 2024-04-26 14:43:08.958875 cocnc-0.1.1/src/cnc/models/resource_use_existing.py
+-rw-r--r--   0        0        0      779 2024-04-02 18:10:45.259229 cocnc-0.1.1/src/cnc/models/stage.py
+-rw-r--r--   0        0        0     4279 2024-05-12 00:57:28.462735 cocnc-0.1.1/src/cnc/models/toolbox.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:10:45.259229 cocnc-0.1.1/src/cnc/tests/__init__.py
+-rw-r--r--   0        0        0     1071 2024-05-05 23:59:45.934092 cocnc-0.1.1/src/cnc/tests/base_test_class.py
+-rw-r--r--   0        0        0       75 2024-05-05 23:59:45.938092 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service/cnc.yml
+-rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-1-db/cnc.yml
+-rw-r--r--   0        0        0      609 2024-04-26 14:43:08.958875 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_cidrs.yml
+-rw-r--r--   0        0        0      673 2024-04-26 14:43:08.958875 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_subnets.yml
+-rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-1-db-both-use-existing/cnc.yml
+-rw-r--r--   0        0        0      472 2024-04-02 18:10:45.259229 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-1-db-both-use-existing/environments.yml
+-rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-1-db-use-existing/cnc.yml
+-rw-r--r--   0        0        0      379 2024-04-02 18:10:45.259229 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-1-db-use-existing/environments.yml
+-rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/cnc.yml
+-rw-r--r--   0        0        0      564 2024-04-02 18:10:45.259229 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/environments.yml
+-rw-r--r--   0        0        0      231 2024-05-05 23:59:45.934092 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-2-db/cnc.yml
+-rw-r--r--   0        0        0      231 2024-05-05 23:59:45.934092 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/cnc.yml
+-rw-r--r--   0        0        0      373 2024-04-02 18:10:45.259229 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments.yml
+-rw-r--r--   0        0        0      479 2024-04-02 18:10:45.259229 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments_aws_ecs.yml
+-rw-r--r--   0        0        0      392 2024-04-26 14:43:08.962875 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments_gcp_run_region_settings.yml
+-rw-r--r--   0        0        0       75 2024-05-05 23:59:45.934092 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-custom/cnc.yml
+-rw-r--r--   0        0        0       22 2024-04-26 14:43:08.962875 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-custom/custom/deploy/main.sh.j2
+-rw-r--r--   0        0        0      341 2024-04-26 14:43:08.962875 cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-custom/environments.yml
+-rw-r--r--   0        0        0      228 2024-05-05 23:59:45.938092 cocnc-0.1.1/src/cnc/tests/fixtures/backend-2-service-1-db/cnc.yml
+-rw-r--r--   0        0        0      322 2024-05-05 23:59:45.938092 cocnc-0.1.1/src/cnc/tests/fixtures/backend-2-service-2-db/cnc.yml
+-rw-r--r--   0        0        0      153 2024-05-05 23:59:45.938092 cocnc-0.1.1/src/cnc/tests/fixtures/shared/cnc.yml
+-rw-r--r--   0        0        0      340 2024-05-05 23:59:45.938092 cocnc-0.1.1/src/cnc/tests/fixtures/shared/environments-custom-provision.yml
+-rw-r--r--   0        0        0      294 2024-04-02 18:10:45.259229 cocnc-0.1.1/src/cnc/tests/fixtures/shared/environments.yml
+-rw-r--r--   0        0        0      400 2024-04-02 18:10:45.259229 cocnc-0.1.1/src/cnc/tests/fixtures/shared/environments_aws_ecs.yml
+-rw-r--r--   0        0        0      474 2024-04-26 14:43:08.962875 cocnc-0.1.1/src/cnc/tests/fixtures/shared/environments_aws_ecs_existing_vpc.yml
+-rw-r--r--   0        0        0      299 2024-04-26 14:43:08.962875 cocnc-0.1.1/src/cnc/tests/fixtures/shared/environments_gcp_run_lite.yml
+-rw-r--r--   0        0        0     5373 2024-05-14 18:02:38.226930 cocnc-0.1.1/src/cnc/tests/test_builder.py
+-rw-r--r--   0        0        0     2683 2024-05-14 18:02:38.226930 cocnc-0.1.1/src/cnc/tests/test_deployer.py
+-rw-r--r--   0        0        0     2445 2024-05-14 18:02:38.226930 cocnc-0.1.1/src/cnc/tests/test_environment_collection.py
+-rw-r--r--   0        0        0     2287 2024-05-14 18:02:38.226930 cocnc-0.1.1/src/cnc/tests/test_environment_variables.py
+-rw-r--r--   0        0        0     1872 2024-05-14 18:02:38.226930 cocnc-0.1.1/src/cnc/tests/test_environments.py
+-rw-r--r--   0        0        0    13574 2024-05-12 00:57:28.462735 cocnc-0.1.1/src/cnc/tests/test_provisioner.py
+-rw-r--r--   0        0        0     2898 2024-05-14 18:02:38.226930 cocnc-0.1.1/src/cnc/tests/test_services.py
+-rw-r--r--   0        0        0     2224 2024-05-12 00:57:28.462735 cocnc-0.1.1/src/cnc/tests/test_toolbox.py
+-rw-r--r--   0        0        0       38 2024-04-26 14:43:08.966875 cocnc-0.1.1/src/cnc/utils/__init__.py
+-rw-r--r--   0        0        0      625 2024-04-26 14:43:08.966875 cocnc-0.1.1/src/cnc/utils/string.py
+-rw-r--r--   0        0        0     6422 1970-01-01 00:00:00.000000 cocnc-0.1.1/PKG-INFO
```

### Comparing `cocnc-0.1.0/LICENSE.txt` & `cocnc-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/README.md` & `cocnc-0.1.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -13,30 +13,31 @@
 `cnc` is an open-source framework that equips developers with the tools to deploy applications with precision. Rooted in the principles of Infrastructure as Code (IaC) using terraform, `cnc` offers a flexible and cloud-agnostic abstraction that excels in managing deployments across various environments — whether it’s for development, staging, production, or ephemeral previews. For those who have used AWS's Amplify CLI, think of `cnc` as a broader, adaptable framework that supports your unique deployment needs.
 
 Core Lifecycle Events Managed by `cnc`:
 
 - Provision: Uses terraform to create, manage, and dismantle cloud resources, ensuring each environment is crafted to fit its specific purpose.
 - Build: Assembles the necessary deployment artifacts for each environment, from docker containers to static assets for web applications.
 - Deploy: Seamlessly updates infrastructure to deploy new artifacts, such as modifying k8s manifests or updating ECS services.
+- Toolbox: A `toolbox` is a managed shell against a `cnc`-managed envionment, making it easy to get a REPL or run database migrations, for example
 
 Getting Started with `cnc`:
 - Experience `cnc` in just a few minutes: install and see for yourself the power of cnc in under 5 minutes without needing any cloud permissions or incurring any costs.
 - Rapid Deployment: Have your first environment up and running in less than 15 minutes, demonstrating the straightforward power of cnc.
 
 `cnc` is designed not just as a tool, but as a partner in development, empowering you to build and manage your infrastructure with the same attention to detail and creativity that you bring to your code. Just like web devs use frameworks to build better products, with `cnc`, you gain the freedom to implement your vision precisely as intended, making each project not only functional but finely tuned to your standards.
 
 ## Getting Started
 
 ### Prerequisites
 
 Ensure that you have Docker installed, along with the `aws` or `gcloud` CLI tools, depending on your cloud provider.
 
-Intall `cnc` from the [PyPI Python Package Index](). For example, using `pip`:
+Intall `cnc` from the [PyPI Python Package Index](https://pypi.org/project/cocnc/). For example, using `pip`:
 ```
-pip install cnc
+pip install cocnc
 ```
 
 ### Annotate docker-compose.yml
 
 Mark the services that CNC should manage by adding the following snippet to your `docker-compose.yml`. You can annotate a subset of your existing `docker-compose.yml`, `cnc` will ignore services without the `x-cnc` extension.
 
 ```yaml
@@ -104,20 +105,27 @@
 cnc deploy perform dev --debug --no-cleanup
 ```
 
 Add a 2nd environment (e.g. `dev2`) to the `environments.yml` and run the commands again, see the power of the framework!
 
 ### Deploy your first environment
 
-Authenticate with your cloud provider using the aws or gcloud CLI, then deploy your environment with:
+Authenticate with your cloud provider using the aws or gcloud CLI, then create your infrastructure with:
 
 ```
-cnc cycle dev
+cnc provision apply
 ```
 
+deploy your `dev` environment with:
+```
+cnc update dev --service-tags app=v1
+```
+
+This will do a `build` and a `deploy` under the hood.
+
 For more details, see the step-by-step [Getting Started Guide](./docs/README.md).
 
 
 # Documentation
 
 Access full documentation and in-depth tutorials at [the CNC Documentation](./docs/README.md).
```

### Comparing `cocnc-0.1.0/pyproject.toml` & `cocnc-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cocnc"
-version = "0.1.0"
+version = "0.1.1"
 description = "CNC is the first framework for application deployment, a fully distributed and customizable PaaS developer experience, based on docker-compose config files"
 authors = [
     "Adam Abdelaziz <adam.abdelaziz@withcoherence.com>",
     "Zachary Zaro <zach@withcoherence.com>",
 ]
 readme = "README.md"
 packages = [
```

### Comparing `cocnc-0.1.0/src/cnc/commands/build.py` & `cocnc-0.1.1/src/cnc/commands/update.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,43 @@
 import typer
+import time
 from typing import List
 
+from cnc.models import DeployStageManager
 from cnc.models import BuildStageManager
 from .telemetry import send_event
 
 from cnc.logger import get_logger
-
 log = get_logger(__name__)
 
 
 app = typer.Typer()
 
 
 @app.command()
 def perform(
     ctx: typer.Context,
     environment_name: str,
+    services: List[str] = typer.Option(
+        [],
+        "--service",
+        help="Set for each service you want to build, if omitted will build all.",
+    ),
     service_tags: List[str] = typer.Option(
         [],
         "--service-tag",
         help="Set the tag to use for this service, default is 'latest'",
     ),
     collection_name: str = "",
     cleanup: bool = True,
     debug: bool = False,
     generate: bool = True,
 ):
-    """Build containers for config-defined services"""
-    send_event("build.perform")
+    start_time = time.time()
+    send_event("update.perform")
     collection = ctx.obj.application.collection_by_name(collection_name)
     if not collection:
         log.error(f"No collection found for: {collection_name}")
         raise typer.Exit(code=1)
 
     environment = collection.environment_by_name(environment_name)
     if not environment:
@@ -39,11 +45,20 @@
         raise typer.Exit(code=1)
 
     builder = BuildStageManager(environment, service_tags=service_tags)
     builder.perform(
         should_cleanup=cleanup,
         should_regenerate_config=generate,
         debug=debug,
+        service_names=services,
+    )
+
+    deployer = DeployStageManager(environment, service_tags=service_tags)
+    deployer.perform(
+        should_cleanup=cleanup,
+        should_regenerate_config=generate,
+        debug=debug,
+        service_names=services,
     )
 
-    log.debug(f"All set building for {builder.config_files_path}")
+    log.debug(f"All set updating for {services}/{service_tags} in {int(time.time() - start_time)} seconds")
     raise typer.Exit()
```

### Comparing `cocnc-0.1.0/src/cnc/commands/deploy.py` & `cocnc-0.1.1/src/cnc/commands/deploy.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import typer
+import time
 from typing import List
 
 from cnc.models import DeployStageManager
 from .telemetry import send_event
 
 from cnc.logger import get_logger
 
@@ -12,24 +13,30 @@
 app = typer.Typer()
 
 
 @app.command()
 def perform(
     ctx: typer.Context,
     environment_name: str,
+    services: List[str] = typer.Option(
+        [],
+        "--service",
+        help="Set for each service you want to build, if omitted will build all.",
+    ),
     service_tags: List[str] = typer.Option(
         [],
         "--service-tag",
         help="Set the tag to use for this service, default is 'latest'",
     ),
     collection_name: str = "",
     cleanup: bool = True,
     debug: bool = False,
     generate: bool = True,
 ):
+    start_time = time.time()
     send_event("deploy.perform")
     collection = ctx.obj.application.collection_by_name(collection_name)
     if not collection:
         log.error(f"No collection found for: {collection_name}")
         raise typer.Exit(code=1)
 
     environment = collection.environment_by_name(environment_name)
@@ -38,11 +45,12 @@
         raise typer.Exit(code=1)
 
     deployer = DeployStageManager(environment, service_tags=service_tags)
     deployer.perform(
         should_cleanup=cleanup,
         should_regenerate_config=generate,
         debug=debug,
+        service_names=services,
     )
 
-    log.debug(f"All set deploying for {deployer.rendered_files_path}")
+    log.debug(f"All set deploying for {deployer.rendered_files_path} in {int(time.time() - start_time)} seconds")
     raise typer.Exit()
```

### Comparing `cocnc-0.1.0/src/cnc/commands/info.py` & `cocnc-0.1.1/src/cnc/commands/info.py`

 * *Files 25% similar despite different names*

```diff
@@ -54,7 +54,41 @@
         headers = list(env_datas[0].keys())
         table_data = [list(d.values()) for d in env_datas]
         print(tabulate(table_data, headers, tablefmt="grid"))
     else:
         print(f"No environments for {collection}")
 
     raise typer.Exit()
+
+
+@app.command()
+def services(
+    ctx: typer.Context,
+    environment_name: str,
+    collection_name: str = "",
+):
+    send_event("info.services")
+    collection = (
+        ctx.obj.application.collection_by_name(collection_name)
+        or ctx.obj.application.default_collection
+    )
+    if not collection:
+        log.error(f"No collection found for: {collection_name}")
+        raise typer.Exit(code=1)
+
+    environment = collection.environment_by_name(environment_name)
+    if not environment:
+        log.error(f"No environment found for: {environment_name}")
+        raise typer.Exit(code=1)
+
+    svc_datas = []
+    for service in environment.services:
+        svc_datas.append(service.cli_info())
+
+    if svc_datas:
+        headers = list(svc_datas[0].keys())
+        table_data = [list(d.values()) for d in svc_datas]
+        print(tabulate(table_data, headers, tablefmt="grid"))
+    else:
+        print(f"No services for {environment}")
+
+    raise typer.Exit()
```

### Comparing `cocnc-0.1.0/src/cnc/commands/provision.py` & `cocnc-0.1.1/src/cnc/commands/provision.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/commands/render.py` & `cocnc-0.1.1/src/cnc/commands/render.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/commands/shell.py` & `cocnc-0.1.1/src/cnc/commands/shell.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/commands/telemetry.py` & `cocnc-0.1.1/src/cnc/commands/telemetry.py`

 * *Files 11% similar despite different names*

```diff
@@ -20,12 +20,18 @@
 
 def send_event(command_name: str):
     command_data = {
         "name": command_name,
     }
     if TELEMETRY_ENABLED:
         try:
-            user_id = os.environ.get("CNC_USER_ID", machineid.id())
+            _id = machineid.id()
+        except Exception as e:
+            print(f"Cannot get machine ID: {e}")
+            _id = None
+
+        try:
+            user_id = os.environ.get("CNC_USER_ID", _id or "UNKNOWN")
             print(f"Sending {command_data} to RS for {user_id}")
             rudder_analytics.track(user_id, "command", command_data)
         except Exception as e:
-            print(f"Cannot send telemetry event: {e}")
+            print(f"Cannot send telemetry event: {e}")
```

### Comparing `cocnc-0.1.0/src/cnc/commands/template_editor/inspector.py` & `cocnc-0.1.1/src/cnc/commands/template_editor/inspector.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/commands/toolbox.py` & `cocnc-0.1.1/src/cnc/commands/toolbox.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 def add_common(
     ctx: typer.Context,
     collection_name: str = typer.Option(
         default="preview", envvar="CNC_COLLECTION_NAME", help="Collection name"
     ),
 ):
     """Common Entry Point for Toolbox"""
+    print(ctx.obj)
     collection = ctx.obj.application.collection_by_name(collection_name)
     if not collection:
         log.error(
             f"No collection found for: {collection_name} | (configured "
             f"collections are: {[c.name for c in ctx.obj.application.collections]})"
         )
         raise typer.Exit(code=1)
```

### Comparing `cocnc-0.1.0/src/cnc/constants.py` & `cocnc-0.1.1/src/cnc/constants.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/build/build_functions.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/build/build_functions.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/build/main.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/build/main.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/ecs_web_task.json.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/ecs_web_task.json.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/main.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/main.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy_status_check.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy_status_check.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/partials/ecs_wait_with_retries.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/partials/ecs_wait_with_retries.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/partials/update_task_definition.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/partials/update_task_definition.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy_functions.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy_functions.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/base.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/base.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/main.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/main.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/active_and_paused_envs.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/active_and_paused_envs.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_backend_deployments.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_backend_deployments.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_deployments.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_deployments.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_frontend_deployments.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_frontend_deployments.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_backend_services.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_backend_services.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/collection/providers.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/collection/providers.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/collection/vpc_configuration.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/collection/vpc_configuration.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/collection_level_resources.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/collection_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/environment/efs.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/environment/efs.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/environment/msg_queue_and_obj_storage.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/environment/msg_queue_and_obj_storage.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/environment_level_resources.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/environment_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_backend.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_backend.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_frontend.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_frontend.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/scheduled_tasks.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/scheduled_tasks.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/workers.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/workers.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/ecs/1/provision/partials/service_level_resources.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/ecs/1/provision/partials/service_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/shared/deploy/deploy_functions_base.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/shared/deploy/deploy_functions_base.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/aws/shared/toolbox/main.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/aws/shared/toolbox/main.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/gke/1/deploy/deploy.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/gke/1/deploy/deploy.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/gke/1/provision/base.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/gke/1/provision/base.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/gke/1/provision/main.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/gke/1/provision/main.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/gke/1/provision/partials/collection_level_resources.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/gke/1/provision/partials/collection_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/gke/1/provision/partials/service_level_resources.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/gke/1/provision/partials/service_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/run/1/deploy/base.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/run/1/deploy/base.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/run/1/provision/base.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/run/1/provision/base.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/run/1/provision/main.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/run/1/provision/main.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/run-lite/1/deploy/run-container.yml.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/run-lite/1/deploy/run-container.yml.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/run-lite/1/provision/base.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/run-lite/1/provision/base.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/run-lite/1/provision/main.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/run-lite/1/provision/main.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/run-lite/1/toolbox/main.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/run-lite/1/toolbox/main.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/build/base.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/build/base.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/build/build_functions.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/build/build_functions.sh.j2`

 * *Files 1% similar despite different names*

```diff
@@ -63,26 +63,27 @@
 
 {% if service.is_frontend %}
 build_{{ service.name }}_assets () {
     echo -e "\\nBuilding assets...\\n"
     mkdir -p .{% if service.build.context != "." %}/{{ service.build.context }}{% endif %}/{{ service.settings.assets_path }}
     docker run --entrypoint sh {% for variable in service.environment_variables %}-e {{ variable.name }}={{ variable.value }} {% endfor %} -d --name app {{ service.image_for_tag(builder.tag_for_service(service.name)) }} -c "sleep 5000"
     docker exec app sh -c "{{ ' '.join(service.settings.build) }}"; build_result=$?
-    if [ $build_result -ne 0 ]; then docker logs app && exit $build_result; fi
+    if [ $build_result -ne 0 ]; then docker logs app && docker stop app && docker rm app && exit $build_result; fi
     docker cp app:$(docker exec app pwd)/{{service.settings.assets_path }}/. .{% if service.build.context != "." %}/{{ service.build.context }}{% endif %}/{{ service.settings.assets_path }}{% if service.settings.url_path != "/" %}/{% endif %}{{ service.settings.url_path.lstrip("/").rstrip("/") }}; copy_result=$?
     if [ $copy_result -ne 0 ]; then exit $copy_result; fi
     docker stop app
     docker rm app
 }
 
 build_{{ service.name }}_run_image () {
     cp {{ builder.rendered_files_path }}/{{ service.name }}-nginx.conf {{ service.build.context }}/{{ service.name }}-nginx.conf
     docker buildx inspect coherencebuilder_{{ service.name }}_run || docker buildx create --name coherencebuilder_{{ service.name }}_run
     docker buildx build -t {{ service.image_for_tag("latest", run=True) }} -t {{ service.image_for_tag(builder.tag_for_service(service.name), run=True) }} \
     --builder=coherencebuilder_{{ service.name }}_run \
     --cache-to=type=registry,ref={{ service.image_for_tag("cache", run=True) }},mode=max \
     --cache-from=type=registry,ref={{ service.image_for_tag("cache", run=True) }} \
     -f {{ builder.rendered_files_path }}/Dockerfile.{{ service.name }} --push {{ service.build.context }}
+    rm {{ service.build.context }}/{{ service.name }}-nginx.conf
 }
 {% endif %}
 
 {% endblock %}
```

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/build/nginx.conf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/build/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/deploy/deploy_functions_base.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/deploy/deploy_functions_base.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/deploy/k8s/scheduled_tasks.yml` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/deploy/k8s/scheduled_tasks.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/deploy/k8s/service_containers/backend-worker.yml` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/deploy/k8s/service_containers/backend-worker.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/deploy/k8s/workers.yml` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/deploy/k8s/workers.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/deploy/run-container.yml.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/deploy/run-container.yml.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/collection/bastion_instance.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/collection/bastion_instance.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/collection/common_setup_resources.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/collection/common_setup_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/collection/default_service.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/collection/default_service.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/collection/gke_cluster.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/collection/gke_cluster.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/collection/providers.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/collection/providers.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/collection/vpc_networking.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/collection/vpc_networking.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/environment/database_resources.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/environment/database_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/environment/object_storage_resources.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/environment/object_storage_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/service/cache.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/service/cache.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service_networking.tf.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service_networking.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/flavors/gcp/shared/toolbox/main.sh.j2` & `cocnc-0.1.1/src/cnc/flavors/gcp/shared/toolbox/main.sh.j2`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
 # Start & exec into docker container
 docker run --entrypoint sh \
 {%- for variable in toolbox.environment_items -%}
 -e {{ variable.name }}={{ variable.value }} \
 {%- endfor -%}
 --network ${CNC_TOOLBOX_NETWORK:-host} \
 {%- if command %}
---rm --name app {{ service.instance_name }}_toolbox -c '{{ command }}'; command_result=$?
+--rm {{ service.instance_name }}_toolbox -c '{{ command }}'; command_result=$?
 {%- else %}
--it --rm --name app {{ service.instance_name }}_toolbox
+-it --rm {{ service.instance_name }}_toolbox
 {%- endif %}
 
 {%- if command %}
 exit $command_result
 {%- endif %}
```

### Comparing `cocnc-0.1.0/src/cnc/logger.py` & `cocnc-0.1.1/src/cnc/logger.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/main.py` & `cocnc-0.1.1/src/cnc/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,16 @@
+import sys
 from pathlib import Path
 from dataclasses import dataclass
 from typing import Any
 
 import typer
 from rich import print
 
-from .commands import provision, build, deploy, info, shell, toolbox
+from .commands import provision, build, deploy, info, shell, toolbox, update
 from .commands.template_editor import inspector
 from .commands.telemetry import send_event
 from .models import Application
 from .check_dependencies import check_deps
 from cnc.logger import get_logger
 
 log = get_logger(__name__)
@@ -18,15 +19,15 @@
 app.add_typer(provision.app, name="provision")
 app.add_typer(build.app, name="build")
 app.add_typer(deploy.app, name="deploy")
 app.add_typer(inspector.app, name="inspector")
 app.add_typer(info.app, name="info")
 app.add_typer(shell.app, name="shell")
 app.add_typer(toolbox.app, name="toolbox")
-
+app.add_typer(update.app, name="update")
 
 @dataclass
 class Common:
     application: Any = None
     collection: Any = None
 
 
@@ -39,14 +40,17 @@
     environments_file_path: Path = typer.Option(
         default="environments.yml",
         envvar="CNC_ENVIRONMENTS_PATH",
         help="Environments data file path",
     ),
 ):
     """Common Entry Point for whole app"""
+    if "--help" in sys.argv:
+        return True
+
     check_deps()
 
     if not config_file_path.is_file():
         log.error(f"Config file not found: {config_file_path}")
         raise typer.Exit(code=1)
 
     if not environments_file_path.is_file():
```

### Comparing `cocnc-0.1.0/src/cnc/models/application.py` & `cocnc-0.1.1/src/cnc/models/application.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/base_model.py` & `cocnc-0.1.1/src/cnc/models/base_model.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/builder.py` & `cocnc-0.1.1/src/cnc/models/builder.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,16 +28,19 @@
 
         for service in self.environment.services:
             self.debug_template_output(f"build-{service.name}-functions.sh")
 
         log.debug(f"All done with debug for {self}")
         return
 
-    def render_build(self):
+    def render_build(self, service_names=None):
         for service in self.environment.services:
+            if service_names:
+                if service.name not in service_names:
+                    continue
 
             if service.settings.is_resource:
                 continue
 
             context = self.template_context(service)
             context["render_template"] = self.write_template_with_context(service)
 
@@ -49,24 +52,24 @@
 
             service_build_script_name = f"build-{service.name}.sh"
             self.write_template(
                 "main.sh.j2", output_name=service_build_script_name, context=context
             )
             self.scripts_to_run.append(service_build_script_name)
 
-    def perform(self, should_cleanup=True, should_regenerate_config=True, debug=False):
+    def perform(self, should_cleanup=True, should_regenerate_config=True, debug=False, service_names=None):
         log.debug(f"Performing build for {self} @ {self.config_files_path}")
         if should_cleanup:
             self.cleanup()
 
         self.setup()
 
         if should_regenerate_config:
-            self.render_build()
-            log.debug(f"Done rendering build for {self}, going to execute...")
+            self.render_build(service_names=service_names)
+            log.debug(f"Done rendering build for {self} (svcs: {service_names}), going to execute...")
 
         if debug:
             self.debug()
             return
 
         for script in self.scripts_to_run:
             # self.debug_template_output(script)
```

### Comparing `cocnc-0.1.0/src/cnc/models/config/config.py` & `cocnc-0.1.1/src/cnc/models/config/config.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/config/resource.py` & `cocnc-0.1.1/src/cnc/models/config/resource.py`

 * *Files 1% similar despite different names*

```diff
@@ -125,15 +125,15 @@
 
 class DatabaseResourceSettings(BaseResourceSettings):
     type: Literal["database"]
     engine: Optional[str] = "postgres"
     snapshot_file_path: Optional[str] = ""
     snapshot_type: Optional[str] = "data"
     raw_adapter: Optional[str] = Field(
-        alias="connection_string_adapter",
+        alias="adapter",
         default=None,
     )
     use_db_proxy: Optional[bool] = True
     version: Union[str, int, float]
 
     # ------------------------------
     # Properties
@@ -295,16 +295,16 @@
     def managed_secret_values_for_tf(self):
         db_url = self.database_url(self.database_password)
         if "@localhost" in db_url:
             db_url_p1, db_url_p2 = db_url.split("@localhost")
             db_url = f"{db_url_p1}@{self.host_output_tf_value_string}{db_url_p2}"
 
         return {
-            self.url_secret_id[:-2].split(":")[-1]: db_url,
-            self.password_secret_id[:-2].split(":")[-1]: self.database_password,
+            self.url_secret_id.replace("::", "").split(":")[-1]: db_url,
+            self.password_secret_id.replace("::", "").split(":")[-1]: self.database_password,
         }
 
     @property
     def database_password(self):
         if not hasattr(self, "_database_password"):
             if self.environment.database_password:
                 self._database_password = self.environment.database_password.value
@@ -538,14 +538,15 @@
     @property
     def managed_environment_variables(self):
         _env = self.common_managed_environment_variables
         _env.update(
             {
                 f"{self.env_var_base}_PORT": self.redis_port,
                 f"{self.env_var_base}_IP": self.redis_ip,
+                f"{self.env_var_base}_HOST": self.redis_ip,
                 f"{self.env_var_base}_URL": f"redis://{self.redis_ip}:{self.redis_port}",
                 "REDIS_URL": f"redis://{self.redis_ip}:{self.redis_port}",
             }
         )
         return _env
 
     @property
```

### Comparing `cocnc-0.1.0/src/cnc/models/config/service.py` & `cocnc-0.1.1/src/cnc/models/config/service.py`

 * *Files 2% similar despite different names*

```diff
@@ -376,7 +376,19 @@
         return f"{self.image_registry_url(run=run, region=region)}:{self.image_tag(environment_tag=environment_tag)}"
 
     def log_stream_prefix(self, task_name="web"):
         return f"{self.instance_name}-{task_name}"
 
     def toolbox_manager(self, environment_tag="latest"):
         return ToolboxManager(self, service_tags={self.name: environment_tag})
+
+    def cli_info(self):
+        _data = {
+            "name": self.name,
+            "type": self.settings.type,
+        }
+
+        if self.is_frontend or self.is_backend:
+            _data["url_path"] = self.settings.url_path 
+
+        return _data
+
```

### Comparing `cocnc-0.1.0/src/cnc/models/config/settings.py` & `cocnc-0.1.1/src/cnc/models/config/settings.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/cycle_stage_base.py` & `cocnc-0.1.1/src/cnc/models/cycle_stage_base.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/deployer.py` & `cocnc-0.1.1/src/cnc/models/deployer.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
             "service": service,
             "environment": self.environment,
             "stage": Stage.model_validate({"name": "deploy"}),
             "load_database_snapshot": False,
             "environment_items": self.environment_items,
         }
 
-    def render_scripts(self):
+    def render_scripts(self, service_names=None):
         context = self.template_context(None)
         if os.path.isfile(f"{self.config_files_path}/pre_deploy_functions.sh.j2"):
             self.write_template(
                 "pre_deploy_functions.sh.j2",
                 output_name=f"pre-deploy-{self.environment.name}-functions.sh",
                 context=context,
             )
@@ -36,14 +36,17 @@
                 "pre_deploy.sh.j2",
                 output_name=f"pre-deploy-{self.environment.name}.sh",
                 context=context,
             )
             self.scripts_to_run.append(f"pre-deploy-{self.environment.name}.sh")
 
         for service in self.environment.services:
+            if service_names:
+                if service.name not in service_names:
+                    continue
 
             if service.settings.is_resource:
                 continue
 
             context = self.template_context(service)
             context["render_template"] = self.write_template_with_context(service)
 
@@ -53,22 +56,22 @@
                 context=context,
             )
             self.write_template(
                 "main.sh.j2", output_name=f"deploy-{service.name}.sh", context=context
             )
             self.scripts_to_run.append(f"deploy-{service.name}.sh")
 
-    def perform(self, should_cleanup=True, should_regenerate_config=True, debug=False):
+    def perform(self, should_cleanup=True, should_regenerate_config=True, debug=False, service_names=None):
         log.debug(f"Performing deploy for {self} @ {self.config_files_path}")
         if should_cleanup:
             self.cleanup()
         self.setup()
         if should_regenerate_config:
-            self.render_scripts()
-            log.debug(f"Done rendering deploy for {self}, going to execute...")
+            self.render_scripts(service_names=service_names)
+            log.debug(f"Done rendering deploy for {self} (svcs: {service_names}), going to execute...")
 
         if debug:
             for script in self.scripts_to_run:
                 self.debug_template_output(script)
 
             log.debug(f"All done with debug for {self}")
             return
```

### Comparing `cocnc-0.1.0/src/cnc/models/environment.py` & `cocnc-0.1.1/src/cnc/models/environment.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/environment_collection.py` & `cocnc-0.1.1/src/cnc/models/environment_collection.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/environment_variable.py` & `cocnc-0.1.1/src/cnc/models/environment_variable.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/providers/amazon/custom_headers.py` & `cocnc-0.1.1/src/cnc/models/providers/amazon/custom_headers.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/providers/amazon/database_resource_settings.py` & `cocnc-0.1.1/src/cnc/models/providers/amazon/database_resource_settings.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/providers/amazon/deploy_resource_limits.py` & `cocnc-0.1.1/src/cnc/models/providers/amazon/deploy_resource_limits.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/providers/amazon/environment_collection.py` & `cocnc-0.1.1/src/cnc/models/providers/amazon/environment_collection.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/providers/google/cache_resource_settings.py` & `cocnc-0.1.1/src/cnc/models/providers/google/cache_resource_settings.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/providers/google/database_resource_settings.py` & `cocnc-0.1.1/src/cnc/models/providers/google/database_resource_settings.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/providers/google/deploy_resource_limits.py` & `cocnc-0.1.1/src/cnc/models/providers/google/deploy_resource_limits.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/providers/google/environment_collection.py` & `cocnc-0.1.1/src/cnc/models/providers/google/environment_collection.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/provisioner.py` & `cocnc-0.1.1/src/cnc/models/provisioner.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,16 +55,16 @@
     ):
         if should_cleanup:
             log.debug(f"Cleaning up & setting up at start for {self}")
 
             if not self.cleanup():
                 return False
 
-        if not self.setup():
-            return False
+            if not self.setup():
+                return False
 
         if should_regenerate_config:
             log.debug(
                 f"Writing {self.application.template_config.provision_filename} for {self}"
             )
             if not self.write_template(
                 self.application.template_config.provision_filename
```

### Comparing `cocnc-0.1.0/src/cnc/models/resource_use_existing.py` & `cocnc-0.1.1/src/cnc/models/resource_use_existing.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/stage.py` & `cocnc-0.1.1/src/cnc/models/stage.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/models/toolbox.py` & `cocnc-0.1.1/src/cnc/models/toolbox.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/tests/base_test_class.py` & `cocnc-0.1.1/src/cnc/tests/base_test_class.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_cidrs.yml` & `cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_cidrs.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_subnets.yml` & `cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_subnets.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/environments.yml` & `cocnc-0.1.1/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/environments.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/tests/test_builder.py` & `cocnc-0.1.1/src/cnc/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/tests/test_deployer.py` & `cocnc-0.1.1/src/cnc/tests/test_deployer.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/tests/test_environment_collection.py` & `cocnc-0.1.1/src/cnc/tests/test_environment_collection.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/tests/test_environment_variables.py` & `cocnc-0.1.1/src/cnc/tests/test_environment_variables.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/tests/test_environments.py` & `cocnc-0.1.1/src/cnc/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/tests/test_provisioner.py` & `cocnc-0.1.1/src/cnc/tests/test_provisioner.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/tests/test_services.py` & `cocnc-0.1.1/src/cnc/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/tests/test_toolbox.py` & `cocnc-0.1.1/src/cnc/tests/test_toolbox.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/src/cnc/utils/string.py` & `cocnc-0.1.1/src/cnc/utils/string.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.0/PKG-INFO` & `cocnc-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocnc
-Version: 0.1.0
+Version: 0.1.1
 Summary: CNC is the first framework for application deployment, a fully distributed and customizable PaaS developer experience, based on docker-compose config files
 Author: Adam Abdelaziz
 Author-email: adam.abdelaziz@withcoherence.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -38,30 +38,31 @@
 `cnc` is an open-source framework that equips developers with the tools to deploy applications with precision. Rooted in the principles of Infrastructure as Code (IaC) using terraform, `cnc` offers a flexible and cloud-agnostic abstraction that excels in managing deployments across various environments — whether it’s for development, staging, production, or ephemeral previews. For those who have used AWS's Amplify CLI, think of `cnc` as a broader, adaptable framework that supports your unique deployment needs.
 
 Core Lifecycle Events Managed by `cnc`:
 
 - Provision: Uses terraform to create, manage, and dismantle cloud resources, ensuring each environment is crafted to fit its specific purpose.
 - Build: Assembles the necessary deployment artifacts for each environment, from docker containers to static assets for web applications.
 - Deploy: Seamlessly updates infrastructure to deploy new artifacts, such as modifying k8s manifests or updating ECS services.
+- Toolbox: A `toolbox` is a managed shell against a `cnc`-managed envionment, making it easy to get a REPL or run database migrations, for example
 
 Getting Started with `cnc`:
 - Experience `cnc` in just a few minutes: install and see for yourself the power of cnc in under 5 minutes without needing any cloud permissions or incurring any costs.
 - Rapid Deployment: Have your first environment up and running in less than 15 minutes, demonstrating the straightforward power of cnc.
 
 `cnc` is designed not just as a tool, but as a partner in development, empowering you to build and manage your infrastructure with the same attention to detail and creativity that you bring to your code. Just like web devs use frameworks to build better products, with `cnc`, you gain the freedom to implement your vision precisely as intended, making each project not only functional but finely tuned to your standards.
 
 ## Getting Started
 
 ### Prerequisites
 
 Ensure that you have Docker installed, along with the `aws` or `gcloud` CLI tools, depending on your cloud provider.
 
-Intall `cnc` from the [PyPI Python Package Index](). For example, using `pip`:
+Intall `cnc` from the [PyPI Python Package Index](https://pypi.org/project/cocnc/). For example, using `pip`:
 ```
-pip install cnc
+pip install cocnc
 ```
 
 ### Annotate docker-compose.yml
 
 Mark the services that CNC should manage by adding the following snippet to your `docker-compose.yml`. You can annotate a subset of your existing `docker-compose.yml`, `cnc` will ignore services without the `x-cnc` extension.
 
 ```yaml
@@ -129,20 +130,27 @@
 cnc deploy perform dev --debug --no-cleanup
 ```
 
 Add a 2nd environment (e.g. `dev2`) to the `environments.yml` and run the commands again, see the power of the framework!
 
 ### Deploy your first environment
 
-Authenticate with your cloud provider using the aws or gcloud CLI, then deploy your environment with:
+Authenticate with your cloud provider using the aws or gcloud CLI, then create your infrastructure with:
 
 ```
-cnc cycle dev
+cnc provision apply
 ```
 
+deploy your `dev` environment with:
+```
+cnc update dev --service-tags app=v1
+```
+
+This will do a `build` and a `deploy` under the hood.
+
 For more details, see the step-by-step [Getting Started Guide](./docs/README.md).
 
 
 # Documentation
 
 Access full documentation and in-depth tutorials at [the CNC Documentation](./docs/README.md).
```

