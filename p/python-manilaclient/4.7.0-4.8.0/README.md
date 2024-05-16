# Comparing `tmp/python-manilaclient-4.7.0.tar.gz` & `tmp/python-manilaclient-4.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-manilaclient-4.7.0.tar", last modified: Mon Nov 20 07:06:08 2023, max compression
+gzip compressed data, was "python-manilaclient-4.8.0.tar", last modified: Fri Mar  1 09:55:55 2024, max compression
```

## Comparing `python-manilaclient-4.7.0.tar` & `python-manilaclient-4.8.0.tar`

### file list

```diff
@@ -1,473 +1,477 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.849259 python-manilaclient-4.7.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7143 2023-11-20 07:06:08.000000 python-manilaclient-4.7.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    33121 2023-11-20 07:06:08.000000 python-manilaclient-4.7.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2275 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/HACKING
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11837 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5859 2023-11-20 07:06:08.849259 python-manilaclient-4.7.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4088 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.773262 python-manilaclient-4.7.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/doc/.gitignore
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/doc/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.773262 python-manilaclient-4.7.0/doc/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.777262 python-manilaclient-4.7.0/doc/source/cli/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/doc/source/cli/decoder.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.777262 python-manilaclient-4.7.0/doc/source/cli/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13353 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/doc/source/cli/osc/manila.csv
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.777262 python-manilaclient-4.7.0/doc/source/cli/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4537 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/doc/source/cli/osc/v2/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/doc/source/cli/osc_plugin_cli.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.777262 python-manilaclient-4.7.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/doc/source/contributor/contributing.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8806 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/doc/source/contributor/functional-tests.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1523 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.777262 python-manilaclient-4.7.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/doc/source/user/api.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/doc/source/user/shell.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.769262 python-manilaclient-4.7.0/etc/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.777262 python-manilaclient-4.7.0/etc/manilaclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/etc/manilaclient/README.manilaclient.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.777262 python-manilaclient-4.7.0/etc/oslo-config-generator/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/etc/oslo-config-generator/manilaclient.conf
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.777262 python-manilaclient-4.7.0/manilaclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1248 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15186 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/api_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18336 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.781262 python-manilaclient-4.7.0/manilaclient/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/common/_i18n.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.781262 python-manilaclient-4.7.0/manilaclient/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12887 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/common/apiclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/common/apiclient/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8150 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/common/cliutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4098 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/common/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7277 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/common/httpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10524 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/config.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/extension.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.781262 python-manilaclient-4.7.0/manilaclient/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4367 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/plugin.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.785261 python-manilaclient-4.7.0/manilaclient/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/availability_zones.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.785261 python-manilaclient-4.7.0/manilaclient/osc/v2/data/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13353 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/data/manila.csv
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6631 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14775 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14033 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/resource_locks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20321 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4321 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    53039 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17889 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14055 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14824 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6315 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11713 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18730 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7645 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2202 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13048 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27777 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2831 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14367 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23898 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3244 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5018 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30280 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9165 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_transfers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16122 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/osc/v2/share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    32358 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.785261 python-manilaclient-4.7.0/manilaclient/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.793261 python-manilaclient-4.7.0/manilaclient/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21493 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    90065 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2322 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.797261 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17506 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      980 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4110 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7052 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_resource_locks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9286 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5178 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3533 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1418 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3896 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2618 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2264 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7773 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3541 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_transfers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8626 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6111 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_shares_group_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2146 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6668 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2755 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13085 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2727 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13367 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4622 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    23687 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4371 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14265 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4050 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_transfers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20496 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11999 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14916 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_shares_listing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5391 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_shares_metadata.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7615 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_snapshot_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4968 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4634 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3584 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/test_snapshots_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4955 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/functional/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.797261 python-manilaclient-4.7.0/manilaclient/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.797261 python-manilaclient-4.7.0/manilaclient/tests/unit/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/common/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.797261 python-manilaclient-4.7.0/manilaclient/tests/unit/common/apiclient/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/common/apiclient/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8145 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/common/test_httpclient.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2919 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/fakes.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.797261 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6610 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/osc_fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2555 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/osc_utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.805261 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    51641 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6194 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15984 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10236 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_resource_locks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22375 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6858 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    67767 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20521 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13644 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21560 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17697 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6874 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24594 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5208 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12339 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3044 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16353 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    27426 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5395 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_pools.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3996 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    22544 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24995 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5687 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8248 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    44426 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8938 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_transfers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20743 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_type.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6357 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14907 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/test_api_versions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2734 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/test_base.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5305 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7759 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/test_functional_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17744 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3104 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.805261 python-manilaclient-4.7.0/manilaclient/tests/unit/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1206 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1239 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1192 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_shares.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.813261 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6889 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/fake_clients.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    47272 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/fakes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2129 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13669 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_client.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5456 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4375 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2780 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12085 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2962 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8545 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3758 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3604 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9947 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7915 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11617 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2142 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4436 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11773 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1894 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5851 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11823 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1653 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3612 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9976 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_transfers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    30414 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   157650 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3595 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18918 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/utils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.813261 python-manilaclient-4.7.0/manilaclient/v1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10490 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.817261 python-manilaclient-4.7.0/manilaclient/v1/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1253 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/contrib/list_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v1/shares.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.821260 python-manilaclient-4.7.0/manilaclient/v2/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/availability_zones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13178 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/client.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.821260 python-manilaclient-4.7.0/manilaclient/v2/contrib/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/contrib/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1448 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/contrib/list_extensions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2873 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/limits.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6071 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/quota_classes.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11053 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/quotas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4713 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/resource_locks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/scheduler_stats.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9732 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/security_services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3357 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/services.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2994 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_access_rules.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4832 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_backups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9326 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_group_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3695 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_group_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7367 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_group_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11213 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_groups.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4228 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5217 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_network_subnets.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13094 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_networks.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2943 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_replica_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11234 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_replicas.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10761 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_servers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_snapshot_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_snapshot_instance_export_locations.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2700 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_snapshot_instances.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9276 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_snapshots.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4526 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_transfers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_type_access.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10307 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/share_types.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    31781 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/shares.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   225607 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/manilaclient/v2/shell.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.821260 python-manilaclient-4.7.0/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/playbooks/enable-fips.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.821260 python-manilaclient-4.7.0/playbooks/python-manilaclient-functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/playbooks/python-manilaclient-functional/post.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/playbooks/python-manilaclient-functional/run.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.825260 python-manilaclient-4.7.0/python_manilaclient.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5859 2023-11-20 07:06:08.000000 python-manilaclient-4.7.0/python_manilaclient.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    21790 2023-11-20 07:06:08.000000 python-manilaclient-4.7.0/python_manilaclient.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-11-20 07:06:08.000000 python-manilaclient-4.7.0/python_manilaclient.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11626 2023-11-20 07:06:08.000000 python-manilaclient-4.7.0/python_manilaclient.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-11-20 07:06:08.000000 python-manilaclient-4.7.0/python_manilaclient.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2023-11-20 07:06:08.000000 python-manilaclient-4.7.0/python_manilaclient.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2023-11-20 07:06:08.000000 python-manilaclient-4.7.0/python_manilaclient.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2023-11-20 07:06:08.000000 python-manilaclient-4.7.0/python_manilaclient.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.825260 python-manilaclient-4.7.0/rally-jobs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1890 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/rally-jobs/rally-manila-no-ss.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/rally-jobs/rally-manila.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.769262 python-manilaclient-4.7.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.845260 python-manilaclient-4.7.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/Bug-1990013-fix-share-grou-from-snapshot-create-fa3629cf1417ba20.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-access-visibility-and-deletion-locks-69978f052e25334c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-count-info-in-share-21a6b36c0f4c87b2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-count-info-in-snapshot-c9600adad648a486.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-dash-dash-help-subcomand-ad4226454aa07bc6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-defaultadsite-to-security-service-33fd0a5d1b865b11.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-export-location-filter-4cf3114doe40k598.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-ipv6-access-type-4dko90r1a9a1e0b8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-like-filter-591572762357ef4b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-message-list-and-delete-41b3323edd63d894.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-metadata-for-share-access-rule-11a6b36c0f4c87c2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-per-share-gigabytes-quotas-40bc404bd3cbdd89.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-query-params-pools-list-api-12cf1s14ddf40kdd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-quiesce-wait-time-for-replica-promote-30d9fa66afc854f2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-quota-per-share-type-support-3b2708ea232e69bc.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-scheduler-hints-to-share-create-70d429cb0aaf8f11.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-scheduler-hints-to-share-replica-create-d152a3934e5ad3a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-share-group-quotas-support-b6563cec58209a1d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-share-group-support-a3166f6ca4d06a81.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-share-replicas-and-replica-gigabytes-quotas-909436c2b2420f2c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-snapshot-instances-admin-api-3cf3114doe40k598.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-snapshot-metadata-49b0288bf2f12bf0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-subnet-metadata-82426986431b0179.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-support-filter-search-for-share-type-fdbaaa9510cc59dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add-support-to-check-quota-usage-scfdg14dod40k71a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/add_support_multiple_subnet_per_az-46145c3e90e097be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bp-allow-locking-shares-against-deletion-89e51e27368cda46.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bp-export-locations-replica-az-commands-03aa32c08f59c42d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bp-integrate-os-profiler-4818066dc2fbf7b7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bp-ocata-migration-improvements-f63c5d233856fbee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bp-support-group-spec-search-share-group-type-api-d5d9a6096f084b91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bp-support-query-user-messages-by-timestamp-34b70bba2d1b4d13.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bp-support-share-transfer-between-project-faefead551380eca.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bp-update-share-type-name-or-description-32d98b5a42cd8090.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1558995-fix-endpoint-not-found.yaml-a06a3b0ba5006718.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1608664-add-support-columns-share-replica-list-885bd8c8b4bfa8f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1611506-allow-deletion-multiple-resources
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1622540-add-missing-az-list-command-f90265de5c2f261b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1650774-share-instance-reset-state-9c4b26f44b5da0e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1664877-c462bfad92ce03e5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1674915-allow-user-access-fix-495b3e42bdc985ec.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1682726-remove-sort-key-export-location-from-list-885des26bd5ea2de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1707303-fix-list-command-when-not-given-search-opts-c06af7b344e9cb91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1709746-add-group-specs-in-share-group-type-create-command-f91265de5c2f251b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1717940-dash-dash-column-reports-nothing-for-capabilities-db8c1234fae91af5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1724183-add-share-type-description-8c4b26f44b5da1e9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1733494-allow-user-group-name-with-blank-access-fix-885a3e42bdc985ec.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      118 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1738917-and-1738918-fix-access-share-group-type-by-name-3a8760522c147f28.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1798229-fix-create-share-from-snap-using-name-44100b907ea6a040.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1799934-add-ou-parameter-260f9aaf939d1919.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1802059-fix-is_default-a8d3d95ffa0aede9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1811516-bug-1811627-python3-fixes-4b26130027b2c076.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1814094-fix-_get_base_url-method-168e12292aeec8f1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1830677-fix-13b30d6a89f43246.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1855391-support-force-extend-share-6b5ebcfe1de0ca7b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1871252-update-default-quotas-via-quota-class-share-groups-share-group-snapshots-20ec1dfcc0a7e81c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1898304-add-wait-to-share-create-delete-f121073f2f4402ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1898308-add-wait-to-share-extend-shrink-c9cc413c50d9832a.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1898309-add-wait-to-share-manage-unmanage-d2060c61cc295bfd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1898315-add-wait-flag-to-manage-share-server-operation-be6488c2a57536e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1898316-add-wait-option-for-deleting-a-share-server-e2228018585de5cb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1898317-add-wait-option-for-force-deleting-share-snapshot-share-instance-fb2531b6033f0ae5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1898318-add-wait-flag-for-deleting-a-share-group-operation-c602ba9faad411be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1898318-add-wait-flag-to-create-sharee-group-operation-cd8310b241d377b0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1899325-implement-usage-of-c-or-column-without-additional-logic-2970ee294f32bd31.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1902873-fix-py-raw-error-msg-a839fee2ac7b9d3d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1909477-fix-forbid-users-to-create-shares-with-the-name-none-cfb0a59baa597803.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1920888-fix-error-in-cli-manila-list-with-sorting-key-availabilityzone-cea5a1f5d8a38fc3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1925486-add-share-network-option-to-replica-create-api-7d2ff3628e93fc77.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1953670-fix-id-attr-for-share-group-type-access-repr-008338a53d7a6a50.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1959329-fix-server-listing-by-subnets-fa6447fd43093cae.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1960422-fix-no-default-share-type-d6191ea0aa1e57fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1960490-use-suitable-version-for-osc-b375a32273b56522.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1962288-fixed-share-network-create-command-879dc3deca131ef9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1975488-skip-force-kwarg-if-unspecified-f98c717df1d6e364.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1980985-dont-use-share-type-with-snapshot-ref-de0331c640afbbd3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-1999775-add-os-key-0cfc95c7b480df05.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-2030686-fix-default-share-lookup-cc7e592a0dc855e1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug-share-access-list-3cf3114doe40k599.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug_1570085_fix-905786b797379309.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug_1603387_fix_env_variable_8ed5450aab41aa5f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug_1606168_fix-54d3c3bb78389f01.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug_1715769_fix-3ec701b0fb9d7910.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug_1777849_1779935_fix-344cb8f09b7df502.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/bug_1782672-1954059b373f03de.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/deprecate-manila-shell-0061cbcab5d3d75b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/drop-py36-and-py37-85cf389b2842f045.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/drop-python2-support-71c7b9e1dcf8c890.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/expose-access-key-in-access-list-API-b57c386c9048ae55.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/fix-and-improve-access-rules-a118a7f8e22f65bb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/fix-is-default-empty-557844001e0401e2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/graduate-share-replication-feature-49770e921b4338fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/handle-missing-api-minor-version-5a6d242f28883442.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/manage-unmanage-share-servers-8c7b27a1fe80e5fa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/manila-client-support-recycle-bin-4ecb5de770bd525f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2119 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/migration-share-type-4fc3b7c6187f5201.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/mountable_snapshot-ced01da7dffc6d7e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/remove-nova-net-id-option-for-share-nets-82e424b75221528b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/share-backup-98e11c6a28897e94.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/share-revert-to-snapshot-e899a4b7e1126749.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/share_type-skip-format-119595e62900e571.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/start-using-reno-b744cd0259c7a88c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/support-create-share-from-snapshot-extra-spec-cdba92f179c1c5c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/support-share-server-migration-9804752270c6b153.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/support-show-type-6380b7c539c95ba8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/type-create-extra-specs-691572762357ef3b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/update-api-version-create-share-from-snapshot-another-pool-or-backend-694cfda84a41c4ff.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/notes/v2-0-0-deprecated-opts-removal-863565618535733d.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.849259 python-manilaclient-4.7.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.849259 python-manilaclient-4.7.0/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.849259 python-manilaclient-4.7.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8911 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/newton.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/ocata.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      847 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.769262 python-manilaclient-4.7.0/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.849259 python-manilaclient-4.7.0/roles/populate-manilaclient-config/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/roles/populate-manilaclient-config/README.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.849259 python-manilaclient-4.7.0/roles/populate-manilaclient-config/defaults/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/roles/populate-manilaclient-config/defaults/main.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.849259 python-manilaclient-4.7.0/roles/populate-manilaclient-config/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/roles/populate-manilaclient-config/tasks/main.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5570 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12673 2023-11-20 07:06:08.853259 python-manilaclient-4.7.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.849259 python-manilaclient-4.7.0/tools/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/tools/manila.bash_completion
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2575 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-11-20 07:06:08.849259 python-manilaclient-4.7.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/zuul.d/project.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4755 2023-11-20 07:05:46.000000 python-manilaclient-4.7.0/zuul.d/python-manilaclient-jobs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.633288 python-manilaclient-4.8.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       74 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7221 2024-03-01 09:55:55.000000 python-manilaclient-4.8.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      649 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    33453 2024-03-01 09:55:55.000000 python-manilaclient-4.8.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2275 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/HACKING
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11837 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5961 2024-03-01 09:55:55.633288 python-manilaclient-4.8.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4088 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.553266 python-manilaclient-4.8.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        7 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/doc/.gitignore
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3188 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/doc/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.553266 python-manilaclient-4.8.0/doc/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.553266 python-manilaclient-4.8.0/doc/source/cli/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      460 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/doc/source/cli/decoder.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.553266 python-manilaclient-4.8.0/doc/source/cli/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13353 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/doc/source/cli/osc/manila.csv
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.553266 python-manilaclient-4.8.0/doc/source/cli/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4537 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/doc/source/cli/osc/v2/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1695 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/doc/source/cli/osc_plugin_cli.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3599 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.557267 python-manilaclient-4.8.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2761 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/doc/source/contributor/contributing.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8806 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/doc/source/contributor/functional-tests.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      482 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1523 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.557267 python-manilaclient-4.8.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2118 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/doc/source/user/api.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1746 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/doc/source/user/shell.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.545264 python-manilaclient-4.8.0/etc/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.557267 python-manilaclient-4.8.0/etc/manilaclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/etc/manilaclient/README.manilaclient.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.557267 python-manilaclient-4.8.0/etc/oslo-config-generator/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/etc/oslo-config-generator/manilaclient.conf
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.557267 python-manilaclient-4.8.0/manilaclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1248 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15186 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/api_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18336 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2387 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.557267 python-manilaclient-4.8.0/manilaclient/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1131 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/common/_i18n.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.557267 python-manilaclient-4.8.0/manilaclient/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12887 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/common/apiclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2781 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/common/apiclient/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8172 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/common/cliutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4098 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/common/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7277 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/common/httpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10524 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/config.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1825 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1405 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/extension.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.561268 python-manilaclient-4.8.0/manilaclient/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4367 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/plugin.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4021 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.565269 python-manilaclient-4.8.0/manilaclient/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1310 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/availability_zones.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.565269 python-manilaclient-4.8.0/manilaclient/osc/v2/data/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13353 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/data/manila.csv
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6631 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14707 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14033 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/resource_locks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20321 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5486 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    53041 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17889 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14055 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14824 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6315 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11713 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18730 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3089 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7645 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2202 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13048 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27777 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3636 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2831 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14367 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23898 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3244 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5018 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30280 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9165 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3975 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16122 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/osc/v2/share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    32358 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.565269 python-manilaclient-4.8.0/manilaclient/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.573271 python-manilaclient-4.8.0/manilaclient/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21492 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    90065 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2322 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.577273 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17567 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      980 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4110 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7076 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_resource_locks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9281 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5178 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3533 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1281 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1418 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3896 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1539 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2618 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2349 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3329 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7773 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3541 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5408 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8626 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6111 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_shares_group_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2146 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2442 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6668 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1002 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2755 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13085 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2727 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1729 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13367 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4622 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    23687 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4371 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1966 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14265 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4050 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20496 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11999 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14916 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_shares_listing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5391 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_shares_metadata.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7615 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_snapshot_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4968 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4634 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3584 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/test_snapshots_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4955 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/functional/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.577273 python-manilaclient-4.8.0/manilaclient/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.577273 python-manilaclient-4.8.0/manilaclient/tests/unit/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/common/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.577273 python-manilaclient-4.8.0/manilaclient/tests/unit/common/apiclient/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/common/apiclient/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8145 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/common/test_httpclient.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2935 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/fakes.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.577273 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6610 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/osc_fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2555 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/osc_utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.585275 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    51641 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1963 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6194 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16278 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10236 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_resource_locks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22375 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9276 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    68101 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20521 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13644 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    21560 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17697 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6874 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24594 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5208 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12339 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3044 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16353 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    27426 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5395 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_pools.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3996 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22544 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24995 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5687 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8248 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    44426 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8938 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20743 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_type.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6357 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14907 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/test_api_versions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2734 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/test_base.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5305 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7759 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/test_functional_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17744 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3104 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.585275 python-manilaclient-4.8.0/manilaclient/tests/unit/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1187 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1212 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1161 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1206 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1240 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1216 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1208 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1224 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1239 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1192 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1155 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_shares.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.593277 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6889 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/fake_clients.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    47273 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/fakes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2129 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13669 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_client.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5458 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4375 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2780 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12085 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2962 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8545 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3758 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3604 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1945 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9947 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4083 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7915 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11617 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2142 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4436 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3069 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11771 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1894 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5851 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11823 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1653 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1831 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3612 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9976 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    30414 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   157650 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3595 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18918 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2107 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/utils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.597278 python-manilaclient-4.8.0/manilaclient/v1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      917 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10490 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.597278 python-manilaclient-4.8.0/manilaclient/v1/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1253 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/contrib/list_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1225 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1269 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1265 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1260 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1256 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1285 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1252 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1211 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v1/shares.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.605280 python-manilaclient-4.8.0/manilaclient/v2/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      681 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1313 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/availability_zones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13178 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/client.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.605280 python-manilaclient-4.8.0/manilaclient/v2/contrib/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/contrib/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1448 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/contrib/list_extensions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2873 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/limits.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2710 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6071 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/quota_classes.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11053 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/quotas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4713 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/resource_locks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1528 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/scheduler_stats.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9732 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/security_services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3717 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/services.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2994 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_access_rules.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4832 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_backups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1801 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9326 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_group_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3695 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_group_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7367 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_group_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11213 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_groups.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1994 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4228 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5217 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_network_subnets.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13094 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_networks.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2943 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_replica_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11234 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_replicas.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10761 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_servers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1826 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_snapshot_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1940 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_snapshot_instance_export_locations.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2700 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_snapshot_instances.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9276 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_snapshots.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4526 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_transfers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2373 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_type_access.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10307 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/share_types.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    31842 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/shares.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   225608 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/manilaclient/v2/shell.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.605280 python-manilaclient-4.8.0/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       40 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/playbooks/enable-fips.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.605280 python-manilaclient-4.8.0/playbooks/python-manilaclient-functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/playbooks/python-manilaclient-functional/post.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/playbooks/python-manilaclient-functional/run.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.605280 python-manilaclient-4.8.0/python_manilaclient.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5961 2024-03-01 09:55:55.000000 python-manilaclient-4.8.0/python_manilaclient.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    22113 2024-03-01 09:55:55.000000 python-manilaclient-4.8.0/python_manilaclient.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-01 09:55:55.000000 python-manilaclient-4.8.0/python_manilaclient.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11626 2024-03-01 09:55:55.000000 python-manilaclient-4.8.0/python_manilaclient.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-03-01 09:55:55.000000 python-manilaclient-4.8.0/python_manilaclient.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-03-01 09:55:55.000000 python-manilaclient-4.8.0/python_manilaclient.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      251 2024-03-01 09:55:55.000000 python-manilaclient-4.8.0/python_manilaclient.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       13 2024-03-01 09:55:55.000000 python-manilaclient-4.8.0/python_manilaclient.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.605280 python-manilaclient-4.8.0/rally-jobs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1890 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/rally-jobs/rally-manila-no-ss.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4247 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/rally-jobs/rally-manila.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.549265 python-manilaclient-4.8.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.629287 python-manilaclient-4.8.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/Bug-1990013-fix-share-grou-from-snapshot-create-fa3629cf1417ba20.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-access-visibility-and-deletion-locks-69978f052e25334c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-count-info-in-share-21a6b36c0f4c87b2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-count-info-in-snapshot-c9600adad648a486.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-dash-dash-help-subcomand-ad4226454aa07bc6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      250 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-defaultadsite-to-security-service-33fd0a5d1b865b11.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-export-location-filter-4cf3114doe40k598.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-ipv6-access-type-4dko90r1a9a1e0b8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      315 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-like-filter-591572762357ef4b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-message-list-and-delete-41b3323edd63d894.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-metadata-for-share-access-rule-11a6b36c0f4c87c2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      196 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-per-share-gigabytes-quotas-40bc404bd3cbdd89.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-query-params-pools-list-api-12cf1s14ddf40kdd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      319 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-quiesce-wait-time-for-replica-promote-30d9fa66afc854f2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       59 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-quota-per-share-type-support-3b2708ea232e69bc.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-scheduler-hints-to-share-create-70d429cb0aaf8f11.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      431 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-scheduler-hints-to-share-replica-create-d152a3934e5ad3a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-share-group-quotas-support-b6563cec58209a1d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      216 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-share-group-support-a3166f6ca4d06a81.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      774 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-share-replicas-and-replica-gigabytes-quotas-909436c2b2420f2c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-snapshot-instances-admin-api-3cf3114doe40k598.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      166 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-snapshot-metadata-49b0288bf2f12bf0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      181 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-subnet-metadata-82426986431b0179.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       72 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-support-filter-search-for-share-type-fdbaaa9510cc59dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       79 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add-support-to-check-quota-usage-scfdg14dod40k71a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/add_support_multiple_subnet_per_az-46145c3e90e097be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      146 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bp-allow-locking-shares-against-deletion-89e51e27368cda46.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      197 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bp-export-locations-replica-az-commands-03aa32c08f59c42d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bp-integrate-os-profiler-4818066dc2fbf7b7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      339 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bp-ocata-migration-improvements-f63c5d233856fbee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bp-support-group-spec-search-share-group-type-api-d5d9a6096f084b91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bp-support-query-user-messages-by-timestamp-34b70bba2d1b4d13.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       98 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bp-support-share-transfer-between-project-faefead551380eca.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      180 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bp-update-share-type-name-or-description-32d98b5a42cd8090.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1558995-fix-endpoint-not-found.yaml-a06a3b0ba5006718.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1608664-add-support-columns-share-replica-list-885bd8c8b4bfa8f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      231 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1611506-allow-deletion-multiple-resources
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       96 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1622540-add-missing-az-list-command-f90265de5c2f261b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1650774-share-instance-reset-state-9c4b26f44b5da0e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      380 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1664877-c462bfad92ce03e5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1674915-allow-user-access-fix-495b3e42bdc985ec.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1682726-remove-sort-key-export-location-from-list-885des26bd5ea2de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1707303-fix-list-command-when-not-given-search-opts-c06af7b344e9cb91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       65 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1709746-add-group-specs-in-share-group-type-create-command-f91265de5c2f251b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1717940-dash-dash-column-reports-nothing-for-capabilities-db8c1234fae91af5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1724183-add-share-type-description-8c4b26f44b5da1e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      115 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1733494-allow-user-group-name-with-blank-access-fix-885a3e42bdc985ec.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      118 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1738917-and-1738918-fix-access-share-group-type-by-name-3a8760522c147f28.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      259 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1798229-fix-create-share-from-snap-using-name-44100b907ea6a040.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1799934-add-ou-parameter-260f9aaf939d1919.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      102 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1802059-fix-is_default-a8d3d95ffa0aede9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      110 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1811516-bug-1811627-python3-fixes-4b26130027b2c076.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      235 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1814094-fix-_get_base_url-method-168e12292aeec8f1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      211 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1830677-fix-13b30d6a89f43246.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      189 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1855391-support-force-extend-share-6b5ebcfe1de0ca7b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      395 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1871252-update-default-quotas-via-quota-class-share-groups-share-group-snapshots-20ec1dfcc0a7e81c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1898304-add-wait-to-share-create-delete-f121073f2f4402ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      204 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1898308-add-wait-to-share-extend-shrink-c9cc413c50d9832a.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      202 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1898309-add-wait-to-share-manage-unmanage-d2060c61cc295bfd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1898315-add-wait-flag-to-manage-share-server-operation-be6488c2a57536e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      186 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1898316-add-wait-option-for-deleting-a-share-server-e2228018585de5cb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      269 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1898317-add-wait-option-for-force-deleting-share-snapshot-share-instance-fb2531b6033f0ae5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1898318-add-wait-flag-for-deleting-a-share-group-operation-c602ba9faad411be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1898318-add-wait-flag-to-create-sharee-group-operation-cd8310b241d377b0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      188 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1899325-implement-usage-of-c-or-column-without-additional-logic-2970ee294f32bd31.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1902873-fix-py-raw-error-msg-a839fee2ac7b9d3d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      221 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1909477-fix-forbid-users-to-create-shares-with-the-name-none-cfb0a59baa597803.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1920888-fix-error-in-cli-manila-list-with-sorting-key-availabilityzone-cea5a1f5d8a38fc3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1925486-add-share-network-option-to-replica-create-api-7d2ff3628e93fc77.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      220 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1953670-fix-id-attr-for-share-group-type-access-repr-008338a53d7a6a50.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      170 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1959329-fix-server-listing-by-subnets-fa6447fd43093cae.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      218 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1960422-fix-no-default-share-type-d6191ea0aa1e57fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1960490-use-suitable-version-for-osc-b375a32273b56522.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1962288-fixed-share-network-create-command-879dc3deca131ef9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1975488-skip-force-kwarg-if-unspecified-f98c717df1d6e364.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1980985-dont-use-share-type-with-snapshot-ref-de0331c640afbbd3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      149 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-1999775-add-os-key-0cfc95c7b480df05.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      329 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-2030686-fix-default-share-lookup-cc7e592a0dc855e1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      234 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-2047249-fix-osc-quota-set-per-share-gigabytes-fcff7f8ce2cc3c75.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-2051737-fix-share-force-delete-request-6d2578fb7da61e3f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      164 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug-share-access-list-3cf3114doe40k599.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      175 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug_1570085_fix-905786b797379309.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      132 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug_1603387_fix_env_variable_8ed5450aab41aa5f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug_1606168_fix-54d3c3bb78389f01.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug_1715769_fix-3ec701b0fb9d7910.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug_1777849_1779935_fix-344cb8f09b7df502.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       83 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/bug_1782672-1954059b373f03de.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      673 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/deprecate-manila-shell-0061cbcab5d3d75b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      589 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/drop-py36-and-py37-85cf389b2842f045.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      293 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/drop-python2-support-71c7b9e1dcf8c890.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/expose-access-key-in-access-list-API-b57c386c9048ae55.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/fix-and-improve-access-rules-a118a7f8e22f65bb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/fix-is-default-empty-557844001e0401e2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      499 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/graduate-share-replication-feature-49770e921b4338fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       81 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/handle-missing-api-minor-version-5a6d242f28883442.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      165 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/manage-unmanage-share-servers-8c7b27a1fe80e5fa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/manila-client-support-recycle-bin-4ecb5de770bd525f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2119 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/migration-share-type-4fc3b7c6187f5201.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/mountable_snapshot-ced01da7dffc6d7e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      823 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      582 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      272 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/remove-nova-net-id-option-for-share-nets-82e424b75221528b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      320 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/share-backup-98e11c6a28897e94.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      550 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/share-revert-to-snapshot-e899a4b7e1126749.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      304 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/share_type-skip-format-119595e62900e571.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/start-using-reno-b744cd0259c7a88c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/support-create-share-from-snapshot-extra-spec-cdba92f179c1c5c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      322 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/support-share-server-migration-9804752270c6b153.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       53 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/support-show-type-6380b7c539c95ba8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/support_add_disabled_reason_to_services-08cb52e4711745c7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       73 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/type-create-extra-specs-691572762357ef3b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      262 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/update-api-version-create-share-from-snapshot-another-pool-or-backend-694cfda84a41c4ff.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      394 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/notes/v2-0-0-deprecated-opts-removal-863565618535733d.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.633288 python-manilaclient-4.8.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/2023.2.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.633288 python-manilaclient-4.8.0/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.633288 python-manilaclient-4.8.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8911 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      288 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/newton.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/ocata.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      107 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      847 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.549265 python-manilaclient-4.8.0/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.633288 python-manilaclient-4.8.0/roles/populate-manilaclient-config/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1257 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/roles/populate-manilaclient-config/README.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.633288 python-manilaclient-4.8.0/roles/populate-manilaclient-config/defaults/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      199 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/roles/populate-manilaclient-config/defaults/main.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.633288 python-manilaclient-4.8.0/roles/populate-manilaclient-config/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2541 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/roles/populate-manilaclient-config/tasks/main.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5570 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12753 2024-03-01 09:55:55.637289 python-manilaclient-4.8.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      697 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.633288 python-manilaclient-4.8.0/tools/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      367 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/tools/manila.bash_completion
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2575 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-03-01 09:55:55.633288 python-manilaclient-4.8.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      492 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/zuul.d/project.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4755 2024-03-01 09:55:26.000000 python-manilaclient-4.8.0/zuul.d/python-manilaclient-jobs.yaml
```

### Comparing `python-manilaclient-4.7.0/AUTHORS` & `python-manilaclient-4.8.0/AUTHORS`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,15 @@
 Shane Wang <shane.wang@intel.com>
 Shuquan Huang <huang.shuquan@99cloud.net>
 Spyros Trigazis <spyridon.trigazis@cern.ch>
 Stephen Finucane <sfinucan@redhat.com>
 Stephen Finucane <stephenfin@redhat.com>
 Sun Jun <jun.sun@intel.com>
 Swapnil Kulkarni (coolsvap) <me@coolsvap.net>
+Takashi Kajinami <kajinamit@oss.nttdata.com>
 Takashi Kajinami <tkajinam@redhat.com>
 Thomas Bechtold <tbechtold@suse.com>
 Tom Barron <tpb@dyncloud.net>
 Tom Patzig <tom.patzig@sap.com>
 Tony Breeds <tony@bakeyournoodle.com>
 Tony Xu <hhktony@gmail.com>
 Valeriy Ponomaryov <vponomaryov@mirantis.com>
@@ -161,14 +162,15 @@
 melissaml <ma.lei@99cloud.net>
 namrata <namrata.sitlani@citynetwork.eu>
 nidhimittalhada <nidhimittal19@gmail.com>
 paulali <paulali@protonmail.com>
 pengyuesheng <pengyuesheng@gohighsec.com>
 qingszhao <zhao.daqing@99cloud.net>
 ricolin <rico.l@inwinstack.com>
+sdailey <samuel.dailey@ndus.edu>
 shu-mutou <shu-mutou@rf.jp.nec.com>
 silvacarloss <ces.eduardo98@gmail.com>
 sneha.gaddam <sneha.gaddam@capitalone.com>
 sonu.kumar <sonu.kumar@nectechnologies.in>
 sriram ramakrishnan <sramakr@gmail.com>
 sunjia <sunjia@inspur.com>
 ting.wang <ting.wang@easystack.cn>
```

