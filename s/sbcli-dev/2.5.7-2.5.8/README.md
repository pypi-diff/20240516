# Comparing `tmp/sbcli_dev-2.5.7.zip` & `tmp/sbcli_dev-2.5.8.zip`

## zipinfo {}

```diff
@@ -1,148 +1,148 @@
-Zip file size: 213899 bytes, number of entries: 146
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 11:03 sbcli_dev-2.5.7/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 11:03 sbcli_dev-2.5.7/sbcli_dev.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/
--rw-r--r--  2.0 unx     2269 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/setup.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/README.md
--rw-r--r--  2.0 unx      148 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/env_var
--rw-r--r--  2.0 unx       84 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/pyproject.toml
--rw-r--r--  2.0 unx       38 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/setup.cfg
--rw-r--r--  2.0 unx     1489 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/PKG-INFO
--rw-r--r--  2.0 unx    77873 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_cli/main.py
--rw-r--r--  2.0 unx        1 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/sbcli_dev.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     5188 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/sbcli_dev.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       49 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/sbcli_dev.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1489 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/sbcli_dev.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       73 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/sbcli_dev.egg-info/requires.txt
--rw-r--r--  2.0 unx       55 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/sbcli_dev.egg-info/entry_points.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/
--rw-r--r--  2.0 unx    66264 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1501 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3153 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     3638 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx      279 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx      938 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3193 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     8343 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     7640 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/utils.py
--rw-r--r--  2.0 unx    23423 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx     5112 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    21493 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     7504 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx     2189 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx     3203 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     5462 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx      229 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     5268 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     2410 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5140 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx     7439 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2423 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     4118 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx      837 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2671 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6577 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/services/storage_node_monitor.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx      930 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx      152 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx     5333 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx       54 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx     4409 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
--rw-r--r--  2.0 unx      453 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx     1782 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx      311 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx      118 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx      360 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx       43 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1420 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx      311 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/prometheus.yml
--rwxr-xr-x  2.0 unx      657 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx    25433 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1856 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx   106705 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx   799409 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/node-exporter.json
--rw-r--r--  2.0 unx    99758 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    99862 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/pools.json
--rw-r--r--  2.0 unx    13877 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1120 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     3191 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx     1521 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1630 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    10557 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx    10375 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1900 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx    23245 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx    47534 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx    11294 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx     1500 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx      806 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4846 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      917 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx      736 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     1602 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     1228 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     1020 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx     3696 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     4242 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     2565 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx     3766 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     2094 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_core/models/nvme_device.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/
--rw-r--r--  2.0 unx      725 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     5098 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx      703 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     1263 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     2513 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      507 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      322 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      434 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      827 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx     1302 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     2905 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5547 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     4883 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5491 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     9573 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx     8547 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx    11244 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx    12198 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx      975 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     6326 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     8075 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     2940 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     5274 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx     6206 b- defN 24-May-09 11:03 sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_pool.py
-146 files, 1927349 bytes uncompressed, 187321 bytes compressed:  90.3%
+Zip file size: 212734 bytes, number of entries: 146
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 19:29 sbcli_dev-2.5.8/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 19:29 sbcli_dev-2.5.8/sbcli_dev.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/README.md
+-rw-r--r--  2.0 unx       84 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/pyproject.toml
+-rw-r--r--  2.0 unx     1489 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/PKG-INFO
+-rw-r--r--  2.0 unx      148 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/env_var
+-rw-r--r--  2.0 unx       38 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/setup.cfg
+-rw-r--r--  2.0 unx     2269 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/setup.py
+-rw-r--r--  2.0 unx    77873 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_cli/main.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/templates/
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      703 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx      717 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx     2513 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/app.py
+-rw-r--r--  2.0 unx      725 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx      322 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx      507 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      434 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_pool.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     8547 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx     9565 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx     5274 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     8075 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     4883 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5547 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     5491 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx      975 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     2905 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5188 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/sbcli_dev.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       73 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/sbcli_dev.egg-info/requires.txt
+-rw-r--r--  2.0 unx     1489 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/sbcli_dev.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       49 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/sbcli_dev.egg-info/top_level.txt
+-rw-r--r--  2.0 unx       55 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/sbcli_dev.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/sbcli_dev.egg-info/dependency_links.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/
+-rw-r--r--  2.0 unx    23423 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx      938 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8343 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    21493 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx     7504 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx      279 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx     3638 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx    66205 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1501 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx      229 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx      837 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     4118 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx     7439 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     5268 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6577 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/storage_node_monitor.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     5140 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx    47534 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10557 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx     3191 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx    11294 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx    13877 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx    23245 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2094 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/nvme_device.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx      917 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      736 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     3696 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx      806 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/models/port_stat.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx     1420 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx     1782 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx       43 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx      118 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx     5333 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx      152 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/set_db_config.sh
+-rwxr-xr-x  2.0 unx      657 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/prometheus.yml
+-rw-r--r--  2.0 unx      311 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx     4409 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+-rw-r--r--  2.0 unx      930 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx       54 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx    25433 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1856 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx    88820 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    88911 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    88776 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    88868 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/pools.json
+-rw-r--r--  2.0 unx   799409 b- defN 24-May-16 19:29 sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/node-exporter.json
+146 files, 1876625 bytes uncompressed, 186156 bytes compressed:  90.1%
```

## zipnote {}

