# Comparing `tmp/cocnc-0.1.3.tar.gz` & `tmp/cocnc-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cocnc-0.1.3.tar", max compression
+gzip compressed data, was "cocnc-0.1.4.tar", max compression
```

## Comparing `cocnc-0.1.3.tar` & `cocnc-0.1.4.tar`

### file list

```diff
@@ -1,174 +1,174 @@
--rw-r--r--   0        0        0    35148 2024-04-02 18:10:45.243229 cocnc-0.1.3/LICENSE.txt
--rw-r--r--   0        0        0     5336 2024-05-16 00:58:59.838603 cocnc-0.1.3/README.md
--rw-r--r--   0        0        0      945 2024-05-16 20:14:23.594471 cocnc-0.1.3/pyproject.toml
--rw-r--r--   0        0        0      199 2024-05-12 00:57:28.450735 cocnc-0.1.3/src/cnc/__init__.py
--rw-r--r--   0        0        0      498 2024-05-12 00:57:28.450735 cocnc-0.1.3/src/cnc/check_dependencies.py
--rw-r--r--   0        0        0        0 2024-04-02 18:10:45.243229 cocnc-0.1.3/src/cnc/commands/__init__.py
--rw-r--r--   0        0        0     1590 2024-05-16 00:52:25.626595 cocnc-0.1.3/src/cnc/commands/build.py
--rw-r--r--   0        0        0     1545 2024-05-15 22:32:34.815388 cocnc-0.1.3/src/cnc/commands/deploy.py
--rw-r--r--   0        0        0     2409 2024-05-16 01:31:54.206647 cocnc-0.1.3/src/cnc/commands/info.py
--rw-r--r--   0        0        0     4136 2024-05-12 00:57:28.450735 cocnc-0.1.3/src/cnc/commands/provision.py
--rw-r--r--   0        0        0      753 2024-05-12 00:57:28.450735 cocnc-0.1.3/src/cnc/commands/render.py
--rw-r--r--   0        0        0      663 2024-04-02 18:10:45.243229 cocnc-0.1.3/src/cnc/commands/shell.py
--rw-r--r--   0        0        0     1079 2024-05-15 22:12:13.119371 cocnc-0.1.3/src/cnc/commands/telemetry.py
--rw-r--r--   0        0        0        0 2024-04-02 18:10:45.247229 cocnc-0.1.3/src/cnc/commands/template_editor/__init__.py
--rw-r--r--   0        0        0     5650 2024-05-14 18:02:38.226930 cocnc-0.1.3/src/cnc/commands/template_editor/inspector.py
--rw-r--r--   0        0        0     2956 2024-05-15 23:34:56.487440 cocnc-0.1.3/src/cnc/commands/toolbox.py
--rw-r--r--   0        0        0     1807 2024-05-16 01:03:27.678609 cocnc-0.1.3/src/cnc/commands/update.py
--rw-r--r--   0        0        0      739 2024-04-02 18:10:45.247229 cocnc-0.1.3/src/cnc/constants.py
--rw-r--r--   0        0        0     3780 2024-05-10 01:36:08.673102 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/build/build_functions.sh.j2
--rw-r--r--   0        0        0      689 2024-05-16 14:40:59.584350 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/build/main.sh.j2
--rw-r--r--   0        0        0       43 2024-04-02 18:10:45.247229 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/deploy_functions.sh.j2
--rw-r--r--   0        0        0     2427 2024-05-16 19:06:31.622612 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/ecs_web_task.json.j2
--rw-r--r--   0        0        0     1257 2024-05-01 01:07:56.387004 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/main.sh.j2
--rw-r--r--   0        0        0     1623 2024-05-01 01:07:56.387004 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy.sh.j2
--rw-r--r--   0        0        0     2468 2024-05-01 01:07:56.387004 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy_status_check.sh.j2
--rw-r--r--   0        0        0      766 2024-04-26 14:43:08.898875 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/partials/ecs_wait_with_retries.sh.j2
--rw-r--r--   0        0        0      645 2024-05-01 01:07:56.387004 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/partials/update_task_definition.sh.j2
--rw-r--r--   0        0        0      200 2024-05-01 01:07:56.387004 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy.sh.j2
--rw-r--r--   0        0        0     1047 2024-05-01 01:07:56.387004 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy_functions.sh.j2
--rw-r--r--   0        0        0     1478 2024-05-03 17:48:33.699163 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/base.tf.j2
--rw-r--r--   0        0        0      396 2024-04-02 18:10:45.247229 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/frontend_routing_lambda/index.js
--rw-r--r--   0        0        0      561 2024-04-26 14:43:08.902875 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/main.tf.j2
--rw-r--r--   0        0        0     4651 2024-04-26 14:43:08.902875 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/active_and_paused_envs.tf.j2
--rw-r--r--   0        0        0     5481 2024-04-26 14:43:08.906875 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_backend_deployments.tf.j2
--rw-r--r--   0        0        0     5640 2024-04-26 14:43:08.906875 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_deployments.tf.j2
--rw-r--r--   0        0        0     1759 2024-05-01 01:07:56.387004 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_frontend_deployments.tf.j2
--rw-r--r--   0        0        0    11529 2024-04-26 14:43:08.910875 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_backend_services.tf.j2
--rw-r--r--   0        0        0      813 2024-05-12 00:57:28.450735 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/collection/providers.tf.j2
--rw-r--r--   0        0        0     8800 2024-05-08 16:39:58.931845 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/collection/vpc_configuration.tf.j2
--rw-r--r--   0        0        0     1888 2024-05-12 00:57:28.450735 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/collection_level_resources.tf.j2
--rw-r--r--   0        0        0     1432 2024-04-26 14:43:08.918875 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/environment/efs.tf.j2
--rw-r--r--   0        0        0     1886 2024-04-02 18:10:45.251229 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/environment/msg_queue_and_obj_storage.tf.j2
--rw-r--r--   0        0        0    26090 2024-05-01 01:07:56.391004 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/environment_level_resources.tf.j2
--rw-r--r--   0        0        0     9699 2024-05-01 01:07:56.391004 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_backend.tf.j2
--rw-r--r--   0        0        0     6430 2024-04-26 14:43:08.922875 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_frontend.tf.j2
--rw-r--r--   0        0        0     2382 2024-05-01 01:07:56.391004 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/scheduled_tasks.tf.j2
--rw-r--r--   0        0        0     5446 2024-05-01 01:07:56.391004 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/workers.tf.j2
--rw-r--r--   0        0        0      965 2024-04-26 14:43:08.926875 cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/service_level_resources.tf.j2
--rw-r--r--   0        0        0    11326 2024-05-16 19:06:31.622612 cocnc-0.1.3/src/cnc/flavors/aws/shared/deploy/deploy_functions_base.sh.j2
--rw-r--r--   0        0        0      336 2024-05-10 01:36:08.677103 cocnc-0.1.3/src/cnc/flavors/aws/shared/toolbox/Dockerfile.j2
--rw-r--r--   0        0        0     4184 2024-05-01 01:07:56.391004 cocnc-0.1.3/src/cnc/flavors/aws/shared/toolbox/main.sh.j2
--rw-r--r--   0        0        0      615 2024-04-02 18:10:45.251229 cocnc-0.1.3/src/cnc/flavors/gcp/gke/1/deploy/deploy.sh.j2
--rw-r--r--   0        0        0      290 2024-04-26 14:43:08.930875 cocnc-0.1.3/src/cnc/flavors/gcp/gke/1/deploy/deploy_functions.sh.j2
--rw-r--r--   0        0        0     1953 2024-04-26 14:43:08.930875 cocnc-0.1.3/src/cnc/flavors/gcp/gke/1/provision/base.tf.j2
--rw-r--r--   0        0        0      561 2024-04-26 14:43:08.930875 cocnc-0.1.3/src/cnc/flavors/gcp/gke/1/provision/main.tf.j2
--rw-r--r--   0        0        0     1189 2024-04-26 14:43:08.930875 cocnc-0.1.3/src/cnc/flavors/gcp/gke/1/provision/partials/collection_level_resources.tf.j2
--rw-r--r--   0        0        0     4347 2024-04-26 14:43:08.930875 cocnc-0.1.3/src/cnc/flavors/gcp/gke/1/provision/partials/service_level_resources.tf.j2
--rw-r--r--   0        0        0      299 2024-04-02 18:10:45.251229 cocnc-0.1.3/src/cnc/flavors/gcp/run/1/build/main.sh.j2
--rw-r--r--   0        0        0      104 2024-04-02 18:10:45.251229 cocnc-0.1.3/src/cnc/flavors/gcp/run/1/cnc-flavor.yml
--rw-r--r--   0        0        0      661 2024-04-26 14:43:08.934875 cocnc-0.1.3/src/cnc/flavors/gcp/run/1/deploy/base.sh.j2
--rw-r--r--   0        0        0       43 2024-04-02 18:10:45.255229 cocnc-0.1.3/src/cnc/flavors/gcp/run/1/deploy/deploy_functions.sh.j2
--rw-r--r--   0        0        0      303 2024-04-02 18:10:45.255229 cocnc-0.1.3/src/cnc/flavors/gcp/run/1/deploy/main.sh.j2
--rw-r--r--   0        0        0     2512 2024-05-03 17:48:33.699163 cocnc-0.1.3/src/cnc/flavors/gcp/run/1/provision/base.tf.j2
--rw-r--r--   0        0        0      561 2024-04-26 14:43:08.934875 cocnc-0.1.3/src/cnc/flavors/gcp/run/1/provision/main.tf.j2
--rw-r--r--   0        0        0      299 2024-04-26 14:43:08.930875 cocnc-0.1.3/src/cnc/flavors/gcp/run-lite/1/build/main.sh.j2
--rw-r--r--   0        0        0      493 2024-04-26 14:43:08.934875 cocnc-0.1.3/src/cnc/flavors/gcp/run-lite/1/deploy/base.sh.j2
--rw-r--r--   0        0        0      331 2024-04-26 14:43:08.934875 cocnc-0.1.3/src/cnc/flavors/gcp/run-lite/1/deploy/deploy_functions.sh.j2
--rw-r--r--   0        0        0      303 2024-04-26 14:43:08.934875 cocnc-0.1.3/src/cnc/flavors/gcp/run-lite/1/deploy/main.sh.j2
--rw-r--r--   0        0        0     1778 2024-05-10 01:36:08.677103 cocnc-0.1.3/src/cnc/flavors/gcp/run-lite/1/deploy/run-container.yml.j2
--rw-r--r--   0        0        0     1364 2024-04-26 20:51:50.243437 cocnc-0.1.3/src/cnc/flavors/gcp/run-lite/1/provision/base.tf.j2
--rw-r--r--   0        0        0      561 2024-04-26 14:43:08.934875 cocnc-0.1.3/src/cnc/flavors/gcp/run-lite/1/provision/main.tf.j2
--rw-r--r--   0        0        0     1926 2024-05-01 01:07:56.391004 cocnc-0.1.3/src/cnc/flavors/gcp/run-lite/1/toolbox/main.sh.j2
--rw-r--r--   0        0        0      273 2024-05-01 01:07:56.391004 cocnc-0.1.3/src/cnc/flavors/gcp/shared/build/Dockerfile.run.j2
--rw-r--r--   0        0        0     1017 2024-05-01 01:07:56.391004 cocnc-0.1.3/src/cnc/flavors/gcp/shared/build/base.sh.j2
--rw-r--r--   0        0        0     4542 2024-05-15 23:31:32.787438 cocnc-0.1.3/src/cnc/flavors/gcp/shared/build/build_functions.sh.j2
--rw-r--r--   0        0        0     3555 2024-05-01 01:07:56.391004 cocnc-0.1.3/src/cnc/flavors/gcp/shared/build/nginx.conf.j2
--rw-r--r--   0        0        0       59 2024-04-26 14:43:08.938875 cocnc-0.1.3/src/cnc/flavors/gcp/shared/deploy/all-access-policy.yml.j2
--rw-r--r--   0        0        0     4572 2024-05-10 01:36:08.677103 cocnc-0.1.3/src/cnc/flavors/gcp/shared/deploy/deploy_functions_base.sh.j2
--rw-r--r--   0        0        0     2241 2024-05-16 17:25:36.526822 cocnc-0.1.3/src/cnc/flavors/gcp/shared/deploy/k8s/scheduled_tasks.yml
--rw-r--r--   0        0        0      828 2024-05-10 01:36:08.677103 cocnc-0.1.3/src/cnc/flavors/gcp/shared/deploy/k8s/service_containers/backend-worker.yml
--rw-r--r--   0        0        0     1391 2024-05-16 17:25:31.014822 cocnc-0.1.3/src/cnc/flavors/gcp/shared/deploy/k8s/workers.yml
--rw-r--r--   0        0        0     2083 2024-05-16 18:11:06.754727 cocnc-0.1.3/src/cnc/flavors/gcp/shared/deploy/run-container.yml.j2
--rw-r--r--   0        0        0      165 2024-05-16 17:03:33.710868 cocnc-0.1.3/src/cnc/flavors/gcp/shared/deploy/run-job.yml.j2
--rw-r--r--   0        0        0      278 2024-04-26 14:43:08.942875 cocnc-0.1.3/src/cnc/flavors/gcp/shared/deploy/run-svc.yml.j2
--rw-r--r--   0        0        0     1496 2024-04-26 14:43:08.942875 cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/collection/bastion_instance.tf.j2
--rw-r--r--   0        0        0     3790 2024-05-16 17:27:07.502819 cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/collection/common_setup_resources.tf.j2
--rw-r--r--   0        0        0     2503 2024-05-01 01:07:56.391004 cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/collection/default_service.tf.j2
--rw-r--r--   0        0        0     3338 2024-05-16 17:47:05.282777 cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/collection/gke_cluster.tf.j2
--rw-r--r--   0        0        0      794 2024-05-16 17:30:03.578813 cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/collection/providers.tf.j2
--rw-r--r--   0        0        0     8353 2024-05-01 01:07:56.391004 cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/collection/vpc_networking.tf.j2
--rw-r--r--   0        0        0     3584 2024-05-01 01:07:56.391004 cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/environment/database_resources.tf.j2
--rw-r--r--   0        0        0     1332 2024-04-26 20:51:50.247437 cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/environment/object_storage_resources.tf.j2
--rw-r--r--   0        0        0      463 2024-04-26 14:43:08.942875 cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/environment/resource_managed_secrets.tf.j2
--rw-r--r--   0        0        0     1142 2024-04-26 20:51:50.251437 cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/service/cache.tf.j2
--rw-r--r--   0        0        0     1342 2024-05-10 01:36:08.677103 cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service.tf.j2
--rw-r--r--   0        0        0     1755 2024-04-26 14:43:08.946875 cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service_networking.tf.j2
--rw-r--r--   0        0        0      332 2024-05-10 01:36:08.677103 cocnc-0.1.3/src/cnc/flavors/gcp/shared/toolbox/Dockerfile.j2
--rw-r--r--   0        0        0     4484 2024-05-15 15:08:21.561546 cocnc-0.1.3/src/cnc/flavors/gcp/shared/toolbox/main.sh.j2
--rw-r--r--   0        0        0      913 2024-05-12 00:57:28.450735 cocnc-0.1.3/src/cnc/logger.py
--rw-r--r--   0        0        0     2120 2024-05-16 00:59:53.626605 cocnc-0.1.3/src/cnc/main.py
--rw-r--r--   0        0        0      426 2024-04-26 14:43:08.946875 cocnc-0.1.3/src/cnc/models/__init__.py
--rw-r--r--   0        0        0     4488 2024-05-12 00:57:28.450735 cocnc-0.1.3/src/cnc/models/application.py
--rw-r--r--   0        0        0      906 2024-05-12 00:57:28.454735 cocnc-0.1.3/src/cnc/models/base_model.py
--rw-r--r--   0        0        0     3088 2024-05-15 21:55:12.227357 cocnc-0.1.3/src/cnc/models/builder.py
--rw-r--r--   0        0        0       30 2024-04-02 18:10:45.255229 cocnc-0.1.3/src/cnc/models/config/__init__.py
--rw-r--r--   0        0        0     7925 2024-05-16 16:39:24.730918 cocnc-0.1.3/src/cnc/models/config/config.py
--rw-r--r--   0        0        0      324 2024-05-12 00:57:28.454735 cocnc-0.1.3/src/cnc/models/config/deploy_resource_limits.py
--rw-r--r--   0        0        0    17833 2024-05-15 22:25:07.115382 cocnc-0.1.3/src/cnc/models/config/resource.py
--rw-r--r--   0        0        0    11842 2024-05-16 19:06:31.622612 cocnc-0.1.3/src/cnc/models/config/service.py
--rw-r--r--   0        0        0    10437 2024-05-12 00:57:28.458735 cocnc-0.1.3/src/cnc/models/config/settings.py
--rw-r--r--   0        0        0      119 2024-04-02 18:10:45.255229 cocnc-0.1.3/src/cnc/models/config/utils.py
--rw-r--r--   0        0        0      257 2024-04-26 14:43:08.946875 cocnc-0.1.3/src/cnc/models/custom_header.py
--rw-r--r--   0        0        0     8616 2024-05-12 00:57:28.458735 cocnc-0.1.3/src/cnc/models/cycle_stage_base.py
--rw-r--r--   0        0        0     3692 2024-05-15 21:55:16.643357 cocnc-0.1.3/src/cnc/models/deployer.py
--rw-r--r--   0        0        0     8062 2024-05-14 18:02:38.226930 cocnc-0.1.3/src/cnc/models/environment.py
--rw-r--r--   0        0        0    10525 2024-05-16 20:13:29.850473 cocnc-0.1.3/src/cnc/models/environment_collection.py
--rw-r--r--   0        0        0     3646 2024-05-14 18:02:38.226930 cocnc-0.1.3/src/cnc/models/environment_variable.py
--rw-r--r--   0        0        0        0 2024-04-02 18:10:45.259229 cocnc-0.1.3/src/cnc/models/providers/__init__.py
--rw-r--r--   0        0        0      288 2024-04-26 20:51:50.255437 cocnc-0.1.3/src/cnc/models/providers/amazon/__init__.py
--rw-r--r--   0        0        0      485 2024-05-12 00:57:28.458735 cocnc-0.1.3/src/cnc/models/providers/amazon/cache_resource_settings.py
--rw-r--r--   0        0        0     7166 2024-05-12 00:57:28.458735 cocnc-0.1.3/src/cnc/models/providers/amazon/custom_headers.py
--rw-r--r--   0        0        0     3187 2024-05-12 00:57:28.458735 cocnc-0.1.3/src/cnc/models/providers/amazon/database_resource_settings.py
--rw-r--r--   0        0        0     3377 2024-05-12 00:57:28.458735 cocnc-0.1.3/src/cnc/models/providers/amazon/deploy_resource_limits.py
--rw-r--r--   0        0        0     5379 2024-05-14 18:02:38.226930 cocnc-0.1.3/src/cnc/models/providers/amazon/environment_collection.py
--rw-r--r--   0        0        0      168 2024-04-02 18:10:45.259229 cocnc-0.1.3/src/cnc/models/providers/amazon/service_account.py
--rw-r--r--   0        0        0      190 2024-04-26 20:51:50.255437 cocnc-0.1.3/src/cnc/models/providers/google/__init__.py
--rw-r--r--   0        0        0      756 2024-04-26 20:51:50.255437 cocnc-0.1.3/src/cnc/models/providers/google/cache_resource_settings.py
--rw-r--r--   0        0        0     2074 2024-05-12 00:57:28.462735 cocnc-0.1.3/src/cnc/models/providers/google/database_resource_settings.py
--rw-r--r--   0        0        0     2837 2024-05-12 00:57:28.462735 cocnc-0.1.3/src/cnc/models/providers/google/deploy_resource_limits.py
--rw-r--r--   0        0        0     9942 2024-05-14 18:02:38.226930 cocnc-0.1.3/src/cnc/models/providers/google/environment_collection.py
--rw-r--r--   0        0        0        0 2024-04-02 18:10:45.259229 cocnc-0.1.3/src/cnc/models/providers/google/service_account.py
--rw-r--r--   0        0        0    14435 2024-05-16 19:43:29.858535 cocnc-0.1.3/src/cnc/models/provisioner.py
--rw-r--r--   0        0        0      802 2024-04-26 14:43:08.958875 cocnc-0.1.3/src/cnc/models/resource_use_existing.py
--rw-r--r--   0        0        0      779 2024-04-02 18:10:45.259229 cocnc-0.1.3/src/cnc/models/stage.py
--rw-r--r--   0        0        0     4279 2024-05-12 00:57:28.462735 cocnc-0.1.3/src/cnc/models/toolbox.py
--rw-r--r--   0        0        0        0 2024-04-02 18:10:45.259229 cocnc-0.1.3/src/cnc/tests/__init__.py
--rw-r--r--   0        0        0     1071 2024-05-05 23:59:45.934092 cocnc-0.1.3/src/cnc/tests/base_test_class.py
--rw-r--r--   0        0        0       75 2024-05-05 23:59:45.938092 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service/cnc.yml
--rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-1-db/cnc.yml
--rw-r--r--   0        0        0      609 2024-04-26 14:43:08.958875 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_cidrs.yml
--rw-r--r--   0        0        0      673 2024-04-26 14:43:08.958875 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_subnets.yml
--rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-1-db-both-use-existing/cnc.yml
--rw-r--r--   0        0        0      472 2024-04-02 18:10:45.259229 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-1-db-both-use-existing/environments.yml
--rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-1-db-use-existing/cnc.yml
--rw-r--r--   0        0        0      379 2024-04-02 18:10:45.259229 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-1-db-use-existing/environments.yml
--rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/cnc.yml
--rw-r--r--   0        0        0      564 2024-04-02 18:10:45.259229 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/environments.yml
--rw-r--r--   0        0        0      231 2024-05-05 23:59:45.934092 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-2-db/cnc.yml
--rw-r--r--   0        0        0      231 2024-05-05 23:59:45.934092 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/cnc.yml
--rw-r--r--   0        0        0      373 2024-04-02 18:10:45.259229 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments.yml
--rw-r--r--   0        0        0      479 2024-04-02 18:10:45.259229 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments_aws_ecs.yml
--rw-r--r--   0        0        0      392 2024-04-26 14:43:08.962875 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments_gcp_run_region_settings.yml
--rw-r--r--   0        0        0       75 2024-05-05 23:59:45.934092 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-custom/cnc.yml
--rw-r--r--   0        0        0       22 2024-04-26 14:43:08.962875 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-custom/custom/deploy/main.sh.j2
--rw-r--r--   0        0        0      341 2024-04-26 14:43:08.962875 cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-custom/environments.yml
--rw-r--r--   0        0        0      228 2024-05-05 23:59:45.938092 cocnc-0.1.3/src/cnc/tests/fixtures/backend-2-service-1-db/cnc.yml
--rw-r--r--   0        0        0      322 2024-05-05 23:59:45.938092 cocnc-0.1.3/src/cnc/tests/fixtures/backend-2-service-2-db/cnc.yml
--rw-r--r--   0        0        0      153 2024-05-05 23:59:45.938092 cocnc-0.1.3/src/cnc/tests/fixtures/shared/cnc.yml
--rw-r--r--   0        0        0      340 2024-05-05 23:59:45.938092 cocnc-0.1.3/src/cnc/tests/fixtures/shared/environments-custom-provision.yml
--rw-r--r--   0        0        0      294 2024-04-02 18:10:45.259229 cocnc-0.1.3/src/cnc/tests/fixtures/shared/environments.yml
--rw-r--r--   0        0        0      400 2024-04-02 18:10:45.259229 cocnc-0.1.3/src/cnc/tests/fixtures/shared/environments_aws_ecs.yml
--rw-r--r--   0        0        0      474 2024-04-26 14:43:08.962875 cocnc-0.1.3/src/cnc/tests/fixtures/shared/environments_aws_ecs_existing_vpc.yml
--rw-r--r--   0        0        0      299 2024-04-26 14:43:08.962875 cocnc-0.1.3/src/cnc/tests/fixtures/shared/environments_gcp_run_lite.yml
--rw-r--r--   0        0        0     5373 2024-05-14 18:02:38.226930 cocnc-0.1.3/src/cnc/tests/test_builder.py
--rw-r--r--   0        0        0     2683 2024-05-14 18:02:38.226930 cocnc-0.1.3/src/cnc/tests/test_deployer.py
--rw-r--r--   0        0        0     2445 2024-05-14 18:02:38.226930 cocnc-0.1.3/src/cnc/tests/test_environment_collection.py
--rw-r--r--   0        0        0     2287 2024-05-14 18:02:38.226930 cocnc-0.1.3/src/cnc/tests/test_environment_variables.py
--rw-r--r--   0        0        0     1872 2024-05-14 18:02:38.226930 cocnc-0.1.3/src/cnc/tests/test_environments.py
--rw-r--r--   0        0        0    13574 2024-05-12 00:57:28.462735 cocnc-0.1.3/src/cnc/tests/test_provisioner.py
--rw-r--r--   0        0        0     2898 2024-05-16 18:50:06.514646 cocnc-0.1.3/src/cnc/tests/test_services.py
--rw-r--r--   0        0        0     2224 2024-05-12 00:57:28.462735 cocnc-0.1.3/src/cnc/tests/test_toolbox.py
--rw-r--r--   0        0        0       38 2024-04-26 14:43:08.966875 cocnc-0.1.3/src/cnc/utils/__init__.py
--rw-r--r--   0        0        0      625 2024-04-26 14:43:08.966875 cocnc-0.1.3/src/cnc/utils/string.py
--rw-r--r--   0        0        0     6422 1970-01-01 00:00:00.000000 cocnc-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0    35148 2024-04-02 18:10:45.243229 cocnc-0.1.4/LICENSE.txt
+-rw-r--r--   0        0        0     5336 2024-05-16 00:58:59.838603 cocnc-0.1.4/README.md
+-rw-r--r--   0        0        0      945 2024-05-16 21:11:50.094351 cocnc-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0      199 2024-05-12 00:57:28.450735 cocnc-0.1.4/src/cnc/__init__.py
+-rw-r--r--   0        0        0      498 2024-05-12 00:57:28.450735 cocnc-0.1.4/src/cnc/check_dependencies.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:10:45.243229 cocnc-0.1.4/src/cnc/commands/__init__.py
+-rw-r--r--   0        0        0     1590 2024-05-16 00:52:25.626595 cocnc-0.1.4/src/cnc/commands/build.py
+-rw-r--r--   0        0        0     1545 2024-05-15 22:32:34.815388 cocnc-0.1.4/src/cnc/commands/deploy.py
+-rw-r--r--   0        0        0     2409 2024-05-16 01:31:54.206647 cocnc-0.1.4/src/cnc/commands/info.py
+-rw-r--r--   0        0        0     4136 2024-05-12 00:57:28.450735 cocnc-0.1.4/src/cnc/commands/provision.py
+-rw-r--r--   0        0        0      753 2024-05-12 00:57:28.450735 cocnc-0.1.4/src/cnc/commands/render.py
+-rw-r--r--   0        0        0      663 2024-04-02 18:10:45.243229 cocnc-0.1.4/src/cnc/commands/shell.py
+-rw-r--r--   0        0        0     1079 2024-05-15 22:12:13.119371 cocnc-0.1.4/src/cnc/commands/telemetry.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:10:45.247229 cocnc-0.1.4/src/cnc/commands/template_editor/__init__.py
+-rw-r--r--   0        0        0     5650 2024-05-14 18:02:38.226930 cocnc-0.1.4/src/cnc/commands/template_editor/inspector.py
+-rw-r--r--   0        0        0     2956 2024-05-15 23:34:56.487440 cocnc-0.1.4/src/cnc/commands/toolbox.py
+-rw-r--r--   0        0        0     1807 2024-05-16 01:03:27.678609 cocnc-0.1.4/src/cnc/commands/update.py
+-rw-r--r--   0        0        0      739 2024-04-02 18:10:45.247229 cocnc-0.1.4/src/cnc/constants.py
+-rw-r--r--   0        0        0     3780 2024-05-10 01:36:08.673102 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/build/build_functions.sh.j2
+-rw-r--r--   0        0        0      689 2024-05-16 14:40:59.584350 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/build/main.sh.j2
+-rw-r--r--   0        0        0       43 2024-04-02 18:10:45.247229 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/deploy_functions.sh.j2
+-rw-r--r--   0        0        0     2427 2024-05-16 19:06:31.622612 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/ecs_web_task.json.j2
+-rw-r--r--   0        0        0     1257 2024-05-01 01:07:56.387004 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/main.sh.j2
+-rw-r--r--   0        0        0     1623 2024-05-01 01:07:56.387004 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy.sh.j2
+-rw-r--r--   0        0        0     2468 2024-05-01 01:07:56.387004 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy_status_check.sh.j2
+-rw-r--r--   0        0        0      766 2024-04-26 14:43:08.898875 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/partials/ecs_wait_with_retries.sh.j2
+-rw-r--r--   0        0        0      645 2024-05-01 01:07:56.387004 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/partials/update_task_definition.sh.j2
+-rw-r--r--   0        0        0      200 2024-05-01 01:07:56.387004 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy.sh.j2
+-rw-r--r--   0        0        0     1047 2024-05-01 01:07:56.387004 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy_functions.sh.j2
+-rw-r--r--   0        0        0     1478 2024-05-03 17:48:33.699163 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/base.tf.j2
+-rw-r--r--   0        0        0      396 2024-04-02 18:10:45.247229 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/frontend_routing_lambda/index.js
+-rw-r--r--   0        0        0      561 2024-04-26 14:43:08.902875 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/main.tf.j2
+-rw-r--r--   0        0        0     4651 2024-04-26 14:43:08.902875 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/active_and_paused_envs.tf.j2
+-rw-r--r--   0        0        0     5481 2024-04-26 14:43:08.906875 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_backend_deployments.tf.j2
+-rw-r--r--   0        0        0     5640 2024-04-26 14:43:08.906875 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_deployments.tf.j2
+-rw-r--r--   0        0        0     1759 2024-05-01 01:07:56.387004 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_frontend_deployments.tf.j2
+-rw-r--r--   0        0        0    11529 2024-04-26 14:43:08.910875 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_backend_services.tf.j2
+-rw-r--r--   0        0        0      813 2024-05-12 00:57:28.450735 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/collection/providers.tf.j2
+-rw-r--r--   0        0        0     8800 2024-05-08 16:39:58.931845 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/collection/vpc_configuration.tf.j2
+-rw-r--r--   0        0        0     1888 2024-05-12 00:57:28.450735 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/collection_level_resources.tf.j2
+-rw-r--r--   0        0        0     1432 2024-04-26 14:43:08.918875 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/environment/efs.tf.j2
+-rw-r--r--   0        0        0     1886 2024-04-02 18:10:45.251229 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/environment/msg_queue_and_obj_storage.tf.j2
+-rw-r--r--   0        0        0    26090 2024-05-01 01:07:56.391004 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/environment_level_resources.tf.j2
+-rw-r--r--   0        0        0     9699 2024-05-01 01:07:56.391004 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_backend.tf.j2
+-rw-r--r--   0        0        0     6430 2024-04-26 14:43:08.922875 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_frontend.tf.j2
+-rw-r--r--   0        0        0     2382 2024-05-01 01:07:56.391004 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/scheduled_tasks.tf.j2
+-rw-r--r--   0        0        0     5446 2024-05-01 01:07:56.391004 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/workers.tf.j2
+-rw-r--r--   0        0        0      965 2024-04-26 14:43:08.926875 cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/service_level_resources.tf.j2
+-rw-r--r--   0        0        0    11326 2024-05-16 19:06:31.622612 cocnc-0.1.4/src/cnc/flavors/aws/shared/deploy/deploy_functions_base.sh.j2
+-rw-r--r--   0        0        0      336 2024-05-10 01:36:08.677103 cocnc-0.1.4/src/cnc/flavors/aws/shared/toolbox/Dockerfile.j2
+-rw-r--r--   0        0        0     4184 2024-05-01 01:07:56.391004 cocnc-0.1.4/src/cnc/flavors/aws/shared/toolbox/main.sh.j2
+-rw-r--r--   0        0        0      615 2024-04-02 18:10:45.251229 cocnc-0.1.4/src/cnc/flavors/gcp/gke/1/deploy/deploy.sh.j2
+-rw-r--r--   0        0        0      290 2024-04-26 14:43:08.930875 cocnc-0.1.4/src/cnc/flavors/gcp/gke/1/deploy/deploy_functions.sh.j2
+-rw-r--r--   0        0        0     1953 2024-04-26 14:43:08.930875 cocnc-0.1.4/src/cnc/flavors/gcp/gke/1/provision/base.tf.j2
+-rw-r--r--   0        0        0      561 2024-04-26 14:43:08.930875 cocnc-0.1.4/src/cnc/flavors/gcp/gke/1/provision/main.tf.j2
+-rw-r--r--   0        0        0     1189 2024-04-26 14:43:08.930875 cocnc-0.1.4/src/cnc/flavors/gcp/gke/1/provision/partials/collection_level_resources.tf.j2
+-rw-r--r--   0        0        0     4347 2024-04-26 14:43:08.930875 cocnc-0.1.4/src/cnc/flavors/gcp/gke/1/provision/partials/service_level_resources.tf.j2
+-rw-r--r--   0        0        0      299 2024-04-02 18:10:45.251229 cocnc-0.1.4/src/cnc/flavors/gcp/run/1/build/main.sh.j2
+-rw-r--r--   0        0        0      104 2024-04-02 18:10:45.251229 cocnc-0.1.4/src/cnc/flavors/gcp/run/1/cnc-flavor.yml
+-rw-r--r--   0        0        0      661 2024-04-26 14:43:08.934875 cocnc-0.1.4/src/cnc/flavors/gcp/run/1/deploy/base.sh.j2
+-rw-r--r--   0        0        0       43 2024-04-02 18:10:45.255229 cocnc-0.1.4/src/cnc/flavors/gcp/run/1/deploy/deploy_functions.sh.j2
+-rw-r--r--   0        0        0      303 2024-04-02 18:10:45.255229 cocnc-0.1.4/src/cnc/flavors/gcp/run/1/deploy/main.sh.j2
+-rw-r--r--   0        0        0     2512 2024-05-03 17:48:33.699163 cocnc-0.1.4/src/cnc/flavors/gcp/run/1/provision/base.tf.j2
+-rw-r--r--   0        0        0      561 2024-04-26 14:43:08.934875 cocnc-0.1.4/src/cnc/flavors/gcp/run/1/provision/main.tf.j2
+-rw-r--r--   0        0        0      299 2024-04-26 14:43:08.930875 cocnc-0.1.4/src/cnc/flavors/gcp/run-lite/1/build/main.sh.j2
+-rw-r--r--   0        0        0      493 2024-04-26 14:43:08.934875 cocnc-0.1.4/src/cnc/flavors/gcp/run-lite/1/deploy/base.sh.j2
+-rw-r--r--   0        0        0      331 2024-04-26 14:43:08.934875 cocnc-0.1.4/src/cnc/flavors/gcp/run-lite/1/deploy/deploy_functions.sh.j2
+-rw-r--r--   0        0        0      303 2024-04-26 14:43:08.934875 cocnc-0.1.4/src/cnc/flavors/gcp/run-lite/1/deploy/main.sh.j2
+-rw-r--r--   0        0        0     1778 2024-05-10 01:36:08.677103 cocnc-0.1.4/src/cnc/flavors/gcp/run-lite/1/deploy/run-container.yml.j2
+-rw-r--r--   0        0        0     1364 2024-04-26 20:51:50.243437 cocnc-0.1.4/src/cnc/flavors/gcp/run-lite/1/provision/base.tf.j2
+-rw-r--r--   0        0        0      561 2024-04-26 14:43:08.934875 cocnc-0.1.4/src/cnc/flavors/gcp/run-lite/1/provision/main.tf.j2
+-rw-r--r--   0        0        0     1926 2024-05-01 01:07:56.391004 cocnc-0.1.4/src/cnc/flavors/gcp/run-lite/1/toolbox/main.sh.j2
+-rw-r--r--   0        0        0      273 2024-05-01 01:07:56.391004 cocnc-0.1.4/src/cnc/flavors/gcp/shared/build/Dockerfile.run.j2
+-rw-r--r--   0        0        0     1017 2024-05-01 01:07:56.391004 cocnc-0.1.4/src/cnc/flavors/gcp/shared/build/base.sh.j2
+-rw-r--r--   0        0        0     4542 2024-05-15 23:31:32.787438 cocnc-0.1.4/src/cnc/flavors/gcp/shared/build/build_functions.sh.j2
+-rw-r--r--   0        0        0     3555 2024-05-01 01:07:56.391004 cocnc-0.1.4/src/cnc/flavors/gcp/shared/build/nginx.conf.j2
+-rw-r--r--   0        0        0       59 2024-04-26 14:43:08.938875 cocnc-0.1.4/src/cnc/flavors/gcp/shared/deploy/all-access-policy.yml.j2
+-rw-r--r--   0        0        0     4572 2024-05-10 01:36:08.677103 cocnc-0.1.4/src/cnc/flavors/gcp/shared/deploy/deploy_functions_base.sh.j2
+-rw-r--r--   0        0        0     2241 2024-05-16 17:25:36.526822 cocnc-0.1.4/src/cnc/flavors/gcp/shared/deploy/k8s/scheduled_tasks.yml
+-rw-r--r--   0        0        0      828 2024-05-10 01:36:08.677103 cocnc-0.1.4/src/cnc/flavors/gcp/shared/deploy/k8s/service_containers/backend-worker.yml
+-rw-r--r--   0        0        0     1391 2024-05-16 17:25:31.014822 cocnc-0.1.4/src/cnc/flavors/gcp/shared/deploy/k8s/workers.yml
+-rw-r--r--   0        0        0     2083 2024-05-16 18:11:06.754727 cocnc-0.1.4/src/cnc/flavors/gcp/shared/deploy/run-container.yml.j2
+-rw-r--r--   0        0        0      165 2024-05-16 17:03:33.710868 cocnc-0.1.4/src/cnc/flavors/gcp/shared/deploy/run-job.yml.j2
+-rw-r--r--   0        0        0      278 2024-04-26 14:43:08.942875 cocnc-0.1.4/src/cnc/flavors/gcp/shared/deploy/run-svc.yml.j2
+-rw-r--r--   0        0        0     1496 2024-04-26 14:43:08.942875 cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/collection/bastion_instance.tf.j2
+-rw-r--r--   0        0        0     3790 2024-05-16 17:27:07.502819 cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/collection/common_setup_resources.tf.j2
+-rw-r--r--   0        0        0     2503 2024-05-01 01:07:56.391004 cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/collection/default_service.tf.j2
+-rw-r--r--   0        0        0     3338 2024-05-16 17:47:05.282777 cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/collection/gke_cluster.tf.j2
+-rw-r--r--   0        0        0      794 2024-05-16 17:30:03.578813 cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/collection/providers.tf.j2
+-rw-r--r--   0        0        0     8353 2024-05-01 01:07:56.391004 cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/collection/vpc_networking.tf.j2
+-rw-r--r--   0        0        0     3584 2024-05-01 01:07:56.391004 cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/environment/database_resources.tf.j2
+-rw-r--r--   0        0        0     1332 2024-04-26 20:51:50.247437 cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/environment/object_storage_resources.tf.j2
+-rw-r--r--   0        0        0      463 2024-04-26 14:43:08.942875 cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/environment/resource_managed_secrets.tf.j2
+-rw-r--r--   0        0        0     1142 2024-04-26 20:51:50.251437 cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/service/cache.tf.j2
+-rw-r--r--   0        0        0     1342 2024-05-10 01:36:08.677103 cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service.tf.j2
+-rw-r--r--   0        0        0     1755 2024-04-26 14:43:08.946875 cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service_networking.tf.j2
+-rw-r--r--   0        0        0      332 2024-05-10 01:36:08.677103 cocnc-0.1.4/src/cnc/flavors/gcp/shared/toolbox/Dockerfile.j2
+-rw-r--r--   0        0        0     4484 2024-05-15 15:08:21.561546 cocnc-0.1.4/src/cnc/flavors/gcp/shared/toolbox/main.sh.j2
+-rw-r--r--   0        0        0      913 2024-05-12 00:57:28.450735 cocnc-0.1.4/src/cnc/logger.py
+-rw-r--r--   0        0        0     2120 2024-05-16 00:59:53.626605 cocnc-0.1.4/src/cnc/main.py
+-rw-r--r--   0        0        0      426 2024-04-26 14:43:08.946875 cocnc-0.1.4/src/cnc/models/__init__.py
+-rw-r--r--   0        0        0     4488 2024-05-12 00:57:28.450735 cocnc-0.1.4/src/cnc/models/application.py
+-rw-r--r--   0        0        0      906 2024-05-12 00:57:28.454735 cocnc-0.1.4/src/cnc/models/base_model.py
+-rw-r--r--   0        0        0     3088 2024-05-15 21:55:12.227357 cocnc-0.1.4/src/cnc/models/builder.py
+-rw-r--r--   0        0        0       30 2024-04-02 18:10:45.255229 cocnc-0.1.4/src/cnc/models/config/__init__.py
+-rw-r--r--   0        0        0     7925 2024-05-16 16:39:24.730918 cocnc-0.1.4/src/cnc/models/config/config.py
+-rw-r--r--   0        0        0      324 2024-05-12 00:57:28.454735 cocnc-0.1.4/src/cnc/models/config/deploy_resource_limits.py
+-rw-r--r--   0        0        0    17833 2024-05-15 22:25:07.115382 cocnc-0.1.4/src/cnc/models/config/resource.py
+-rw-r--r--   0        0        0    11842 2024-05-16 19:06:31.622612 cocnc-0.1.4/src/cnc/models/config/service.py
+-rw-r--r--   0        0        0    10437 2024-05-12 00:57:28.458735 cocnc-0.1.4/src/cnc/models/config/settings.py
+-rw-r--r--   0        0        0      119 2024-04-02 18:10:45.255229 cocnc-0.1.4/src/cnc/models/config/utils.py
+-rw-r--r--   0        0        0      257 2024-04-26 14:43:08.946875 cocnc-0.1.4/src/cnc/models/custom_header.py
+-rw-r--r--   0        0        0     8616 2024-05-12 00:57:28.458735 cocnc-0.1.4/src/cnc/models/cycle_stage_base.py
+-rw-r--r--   0        0        0     3692 2024-05-15 21:55:16.643357 cocnc-0.1.4/src/cnc/models/deployer.py
+-rw-r--r--   0        0        0     8062 2024-05-14 18:02:38.226930 cocnc-0.1.4/src/cnc/models/environment.py
+-rw-r--r--   0        0        0    10653 2024-05-16 21:07:31.686360 cocnc-0.1.4/src/cnc/models/environment_collection.py
+-rw-r--r--   0        0        0     3646 2024-05-14 18:02:38.226930 cocnc-0.1.4/src/cnc/models/environment_variable.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:10:45.259229 cocnc-0.1.4/src/cnc/models/providers/__init__.py
+-rw-r--r--   0        0        0      288 2024-04-26 20:51:50.255437 cocnc-0.1.4/src/cnc/models/providers/amazon/__init__.py
+-rw-r--r--   0        0        0      485 2024-05-12 00:57:28.458735 cocnc-0.1.4/src/cnc/models/providers/amazon/cache_resource_settings.py
+-rw-r--r--   0        0        0     7166 2024-05-12 00:57:28.458735 cocnc-0.1.4/src/cnc/models/providers/amazon/custom_headers.py
+-rw-r--r--   0        0        0     3187 2024-05-12 00:57:28.458735 cocnc-0.1.4/src/cnc/models/providers/amazon/database_resource_settings.py
+-rw-r--r--   0        0        0     3377 2024-05-12 00:57:28.458735 cocnc-0.1.4/src/cnc/models/providers/amazon/deploy_resource_limits.py
+-rw-r--r--   0        0        0     5379 2024-05-14 18:02:38.226930 cocnc-0.1.4/src/cnc/models/providers/amazon/environment_collection.py
+-rw-r--r--   0        0        0      168 2024-04-02 18:10:45.259229 cocnc-0.1.4/src/cnc/models/providers/amazon/service_account.py
+-rw-r--r--   0        0        0      190 2024-04-26 20:51:50.255437 cocnc-0.1.4/src/cnc/models/providers/google/__init__.py
+-rw-r--r--   0        0        0      756 2024-04-26 20:51:50.255437 cocnc-0.1.4/src/cnc/models/providers/google/cache_resource_settings.py
+-rw-r--r--   0        0        0     2074 2024-05-12 00:57:28.462735 cocnc-0.1.4/src/cnc/models/providers/google/database_resource_settings.py
+-rw-r--r--   0        0        0     2837 2024-05-12 00:57:28.462735 cocnc-0.1.4/src/cnc/models/providers/google/deploy_resource_limits.py
+-rw-r--r--   0        0        0     9942 2024-05-14 18:02:38.226930 cocnc-0.1.4/src/cnc/models/providers/google/environment_collection.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:10:45.259229 cocnc-0.1.4/src/cnc/models/providers/google/service_account.py
+-rw-r--r--   0        0        0    14435 2024-05-16 19:43:29.858535 cocnc-0.1.4/src/cnc/models/provisioner.py
+-rw-r--r--   0        0        0      802 2024-04-26 14:43:08.958875 cocnc-0.1.4/src/cnc/models/resource_use_existing.py
+-rw-r--r--   0        0        0      779 2024-04-02 18:10:45.259229 cocnc-0.1.4/src/cnc/models/stage.py
+-rw-r--r--   0        0        0     4279 2024-05-12 00:57:28.462735 cocnc-0.1.4/src/cnc/models/toolbox.py
+-rw-r--r--   0        0        0        0 2024-04-02 18:10:45.259229 cocnc-0.1.4/src/cnc/tests/__init__.py
+-rw-r--r--   0        0        0     1071 2024-05-05 23:59:45.934092 cocnc-0.1.4/src/cnc/tests/base_test_class.py
+-rw-r--r--   0        0        0       75 2024-05-05 23:59:45.938092 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service/cnc.yml
+-rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-1-db/cnc.yml
+-rw-r--r--   0        0        0      609 2024-04-26 14:43:08.958875 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_cidrs.yml
+-rw-r--r--   0        0        0      673 2024-04-26 14:43:08.958875 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_subnets.yml
+-rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-1-db-both-use-existing/cnc.yml
+-rw-r--r--   0        0        0      472 2024-04-02 18:10:45.259229 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-1-db-both-use-existing/environments.yml
+-rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-1-db-use-existing/cnc.yml
+-rw-r--r--   0        0        0      379 2024-04-02 18:10:45.259229 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-1-db-use-existing/environments.yml
+-rw-r--r--   0        0        0      153 2024-05-05 23:59:45.934092 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/cnc.yml
+-rw-r--r--   0        0        0      564 2024-04-02 18:10:45.259229 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/environments.yml
+-rw-r--r--   0        0        0      231 2024-05-05 23:59:45.934092 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-2-db/cnc.yml
+-rw-r--r--   0        0        0      231 2024-05-05 23:59:45.934092 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/cnc.yml
+-rw-r--r--   0        0        0      373 2024-04-02 18:10:45.259229 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments.yml
+-rw-r--r--   0        0        0      479 2024-04-02 18:10:45.259229 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments_aws_ecs.yml
+-rw-r--r--   0        0        0      392 2024-04-26 14:43:08.962875 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-2-db-2-envs/environments_gcp_run_region_settings.yml
+-rw-r--r--   0        0        0       75 2024-05-05 23:59:45.934092 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-custom/cnc.yml
+-rw-r--r--   0        0        0       22 2024-04-26 14:43:08.962875 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-custom/custom/deploy/main.sh.j2
+-rw-r--r--   0        0        0      341 2024-04-26 14:43:08.962875 cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-custom/environments.yml
+-rw-r--r--   0        0        0      228 2024-05-05 23:59:45.938092 cocnc-0.1.4/src/cnc/tests/fixtures/backend-2-service-1-db/cnc.yml
+-rw-r--r--   0        0        0      322 2024-05-05 23:59:45.938092 cocnc-0.1.4/src/cnc/tests/fixtures/backend-2-service-2-db/cnc.yml
+-rw-r--r--   0        0        0      153 2024-05-05 23:59:45.938092 cocnc-0.1.4/src/cnc/tests/fixtures/shared/cnc.yml
+-rw-r--r--   0        0        0      340 2024-05-05 23:59:45.938092 cocnc-0.1.4/src/cnc/tests/fixtures/shared/environments-custom-provision.yml
+-rw-r--r--   0        0        0      294 2024-04-02 18:10:45.259229 cocnc-0.1.4/src/cnc/tests/fixtures/shared/environments.yml
+-rw-r--r--   0        0        0      400 2024-04-02 18:10:45.259229 cocnc-0.1.4/src/cnc/tests/fixtures/shared/environments_aws_ecs.yml
+-rw-r--r--   0        0        0      474 2024-04-26 14:43:08.962875 cocnc-0.1.4/src/cnc/tests/fixtures/shared/environments_aws_ecs_existing_vpc.yml
+-rw-r--r--   0        0        0      299 2024-04-26 14:43:08.962875 cocnc-0.1.4/src/cnc/tests/fixtures/shared/environments_gcp_run_lite.yml
+-rw-r--r--   0        0        0     5373 2024-05-14 18:02:38.226930 cocnc-0.1.4/src/cnc/tests/test_builder.py
+-rw-r--r--   0        0        0     2683 2024-05-14 18:02:38.226930 cocnc-0.1.4/src/cnc/tests/test_deployer.py
+-rw-r--r--   0        0        0     2445 2024-05-14 18:02:38.226930 cocnc-0.1.4/src/cnc/tests/test_environment_collection.py
+-rw-r--r--   0        0        0     2287 2024-05-14 18:02:38.226930 cocnc-0.1.4/src/cnc/tests/test_environment_variables.py
+-rw-r--r--   0        0        0     1872 2024-05-14 18:02:38.226930 cocnc-0.1.4/src/cnc/tests/test_environments.py
+-rw-r--r--   0        0        0    13574 2024-05-12 00:57:28.462735 cocnc-0.1.4/src/cnc/tests/test_provisioner.py
+-rw-r--r--   0        0        0     2898 2024-05-16 18:50:06.514646 cocnc-0.1.4/src/cnc/tests/test_services.py
+-rw-r--r--   0        0        0     2224 2024-05-12 00:57:28.462735 cocnc-0.1.4/src/cnc/tests/test_toolbox.py
+-rw-r--r--   0        0        0       38 2024-04-26 14:43:08.966875 cocnc-0.1.4/src/cnc/utils/__init__.py
+-rw-r--r--   0        0        0      625 2024-04-26 14:43:08.966875 cocnc-0.1.4/src/cnc/utils/string.py
+-rw-r--r--   0        0        0     6422 1970-01-01 00:00:00.000000 cocnc-0.1.4/PKG-INFO
```

### Comparing `cocnc-0.1.3/LICENSE.txt` & `cocnc-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/README.md` & `cocnc-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/pyproject.toml` & `cocnc-0.1.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cocnc"
-version = "0.1.3"
+version = "0.1.4"
 description = "CNC is the first framework for application deployment, a fully distributed and customizable PaaS developer experience, based on docker-compose config files"
 authors = [
     "Adam Abdelaziz <adam.abdelaziz@withcoherence.com>",
     "Zachary Zaro <zach@withcoherence.com>",
 ]
 readme = "README.md"
 packages = [
```

### Comparing `cocnc-0.1.3/src/cnc/commands/build.py` & `cocnc-0.1.4/src/cnc/commands/build.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/commands/deploy.py` & `cocnc-0.1.4/src/cnc/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/commands/info.py` & `cocnc-0.1.4/src/cnc/commands/info.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/commands/provision.py` & `cocnc-0.1.4/src/cnc/commands/provision.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/commands/render.py` & `cocnc-0.1.4/src/cnc/commands/render.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/commands/shell.py` & `cocnc-0.1.4/src/cnc/commands/shell.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/commands/telemetry.py` & `cocnc-0.1.4/src/cnc/commands/telemetry.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/commands/template_editor/inspector.py` & `cocnc-0.1.4/src/cnc/commands/template_editor/inspector.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/commands/toolbox.py` & `cocnc-0.1.4/src/cnc/commands/toolbox.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/commands/update.py` & `cocnc-0.1.4/src/cnc/commands/update.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/constants.py` & `cocnc-0.1.4/src/cnc/constants.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/build/build_functions.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/build/build_functions.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/build/main.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/build/main.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/ecs_web_task.json.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/ecs_web_task.json.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/main.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/main.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy_status_check.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/partials/backend_deploy_status_check.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/partials/ecs_wait_with_retries.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/partials/ecs_wait_with_retries.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/partials/update_task_definition.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/partials/update_task_definition.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy_functions.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/deploy/pre_deploy_functions.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/base.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/base.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/main.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/main.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/active_and_paused_envs.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/active_and_paused_envs.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_backend_deployments.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_backend_deployments.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_deployments.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_deployments.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_frontend_deployments.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_active_frontend_deployments.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_backend_services.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/collection/has_backend_services.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/collection/providers.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/collection/providers.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/collection/vpc_configuration.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/collection/vpc_configuration.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/collection_level_resources.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/collection_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/environment/efs.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/environment/efs.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/environment/msg_queue_and_obj_storage.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/environment/msg_queue_and_obj_storage.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/environment_level_resources.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/environment_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_backend.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_backend.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_frontend.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/service/active_frontend.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/scheduled_tasks.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/scheduled_tasks.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/workers.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/service/backend/workers.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/ecs/1/provision/partials/service_level_resources.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/ecs/1/provision/partials/service_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/shared/deploy/deploy_functions_base.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/shared/deploy/deploy_functions_base.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/aws/shared/toolbox/main.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/aws/shared/toolbox/main.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/gke/1/deploy/deploy.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/gke/1/deploy/deploy.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/gke/1/provision/base.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/gke/1/provision/base.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/gke/1/provision/main.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/gke/1/provision/main.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/gke/1/provision/partials/collection_level_resources.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/gke/1/provision/partials/collection_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/gke/1/provision/partials/service_level_resources.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/gke/1/provision/partials/service_level_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/run/1/deploy/base.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/run/1/deploy/base.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/run/1/provision/base.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/run/1/provision/base.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/run/1/provision/main.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/run/1/provision/main.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/run-lite/1/deploy/run-container.yml.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/run-lite/1/deploy/run-container.yml.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/run-lite/1/provision/base.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/run-lite/1/provision/base.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/run-lite/1/provision/main.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/run-lite/1/provision/main.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/run-lite/1/toolbox/main.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/run-lite/1/toolbox/main.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/build/base.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/build/base.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/build/build_functions.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/build/build_functions.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/build/nginx.conf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/build/nginx.conf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/deploy/deploy_functions_base.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/deploy/deploy_functions_base.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/deploy/k8s/scheduled_tasks.yml` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/deploy/k8s/scheduled_tasks.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/deploy/k8s/service_containers/backend-worker.yml` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/deploy/k8s/service_containers/backend-worker.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/deploy/k8s/workers.yml` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/deploy/k8s/workers.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/deploy/run-container.yml.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/deploy/run-container.yml.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/collection/bastion_instance.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/collection/bastion_instance.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/collection/common_setup_resources.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/collection/common_setup_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/collection/default_service.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/collection/default_service.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/collection/gke_cluster.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/collection/gke_cluster.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/collection/providers.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/collection/providers.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/collection/vpc_networking.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/collection/vpc_networking.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/environment/database_resources.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/environment/database_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/environment/object_storage_resources.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/environment/object_storage_resources.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/service/cache.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/service/cache.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service_networking.tf.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/provision/partials/service/cloud_run_service_networking.tf.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/flavors/gcp/shared/toolbox/main.sh.j2` & `cocnc-0.1.4/src/cnc/flavors/gcp/shared/toolbox/main.sh.j2`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/logger.py` & `cocnc-0.1.4/src/cnc/logger.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/main.py` & `cocnc-0.1.4/src/cnc/main.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/application.py` & `cocnc-0.1.4/src/cnc/models/application.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/base_model.py` & `cocnc-0.1.4/src/cnc/models/base_model.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/builder.py` & `cocnc-0.1.4/src/cnc/models/builder.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/config/config.py` & `cocnc-0.1.4/src/cnc/models/config/config.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/config/resource.py` & `cocnc-0.1.4/src/cnc/models/config/resource.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/config/service.py` & `cocnc-0.1.4/src/cnc/models/config/service.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/config/settings.py` & `cocnc-0.1.4/src/cnc/models/config/settings.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/cycle_stage_base.py` & `cocnc-0.1.4/src/cnc/models/cycle_stage_base.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/deployer.py` & `cocnc-0.1.4/src/cnc/models/deployer.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/environment.py` & `cocnc-0.1.4/src/cnc/models/environment.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/environment_collection.py` & `cocnc-0.1.4/src/cnc/models/environment_collection.py`

 * *Files 2% similar despite different names*

```diff
@@ -296,14 +296,15 @@
 
         return sorted(_all, key=lambda x: x.settings.unique_id)
 
     def get_terraform_output(self, output_name, force_cache_refresh=False):
         _config = None
 
         if "infrastructure_outputs" not in self.data:
+            log.debug(f"Going to get outputs for {self}: {self.data}")
             try:
                 if (not hasattr(self, "_infra_outputs_cache")) or force_cache_refresh:
                     _config = ProvisionStageManager(
                         self,
                         output_only=True,
                     )
                     _config.make_ready_for_use()
@@ -311,14 +312,16 @@
             except Exception as e:
                 log.debug(f"Cannot get TF output ({output_name}) for {self}: {e}")
                 if not hasattr(self, "_infra_outputs_cache"):
                     self._infra_outputs_cache = {}
             finally:
                 if _config:
                     _config.cleanup()
+        else:
+            self._infra_outputs_cache = {}
 
         infra_outputs = {}
         infra_outputs.update(self.data.get("infrastructure_outputs", {}))
         infra_outputs.update(self._infra_outputs_cache)
 
         return infra_outputs.get(output_name, {}).get("value", "")
```

### Comparing `cocnc-0.1.3/src/cnc/models/environment_variable.py` & `cocnc-0.1.4/src/cnc/models/environment_variable.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/providers/amazon/custom_headers.py` & `cocnc-0.1.4/src/cnc/models/providers/amazon/custom_headers.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/providers/amazon/database_resource_settings.py` & `cocnc-0.1.4/src/cnc/models/providers/amazon/database_resource_settings.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/providers/amazon/deploy_resource_limits.py` & `cocnc-0.1.4/src/cnc/models/providers/amazon/deploy_resource_limits.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/providers/amazon/environment_collection.py` & `cocnc-0.1.4/src/cnc/models/providers/amazon/environment_collection.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/providers/google/cache_resource_settings.py` & `cocnc-0.1.4/src/cnc/models/providers/google/cache_resource_settings.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/providers/google/database_resource_settings.py` & `cocnc-0.1.4/src/cnc/models/providers/google/database_resource_settings.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/providers/google/deploy_resource_limits.py` & `cocnc-0.1.4/src/cnc/models/providers/google/deploy_resource_limits.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/providers/google/environment_collection.py` & `cocnc-0.1.4/src/cnc/models/providers/google/environment_collection.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/provisioner.py` & `cocnc-0.1.4/src/cnc/models/provisioner.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/resource_use_existing.py` & `cocnc-0.1.4/src/cnc/models/resource_use_existing.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/stage.py` & `cocnc-0.1.4/src/cnc/models/stage.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/models/toolbox.py` & `cocnc-0.1.4/src/cnc/models/toolbox.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/tests/base_test_class.py` & `cocnc-0.1.4/src/cnc/tests/base_test_class.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_cidrs.yml` & `cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_cidrs.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_subnets.yml` & `cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-1-db/environments_aws_ecs_existing_vpc_subnets.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/environments.yml` & `cocnc-0.1.4/src/cnc/tests/fixtures/backend-1-service-1-db-variables-aliases/environments.yml`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/tests/test_builder.py` & `cocnc-0.1.4/src/cnc/tests/test_builder.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/tests/test_deployer.py` & `cocnc-0.1.4/src/cnc/tests/test_deployer.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/tests/test_environment_collection.py` & `cocnc-0.1.4/src/cnc/tests/test_environment_collection.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/tests/test_environment_variables.py` & `cocnc-0.1.4/src/cnc/tests/test_environment_variables.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/tests/test_environments.py` & `cocnc-0.1.4/src/cnc/tests/test_environments.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/tests/test_provisioner.py` & `cocnc-0.1.4/src/cnc/tests/test_provisioner.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/tests/test_services.py` & `cocnc-0.1.4/src/cnc/tests/test_services.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/tests/test_toolbox.py` & `cocnc-0.1.4/src/cnc/tests/test_toolbox.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/src/cnc/utils/string.py` & `cocnc-0.1.4/src/cnc/utils/string.py`

 * *Files identical despite different names*

### Comparing `cocnc-0.1.3/PKG-INFO` & `cocnc-0.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cocnc
-Version: 0.1.3
+Version: 0.1.4
 Summary: CNC is the first framework for application deployment, a fully distributed and customizable PaaS developer experience, based on docker-compose config files
 Author: Adam Abdelaziz
 Author-email: adam.abdelaziz@withcoherence.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