### Comparing `python-manilaclient-4.7.0/CONTRIBUTING.rst` & `python-manilaclient-4.8.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/ChangeLog` & `python-manilaclient-4.8.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,28 @@
 CHANGES
 =======
 
+4.8.0
+-----
+
+* CLI for disable service reason
+* reno: Update master for unmaintained/yoga
+* Fix share force delete case
+* Bump hacking
+* Fix "per\_share\_gigabytes" in "openstack quota set"
+* Fix list call when search\_opts isn't provided
+* Update python classifier in setup.cfg
+
 4.7.0
 -----
 
 * Fix default share type resolution in OSC
 * Fix "test\_share\_access\_show" osc functional test
 * Fix decoder path and add transfer commands
+* [OSC] Add OSC Functional Tests Snapshot Instances
 * Update master for stable/2023.2
 
 4.6.0
 -----
 
 * Bump tox version
 * Implement share backup
```

### Comparing `python-manilaclient-4.7.0/HACKING` & `python-manilaclient-4.8.0/HACKING`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/LICENSE` & `python-manilaclient-4.8.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/PKG-INFO` & `python-manilaclient-4.8.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-manilaclient
-Version: 4.7.0
+Version: 4.8.0
 Summary: Client library for OpenStack Manila API.
 Home-page: https://docs.openstack.org/python-manilaclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -124,8 +124,10 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
```