```diff
@@ -1,439 +1,439 @@
-Filename: sbcli_dev-2.5.7/
+Filename: sbcli_dev-2.5.8/
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_cli/
+Filename: sbcli_dev-2.5.8/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_dev-2.5.7/sbcli_dev.egg-info/
+Filename: sbcli_dev-2.5.8/simplyblock_web/
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/
+Filename: sbcli_dev-2.5.8/sbcli_dev.egg-info/
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/
+Filename: sbcli_dev-2.5.8/simplyblock_core/
 Comment: 
 
-Filename: sbcli_dev-2.5.7/setup.py
+Filename: sbcli_dev-2.5.8/README.md
 Comment: 
 
-Filename: sbcli_dev-2.5.7/README.md
+Filename: sbcli_dev-2.5.8/pyproject.toml
 Comment: 
 
-Filename: sbcli_dev-2.5.7/env_var
+Filename: sbcli_dev-2.5.8/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.5.7/pyproject.toml
+Filename: sbcli_dev-2.5.8/env_var
 Comment: 
 
-Filename: sbcli_dev-2.5.7/setup.cfg
+Filename: sbcli_dev-2.5.8/setup.cfg
 Comment: 
 
-Filename: sbcli_dev-2.5.7/PKG-INFO
+Filename: sbcli_dev-2.5.8/setup.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_cli/cli.py
+Filename: sbcli_dev-2.5.8/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_cli/main.py
+Filename: sbcli_dev-2.5.8/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/sbcli_dev.egg-info/dependency_links.txt
+Filename: sbcli_dev-2.5.8/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_dev-2.5.7/sbcli_dev.egg-info/SOURCES.txt
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_dev-2.5.7/sbcli_dev.egg-info/top_level.txt
+Filename: sbcli_dev-2.5.8/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_dev-2.5.7/sbcli_dev.egg-info/PKG-INFO
+Filename: sbcli_dev-2.5.8/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/sbcli_dev.egg-info/requires.txt
+Filename: sbcli_dev-2.5.8/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/sbcli_dev.egg-info/entry_points.txt
+Filename: sbcli_dev-2.5.8/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/
+Filename: sbcli_dev-2.5.8/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/
+Filename: sbcli_dev-2.5.8/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/
+Filename: sbcli_dev-2.5.8/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/
+Filename: sbcli_dev-2.5.8/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/storage_node_ops.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/constants.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/cnode_client.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/shell_utils.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/pci_utils.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/__init__.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/snode_client.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/kv_store.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/utils.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/cluster_ops.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/compute_node_ops.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/rpc_client.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/distr_controller.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/health_check_service.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/service_template.service
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/remove_service.sh
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/device_monitor.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/__init__.py
+Filename: sbcli_dev-2.5.8/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/install_service.sh
+Filename: sbcli_dev-2.5.8/sbcli_dev.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_dev-2.5.8/sbcli_dev.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_dev-2.5.8/sbcli_dev.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_dev-2.5.8/sbcli_dev.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/alerting/
+Filename: sbcli_dev-2.5.8/sbcli_dev.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/
+Filename: sbcli_dev-2.5.8/sbcli_dev.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_dev-2.5.8/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_dev-2.5.8/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+Filename: sbcli_dev-2.5.8/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_dev-2.5.8/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/__init__.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_dev-2.5.8/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_dev-2.5.8/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_dev-2.5.8/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_dev-2.5.8/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_dev-2.5.8/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_dev-2.5.8/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_dev-2.5.8/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_dev-2.5.8/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_dev-2.5.8/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/node-exporter.json
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/pools.json
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/device_events.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/__init__.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/events.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/iface.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/base_model.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/lvol_model.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/compute_node.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/snapshot.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/pool.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/global_settings.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/port_stat.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/storage_node.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/__init__.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/stats.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/cluster.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/caching_node.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_core/models/nvme_device.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/static/
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/templates/
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/node_utils.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/snode_app.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/app.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/auth_middleware.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/__init__.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/caching_node_app.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/utils.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/node_webapp.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/static/tst.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/static/is_up.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/static/delete.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/static/deploy.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/static/rpac.yaml
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/static/list_deps.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/csi.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/pools.json
 Comment: 
 
-Filename: sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/node-exporter.json
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_dev-2.5.7/setup.py` & `sbcli_dev-2.5.8/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/README.md` & `sbcli_dev-2.5.8/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/PKG-INFO` & `sbcli_dev-2.5.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.5.7
+Version: 2.5.8
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.5.7/simplyblock_cli/cli.py` & `sbcli_dev-2.5.8/simplyblock_cli/cli.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/sbcli_dev.egg-info/SOURCES.txt` & `sbcli_dev-2.5.8/sbcli_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/sbcli_dev.egg-info/PKG-INFO` & `sbcli_dev-2.5.8/sbcli_dev.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.5.7
+Version: 2.5.8
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_dev-2.5.7/simplyblock_core/storage_node_ops.py` & `sbcli_dev-2.5.8/simplyblock_core/storage_node_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -1185,21 +1185,18 @@
 
     logger.info("Shutting down node")
     old_status = snode.status
     snode.status = StorageNode.STATUS_IN_SHUTDOWN
     snode.write_to_db(db_controller.kv_store)
     storage_events.snode_status_change(snode, snode.status, old_status)
 
-    logger.debug("Setting LVols to offline")
+    logger.debug("Removing LVols")
     for lvol_id in snode.lvols:
         logger.debug(lvol_id)
-        lvol = db_controller.get_lvol_by_id(lvol_id)
-        if lvol:
-            lvol.status = lvol.STATUS_OFFLINE
-            lvol.write_to_db(db_controller.kv_store)
+        lvol_controller.delete_lvol_from_node(lvol_id, snode.get_id(), clear_data=False)
 
     for dev in snode.nvme_devices:
         if dev.status in [NVMeDevice.STATUS_ONLINE, NVMeDevice.STATUS_READONLY]:
             device_controller.device_set_unavailable(dev.get_id())
     distr_controller.send_node_status_event(snode.get_id(), "in_shutdown")
 
     # shutdown node
@@ -1209,14 +1206,15 @@
         distr_controller.disconnect_device(dev)
 
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password)
 
     # delete jm
+    logger.info("Removing JM")
     rpc_client.bdev_jm_delete(f"jm_{snode.get_id()}")
 
     logger.info("Stopping SPDK")
     snode_api = SNodeClient(snode.api_endpoint)
     results, err = snode_api.spdk_process_kill()
 
     distr_controller.send_node_status_event(snode.get_id(), StorageNode.STATUS_OFFLINE)
```

## Comparing `sbcli_dev-2.5.7/simplyblock_core/constants.py` & `sbcli_dev-2.5.8/simplyblock_core/constants.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/mgmt_node_ops.py` & `sbcli_dev-2.5.8/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/cnode_client.py` & `sbcli_dev-2.5.8/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/pci_utils.py` & `sbcli_dev-2.5.8/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/snode_client.py` & `sbcli_dev-2.5.8/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/kv_store.py` & `sbcli_dev-2.5.8/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/utils.py` & `sbcli_dev-2.5.8/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/cluster_ops.py` & `sbcli_dev-2.5.8/simplyblock_core/cluster_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/compute_node_ops.py` & `sbcli_dev-2.5.8/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/rpc_client.py` & `sbcli_dev-2.5.8/simplyblock_core/rpc_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/distr_controller.py` & `sbcli_dev-2.5.8/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/services/lvol_monitor.py` & `sbcli_dev-2.5.8/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/services/caching_node_monitor.py` & `sbcli_dev-2.5.8/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/services/health_check_service.py` & `sbcli_dev-2.5.8/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_dev-2.5.8/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/services/log_agg_service.py` & `sbcli_dev-2.5.8/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/services/distr_event_collector.py` & `sbcli_dev-2.5.8/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_dev-2.5.8/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/services/port_stat_collector.py` & `sbcli_dev-2.5.8/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/services/device_monitor.py` & `sbcli_dev-2.5.8/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/services/__init__.py` & `sbcli_dev-2.5.8/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/services/install_service.sh` & `sbcli_dev-2.5.8/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_dev-2.5.8/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/services/cap_monitor.py` & `sbcli_dev-2.5.8/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/services/storage_node_monitor.py` & `sbcli_dev-2.5.8/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_dev-2.5.8/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/haproxy.cfg` & `sbcli_dev-2.5.8/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_dev-2.5.8/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_dev-2.5.8/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml` & `sbcli_dev-2.5.8/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/__init__.py` & `sbcli_dev-2.5.8/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/install_deps.sh` & `sbcli_dev-2.5.8/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_dev-2.5.8/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_dev-2.5.8/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_dev-2.5.8/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/devices.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.997343982514881%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'bytes'}}}, 2: "*

 * *                "{'fieldConfig': {'defaults': {'unit': 'bytes'}}}, 3: {'fieldConfig': {'defaults': "*

 * *                "{'unit': 'bytes'}}}, 4: {'fieldConfig': {'defaults': {'unit': 'bytes'}}}, 5: "*

 * *                "{'fieldConfig': {'defaults': {'unit': 'percent'}}}, 6: {'fieldConfig': "*

 * *                "{'defaults': {'unit': 'percent'}}}, 8: {'fieldConfig': {'defaults': {'unit': "*

 * *                "'bytes'}}}, 9: {'fieldCon […]*

