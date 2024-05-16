# Comparing `tmp/rapyuta-io-cli-7.3.3.tar.gz` & `tmp/rapyuta-io-cli-7.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapyuta-io-cli-7.3.3.tar", last modified: Wed Mar 27 05:51:19 2024, max compression
+gzip compressed data, was "rapyuta-io-cli-7.4.0.tar", last modified: Thu May 16 12:01:51 2024, max compression
```

## Comparing `rapyuta-io-cli-7.3.3.tar` & `rapyuta-io-cli-7.4.0.tar`

### file list

```diff
@@ -1,210 +1,220 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.606536 rapyuta-io-cli-7.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-03-27 05:51:19.606536 rapyuta-io-cli-7.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.586536 rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-03-27 05:51:19.000000 rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-03-27 05:51:19.000000 rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 05:51:19.000000 rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-27 05:51:19.000000 rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-27 05:51:19.000000 rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 05:51:19.000000 rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.586536 rapyuta-io-cli-7.3.3/riocli/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.586536 rapyuta-io-cli-7.3.3/riocli/apply/
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/apply/explain.py
--rw-r--r--   0 runner    (1001) docker     (127)    16534 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/apply/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/apply/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/apply/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/apply/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.590536 rapyuta-io-cli-7.3.3/riocli/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/logout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/staging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.590536 rapyuta-io-cli-7.3.3/riocli/chart/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.590536 rapyuta-io-cli-7.3.3/riocli/completion/
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/completion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.590536 rapyuta-io-cli-7.3.3/riocli/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.590536 rapyuta-io-cli-7.3.3/riocli/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/constants/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/constants/symbols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.590536 rapyuta-io-cli-7.3.3/riocli/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18482 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.594536 rapyuta-io-cli-7.3.3/riocli/device/
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/onboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.594536 rapyuta-io-cli-7.3.3/riocli/device/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/device_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/rapyuta_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/scp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.594536 rapyuta-io-cli-7.3.3/riocli/disk/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/disk/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/disk/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/disk/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/disk/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/disk/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.594536 rapyuta-io-cli-7.3.3/riocli/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.594536 rapyuta-io-cli-7.3.3/riocli/jsonschema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/jsonschema/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.594536 rapyuta-io-cli-7.3.3/riocli/managedservice/
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/managedservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/managedservice/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/managedservice/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/managedservice/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/managedservice/list_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/managedservice/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.594536 rapyuta-io-cli-7.3.3/riocli/model/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.598536 rapyuta-io-cli-7.3.3/riocli/network/
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/native_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/routed_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.598536 rapyuta-io-cli-7.3.3/riocli/organization/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/invite_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/remove_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.598536 rapyuta-io-cli-7.3.3/riocli/package/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/package/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/package/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/package/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/package/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/package/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/package/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.598536 rapyuta-io-cli-7.3.3/riocli/parameter/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.598536 rapyuta-io-cli-7.3.3/riocli/project/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.598536 rapyuta-io-cli-7.3.3/riocli/project/features/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/features/vpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.602536 rapyuta-io-cli-7.3.3/riocli/rosbag/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/rosbag/blob.py
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/rosbag/job.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/rosbag/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.602536 rapyuta-io-cli-7.3.3/riocli/secret/
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/secret/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/secret/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/secret/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/secret/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.602536 rapyuta-io-cli-7.3.3/riocli/shell/
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/shell/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.602536 rapyuta-io-cli-7.3.3/riocli/static_route/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.602536 rapyuta-io-cli-7.3.3/riocli/usergroup/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/usergroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/usergroup/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/usergroup/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/usergroup/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/usergroup/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/usergroup/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.602536 rapyuta-io-cli-7.3.3/riocli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.602536 rapyuta-io-cli-7.3.3/riocli/v2client/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/v2client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/v2client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.606536 rapyuta-io-cli-7.3.3/riocli/vpn/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/vpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/vpn/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/vpn/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/vpn/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/vpn/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/vpn/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 05:51:19.606536 rapyuta-io-cli-7.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.853839 rapyuta-io-cli-7.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-16 12:01:51.853839 rapyuta-io-cli-7.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.833840 rapyuta-io-cli-7.4.0/rapyuta_io_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-05-16 12:01:51.000000 rapyuta-io-cli-7.4.0/rapyuta_io_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4860 2024-05-16 12:01:51.000000 rapyuta-io-cli-7.4.0/rapyuta_io_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 12:01:51.000000 rapyuta-io-cli-7.4.0/rapyuta_io_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 12:01:51.000000 rapyuta-io-cli-7.4.0/rapyuta_io_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-16 12:01:51.000000 rapyuta-io-cli-7.4.0/rapyuta_io_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 12:01:51.000000 rapyuta-io-cli-7.4.0/rapyuta_io_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.833840 rapyuta-io-cli-7.4.0/riocli/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.833840 rapyuta-io-cli-7.4.0/riocli/apply/
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/apply/explain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16293 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/apply/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8491 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/apply/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/apply/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/apply/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.833840 rapyuta-io-cli-7.4.0/riocli/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/auth/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/auth/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/auth/refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/auth/staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/auth/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/auth/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/auth/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4069 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.833840 rapyuta-io-cli-7.4.0/riocli/chart/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/chart/apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/chart/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/chart/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/chart/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/chart/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/chart/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/chart/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.837839 rapyuta-io-cli-7.4.0/riocli/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/completion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.837839 rapyuta-io-cli-7.4.0/riocli/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1796 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5418 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.837839 rapyuta-io-cli-7.4.0/riocli/configtree/
+-rw-r--r--   0 runner    (1001) docker     (127)     1612 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/configtree/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1821 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/configtree/etcd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5827 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/configtree/import_keys.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16367 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/configtree/revision.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10455 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/configtree/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4589 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/configtree/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.837839 rapyuta-io-cli-7.4.0/riocli/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/constants/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/constants/symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.837839 rapyuta-io-cli-7.4.0/riocli/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/deployment/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/deployment/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/deployment/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/deployment/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/deployment/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/deployment/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18482 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/deployment/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/deployment/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/deployment/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/deployment/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/deployment/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.841839 rapyuta-io-cli-7.4.0/riocli/device/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/onboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.841839 rapyuta-io-cli-7.4.0/riocli/device/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/tools/device_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/tools/forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/tools/rapyuta_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/tools/scp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/tools/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/tools/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/device/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.841839 rapyuta-io-cli-7.4.0/riocli/disk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/disk/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/disk/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/disk/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/disk/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/disk/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.841839 rapyuta-io-cli-7.4.0/riocli/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.841839 rapyuta-io-cli-7.4.0/riocli/jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/jsonschema/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.841839 rapyuta-io-cli-7.4.0/riocli/managedservice/
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/managedservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/managedservice/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/managedservice/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/managedservice/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/managedservice/list_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/managedservice/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.841839 rapyuta-io-cli-7.4.0/riocli/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.841839 rapyuta-io-cli-7.4.0/riocli/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/network/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/network/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/network/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/network/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/network/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/network/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/network/native_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/network/routed_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/network/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.845840 rapyuta-io-cli-7.4.0/riocli/organization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/organization/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/organization/invite_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/organization/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/organization/remove_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/organization/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/organization/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/organization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.845840 rapyuta-io-cli-7.4.0/riocli/package/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/package/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/package/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/package/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/package/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/package/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/package/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.845840 rapyuta-io-cli-7.4.0/riocli/parameter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/parameter/apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/parameter/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/parameter/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/parameter/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/parameter/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/parameter/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/parameter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.845840 rapyuta-io-cli-7.4.0/riocli/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/project/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/project/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.845840 rapyuta-io-cli-7.4.0/riocli/project/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/project/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/project/features/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/project/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/project/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/project/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/project/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/project/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/project/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.845840 rapyuta-io-cli-7.4.0/riocli/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/rosbag/blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/rosbag/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/rosbag/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.849840 rapyuta-io-cli-7.4.0/riocli/secret/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/secret/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/secret/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/secret/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/secret/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.849840 rapyuta-io-cli-7.4.0/riocli/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/shell/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.849840 rapyuta-io-cli-7.4.0/riocli/static_route/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/static_route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/static_route/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/static_route/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/static_route/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/static_route/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/static_route/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/static_route/open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/static_route/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.849840 rapyuta-io-cli-7.4.0/riocli/usergroup/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/usergroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/usergroup/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/usergroup/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/usergroup/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/usergroup/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/usergroup/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.849840 rapyuta-io-cli-7.4.0/riocli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2896 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/utils/graph.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/utils/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/utils/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/utils/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/utils/ssh_tunnel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2400 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/utils/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.849840 rapyuta-io-cli-7.4.0/riocli/v2client/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/v2client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23879 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/v2client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 12:01:51.853839 rapyuta-io-cli-7.4.0/riocli/vpn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/vpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/vpn/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/vpn/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4190 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/vpn/machines.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/vpn/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/vpn/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5654 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/riocli/vpn/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 12:01:51.853839 rapyuta-io-cli-7.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-16 12:01:44.000000 rapyuta-io-cli-7.4.0/setup.py
```

### Comparing `rapyuta-io-cli-7.3.3/PKG-INFO` & `rapyuta-io-cli-7.4.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 7.3.3
+Version: 7.4.0
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: UNKNOWN
 Description: # Rapyuta CLI