### Comparing `python-manilaclient-4.7.0/README.rst` & `python-manilaclient-4.8.0/README.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/doc/Makefile` & `python-manilaclient-4.8.0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/doc/source/cli/osc/manila.csv` & `python-manilaclient-4.8.0/doc/source/cli/osc/manila.csv`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/doc/source/cli/osc/v2/index.rst` & `python-manilaclient-4.8.0/doc/source/cli/osc/v2/index.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/doc/source/cli/osc_plugin_cli.rst` & `python-manilaclient-4.8.0/doc/source/cli/osc_plugin_cli.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/doc/source/conf.py` & `python-manilaclient-4.8.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/doc/source/contributor/contributing.rst` & `python-manilaclient-4.8.0/doc/source/contributor/contributing.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/doc/source/contributor/functional-tests.rst` & `python-manilaclient-4.8.0/doc/source/contributor/functional-tests.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/doc/source/index.rst` & `python-manilaclient-4.8.0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/doc/source/user/api.rst` & `python-manilaclient-4.8.0/doc/source/user/api.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/doc/source/user/shell.rst` & `python-manilaclient-4.8.0/doc/source/user/shell.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/__init__.py` & `python-manilaclient-4.8.0/manilaclient/__init__.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/api_versions.py` & `python-manilaclient-4.8.0/manilaclient/api_versions.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 from manilaclient.common import cliutils
 from manilaclient.common import constants
 from manilaclient import exceptions
 from manilaclient import utils
 
 LOG = logging.getLogger(__name__)
 