```diff
@@ -86,15 +86,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -179,15 +179,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -272,15 +272,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 8,
                     "x": 14,
@@ -365,15 +365,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -458,15 +458,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "percent"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -551,15 +551,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "percent"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 8,
                     "x": 14,
@@ -657,15 +657,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -750,15 +750,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "Bps"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
@@ -843,15 +843,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "ns"
+                        "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 8,
                     "x": 14,
@@ -1225,15 +1225,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -1318,15 +1318,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "Bps"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
@@ -1410,15 +1410,16 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 8,
                     "x": 14,
@@ -1726,898 +1727,606 @@
                         "refId": "A"
                     }
                 ],
                 "title": "device_read_latency_ticks",
                 "type": "timeseries"
             },
             {
-                "collapsed": true,
+                "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
                     "x": 0,
                     "y": 48
                 },
                 "id": 29,
-                "panels": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
+                "panels": [],
+                "title": "unmap",
+                "type": "row"
+            },
+            {
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
                         },
-                        "fieldConfig": {
-                            "defaults": {
-                                "color": {
-                                    "mode": "palette-classic"
-                                },
-                                "custom": {
-                                    "axisCenteredZero": false,
-                                    "axisColorMode": "text",
-                                    "axisLabel": "",
-                                    "axisPlacement": "auto",
-                                    "barAlignment": 0,
-                                    "drawStyle": "line",
-                                    "fillOpacity": 0,
-                                    "gradientMode": "none",
-                                    "hideFrom": {
-                                        "legend": false,
-                                        "tooltip": false,
-                                        "viz": false
-                                    },
-                                    "lineInterpolation": "linear",
-                                    "lineWidth": 1,
-                                    "pointSize": 5,
-                                    "scaleDistribution": {
-                                        "type": "linear"
-                                    },
-                                    "showPoints": "auto",
-                                    "spanNulls": false,
-                                    "stacking": {
-                                        "group": "A",
-                                        "mode": "none"
-                                    },
-                                    "thresholdsStyle": {
-                                        "mode": "off"
-                                    }
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
                                 },
-                                "mappings": [],
-                                "thresholds": {
-                                    "mode": "absolute",
-                                    "steps": [
-                                        {
-                                            "color": "green",
-                                            "value": null
-                                        },
-                                        {
-                                            "color": "red",
-                                            "value": 80
-                                        }
-                                    ]
-                                }
-                            },
-                            "overrides": []
-                        },
-                        "gridPos": {
-                            "h": 7,
-                            "w": 7,
-                            "x": 0,
-                            "y": 48
-                        },
-                        "id": 21,
-                        "options": {
-                            "legend": {
-                                "calcs": [],
-                                "displayMode": "list",
-                                "placement": "bottom",
-                                "showLegend": true
-                            },
-                            "tooltip": {
-                                "mode": "single",
-                                "sort": "none"
-                            }
-                        },
-                        "targets": [
-                            {
-                                "datasource": {
-                                    "type": "prometheus",
-                                    "uid": "PBFA97CFB590B2093"
-                                },
-                                "editorMode": "builder",
-                                "expr": "device_unmap_latency_ticks",
-                                "legendFormat": "__auto",
-                                "range": true,
-                                "refId": "A"
-                            }
-                        ],
-                        "title": "device_unmap_latency_ticks",
-                        "type": "timeseries"
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        }
                     },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 0,
+                    "y": 49
+                },
+                "id": 21,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "fieldConfig": {
-                            "defaults": {
-                                "color": {
-                                    "mode": "palette-classic"
-                                },
-                                "custom": {
-                                    "axisCenteredZero": false,
-                                    "axisColorMode": "text",
-                                    "axisLabel": "",
-                                    "axisPlacement": "auto",
-                                    "barAlignment": 0,
-                                    "drawStyle": "line",
-                                    "fillOpacity": 0,
-                                    "gradientMode": "none",
-                                    "hideFrom": {
-                                        "legend": false,
-                                        "tooltip": false,
-                                        "viz": false
-                                    },
-                                    "lineInterpolation": "linear",
-                                    "lineWidth": 1,
-                                    "pointSize": 5,
-                                    "scaleDistribution": {
-                                        "type": "linear"
-                                    },
-                                    "showPoints": "auto",
-                                    "spanNulls": false,
-                                    "stacking": {
-                                        "group": "A",
-                                        "mode": "none"
-                                    },
-                                    "thresholdsStyle": {
-                                        "mode": "off"
-                                    }
+                        "editorMode": "builder",
+                        "expr": "device_unmap_latency_ticks",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "device_unmap_latency_ticks",
+                "type": "timeseries"
+            },
+            {
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
                                 },
-                                "mappings": [],
-                                "thresholds": {
-                                    "mode": "absolute",
-                                    "steps": [
-                                        {
-                                            "color": "green",
-                                            "value": null
-                                        },
-                                        {
-                                            "color": "red",
-                                            "value": 80
-                                        }
-                                    ]
-                                },
-                                "unit": "decbytes"
-                            },
-                            "overrides": []
-                        },
-                        "gridPos": {
-                            "h": 7,
-                            "w": 7,
-                            "x": 7,
-                            "y": 48
-                        },
-                        "id": 17,
-                        "options": {
-                            "legend": {
-                                "calcs": [],
-                                "displayMode": "list",
-                                "placement": "bottom",
-                                "showLegend": true
-                            },
-                            "tooltip": {
-                                "mode": "single",
-                                "sort": "none"
-                            }
-                        },
-                        "targets": [
-                            {
-                                "datasource": {
-                                    "type": "prometheus",
-                                    "uid": "PBFA97CFB590B2093"
-                                },
-                                "editorMode": "builder",
-                                "expr": "device_unmap_bytes_ps",
-                                "legendFormat": "__auto",
-                                "range": true,
-                                "refId": "A"
-                            }
-                        ],
-                        "title": "device_unmap_bytes_ps",
-                        "type": "timeseries"
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        },
+                        "unit": "bytes"
                     },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 7,
+                    "y": 49
+                },
+                "id": 17,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "description": "",
-                        "fieldConfig": {
-                            "defaults": {
-                                "color": {
-                                    "mode": "palette-classic"
-                                },
-                                "custom": {
-                                    "axisCenteredZero": false,
-                                    "axisColorMode": "text",
-                                    "axisLabel": "",
-                                    "axisPlacement": "auto",
-                                    "barAlignment": 0,
-                                    "drawStyle": "line",
-                                    "fillOpacity": 0,
-                                    "gradientMode": "none",
-                                    "hideFrom": {
-                                        "legend": false,
-                                        "tooltip": false,
-                                        "viz": false
-                                    },
-                                    "lineInterpolation": "linear",
-                                    "lineWidth": 1,
-                                    "pointSize": 5,
-                                    "scaleDistribution": {
-                                        "type": "linear"
-                                    },
-                                    "showPoints": "auto",
-                                    "spanNulls": false,
-                                    "stacking": {
-                                        "group": "A",
-                                        "mode": "none"
-                                    },
-                                    "thresholdsStyle": {
-                                        "mode": "off"
-                                    }
+                        "editorMode": "builder",
+                        "expr": "device_unmap_bytes_ps",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "device_unmap_bytes_ps",
+                "type": "timeseries"
+            },
+            {
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "description": "",
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
                                 },
-                                "mappings": [],
-                                "thresholds": {
-                                    "mode": "absolute",
-                                    "steps": [
-                                        {
-                                            "color": "green",
-                                            "value": null
-                                        },
-                                        {
-                                            "color": "red",
-                                            "value": 80
-                                        }
-                                    ]
-                                }
-                            },
-                            "overrides": []
-                        },
-                        "gridPos": {
-                            "h": 7,
-                            "w": 8,
-                            "x": 14,
-                            "y": 48
-                        },
-                        "id": 20,
-                        "options": {
-                            "legend": {
-                                "calcs": [],
-                                "displayMode": "list",
-                                "placement": "bottom",
-                                "showLegend": true
-                            },
-                            "tooltip": {
-                                "mode": "single",
-                                "sort": "none"
-                            }
-                        },
-                        "targets": [
-                            {
-                                "datasource": {
-                                    "type": "prometheus",
-                                    "uid": "PBFA97CFB590B2093"
-                                },
-                                "editorMode": "builder",
-                                "expr": "device_unmap_latency_ps",
-                                "legendFormat": "__auto",
-                                "range": true,
-                                "refId": "A"
-                            }
-                        ],
-                        "title": "device_unmap_latency_ps",
-                        "type": "timeseries"
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        },
+                        "unit": "\u00b5s"
+                    },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 8,
+                    "x": 14,
+                    "y": 49
+                },
+                "id": 20,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
                     },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "fieldConfig": {
-                            "defaults": {
-                                "color": {
-                                    "mode": "palette-classic"
-                                },
-                                "custom": {
-                                    "axisCenteredZero": false,
-                                    "axisColorMode": "text",
-                                    "axisLabel": "",
-                                    "axisPlacement": "auto",
-                                    "barAlignment": 0,
-                                    "drawStyle": "line",
-                                    "fillOpacity": 0,
-                                    "gradientMode": "none",
-                                    "hideFrom": {
-                                        "legend": false,
-                                        "tooltip": false,
-                                        "viz": false
-                                    },
-                                    "lineInterpolation": "linear",
-                                    "lineWidth": 1,
-                                    "pointSize": 5,
-                                    "scaleDistribution": {
-                                        "type": "linear"
-                                    },
-                                    "showPoints": "auto",
-                                    "spanNulls": false,
-                                    "stacking": {
-                                        "group": "A",
-                                        "mode": "none"
-                                    },
-                                    "thresholdsStyle": {
-                                        "mode": "off"
-                                    }
+                        "editorMode": "builder",
+                        "expr": "device_unmap_latency_ps",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "device_unmap_latency_ps",
+                "type": "timeseries"
+            },
+            {
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
                                 },
-                                "mappings": [],
-                                "thresholds": {
-                                    "mode": "absolute",
-                                    "steps": [
-                                        {
-                                            "color": "green",
-                                            "value": null
-                                        },
-                                        {
-                                            "color": "red",
-                                            "value": 80
-                                        }
-                                    ]
-                                }
-                            },
-                            "overrides": [
-                                {
-                                    "__systemRef": "hideSeriesFrom",
-                                    "matcher": {
-                                        "id": "byNames",
-                                        "options": {
-                                            "mode": "exclude",
-                                            "names": [
-                                                "{__name__=\"device_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
-                                            ],
-                                            "prefix": "All except:",
-                                            "readOnly": true
-                                        }
-                                    },
-                                    "properties": [
-                                        {
-                                            "id": "custom.hideFrom",
-                                            "value": {
-                                                "legend": false,
-                                                "tooltip": false,
-                                                "viz": true
-                                            }
-                                        }
-                                    ]
-                                }
-                            ]
-                        },
-                        "gridPos": {
-                            "h": 7,
-                            "w": 7,
-                            "x": 0,
-                            "y": 55
-                        },
-                        "id": 19,
-                        "options": {
-                            "legend": {
-                                "calcs": [],
-                                "displayMode": "list",
-                                "placement": "bottom",
-                                "showLegend": true
-                            },
-                            "tooltip": {
-                                "mode": "single",
-                                "sort": "none"
-                            }
-                        },
-                        "targets": [
-                            {
-                                "datasource": {
-                                    "type": "prometheus",
-                                    "uid": "PBFA97CFB590B2093"
-                                },
-                                "editorMode": "builder",
-                                "expr": "device_unmap_io_ps",
-                                "legendFormat": "__auto",
-                                "range": true,
-                                "refId": "A"
-                            }
-                        ],
-                        "title": "device_unmap_io_ps",
-                        "type": "timeseries"
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        }
                     },
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "fieldConfig": {
-                            "defaults": {
-                                "color": {
-                                    "mode": "palette-classic"
-                                },
-                                "custom": {
-                                    "axisCenteredZero": false,
-                                    "axisColorMode": "text",
-                                    "axisLabel": "",
-                                    "axisPlacement": "auto",
-                                    "barAlignment": 0,
-                                    "drawStyle": "line",
-                                    "fillOpacity": 0,
-                                    "gradientMode": "none",
-                                    "hideFrom": {
+                    "overrides": [
+                        {
+                            "__systemRef": "hideSeriesFrom",
+                            "matcher": {
+                                "id": "byNames",
+                                "options": {
+                                    "mode": "exclude",
+                                    "names": [
+                                        "{__name__=\"device_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
+                                    ],
+                                    "prefix": "All except:",
+                                    "readOnly": true
+                                }
+                            },
+                            "properties": [
+                                {
+                                    "id": "custom.hideFrom",
+                                    "value": {
                                         "legend": false,
                                         "tooltip": false,
-                                        "viz": false
-                                    },
-                                    "lineInterpolation": "linear",
-                                    "lineWidth": 1,
-                                    "pointSize": 5,
-                                    "scaleDistribution": {
-                                        "type": "linear"
-                                    },
-                                    "showPoints": "auto",
-                                    "spanNulls": false,
-                                    "stacking": {
-                                        "group": "A",
-                                        "mode": "none"
-                                    },
-                                    "thresholdsStyle": {
-                                        "mode": "off"
+                                        "viz": true
                                     }
-                                },
-                                "mappings": [],
-                                "thresholds": {
-                                    "mode": "absolute",
-                                    "steps": [
-                                        {
-                                            "color": "green",
-                                            "value": null
-                                        },
-                                        {
-                                            "color": "red",
-                                            "value": 80
-                                        }
-                                    ]
-                                }
-                            },
-                            "overrides": []
-                        },
-                        "gridPos": {
-                            "h": 7,
-                            "w": 7,
-                            "x": 7,
-                            "y": 55
-                        },
-                        "id": 18,
-                        "options": {
-                            "legend": {
-                                "calcs": [],
-                                "displayMode": "list",
-                                "placement": "bottom",
-                                "showLegend": true
-                            },
-                            "tooltip": {
-                                "mode": "single",
-                                "sort": "none"
-                            }
-                        },
-                        "targets": [
-                            {
-                                "datasource": {
-                                    "type": "prometheus",
-                                    "uid": "PBFA97CFB590B2093"
-                                },
-                                "editorMode": "builder",
-                                "expr": "device_unmap_io",
-                                "legendFormat": "__auto",
-                                "range": true,
-                                "refId": "A"
-                            }
-                        ],
-                        "title": "device_unmap_io",
-                        "type": "timeseries"
+                                }
+                            ]
+                        }
+                    ]
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 0,
+                    "y": 56
+                },
+                "id": 19,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
                     },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "fieldConfig": {
-                            "defaults": {
-                                "color": {
-                                    "mode": "palette-classic"
-                                },
-                                "custom": {
-                                    "axisCenteredZero": false,
-                                    "axisColorMode": "text",
-                                    "axisLabel": "",
-                                    "axisPlacement": "auto",
-                                    "barAlignment": 0,
-                                    "drawStyle": "line",
-                                    "fillOpacity": 0,
-                                    "gradientMode": "none",
-                                    "hideFrom": {
-                                        "legend": false,
-                                        "tooltip": false,
-                                        "viz": false
-                                    },
-                                    "lineInterpolation": "linear",
-                                    "lineWidth": 1,
-                                    "pointSize": 5,
-                                    "scaleDistribution": {
-                                        "type": "linear"
-                                    },
-                                    "showPoints": "auto",
-                                    "spanNulls": false,
-                                    "stacking": {
-                                        "group": "A",
-                                        "mode": "none"
-                                    },
-                                    "thresholdsStyle": {
-                                        "mode": "off"
-                                    }
-                                },
-                                "mappings": [],
-                                "thresholds": {
-                                    "mode": "absolute",
-                                    "steps": [
-                                        {
-                                            "color": "green",
-                                            "value": null
-                                        },
-                                        {
-                                            "color": "red",
-                                            "value": 80
-                                        }
-                                    ]
-                                },
-                                "unit": "decbytes"
-                            },
-                            "overrides": []
-                        },
-                        "gridPos": {
-                            "h": 7,
-                            "w": 8,
-                            "x": 14,
-                            "y": 55
-                        },
-                        "id": 16,
-                        "options": {
-                            "legend": {
-                                "calcs": [],
-                                "displayMode": "list",
-                                "placement": "bottom",
-                                "showLegend": true
-                            },
-                            "tooltip": {
-                                "mode": "single",
-                                "sort": "none"
-                            }
-                        },
-                        "targets": [
-                            {
-                                "datasource": {
-                                    "type": "prometheus",
-                                    "uid": "PBFA97CFB590B2093"
-                                },
-                                "editorMode": "builder",
-                                "expr": "device_unmap_bytes",
-                                "legendFormat": "__auto",
-                                "range": true,
-                                "refId": "A"
-                            }
-                        ],
-                        "title": "device_unmap_bytes",
-                        "type": "timeseries"
+                        "editorMode": "builder",
+                        "expr": "device_unmap_io_ps",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
                     }
                 ],
-                "title": "unmap",
-                "type": "row"
+                "title": "device_unmap_io_ps",
+                "type": "timeseries"
             },
             {
-                "collapsed": true,
-                "gridPos": {
-                    "h": 1,
-                    "w": 24,
-                    "x": 0,
-                    "y": 49
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
                 },
-                "id": 32,
-                "panels": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
                         },
-                        "fieldConfig": {
-                            "defaults": {
-                                "color": {
-                                    "mode": "palette-classic"
-                                },
-                                "custom": {
-                                    "axisCenteredZero": false,
-                                    "axisColorMode": "text",
-                                    "axisLabel": "",
-                                    "axisPlacement": "auto",
-                                    "barAlignment": 0,
-                                    "drawStyle": "line",
-                                    "fillOpacity": 0,
-                                    "gradientMode": "none",
-                                    "hideFrom": {
-                                        "legend": false,
-                                        "tooltip": false,
-                                        "viz": false
-                                    },
-                                    "lineInterpolation": "linear",
-                                    "lineWidth": 1,
-                                    "pointSize": 5,
-                                    "scaleDistribution": {
-                                        "type": "linear"
-                                    },
-                                    "showPoints": "auto",
-                                    "spanNulls": false,
-                                    "stacking": {
-                                        "group": "A",
-                                        "mode": "none"
-                                    },
-                                    "thresholdsStyle": {
-                                        "mode": "off"
-                                    }
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
                                 },
-                                "mappings": [],
-                                "thresholds": {
-                                    "mode": "absolute",
-                                    "steps": [
-                                        {
-                                            "color": "green",
-                                            "value": null
-                                        },
-                                        {
-                                            "color": "red",
-                                            "value": 80
-                                        }
-                                    ]
-                                }
-                            },
-                            "overrides": []
-                        },
-                        "gridPos": {
-                            "h": 7,
-                            "w": 7,
-                            "x": 0,
-                            "y": 49
-                        },
-                        "id": 8,
-                        "options": {
-                            "legend": {
-                                "calcs": [],
-                                "displayMode": "list",
-                                "placement": "bottom",
-                                "showLegend": true
-                            },
-                            "tooltip": {
-                                "mode": "single",
-                                "sort": "none"
-                            }
-                        },
-                        "targets": [
-                            {
-                                "datasource": {
-                                    "type": "prometheus",
-                                    "uid": "PBFA97CFB590B2093"
-                                },
-                                "editorMode": "builder",
-                                "expr": "device_record_end_time",
-                                "legendFormat": "__auto",
-                                "range": true,
-                                "refId": "A"
-                            }
-                        ],
-                        "title": "device_record_end_time",
-                        "type": "timeseries"
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        }
                     },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 7,
+                    "x": 7,
+                    "y": 56
+                },
+                "id": 18,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
+                    },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "description": "",
-                        "fieldConfig": {
-                            "defaults": {
-                                "color": {
-                                    "mode": "palette-classic"
-                                },
-                                "custom": {
-                                    "axisCenteredZero": false,
-                                    "axisColorMode": "text",
-                                    "axisLabel": "",
-                                    "axisPlacement": "auto",
-                                    "barAlignment": 0,
-                                    "drawStyle": "line",
-                                    "fillOpacity": 0,
-                                    "gradientMode": "none",
-                                    "hideFrom": {
-                                        "legend": false,
-                                        "tooltip": false,
-                                        "viz": false
-                                    },
-                                    "lineInterpolation": "linear",
-                                    "lineWidth": 1,
-                                    "pointSize": 5,
-                                    "scaleDistribution": {
-                                        "type": "linear"
-                                    },
-                                    "showPoints": "auto",
-                                    "spanNulls": false,
-                                    "stacking": {
-                                        "group": "A",
-                                        "mode": "none"
-                                    },
-                                    "thresholdsStyle": {
-                                        "mode": "off"
-                                    }
+                        "editorMode": "builder",
+                        "expr": "device_unmap_io",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
+                    }
+                ],
+                "title": "device_unmap_io",
+                "type": "timeseries"
+            },
+            {
+                "datasource": {
+                    "type": "prometheus",
+                    "uid": "PBFA97CFB590B2093"
+                },
+                "fieldConfig": {
+                    "defaults": {
+                        "color": {
+                            "mode": "palette-classic"
+                        },
+                        "custom": {
+                            "axisCenteredZero": false,
+                            "axisColorMode": "text",
+                            "axisLabel": "",
+                            "axisPlacement": "auto",
+                            "barAlignment": 0,
+                            "drawStyle": "line",
+                            "fillOpacity": 0,
+                            "gradientMode": "none",
+                            "hideFrom": {
+                                "legend": false,
+                                "tooltip": false,
+                                "viz": false
+                            },
+                            "lineInterpolation": "linear",
+                            "lineWidth": 1,
+                            "pointSize": 5,
+                            "scaleDistribution": {
+                                "type": "linear"
+                            },
+                            "showPoints": "auto",
+                            "spanNulls": false,
+                            "stacking": {
+                                "group": "A",
+                                "mode": "none"
+                            },
+                            "thresholdsStyle": {
+                                "mode": "off"
+                            }
+                        },
+                        "mappings": [],
+                        "thresholds": {
+                            "mode": "absolute",
+                            "steps": [
+                                {
+                                    "color": "green",
+                                    "value": null
                                 },
-                                "mappings": [],
-                                "thresholds": {
-                                    "mode": "absolute",
-                                    "steps": [
-                                        {
-                                            "color": "green",
-                                            "value": null
-                                        },
-                                        {
-                                            "color": "red",
-                                            "value": 80
-                                        }
-                                    ]
-                                }
-                            },
-                            "overrides": []
-                        },
-                        "gridPos": {
-                            "h": 7,
-                            "w": 7,
-                            "x": 7,
-                            "y": 49
-                        },
-                        "id": 7,
-                        "options": {
-                            "legend": {
-                                "calcs": [],
-                                "displayMode": "list",
-                                "placement": "bottom",
-                                "showLegend": true
-                            },
-                            "tooltip": {
-                                "mode": "single",
-                                "sort": "none"
-                            }
-                        },
-                        "targets": [
-                            {
-                                "datasource": {
-                                    "type": "prometheus",
-                                    "uid": "PBFA97CFB590B2093"
-                                },
-                                "editorMode": "builder",
-                                "expr": "device_record_duration",
-                                "legendFormat": "__auto",
-                                "range": true,
-                                "refId": "A"
-                            }
-                        ],
-                        "title": "device_record_duration",
-                        "type": "timeseries"
+                                {
+                                    "color": "red",
+                                    "value": 80
+                                }
+                            ]
+                        },
+                        "unit": "decbytes"
+                    },
+                    "overrides": []
+                },
+                "gridPos": {
+                    "h": 7,
+                    "w": 8,
+                    "x": 14,
+                    "y": 56
+                },
+                "id": 16,
+                "options": {
+                    "legend": {
+                        "calcs": [],
+                        "displayMode": "list",
+                        "placement": "bottom",
+                        "showLegend": true
                     },
+                    "tooltip": {
+                        "mode": "single",
+                        "sort": "none"
+                    }
+                },
+                "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
-                        "fieldConfig": {
-                            "defaults": {
-                                "color": {
-                                    "mode": "palette-classic"
-                                },
-                                "custom": {
-                                    "axisCenteredZero": false,
-                                    "axisColorMode": "text",
-                                    "axisLabel": "",
-                                    "axisPlacement": "auto",
-                                    "barAlignment": 0,
-                                    "drawStyle": "line",
-                                    "fillOpacity": 0,
-                                    "gradientMode": "none",
-                                    "hideFrom": {
-                                        "legend": false,
-                                        "tooltip": false,
-                                        "viz": false
-                                    },
-                                    "lineInterpolation": "linear",
-                                    "lineWidth": 1,
-                                    "pointSize": 5,
-                                    "scaleDistribution": {
-                                        "type": "linear"
-                                    },
-                                    "showPoints": "auto",
-                                    "spanNulls": false,
-                                    "stacking": {
-                                        "group": "A",
-                                        "mode": "none"
-                                    },
-                                    "thresholdsStyle": {
-                                        "mode": "off"
-                                    }
-                                },
-                                "mappings": [],
-                                "thresholds": {
-                                    "mode": "absolute",
-                                    "steps": [
-                                        {
-                                            "color": "green",
-                                            "value": null
-                                        },
-                                        {
-                                            "color": "red",
-                                            "value": 80
-                                        }
-                                    ]
-                                },
-                                "unit": "decbytes"
-                            },
-                            "overrides": []
-                        },
-                        "gridPos": {
-                            "h": 7,
-                            "w": 8,
-                            "x": 14,
-                            "y": 49
-                        },
-                        "id": 9,
-                        "options": {
-                            "legend": {
-                                "calcs": [],
-                                "displayMode": "list",
-                                "placement": "bottom",
-                                "showLegend": true
-                            },
-                            "tooltip": {
-                                "mode": "single",
-                                "sort": "none"
-                            }
-                        },
-                        "targets": [
-                            {
-                                "datasource": {
-                                    "type": "prometheus",
-                                    "uid": "PBFA97CFB590B2093"
-                                },
-                                "editorMode": "builder",
-                                "expr": "device_record_start_time",
-                                "legendFormat": "__auto",
-                                "range": true,
-                                "refId": "A"
-                            }
-                        ],
-                        "title": "device_record_start_time",
-                        "type": "timeseries"
+                        "editorMode": "builder",
+                        "expr": "device_unmap_bytes",
+                        "legendFormat": "__auto",
+                        "range": true,
+                        "refId": "A"
                     }
                 ],
-                "title": "others",
-                "type": "row"
+                "title": "device_unmap_bytes",
+                "type": "timeseries"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
         "templating": {
```

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/node-exporter.json` & `sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/node-exporter.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9984272596571181%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'bytes'}}}, 2: "*

 * *                "{'fieldConfig': {'defaults': {'unit': 'bytes'}}}, 3: {'fieldConfig': {'defaults': "*

 * *                "{'unit': 'bytes'}}}, 4: {'fieldConfig': {'defaults': {'unit': 'bytes'}}}, 5: "*

 * *                "{'fieldConfig': {'defaults': {'unit': 'percent'}}}, 6: {'fieldConfig': "*

 * *                "{'defaults': {'unit': 'percent'}}}, 8: {'fieldConfig': {'defaults': {'unit': "*

 * *                "'bytes'}}}, 9: {'fieldCon […]*