```

### Comparing `rapyuta-io-cli-7.3.3/README.md` & `rapyuta-io-cli-7.4.0/README.md`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/PKG-INFO` & `rapyuta-io-cli-7.4.0/rapyuta_io_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 7.3.3
+Version: 7.4.0
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: UNKNOWN
 Description: # Rapyuta CLI
```

### Comparing `rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/SOURCES.txt` & `rapyuta-io-cli-7.4.0/rapyuta_io_cli.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -30,14 +30,20 @@
 riocli/chart/info.py
 riocli/chart/list.py
 riocli/chart/search.py
 riocli/chart/util.py
 riocli/completion/__init__.py
 riocli/config/__init__.py
 riocli/config/config.py
+riocli/configtree/__init__.py
+riocli/configtree/etcd.py
+riocli/configtree/import_keys.py
+riocli/configtree/revision.py
+riocli/configtree/tree.py
+riocli/configtree/util.py
 riocli/constants/__init__.py
 riocli/constants/colors.py
 riocli/constants/symbols.py
 riocli/deployment/__init__.py
 riocli/deployment/delete.py
 riocli/deployment/errors.py
 riocli/deployment/execute.py
@@ -159,19 +165,22 @@
 riocli/usergroup/list.py
 riocli/usergroup/model.py
 riocli/usergroup/util.py
 riocli/utils/__init__.py
 riocli/utils/cache.py
 riocli/utils/context.py
 riocli/utils/execute.py
+riocli/utils/graph.py
 riocli/utils/mermaid.py
 riocli/utils/selector.py
 riocli/utils/spinner.py
 riocli/utils/ssh_tunnel.py
+riocli/utils/state.py
 riocli/v2client/__init__.py
 riocli/v2client/client.py
 riocli/vpn/__init__.py
 riocli/vpn/connect.py
 riocli/vpn/disconnect.py
+riocli/vpn/machines.py
 riocli/vpn/ping.py
 riocli/vpn/status.py
 riocli/vpn/util.py
```

### Comparing `rapyuta-io-cli-7.3.3/riocli/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/__main__.py` & `rapyuta-io-cli-7.4.0/riocli/__main__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/apply/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/apply/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/apply/explain.py` & `rapyuta-io-cli-7.4.0/riocli/apply/explain.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/apply/parse.py` & `rapyuta-io-cli-7.4.0/riocli/apply/parse.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import yaml
 from tabulate import tabulate
 
 from riocli.apply.resolver import ResolverCache
 from riocli.config import Configuration
 from riocli.constants import Colors, Symbols
 from riocli.utils import dump_all_yaml, print_separator, run_bash
