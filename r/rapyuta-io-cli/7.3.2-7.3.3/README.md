# Comparing `tmp/rapyuta-io-cli-7.3.2.tar.gz` & `tmp/rapyuta-io-cli-7.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rapyuta-io-cli-7.3.2.tar", last modified: Tue Mar 26 10:54:09 2024, max compression
+gzip compressed data, was "rapyuta-io-cli-7.3.3.tar", last modified: Wed Mar 27 05:51:19 2024, max compression
```

## Comparing `rapyuta-io-cli-7.3.2.tar` & `rapyuta-io-cli-7.3.3.tar`

### file list

```diff
@@ -1,210 +1,210 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.393727 rapyuta-io-cli-7.3.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-03-26 10:54:09.393727 rapyuta-io-cli-7.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.373727 rapyuta-io-cli-7.3.2/rapyuta_io_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-03-26 10:54:09.000000 rapyuta-io-cli-7.3.2/rapyuta_io_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-03-26 10:54:09.000000 rapyuta-io-cli-7.3.2/rapyuta_io_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-26 10:54:09.000000 rapyuta-io-cli-7.3.2/rapyuta_io_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-26 10:54:09.000000 rapyuta-io-cli-7.3.2/rapyuta_io_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-26 10:54:09.000000 rapyuta-io-cli-7.3.2/rapyuta_io_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-26 10:54:09.000000 rapyuta-io-cli-7.3.2/rapyuta_io_cli.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.373727 rapyuta-io-cli-7.3.2/riocli/
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.377727 rapyuta-io-cli-7.3.2/riocli/apply/
--rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/apply/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/apply/explain.py
--rw-r--r--   0 runner    (1001) docker     (127)    16534 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/apply/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/apply/resolver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/apply/template.py
--rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/apply/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.377727 rapyuta-io-cli-7.3.2/riocli/auth/
--rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/auth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/auth/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/auth/logout.py
--rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/auth/refresh_token.py
--rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/auth/staging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/auth/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/auth/token.py
--rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/auth/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/bootstrap.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.377727 rapyuta-io-cli-7.3.2/riocli/chart/
--rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/chart/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/chart/apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/chart/chart.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/chart/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/chart/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/chart/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/chart/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/chart/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.377727 rapyuta-io-cli-7.3.2/riocli/completion/
--rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/completion/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.377727 rapyuta-io-cli-7.3.2/riocli/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/config/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.377727 rapyuta-io-cli-7.3.2/riocli/constants/
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/constants/colors.py
--rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/constants/symbols.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.377727 rapyuta-io-cli-7.3.2/riocli/deployment/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/deployment/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/deployment/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/deployment/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/deployment/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/deployment/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/deployment/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/deployment/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)    18482 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/deployment/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/deployment/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/deployment/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/deployment/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/deployment/wait.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.381727 rapyuta-io-cli-7.3.2/riocli/device/
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/files.py
--rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/label.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/metric.py
--rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/onboard.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.381727 rapyuta-io-cli-7.3.2/riocli/device/tools/
--rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/tools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/tools/device_init.py
--rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/tools/forward.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/tools/rapyuta_logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/tools/scp.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/tools/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/tools/ssh.py
--rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/tools/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/topic.py
--rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/device/vpn.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.381727 rapyuta-io-cli-7.3.2/riocli/disk/
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/disk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/disk/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/disk/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/disk/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/disk/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/disk/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.381727 rapyuta-io-cli-7.3.2/riocli/exceptions/
--rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/exceptions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.381727 rapyuta-io-cli-7.3.2/riocli/jsonschema/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/jsonschema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/jsonschema/validate.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.381727 rapyuta-io-cli-7.3.2/riocli/managedservice/
--rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/managedservice/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/managedservice/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/managedservice/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/managedservice/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/managedservice/list_providers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/managedservice/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.385727 rapyuta-io-cli-7.3.2/riocli/model/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/model/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/model/base.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.385727 rapyuta-io-cli-7.3.2/riocli/network/
--rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/network/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/network/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/network/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/network/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/network/logs.py
--rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/network/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/network/native_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/network/routed_network.py
--rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/network/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.385727 rapyuta-io-cli-7.3.2/riocli/organization/
--rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/organization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/organization/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/organization/invite_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/organization/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/organization/remove_user.py
--rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/organization/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/organization/users.py
--rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/organization/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.385727 rapyuta-io-cli-7.3.2/riocli/package/
--rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/package/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/package/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/package/deployment.py
--rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/package/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/package/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/package/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/package/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.385727 rapyuta-io-cli-7.3.2/riocli/parameter/
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/parameter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/parameter/apply.py
--rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/parameter/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/parameter/diff.py
--rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/parameter/download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/parameter/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/parameter/upload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/parameter/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.389727 rapyuta-io-cli-7.3.2/riocli/project/
--rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/project/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/project/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/project/delete.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.389727 rapyuta-io-cli-7.3.2/riocli/project/features/
--rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/project/features/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/project/features/vpn.py
--rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/project/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/project/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/project/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/project/select.py
--rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/project/util.py
--rw-r--r--   0 runner    (1001) docker     (127)     3470 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/project/whoami.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.389727 rapyuta-io-cli-7.3.2/riocli/rosbag/
--rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/rosbag/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/rosbag/blob.py
--rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/rosbag/job.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/rosbag/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.389727 rapyuta-io-cli-7.3.2/riocli/secret/
--rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/secret/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/secret/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/secret/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/secret/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/secret/model.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.389727 rapyuta-io-cli-7.3.2/riocli/shell/
--rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/shell/prompt.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.389727 rapyuta-io-cli-7.3.2/riocli/static_route/
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/static_route/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/static_route/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/static_route/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/static_route/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/static_route/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/static_route/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/static_route/open.py
--rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/static_route/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.389727 rapyuta-io-cli-7.3.2/riocli/usergroup/
--rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/usergroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/usergroup/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/usergroup/inspect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/usergroup/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/usergroup/model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/usergroup/util.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.393727 rapyuta-io-cli-7.3.2/riocli/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/utils/cache.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/utils/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/utils/execute.py
--rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/utils/mermaid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/utils/selector.py
--rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/utils/spinner.py
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/utils/ssh_tunnel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.393727 rapyuta-io-cli-7.3.2/riocli/v2client/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/v2client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/v2client/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-26 10:54:09.393727 rapyuta-io-cli-7.3.2/riocli/vpn/
--rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/vpn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/vpn/connect.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/vpn/disconnect.py
--rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/vpn/ping.py
--rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/vpn/status.py
--rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/riocli/vpn/util.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-26 10:54:09.393727 rapyuta-io-cli-7.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-26 10:54:01.000000 rapyuta-io-cli-7.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.606536 rapyuta-io-cli-7.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-03-27 05:51:19.606536 rapyuta-io-cli-7.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2453 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.586536 rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3522 2024-03-27 05:51:19.000000 rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4622 2024-03-27 05:51:19.000000 rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-27 05:51:19.000000 rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-03-27 05:51:19.000000 rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-03-27 05:51:19.000000 rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-27 05:51:19.000000 rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.586536 rapyuta-io-cli-7.3.3/riocli/
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      675 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.586536 rapyuta-io-cli-7.3.3/riocli/apply/
+-rw-r--r--   0 runner    (1001) docker     (127)     5060 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/apply/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/apply/explain.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16534 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/apply/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8444 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/apply/resolver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/apply/template.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1969 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/apply/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.590536 rapyuta-io-cli-7.3.3/riocli/auth/
+-rw-r--r--   0 runner    (1001) docker     (127)     1432 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4557 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/logout.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1409 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/refresh_token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3460 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/staging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1140 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1891 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5573 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/auth/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3996 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/bootstrap.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.590536 rapyuta-io-cli-7.3.3/riocli/chart/
+-rw-r--r--   0 runner    (1001) docker     (127)     1341 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2796 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/chart.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1374 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1637 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/chart/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.590536 rapyuta-io-cli-7.3.3/riocli/completion/
+-rw-r--r--   0 runner    (1001) docker     (127)     1361 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/completion/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.590536 rapyuta-io-cli-7.3.3/riocli/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4676 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/config/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.590536 rapyuta-io-cli-7.3.3/riocli/constants/
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/constants/colors.py
+-rw-r--r--   0 runner    (1001) docker     (127)      697 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/constants/symbols.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.590536 rapyuta-io-cli-7.3.3/riocli/deployment/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4315 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10299 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2162 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3086 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2801 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2786 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18482 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1311 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5702 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7040 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2417 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/deployment/wait.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.594536 rapyuta-io-cli-7.3.3/riocli/device/
+-rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5698 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2837 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5495 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1747 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8382 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/files.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1783 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4159 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/label.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3301 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/metric.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2718 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1268 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/onboard.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.594536 rapyuta-io-cli-7.3.3/riocli/device/tools/
+-rw-r--r--   0 runner    (1001) docker     (127)     1313 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3129 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/device_init.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1824 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/forward.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/rapyuta_logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2356 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/scp.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4050 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/ssh.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2692 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/tools/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3736 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/topic.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4585 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4437 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/device/vpn.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.594536 rapyuta-io-cli-7.3.3/riocli/disk/
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/disk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/disk/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1898 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/disk/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/disk/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3142 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/disk/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3527 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/disk/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.594536 rapyuta-io-cli-7.3.3/riocli/exceptions/
+-rw-r--r--   0 runner    (1001) docker     (127)      892 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/exceptions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.594536 rapyuta-io-cli-7.3.3/riocli/jsonschema/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/jsonschema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1841 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/jsonschema/validate.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.594536 rapyuta-io-cli-7.3.3/riocli/managedservice/
+-rw-r--r--   0 runner    (1001) docker     (127)     1427 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/managedservice/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/managedservice/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1287 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/managedservice/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/managedservice/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/managedservice/list_providers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2022 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/managedservice/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.594536 rapyuta-io-cli-7.3.3/riocli/model/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/model/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6887 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/model/base.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.598536 rapyuta-io-cli-7.3.3/riocli/network/
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2169 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2471 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1739 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2638 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/logs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4481 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/native_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3273 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/routed_network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6455 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/network/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.598536 rapyuta-io-cli-7.3.3/riocli/organization/
+-rw-r--r--   0 runner    (1001) docker     (127)     1503 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/invite_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1935 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1774 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/remove_user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2401 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1956 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/users.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2087 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/organization/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.598536 rapyuta-io-cli-7.3.3/riocli/package/
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/package/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/package/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/package/deployment.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2294 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/package/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/package/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9264 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/package/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3241 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/package/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.598536 rapyuta-io-cli-7.3.3/riocli/parameter/
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4907 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/apply.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2150 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4054 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/diff.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2802 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1226 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2987 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/upload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3538 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/parameter/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.598536 rapyuta-io-cli-7.3.3/riocli/project/
+-rw-r--r--   0 runner    (1001) docker     (127)     1442 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2254 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/delete.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.598536 rapyuta-io-cli-7.3.3/riocli/project/features/
+-rw-r--r--   0 runner    (1001) docker     (127)      974 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2823 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/features/vpn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1591 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3039 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1520 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/select.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4541 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3441 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/project/whoami.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.602536 rapyuta-io-cli-7.3.3/riocli/rosbag/
+-rw-r--r--   0 runner    (1001) docker     (127)     1019 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/rosbag/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4323 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/rosbag/blob.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11554 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/rosbag/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/rosbag/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.602536 rapyuta-io-cli-7.3.3/riocli/secret/
+-rw-r--r--   0 runner    (1001) docker     (127)     1176 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/secret/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1803 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/secret/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1456 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/secret/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1700 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/secret/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2189 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/secret/model.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.602536 rapyuta-io-cli-7.3.3/riocli/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)     2040 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      831 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/shell/prompt.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.602536 rapyuta-io-cli-7.3.3/riocli/static_route/
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1651 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1842 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1516 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2266 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1273 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/open.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1024 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/static_route/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.602536 rapyuta-io-cli-7.3.3/riocli/usergroup/
+-rw-r--r--   0 runner    (1001) docker     (127)     1193 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/usergroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/usergroup/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/usergroup/inspect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1877 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/usergroup/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6445 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/usergroup/model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2486 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/usergroup/util.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.602536 rapyuta-io-cli-7.3.3/riocli/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     7444 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1215 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/cache.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4548 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/execute.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1312 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/mermaid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/selector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2451 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/spinner.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/utils/ssh_tunnel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.602536 rapyuta-io-cli-7.3.3/riocli/v2client/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/v2client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17367 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/v2client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-27 05:51:19.606536 rapyuta-io-cli-7.3.3/riocli/vpn/
+-rw-r--r--   0 runner    (1001) docker     (127)     1151 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/vpn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5746 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/vpn/connect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/vpn/disconnect.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2237 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/vpn/ping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3380 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/vpn/status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3918 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/riocli/vpn/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-27 05:51:19.606536 rapyuta-io-cli-7.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1759 2024-03-27 05:51:10.000000 rapyuta-io-cli-7.3.3/setup.py
```

### Comparing `rapyuta-io-cli-7.3.2/PKG-INFO` & `rapyuta-io-cli-7.3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 7.3.2
+Version: 7.3.3
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: UNKNOWN
 Description: # Rapyuta CLI