```diff
@@ -86,15 +86,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -179,15 +179,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -272,15 +272,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -365,15 +365,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -458,15 +458,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "percent"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -551,15 +551,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "percent"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -657,15 +657,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -750,15 +750,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "Bps"
+                        "unit": "binBps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -1119,15 +1119,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "ns"
+                        "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
@@ -1225,15 +1225,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -1318,15 +1318,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "Bps"
+                        "unit": "binBps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
@@ -1410,15 +1410,16 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
@@ -1884,15 +1885,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -1977,15 +1978,16 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -2279,15 +2281,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -2317,305 +2319,14 @@
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "snode_unmap_bytes",
                 "type": "timeseries"
-            },
-            {
-                "collapsed": false,
-                "gridPos": {
-                    "h": 1,
-                    "w": 24,
-                    "x": 0,
-                    "y": 62
-                },
-                "id": 32,
-                "panels": [],
-                "title": "others",
-                "type": "row"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        }
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 0,
-                    "y": 63
-                },
-                "id": 8,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "snode_record_end_time",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "snode_record_end_time",
-                "type": "timeseries"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "description": "",
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        }
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 7,
-                    "y": 63
-                },
-                "id": 7,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "snode_record_duration",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "snode_record_duration",
-                "type": "timeseries"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        },
-                        "unit": "decbytes"
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 14,
-                    "y": 63
-                },
-                "id": 9,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "snode_record_start_time",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "snode_record_start_time",
-                "type": "timeseries"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
         "templating": {
```

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/pools.json`

 * *Files 3% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9742892929359719%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'targets': {0: {'expr': 'pool_size_total'}}, 'title': "*

 * *                "'pool_size_total'}, 2: {'targets': {0: {'expr': 'pool_size_free'}}, 'title': "*

 * *                "'pool_size_free'}, 3: {'targets': {0: {'expr': 'pool_size_used'}}, 'title': "*

 * *                "'pool_size_used'}, 4: {'targets': {0: {'expr': 'pool_size_prov'}}, 'title': "*

 * *                "'pool_size_prov'}, 5: {'targets': {0: {'expr': 'pool_size_prov_util'}}, 'title': "*

 * *                "'pool_size_prov_util […]*

```diff
@@ -116,21 +116,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_size_total",
+                        "expr": "pool_size_total",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_total",
+                "title": "pool_size_total",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -209,21 +209,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_size_free",
+                        "expr": "pool_size_free",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_free",
+                "title": "pool_size_free",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -302,21 +302,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_size_used",
+                        "expr": "pool_size_used",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_used",
+                "title": "pool_size_used",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -395,21 +395,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_size_prov",
+                        "expr": "pool_size_prov",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_prov",
+                "title": "pool_size_prov",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -488,21 +488,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_size_prov_util",
+                        "expr": "pool_size_prov_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_prov_util",
+                "title": "pool_size_prov_util",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -581,21 +581,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_size_util",
+                        "expr": "pool_size_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_size_util",
+                "title": "pool_size_util",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -687,21 +687,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_write_bytes",
+                        "expr": "pool_write_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_write_bytes",
+                "title": "pool_write_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -749,25 +749,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "Bps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
                     "y": 16
                 },