-from riocli.utils.mermaid import mermaid_link, mermaid_safe
+from riocli.utils.graph import Graphviz
 from riocli.utils.spinner import with_spinner
 
 
 class Applier(object):
     DEFAULT_MAX_WORKERS = 6
 
     EXPECTED_TIME = {
@@ -56,15 +56,15 @@
         self.objects = {}
         self.resolved_objects = {}
         self.files = {}
         self.graph = TopologicalSorter()
         self.rc = ResolverCache(self.client)
         self.secrets = {}
         self.values = {}
-        self.diagram = ["flowchart LR"]
+        self.diagram = Graphviz(direction='LR', format='svg')
         if values or secrets:
             self.environment = jinja2.Environment()
 
         if values:
             self.values = self._load_file_content(
                 values, is_value=True, is_secret=False)[0]
 
@@ -300,21 +300,19 @@
 
         return loaded_data
 
     # Graph Operations
 
     def _add_graph_node(self, key):
         self.graph.add(key)
-        self.diagram.append('\t{}[{}]'.format(mermaid_safe(key), key))
+        self.diagram.node(key)
 
     def _add_graph_edge(self, dependent_key, key):
         self.graph.add(dependent_key, key)
-        self.diagram.append('\t{}[{}] --> {}[{}] '.format(mermaid_safe(key),
-                                                          key, mermaid_safe(
-                dependent_key), dependent_key))
+        self.diagram.edge(key, dependent_key)
 
     # Dependency Resolution
     def _parse_dependency(self, dependent_key, model):
         for key, value in model.items():
             if key == "depends":
                 if 'kind' in value and value.get('kind'):
                     self._resolve_dependency(dependent_key, value)
@@ -398,16 +396,15 @@
 
     def _initialize_kind_dependency(self, kind):
         if not self.dependencies.get(kind):
             self.dependencies[kind] = {}
 
     def show_dependency_graph(self):
         """Lauches mermaid.live dependency graph"""
-        link = mermaid_link("\n".join(self.diagram))
-        click.launch(link)
+        self.diagram.visualize()
 
     # Utils
     def _display_context(
             self,
             total_time: int,
             total_objects: int,
             resource_list: typing.List
```

### Comparing `rapyuta-io-cli-7.3.3/riocli/apply/resolver.py` & `rapyuta-io-cli-7.4.0/riocli/apply/resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2022 Rapyuta Robotics
+# Copyright 2024 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -112,15 +112,15 @@
                 return self._guid_functor(depends['kind'])(obj_match[0]), obj_match[0]
             else:
                 return None, None
         return None, None
 
     def _guid_functor(self, kind):
         mapping = {
-            'secret': lambda x: munchify(x).guid,
+            'secret': lambda x: munchify(x).metadata.name,
             "project": lambda x: munchify(x).metadata.guid,
             "package": lambda x: munchify(x)['id'],
             "staticroute": lambda x: munchify(x)['metadata']['guid'],
             "deployment": lambda x: munchify(x)['deploymentId'],
             "network": lambda x: munchify(x).guid,
             # This is only temporarily like this
             "disk": lambda x: munchify(x)['internalDeploymentGUID'],
@@ -146,15 +146,15 @@
             "usergroup": self.client.list_usergroups
         }
 
         return mapping[kind]
 
     def _find_functors(self, kind):
         mapping = {
-            'secret': self._generate_find_guid_functor(),
+            'secret': lambda name, secrets: filter(lambda i: i.metadata.name == name, secrets),
             "project": lambda name, projects: filter(lambda i: i.metadata.name == name, projects),
             "package": lambda name, obj_list, version: filter(
                 lambda x: name == x.name and version == x['packageVersion'], obj_list),
             "staticroute": lambda name, obj_list: filter(
                 lambda x: name == x.metadata.name.rsplit('-', 1)[0], obj_list),
             "deployment": self._generate_find_guid_functor(),
             "network": self._generate_find_guid_functor(),
```

### Comparing `rapyuta-io-cli-7.3.3/riocli/apply/template.py` & `rapyuta-io-cli-7.4.0/riocli/apply/template.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/apply/util.py` & `rapyuta-io-cli-7.4.0/riocli/apply/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/auth/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/auth/login.py` & `rapyuta-io-cli-7.4.0/riocli/auth/login.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/auth/logout.py` & `rapyuta-io-cli-7.4.0/riocli/auth/logout.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/auth/refresh_token.py` & `rapyuta-io-cli-7.4.0/riocli/auth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/auth/staging.py` & `rapyuta-io-cli-7.4.0/riocli/auth/staging.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/auth/status.py` & `rapyuta-io-cli-7.4.0/riocli/auth/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/auth/token.py` & `rapyuta-io-cli-7.4.0/riocli/auth/token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/auth/util.py` & `rapyuta-io-cli-7.4.0/riocli/auth/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/bootstrap.py` & `rapyuta-io-cli-7.4.0/riocli/bootstrap.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,36 +1,37 @@
 # -*- coding: utf-8 -*-
-# Copyright 2021 Rapyuta Robotics
+# Copyright 2024 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "7.3.3"
+__version__ = "7.4.0"
 
 import click
 import rapyuta_io.version
 from click import Context
 from click_help_colors import HelpColorsGroup
 from click_plugins import with_plugins
 from pkg_resources import iter_entry_points
 
 from riocli.apply import apply, explain, delete, template
 from riocli.auth import auth
 from riocli.chart import chart
 from riocli.completion import completion
 from riocli.config import Configuration
+from riocli.configtree import config_trees
 from riocli.constants import Colors, Symbols
 from riocli.deployment import deployment
 from riocli.device import device
 from riocli.disk import disk
 from riocli.managedservice import managedservice
 from riocli.network import network
 from riocli.organization import organization
@@ -132,7 +133,8 @@
 cli.add_command(shell)
 cli.add_command(deprecated_repl)
 cli.add_command(managedservice)
 cli.add_command(template)
 cli.add_command(organization)
 cli.add_command(vpn)
 cli.add_command(usergroup)
+cli.add_command(config_trees)
```

### Comparing `rapyuta-io-cli-7.3.3/riocli/chart/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/chart/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/chart/apply.py` & `rapyuta-io-cli-7.4.0/riocli/chart/apply.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/chart/chart.py` & `rapyuta-io-cli-7.4.0/riocli/chart/chart.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/chart/delete.py` & `rapyuta-io-cli-7.4.0/riocli/chart/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/chart/info.py` & `rapyuta-io-cli-7.4.0/riocli/chart/info.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/chart/list.py` & `rapyuta-io-cli-7.4.0/riocli/chart/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/chart/search.py` & `rapyuta-io-cli-7.4.0/riocli/chart/search.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/chart/util.py` & `rapyuta-io-cli-7.4.0/riocli/chart/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/completion/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/config/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/config/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+import click
 from riocli.config.config import Configuration
 
 
 def new_client(config_inst: Configuration = None, with_project: bool = True):
     """
     new_client is a simple wrapper around the Configuration's new_client method. It can be called
     directly without initializing the Configuration first. It initializes the Configuration if not
@@ -24,15 +25,24 @@
         config_inst = Configuration()
 
     return config_inst.new_client(with_project=with_project)
 
 
 def new_v2_client(config_inst: Configuration = None, with_project: bool = True):
     """
-        new_v2_client is a simple wrapper around the Configuration's new_v2_client method. It can be called
-        directly without initializing the Configuration first. It initializes the Configuration if not
-        given already and then calls its new_client method.
-        """
+    new_v2_client is a simple wrapper around the Configuration's new_v2_client method. It can be called
+    directly without initializing the Configuration first. It initializes the Configuration if not
+    given already and then calls its new_client method.
+    """
     if not config_inst:
         config_inst = Configuration()
 
     return config_inst.new_v2_client(with_project=with_project)
+
+
+def get_config_from_context(ctx: click.Context) -> Configuration:
+    config_obj = ctx.obj
+
+    if not isinstance(config_obj, Configuration):
+        return Configuration()
+
+    return config_obj
```

### Comparing `rapyuta-io-cli-7.3.3/riocli/config/config.py` & `rapyuta-io-cli-7.4.0/riocli/config/config.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,24 +7,27 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
+
 import errno
 import json
 import os
 import uuid
 from functools import lru_cache
+from typing import Optional
 
 from click import get_app_dir
 from rapyuta_io import Client
 
-from riocli.exceptions import LoggedOut, NoProjectSelected
+from riocli.exceptions import LoggedOut, NoOrganizationSelected, NoProjectSelected
 from riocli.v2client import Client as v2Client
 
 
 class Configuration(object):
     """
     Configuration defines a class to define operations on the CLI's configuration file centrally.
     The class can be initialized irrespective of if the actual file exists or not. The object will
@@ -37,28 +40,29 @@
             "auth_token": "<rapyuta-auth-token>",
             "project_id": "<project-guid>"
         }
     """
     APP_NAME = 'rio-cli'
     PIPING_SERVER = 'https://piping-server-v0-rapyuta-infra.apps.okd4v2.okd4beta.rapyuta.io'
 
-    def __init__(self, filepath: str = None):
-        self.filepath = filepath
+    def __init__(self, filepath: Optional[str] = None):
+        self._filepath = filepath
         self.exists = True
 
+
         # If config file does not exist, then initialize an empty dictionary instead.
         if not os.path.exists(self.filepath):
             self.exists = False
             self.data = dict()
             return
 
         with open(self.filepath, 'r') as config_file:
             self.data = json.load(config_file)
 
-    def save(self):
+    def save(self: Configuration):
         if not os.path.exists(self.filepath):
             try:
                 os.makedirs(os.path.dirname(self.filepath))
             except OSError as exc:  # Guard against race condition
                 if exc.errno != errno.EEXIST:
                     raise
 
@@ -66,15 +70,15 @@
             json.dump(self.data, config_file)
 
     # We are using lru_cache to cache the calls to new_v2_client
     # with project and without project. This is to avoid creating a
     # new client object every time we call new_v2_client.
     # https://docs.python.org/3.8/library/functools.html#functools.lru_cache
     @lru_cache(maxsize=2)
-    def new_client(self, with_project: bool = True) -> Client:
+    def new_client(self: Configuration, with_project: bool = True) -> Client:
         if 'auth_token' not in self.data:
             raise LoggedOut
 
         if 'environment' in self.data:
             os.environ['RIO_CONFIG'] = self.filepath
 
         token = self.data.get('auth_token', None)
@@ -84,15 +88,15 @@
 
         if not with_project:
             project = None
 
         return Client(auth_token=token, project=project)
 
     @lru_cache(maxsize=2)
-    def new_v2_client(self, with_project: bool = True) -> v2Client:
+    def new_v2_client(self: Configuration, with_project: bool = True) -> v2Client:
         if 'auth_token' not in self.data:
             raise LoggedOut
 
         if 'environment' in self.data:
             os.environ['RIO_CONFIG'] = self.filepath
 
         token = self.data.get('auth_token', None)
@@ -101,39 +105,60 @@
             raise NoProjectSelected
 
         if not with_project:
             project = None
 
         return v2Client(self, auth_token=token, project=project)
 
-    def get_auth_header(self) -> dict:
+    def get_auth_header(self: Configuration) -> dict:
         if not ('auth_token' in self.data and 'project_id' in self.data):
             raise LoggedOut
 
         token, project = self.data['auth_token'], self.data['project_id']
         if not token.startswith('Bearer'):
             token = 'Bearer {}'.format(token)
 
         return dict(Authorization=token, project=project)
 
     @property
-    def filepath(self) -> str:
+    def filepath(self: Configuration) -> str:
         path = self._filepath
         if path is None:
             path = os.path.join(get_app_dir(self.APP_NAME), "config.json")
         return os.path.abspath(path)
 
-    @filepath.setter
-    def filepath(self, value: str):
-        self._filepath = value
+    @property
+    def project_guid(self: Configuration) -> str:
+        if 'auth_token' not in self.data:
+            raise LoggedOut
+
+        if 'organization_id' not in self.data:
+            raise NoOrganizationSelected
+
+        guid = self.data.get('project_id')
+        if guid is None:
+            raise NoProjectSelected
+
+        return guid
+
+    @property
+    def organization_guid(self: Configuration) -> str:
+        if 'auth_token' not in self.data:
+            raise LoggedOut
+
+        guid = self.data.get('organization_id')
+        if guid is None:
+            raise NoOrganizationSelected
+
+        return guid
 
     @property
-    def piping_server(self):
+    def piping_server(self: Configuration):
         return self.data.get('piping_server', self.PIPING_SERVER)
 
     @property
-    def machine_id(self):
+    def machine_id(self: Configuration):
         if 'machine_id' not in self.data:
             self.data['machine_id'] = str(uuid.uuid4())
             self.save()
 
         return self.data.get('machine_id')
```

### Comparing `rapyuta-io-cli-7.3.3/riocli/constants/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/constants/colors.py` & `rapyuta-io-cli-7.4.0/riocli/constants/colors.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/constants/symbols.py` & `rapyuta-io-cli-7.4.0/riocli/constants/symbols.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/deployment/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/deployment/delete.py` & `rapyuta-io-cli-7.4.0/riocli/deployment/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/deployment/errors.py` & `rapyuta-io-cli-7.4.0/riocli/deployment/errors.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/deployment/execute.py` & `rapyuta-io-cli-7.4.0/riocli/deployment/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/deployment/inspect.py` & `rapyuta-io-cli-7.4.0/riocli/deployment/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/deployment/list.py` & `rapyuta-io-cli-7.4.0/riocli/deployment/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/deployment/logs.py` & `rapyuta-io-cli-7.4.0/riocli/deployment/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/deployment/model.py` & `rapyuta-io-cli-7.4.0/riocli/deployment/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/deployment/status.py` & `rapyuta-io-cli-7.4.0/riocli/deployment/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/deployment/update.py` & `rapyuta-io-cli-7.4.0/riocli/deployment/update.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/deployment/util.py` & `rapyuta-io-cli-7.4.0/riocli/deployment/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/deployment/wait.py` & `rapyuta-io-cli-7.4.0/riocli/deployment/wait.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/device/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/config.py` & `rapyuta-io-cli-7.4.0/riocli/device/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/create.py` & `rapyuta-io-cli-7.4.0/riocli/device/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/delete.py` & `rapyuta-io-cli-7.4.0/riocli/device/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/deployment.py` & `rapyuta-io-cli-7.4.0/riocli/device/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/execute.py` & `rapyuta-io-cli-7.4.0/riocli/device/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/files.py` & `rapyuta-io-cli-7.4.0/riocli/device/files.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/inspect.py` & `rapyuta-io-cli-7.4.0/riocli/device/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/label.py` & `rapyuta-io-cli-7.4.0/riocli/device/label.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/list.py` & `rapyuta-io-cli-7.4.0/riocli/device/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/metric.py` & `rapyuta-io-cli-7.4.0/riocli/device/metric.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/model.py` & `rapyuta-io-cli-7.4.0/riocli/device/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/onboard.py` & `rapyuta-io-cli-7.4.0/riocli/device/onboard.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/tools/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/device/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/tools/device_init.py` & `rapyuta-io-cli-7.4.0/riocli/device/tools/device_init.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/tools/forward.py` & `rapyuta-io-cli-7.4.0/riocli/device/tools/forward.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/tools/rapyuta_logs.py` & `rapyuta-io-cli-7.4.0/riocli/device/tools/rapyuta_logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/tools/scp.py` & `rapyuta-io-cli-7.4.0/riocli/device/tools/scp.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/tools/service.py` & `rapyuta-io-cli-7.4.0/riocli/device/tools/service.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/tools/ssh.py` & `rapyuta-io-cli-7.4.0/riocli/device/tools/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/tools/util.py` & `rapyuta-io-cli-7.4.0/riocli/device/tools/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/topic.py` & `rapyuta-io-cli-7.4.0/riocli/device/topic.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/util.py` & `rapyuta-io-cli-7.4.0/riocli/device/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/device/vpn.py` & `rapyuta-io-cli-7.4.0/riocli/device/vpn.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/disk/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/disk/create.py` & `rapyuta-io-cli-7.4.0/riocli/disk/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/disk/delete.py` & `rapyuta-io-cli-7.4.0/riocli/disk/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/disk/list.py` & `rapyuta-io-cli-7.4.0/riocli/disk/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/disk/model.py` & `rapyuta-io-cli-7.4.0/riocli/disk/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/disk/util.py` & `rapyuta-io-cli-7.4.0/riocli/disk/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/exceptions/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/exceptions/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -16,13 +16,21 @@
 
     def __str__(self):
         return """No project is selected. Select a project first
         $ rio project select 
         """
 
 
+class NoOrganizationSelected(Exception):
+
+    def __str__(self):
+        return """No organization is selected. Select an organization first
+        $ rio organization select
+        """
+
+
 class LoggedOut(Exception):
 
     def __str__(self):
         return """Not logged in. Please login first
         $ rio auth login 
         """
```

### Comparing `rapyuta-io-cli-7.3.3/riocli/jsonschema/validate.py` & `rapyuta-io-cli-7.4.0/riocli/jsonschema/validate.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/managedservice/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/managedservice/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/managedservice/delete.py` & `rapyuta-io-cli-7.4.0/riocli/managedservice/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/managedservice/inspect.py` & `rapyuta-io-cli-7.4.0/riocli/managedservice/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/managedservice/list.py` & `rapyuta-io-cli-7.4.0/riocli/managedservice/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/managedservice/list_providers.py` & `rapyuta-io-cli-7.4.0/riocli/managedservice/list_providers.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/managedservice/model.py` & `rapyuta-io-cli-7.4.0/riocli/managedservice/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/model/base.py` & `rapyuta-io-cli-7.4.0/riocli/model/base.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/network/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/network/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/network/create.py` & `rapyuta-io-cli-7.4.0/riocli/network/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/network/delete.py` & `rapyuta-io-cli-7.4.0/riocli/network/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/network/inspect.py` & `rapyuta-io-cli-7.4.0/riocli/network/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/network/list.py` & `rapyuta-io-cli-7.4.0/riocli/network/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/network/logs.py` & `rapyuta-io-cli-7.4.0/riocli/network/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/network/model.py` & `rapyuta-io-cli-7.4.0/riocli/network/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/network/native_network.py` & `rapyuta-io-cli-7.4.0/riocli/network/native_network.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/network/routed_network.py` & `rapyuta-io-cli-7.4.0/riocli/network/routed_network.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/network/util.py` & `rapyuta-io-cli-7.4.0/riocli/network/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/organization/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/organization/inspect.py` & `rapyuta-io-cli-7.4.0/riocli/organization/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/organization/invite_user.py` & `rapyuta-io-cli-7.4.0/riocli/organization/invite_user.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/organization/list.py` & `rapyuta-io-cli-7.4.0/riocli/organization/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/organization/remove_user.py` & `rapyuta-io-cli-7.4.0/riocli/organization/remove_user.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/organization/select.py` & `rapyuta-io-cli-7.4.0/riocli/organization/select.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/organization/users.py` & `rapyuta-io-cli-7.4.0/riocli/organization/users.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/organization/utils.py` & `rapyuta-io-cli-7.4.0/riocli/organization/utils.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/package/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/package/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/package/delete.py` & `rapyuta-io-cli-7.4.0/riocli/package/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/package/deployment.py` & `rapyuta-io-cli-7.4.0/riocli/package/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/package/inspect.py` & `rapyuta-io-cli-7.4.0/riocli/package/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/package/list.py` & `rapyuta-io-cli-7.4.0/riocli/package/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/package/model.py` & `rapyuta-io-cli-7.4.0/riocli/package/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/package/util.py` & `rapyuta-io-cli-7.4.0/riocli/package/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/parameter/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/parameter/apply.py` & `rapyuta-io-cli-7.4.0/riocli/parameter/apply.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/parameter/delete.py` & `rapyuta-io-cli-7.4.0/riocli/parameter/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/parameter/diff.py` & `rapyuta-io-cli-7.4.0/riocli/parameter/diff.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/parameter/download.py` & `rapyuta-io-cli-7.4.0/riocli/parameter/download.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/parameter/list.py` & `rapyuta-io-cli-7.4.0/riocli/parameter/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/parameter/upload.py` & `rapyuta-io-cli-7.4.0/riocli/parameter/upload.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/parameter/utils.py` & `rapyuta-io-cli-7.4.0/riocli/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/project/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/project/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/project/create.py` & `rapyuta-io-cli-7.4.0/riocli/project/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/project/delete.py` & `rapyuta-io-cli-7.4.0/riocli/project/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/project/features/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/project/features/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/project/features/vpn.py` & `rapyuta-io-cli-7.4.0/riocli/project/features/vpn.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/project/inspect.py` & `rapyuta-io-cli-7.4.0/riocli/project/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/project/list.py` & `rapyuta-io-cli-7.4.0/riocli/project/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/project/model.py` & `rapyuta-io-cli-7.4.0/riocli/project/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/project/select.py` & `rapyuta-io-cli-7.4.0/riocli/project/select.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/project/util.py` & `rapyuta-io-cli-7.4.0/riocli/project/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/project/whoami.py` & `rapyuta-io-cli-7.4.0/riocli/project/whoami.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/rosbag/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/rosbag/blob.py` & `rapyuta-io-cli-7.4.0/riocli/rosbag/blob.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/rosbag/job.py` & `rapyuta-io-cli-7.4.0/riocli/rosbag/job.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/secret/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/secret/delete.py` & `rapyuta-io-cli-7.4.0/riocli/secret/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/secret/inspect.py` & `rapyuta-io-cli-7.4.0/riocli/secret/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/secret/list.py` & `rapyuta-io-cli-7.4.0/riocli/secret/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/secret/model.py` & `rapyuta-io-cli-7.4.0/riocli/secret/model.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-# Copyright 2023 Rapyuta Robotics
+# Copyright 2024 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import typing
-from munch import unmunchify
 
+from munch import unmunchify
 from rapyuta_io import Client
 
 from riocli.config import new_v2_client
 from riocli.jsonschema.validate import load_schema
 from riocli.model import Model
 
+
 class Secret(Model):
     def __init__(self, *args, **kwargs):
         self.update(*args, **kwargs)
 
     def find_object(self, client: Client) -> bool:
         _, secret = self.rc.find_depends({
             'kind': 'secret',
@@ -47,20 +48,20 @@
 
     def update_object(self, client: Client, obj: typing.Any) -> typing.Any:
         client = new_v2_client()
 
         secret = unmunchify(self)
         secret.pop("rc", None)
 
-        r = client.update_secret(obj.name, secret)
+        r = client.update_secret(obj.metadata.name, secret)
         return unmunchify(r)
 
     def delete_object(self, client: Client, obj: typing.Any) -> typing.Any:
         client = new_v2_client()
-        client.delete_secret(obj.name)
+        client.delete_secret(obj.metadata.name)
 
     @classmethod
     def pre_process(cls, client: Client, d: typing.Dict) -> None:
         pass
 
     @staticmethod
     def validate(data):
```

### Comparing `rapyuta-io-cli-7.3.3/riocli/shell/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/shell/prompt.py` & `rapyuta-io-cli-7.4.0/riocli/shell/prompt.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/static_route/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/static_route/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/static_route/create.py` & `rapyuta-io-cli-7.4.0/riocli/static_route/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/static_route/delete.py` & `rapyuta-io-cli-7.4.0/riocli/static_route/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/static_route/inspect.py` & `rapyuta-io-cli-7.4.0/riocli/static_route/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/static_route/list.py` & `rapyuta-io-cli-7.4.0/riocli/static_route/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/static_route/model.py` & `rapyuta-io-cli-7.4.0/riocli/static_route/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/static_route/open.py` & `rapyuta-io-cli-7.4.0/riocli/static_route/open.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/static_route/util.py` & `rapyuta-io-cli-7.4.0/riocli/static_route/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/usergroup/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/usergroup/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/usergroup/delete.py` & `rapyuta-io-cli-7.4.0/riocli/usergroup/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/usergroup/inspect.py` & `rapyuta-io-cli-7.4.0/riocli/usergroup/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/usergroup/list.py` & `rapyuta-io-cli-7.4.0/riocli/usergroup/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/usergroup/model.py` & `rapyuta-io-cli-7.4.0/riocli/usergroup/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/usergroup/util.py` & `rapyuta-io-cli-7.4.0/riocli/usergroup/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/utils/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/utils/cache.py` & `rapyuta-io-cli-7.4.0/riocli/utils/cache.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/utils/context.py` & `rapyuta-io-cli-7.4.0/riocli/utils/context.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/utils/execute.py` & `rapyuta-io-cli-7.4.0/riocli/utils/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/utils/mermaid.py` & `rapyuta-io-cli-7.4.0/riocli/configtree/etcd.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,49 +1,63 @@
-# Copyright 2023 Rapyuta Robotics
+# Copyright 2024 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import base64
-import json
-
-
-def mermaid_safe(s: str):
-    return s.replace(" ", "_")
-
-
-def js_string_to_byte(data: str):
-    return bytes(data, 'iso-8859-1')
-
-
-def js_bytes_to_string(data: bytes):
-    return data.decode('iso-8859-1')
-
+from typing import Optional
+from base64 import b64encode
+from etcd3gw import Etcd3Client
+
+
+def import_in_etcd(data: dict, endpoint: str, port: Optional[int] = None, prefix: Optional[str] = None) -> None:
+    if port is None:
+        port = 2379
+
+    cli = Etcd3Client(host=endpoint, port=port)
+
+    if prefix:
+        cli.delete_prefix(prefix)
+    else:
+        _delete_all_keys(client=cli)
+
+    compares, failures = [], []
+
+    for key, val in data.items():
+        if prefix:
+            key = '{}/{}'.format(prefix, key)
+
+        enc_key = b64encode(str(key).encode('utf-8')).decode()
+        enc_val = b64encode(str(val).encode('utf-8')).decode()
+        compares.append({
+            'key': enc_key,
+            'result': 'EQUAL',
+            'target': 'VALUE',
+            'value': enc_val,
+        })
+        failures.append({
+            'request_put': {
+                'key': enc_key,
+                'value': enc_val
+            }
+        })
+
+    txn = {
+        'compare': compares,
+        'failure': failures,
+    }
 
-def js_btoa(data: bytes):
-    return base64.b64encode(data)
+    cli.transaction(txn)
 
+def _delete_all_keys(client: Etcd3Client) -> None:
+    null_char = '\x00'
+    enc_null  = b64encode(null_char.encode('utf-8')).decode()
 
-def mermaid_link(diagram):
-    obj = {
-        "code": diagram,
-        "mermaid": {
-            "theme": "default"
-        },
-        "updateEditor": False,
-        "autoSync": True,
-        "updateDiagram": False
-    }
-    json_str = json.dumps(obj)
-    json_bytes = js_string_to_byte(json_str)
-    encoded_uri = js_btoa(json_bytes)
-    return 'https://mermaid.live/view#base64:{}'.format(
-        js_bytes_to_string(encoded_uri))
+    client.delete('\x00', range_end=enc_null)
```

### Comparing `rapyuta-io-cli-7.3.3/riocli/utils/selector.py` & `rapyuta-io-cli-7.4.0/riocli/utils/selector.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/utils/spinner.py` & `rapyuta-io-cli-7.4.0/riocli/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/utils/ssh_tunnel.py` & `rapyuta-io-cli-7.4.0/riocli/utils/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/v2client/client.py` & `rapyuta-io-cli-7.4.0/riocli/v2client/client.py`

 * *Files 25% similar despite different names*

```diff
@@ -7,17 +7,22 @@
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from __future__ import annotations
+import os
+
 import http
 import json
-import typing
+import magic
+from typing import List, Optional, Dict, Any
+from hashlib import md5
 
 import requests
 from munch import munchify, Munch
 from rapyuta_io.utils.rest_client import HttpMethod, RestClient
 
 
 def handle_server_errors(response: requests.Response):
@@ -44,73 +49,63 @@
 
 class Client(object):
     """
     v2 API Client
     """
     PROD_V2API_URL = "https://api.rapyuta.io"
 
-    def __init__(self, config, auth_token: str, project: str = None):
-        super().__init__()
+    def __init__(self, config, auth_token: str, project: Optional[str] = None):
         self._config = config
         self._host = config.data.get('v2api_host', self.PROD_V2API_URL)
         self._project = project
-        self._token = auth_token
+        self._token = 'Bearer {}'.format(auth_token)
+
+    def _get_auth_header(self: Client, with_org: bool = False, with_project: bool = True) -> dict:
+        headers = dict(Authorization=self._token)
+
+        if with_project and self._project is not None:
+            headers['project'] = self._project
 
-    def _get_auth_token(self) -> typing.Text:
-        return "Bearer {}".format(self._token)
+        if with_org:
+            headers['organizationguid'] = self._config.organization_guid
+
+        return headers
 
     # Project APIs
 
     def list_projects(
             self,
             organization_guid: str = None,
             query: dict = None
     ) -> Munch:
         """
         List all projects in an organization
         """
 
         url = "{}/v2/projects/".format(self._host)
-        headers = {"Authorization": self._get_auth_token()}
+        headers = self._get_auth_header(with_project=False)
 
         params = {}
 
         if organization_guid:
             params.update({
                 "organizations": organization_guid,
             })
 
         params.update(query or {})
 
-        offset, result = 0, []
-        while True:
-            params.update({
-                "continue": offset,
-                "limit": 500,
-            })
-            response = RestClient(url).method(HttpMethod.GET).query_param(
-                params).headers(headers).execute()
-            data = json.loads(response.text)
-            if not response.ok:
-                err_msg = data.get('error')
-                raise Exception("projects: {}".format(err_msg))
-            projects = data.get('items', [])
-            if not projects:
-                break
-            offset = data['metadata']['continue']
-            result.extend(projects)
-
-        return munchify(result)
+        client = RestClient(url).method(HttpMethod.GET).headers(headers)
+        return self._walk_pages(client, params=params)
 
     def get_project(self, project_guid: str) -> Munch:
         """
         Get a project by its GUID
         """
         url = "{}/v2/projects/{}/".format(self._host, project_guid)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
         response = RestClient(url).method(
             HttpMethod.GET).headers(headers).execute()
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
@@ -120,15 +115,15 @@
         return munchify(data)
 
     def create_project(self, spec: dict) -> Munch:
         """
         Create a new project
         """
         url = "{}/v2/projects/".format(self._host)
-        headers = {"Authorization": self._get_auth_token()}
+        headers = self._get_auth_header(with_project=False)
         response = RestClient(url).method(HttpMethod.POST).headers(
             headers).execute(payload=spec)
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
@@ -138,15 +133,15 @@
         return munchify(data)
 
     def update_project(self, project_guid: str, spec: dict) -> Munch:
         """
         Update an existing project
         """
         url = "{}/v2/projects/{}/".format(self._host, project_guid)
-        headers = {"Authorization": self._get_auth_token()}
+        headers = self._get_auth_header(with_project=False)
         response = RestClient(url).method(HttpMethod.PUT).headers(
             headers).execute(payload=spec)
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
@@ -156,91 +151,77 @@
         return munchify(data)
 
     def delete_project(self, project_guid: str) -> Munch:
         """
         Delete a project by its GUID
         """
         url = "{}/v2/projects/{}/".format(self._host, project_guid)
-        headers = {"Authorization": self._get_auth_token()}
+        headers = self._get_auth_header(with_project=False)
         response = RestClient(url).method(
             HttpMethod.DELETE).headers(headers).execute()
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
             err_msg = data.get('error')
             raise Exception("projects: {}".format(err_msg))
 
         return munchify(data)
 
     # ManagedService APIs
-    def list_providers(self) -> typing.List:
+    def list_providers(self) -> List:
         """
         List all managedservice provider
         """
         url = "{}/v2/managedservices/providers/".format(self._host)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header(with_project=False)
         response = RestClient(url).method(
             HttpMethod.GET).headers(headers).execute()
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
             err_msg = data.get('error')
             raise Exception("managedservice: {}".format(err_msg))
 
         return munchify(data.get('items', []))
 
-    def list_instances(self) -> typing.List:
+    def list_instances(self) -> List:
         """
         List all managedservice instances in a project
         """
         url = "{}/v2/managedservices/".format(self._host)
-        headers = self._config.get_auth_header()
-        offset = 0
-        result = []
-        while True:
-            response = RestClient(url).method(HttpMethod.GET).query_param({
-                "continue": offset,
-            }).headers(headers).execute()
-            data = json.loads(response.text)
-            if not response.ok:
-                err_msg = data.get('error')
-                raise Exception("managedservice: {}".format(err_msg))
-            instances = data.get('items', [])
-            if not instances:
-                break
-            offset = data['metadata']['continue']
-            result.extend(instances)
+        headers = self._get_auth_header()
 
-        return munchify(sorted(result, key=lambda x: x['metadata']['name']))
+        client = RestClient(url).method(HttpMethod.GET).headers(headers)
+        return self._walk_pages(client)
 
     def get_instance(self, instance_name: str) -> Munch:
         """
         Get a managedservice instance by instance_name
         """
         url = "{}/v2/managedservices/{}/".format(self._host, instance_name)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
         response = RestClient(url).method(
             HttpMethod.GET).headers(headers).execute()
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
             err_msg = data.get('error')
             raise Exception("managedservice: {}".format(err_msg))
 
         return munchify(data)
 
-    def create_instance(self, instance: typing.Dict) -> Munch:
+    def create_instance(self, instance: Dict) -> Munch:
         url = "{}/v2/managedservices/".format(self._host)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
 
         response = RestClient(url).method(HttpMethod.POST).headers(
             headers).execute(payload=instance)
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
@@ -248,34 +229,45 @@
             err_msg = data.get('error')
             raise Exception("managedservice: {}".format(err_msg))
 
         return munchify(data)
 
     def delete_instance(self, instance_name) -> Munch:
         url = "{}/v2/managedservices/{}/".format(self._host, instance_name)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
         response = RestClient(url).method(
             HttpMethod.DELETE).headers(headers).execute()
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
             err_msg = data.get('error')
             raise Exception("managedservice: {}".format(err_msg))
 
         return munchify(data)
 
+    def list_instance_bindings(self, instance_name: str, labels: str = '') -> List:
+        """
+        List all managedservice instances in a project
+        """
+        url = "{}/v2/managedservices/{}/bindings/".format(self._host, instance_name)
+        headers = self._get_auth_header()
+
+        client = RestClient(url).method(HttpMethod.GET).headers(headers)
+        return self._walk_pages(client, params={'labelSelector': labels})
+
+
     def create_instance_binding(self, instance_name, binding: dict) -> Munch:
         """
         Create a new managed service instance binding
         """
         url = "{}/v2/managedservices/{}/bindings/".format(
             self._host, instance_name)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
         response = RestClient(url).method(
             HttpMethod.POST).headers(headers).execute(payload=binding)
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
@@ -286,15 +278,15 @@
 
     def get_instance_binding(self, instance_name: str, binding_name: str) -> Munch:
         """
         Get a managed service instance binding
         """
         url = "{}/v2/managedservices/{}/bindings/{}/".format(
             self._host, instance_name, binding_name)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
         response = RestClient(url).method(
             HttpMethod.GET).headers(headers).execute()
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
@@ -305,15 +297,15 @@
 
     def delete_instance_binding(self, instance_name: str, binding_name: str) -> Munch:
         """
         Delete a managed service instance binding
         """
         url = "{}/v2/managedservices/{}/bindings/{}/".format(
             self._host, instance_name, binding_name)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
         response = RestClient(url).method(
             HttpMethod.DELETE).headers(headers).execute()
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
@@ -326,44 +318,28 @@
             self,
             query: dict = None
     ) -> Munch:
         """
         List all static routes in a project
         """
         url = "{}/v2/staticroutes/".format(self._host)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
 
         params = {}
         params.update(query or {})
 
-        offset, result = 0, []
-        while True:
-            params.update({
-                "continue": offset,
-            })
-            response = RestClient(url).method(HttpMethod.GET).query_param(
-                params).headers(headers).execute()
-            data = json.loads(response.text)
-            if not response.ok:
-                err_msg = data.get('error')
-                raise Exception("static routes: {}".format(err_msg))
-            staticRoutes = data.get('items', [])
-            if not staticRoutes:
-                break
-            offset = data['metadata']['continue']
-            result.extend(staticRoutes)
-
-        return munchify(result)
+        client = RestClient(url).method(HttpMethod.GET).headers(headers)
+        return self._walk_pages(client, params=params)
 
     def get_static_route(self, name: str) -> Munch:
         """
         Get a static route by its name
         """
         url = "{}/v2/staticroutes/{}/".format(self._host, name)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
         response = RestClient(url).method(
             HttpMethod.GET).headers(headers).execute()
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
@@ -373,15 +349,15 @@
         return munchify(data)
 
     def create_static_route(self, metadata: dict) -> Munch:
         """
         Create a new static route
         """
         url = "{}/v2/staticroutes/".format(self._host)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
         response = RestClient(url).method(HttpMethod.POST).headers(
             headers).execute(payload=metadata)
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
@@ -391,15 +367,15 @@
         return munchify(data)
 
     def update_static_route(self, name: str, sr: dict) -> Munch:
         """
         Update the new static route
         """
         url = "{}/v2/staticroutes/{}/".format(self._host, name)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
         response = RestClient(url).method(HttpMethod.PUT).headers(
             headers).execute(payload=sr)
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
@@ -409,15 +385,15 @@
         return munchify(data)
 
     def delete_static_route(self, name: str) -> Munch:
         """
         Delete a static route by its name
         """
         url = "{}/v2/staticroutes/{}/".format(self._host, name)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
         response = RestClient(url).method(
             HttpMethod.DELETE).headers(headers).execute()
 
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
@@ -427,15 +403,15 @@
         return munchify(data)
 
     def create_secret(self, payload: dict) -> Munch:
         """
         Create a new secret
         """
         url = "{}/v2/secrets/".format(self._host)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
         response = RestClient(url).method(HttpMethod.POST).headers(
             headers).execute(payload=payload)
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
             err_msg = data.get('error')
@@ -444,15 +420,15 @@
         return munchify(data)
 
     def delete_secret(self, secret_name: str) -> Munch:
         """
         Delete a secret
         """
         url = "{}/v2/secrets/{}/".format(self._host, secret_name)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
         response = RestClient(url).method(HttpMethod.DELETE).headers(
             headers).execute()
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
             err_msg = data.get('error')
@@ -464,67 +440,255 @@
             self,
             query: dict = None
     ) -> Munch:
         """
         List all secrets in a project
         """
         url = "{}/v2/secrets/".format(self._host)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
 
         params = {}
         params.update(query or {})
 
-        offset, result = 0, []
-        while True:
-            params.update({
-                "continue": offset,
-                "limit": 50,
-            })
-            response = RestClient(url).method(HttpMethod.GET).query_param(
-                params).headers(headers).execute()
-            data = json.loads(response.text)
-            if not response.ok:
-                err_msg = data.get('error')
-                raise Exception("secrets: {}".format(err_msg))
-            secrets = data.get('items', [])
-            if not secrets:
-                break
-            offset = data['metadata']['continue']
-            for secret in secrets:
-                result.append(secret['metadata'])
-
-        return munchify(result)
+        client = RestClient(url).method(HttpMethod.GET).headers(headers)
+        return self._walk_pages(client, params=params)
 
     def get_secret(
             self,
             secret_name: str
     ) -> Munch:
         """
         Get secret by name
         """
         url = "{}/v2/secrets/{}/".format(self._host, secret_name)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
 
         response = RestClient(url).method(HttpMethod.GET).headers(headers).execute()
         data = json.loads(response.text)
         if not response.ok:
             err_msg = data.get('error')
             raise Exception("secrets: {}".format(err_msg))
 
         return munchify(data)
 
     def update_secret(self, secret_name: str, spec: dict) -> Munch:
         """
         Update a secret
         """
         url = "{}/v2/secrets/{}/".format(self._host, secret_name)
-        headers = self._config.get_auth_header()
+        headers = self._get_auth_header()
         response = RestClient(url).method(HttpMethod.PUT).headers(
             headers).execute(payload=spec)
         handle_server_errors(response)
 
         data = json.loads(response.text)
         if not response.ok:
             err_msg = data.get('error')
             raise Exception("secret: {}".format(err_msg))
 
         return munchify(data)
+
+    # ConfigTrees APIs
+    def list_config_trees(self) -> Munch:
+        url = "{}/v2/configtrees/".format(self._host)
+        headers = self._get_auth_header(with_org=True)
+        client = RestClient(url).method(HttpMethod.GET).headers(headers)
+        return self._walk_pages(client)
+
+    def create_config_tree(self, tree_spec: dict) -> Munch:
+        url = "{}/v2/configtrees/".format(self._host)
+        headers = self._get_auth_header(with_org=True)
+        response = RestClient(url).method(HttpMethod.POST).headers(
+            headers).execute(payload=tree_spec)
+        handle_server_errors(response)
+
+        data = json.loads(response.text)
+        if not response.ok:
+            err_msg = data.get('error')
+            raise Exception("configtree: {}".format(err_msg))
+
+        return munchify(data)
+
+    def delete_config_tree(self, tree_name: str) -> Munch:
+        url = "{}/v2/configtrees/{}/".format(self._host, tree_name)
+        headers = self._get_auth_header(with_org=True)
+        response = RestClient(url).method(HttpMethod.DELETE).headers(
+            headers).execute()
+        handle_server_errors(response)
+
+        data = json.loads(response.text)
+        if not response.ok:
+            err_msg = data.get('error')
+            raise Exception("configtree: {}".format(err_msg))
+
+        return munchify(data)
+
+    def get_config_tree(self, tree_name: str, rev_id: Optional[str] = None,
+                               include_data: bool = False, filter_content_types: Optional[List[str]] = None,
+                               filter_prefixes: Optional[List[str]] = None) -> Munch:
+        url = "{}/v2/configtrees/{}/".format(self._host, tree_name)
+        query = {
+            'includeData': include_data,
+            'contentTypes': filter_content_types,
+            'keyPrefixes': filter_prefixes,
+            'revision': rev_id,
+        }
+        headers = self._get_auth_header(with_org=True)
+        response = RestClient(url).method(HttpMethod.GET).headers(
+            headers).query_param(query).execute()
+        handle_server_errors(response)
+
+        data = json.loads(response.text)
+        if not response.ok:
+            err_msg = data.get('error')
+            raise Exception("configtree: {}".format(err_msg))
+
+        return munchify(data)
+
+    def set_revision_config_tree(self, tree_name: str, spec: dict) -> Munch:
+        url = "{}/v2/configtrees/{}/".format(self._host, tree_name)
+        headers = self._get_auth_header(with_org=True)
+        response = RestClient(url).method(HttpMethod.PUT).headers(
+            headers).execute(payload=spec)
+        handle_server_errors(response)
+
+        data = json.loads(response.text)
+        if not response.ok:
+            err_msg = data.get('error')
+            raise Exception("configtree: {}".format(err_msg))
+
+        return munchify(data)
+
+    def list_config_tree_revisions(self, tree_name: str) -> Munch:
+        url = "{}/v2/configtrees/{}/revisions/".format(self._host, tree_name)
+        headers = self._get_auth_header(with_org=True)
+        client = RestClient(url).method(HttpMethod.GET).headers(headers)
+        return self._walk_pages(client)
+
+    def initialize_config_tree_revision(self, tree_name: str) -> Munch:
+        url = "{}/v2/configtrees/{}/revisions/".format(self._host, tree_name)
+        headers = self._get_auth_header(with_org=True)
+        response = RestClient(url).method(HttpMethod.POST).headers(
+            headers).execute()
+        handle_server_errors(response)
+
+        data = json.loads(response.text)
+        if not response.ok:
+            err_msg = data.get('error')
+            raise Exception("configtree: {}".format(err_msg))
+
+        return munchify(data)
+
+    def commit_config_tree_revision(self, tree_name: str, rev_id: str, payload: dict) -> Munch:
+        url = "{}/v2/configtrees/{}/revisions/{}/".format(self._host, tree_name, rev_id)
+        headers = self._get_auth_header(with_org=True)
+        response = RestClient(url).method(HttpMethod.PATCH).headers(
+            headers).execute(payload=payload)
+        handle_server_errors(response)
+
+        data = json.loads(response.text)
+        if not response.ok:
+            err_msg = data.get('error')
+            raise Exception("configtree: {}".format(err_msg))
+
+        return munchify(data)
+
+    def store_keys_in_revision(self, tree_name: str, rev_id: str, payload: Any) -> Munch:
+        url = "{}/v2/configtrees/{}/revisions/{}/".format(self._host, tree_name, rev_id)
+        headers = self._get_auth_header(with_org=True)
+        response = RestClient(url).method(HttpMethod.PUT).headers(
+            headers).execute(payload=payload)
+        handle_server_errors(response)
+
+        data = json.loads(response.text)
+        if not response.ok:
+            err_msg = data.get('error')
+            raise Exception("configtree: {}".format(err_msg))
+
+        return munchify(data)
+
+
+    def store_key_in_revision(self, tree_name: str, rev_id: str, key: str, value: str, perms: int = 644) -> Munch:
+        url = "{}/v2/configtrees/{}/revisions/{}/{}".format(self._host, tree_name, rev_id, key)
+        headers = self._get_auth_header(with_org=True)
+        headers['Content-Type'] = 'kv'
+        headers['X-Checksum'] = md5(str(value).encode('utf-8')).hexdigest()
+        headers['X-Permissions'] = str(perms)
+
+        response = RestClient(url).method(HttpMethod.PUT).headers(
+            headers).execute(value)
+        handle_server_errors(response)
+
+        data = json.loads(response.text)
+        if not response.ok:
+            err_msg = data.get('error')
+            raise Exception("configtree: {}".format(err_msg))
+
+        return munchify(data)
+
+    def store_file_in_revision(self, tree_name: str, rev_id: str, key: str, file_path: str) -> Munch:
+        stat = os.stat(file_path)
+        perms = oct(stat.st_mode & 0o777)[-3:]
+
+        content_type = magic.from_file(file_path, mime=True)
+
+        url = "{}/v2/configtrees/{}/revisions/{}/{}".format(self._host, tree_name, rev_id, key)
+        headers = self._get_auth_header(with_org=True)
+        headers['Content-Type'] = content_type
+        headers['X-Permissions'] = perms
+
+        with open(file_path, 'rb') as f:
+            file_hash = md5()
+            chunk = f.read(8192)
+            while chunk:
+                file_hash.update(chunk)
+                chunk = f.read(8192)
+
+            headers['X-Checksum'] = file_hash.hexdigest()
+            f.seek(0)
+
+            response = RestClient(url).method(HttpMethod.PUT).headers(headers).execute(payload=f, raw=True)
+            handle_server_errors(response)
+
+        data = json.loads(response.text)
+        if not response.ok:
+            err_msg = data.get('error')
+            raise Exception("configtree: {}".format(err_msg))
+
+        return munchify(data)
+
+    def delete_key_in_revision(self, tree_name: str, rev_id: str, key: str) -> Munch:
+        url = "{}/v2/configtrees/{}/revisions/{}/{}".format(self._host, tree_name, rev_id, key)
+        headers = self._get_auth_header(with_org=True)
+        response = RestClient(url).method(HttpMethod.DELETE).headers(headers).execute()
+        handle_server_errors(response)
+
+        data = json.loads(response.text)
+        if not response.ok:
+            err_msg = data.get('error')
+            raise Exception("configtree: {}".format(err_msg))
+
+        return munchify(data)
+
+    def _walk_pages(self, c: RestClient, params: dict = {}, limit: Optional[int] = None) -> Munch:
+        offset, result = 0, []
+
+        if limit is not None:
+            params["limit"] = limit
+
+        while True:
+            params["continue"] = offset
+
+            response = c.query_param(params).execute()
+            data = json.loads(response.text)
+            if not response.ok:
+                err_msg = data.get('error')
+                raise Exception("listing: {}".format(err_msg))
+
+            items = data.get('items', [])
+            if not items:
+                break
+
+            offset = data['metadata']['continue']
+            result.extend(items)
+
+        return munchify(result)
```

### Comparing `rapyuta-io-cli-7.3.3/riocli/vpn/__init__.py` & `rapyuta-io-cli-7.4.0/riocli/vpn/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Copyright 2023 Rapyuta Robotics
+# Copyright 2024 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
@@ -12,14 +12,15 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 import click
 from click_help_colors import HelpColorsGroup
 
 from riocli.vpn.connect import connect
 from riocli.vpn.disconnect import disconnect
+from riocli.vpn.machines import machines
 from riocli.vpn.ping import ping_all
 from riocli.vpn.status import status
 
 
 @click.group(
     invoke_without_command=False,
     cls=HelpColorsGroup,
@@ -33,7 +34,8 @@
     pass
 
 
 vpn.add_command(connect)
 vpn.add_command(disconnect)
 vpn.add_command(status)
 vpn.add_command(ping_all)
+vpn.add_command(machines)
```

### Comparing `rapyuta-io-cli-7.3.3/riocli/vpn/connect.py` & `rapyuta-io-cli-7.4.0/riocli/vpn/connect.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,66 +1,66 @@
-# Copyright 2023 Rapyuta Robotics
+# Copyright 2024 Rapyuta Robotics
 #
 # Licensed under the Apache License, Version 2.0 (the "License");
 # you may not use this file except in compliance with the License.
 # You may obtain a copy of the License at
 #
 #     http://www.apache.org/licenses/LICENSE-2.0
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-import getpass
-import time
-from datetime import datetime, timedelta
 
+from datetime import timedelta
 import click
 from click_help_colors import HelpColorsCommand
-from munch import Munch
 from yaspin.api import Yaspin
 
-from riocli.config import new_v2_client
+from riocli.config import get_config_from_context
 from riocli.constants import Colors, Symbols
 from riocli.utils import run_bash_with_return_code
 from riocli.utils.spinner import with_spinner
-from riocli.v2client import Client as v2Client
 from riocli.vpn.util import (
-    get_command,
+    create_binding,
+    get_binding_labels,
     is_tailscale_up,
+    priviledged_command,
     stop_tailscale,
     install_vpn_tools,
-    get_host_name,
-    get_host_ip,
     is_vpn_enabled_in_project
 )
 
+_TAILSCALE_CMD_FORMAT = 'tailscale up --auth-key={} --login-server={} --reset --force-reauth ' \
+'--accept-routes --accept-dns --advertise-tags={} --timeout=30s'
+
 
 @click.command(
     'connect',
     cls=HelpColorsCommand,
     help_headers_color=Colors.YELLOW,
     help_options_color=Colors.GREEN,
 )
 @click.pass_context
 @with_spinner(text="Connecting...")
-def connect(ctx: click.Context, spinner: Yaspin = None):
+def connect(ctx: click.Context, spinner: Yaspin):
     """
     Connect to the current project's VPN network
     """
+    config = get_config_from_context(ctx)
+
     try:
         with spinner.hidden():
             install_vpn_tools()
 
-        client = new_v2_client()
+        client = config.new_v2_client()
 
-        if not is_vpn_enabled_in_project(
-                client, ctx.obj.data.get('project_id')):
+        if not is_vpn_enabled_in_project(client, config.project_guid):
             spinner.write(
                 click.style('{} VPN is not enabled in the project. '
                             'Please ask the organization or project '
                             'creator to enable VPN'.format(Symbols.WAITING),
                             fg=Colors.YELLOW))
             raise SystemExit(1)
 
@@ -82,15 +82,15 @@
 
         spinner.write(
             click.style(
                 '{} VPN is enabled in the project ({})'.format(
                     Symbols.INFO, ctx.obj.data.get('project_name')),
                 fg=Colors.CYAN))
 
-        if not start_tailscale(ctx, client, spinner):
+        if not start_tailscale(ctx, spinner):
             click.secho('{} Failed to connect to the project VPN'.format(
                 Symbols.ERROR), fg=Colors.RED)
             raise SystemExit(1)
 
         spinner.green.text = 'You are now connected to the project\'s VPN'
         spinner.green.ok(Symbols.SUCCESS)
     except click.exceptions.Abort as e:
@@ -99,74 +99,26 @@
         raise SystemExit(1) from e
     except Exception as e:
         spinner.red.text = str(e)
         spinner.red.fail(Symbols.ERROR)
         raise SystemExit(1) from e
 
 
-def start_tailscale(
-        ctx: click.Context,
-        client: v2Client,
-        spinner: Yaspin,
-) -> bool:
-    cmd = get_command('tailscale up --auth-key={} --login-server={} --reset --force-reauth '
-                      '--accept-routes --accept-dns --advertise-tags={} --timeout=30s')
-    args = generate_tailscale_args(ctx, client, spinner)
-    command = cmd.format(args.HEADSCALE_PRE_AUTH_KEY, args.HEADSCALE_URL, args.HEADSCALE_ACL_TAG)
+def start_tailscale(ctx: click.Context, spinner: Yaspin) -> bool:
+    spinner.text = 'Generating a token to join the network...'
+
+    binding = create_binding(ctx, delta=timedelta(minutes=10), labels=get_binding_labels())
+    cmd = _TAILSCALE_CMD_FORMAT.format(binding.HEADSCALE_PRE_AUTH_KEY, binding.HEADSCALE_URL, binding.HEADSCALE_ACL_TAG)
+    cmd = priviledged_command(cmd)
 
     with spinner.hidden():
-        output, code = run_bash_with_return_code(command)
+        _, code = run_bash_with_return_code(cmd)
 
     if code != 0:
         spinner.write(
             click.style('{} Failed to start vpn client'.format(Symbols.ERROR),
                         fg=Colors.RED))
         return False
 
     return True
 
 
-def generate_tailscale_args(
-        ctx: click.Context,
-        client: v2Client,
-        spinner: Yaspin,
-) -> Munch:
-    vpn_instance = 'rio-internal-headscale'
-    binding_name = '{}-{}'.format(ctx.obj.machine_id, int(time.time()))
-
-    body = {
-        'metadata': {
-            'name': binding_name,
-            'labels': {
-                'creator': 'riocli',
-                'hostname': get_host_name(),
-                'ip_address': str(get_host_ip()),
-                'username': getpass.getuser(),
-                'rapyuta.io/internal': 'true',
-            }
-        },
-        'spec': {
-            'instance': vpn_instance,
-            'provider': 'headscalevpn',
-            'config': {
-                'ephemeral': True,
-                'throwaway': True,
-                'expirationTime': get_key_expiry_time(),
-            }
-        }
-    }
-
-    spinner.text = 'Generating a token to join the network...'
-
-    try:
-        # We may end up creating multiple throwaway tokens in the database.
-        # But that's okay and something that we can live with
-        binding = client.create_instance_binding(vpn_instance, binding=body)
-        return binding.spec.environment
-    except Exception as e:
-        raise SystemExit(1) from e
-
-
-def get_key_expiry_time() -> str:
-    expiry = datetime.utcnow()
-    expiry = expiry + timedelta(minutes=10)
-    return expiry.isoformat('T') + 'Z'
```

### Comparing `rapyuta-io-cli-7.3.3/riocli/vpn/disconnect.py` & `rapyuta-io-cli-7.4.0/riocli/vpn/disconnect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/vpn/ping.py` & `rapyuta-io-cli-7.4.0/riocli/vpn/ping.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/riocli/vpn/status.py` & `rapyuta-io-cli-7.4.0/riocli/vpn/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.3/setup.py` & `rapyuta-io-cli-7.4.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -56,10 +56,14 @@
         "pyrfc3339>=1.1",
         "directory-tree>=0.0.3.1",
         "yaspin==2.5.0",
         "jsonschema==4.0.0",
         "waiting>=1.4.1",
         "semver>=3.0.0",
         "email-validator==2.0.0.post2",
+        "python-benedict>=0.33.2",
+        "etcd3gw>=2.4.0",
+        "graphviz>=0.20.3",
+        "python-magic>=0.4.27",
     ],
     setup_requires=["flake8"],
 )
```