```

### Comparing `rapyuta-io-cli-7.3.2/README.md` & `rapyuta-io-cli-7.3.3/README.md`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/rapyuta_io_cli.egg-info/PKG-INFO` & `rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rapyuta-io-cli
-Version: 7.3.2
+Version: 7.3.3
 Summary: Rapyuta.io CLI Python command line application.
 Home-page: http://docs.rapyuta.io
 Author: Rapyuta Robotics
 Author-email: opensource@rapyuta-robotics.com
 License: UNKNOWN
 Description: # Rapyuta CLI
```

### Comparing `rapyuta-io-cli-7.3.2/rapyuta_io_cli.egg-info/SOURCES.txt` & `rapyuta-io-cli-7.3.3/rapyuta_io_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/__main__.py` & `rapyuta-io-cli-7.3.3/riocli/__main__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/apply/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/apply/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/apply/explain.py` & `rapyuta-io-cli-7.3.3/riocli/apply/explain.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/apply/parse.py` & `rapyuta-io-cli-7.3.3/riocli/apply/parse.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/apply/resolver.py` & `rapyuta-io-cli-7.3.3/riocli/apply/resolver.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/apply/template.py` & `rapyuta-io-cli-7.3.3/riocli/apply/template.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/apply/util.py` & `rapyuta-io-cli-7.3.3/riocli/apply/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/auth/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/auth/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/auth/login.py` & `rapyuta-io-cli-7.3.3/riocli/auth/login.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/auth/logout.py` & `rapyuta-io-cli-7.3.3/riocli/auth/logout.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/auth/refresh_token.py` & `rapyuta-io-cli-7.3.3/riocli/auth/refresh_token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/auth/staging.py` & `rapyuta-io-cli-7.3.3/riocli/auth/staging.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/auth/status.py` & `rapyuta-io-cli-7.3.3/riocli/auth/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/auth/token.py` & `rapyuta-io-cli-7.3.3/riocli/auth/token.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/auth/util.py` & `rapyuta-io-cli-7.3.3/riocli/auth/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/bootstrap.py` & `rapyuta-io-cli-7.3.3/riocli/bootstrap.py`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 #
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
-__version__ = "7.3.2"
+__version__ = "7.3.3"
 
 import click
 import rapyuta_io.version
 from click import Context
 from click_help_colors import HelpColorsGroup
 from click_plugins import with_plugins
 from pkg_resources import iter_entry_points