-                "id": 25,
+                "id": 23,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -779,21 +780,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_write_io_ps",
+                        "expr": "pool_write_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "write_iops",
+                "title": "write_speed",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -871,21 +872,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_write_latency_ticks",
+                        "expr": "pool_write_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_wite_latency_ticks",
+                "title": "pool_wite_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -963,21 +964,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_write_io",
+                        "expr": "pool_write_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_write_io",
+                "title": "pool_write_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1025,26 +1026,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "Bps"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
                     "y": 24
                 },
-                "id": 23,
+                "id": 25,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1056,21 +1056,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_write_bytes_ps",
+                        "expr": "pool_write_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "write_speed",
+                "title": "write_iops",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1149,21 +1149,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_write_latency_ps / 1000",
+                        "expr": "pool_write_latency_ps / 1000",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_write_latency_ps",
+                "title": "pool_write_latency_ps",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -1255,21 +1255,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_read_bytes",
+                        "expr": "pool_read_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_read_bytes",
+                "title": "pool_read_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1348,15 +1348,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_read_bytes_ps",
+                        "expr": "pool_read_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_speed",
                 "type": "timeseries"
@@ -1440,21 +1440,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_read_latency_ps",
+                        "expr": "pool_read_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_read_latency_ps",
+                "title": "pool_read_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1532,21 +1532,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_read_io",
+                        "expr": "pool_read_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_read_io",
+                "title": "pool_read_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1624,15 +1624,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_read_io_ps",
+                        "expr": "pool_read_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_iops",
                 "type": "timeseries"