-MAX_VERSION = '2.82'
+MAX_VERSION = '2.83'
 MIN_VERSION = '2.0'
 DEPRECATED_VERSION = '1.0'
 _VERSIONED_METHOD_MAP = {}
 
 
 class APIVersion(object):
     """Top level object to support Manila API Versioning.
```

### Comparing `python-manilaclient-4.7.0/manilaclient/base.py` & `python-manilaclient-4.8.0/manilaclient/base.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/client.py` & `python-manilaclient-4.8.0/manilaclient/client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/common/_i18n.py` & `python-manilaclient-4.8.0/manilaclient/common/_i18n.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/common/apiclient/exceptions.py` & `python-manilaclient-4.8.0/manilaclient/common/apiclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/common/apiclient/utils.py` & `python-manilaclient-4.8.0/manilaclient/common/apiclient/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/common/cliutils.py` & `python-manilaclient-4.8.0/manilaclient/common/cliutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -247,16 +247,16 @@
 
 
 def get_service_type(f):
     """Retrieves service type from function."""
     return getattr(f, 'service_type', None)
 
 
-def pretty_choice_list(l):
-    return ', '.join("'%s'" % i for i in l)
+def pretty_choice_list(choices):
+    return ', '.join("'%s'" % choice for choice in choices)
 
 
 def exit(msg=''):
     if msg:
         print(msg, file=sys.stderr)
     sys.exit(1)
```

### Comparing `python-manilaclient-4.7.0/manilaclient/common/constants.py` & `python-manilaclient-4.8.0/manilaclient/common/constants.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/common/httpclient.py` & `python-manilaclient-4.8.0/manilaclient/common/httpclient.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/config.py` & `python-manilaclient-4.8.0/manilaclient/config.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/exceptions.py` & `python-manilaclient-4.8.0/manilaclient/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/extension.py` & `python-manilaclient-4.8.0/manilaclient/extension.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/plugin.py` & `python-manilaclient-4.8.0/manilaclient/osc/plugin.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/utils.py` & `python-manilaclient-4.8.0/manilaclient/osc/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/availability_zones.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/data/manila.csv` & `python-manilaclient-4.8.0/manilaclient/osc/v2/data/manila.csv`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/messages.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/quotas.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/quotas.py`

 * *Files 1% similar despite different names*

```diff
@@ -156,15 +156,14 @@
 
         kwargs = {
             "shares": parsed_args.shares,
             "snapshots": parsed_args.snapshots,
             "gigabytes": parsed_args.gigabytes,
             "snapshot_gigabytes": parsed_args.snapshot_gigabytes,
             "share_networks": parsed_args.share_networks,
-            "per_share_gigabytes": parsed_args.per_share_gigabytes,
         }
 
         if parsed_args.share_type is not None:
             if share_client.api_version < api_versions.APIVersion('2.39'):
                 raise exceptions.CommandError(_(
                     "'share type' quotas are available only starting with "
                     "'2.39' API microversion."))
```

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/resource_locks.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/resource_locks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/security_services.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/services.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/services.py`

 * *Files 15% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 #   WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #   License for the specific language governing permissions and limitations
 #   under the License.
 from osc_lib.command import command
 from osc_lib import exceptions
 from osc_lib import utils as osc_utils
 
+from manilaclient import api_versions
 from manilaclient.common._i18n import _
 
 
 class SetShareService(command.Command):
     """Enable/disable share service (Admin only)."""
     _description = _("Enable/Disable share service (Admin only).")
 
@@ -40,31 +41,52 @@
             help=_('Enable share service'),
         )
         enable_group.add_argument(
             '--disable',
             action='store_true',
             help=_('Disable share service'),
         )
+        parser.add_argument(
+            "--disable-reason",
+            metavar="<reason>",
+            help=_("Reason for disabling the service "
+                   "(should be used with --disable option)")
+        )
         return parser
 
     def take_action(self, parsed_args):
+        if parsed_args.disable_reason and not parsed_args.disable:
+            msg = _("Cannot specify option --disable-reason without "
+                    "--disable specified.")
+            raise exceptions.CommandError(msg)
+
         share_client = self.app.client_manager.share
 
         if parsed_args.enable:
             try:
                 share_client.services.enable(
                     parsed_args.host, parsed_args.binary)
             except Exception as e:
                 raise exceptions.CommandError(_(
                     "Failed to enable service: %s" % e))
 
         if parsed_args.disable:
+            if parsed_args.disable_reason:
+                if share_client.api_version < api_versions.APIVersion("2.83"):
+                    raise exceptions.CommandError(
+                        "Service disable reason can be specified only with "
+                        "manila API version >= 2.83")
             try:
-                share_client.services.disable(
-                    parsed_args.host, parsed_args.binary)
+                if parsed_args.disable_reason:
+                    share_client.services.disable(
+                        parsed_args.host, parsed_args.binary,
+                        disable_reason=parsed_args.disable_reason)
+                else:
+                    share_client.services.disable(
+                        parsed_args.host, parsed_args.binary)
             except Exception as e:
                 raise exceptions.CommandError(_(
                     "Failed to disable service: %s" % e))
 
 
 class ListShareService(command.Lister):
     """List share services (Admin only)."""
@@ -123,12 +145,14 @@
             'Binary',
             'Host',
             'Zone',
             'Status',
             'State',
             'Updated At'
         ]
+        if share_client.api_version >= api_versions.APIVersion("2.83"):
+            columns.append('Disabled Reason')
 
         data = (osc_utils.get_dict_properties(
             service._info, columns) for service in services)
 
         return (columns, data)
```

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share.py`

 * *Files 0% similar despite different names*

```diff
@@ -346,15 +346,15 @@
                 share_group_id = None
                 if parsed_args.share_group:
                     share_group_id = apiutils.find_resource(
                         share_client.share_groups, parsed_args.share_group).id
 
                 if parsed_args.force:
                     share_client.shares.force_delete(share_obj)
-                if parsed_args.soft:
+                elif parsed_args.soft:
                     if share_client.api_version >= api_versions.APIVersion(
                             '2.69'):
                         share_client.shares.soft_delete(share_obj)
                     else:
                         raise exceptions.CommandError(
                             "Soft Deleting shares is only "
                             "available with manila API version >= 2.69")
```

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_access_rules.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_backups.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_backups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_group_snapshots.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_group_type_access.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_group_types.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_group_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_groups.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_instance_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_instances.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_limits.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_network_subnets.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_networks.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_pools.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_pools.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_replica_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_replicas.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_servers.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_snapshot_instances.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_snapshots.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_transfers.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_transfers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_type_access.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/osc/v2/share_types.py` & `python-manilaclient-4.8.0/manilaclient/osc/v2/share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/shell.py` & `python-manilaclient-4.8.0/manilaclient/shell.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/base.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -94,15 +94,15 @@
         if resources is None:
             resources = cls.method_resources
         for res in resources:
             if "deleted" not in res:
                 res["deleted"] = False
             if "client" not in res:
                 res["client"] = cls.get_cleanup_client()
-            if not(res["deleted"]):
+            if not res["deleted"]:
                 res_id = res["id"]
                 client = res["client"]
                 deletion_params = res.get("deletion_params")
                 with handle_cleanup_exceptions():
                     # TODO(vponomaryov): add support for other resources
                     if res["type"] == "share_type":
                         client.delete_share_type(
```

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/client.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/exceptions.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/exceptions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/base.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -141,15 +141,15 @@
         result_dict = self._get_property_from_output(output)
         return result_dict
 
     def create_share(self, share_protocol=None, size=None, name=None,
                      snapshot_id=None, properties=None, share_network=None,
                      description=None, public=False, share_type=None,
                      availability_zone=None, share_group=None,
-                     add_cleanup=True, client=None,
+                     add_cleanup=True, client=None, wait=None,
                      wait_for_status='available'):
 
         name = name or data_utils.rand_name('autotest_share_name')
         # share_type = dhss_false until we have implemented
         # share network commands for osc
         share_type = share_type or 'dhss_false'
 
@@ -170,14 +170,16 @@
                        % {'key': key, 'value': value})
         if share_network:
             cmd = cmd + ' --share-network %s' % share_network
         if availability_zone:
             cmd = cmd + ' --availability-zone %s' % availability_zone
         if share_group:
             cmd = cmd + ' --share-group %s' % share_group
+        if wait:
+            cmd = cmd + ' --wait'
 
         share_object = self.dict_result('share', cmd, client=client)
         self._wait_for_object_status(
             'share', share_object['id'], wait_for_status)
 
         if add_cleanup:
             self.addCleanup(
@@ -418,15 +420,15 @@
         if neutron_net_id:
             cmd += f' --neutron-net-id {neutron_net_id}'
         if neutron_subnet_id:
             cmd += f' --neutron-subnet-id {neutron_subnet_id}'
         if availability_zone:
             cmd += f' --availability-zone {availability_zone}'
         if restart_check:
-            cmd += f' --restart-check'
+            cmd += ' --restart-check'
 
         check_result = self.dict_result('share', cmd)
         return check_result
 
     def create_resource_lock(self, resource_id, resource_type='share',
                              resource_action='delete', lock_reason=None,
                              add_cleanup=True, client=None):
```

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_availability_zones.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_messages.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_resource_locks.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_resource_locks.py`

 * *Files 3% similar despite different names*

```diff
@@ -105,26 +105,26 @@
         self.assertEqual(sorted(LOCK_SUMMARY_ATTRIBUTES),
                          sorted(locks[0].keys()))
 
         locks = self.listing_result('share',
                                     'lock list --lock-context user '
                                     f' --resource {self.share["id"]}')
         self.assertEqual(2, len(locks))
-        self.assertNotIn(lock_3['id'], [l['ID'] for l in locks])
+        self.assertNotIn(lock_3['id'], [lock['ID'] for lock in locks])
 
         locks = self.listing_result('share',
                                     'lock list --lock-context user'
                                     f' --resource {self.share["id"]}'
                                     ' --sort-key created_at '
                                     ' --sort-dir desc '
                                     ' --limit 1')
         self.assertEqual(1, len(locks))
-        self.assertIn(lock_2['id'], [l['ID'] for l in locks])
-        self.assertNotIn(lock_1['id'], [l['ID'] for l in locks])
-        self.assertNotIn(lock_3['id'], [l['ID'] for l in locks])
+        self.assertIn(lock_2['id'], [lock['ID'] for lock in locks])
+        self.assertNotIn(lock_1['id'], [lock['ID'] for lock in locks])
+        self.assertNotIn(lock_3['id'], [lock['ID'] for lock in locks])
 
     def test_lock_set_unset_lock_reason(self):
         lock = self.create_resource_lock(self.share['id'],
                                          client=self.user_client)
         self.assertEqual('None', lock['lock_reason'])
 
         self.openstack('share lock set '
```

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_access_rules.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_access_rules.py`

 * *Files 2% similar despite different names*

```diff
@@ -182,15 +182,15 @@
             access_type='ip',
             access_to=access_to_filter,
             wait=True)
 
         output = self.openstack(
             'share',
             params=f'access list {share["id"]} --access-to {access_to_filter}',
-            flags=f'--os-share-api-version 2.82')
+            flags='--os-share-api-version 2.82')
         access_rule_list = self.parser.listing(output)
 
         self.assertTrue(len(access_rule_list) == 1)
 
 
 class ShowShareAccessRulesTestCase(base.OSCClientTestBase):
     def test_share_access_show(self):
@@ -210,15 +210,15 @@
         self.assertEqual(access_rule_show['access_to'], '0.0.0.0/0')
         self.assertEqual(access_rule_show['access_type'], 'ip')
         self.assertEqual(access_rule_show['state'], 'active')
         self.assertEqual(access_rule_show['access_key'], 'None')
         self.assertEqual(access_rule_show['created_at'],
                          access_rule['created_at'])
         self.assertEqual(access_rule_show['properties'], '')
-        self.assertTrue('updated_at' in access_rule_show)
+        self.assertIn('updated_at', access_rule_show)
 
 
 class SetShareAccessTestCase(base.OSCClientTestBase):
     def test_set_share_access(self):
         share = self.create_share()
         access_rule = self.create_share_access_rule(
             share=share['name'],
```

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_backups.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_backups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_group_type_access.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_limits.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_network_subnets.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_networks.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_pools.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_pools.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_replicas.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_services.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_services.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,17 +41,18 @@
     def test_services_set(self):
         services = self.list_services()
         service = [service for service in services if
                    service["Binary"] == "manila-data"]
         first_service = service[0]
         self.openstack(f'share service set {first_service["Host"]} '
                        f'{first_service["Binary"]} '
-                       '--disable')
+                       '--disable --disable-reason test')
         result = self.listing_result('share service',
                                      'list --status disabled')
         self.assertEqual(first_service['ID'], result[0]['ID'])
         self.assertEqual('disabled', result[0]['Status'])
+        self.assertEqual('test', result[0]['Disabled Reason'])
 
         # enable the share service again
         self.openstack(f'share service set {first_service["Host"]} '
                        f'{first_service["Binary"]} '
                        '--enable')
```

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_snapshots.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_transfers.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_transfers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_share_types.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_shares.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/osc/test_shares_group_type.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/osc/test_shares_group_type.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_availability_zones.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_common.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_common.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_limits.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_messages.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_quotas.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_scheduler_stats.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_security_services.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_services.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_access.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_network_subnets.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_networks.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_replica_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_replicas.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_servers.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_transfers.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_transfers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_share_types.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_shares.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_shares_listing.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_shares_listing.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_shares_metadata.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_shares_metadata.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_snapshot_access.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_snapshot_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_snapshot_instances.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_snapshot_instances_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/test_snapshots_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/test_snapshots_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/functional/utils.py` & `python-manilaclient-4.8.0/manilaclient/tests/functional/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/common/test_httpclient.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/common/test_httpclient.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/fakes.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/fakes.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         found = False
         for entry in self.client.callstack:
             if expected == entry[0:2]:
                 found = True
                 break
 
         assert found, 'Expected %s %s; got %s' % (
-            expected, self.client.callstack)
+            expected[0], expected[1], self.client.callstack)
 
         if body is not None:
             try:
                 assert entry[2] == body
             except AssertionError:
                 print(entry[2])
                 print("!=")
```

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/osc_fakes.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/osc_fakes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/osc_utils.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/osc_utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/fakes.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/fakes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_messages.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_quotas.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_quotas.py`

 * *Files 8% similar despite different names*

```diff
@@ -74,16 +74,15 @@
             result = self.cmd.take_action(parsed_args)
             self.quota_classes_mock.update.assert_called_with(
                 class_name='default',
                 gigabytes=None,
                 share_networks=None,
                 shares=40,
                 snapshot_gigabytes=None,
-                snapshots=None,
-                per_share_gigabytes=None)
+                snapshots=None)
             self.assertIsNone(result)
             mock_find_resource.assert_not_called()
             self.quotas_mock.assert_not_called()
 
     def test_quota_set_shares(self):
         arglist = [
             self.project.id,
@@ -103,15 +102,14 @@
             self.quotas_mock.update.assert_called_with(
                 force=None,
                 gigabytes=None,
                 share_networks=None,
                 shares=40,
                 snapshot_gigabytes=None,
                 snapshots=None,
-                per_share_gigabytes=None,
                 tenant_id=self.project.id,
                 user_id=None)
             self.assertIsNone(result)
 
     def test_quota_set_gigabytes(self):
         arglist = [
             self.project.id,
@@ -131,15 +129,14 @@
             self.quotas_mock.update.assert_called_with(
                 force=None,
                 gigabytes=1100,
                 share_networks=None,
                 shares=None,
                 snapshot_gigabytes=None,
                 snapshots=None,
-                per_share_gigabytes=None,
                 tenant_id=self.project.id,
                 user_id=None)
             self.assertIsNone(result)
 
     def test_quota_set_share_type(self):
         arglist = [
             self.project.id,
@@ -160,15 +157,14 @@
                 force=None,
                 gigabytes=None,
                 share_networks=None,
                 share_type='default',
                 shares=None,
                 snapshot_gigabytes=None,
                 snapshots=None,
-                per_share_gigabytes=None,
                 tenant_id=self.project.id,
                 user_id=None)
             self.assertIsNone(result)
 
     def test_quota_set_force(self):
         arglist = [
             self.project.id,
@@ -191,15 +187,14 @@
                 force=True,
                 gigabytes=None,
                 share_networks=None,
                 shares=40,
                 snapshot_gigabytes=None,
                 snapshots=None,
                 tenant_id=self.project.id,
-                per_share_gigabytes=None,
                 user_id=None)
             self.assertIsNone(result)
 
     def test_quota_set_api_version_exception(self):
         self.app.client_manager.share.api_version = api_versions.APIVersion(
             '2.39'
         )
@@ -286,15 +281,14 @@
                 force=None,
                 gigabytes=None,
                 share_networks=None,
                 share_replicas=2,
                 shares=None,
                 snapshot_gigabytes=None,
                 snapshots=None,
-                per_share_gigabytes=None,
                 tenant_id=self.project.id,
                 user_id=None)
             self.assertIsNone(result)
 
     def test_quota_set_replica_gigabytes_exception(self):
         self.app.client_manager.share.api_version = api_versions.APIVersion(
             '2.51')
@@ -307,14 +301,30 @@
             ('replica_gigabytes', 10)
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
         self.assertRaises(
             exceptions.CommandError, self.cmd.take_action, parsed_args)
 
+    def test_quota_set_per_share_gigabytes_exception(self):
+        self.app.client_manager.share.api_version = api_versions.APIVersion(
+            '2.61')
+        arglist = [
+            self.project.id,
+            '--per-share-gigabytes', '10',
+        ]
+        verifylist = [
+            ('project', self.project.id),
+            ('per_share_gigabytes', 10)
+        ]
+
+        parsed_args = self.check_parser(self.cmd, arglist, verifylist)
+        self.assertRaises(
+            exceptions.CommandError, self.cmd.take_action, parsed_args)
+
     def test_quota_set_per_share_gigabytes(self):
         arglist = [
             self.project.id,
             '--per-share-gigabytes', '10',
         ]
         verifylist = [
             ('project', self.project.id),
```

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_resource_locks.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_resource_locks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_security_services.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share.py`

 * *Files 1% similar despite different names*

```diff
@@ -421,14 +421,16 @@
             ('shares', [shares[0].name])
         ]
 
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         result = self.cmd.take_action(parsed_args)
         self.shares_mock.delete.assert_called_with(shares[0], None)
+        self.shares_mock.soft_delete.assert_not_called()
+        self.shares_mock.force_delete.assert_not_called()
         self.assertIsNone(result)
 
     def test_share_delete_many(self):
         shares = self.setup_shares_mock(count=3)
 
         arglist = [v.id for v in shares]
         verifylist = [
@@ -477,14 +479,16 @@
             ('shares', [shares[0].name]),
         ]
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         result = self.cmd.take_action(parsed_args)
 
         self.shares_mock.force_delete.assert_called_once_with(shares[0])
+        self.shares_mock.delete.assert_not_called()
+        self.shares_mock.soft_delete.assert_not_called()
         self.assertIsNone(result)
 
     def test_share_delete_with_soft(self):
         shares = self.setup_shares_mock(count=1)
 
         arglist = [
             '--soft',
@@ -496,14 +500,16 @@
             ('shares', [shares[0].name]),
         ]
         parsed_args = self.check_parser(self.cmd, arglist, verifylist)
 
         result = self.cmd.take_action(parsed_args)
 
         self.shares_mock.soft_delete.assert_called_once_with(shares[0])
+        self.shares_mock.delete.assert_not_called()
+        self.shares_mock.force_delete.assert_not_called()
         self.assertIsNone(result)
 
     def test_share_delete_wrong_name(self):
         shares = self.setup_shares_mock(count=1)
 
         arglist = [
             shares[0].name + '-wrong-name'
```

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_backups.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_backups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_group_type.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_groups.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_instances.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_limits.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_networks.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_pools.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_pools.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_servers.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_transfers.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_transfers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_type.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_type.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/osc/v2/test_share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/test_api_versions.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/test_api_versions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/test_base.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/test_base.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/test_client.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/test_client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/test_functional_utils.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/test_functional_utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/test_shell.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/utils.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_limits.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_quota_classes.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_quotas.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_scheduler_stats.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_security_services.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_services.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_share_networks.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_share_servers.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_share_snapshots.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_share_type_access.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_share_types.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v1/test_shares.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v1/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/fake_clients.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/fake_clients.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/fakes.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/fakes.py`

 * *Files 0% similar despite different names*

```diff
@@ -1083,15 +1083,15 @@
         return (resp, {}, _body)
 
     def post_types_1_extra_specs(self, body, **kw):
         assert list(body) == ['extra_specs']
         return (200, {}, {'extra_specs': {'k': 'v'}})
 
     def delete_types_1_extra_specs_k(self, **kw):
-        return(204, {}, None)
+        return (204, {}, None)
 
     def delete_types_1(self, **kw):
         return (202, {}, None)
 
     def get_types_3_os_share_type_access(self, **kw):
         return (200, {}, {'share_type_access': [
             {'share_type_id': '11111111-1111-1111-1111-111111111111',
```

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_availability_zones.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_client.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_limits.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_limits.py`

 * *Files 0% similar despite different names*

```diff
@@ -156,9 +156,9 @@
         l1 = limits.AbsoluteLimit("name1", "value1")
         limitsManager = limits.LimitsManager(api)
 
         lim = limitsManager.get()
         api.client.get.assert_called_once_with('/limits')
 
         self.assertIsInstance(lim, limits.Limits)
-        for l in lim.absolute:
-            self.assertEqual(l1, l)
+        for li in lim.absolute:
+            self.assertEqual(l1, li)
```

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_messages.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_quota_classes.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_quotas.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_scheduler_stats.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_security_services.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_services.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_backups.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_backups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_group_type_access.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_group_types.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_group_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_groups.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_instances.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_network_subnets.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_networks.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_networks.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         }
 
     @ddt.data("2.25", "2.26")
     def test_create(self, microversion):
         api_version = api_versions.APIVersion(microversion)
         values = self.values.copy()
         if (api_version >= api_versions.APIVersion("2.26")):
-            del(values['nova_net_id'])
+            del values['nova_net_id']
         body_expected = {share_networks.RESOURCE_NAME: values}
 
         manager = share_networks.ShareNetworkManager(
             fakes.FakeClient(api_version=api_version))
         with mock.patch.object(manager, '_create', fakes.fake_create):
             result = manager.create(**values)
 
@@ -119,15 +119,15 @@
         ['fake share nw', _FakeShareNetwork()]
     ))
     @ddt.unpack
     def test_update_share_network(self, microversion, share_nw):
         api_version = api_versions.APIVersion(microversion)
         values = self.values.copy()
         if (api_version >= api_versions.APIVersion("2.26")):
-            del(values['nova_net_id'])
+            del values['nova_net_id']
         body_expected = {share_networks.RESOURCE_NAME: values}
 
         manager = share_networks.ShareNetworkManager(
             fakes.FakeClient(api_version=api_version))
         with mock.patch.object(manager, '_update', fakes.fake_update):
             result = manager.update(share_nw, **values)
             id = share_nw.id if hasattr(share_nw, 'id') else share_nw
```

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_replicas.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_servers.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_snapshot_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_snapshots.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_share_transfers.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_share_transfers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_shares.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_shell.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_shell.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_type_access.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/tests/unit/v2/test_types.py` & `python-manilaclient-4.8.0/manilaclient/tests/unit/v2/test_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/utils.py` & `python-manilaclient-4.8.0/manilaclient/utils.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/__init__.py` & `python-manilaclient-4.8.0/manilaclient/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/client.py` & `python-manilaclient-4.8.0/manilaclient/v1/client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/contrib/list_extensions.py` & `python-manilaclient-4.8.0/manilaclient/v1/contrib/list_extensions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/limits.py` & `python-manilaclient-4.8.0/manilaclient/v1/limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/quota_classes.py` & `python-manilaclient-4.8.0/manilaclient/v1/quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/quotas.py` & `python-manilaclient-4.8.0/manilaclient/v1/quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/scheduler_stats.py` & `python-manilaclient-4.8.0/manilaclient/v1/scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/security_services.py` & `python-manilaclient-4.8.0/manilaclient/v1/security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/services.py` & `python-manilaclient-4.8.0/manilaclient/v1/services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/share_networks.py` & `python-manilaclient-4.8.0/manilaclient/v1/share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/share_servers.py` & `python-manilaclient-4.8.0/manilaclient/v1/share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/share_snapshots.py` & `python-manilaclient-4.8.0/manilaclient/v1/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/share_type_access.py` & `python-manilaclient-4.8.0/manilaclient/v1/share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/share_types.py` & `python-manilaclient-4.8.0/manilaclient/v1/share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v1/shares.py` & `python-manilaclient-4.8.0/manilaclient/v1/shares.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/__init__.py` & `python-manilaclient-4.8.0/manilaclient/v2/__init__.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/availability_zones.py` & `python-manilaclient-4.8.0/manilaclient/v2/availability_zones.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/client.py` & `python-manilaclient-4.8.0/manilaclient/v2/client.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/contrib/list_extensions.py` & `python-manilaclient-4.8.0/manilaclient/v2/contrib/list_extensions.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/limits.py` & `python-manilaclient-4.8.0/manilaclient/v2/limits.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/messages.py` & `python-manilaclient-4.8.0/manilaclient/v2/messages.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/quota_classes.py` & `python-manilaclient-4.8.0/manilaclient/v2/quota_classes.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/quotas.py` & `python-manilaclient-4.8.0/manilaclient/v2/quotas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/resource_locks.py` & `python-manilaclient-4.8.0/manilaclient/v2/resource_locks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/scheduler_stats.py` & `python-manilaclient-4.8.0/manilaclient/v2/scheduler_stats.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/security_services.py` & `python-manilaclient-4.8.0/manilaclient/v2/security_services.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/services.py` & `python-manilaclient-4.8.0/manilaclient/v2/services.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,27 +62,35 @@
     def enable(self, host, binary):
         return self._do_enable(host, binary, RESOURCE_PATH_LEGACY)
 
     @api_versions.wraps("2.7")  # noqa
     def enable(self, host, binary):  # noqa
         return self._do_enable(host, binary, RESOURCE_PATH)
 
-    def _do_disable(self, host, binary, resource_path=RESOURCE_PATH):
+    def _do_disable(self, host, binary, resource_path=RESOURCE_PATH,
+                    disable_reason=None):
         """Disable the service specified by hostname and binary."""
         body = {"host": host, "binary": binary}
+        if disable_reason:
+            body["disabled_reason"] = disable_reason
         return self._update("%s/disable" % resource_path, body)
 
     @api_versions.wraps("1.0", "2.6")
     def disable(self, host, binary):
         return self._do_disable(host, binary, RESOURCE_PATH_LEGACY)
 
-    @api_versions.wraps("2.7")  # noqa
+    @api_versions.wraps("2.7", "2.82")  # noqa
     def disable(self, host, binary):  # noqa
         return self._do_disable(host, binary, RESOURCE_PATH)
 
+    @api_versions.wraps("2.83")  # noqa
+    def disable(self, host, binary, disable_reason=None):  # noqa
+        return self._do_disable(host, binary, RESOURCE_PATH,
+                                disable_reason=disable_reason)
+
     def server_api_version(self, url_append=""):
         """Returns the API Version supported by the server.
 
         :param url_append: String to append to url to obtain specific version
         :return: Returns response obj for a server that supports microversions.
                  Returns an empty list for Kilo and prior Manila servers.
         """
```

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_access_rules.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_access_rules.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_backups.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_backups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_group_snapshots.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_group_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_group_type_access.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_group_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_group_types.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_group_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_groups.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_groups.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_instance_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_instances.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_network_subnets.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_network_subnets.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_networks.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_networks.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_replica_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_replica_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_replicas.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_replicas.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_servers.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_servers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_snapshot_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_snapshot_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_snapshot_instance_export_locations.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_snapshot_instance_export_locations.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_snapshot_instances.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_snapshot_instances.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_snapshots.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_snapshots.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_transfers.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_transfers.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_type_access.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_type_access.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/share_types.py` & `python-manilaclient-4.8.0/manilaclient/v2/share_types.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/shares.py` & `python-manilaclient-4.8.0/manilaclient/v2/shares.py`

 * *Files 0% similar despite different names*

```diff
@@ -353,14 +353,16 @@
                             sort_key=sort_key, sort_dir=sort_dir,
                             return_raw=return_raw)
 
     @api_versions.wraps("2.35", "2.68")   # noqa
     def list(self, detailed=True, search_opts=None,   # noqa
              sort_key=None, sort_dir=None, return_raw=False):
         """Get a list of all shares."""
+        if search_opts is None:
+            search_opts = {}
         search_opts.pop("is_soft_deleted", None)
         return self.do_list(detailed=detailed, search_opts=search_opts,
                             sort_key=sort_key, sort_dir=sort_dir,
                             return_raw=return_raw)
 
     @api_versions.wraps("2.69")  # noqa
     def list(self, detailed=True, search_opts=None,  # noqa
```

### Comparing `python-manilaclient-4.7.0/manilaclient/v2/shell.py` & `python-manilaclient-4.8.0/manilaclient/v2/shell.py`

 * *Files 0% similar despite different names*

```diff
@@ -4880,14 +4880,15 @@
 
     if args.wait:
         share = _wait_for_share_status(cs, share)
     else:
         share = _find_share(cs, args.share)
     _print_share(cs, share)
 
+
 @cliutils.arg('share', metavar='<share>',
               help='Name or ID of share to shrink.')
 @cliutils.arg('new_size',
               metavar='<new_size>',
               type=int,
               help='New size of share, in GiBs.')
 @cliutils.arg(
```

### Comparing `python-manilaclient-4.7.0/python_manilaclient.egg-info/PKG-INFO` & `python-manilaclient-4.8.0/python_manilaclient.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: python-manilaclient
-Version: 4.7.0
+Version: 4.8.0
 Summary: Client library for OpenStack Manila API.
 Home-page: https://docs.openstack.org/python-manilaclient/latest/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========================
         Team and repository tags
@@ -124,8 +124,10 @@
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.8
```

### Comparing `python-manilaclient-4.7.0/python_manilaclient.egg-info/SOURCES.txt` & `python-manilaclient-4.8.0/python_manilaclient.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -119,14 +119,15 @@
 manilaclient/tests/functional/osc/test_share_limits.py
 manilaclient/tests/functional/osc/test_share_network_subnets.py
 manilaclient/tests/functional/osc/test_share_networks.py
 manilaclient/tests/functional/osc/test_share_pools.py
 manilaclient/tests/functional/osc/test_share_replica_export_locations.py
 manilaclient/tests/functional/osc/test_share_replicas.py
 manilaclient/tests/functional/osc/test_share_services.py
+manilaclient/tests/functional/osc/test_share_snapshot_instances.py
 manilaclient/tests/functional/osc/test_share_snapshots.py
 manilaclient/tests/functional/osc/test_share_transfers.py
 manilaclient/tests/functional/osc/test_share_types.py
 manilaclient/tests/functional/osc/test_shares.py
 manilaclient/tests/functional/osc/test_shares_group_type.py
 manilaclient/tests/unit/__init__.py
 manilaclient/tests/unit/fakes.py
@@ -359,14 +360,16 @@
 releasenotes/notes/bug-1960422-fix-no-default-share-type-d6191ea0aa1e57fa.yaml
 releasenotes/notes/bug-1960490-use-suitable-version-for-osc-b375a32273b56522.yaml
 releasenotes/notes/bug-1962288-fixed-share-network-create-command-879dc3deca131ef9.yaml
 releasenotes/notes/bug-1975488-skip-force-kwarg-if-unspecified-f98c717df1d6e364.yaml
 releasenotes/notes/bug-1980985-dont-use-share-type-with-snapshot-ref-de0331c640afbbd3.yaml
 releasenotes/notes/bug-1999775-add-os-key-0cfc95c7b480df05.yaml
 releasenotes/notes/bug-2030686-fix-default-share-lookup-cc7e592a0dc855e1.yaml
+releasenotes/notes/bug-2047249-fix-osc-quota-set-per-share-gigabytes-fcff7f8ce2cc3c75.yaml
+releasenotes/notes/bug-2051737-fix-share-force-delete-request-6d2578fb7da61e3f.yaml
 releasenotes/notes/bug-share-access-list-3cf3114doe40k599.yaml
 releasenotes/notes/bug_1570085_fix-905786b797379309.yaml
 releasenotes/notes/bug_1603387_fix_env_variable_8ed5450aab41aa5f.yaml
 releasenotes/notes/bug_1606168_fix-54d3c3bb78389f01.yaml
 releasenotes/notes/bug_1715769_fix-3ec701b0fb9d7910.yaml
 releasenotes/notes/bug_1777849_1779935_fix-344cb8f09b7df502.yaml
 releasenotes/notes/bug_1782672-1954059b373f03de.yaml
@@ -391,14 +394,15 @@
 releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml
 releasenotes/notes/share-revert-to-snapshot-e899a4b7e1126749.yaml
 releasenotes/notes/share_type-skip-format-119595e62900e571.yaml
 releasenotes/notes/start-using-reno-b744cd0259c7a88c.yaml
 releasenotes/notes/support-create-share-from-snapshot-extra-spec-cdba92f179c1c5c6.yaml
 releasenotes/notes/support-share-server-migration-9804752270c6b153.yaml
 releasenotes/notes/support-show-type-6380b7c539c95ba8.yaml
+releasenotes/notes/support_add_disabled_reason_to_services-08cb52e4711745c7.yaml
 releasenotes/notes/type-create-extra-specs-691572762357ef3b.yaml
 releasenotes/notes/update-api-version-create-share-from-snapshot-another-pool-or-backend-694cfda84a41c4ff.yaml
 releasenotes/notes/v2-0-0-deprecated-opts-removal-863565618535733d.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
```

### Comparing `python-manilaclient-4.7.0/python_manilaclient.egg-info/entry_points.txt` & `python-manilaclient-4.8.0/python_manilaclient.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/rally-jobs/rally-manila-no-ss.yaml` & `python-manilaclient-4.8.0/rally-jobs/rally-manila-no-ss.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/rally-jobs/rally-manila.yaml` & `python-manilaclient-4.8.0/rally-jobs/rally-manila.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml` & `python-manilaclient-4.8.0/releasenotes/notes/add-share-network-sec-service-add-update-to-in-use-networks-ec7a60d07ebceaf4.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/releasenotes/notes/deprecate-manila-shell-0061cbcab5d3d75b.yaml` & `python-manilaclient-4.8.0/releasenotes/notes/deprecate-manila-shell-0061cbcab5d3d75b.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml` & `python-manilaclient-4.8.0/releasenotes/notes/deprecate-v1-a0cfa6fd723c2f46.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml` & `python-manilaclient-4.8.0/releasenotes/notes/manila-openstackclient-bf61ceb270d3afb7.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml` & `python-manilaclient-4.8.0/releasenotes/notes/newton-migration-improvements-166a03472948bdef.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml` & `python-manilaclient-4.8.0/releasenotes/notes/remove-experimental-flag-from-share-groups-feature-dcf2b0b67fe4cac4.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml` & `python-manilaclient-4.8.0/releasenotes/notes/share-network-multiple-subnets-732309abfbf5987c.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/releasenotes/source/conf.py` & `python-manilaclient-4.8.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/requirements.txt` & `python-manilaclient-4.8.0/requirements.txt`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/roles/populate-manilaclient-config/README.rst` & `python-manilaclient-4.8.0/roles/populate-manilaclient-config/README.rst`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/roles/populate-manilaclient-config/tasks/main.yaml` & `python-manilaclient-4.8.0/roles/populate-manilaclient-config/tasks/main.yaml`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/run_tests.sh` & `python-manilaclient-4.8.0/run_tests.sh`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/setup.cfg` & `python-manilaclient-4.8.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 	License :: OSI Approved :: Apache Software License
 	Operating System :: OS Independent
 	Programming Language :: Python
 	Programming Language :: Python :: 3 :: Only
 	Programming Language :: Python :: 3
 	Programming Language :: Python :: 3.8
 	Programming Language :: Python :: 3.9
+	Programming Language :: Python :: 3.10
+	Programming Language :: Python :: 3.11
 
 [files]
 packages = 
 	manilaclient
 
 [entry_points]
 console_scripts =
```

### Comparing `python-manilaclient-4.7.0/setup.py` & `python-manilaclient-4.8.0/setup.py`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/tox.ini` & `python-manilaclient-4.8.0/tox.ini`

 * *Files identical despite different names*

### Comparing `python-manilaclient-4.7.0/zuul.d/python-manilaclient-jobs.yaml` & `python-manilaclient-4.8.0/zuul.d/python-manilaclient-jobs.yaml`

 * *Files identical despite different names*