```

### Comparing `rapyuta-io-cli-7.3.2/riocli/chart/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/chart/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/chart/apply.py` & `rapyuta-io-cli-7.3.3/riocli/chart/apply.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/chart/chart.py` & `rapyuta-io-cli-7.3.3/riocli/chart/chart.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/chart/delete.py` & `rapyuta-io-cli-7.3.3/riocli/chart/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/chart/info.py` & `rapyuta-io-cli-7.3.3/riocli/chart/info.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/chart/list.py` & `rapyuta-io-cli-7.3.3/riocli/chart/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/chart/search.py` & `rapyuta-io-cli-7.3.3/riocli/chart/search.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/chart/util.py` & `rapyuta-io-cli-7.3.3/riocli/chart/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/completion/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/completion/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/config/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/config/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/config/config.py` & `rapyuta-io-cli-7.3.3/riocli/config/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/constants/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/constants/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/constants/colors.py` & `rapyuta-io-cli-7.3.3/riocli/constants/colors.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/constants/symbols.py` & `rapyuta-io-cli-7.3.3/riocli/constants/symbols.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/deployment/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/deployment/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/deployment/delete.py` & `rapyuta-io-cli-7.3.3/riocli/deployment/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/deployment/errors.py` & `rapyuta-io-cli-7.3.3/riocli/deployment/errors.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/deployment/execute.py` & `rapyuta-io-cli-7.3.3/riocli/deployment/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/deployment/inspect.py` & `rapyuta-io-cli-7.3.3/riocli/deployment/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/deployment/list.py` & `rapyuta-io-cli-7.3.3/riocli/deployment/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/deployment/logs.py` & `rapyuta-io-cli-7.3.3/riocli/deployment/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/deployment/model.py` & `rapyuta-io-cli-7.3.3/riocli/deployment/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/deployment/status.py` & `rapyuta-io-cli-7.3.3/riocli/deployment/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/deployment/update.py` & `rapyuta-io-cli-7.3.3/riocli/deployment/update.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/deployment/util.py` & `rapyuta-io-cli-7.3.3/riocli/deployment/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/deployment/wait.py` & `rapyuta-io-cli-7.3.3/riocli/deployment/wait.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/device/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/config.py` & `rapyuta-io-cli-7.3.3/riocli/device/config.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/create.py` & `rapyuta-io-cli-7.3.3/riocli/device/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/delete.py` & `rapyuta-io-cli-7.3.3/riocli/device/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/deployment.py` & `rapyuta-io-cli-7.3.3/riocli/device/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/execute.py` & `rapyuta-io-cli-7.3.3/riocli/device/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/files.py` & `rapyuta-io-cli-7.3.3/riocli/device/files.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/inspect.py` & `rapyuta-io-cli-7.3.3/riocli/device/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/label.py` & `rapyuta-io-cli-7.3.3/riocli/device/label.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/list.py` & `rapyuta-io-cli-7.3.3/riocli/device/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/metric.py` & `rapyuta-io-cli-7.3.3/riocli/device/metric.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/model.py` & `rapyuta-io-cli-7.3.3/riocli/device/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/onboard.py` & `rapyuta-io-cli-7.3.3/riocli/device/onboard.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/tools/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/device/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/tools/device_init.py` & `rapyuta-io-cli-7.3.3/riocli/device/tools/device_init.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/tools/forward.py` & `rapyuta-io-cli-7.3.3/riocli/device/tools/forward.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/tools/rapyuta_logs.py` & `rapyuta-io-cli-7.3.3/riocli/device/tools/rapyuta_logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/tools/scp.py` & `rapyuta-io-cli-7.3.3/riocli/device/tools/scp.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/tools/service.py` & `rapyuta-io-cli-7.3.3/riocli/device/tools/service.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/tools/ssh.py` & `rapyuta-io-cli-7.3.3/riocli/device/tools/ssh.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/tools/util.py` & `rapyuta-io-cli-7.3.3/riocli/device/tools/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/topic.py` & `rapyuta-io-cli-7.3.3/riocli/device/topic.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/util.py` & `rapyuta-io-cli-7.3.3/riocli/device/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/device/vpn.py` & `rapyuta-io-cli-7.3.3/riocli/device/vpn.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/disk/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/disk/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/disk/create.py` & `rapyuta-io-cli-7.3.3/riocli/disk/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/disk/delete.py` & `rapyuta-io-cli-7.3.3/riocli/disk/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/disk/list.py` & `rapyuta-io-cli-7.3.3/riocli/disk/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/disk/model.py` & `rapyuta-io-cli-7.3.3/riocli/disk/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/disk/util.py` & `rapyuta-io-cli-7.3.3/riocli/disk/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/exceptions/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/exceptions/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/jsonschema/validate.py` & `rapyuta-io-cli-7.3.3/riocli/jsonschema/validate.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/managedservice/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/managedservice/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/managedservice/delete.py` & `rapyuta-io-cli-7.3.3/riocli/managedservice/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/managedservice/inspect.py` & `rapyuta-io-cli-7.3.3/riocli/managedservice/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/managedservice/list.py` & `rapyuta-io-cli-7.3.3/riocli/managedservice/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/managedservice/list_providers.py` & `rapyuta-io-cli-7.3.3/riocli/managedservice/list_providers.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/managedservice/model.py` & `rapyuta-io-cli-7.3.3/riocli/managedservice/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/model/base.py` & `rapyuta-io-cli-7.3.3/riocli/model/base.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/network/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/network/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/network/create.py` & `rapyuta-io-cli-7.3.3/riocli/network/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/network/delete.py` & `rapyuta-io-cli-7.3.3/riocli/network/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/network/inspect.py` & `rapyuta-io-cli-7.3.3/riocli/network/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/network/list.py` & `rapyuta-io-cli-7.3.3/riocli/network/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/network/logs.py` & `rapyuta-io-cli-7.3.3/riocli/network/logs.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/network/model.py` & `rapyuta-io-cli-7.3.3/riocli/network/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/network/native_network.py` & `rapyuta-io-cli-7.3.3/riocli/network/native_network.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/network/routed_network.py` & `rapyuta-io-cli-7.3.3/riocli/network/routed_network.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/network/util.py` & `rapyuta-io-cli-7.3.3/riocli/network/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/organization/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/organization/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/organization/inspect.py` & `rapyuta-io-cli-7.3.3/riocli/organization/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/organization/invite_user.py` & `rapyuta-io-cli-7.3.3/riocli/organization/invite_user.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/organization/list.py` & `rapyuta-io-cli-7.3.3/riocli/organization/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/organization/remove_user.py` & `rapyuta-io-cli-7.3.3/riocli/organization/remove_user.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/organization/select.py` & `rapyuta-io-cli-7.3.3/riocli/organization/select.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/organization/users.py` & `rapyuta-io-cli-7.3.3/riocli/organization/users.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/organization/utils.py` & `rapyuta-io-cli-7.3.3/riocli/organization/utils.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/package/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/package/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/package/delete.py` & `rapyuta-io-cli-7.3.3/riocli/package/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/package/deployment.py` & `rapyuta-io-cli-7.3.3/riocli/package/deployment.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/package/inspect.py` & `rapyuta-io-cli-7.3.3/riocli/package/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/package/list.py` & `rapyuta-io-cli-7.3.3/riocli/package/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/package/model.py` & `rapyuta-io-cli-7.3.3/riocli/package/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/package/util.py` & `rapyuta-io-cli-7.3.3/riocli/package/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/parameter/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/parameter/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/parameter/apply.py` & `rapyuta-io-cli-7.3.3/riocli/parameter/apply.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/parameter/delete.py` & `rapyuta-io-cli-7.3.3/riocli/parameter/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/parameter/diff.py` & `rapyuta-io-cli-7.3.3/riocli/parameter/diff.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/parameter/download.py` & `rapyuta-io-cli-7.3.3/riocli/parameter/download.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/parameter/list.py` & `rapyuta-io-cli-7.3.3/riocli/parameter/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/parameter/upload.py` & `rapyuta-io-cli-7.3.3/riocli/parameter/upload.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/parameter/utils.py` & `rapyuta-io-cli-7.3.3/riocli/parameter/utils.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/project/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/project/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/project/create.py` & `rapyuta-io-cli-7.3.3/riocli/project/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/project/delete.py` & `rapyuta-io-cli-7.3.3/riocli/project/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/project/features/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/project/features/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/project/features/vpn.py` & `rapyuta-io-cli-7.3.3/riocli/project/features/vpn.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/project/inspect.py` & `rapyuta-io-cli-7.3.3/riocli/project/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/project/list.py` & `rapyuta-io-cli-7.3.3/riocli/project/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/project/model.py` & `rapyuta-io-cli-7.3.3/riocli/project/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/project/select.py` & `rapyuta-io-cli-7.3.3/riocli/project/select.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/project/util.py` & `rapyuta-io-cli-7.3.3/riocli/project/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/project/whoami.py` & `rapyuta-io-cli-7.3.3/riocli/project/whoami.py`

 * *Files 2% similar despite different names*

```diff
@@ -101,17 +101,16 @@
 
     for group in project.spec.get('userGroups', []):
         if group['name'] not in user_groups:
             continue
 
         # If the user is part of a group that has admin access then no
         # need to check further.