@@ -1716,21 +1716,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_read_latency_ticks",
+                        "expr": "pool_read_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_read_latency_ticks",
+                "title": "pool_read_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -1821,21 +1821,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_unmap_latency_ticks",
+                        "expr": "pool_unmap_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_latency_ticks",
+                "title": "pool_unmap_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1914,21 +1914,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_unmap_bytes_ps",
+                        "expr": "pool_unmap_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_bytes_ps",
+                "title": "pool_unmap_bytes_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2007,21 +2007,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_unmap_latency_ps",
+                        "expr": "pool_unmap_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_latency_ps",
+                "title": "pool_unmap_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2079,15 +2079,15 @@
                         {
                             "__systemRef": "hideSeriesFrom",
                             "matcher": {
                                 "id": "byNames",
                                 "options": {
                                     "mode": "exclude",
                                     "names": [
-                                        "{__name__=\"lvol_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
+                                        "{__name__=\"pool_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
                                     ],
                                     "prefix": "All except:",
                                     "readOnly": true
                                 }
                             },
                             "properties": [
                                 {
@@ -2124,21 +2124,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_unmap_io_ps",
+                        "expr": "pool_unmap_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_io_ps",
+                "title": "pool_unmap_io_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2216,21 +2216,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_unmap_io",
+                        "expr": "pool_unmap_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_io",
+                "title": "pool_unmap_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2309,21 +2309,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_unmap_bytes",
+                        "expr": "pool_unmap_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_unmap_bytes",
+                "title": "pool_unmap_bytes",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -2414,21 +2414,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_record_end_time",
+                        "expr": "pool_record_end_time",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_record_end_time",
+                "title": "pool_record_end_time",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2507,21 +2507,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_record_duration",
+                        "expr": "pool_record_duration",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_record_duration",
+                "title": "pool_record_duration",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2600,21 +2600,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "lvol_record_start_time",
+                        "expr": "pool_record_start_time",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "lvol_record_start_time",
+                "title": "pool_record_start_time",
                 "type": "timeseries"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
@@ -2623,13 +2623,13 @@
         },
         "time": {
             "from": "now-1h",
             "to": "now"
         },
         "timepicker": {},
         "timezone": "",
-        "title": "LvolsDashboard",
-        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e19",
+        "title": "PoolsDashboard",
+        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e40",
         "version": 5,
         "weekStart": ""
     }
 }
```

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files 1% similar despite different names*

### Pretty-printed

 * *Similarity: 0.9984272596571181%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'bytes'}}}, 2: "*

 * *                "{'fieldConfig': {'defaults': {'unit': 'bytes'}}}, 3: {'fieldConfig': {'defaults': "*

 * *                "{'unit': 'bytes'}}}, 4: {'fieldConfig': {'defaults': {'unit': 'bytes'}}}, 5: "*

 * *                "{'fieldConfig': {'defaults': {'unit': 'percent'}}}, 6: {'fieldConfig': "*

 * *                "{'defaults': {'unit': 'percent'}}}, 8: {'fieldConfig': {'defaults': {'unit': "*

 * *                "'bytes'}}}, 9: {'fieldCon […]*

```diff
@@ -86,15 +86,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -179,15 +179,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -272,15 +272,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -365,15 +365,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -458,15 +458,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "percent"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -551,15 +551,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "percent"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -657,15 +657,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -750,15 +750,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "Bps"
+                        "unit": "binBps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -843,15 +843,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "ns"
+                        "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -1225,15 +1225,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -1318,15 +1318,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "Bps"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
@@ -1410,15 +1410,16 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
@@ -1884,15 +1885,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -1977,15 +1978,16 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -2279,15 +2281,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -2317,305 +2319,14 @@
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "cluster_unmap_bytes",
                 "type": "timeseries"
-            },
-            {
-                "collapsed": false,
-                "gridPos": {
-                    "h": 1,
-                    "w": 24,
-                    "x": 0,
-                    "y": 61
-                },
-                "id": 32,
-                "panels": [],
-                "title": "others",
-                "type": "row"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        }
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 0,
-                    "y": 62
-                },
-                "id": 8,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "cluster_record_end_time",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "cluster_record_end_time",
-                "type": "timeseries"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "description": "",
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        }
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 7,
-                    "y": 62
-                },
-                "id": 7,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "cluster_record_duration",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "cluster_record_duration",
-                "type": "timeseries"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        },
-                        "unit": "decbytes"
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 14,
-                    "y": 62
-                },
-                "id": 9,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "cluster_record_start_time",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "cluster_record_start_time",
-                "type": "timeseries"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
         "templating": {
```

## Comparing `sbcli_dev-2.5.7/simplyblock_core/scripts/dashboards/pools.json` & `sbcli_dev-2.5.8/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files 8% similar despite different names*

### Pretty-printed

 * *Similarity: 0.972793569918032%*

 * *Differences: {"'dashboard'": "{'panels': {1: {'fieldConfig': {'defaults': {'unit': 'bytes'}}, 'targets': {0: "*

 * *                "{'expr': 'lvol_size_total'}}, 'title': 'lvol_size_total'}, 2: {'fieldConfig': "*

 * *                "{'defaults': {'unit': 'bytes'}}, 'targets': {0: {'expr': 'lvol_size_free'}}, "*

 * *                "'title': 'lvol_size_free'}, 3: {'fieldConfig': {'defaults': {'unit': 'bytes'}}, "*

 * *                "'targets': {0: {'expr': 'lvol_size_used'}}, 'title': 'lvol_size_used'}, 4: "*

 * *                "{'fieldConf […]*

```diff
@@ -86,15 +86,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -116,21 +116,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_size_total",
+                        "expr": "lvol_size_total",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_total",
+                "title": "lvol_size_total",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -179,15 +179,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -209,21 +209,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_size_free",
+                        "expr": "lvol_size_free",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_free",
+                "title": "lvol_size_free",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -272,15 +272,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -302,21 +302,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_size_used",
+                        "expr": "lvol_size_used",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_used",
+                "title": "lvol_size_used",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -365,15 +365,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 0,
@@ -395,21 +395,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_size_prov",
+                        "expr": "lvol_size_prov",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_prov",
+                "title": "lvol_size_prov",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -458,15 +458,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "percent"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -488,21 +488,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_size_prov_util",
+                        "expr": "lvol_size_prov_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_prov_util",
+                "title": "lvol_size_prov_util",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -551,15 +551,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "percent"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -581,21 +581,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_size_util",
+                        "expr": "lvol_size_util",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_size_util",
+                "title": "lvol_size_util",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -657,15 +657,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -687,21 +687,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_write_bytes",
+                        "expr": "lvol_write_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_bytes",
+                "title": "lvol_write_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -749,26 +749,25 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        },
-                        "unit": "Bps"
+                        }
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
                     "y": 16
                 },
-                "id": 23,
+                "id": 25,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -780,21 +779,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_write_bytes_ps",
+                        "expr": "lvol_write_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "write_speed",
+                "title": "write_iops",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -872,21 +871,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_write_latency_ticks",
+                        "expr": "lvol_write_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_wite_latency_ticks",
+                "title": "lvol_wite_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -964,21 +963,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_write_io",
+                        "expr": "lvol_write_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_io",
+                "title": "lvol_write_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1026,25 +1025,26 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "binBps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
                     "y": 24
                 },
-                "id": 25,
+                "id": 23,
                 "options": {
                     "legend": {
                         "calcs": [],
                         "displayMode": "list",
                         "placement": "bottom",
                         "showLegend": true
                     },
@@ -1056,21 +1056,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_write_io_ps",
+                        "expr": "lvol_write_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "write_iops",
+                "title": "write_speed",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1119,15 +1119,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "ns"
+                        "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
@@ -1149,21 +1149,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_write_latency_ps / 1000",
+                        "expr": "lvol_write_latency_ps / 1000",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_write_latency_ps",
+                "title": "lvol_write_latency_ps",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -1225,15 +1225,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 0,
@@ -1255,21 +1255,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_read_bytes",
+                        "expr": "lvol_read_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_bytes",
+                "title": "lvol_read_bytes",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1318,15 +1318,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "Bps"
+                        "unit": "binBps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 7,
@@ -1348,15 +1348,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_read_bytes_ps",
+                        "expr": "lvol_read_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_speed",
                 "type": "timeseries"
@@ -1410,15 +1410,16 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 8,
                     "w": 7,
                     "x": 14,
@@ -1440,21 +1441,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_read_latency_ps",
+                        "expr": "lvol_read_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_latency_ps",
+                "title": "lvol_read_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1532,21 +1533,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_read_io",
+                        "expr": "lvol_read_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_io",
+                "title": "lvol_read_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1624,15 +1625,15 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_read_io_ps",
+                        "expr": "lvol_read_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
                 "title": "read_iops",
                 "type": "timeseries"
@@ -1716,21 +1717,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_read_latency_ticks",
+                        "expr": "lvol_read_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_read_latency_ticks",
+                "title": "lvol_read_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "collapsed": false,
                 "gridPos": {
                     "h": 1,
                     "w": 24,
@@ -1821,21 +1822,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_unmap_latency_ticks",
+                        "expr": "lvol_unmap_latency_ticks",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_latency_ticks",
+                "title": "lvol_unmap_latency_ticks",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1884,15 +1885,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "bytes"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 7,
@@ -1914,21 +1915,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_unmap_bytes_ps",
+                        "expr": "lvol_unmap_bytes_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_bytes_ps",
+                "title": "lvol_unmap_bytes_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -1977,15 +1978,16 @@
                                     "value": null
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
-                        }
+                        },
+                        "unit": "\u00b5s"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -2007,21 +2009,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_unmap_latency_ps",
+                        "expr": "lvol_unmap_latency_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_latency_ps",
+                "title": "lvol_unmap_latency_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2079,15 +2081,15 @@
                         {
                             "__systemRef": "hideSeriesFrom",
                             "matcher": {
                                 "id": "byNames",
                                 "options": {
                                     "mode": "exclude",
                                     "names": [
-                                        "{__name__=\"pool_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
+                                        "{__name__=\"lvol_unmap_io_ps\", cluster=\"c3663938-6610-44d5-9897-d7bfa60a43e1\", exported_job=\"collector\", instance=\"192.168.178.52:9091\", job=\"metricsgateway\"}"
                                     ],
                                     "prefix": "All except:",
                                     "readOnly": true
                                 }
                             },
                             "properties": [
                                 {
@@ -2124,21 +2126,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_unmap_io_ps",
+                        "expr": "lvol_unmap_io_ps",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_io_ps",
+                "title": "lvol_unmap_io_ps",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2216,21 +2218,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_unmap_io",
+                        "expr": "lvol_unmap_io",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_unmap_io",
+                "title": "lvol_unmap_io",
                 "type": "timeseries"
             },
             {
                 "datasource": {
                     "type": "prometheus",
                     "uid": "PBFA97CFB590B2093"
                 },
@@ -2279,15 +2281,15 @@
                                 },
                                 {
                                     "color": "red",
                                     "value": 80
                                 }
                             ]
                         },
-                        "unit": "decbytes"
+                        "unit": "binBps"
                     },
                     "overrides": []
                 },
                 "gridPos": {
                     "h": 7,
                     "w": 7,
                     "x": 14,
@@ -2309,312 +2311,21 @@
                 "targets": [
                     {
                         "datasource": {
                             "type": "prometheus",
                             "uid": "PBFA97CFB590B2093"
                         },
                         "editorMode": "builder",
-                        "expr": "pool_unmap_bytes",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "pool_unmap_bytes",
-                "type": "timeseries"
-            },
-            {
-                "collapsed": false,
-                "gridPos": {
-                    "h": 1,
-                    "w": 24,
-                    "x": 0,
-                    "y": 63
-                },
-                "id": 32,
-                "panels": [],
-                "title": "others",
-                "type": "row"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        }
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 0,
-                    "y": 64
-                },
-                "id": 8,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "pool_record_end_time",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "pool_record_end_time",
-                "type": "timeseries"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "description": "",
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        }
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 7,
-                    "y": 64
-                },
-                "id": 7,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "pool_record_duration",
-                        "legendFormat": "__auto",
-                        "range": true,
-                        "refId": "A"
-                    }
-                ],
-                "title": "pool_record_duration",
-                "type": "timeseries"
-            },
-            {
-                "datasource": {
-                    "type": "prometheus",
-                    "uid": "PBFA97CFB590B2093"
-                },
-                "fieldConfig": {
-                    "defaults": {
-                        "color": {
-                            "mode": "palette-classic"
-                        },
-                        "custom": {
-                            "axisCenteredZero": false,
-                            "axisColorMode": "text",
-                            "axisLabel": "",
-                            "axisPlacement": "auto",
-                            "barAlignment": 0,
-                            "drawStyle": "line",
-                            "fillOpacity": 0,
-                            "gradientMode": "none",
-                            "hideFrom": {
-                                "legend": false,
-                                "tooltip": false,
-                                "viz": false
-                            },
-                            "lineInterpolation": "linear",
-                            "lineWidth": 1,
-                            "pointSize": 5,
-                            "scaleDistribution": {
-                                "type": "linear"
-                            },
-                            "showPoints": "auto",
-                            "spanNulls": false,
-                            "stacking": {
-                                "group": "A",
-                                "mode": "none"
-                            },
-                            "thresholdsStyle": {
-                                "mode": "off"
-                            }
-                        },
-                        "mappings": [],
-                        "thresholds": {
-                            "mode": "absolute",
-                            "steps": [
-                                {
-                                    "color": "green",
-                                    "value": null
-                                },
-                                {
-                                    "color": "red",
-                                    "value": 80
-                                }
-                            ]
-                        },
-                        "unit": "decbytes"
-                    },
-                    "overrides": []
-                },
-                "gridPos": {
-                    "h": 7,
-                    "w": 7,
-                    "x": 14,
-                    "y": 64
-                },
-                "id": 9,
-                "options": {
-                    "legend": {
-                        "calcs": [],
-                        "displayMode": "list",
-                        "placement": "bottom",
-                        "showLegend": true
-                    },
-                    "tooltip": {
-                        "mode": "single",
-                        "sort": "none"
-                    }
-                },
-                "targets": [
-                    {
-                        "datasource": {
-                            "type": "prometheus",
-                            "uid": "PBFA97CFB590B2093"
-                        },
-                        "editorMode": "builder",
-                        "expr": "pool_record_start_time",
+                        "expr": "lvol_unmap_bytes",
                         "legendFormat": "__auto",
                         "range": true,
                         "refId": "A"
                     }
                 ],
-                "title": "pool_record_start_time",
+                "title": "lvol_unmap_bytes",
                 "type": "timeseries"
             }
         ],
         "refresh": "",
         "schemaVersion": 38,
         "style": "dark",
         "tags": [],
@@ -2623,13 +2334,13 @@
         },
         "time": {
             "from": "now-1h",
             "to": "now"
         },
         "timepicker": {},
         "timezone": "",
-        "title": "PoolsDashboard",
-        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e40",
+        "title": "LvolsDashboard",
+        "uid": "d56e0ae7-48d5-481d-a2ea-3192da4d9e19",
         "version": 5,
         "weekStart": ""
     }
 }
```

## Comparing `sbcli_dev-2.5.7/simplyblock_core/controllers/device_controller.py` & `sbcli_dev-2.5.8/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/controllers/mgmt_events.py` & `sbcli_dev-2.5.8/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/controllers/events_controller.py` & `sbcli_dev-2.5.8/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/controllers/storage_events.py` & `sbcli_dev-2.5.8/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/controllers/lvol_events.py` & `sbcli_dev-2.5.8/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_dev-2.5.8/simplyblock_core/controllers/snapshot_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/controllers/device_events.py` & `sbcli_dev-2.5.8/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/controllers/pool_controller.py` & `sbcli_dev-2.5.8/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/controllers/cluster_events.py` & `sbcli_dev-2.5.8/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_dev-2.5.8/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/controllers/snapshot_events.py` & `sbcli_dev-2.5.8/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/controllers/lvol_controller.py` & `sbcli_dev-2.5.8/simplyblock_core/controllers/lvol_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/controllers/health_controller.py` & `sbcli_dev-2.5.8/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/controllers/pool_events.py` & `sbcli_dev-2.5.8/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/events.py` & `sbcli_dev-2.5.8/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/iface.py` & `sbcli_dev-2.5.8/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/base_model.py` & `sbcli_dev-2.5.8/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/lvol_model.py` & `sbcli_dev-2.5.8/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/compute_node.py` & `sbcli_dev-2.5.8/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/snapshot.py` & `sbcli_dev-2.5.8/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/pool.py` & `sbcli_dev-2.5.8/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/global_settings.py` & `sbcli_dev-2.5.8/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/port_stat.py` & `sbcli_dev-2.5.8/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/storage_node.py` & `sbcli_dev-2.5.8/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/stats.py` & `sbcli_dev-2.5.8/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/cluster.py` & `sbcli_dev-2.5.8/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/mgmt_node.py` & `sbcli_dev-2.5.8/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/caching_node.py` & `sbcli_dev-2.5.8/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_core/models/nvme_device.py` & `sbcli_dev-2.5.8/simplyblock_core/models/nvme_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/caching_node_app_k8s.py` & `sbcli_dev-2.5.8/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/node_utils.py` & `sbcli_dev-2.5.8/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/snode_app.py` & `sbcli_dev-2.5.8/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/app.py` & `sbcli_dev-2.5.8/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/auth_middleware.py` & `sbcli_dev-2.5.8/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/caching_node_app.py` & `sbcli_dev-2.5.8/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/utils.py` & `sbcli_dev-2.5.8/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/node_webapp.py` & `sbcli_dev-2.5.8/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/static/delete.py` & `sbcli_dev-2.5.8/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/static/deploy.py` & `sbcli_dev-2.5.8/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_dev-2.5.8/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_dev-2.5.8/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_dev-2.5.8/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_dev-2.5.8/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/blueprints/snode_ops.py` & `sbcli_dev-2.5.8/simplyblock_web/blueprints/snode_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,27 +189,27 @@
 
 def delete_cluster_id():
     out, _, _ = node_utils.run_command(f"rm -f {cluster_id_file}")
     return out
 
 
 def get_ec2_meta():
-    stream = os.popen('curl -X PUT "http://169.254.169.254/latest/api/token" -H "X-aws-ec2-metadata-token-ttl-seconds: 21600"')
+    stream = os.popen('curl -X PUT "http://169.254.169.254/latest/api/token" -H "X-aws-ec2-metadata-token-ttl-seconds: 1"')
     token = stream.read()
     stream = os.popen(f"curl -H \"X-aws-ec2-metadata-token: {token}\" http://169.254.169.254/latest/dynamic/instance-identity/document")
     out = stream.read()
     try:
         data = json.loads(out)
         return data
     except:
         return {}
 
 
 def get_ec2_public_ip():
-    stream = os.popen('curl -X PUT "http://169.254.169.254/latest/api/token" -H "X-aws-ec2-metadata-token-ttl-seconds: 21600"')
+    stream = os.popen('curl -X PUT "http://169.254.169.254/latest/api/token" -H "X-aws-ec2-metadata-token-ttl-seconds: 1"')
     token = stream.read()
     stream = os.popen(f"curl -H \"X-aws-ec2-metadata-token: {token}\" http://169.254.169.254/latest/meta-data/public-ipv4")
     response = stream.read()
     out = response if "404" not in response else None
     return out
```

## Comparing `sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/blueprints/csi.py` & `sbcli_dev-2.5.8/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_dev-2.5.8/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_dev-2.5.8/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_device.py` & `sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_dev-2.5.8/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.5.7/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_dev-2.5.8/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