-        if role and (role != ADMIN_ROLE and group['role'] == ADMIN_ROLE):
-            role = ADMIN_ROLE
-            break
+        if role != ADMIN_ROLE and group['role'] == ADMIN_ROLE:
+            return ADMIN_ROLE
 
         role = group['role']
 
     if not role:
         raise Exception('User does not have access to the project')
 
     return role
```

### Comparing `rapyuta-io-cli-7.3.2/riocli/rosbag/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/rosbag/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/rosbag/blob.py` & `rapyuta-io-cli-7.3.3/riocli/rosbag/blob.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/rosbag/job.py` & `rapyuta-io-cli-7.3.3/riocli/rosbag/job.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/secret/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/secret/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/secret/delete.py` & `rapyuta-io-cli-7.3.3/riocli/secret/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/secret/inspect.py` & `rapyuta-io-cli-7.3.3/riocli/secret/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/secret/list.py` & `rapyuta-io-cli-7.3.3/riocli/secret/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/secret/model.py` & `rapyuta-io-cli-7.3.3/riocli/secret/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/shell/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/shell/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/shell/prompt.py` & `rapyuta-io-cli-7.3.3/riocli/shell/prompt.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/static_route/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/static_route/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/static_route/create.py` & `rapyuta-io-cli-7.3.3/riocli/static_route/create.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/static_route/delete.py` & `rapyuta-io-cli-7.3.3/riocli/static_route/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/static_route/inspect.py` & `rapyuta-io-cli-7.3.3/riocli/static_route/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/static_route/list.py` & `rapyuta-io-cli-7.3.3/riocli/static_route/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/static_route/model.py` & `rapyuta-io-cli-7.3.3/riocli/static_route/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/static_route/open.py` & `rapyuta-io-cli-7.3.3/riocli/static_route/open.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/static_route/util.py` & `rapyuta-io-cli-7.3.3/riocli/static_route/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/usergroup/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/usergroup/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/usergroup/delete.py` & `rapyuta-io-cli-7.3.3/riocli/usergroup/delete.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/usergroup/inspect.py` & `rapyuta-io-cli-7.3.3/riocli/usergroup/inspect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/usergroup/list.py` & `rapyuta-io-cli-7.3.3/riocli/usergroup/list.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/usergroup/model.py` & `rapyuta-io-cli-7.3.3/riocli/usergroup/model.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/usergroup/util.py` & `rapyuta-io-cli-7.3.3/riocli/usergroup/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/utils/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/utils/cache.py` & `rapyuta-io-cli-7.3.3/riocli/utils/cache.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/utils/context.py` & `rapyuta-io-cli-7.3.3/riocli/utils/context.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/utils/execute.py` & `rapyuta-io-cli-7.3.3/riocli/utils/execute.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/utils/mermaid.py` & `rapyuta-io-cli-7.3.3/riocli/utils/mermaid.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/utils/selector.py` & `rapyuta-io-cli-7.3.3/riocli/utils/selector.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/utils/spinner.py` & `rapyuta-io-cli-7.3.3/riocli/utils/spinner.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/utils/ssh_tunnel.py` & `rapyuta-io-cli-7.3.3/riocli/utils/ssh_tunnel.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/v2client/client.py` & `rapyuta-io-cli-7.3.3/riocli/v2client/client.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/vpn/__init__.py` & `rapyuta-io-cli-7.3.3/riocli/vpn/__init__.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/vpn/connect.py` & `rapyuta-io-cli-7.3.3/riocli/vpn/connect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/vpn/disconnect.py` & `rapyuta-io-cli-7.3.3/riocli/vpn/disconnect.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/vpn/ping.py` & `rapyuta-io-cli-7.3.3/riocli/vpn/ping.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/vpn/status.py` & `rapyuta-io-cli-7.3.3/riocli/vpn/status.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/riocli/vpn/util.py` & `rapyuta-io-cli-7.3.3/riocli/vpn/util.py`

 * *Files identical despite different names*

### Comparing `rapyuta-io-cli-7.3.2/setup.py` & `rapyuta-io-cli-7.3.3/setup.py`

 * *Files identical despite different names*

