# Comparing `tmp/softlayer-6.2.1.tar.gz` & `tmp/softlayer-6.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "softlayer-6.2.1.tar", last modified: Mon May 13 21:44:36 2024, max compression
+gzip compressed data, was "softlayer-6.2.2.tar", last modified: Thu May 16 14:42:17 2024, max compression
```

## Comparing `softlayer-6.2.1.tar` & `softlayer-6.2.2.tar`

### file list

```diff
@@ -1,678 +1,678 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.959179 softlayer-6.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-13 21:44:33.000000 softlayer-6.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-13 21:44:33.000000 softlayer-6.2.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-05-13 21:44:36.959179 softlayer-6.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-05-13 21:44:33.000000 softlayer-6.2.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.855179 softlayer-6.2.1/SoftLayer/
--rw-r--r--   0 runner    (1001) docker     (127)    33205 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/API.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.859179 softlayer-6.2.1/SoftLayer/CLI/
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.863179 softlayer-6.2.1/SoftLayer/CLI/account/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/account/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/account/billing_items.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/account/cancel_item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/account/event_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/account/events.py
--rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/account/hook_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/account/hook_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/account/hooks.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/account/invoice_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/account/invoices.py
--rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/account/item_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/account/licenses.py
--rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/account/orders.py
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/account/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.863179 softlayer-6.2.1/SoftLayer/CLI/bandwidth/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/bandwidth/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/bandwidth/pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/bandwidth/pools_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/bandwidth/pools_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/bandwidth/pools_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/bandwidth/pools_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/bandwidth/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.867179 softlayer-6.2.1/SoftLayer/CLI/block/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.867179 softlayer-6.2.1/SoftLayer/CLI/block/access/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/access/authorize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/access/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/access/password.py
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/access/revoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/duplicate_convert_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/lun.py
--rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/modify.py
--rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/object_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/object_storage_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/object_storage_permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5249 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/order.py
--rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/refresh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.867179 softlayer-6.2.1/SoftLayer/CLI/block/replication/
--rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/replication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/replication/disaster_recovery_failover.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/replication/failback.py
--rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/replication/failover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/replication/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/replication/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/replication/partners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/set_note.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.871179 softlayer-6.2.1/SoftLayer/CLI/block/snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/snapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/snapshot/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/snapshot/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/snapshot/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/snapshot/disable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/snapshot/enable.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/snapshot/get_notify_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/snapshot/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/snapshot/order.py
--rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/snapshot/restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/snapshot/schedule_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/snapshot/set_notify_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.871179 softlayer-6.2.1/SoftLayer/CLI/block/subnets/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/subnets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/subnets/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/subnets/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/block/subnets/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/call_api.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.871179 softlayer-6.2.1/SoftLayer/CLI/cdn/
--rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/cdn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/cdn/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/cdn/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/cdn/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/cdn/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/cdn/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/cdn/origin_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/cdn/origin_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/cdn/origin_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/cdn/purge.py
--rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/columns.py
--rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/command.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.871179 softlayer-6.2.1/SoftLayer/CLI/config/
--rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/config/setup.py
--rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/config/show.py
--rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/custom_types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.875179 softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/cancel_guests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/list_guests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.875179 softlayer-6.2.1/SoftLayer/CLI/dns/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dns/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dns/record_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dns/record_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dns/record_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dns/record_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dns/zone_create.py
--rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dns/zone_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dns/zone_import.py
--rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dns/zone_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/dns/zone_print.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.875179 softlayer-6.2.1/SoftLayer/CLI/email/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/email/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/email/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/email/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/email/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/environment.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.875179 softlayer-6.2.1/SoftLayer/CLI/event_log/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/event_log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/event_log/get.py
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/event_log/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.879179 softlayer-6.2.1/SoftLayer/CLI/file/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.879179 softlayer-6.2.1/SoftLayer/CLI/file/access/
--rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/access/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/access/authorize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/access/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/access/revoke.py
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/convert.py
--rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/count.py
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/duplicate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/duplicate_convert_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/modify.py
--rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5674 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/refresh.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.879179 softlayer-6.2.1/SoftLayer/CLI/file/replication/
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/replication/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/replication/disaster_recovery_failover.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/replication/failback.py
--rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/replication/failover.py
--rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/replication/locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/replication/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/replication/partners.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/set_note.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.883179 softlayer-6.2.1/SoftLayer/CLI/file/snapshot/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/snapshot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/snapshot/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/snapshot/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/snapshot/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/snapshot/disable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/snapshot/enable.py
--rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/snapshot/get_notify_status.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/snapshot/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/snapshot/order.py
--rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/snapshot/restore.py
--rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/snapshot/schedule_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/file/snapshot/set_notify_status.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.883179 softlayer-6.2.1/SoftLayer/CLI/firewall/
--rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/firewall/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2041 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/firewall/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/firewall/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     4386 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/firewall/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/firewall/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/firewall/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/firewall/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/formatting.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.883179 softlayer-6.2.1/SoftLayer/CLI/globalip/
--rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/globalip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/globalip/assign.py
--rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/globalip/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/globalip/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/globalip/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/globalip/unassign.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.887179 softlayer-6.2.1/SoftLayer/CLI/hardware/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/authorize_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/cancel_reasons.py
--rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/create_credential.py
--rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/notification_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/notification_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/power.py
--rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/ready.py
--rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/reflash_firmware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/reload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/sensor.py
--rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/toggle_ipmi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/update_firmware.py
--rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/vlan_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/vlan_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/hardware/vlan_trunkable.py
--rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.891179 softlayer-6.2.1/SoftLayer/CLI/image/
--rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/image/datacenter.py
--rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/image/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/image/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/image/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/image/export.py
--rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/image/import.py
--rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/image/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/image/share.py
--rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/image/share_deny.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.891179 softlayer-6.2.1/SoftLayer/CLI/licenses/
--rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/licenses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/licenses/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/licenses/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/licenses/create_options.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.891179 softlayer-6.2.1/SoftLayer/CLI/loadbal/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/loadbal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/loadbal/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/loadbal/health.py
--rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/loadbal/layer7_policy_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/loadbal/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/loadbal/members.py
--rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/loadbal/ns_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/loadbal/ns_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/loadbal/order.py
--rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/loadbal/pools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/loadbal/protocol_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/loadbal/protocol_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/loadbal/protocol_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/login.py
--rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/metadata.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.895179 softlayer-6.2.1/SoftLayer/CLI/nas/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/nas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/nas/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/nas/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.895179 softlayer-6.2.1/SoftLayer/CLI/object_storage/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/object_storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/object_storage/cancel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.895179 softlayer-6.2.1/SoftLayer/CLI/object_storage/credential/
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/object_storage/credential/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/object_storage/credential/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/object_storage/credential/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/object_storage/credential/limit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/object_storage/credential/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/object_storage/list_accounts.py
--rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/object_storage/list_endpoints.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.899179 softlayer-6.2.1/SoftLayer/CLI/order/
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/cancelation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/category_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/item_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/package_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/package_locations.py
--rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/place.py
--rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/place_quote.py
--rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/preset_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/quote.py
--rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/quote_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/quote_detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/quote_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/order/quote_save.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.899179 softlayer-6.2.1/SoftLayer/CLI/report/
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/report/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/report/dc_closures.py
--rw-r--r--   0 runner    (1001) docker     (127)    25519 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/routes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/search.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.899179 softlayer-6.2.1/SoftLayer/CLI/security/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/security/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/security/cert_add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/security/cert_download.py
--rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/security/cert_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/security/cert_list.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/security/cert_remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/security/sshkey_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/security/sshkey_edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/security/sshkey_list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/security/sshkey_print.py
--rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/security/sshkey_remove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.899179 softlayer-6.2.1/SoftLayer/CLI/securitygroup/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/securitygroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/securitygroup/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/securitygroup/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/securitygroup/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/securitygroup/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/securitygroup/event_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/securitygroup/interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/securitygroup/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/securitygroup/rule.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.899179 softlayer-6.2.1/SoftLayer/CLI/sshkey/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/sshkey/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.903179 softlayer-6.2.1/SoftLayer/CLI/ssl/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/ssl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/storage_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.903179 softlayer-6.2.1/SoftLayer/CLI/subnet/
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/subnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/subnet/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/subnet/clear_route.py
--rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/subnet/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/subnet/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/subnet/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/subnet/edit_ip.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/subnet/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/subnet/lookup.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/subnet/route.py
--rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/summary.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.903179 softlayer-6.2.1/SoftLayer/CLI/tags/
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/tags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/tags/cleanup.py
--rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/tags/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/tags/details.py
--rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/tags/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/tags/set.py
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/tags/taggable.py
--rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/template.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.907179 softlayer-6.2.1/SoftLayer/CLI/ticket/
--rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/ticket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/ticket/attach.py
--rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/ticket/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/ticket/detach.py
--rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/ticket/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/ticket/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/ticket/subjects.py
--rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/ticket/summary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/ticket/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/ticket/upload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.907179 softlayer-6.2.1/SoftLayer/CLI/user/
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/apikey.py
--rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/create.py
--rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/device_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/edit_details.py
--rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/edit_notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/edit_permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/grant_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/list.py
--rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/permissions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/remove_access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/vpn_enable_or_disable.py
--rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/vpn_manual.py
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/vpn_password.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/user/vpn_subnet.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.911179 softlayer-6.2.1/SoftLayer/CLI/virt/
--rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/access.py
--rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/authorize_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/billing.py
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/cancel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.915179 softlayer-6.2.1/SoftLayer/CLI/virt/capacity/
--rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/capacity/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/capacity/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/capacity/create_guest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/capacity/create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/capacity/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/capacity/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/capture.py
--rw-r--r--   0 runner    (1001) docker     (127)    14724 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/create.py
--rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/credentials.py
--rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/migrate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/monitoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/notification_add.py
--rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/notification_delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/notifications.py
--rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/os_available.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.915179 softlayer-6.2.1/SoftLayer/CLI/virt/placementgroup/
--rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/placementgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/placementgroup/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/placementgroup/create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/placementgroup/delete.py
--rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/placementgroup/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/placementgroup/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/power.py
--rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/ready.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/reload.py
--rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/upgrade.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/virt/usage.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.915179 softlayer-6.2.1/SoftLayer/CLI/vlan/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vlan/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vlan/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vlan/create.py
--rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vlan/create_options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vlan/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vlan/edit.py
--rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vlan/list.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.915179 softlayer-6.2.1/SoftLayer/CLI/vpn/
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.919179 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/cancel.py
--rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/detail.py
--rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/list.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/order.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.919179 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/subnet/
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/subnet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/subnet/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/subnet/remove.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.919179 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/translation/
--rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/translation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/translation/add.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/translation/remove.py
--rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/translation/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/update.py
--rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)     4490 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/config.py
--rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/consts.py
--rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/decoration.py
--rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.931179 softlayer-6.2.1/SoftLayer/fixtures/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/BluePages_Search.py
--rw-r--r--   0 runner    (1001) docker     (127)    44611 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Account.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Billing_Invoice.py
--rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Billing_Invoice_Item.py
--rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Billing_Item.py
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Billing_Item_Cancellation_Request.py
--rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Billing_Order.py
--rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Billing_Order_Quote.py
--rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Dns_Domain.py
--rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Dns_Domain_ResourceRecord.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Email_Subscription.py
--rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Event_Log.py
--rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)    14237 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Hardware_Server.py
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Location.py
--rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Location_Datacenter.py
--rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Location_Group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Metric_Tracking_Object.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Health_Check_Type.py
--rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Method.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Type.py
--rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Service.py
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Service_Group.py
--rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualServer.py
--rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Bandwidth_Version1_Allotment.py
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Cache_Purge.py
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping_Path.py
--rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Component.py
--rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Component_Firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Firewall_Update_Request.py
--rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_LBaaS_HealthMonitor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_LBaaS_L7Pool.py
--rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Listener.py
--rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_LBaaS_LoadBalancer.py
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Member.py
--rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Message_Delivery_Email_Sendgrid.py
--rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Pod.py
--rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_SecurityGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Service_Vpn_Overrides.py
--rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Storage_Allowed_Host.py
--rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Storage_Hub_Cleversafe_Account.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Storage_Iscsi.py
--rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Subnet.py
--rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress_Global.py
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Subnet_Rwhois_Data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Vlan.py
--rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Vlan_Firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Notification_Occurrence_Event.py
--rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Product_Order.py
--rw-r--r--   0 runner    (1001) docker     (127)    75145 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Product_Package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Product_Package_Preset.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Provisioning_Hook.py
--rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Provisioning_Maintenance_Window.py
--rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Resource_Metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    16122 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Scale_Group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Scale_Policy.py
--rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Search.py
--rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Security_Certificate.py
--rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Security_Ssh_Key.py
--rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Software_AccountLicense.py
--rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Software_Component_Password.py
--rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Tag.py
--rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Ticket.py
--rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Ticket_Subject.py
--rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_User_Customer.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_User_Customer_CustomerPermission_Permission.py
--rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Virtual_Guest.py
--rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_User_Permission_Action.py
--rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Virtual_DedicatedHost.py
--rw-r--r--   0 runner    (1001) docker     (127)    29326 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Virtual_Guest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Virtual_Guest_Block_Device_Template_Group.py
--rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Virtual_Host.py
--rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup_Rule.py
--rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Virtual_ReservedCapacityGroup.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/fixtures/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.939180 softlayer-6.2.1/SoftLayer/managers/
--rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/account.py
--rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/bandwidth.py
--rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/block.py
--rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/cdn.py
--rw-r--r--   0 runner    (1001) docker     (127)    19234 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/dedicated_host.py
--rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/dns.py
--rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/email.py
--rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/event_log.py
--rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/file.py
--rw-r--r--   0 runner    (1001) docker     (127)    13364 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/firewall.py
--rw-r--r--   0 runner    (1001) docker     (127)    60808 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/hardware.py
--rw-r--r--   0 runner    (1001) docker     (127)    10000 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/image.py
--rw-r--r--   0 runner    (1001) docker     (127)    15244 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/ipsec.py
--rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/license.py
--rw-r--r--   0 runner    (1001) docker     (127)    13010 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/load_balancer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/metadata.py
--rw-r--r--   0 runner    (1001) docker     (127)    35045 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/network.py
--rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/object_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    33118 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/ordering.py
--rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/search.py
--rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/sshkey.py
--rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/ssl.py
--rw-r--r--   0 runner    (1001) docker     (127)    23199 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)    42269 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/storage_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/tags.py
--rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/ticket.py
--rw-r--r--   0 runner    (1001) docker     (127)    20345 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/user.py
--rw-r--r--   0 runner    (1001) docker     (127)    62894 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/vs.py
--rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/vs_capacity.py
--rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/managers/vs_placement.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.939180 softlayer-6.2.1/SoftLayer/shell/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/shell/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/shell/cmd_env.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/shell/cmd_exit.py
--rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/shell/cmd_help.py
--rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/shell/completer.py
--rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/shell/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/shell/routes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.939180 softlayer-6.2.1/SoftLayer/testing/
--rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/testing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/testing/xmlrpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.943179 softlayer-6.2.1/SoftLayer/transports/
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/transports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/transports/debug.py
--rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/transports/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/transports/rest.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/transports/timing.py
--rw-r--r--   0 runner    (1001) docker     (127)     4635 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/transports/transport.py
--rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/transports/xmlrpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    15411 2024-05-13 21:44:33.000000 softlayer-6.2.1/SoftLayer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.955180 softlayer-6.2.1/SoftLayer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-05-13 21:44:36.000000 softlayer-6.2.1/SoftLayer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    22925 2024-05-13 21:44:36.000000 softlayer-6.2.1/SoftLayer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:44:36.000000 softlayer-6.2.1/SoftLayer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-13 21:44:36.000000 softlayer-6.2.1/SoftLayer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-13 21:44:36.000000 softlayer-6.2.1/SoftLayer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-13 21:44:36.000000 softlayer-6.2.1/SoftLayer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-13 21:44:36.000000 softlayer-6.2.1/SoftLayer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-13 21:44:36.959179 softlayer-6.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-13 21:44:33.000000 softlayer-6.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.851179 softlayer-6.2.1/tests/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.943179 softlayer-6.2.1/tests/CLI/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/core_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/custom_types_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/environment_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/formatting_table_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/helper_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.951180 softlayer-6.2.1/tests/CLI/modules/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/account_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/bandwidth_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    43925 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/block_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12903 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/call_api_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/cdn_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/config_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/dedicatedhost_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/dns_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/email_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/event_log_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    36599 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/file_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/firewall_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/globalip_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/image_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    27405 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/ipsec_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/licenses_test.py
--rw-r--r--   0 runner    (1001) docker     (127)    15854 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/loadbal_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/nas_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/object_storage_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/order_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/report_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/search_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/security_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/securitygroup_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/sshkey_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/ssl_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/subnet_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/summary_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/tag_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/ticket_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    20619 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/user_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    15070 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/vlan_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.951180 softlayer-6.2.1/tests/CLI/modules/vs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/vs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/vs/vs_capacity_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    33577 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/vs/vs_create_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/vs/vs_placement_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    43881 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/CLI/modules/vs/vs_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.955180 softlayer-6.2.1/tests/managers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/account_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/bandwidth_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    42152 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/block_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/cdn_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    24093 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/dedicated_host_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/dns_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/email_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/event_log_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    34792 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/file_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/firewall_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    42426 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/hardware_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/image_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/ipsec_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/loadbal_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/metadata_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    28050 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/network_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/object_storage_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    40766 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/ordering_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/search_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/sshkey_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/ssl_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/storage_generic_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)   142912 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/storage_utils_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/tag_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/ticket_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    15851 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/user_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.955180 softlayer-6.2.1/tests/managers/vs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/vs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/vs/vs_capacity_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/vs/vs_order_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/vs/vs_placement_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    45298 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/vs/vs_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/managers/vs/vs_waiting_for_ready_tests.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:36.955180 softlayer-6.2.1/tests/transports/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/transports/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/transports/debug_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    11809 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/transports/rest_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/transports/transport_tests.py
--rw-r--r--   0 runner    (1001) docker     (127)    14582 2024-05-13 21:44:33.000000 softlayer-6.2.1/tests/transports/xmlrpc_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.333686 softlayer-6.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1093 2024-05-16 14:42:11.000000 softlayer-6.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 14:42:11.000000 softlayer-6.2.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-05-16 14:42:17.333686 softlayer-6.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6609 2024-05-16 14:42:11.000000 softlayer-6.2.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.237686 softlayer-6.2.2/SoftLayer/
+-rw-r--r--   0 runner    (1001) docker     (127)    33205 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/API.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.241685 softlayer-6.2.2/SoftLayer/CLI/
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.245685 softlayer-6.2.2/SoftLayer/CLI/account/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/account/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/account/billing_items.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/account/cancel_item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2436 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/account/event_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5144 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/account/events.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1014 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/account/hook_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      724 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/account/hook_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      649 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/account/hooks.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/account/invoice_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1749 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/account/invoices.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2236 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/account/item_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1914 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/account/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2219 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/account/orders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/account/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.245685 softlayer-6.2.2/SoftLayer/CLI/bandwidth/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/bandwidth/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2467 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/bandwidth/pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2743 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/bandwidth/pools_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      525 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/bandwidth/pools_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3447 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/bandwidth/pools_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1568 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/bandwidth/pools_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3868 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/bandwidth/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.249686 softlayer-6.2.2/SoftLayer/CLI/block/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.249686 softlayer-6.2.2/SoftLayer/CLI/block/access/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/access/authorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1958 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/access/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      887 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/access/password.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/access/revoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1811 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1601 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4914 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4699 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/duplicate_convert_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1817 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3474 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1190 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/lun.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2755 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)      966 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/object_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/object_storage_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1662 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/object_storage_permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5778 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5264 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      944 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/refresh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.249686 softlayer-6.2.2/SoftLayer/CLI/block/replication/
+-rw-r--r--   0 runner    (1001) docker     (127)       41 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/replication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2141 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/replication/disaster_recovery_failover.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/replication/failback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      763 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/replication/failover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/replication/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3254 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/replication/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/replication/partners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1022 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/set_note.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.253686 softlayer-6.2.2/SoftLayer/CLI/block/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/snapshot/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/snapshot/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      531 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/snapshot/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1017 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/snapshot/disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2474 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/snapshot/enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/snapshot/get_notify_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1737 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/snapshot/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2412 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/snapshot/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      782 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/snapshot/restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/snapshot/schedule_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/snapshot/set_notify_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.253686 softlayer-6.2.2/SoftLayer/CLI/block/subnets/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/subnets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/subnets/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1460 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/subnets/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/block/subnets/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7255 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/call_api.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.253686 softlayer-6.2.2/SoftLayer/CLI/cdn/
+-rw-r--r--   0 runner    (1001) docker     (127)       79 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/cdn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3091 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/cdn/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/cdn/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1615 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/cdn/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4106 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/cdn/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1271 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/cdn/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4546 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/cdn/origin_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      755 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/cdn/origin_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      573 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/cdn/origin_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/cdn/purge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2305 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/columns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9486 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/command.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.253686 softlayer-6.2.2/SoftLayer/CLI/config/
+-rw-r--r--   0 runner    (1001) docker     (127)     1625 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10609 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/config/setup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      462 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/config/show.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7555 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/custom_types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.253686 softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      802 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/cancel_guests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4016 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2345 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2493 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2716 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/list_guests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.257686 softlayer-6.2.2/SoftLayer/CLI/dns/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dns/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3639 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dns/record_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1538 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dns/record_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1600 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dns/record_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      712 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dns/record_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dns/zone_create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      774 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dns/zone_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4088 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dns/zone_import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1276 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dns/zone_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      634 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/dns/zone_print.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.257686 softlayer-6.2.2/SoftLayer/CLI/email/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/email/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1771 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/email/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1405 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/email/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2680 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/email/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8673 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/environment.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.257686 softlayer-6.2.2/SoftLayer/CLI/event_log/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/event_log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3540 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/event_log/get.py
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/event_log/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.261686 softlayer-6.2.2/SoftLayer/CLI/file/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.261686 softlayer-6.2.2/SoftLayer/CLI/file/access/
+-rw-r--r--   0 runner    (1001) docker     (127)       35 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/access/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2422 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/access/authorize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1787 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/access/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2208 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/access/revoke.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/convert.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1519 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/count.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4948 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/duplicate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1007 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/duplicate_convert_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1806 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3446 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2804 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/modify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4711 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5549 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1010 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/refresh.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.261686 softlayer-6.2.2/SoftLayer/CLI/file/replication/
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/replication/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/replication/disaster_recovery_failover.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/replication/failback.py
+-rw-r--r--   0 runner    (1001) docker     (127)      943 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/replication/failover.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1772 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/replication/locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3500 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/replication/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/replication/partners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/set_note.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.265686 softlayer-6.2.2/SoftLayer/CLI/file/snapshot/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/snapshot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1744 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/snapshot/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1080 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/snapshot/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      542 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/snapshot/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1161 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/snapshot/disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2649 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/snapshot/enable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      790 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/snapshot/get_notify_status.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/snapshot/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2055 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/snapshot/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)      925 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/snapshot/restore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2410 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/snapshot/schedule_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/file/snapshot/set_notify_status.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.265686 softlayer-6.2.2/SoftLayer/CLI/firewall/
+-rw-r--r--   0 runner    (1001) docker     (127)      487 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/firewall/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2053 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/firewall/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1194 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/firewall/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4371 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/firewall/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6485 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/firewall/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3837 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/firewall/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1768 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/firewall/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17836 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/formatting.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.265686 softlayer-6.2.2/SoftLayer/CLI/globalip/
+-rw-r--r--   0 runner    (1001) docker     (127)       74 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/globalip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1267 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/globalip/assign.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1031 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/globalip/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/globalip/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1565 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/globalip/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      597 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/globalip/unassign.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.269686 softlayer-6.2.2/SoftLayer/CLI/hardware/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      915 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/authorize_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1974 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1446 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1461 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      627 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/cancel_reasons.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5429 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/create_credential.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6630 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1294 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8169 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3030 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2893 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3782 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1336 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1282 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/notification_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/notification_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3576 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/power.py
+-rw-r--r--   0 runner    (1001) docker     (127)      851 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)      880 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/reflash_firmware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3796 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2892 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)      736 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/toggle_ipmi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1556 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/update_firmware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7557 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2437 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/vlan_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2605 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/vlan_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1242 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/hardware/vlan_trunkable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1435 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.273686 softlayer-6.2.2/SoftLayer/CLI/image/
+-rw-r--r--   0 runner    (1001) docker     (127)      848 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      830 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/image/datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      503 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/image/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4974 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/image/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/image/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/image/export.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2954 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/image/import.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2729 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/image/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      813 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/image/share.py
+-rw-r--r--   0 runner    (1001) docker     (127)      838 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/image/share_deny.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.273686 softlayer-6.2.2/SoftLayer/CLI/licenses/
+-rw-r--r--   0 runner    (1001) docker     (127)       70 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/licenses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/licenses/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1087 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/licenses/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1045 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/licenses/create_options.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.273686 softlayer-6.2.2/SoftLayer/CLI/loadbal/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/loadbal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/loadbal/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3352 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/loadbal/health.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1950 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/loadbal/layer7_policy_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1602 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/loadbal/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2136 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/loadbal/members.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1834 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/loadbal/ns_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1458 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/loadbal/ns_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7648 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/loadbal/order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9306 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/loadbal/pools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2577 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/loadbal/protocol_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      972 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/loadbal/protocol_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/loadbal/protocol_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2510 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/login.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2511 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/metadata.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.273686 softlayer-6.2.2/SoftLayer/CLI/nas/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/nas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      645 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/nas/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/nas/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.277686 softlayer-6.2.2/SoftLayer/CLI/object_storage/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/object_storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1421 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/object_storage/cancel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.277686 softlayer-6.2.2/SoftLayer/CLI/object_storage/credential/
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/object_storage/credential/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      940 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/object_storage/credential/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/object_storage/credential/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      768 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/object_storage/credential/limit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/object_storage/credential/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1004 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/object_storage/list_accounts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2835 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/object_storage/list_endpoints.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.277686 softlayer-6.2.2/SoftLayer/CLI/order/
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1039 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/cancelation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1338 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/category_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5686 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/item_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2506 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1584 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/package_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/package_locations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4459 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/place.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3809 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/place_quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6259 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/preset_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5656 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      551 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/quote_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/quote_detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/quote_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      853 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/order/quote_save.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.277686 softlayer-6.2.2/SoftLayer/CLI/report/
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/report/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5519 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/report/dc_closures.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25519 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/routes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2756 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/search.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.281686 softlayer-6.2.2/SoftLayer/CLI/security/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/security/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/security/cert_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1126 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/security/cert_download.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1487 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/security/cert_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1335 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/security/cert_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/security/cert_remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1321 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/security/sshkey_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      744 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/security/sshkey_edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      922 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/security/sshkey_list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/security/sshkey_print.py
+-rw-r--r--   0 runner    (1001) docker     (127)      703 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/security/sshkey_remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.281686 softlayer-6.2.2/SoftLayer/CLI/securitygroup/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/securitygroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1038 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/securitygroup/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      544 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/securitygroup/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2745 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/securitygroup/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      852 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/securitygroup/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      856 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/securitygroup/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5649 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/securitygroup/interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/securitygroup/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6250 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/securitygroup/rule.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.281686 softlayer-6.2.2/SoftLayer/CLI/sshkey/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/sshkey/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.281686 softlayer-6.2.2/SoftLayer/CLI/ssl/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/ssl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4782 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/storage_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.285686 softlayer-6.2.2/SoftLayer/CLI/subnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/subnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      734 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/subnet/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)      711 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/subnet/clear_route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2280 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/subnet/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4167 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/subnet/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1237 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/subnet/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)      688 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/subnet/edit_ip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/subnet/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2205 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/subnet/lookup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/subnet/route.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1230 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/summary.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.285686 softlayer-6.2.2/SoftLayer/CLI/tags/
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/tags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/tags/cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1082 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/tags/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/tags/details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2461 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/tags/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      995 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/tags/set.py
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/tags/taggable.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2193 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/template.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.285686 softlayer-6.2.2/SoftLayer/CLI/ticket/
+-rw-r--r--   0 runner    (1001) docker     (127)     2596 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/ticket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/ticket/attach.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2824 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/ticket/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1466 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/ticket/detach.py
+-rw-r--r--   0 runner    (1001) docker     (127)      826 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/ticket/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1614 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/ticket/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/ticket/subjects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1234 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/ticket/summary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/ticket/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1195 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/ticket/upload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.289686 softlayer-6.2.2/SoftLayer/CLI/user/
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/apikey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4003 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6394 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2635 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/device_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1388 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/edit_details.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1115 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/edit_notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1586 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/edit_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1717 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/grant_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1883 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)      954 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/permissions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1633 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/remove_access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1191 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/vpn_enable_or_disable.py
+-rw-r--r--   0 runner    (1001) docker     (127)      881 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/vpn_manual.py
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/vpn_password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/user/vpn_subnet.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.293686 softlayer-6.2.2/SoftLayer/CLI/virt/
+-rw-r--r--   0 runner    (1001) docker     (127)     1123 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      811 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/access.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1723 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/authorize_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4061 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/billing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      795 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/cancel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.293686 softlayer-6.2.2/SoftLayer/CLI/virt/capacity/
+-rw-r--r--   0 runner    (1001) docker     (127)     1782 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/capacity/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2258 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/capacity/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/capacity/create_guest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/capacity/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2152 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/capacity/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1207 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/capacity/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1420 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/capture.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14724 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11386 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)      986 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8526 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3014 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2491 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4297 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3616 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1310 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/monitoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/notification_add.py
+-rw-r--r--   0 runner    (1001) docker     (127)      547 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/notification_delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/notifications.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1167 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/os_available.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.293686 softlayer-6.2.2/SoftLayer/CLI/virt/placementgroup/
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/placementgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1412 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/placementgroup/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1256 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/placementgroup/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2374 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/placementgroup/delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1707 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/placementgroup/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)      961 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/placementgroup/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3503 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/power.py
+-rw-r--r--   0 runner    (1001) docker     (127)      778 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/ready.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3412 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2681 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/upgrade.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/virt/usage.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.297686 softlayer-6.2.2/SoftLayer/CLI/vlan/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vlan/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vlan/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2773 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vlan/create.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1101 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vlan/create_options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5475 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vlan/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1223 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vlan/edit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3119 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vlan/list.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.297686 softlayer-6.2.2/SoftLayer/CLI/vpn/
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.297686 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/cancel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1037 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7675 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/detail.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1201 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/list.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/order.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.297686 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/subnet/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/subnet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2942 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/subnet/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1675 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/subnet/remove.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.297686 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/translation/
+-rw-r--r--   0 runner    (1001) docker     (127)       37 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/translation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1447 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/translation/add.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/translation/remove.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/translation/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3687 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/update.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1251 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5564 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4492 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)      520 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/consts.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1874 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/decoration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2285 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.309686 softlayer-6.2.2/SoftLayer/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/BluePages_Search.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44611 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Billing_Invoice.py
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Billing_Invoice_Item.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2111 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Billing_Item.py
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Billing_Item_Cancellation_Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1940 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Billing_Order.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2949 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Billing_Order_Quote.py
+-rw-r--r--   0 runner    (1001) docker     (127)      606 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Dns_Domain.py
+-rw-r--r--   0 runner    (1001) docker     (127)      159 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Dns_Domain_ResourceRecord.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Email_Subscription.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5265 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Event_Log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3879 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14237 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Hardware_Server.py
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Location.py
+-rw-r--r--   0 runner    (1001) docker     (127)      229 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Location_Datacenter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2849 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Location_Group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1299 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Metric_Tracking_Object.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Health_Check_Type.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1657 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Method.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Type.py
+-rw-r--r--   0 runner    (1001) docker     (127)       40 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Service.py
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Service_Group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3115 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualServer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5328 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Bandwidth_Version1_Allotment.py
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Cache_Purge.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1258 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping_Path.py
+-rw-r--r--   0 runner    (1001) docker     (127)      253 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)       89 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Component.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3312 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Component_Firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      104 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Firewall_Update_Request.py
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_LBaaS_HealthMonitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_LBaaS_L7Pool.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3012 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Listener.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5814 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_LBaaS_LoadBalancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Member.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1325 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Message_Delivery_Email_Sendgrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      980 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Pod.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1831 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_SecurityGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Service_Vpn_Overrides.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10038 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1400 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Storage_Allowed_Host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2658 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Storage_Hub_Cleversafe_Account.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Storage_Iscsi.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1180 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Subnet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      834 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress_Global.py
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Subnet_Rwhois_Data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5088 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Vlan.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8928 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Vlan_Firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)      962 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Notification_Occurrence_Event.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9163 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Product_Order.py
+-rw-r--r--   0 runner    (1001) docker     (127)    75145 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Product_Package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1786 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Product_Package_Preset.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Provisioning_Hook.py
+-rw-r--r--   0 runner    (1001) docker     (127)      668 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Provisioning_Maintenance_Window.py
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Resource_Metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16122 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Scale_Group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Scale_Policy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2579 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1021 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Security_Certificate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      284 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Security_Ssh_Key.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1776 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Software_AccountLicense.py
+-rw-r--r--   0 runner    (1001) docker     (127)      317 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Software_Component_Password.py
+-rw-r--r--   0 runner    (1001) docker     (127)      749 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Tag.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1687 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)      361 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Ticket_Subject.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5396 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_User_Customer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_User_Customer_CustomerPermission_Permission.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1939 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1472 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Virtual_Guest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      913 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_User_Permission_Action.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3781 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Virtual_DedicatedHost.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29326 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Virtual_Guest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1465 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Virtual_Guest_Block_Device_Template_Group.py
+-rw-r--r--   0 runner    (1001) docker     (127)      989 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Virtual_Host.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1643 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup_Rule.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2309 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Virtual_ReservedCapacityGroup.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/fixtures/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.317686 softlayer-6.2.2/SoftLayer/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)     2381 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15614 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/account.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2748 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/bandwidth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8548 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/block.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14570 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/cdn.py
+-rw-r--r--   0 runner    (1001) docker     (127)    19313 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/dedicated_host.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10308 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/dns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2912 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/email.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3529 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/event_log.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6647 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13364 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/firewall.py
+-rw-r--r--   0 runner    (1001) docker     (127)    60832 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/hardware.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10000 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/image.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15244 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/ipsec.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2559 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/license.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13010 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/load_balancer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4821 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/metadata.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35045 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/network.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3504 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/object_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33118 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/ordering.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3901 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/search.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2798 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/sshkey.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3245 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/ssl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23199 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42269 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/storage_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9168 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/tags.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5407 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/ticket.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20345 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)    62894 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/vs.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7542 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/vs_capacity.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4582 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/managers/vs_placement.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.317686 softlayer-6.2.2/SoftLayer/shell/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/shell/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/shell/cmd_env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/shell/cmd_exit.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1103 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/shell/cmd_help.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2306 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/shell/completer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2846 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/shell/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      394 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/shell/routes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.317686 softlayer-6.2.2/SoftLayer/testing/
+-rw-r--r--   0 runner    (1001) docker     (127)     6628 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/testing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4144 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/testing/xmlrpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.317686 softlayer-6.2.2/SoftLayer/transports/
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1745 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/transports/debug.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1003 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/transports/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6061 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/transports/rest.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/transports/timing.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4644 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/transports/transport.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6724 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/transports/xmlrpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15411 2024-05-16 14:42:11.000000 softlayer-6.2.2/SoftLayer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.333686 softlayer-6.2.2/SoftLayer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7998 2024-05-16 14:42:17.000000 softlayer-6.2.2/SoftLayer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    22925 2024-05-16 14:42:17.000000 softlayer-6.2.2/SoftLayer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:42:17.000000 softlayer-6.2.2/SoftLayer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 14:42:17.000000 softlayer-6.2.2/SoftLayer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:42:17.000000 softlayer-6.2.2/SoftLayer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      110 2024-05-16 14:42:17.000000 softlayer-6.2.2/SoftLayer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 14:42:17.000000 softlayer-6.2.2/SoftLayer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      183 2024-05-16 14:42:17.333686 softlayer-6.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2042 2024-05-16 14:42:11.000000 softlayer-6.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.237686 softlayer-6.2.2/tests/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.321686 softlayer-6.2.2/tests/CLI/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4941 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/core_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1130 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/custom_types_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2733 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/environment_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/formatting_table_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15307 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/helper_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.325686 softlayer-6.2.2/tests/CLI/modules/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9126 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/account_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11282 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/bandwidth_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43925 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/block_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12903 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/call_api_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8504 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/cdn_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8172 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/config_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17724 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/dedicatedhost_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11932 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/dns_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1216 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/email_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3746 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/event_log_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36599 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/file_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8769 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/firewall_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3910 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/globalip_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3201 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/image_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27405 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/ipsec_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1339 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/licenses_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15854 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/loadbal_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/nas_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/object_storage_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    23416 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/order_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5911 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/report_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      599 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/search_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6075 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/security_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14341 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/securitygroup_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5030 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/sshkey_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1081 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/ssl_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7832 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/subnet_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/summary_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5533 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/tag_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15445 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/ticket_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20619 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/user_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15070 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/vlan_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.325686 softlayer-6.2.2/tests/CLI/modules/vs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/vs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4074 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/vs/vs_capacity_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33577 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/vs/vs_create_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5052 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/vs/vs_placement_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    43881 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/CLI/modules/vs/vs_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.329686 softlayer-6.2.2/tests/managers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7771 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/account_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)      825 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/bandwidth_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42152 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/block_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7552 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/cdn_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24093 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/dedicated_host_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7520 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/dns_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1308 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/email_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7922 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/event_log_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    34792 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/file_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12808 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/firewall_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    42426 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/hardware_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8859 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/image_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16589 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/ipsec_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9915 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/loadbal_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3093 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/metadata_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28050 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/network_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5032 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/object_storage_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40766 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/ordering_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2005 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/search_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2024 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/sshkey_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3052 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/ssl_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1380 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/storage_generic_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)   142912 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/storage_utils_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9155 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/tag_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4226 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/ticket_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15851 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/user_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.329686 softlayer-6.2.2/tests/managers/vs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/vs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8014 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/vs/vs_capacity_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10772 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/vs/vs_order_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2764 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/vs/vs_placement_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    45298 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/vs/vs_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6490 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/managers/vs/vs_waiting_for_ready_tests.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:17.333686 softlayer-6.2.2/tests/transports/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/transports/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2550 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/transports/debug_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11809 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/transports/rest_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/transports/transport_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14582 2024-05-16 14:42:11.000000 softlayer-6.2.2/tests/transports/xmlrpc_tests.py
```

### Comparing `softlayer-6.2.1/LICENSE` & `softlayer-6.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/PKG-INFO` & `softlayer-6.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SoftLayer
-Version: 6.2.1
+Version: 6.2.2
 Summary: A library for SoftLayer's API
 Home-page: https://github.com/SoftLayer/softlayer-python
 Author: SoftLayer, Inc., an IBM Company
 Author-email: SLDNDeveloperRelations@wwpdl.vnet.ibm.com
 License: MIT
 Keywords: softlayer,cloud,slcli,ibmcloud
 Classifier: Environment :: Console
```

### Comparing `softlayer-6.2.1/README.rst` & `softlayer-6.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/API.py` & `softlayer-6.2.2/SoftLayer/API.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/account/billing_items.py` & `softlayer-6.2.2/SoftLayer/CLI/account/billing_items.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/account/cancel_item.py` & `softlayer-6.2.2/SoftLayer/CLI/account/cancel_item.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/account/event_detail.py` & `softlayer-6.2.2/SoftLayer/CLI/account/event_detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/account/events.py` & `softlayer-6.2.2/SoftLayer/CLI/account/events.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/account/hook_create.py` & `softlayer-6.2.2/SoftLayer/CLI/account/hook_create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/account/hook_delete.py` & `softlayer-6.2.2/SoftLayer/CLI/account/hook_delete.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/account/hooks.py` & `softlayer-6.2.2/SoftLayer/CLI/account/hooks.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/account/invoice_detail.py` & `softlayer-6.2.2/SoftLayer/CLI/account/invoice_detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/account/invoices.py` & `softlayer-6.2.2/SoftLayer/CLI/account/invoices.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/account/item_detail.py` & `softlayer-6.2.2/SoftLayer/CLI/account/item_detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/account/licenses.py` & `softlayer-6.2.2/SoftLayer/CLI/account/licenses.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/account/orders.py` & `softlayer-6.2.2/SoftLayer/CLI/account/orders.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/account/summary.py` & `softlayer-6.2.2/SoftLayer/CLI/account/summary.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/bandwidth/pools.py` & `softlayer-6.2.2/SoftLayer/CLI/bandwidth/pools.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/bandwidth/pools_create.py` & `softlayer-6.2.2/SoftLayer/CLI/bandwidth/pools_create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/bandwidth/pools_delete.py` & `softlayer-6.2.2/SoftLayer/CLI/bandwidth/pools_delete.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/bandwidth/pools_detail.py` & `softlayer-6.2.2/SoftLayer/CLI/bandwidth/pools_detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/bandwidth/pools_edit.py` & `softlayer-6.2.2/SoftLayer/CLI/bandwidth/pools_edit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/bandwidth/summary.py` & `softlayer-6.2.2/SoftLayer/CLI/bandwidth/summary.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/access/authorize.py` & `softlayer-6.2.2/SoftLayer/CLI/block/access/authorize.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/access/list.py` & `softlayer-6.2.2/SoftLayer/CLI/block/access/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/access/password.py` & `softlayer-6.2.2/SoftLayer/CLI/block/access/password.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/access/revoke.py` & `softlayer-6.2.2/SoftLayer/CLI/block/access/revoke.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/cancel.py` & `softlayer-6.2.2/SoftLayer/CLI/block/cancel.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/convert.py` & `softlayer-6.2.2/SoftLayer/CLI/block/convert.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/count.py` & `softlayer-6.2.2/SoftLayer/CLI/block/count.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/block/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/duplicate.py` & `softlayer-6.2.2/SoftLayer/CLI/block/duplicate.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/duplicate_convert_status.py` & `softlayer-6.2.2/SoftLayer/CLI/block/duplicate_convert_status.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/limit.py` & `softlayer-6.2.2/SoftLayer/CLI/block/limit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/list.py` & `softlayer-6.2.2/SoftLayer/CLI/block/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/lun.py` & `softlayer-6.2.2/SoftLayer/CLI/block/lun.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/modify.py` & `softlayer-6.2.2/SoftLayer/CLI/block/modify.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/object_list.py` & `softlayer-6.2.2/SoftLayer/CLI/block/object_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/object_storage_detail.py` & `softlayer-6.2.2/SoftLayer/CLI/block/object_storage_detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/object_storage_permission.py` & `softlayer-6.2.2/SoftLayer/CLI/block/object_storage_permission.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/options.py` & `softlayer-6.2.2/SoftLayer/CLI/block/options.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/order.py` & `softlayer-6.2.2/SoftLayer/CLI/block/order.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,15 @@
     if service_offering != 'storage_as_a_service':
         click.secho(f"{service_offering} is a legacy storage offering", fg='red')
         if hourly_billing_flag:
             raise exceptions.CLIAbort(
                 'Hourly billing is only available for the storage_as_a_service service offering'
             )
 
+    order = {}
     if storage_type == 'performance':
         if iops is None:
             raise exceptions.CLIAbort('Option --iops required with Performance')
 
         if service_offering == 'performance' and snapshot_size is not None:
             raise exceptions.CLIAbort(
                 '--snapshot-size is not available for performance service offerings. '
```

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/refresh.py` & `softlayer-6.2.2/SoftLayer/CLI/block/refresh.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/replication/disaster_recovery_failover.py` & `softlayer-6.2.2/SoftLayer/CLI/block/replication/disaster_recovery_failover.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/replication/failback.py` & `softlayer-6.2.2/SoftLayer/CLI/block/replication/failback.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/replication/failover.py` & `softlayer-6.2.2/SoftLayer/CLI/block/replication/failover.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/replication/locations.py` & `softlayer-6.2.2/SoftLayer/CLI/block/replication/locations.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/replication/order.py` & `softlayer-6.2.2/SoftLayer/CLI/block/replication/order.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/replication/partners.py` & `softlayer-6.2.2/SoftLayer/CLI/block/replication/partners.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/set_note.py` & `softlayer-6.2.2/SoftLayer/CLI/block/set_note.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/snapshot/cancel.py` & `softlayer-6.2.2/SoftLayer/CLI/block/snapshot/cancel.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/snapshot/create.py` & `softlayer-6.2.2/SoftLayer/CLI/block/snapshot/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/snapshot/delete.py` & `softlayer-6.2.2/SoftLayer/CLI/block/snapshot/delete.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/snapshot/disable.py` & `softlayer-6.2.2/SoftLayer/CLI/block/snapshot/disable.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/snapshot/enable.py` & `softlayer-6.2.2/SoftLayer/CLI/block/snapshot/enable.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/snapshot/get_notify_status.py` & `softlayer-6.2.2/SoftLayer/CLI/block/snapshot/get_notify_status.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/snapshot/list.py` & `softlayer-6.2.2/SoftLayer/CLI/block/snapshot/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/snapshot/order.py` & `softlayer-6.2.2/SoftLayer/CLI/block/snapshot/order.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/snapshot/restore.py` & `softlayer-6.2.2/SoftLayer/CLI/block/snapshot/restore.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/snapshot/schedule_list.py` & `softlayer-6.2.2/SoftLayer/CLI/block/snapshot/schedule_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/snapshot/set_notify_status.py` & `softlayer-6.2.2/SoftLayer/CLI/block/snapshot/set_notify_status.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/subnets/assign.py` & `softlayer-6.2.2/SoftLayer/CLI/block/subnets/assign.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/subnets/list.py` & `softlayer-6.2.2/SoftLayer/CLI/block/subnets/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/block/subnets/remove.py` & `softlayer-6.2.2/SoftLayer/CLI/block/subnets/remove.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/call_api.py` & `softlayer-6.2.2/SoftLayer/CLI/call_api.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/cdn/create.py` & `softlayer-6.2.2/SoftLayer/CLI/cdn/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/cdn/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/cdn/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/cdn/edit.py` & `softlayer-6.2.2/SoftLayer/CLI/cdn/edit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/cdn/list.py` & `softlayer-6.2.2/SoftLayer/CLI/cdn/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/cdn/origin_add.py` & `softlayer-6.2.2/SoftLayer/CLI/cdn/origin_add.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/cdn/origin_list.py` & `softlayer-6.2.2/SoftLayer/CLI/cdn/origin_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/cdn/origin_remove.py` & `softlayer-6.2.2/SoftLayer/CLI/cdn/origin_remove.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/cdn/purge.py` & `softlayer-6.2.2/SoftLayer/CLI/cdn/purge.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/columns.py` & `softlayer-6.2.2/SoftLayer/CLI/columns.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/command.py` & `softlayer-6.2.2/SoftLayer/CLI/command.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/config/__init__.py` & `softlayer-6.2.2/SoftLayer/CLI/config/__init__.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/config/setup.py` & `softlayer-6.2.2/SoftLayer/CLI/config/setup.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/core.py` & `softlayer-6.2.2/SoftLayer/CLI/core.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/custom_types.py` & `softlayer-6.2.2/SoftLayer/CLI/custom_types.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/cancel.py` & `softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/cancel.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/cancel_guests.py` & `softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/cancel_guests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/create.py` & `softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/create_options.py` & `softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/create_options.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/list.py` & `softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dedicatedhost/list_guests.py` & `softlayer-6.2.2/SoftLayer/CLI/dedicatedhost/list_guests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dns/record_add.py` & `softlayer-6.2.2/SoftLayer/CLI/dns/record_add.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dns/record_edit.py` & `softlayer-6.2.2/SoftLayer/CLI/dns/record_edit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dns/record_list.py` & `softlayer-6.2.2/SoftLayer/CLI/dns/record_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dns/record_remove.py` & `softlayer-6.2.2/SoftLayer/CLI/dns/record_remove.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dns/zone_delete.py` & `softlayer-6.2.2/SoftLayer/CLI/dns/zone_delete.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dns/zone_import.py` & `softlayer-6.2.2/SoftLayer/CLI/dns/zone_import.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dns/zone_list.py` & `softlayer-6.2.2/SoftLayer/CLI/dns/zone_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/dns/zone_print.py` & `softlayer-6.2.2/SoftLayer/CLI/dns/zone_print.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/email/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/email/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/email/edit.py` & `softlayer-6.2.2/SoftLayer/CLI/email/edit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/email/list.py` & `softlayer-6.2.2/SoftLayer/CLI/email/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/environment.py` & `softlayer-6.2.2/SoftLayer/CLI/environment.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/event_log/get.py` & `softlayer-6.2.2/SoftLayer/CLI/event_log/get.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/event_log/types.py` & `softlayer-6.2.2/SoftLayer/CLI/event_log/types.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/exceptions.py` & `softlayer-6.2.2/SoftLayer/CLI/exceptions.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/access/authorize.py` & `softlayer-6.2.2/SoftLayer/CLI/file/access/authorize.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/access/list.py` & `softlayer-6.2.2/SoftLayer/CLI/file/access/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/access/revoke.py` & `softlayer-6.2.2/SoftLayer/CLI/file/access/revoke.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/cancel.py` & `softlayer-6.2.2/SoftLayer/CLI/file/cancel.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/convert.py` & `softlayer-6.2.2/SoftLayer/CLI/file/convert.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/count.py` & `softlayer-6.2.2/SoftLayer/CLI/file/count.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/file/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/duplicate.py` & `softlayer-6.2.2/SoftLayer/CLI/file/duplicate.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/duplicate_convert_status.py` & `softlayer-6.2.2/SoftLayer/CLI/file/duplicate_convert_status.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/limit.py` & `softlayer-6.2.2/SoftLayer/CLI/file/limit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/list.py` & `softlayer-6.2.2/SoftLayer/CLI/file/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/modify.py` & `softlayer-6.2.2/SoftLayer/CLI/file/modify.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/options.py` & `softlayer-6.2.2/SoftLayer/CLI/file/options.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/order.py` & `softlayer-6.2.2/SoftLayer/CLI/file/order.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,48 +8,38 @@
 from SoftLayer.CLI import formatting
 
 
 CONTEXT_SETTINGS = {'token_normalize_func': lambda x: x.upper()}
 
 
 @click.command(cls=SoftLayer.CLI.command.SLCommand, context_settings=CONTEXT_SETTINGS)
-@click.option('--storage-type',
-              help='Type of file storage volume',
-              type=click.Choice(['performance', 'endurance']),
-              required=True)
-@click.option('--size',
-              type=int,
-              help='Size of file storage volume in GB',
-              required=True)
-@click.option('--iops',
-              type=int,
+@click.option('--storage-type', required=True, type=click.Choice(['performance', 'endurance']),
+              help='Type of file storage volume')
+@click.option('--size', type=int, required=True,
+              help='Size of file storage volume in GB')
+@click.option('--iops', type=int,
               help="""Performance Storage IOPs. Options vary based on storage size.
 [required for storage-type performance]""")
-@click.option('--tier',
-              help='Endurance Storage Tier (IOP per GB) [required for storage-type endurance]',
-              type=click.Choice(['0.25', '2', '4', '10']))
-@click.option('-l', '--location',
-              help='Datacenter short name (e.g.: dal09)',
-              required=True)
-@click.option('--snapshot-size',
-              type=int,
+@click.option('--tier', type=click.Choice(['0.25', '2', '4', '10']),
+              help='Endurance Storage Tier (IOP per GB) [required for storage-type endurance]')
+@click.option('-l', '--location', required=True,
+              help='Datacenter short name (e.g.: dal09)')
+@click.option('--snapshot-size', type=int,
               help='Optional parameter for ordering snapshot '
               'space along with endurance file storage; specifies '
               'the size (in GB) of snapshot space to order')
 @click.option('--service-offering',
               help="""The service offering package to use for placing the order.
 [optional, default is \'storage_as_a_service\']. enterprise and performance are depreciated""",
               default='storage_as_a_service',
               type=click.Choice([
                   'storage_as_a_service',
                   'enterprise',
                   'performance']))
-@click.option('--billing',
-              type=click.Choice(['hourly', 'monthly']),
-              default='monthly',
+@click.option('--billing', type=click.Choice(['hourly', 'monthly']), default='monthly',
               help="Optional parameter for Billing rate (default to monthly)")
 @click.option('--force', default=False, is_flag=True, help="Force order file storage volume without confirmation")
 @environment.pass_env
 def cli(env, storage_type, size, iops, tier,
         location, snapshot_size, service_offering, billing, force):
     """Order a file storage volume.
 
@@ -79,14 +69,15 @@
     if service_offering != 'storage_as_a_service':
         click.secho(f'{service_offering} is a legacy storage offering', fg='red')
         if hourly_billing_flag:
             raise exceptions.CLIAbort(
                 'Hourly billing is only available for the storage_as_a_service service offering'
             )
 
+    order = {}
     if storage_type == 'performance':
         if iops is None:
             raise exceptions.CLIAbort('Option --iops required with Performance')
 
         if service_offering == 'performance' and snapshot_size is not None:
             raise exceptions.CLIAbort(
                 '--snapshot-size is not available for performance service offerings. '
```

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/refresh.py` & `softlayer-6.2.2/SoftLayer/CLI/file/refresh.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/replication/disaster_recovery_failover.py` & `softlayer-6.2.2/SoftLayer/CLI/file/replication/disaster_recovery_failover.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/replication/failback.py` & `softlayer-6.2.2/SoftLayer/CLI/file/replication/failback.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/replication/failover.py` & `softlayer-6.2.2/SoftLayer/CLI/file/replication/failover.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/replication/locations.py` & `softlayer-6.2.2/SoftLayer/CLI/file/replication/locations.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/replication/order.py` & `softlayer-6.2.2/SoftLayer/CLI/file/replication/order.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/replication/partners.py` & `softlayer-6.2.2/SoftLayer/CLI/file/replication/partners.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/set_note.py` & `softlayer-6.2.2/SoftLayer/CLI/file/set_note.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/snapshot/cancel.py` & `softlayer-6.2.2/SoftLayer/CLI/file/snapshot/cancel.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/snapshot/create.py` & `softlayer-6.2.2/SoftLayer/CLI/file/snapshot/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/snapshot/delete.py` & `softlayer-6.2.2/SoftLayer/CLI/file/snapshot/delete.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/snapshot/disable.py` & `softlayer-6.2.2/SoftLayer/CLI/file/snapshot/disable.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/snapshot/enable.py` & `softlayer-6.2.2/SoftLayer/CLI/file/snapshot/enable.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/snapshot/get_notify_status.py` & `softlayer-6.2.2/SoftLayer/CLI/file/snapshot/get_notify_status.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/snapshot/list.py` & `softlayer-6.2.2/SoftLayer/CLI/file/snapshot/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/snapshot/order.py` & `softlayer-6.2.2/SoftLayer/CLI/file/snapshot/order.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/snapshot/restore.py` & `softlayer-6.2.2/SoftLayer/CLI/file/snapshot/restore.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/snapshot/schedule_list.py` & `softlayer-6.2.2/SoftLayer/CLI/file/snapshot/schedule_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/file/snapshot/set_notify_status.py` & `softlayer-6.2.2/SoftLayer/CLI/file/snapshot/set_notify_status.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/firewall/add.py` & `softlayer-6.2.2/SoftLayer/CLI/firewall/add.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 def cli(env, target, firewall_type, high_availability, force):
     """Create new firewall.
 
     TARGET: Id of the server the firewall will protect
     """
 
     mgr = SoftLayer.FirewallManager(env.client)
-
+    pkg = {}
     if not env.skip_confirmations:
         if firewall_type == 'vlan':
             pkg = mgr.get_dedicated_package(ha_enabled=high_availability)
         elif firewall_type == 'vs':
             pkg = mgr.get_standard_package(target, is_virt=True)
         elif firewall_type == 'server':
             pkg = mgr.get_standard_package(target, is_virt=False)
```

### Comparing `softlayer-6.2.1/SoftLayer/CLI/firewall/cancel.py` & `softlayer-6.2.2/SoftLayer/CLI/firewall/cancel.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/firewall/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/firewall/detail.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,14 @@
             table = get_rules_table(rules)
 
         env.fout(table)
 
     else:
         click.secho('Invalid firewall type %s: firewall type should be either vlan, multiVlan, vs or server.'
                     % firewall_type, fg='red')
-        return
 
 
 def get_rules_table(rules):
     """Helper to format the rules into a table.
 
     :param list rules: A list containing the rules of the firewall
     :returns: a formatted table of the firewall rules
```

### Comparing `softlayer-6.2.1/SoftLayer/CLI/firewall/edit.py` & `softlayer-6.2.2/SoftLayer/CLI/firewall/edit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/firewall/list.py` & `softlayer-6.2.2/SoftLayer/CLI/firewall/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/firewall/monitoring.py` & `softlayer-6.2.2/SoftLayer/CLI/firewall/monitoring.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/formatting.py` & `softlayer-6.2.2/SoftLayer/CLI/formatting.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/globalip/assign.py` & `softlayer-6.2.2/SoftLayer/CLI/globalip/assign.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/globalip/cancel.py` & `softlayer-6.2.2/SoftLayer/CLI/globalip/cancel.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/globalip/create.py` & `softlayer-6.2.2/SoftLayer/CLI/globalip/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/globalip/list.py` & `softlayer-6.2.2/SoftLayer/CLI/globalip/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/globalip/unassign.py` & `softlayer-6.2.2/SoftLayer/CLI/globalip/unassign.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/authorize_storage.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/authorize_storage.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/bandwidth.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/bandwidth.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/billing.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/billing.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/cancel.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/cancel.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/cancel_reasons.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/cancel_reasons.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/create.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/create_credential.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/create_credential.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/create_options.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/create_options.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/credentials.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/credentials.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/dns.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/dns.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/edit.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/edit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/list.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/monitoring.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/monitoring.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/notification_add.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/notification_add.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/notification_delete.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/notification_delete.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/notifications.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/notifications.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/power.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/power.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/ready.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/ready.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/reflash_firmware.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/reflash_firmware.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/reload.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/reload.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/sensor.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/sensor.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/storage.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/storage.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/toggle_ipmi.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/toggle_ipmi.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/update_firmware.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/update_firmware.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/upgrade.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/upgrade.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/vlan_add.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/vlan_add.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/vlan_remove.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/vlan_remove.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/hardware/vlan_trunkable.py` & `softlayer-6.2.2/SoftLayer/CLI/hardware/vlan_trunkable.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/helpers.py` & `softlayer-6.2.2/SoftLayer/CLI/helpers.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/image/__init__.py` & `softlayer-6.2.2/SoftLayer/CLI/image/__init__.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/image/datacenter.py` & `softlayer-6.2.2/SoftLayer/CLI/image/datacenter.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/image/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/image/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/image/edit.py` & `softlayer-6.2.2/SoftLayer/CLI/image/edit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/image/export.py` & `softlayer-6.2.2/SoftLayer/CLI/image/export.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/image/import.py` & `softlayer-6.2.2/SoftLayer/CLI/image/import.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/image/list.py` & `softlayer-6.2.2/SoftLayer/CLI/image/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/image/share.py` & `softlayer-6.2.2/SoftLayer/CLI/image/share.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/image/share_deny.py` & `softlayer-6.2.2/SoftLayer/CLI/image/share_deny.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/licenses/cancel.py` & `softlayer-6.2.2/SoftLayer/CLI/licenses/cancel.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/licenses/create.py` & `softlayer-6.2.2/SoftLayer/CLI/licenses/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/licenses/create_options.py` & `softlayer-6.2.2/SoftLayer/CLI/licenses/create_options.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/loadbal/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/loadbal/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/loadbal/health.py` & `softlayer-6.2.2/SoftLayer/CLI/loadbal/health.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/loadbal/layer7_policy_list.py` & `softlayer-6.2.2/SoftLayer/CLI/loadbal/layer7_policy_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/loadbal/list.py` & `softlayer-6.2.2/SoftLayer/CLI/loadbal/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/loadbal/members.py` & `softlayer-6.2.2/SoftLayer/CLI/loadbal/members.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/loadbal/ns_detail.py` & `softlayer-6.2.2/SoftLayer/CLI/loadbal/ns_detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/loadbal/ns_list.py` & `softlayer-6.2.2/SoftLayer/CLI/loadbal/ns_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/loadbal/order.py` & `softlayer-6.2.2/SoftLayer/CLI/loadbal/order.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/loadbal/pools.py` & `softlayer-6.2.2/SoftLayer/CLI/loadbal/pools.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/loadbal/protocol_add.py` & `softlayer-6.2.2/SoftLayer/CLI/loadbal/protocol_add.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/loadbal/protocol_delete.py` & `softlayer-6.2.2/SoftLayer/CLI/loadbal/protocol_delete.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/loadbal/protocol_edit.py` & `softlayer-6.2.2/SoftLayer/CLI/loadbal/protocol_edit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/login.py` & `softlayer-6.2.2/SoftLayer/CLI/login.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/metadata.py` & `softlayer-6.2.2/SoftLayer/CLI/metadata.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/nas/credentials.py` & `softlayer-6.2.2/SoftLayer/CLI/nas/credentials.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/nas/list.py` & `softlayer-6.2.2/SoftLayer/CLI/nas/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/object_storage/cancel.py` & `softlayer-6.2.2/SoftLayer/CLI/object_storage/cancel.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/object_storage/credential/__init__.py` & `softlayer-6.2.2/SoftLayer/CLI/object_storage/credential/__init__.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/object_storage/credential/create.py` & `softlayer-6.2.2/SoftLayer/CLI/object_storage/credential/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/object_storage/credential/delete.py` & `softlayer-6.2.2/SoftLayer/CLI/object_storage/credential/delete.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/object_storage/credential/limit.py` & `softlayer-6.2.2/SoftLayer/CLI/object_storage/credential/limit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/object_storage/credential/list.py` & `softlayer-6.2.2/SoftLayer/CLI/object_storage/credential/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/object_storage/list_accounts.py` & `softlayer-6.2.2/SoftLayer/CLI/object_storage/list_accounts.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/object_storage/list_endpoints.py` & `softlayer-6.2.2/SoftLayer/CLI/object_storage/list_endpoints.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/order/cancelation.py` & `softlayer-6.2.2/SoftLayer/CLI/order/cancelation.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/order/category_list.py` & `softlayer-6.2.2/SoftLayer/CLI/order/category_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/order/item_list.py` & `softlayer-6.2.2/SoftLayer/CLI/order/item_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/order/lookup.py` & `softlayer-6.2.2/SoftLayer/CLI/order/lookup.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/order/package_list.py` & `softlayer-6.2.2/SoftLayer/CLI/order/package_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/order/package_locations.py` & `softlayer-6.2.2/SoftLayer/CLI/order/package_locations.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/order/place.py` & `softlayer-6.2.2/SoftLayer/CLI/order/place.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/order/place_quote.py` & `softlayer-6.2.2/SoftLayer/CLI/order/place_quote.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/order/preset_list.py` & `softlayer-6.2.2/SoftLayer/CLI/order/preset_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/order/quote.py` & `softlayer-6.2.2/SoftLayer/CLI/order/quote.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/order/quote_delete.py` & `softlayer-6.2.2/SoftLayer/CLI/order/quote_delete.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/order/quote_detail.py` & `softlayer-6.2.2/SoftLayer/CLI/order/quote_detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/order/quote_list.py` & `softlayer-6.2.2/SoftLayer/CLI/order/quote_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/order/quote_save.py` & `softlayer-6.2.2/SoftLayer/CLI/order/quote_save.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/report/dc_closures.py` & `softlayer-6.2.2/SoftLayer/CLI/report/dc_closures.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/routes.py` & `softlayer-6.2.2/SoftLayer/CLI/routes.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/search.py` & `softlayer-6.2.2/SoftLayer/CLI/search.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/security/cert_add.py` & `softlayer-6.2.2/SoftLayer/CLI/security/cert_add.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/security/cert_download.py` & `softlayer-6.2.2/SoftLayer/CLI/security/cert_download.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/security/cert_edit.py` & `softlayer-6.2.2/SoftLayer/CLI/security/cert_edit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/security/cert_list.py` & `softlayer-6.2.2/SoftLayer/CLI/security/cert_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/security/cert_remove.py` & `softlayer-6.2.2/SoftLayer/CLI/security/cert_remove.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/security/sshkey_add.py` & `softlayer-6.2.2/SoftLayer/CLI/security/sshkey_add.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/security/sshkey_edit.py` & `softlayer-6.2.2/SoftLayer/CLI/security/sshkey_edit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/security/sshkey_list.py` & `softlayer-6.2.2/SoftLayer/CLI/security/sshkey_list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/security/sshkey_print.py` & `softlayer-6.2.2/SoftLayer/CLI/security/sshkey_print.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/security/sshkey_remove.py` & `softlayer-6.2.2/SoftLayer/CLI/security/sshkey_remove.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/securitygroup/create.py` & `softlayer-6.2.2/SoftLayer/CLI/securitygroup/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/securitygroup/delete.py` & `softlayer-6.2.2/SoftLayer/CLI/securitygroup/delete.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/securitygroup/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/securitygroup/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/securitygroup/edit.py` & `softlayer-6.2.2/SoftLayer/CLI/securitygroup/edit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/securitygroup/event_log.py` & `softlayer-6.2.2/SoftLayer/CLI/securitygroup/event_log.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/securitygroup/interface.py` & `softlayer-6.2.2/SoftLayer/CLI/securitygroup/interface.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/securitygroup/list.py` & `softlayer-6.2.2/SoftLayer/CLI/securitygroup/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/securitygroup/rule.py` & `softlayer-6.2.2/SoftLayer/CLI/securitygroup/rule.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/storage_utils.py` & `softlayer-6.2.2/SoftLayer/CLI/storage_utils.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/subnet/cancel.py` & `softlayer-6.2.2/SoftLayer/CLI/subnet/cancel.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/subnet/clear_route.py` & `softlayer-6.2.2/SoftLayer/CLI/subnet/clear_route.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/subnet/create.py` & `softlayer-6.2.2/SoftLayer/CLI/subnet/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/subnet/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/subnet/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/subnet/edit.py` & `softlayer-6.2.2/SoftLayer/CLI/subnet/edit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/subnet/edit_ip.py` & `softlayer-6.2.2/SoftLayer/CLI/subnet/edit_ip.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/subnet/list.py` & `softlayer-6.2.2/SoftLayer/CLI/subnet/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/subnet/lookup.py` & `softlayer-6.2.2/SoftLayer/CLI/subnet/lookup.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/subnet/route.py` & `softlayer-6.2.2/SoftLayer/CLI/subnet/route.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/summary.py` & `softlayer-6.2.2/SoftLayer/CLI/summary.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/tags/cleanup.py` & `softlayer-6.2.2/SoftLayer/CLI/tags/cleanup.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/tags/delete.py` & `softlayer-6.2.2/SoftLayer/CLI/tags/delete.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/tags/details.py` & `softlayer-6.2.2/SoftLayer/CLI/tags/details.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/tags/list.py` & `softlayer-6.2.2/SoftLayer/CLI/tags/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/tags/set.py` & `softlayer-6.2.2/SoftLayer/CLI/tags/set.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/tags/taggable.py` & `softlayer-6.2.2/SoftLayer/CLI/tags/taggable.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/template.py` & `softlayer-6.2.2/SoftLayer/CLI/template.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/ticket/__init__.py` & `softlayer-6.2.2/SoftLayer/CLI/ticket/__init__.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/ticket/attach.py` & `softlayer-6.2.2/SoftLayer/CLI/ticket/attach.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/ticket/create.py` & `softlayer-6.2.2/SoftLayer/CLI/ticket/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/ticket/detach.py` & `softlayer-6.2.2/SoftLayer/CLI/ticket/detach.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/ticket/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/ticket/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/ticket/list.py` & `softlayer-6.2.2/SoftLayer/CLI/ticket/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/ticket/subjects.py` & `softlayer-6.2.2/SoftLayer/CLI/ticket/subjects.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/ticket/summary.py` & `softlayer-6.2.2/SoftLayer/CLI/ticket/summary.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/ticket/update.py` & `softlayer-6.2.2/SoftLayer/CLI/ticket/update.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/ticket/upload.py` & `softlayer-6.2.2/SoftLayer/CLI/ticket/upload.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/apikey.py` & `softlayer-6.2.2/SoftLayer/CLI/user/apikey.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/create.py` & `softlayer-6.2.2/SoftLayer/CLI/user/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/delete.py` & `softlayer-6.2.2/SoftLayer/CLI/user/delete.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/user/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/device_access.py` & `softlayer-6.2.2/SoftLayer/CLI/user/device_access.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/edit_details.py` & `softlayer-6.2.2/SoftLayer/CLI/user/edit_details.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/edit_notifications.py` & `softlayer-6.2.2/SoftLayer/CLI/user/edit_notifications.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/edit_permissions.py` & `softlayer-6.2.2/SoftLayer/CLI/user/edit_permissions.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/grant_access.py` & `softlayer-6.2.2/SoftLayer/CLI/user/grant_access.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/list.py` & `softlayer-6.2.2/SoftLayer/CLI/user/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/notifications.py` & `softlayer-6.2.2/SoftLayer/CLI/user/notifications.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/permissions.py` & `softlayer-6.2.2/SoftLayer/CLI/user/permissions.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/remove_access.py` & `softlayer-6.2.2/SoftLayer/CLI/user/remove_access.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/vpn_enable_or_disable.py` & `softlayer-6.2.2/SoftLayer/CLI/user/vpn_enable_or_disable.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/vpn_manual.py` & `softlayer-6.2.2/SoftLayer/CLI/user/vpn_manual.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/vpn_password.py` & `softlayer-6.2.2/SoftLayer/CLI/user/vpn_password.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/user/vpn_subnet.py` & `softlayer-6.2.2/SoftLayer/CLI/user/vpn_subnet.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/__init__.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/__init__.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/access.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/access.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/authorize_storage.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/authorize_storage.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/bandwidth.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/bandwidth.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/billing.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/billing.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/cancel.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/cancel.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/capacity/__init__.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/capacity/__init__.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/capacity/create.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/capacity/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/capacity/create_guest.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/capacity/create_guest.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/capacity/create_options.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/capacity/create_options.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/capacity/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/capacity/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/capacity/list.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/capacity/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/capture.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/capture.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/create.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/create_options.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/create_options.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/credentials.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/credentials.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/dns.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/dns.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/edit.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/edit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/list.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/migrate.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/migrate.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/monitoring.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/monitoring.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/notification_add.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/notification_add.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/notification_delete.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/notification_delete.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/notifications.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/notifications.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/os_available.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/os_available.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/placementgroup/__init__.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/placementgroup/__init__.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/placementgroup/create.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/placementgroup/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/placementgroup/create_options.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/placementgroup/create_options.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/placementgroup/delete.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/placementgroup/delete.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/placementgroup/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/placementgroup/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/placementgroup/list.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/placementgroup/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/power.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/power.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/ready.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/ready.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/reload.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/reload.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/storage.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/storage.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/upgrade.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/upgrade.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/virt/usage.py` & `softlayer-6.2.2/SoftLayer/CLI/virt/usage.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vlan/cancel.py` & `softlayer-6.2.2/SoftLayer/CLI/vlan/cancel.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vlan/create.py` & `softlayer-6.2.2/SoftLayer/CLI/vlan/create.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vlan/create_options.py` & `softlayer-6.2.2/SoftLayer/CLI/vlan/create_options.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vlan/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/vlan/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vlan/edit.py` & `softlayer-6.2.2/SoftLayer/CLI/vlan/edit.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vlan/list.py` & `softlayer-6.2.2/SoftLayer/CLI/vlan/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/cancel.py` & `softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/cancel.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/configure.py` & `softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/configure.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/detail.py` & `softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/detail.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/list.py` & `softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/list.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/order.py` & `softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/order.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/subnet/add.py` & `softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/subnet/add.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/subnet/remove.py` & `softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/subnet/remove.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/translation/add.py` & `softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/translation/add.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/translation/remove.py` & `softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/translation/remove.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/translation/update.py` & `softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/translation/update.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/CLI/vpn/ipsec/update.py` & `softlayer-6.2.2/SoftLayer/CLI/vpn/ipsec/update.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/__init__.py` & `softlayer-6.2.2/SoftLayer/__init__.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/auth.py` & `softlayer-6.2.2/SoftLayer/auth.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/config.py` & `softlayer-6.2.2/SoftLayer/config.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         'username': '',
         'api_key': '',
         'endpoint_url': '',
         'timeout': '0',
         'proxy': '',
         'userid': '',
         'access_token': '',
-        'verify': True
+        'verify': "True"
     })
     config.read(config_files)
 
     if config.has_section('softlayer'):
         r_config = {
             'endpoint_url': config.get('softlayer', 'endpoint_url'),
             'timeout': config.getfloat('softlayer', 'timeout'),
```

### Comparing `softlayer-6.2.1/SoftLayer/consts.py` & `softlayer-6.2.2/SoftLayer/consts.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """
     SoftLayer.consts
     ~~~~~~~~~~~~~~~~
     Contains constants used throughout the library
 
     :license: MIT, see LICENSE for more details.
 """
-VERSION = 'v6.2.1'
+VERSION = 'v6.2.2'
 API_PUBLIC_ENDPOINT = 'https://api.softlayer.com/xmlrpc/v3.1/'
 API_PRIVATE_ENDPOINT = 'https://api.service.softlayer.com/xmlrpc/v3.1/'
 API_PUBLIC_ENDPOINT_REST = 'https://api.softlayer.com/rest/v3.1/'
 API_PRIVATE_ENDPOINT_REST = 'https://api.service.softlayer.com/rest/v3.1/'
 USER_AGENT = "softlayer-python/%s" % VERSION
 CONFIG_FILE = "~/.softlayer"
```

### Comparing `softlayer-6.2.1/SoftLayer/decoration.py` & `softlayer-6.2.2/SoftLayer/decoration.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/exceptions.py` & `softlayer-6.2.2/SoftLayer/exceptions.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Account.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Account.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Billing_Invoice.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Billing_Invoice.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Billing_Item.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Billing_Item.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Billing_Item_Cancellation_Request.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Billing_Item_Cancellation_Request.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Billing_Order.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Billing_Order.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Billing_Order_Quote.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Billing_Order_Quote.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Dns_Domain.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Dns_Domain.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Event_Log.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Event_Log.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Hardware.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Hardware.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Hardware_Server.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Hardware_Server.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Location_Group.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Location_Group.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Metric_Tracking_Object.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Metric_Tracking_Object.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Method.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_Routing_Method.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Application_Delivery_Controller_LoadBalancer_VirtualIpAddress.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Bandwidth_Version1_Allotment.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Bandwidth_Version1_Allotment.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping_Path.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_CdnMarketplace_Configuration_Mapping_Path.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Component_Firewall.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Component_Firewall.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_LBaaS_L7Pool.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_LBaaS_L7Pool.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Listener.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_LBaaS_Listener.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_LBaaS_LoadBalancer.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_LBaaS_LoadBalancer.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Message_Delivery_Email_Sendgrid.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Message_Delivery_Email_Sendgrid.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Pod.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Pod.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_SecurityGroup.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_SecurityGroup.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Storage.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Storage.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Storage_Allowed_Host.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Storage_Allowed_Host.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Storage_Hub_Cleversafe_Account.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Storage_Hub_Cleversafe_Account.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Storage_Iscsi.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Storage_Iscsi.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Subnet.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Subnet.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Subnet_IpAddress.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Vlan.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Vlan.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Network_Vlan_Firewall.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Network_Vlan_Firewall.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Notification_Occurrence_Event.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Notification_Occurrence_Event.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Product_Order.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Product_Order.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Product_Package.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Product_Package.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Product_Package_Preset.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Product_Package_Preset.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Provisioning_Maintenance_Window.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Provisioning_Maintenance_Window.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Scale_Group.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Scale_Group.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Scale_Policy.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Scale_Policy.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Search.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Search.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Security_Certificate.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Security_Certificate.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Software_AccountLicense.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Software_AccountLicense.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Tag.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Tag.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Ticket.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Ticket.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_User_Customer.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_User_Customer.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_User_Customer_CustomerPermission_Permission.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_User_Customer_CustomerPermission_Permission.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Hardware.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Hardware.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Virtual_Guest.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_User_Customer_Notification_Virtual_Guest.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_User_Permission_Action.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_User_Permission_Action.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Virtual_DedicatedHost.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Virtual_DedicatedHost.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Virtual_Guest.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Virtual_Guest.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Virtual_Guest_Block_Device_Template_Group.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Virtual_Guest_Block_Device_Template_Group.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Virtual_Host.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Virtual_Host.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Virtual_PlacementGroup.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/fixtures/SoftLayer_Virtual_ReservedCapacityGroup.py` & `softlayer-6.2.2/SoftLayer/fixtures/SoftLayer_Virtual_ReservedCapacityGroup.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/__init__.py` & `softlayer-6.2.2/SoftLayer/managers/__init__.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/account.py` & `softlayer-6.2.2/SoftLayer/managers/account.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/bandwidth.py` & `softlayer-6.2.2/SoftLayer/managers/bandwidth.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/block.py` & `softlayer-6.2.2/SoftLayer/managers/block.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/cdn.py` & `softlayer-6.2.2/SoftLayer/managers/cdn.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/dedicated_host.py` & `softlayer-6.2.2/SoftLayer/managers/dedicated_host.py`

 * *Files 0% similar despite different names*

```diff
@@ -427,15 +427,17 @@
     def _get_backend_router(self, locations, item):
         """Returns valid router options for ordering a dedicated host."""
         mask = '''
             id,
             hostname
         '''
         cpu_count = item['capacity']
-
+        mem_capacity = {}
+        disk_capacity = {}
+        gpuComponents = {}
         for capacity in item['bundleItems']:
             for category in capacity['categories']:
                 if category['categoryCode'] == 'dedicated_host_ram':
                     mem_capacity = capacity['capacity']
                 if category['categoryCode'] == 'dedicated_host_disk':
                     disk_capacity = capacity['capacity']
```

### Comparing `softlayer-6.2.1/SoftLayer/managers/dns.py` & `softlayer-6.2.2/SoftLayer/managers/dns.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/email.py` & `softlayer-6.2.2/SoftLayer/managers/email.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/event_log.py` & `softlayer-6.2.2/SoftLayer/managers/event_log.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/file.py` & `softlayer-6.2.2/SoftLayer/managers/file.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/firewall.py` & `softlayer-6.2.2/SoftLayer/managers/firewall.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/hardware.py` & `softlayer-6.2.2/SoftLayer/managers/hardware.py`

 * *Files 0% similar despite different names*

```diff
@@ -1119,14 +1119,15 @@
 
         :param disk_data: List of disks to be added or upgraded.
         :param list upgrade_prices: List of item prices.
         :param String disk_channel: Disk position.
         :param String disk_type: Disk type.
 
         """
+        disk_price = {}
         if disk_data.get('description') == disk_type:
             if "add" in disk_type:
                 raise SoftLayerError("Unable to add the disk because this already exists.")
             if "resize" in disk_type:
                 raise SoftLayerError("Unable to resize the disk because this does not exists.")
         else:
             price_id = self._get_prices_for_upgrade_option(upgrade_prices, disk_channel,
```

### Comparing `softlayer-6.2.1/SoftLayer/managers/image.py` & `softlayer-6.2.2/SoftLayer/managers/image.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/ipsec.py` & `softlayer-6.2.2/SoftLayer/managers/ipsec.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/license.py` & `softlayer-6.2.2/SoftLayer/managers/license.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/load_balancer.py` & `softlayer-6.2.2/SoftLayer/managers/load_balancer.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/metadata.py` & `softlayer-6.2.2/SoftLayer/managers/metadata.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/network.py` & `softlayer-6.2.2/SoftLayer/managers/network.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/object_storage.py` & `softlayer-6.2.2/SoftLayer/managers/object_storage.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/ordering.py` & `softlayer-6.2.2/SoftLayer/managers/ordering.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/search.py` & `softlayer-6.2.2/SoftLayer/managers/search.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/sshkey.py` & `softlayer-6.2.2/SoftLayer/managers/sshkey.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/ssl.py` & `softlayer-6.2.2/SoftLayer/managers/ssl.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/storage.py` & `softlayer-6.2.2/SoftLayer/managers/storage.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/storage_utils.py` & `softlayer-6.2.2/SoftLayer/managers/storage_utils.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/tags.py` & `softlayer-6.2.2/SoftLayer/managers/tags.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/ticket.py` & `softlayer-6.2.2/SoftLayer/managers/ticket.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/user.py` & `softlayer-6.2.2/SoftLayer/managers/user.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/vs.py` & `softlayer-6.2.2/SoftLayer/managers/vs.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/vs_capacity.py` & `softlayer-6.2.2/SoftLayer/managers/vs_capacity.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/managers/vs_placement.py` & `softlayer-6.2.2/SoftLayer/managers/vs_placement.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/shell/cmd_help.py` & `softlayer-6.2.2/SoftLayer/shell/cmd_help.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/shell/completer.py` & `softlayer-6.2.2/SoftLayer/shell/completer.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/shell/core.py` & `softlayer-6.2.2/SoftLayer/shell/core.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/testing/__init__.py` & `softlayer-6.2.2/SoftLayer/testing/__init__.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/testing/xmlrpc.py` & `softlayer-6.2.2/SoftLayer/testing/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/transports/__init__.py` & `softlayer-6.2.2/SoftLayer/transports/__init__.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/transports/debug.py` & `softlayer-6.2.2/SoftLayer/transports/debug.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/transports/fixture.py` & `softlayer-6.2.2/SoftLayer/transports/fixture.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/transports/rest.py` & `softlayer-6.2.2/SoftLayer/transports/rest.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/transports/timing.py` & `softlayer-6.2.2/SoftLayer/transports/timing.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/transports/transport.py` & `softlayer-6.2.2/SoftLayer/transports/transport.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     """Sets up urllib sessions"""
 
     client = requests.Session()
     client.headers.update({
         'Content-Type': 'application/json',
         'User-Agent': user_agent,
     })
-    retry = Retry(connect=3, backoff_factor=3)
+    retry = Retry(total=3, connect=1, backoff_factor=1)
     adapter = HTTPAdapter(max_retries=retry)
     client.mount('https://', adapter)
     return client
 
 
 # transports.Request does have a lot of instance attributes. :(
 # pylint: disable=too-many-instance-attributes
```

### Comparing `softlayer-6.2.1/SoftLayer/transports/xmlrpc.py` & `softlayer-6.2.2/SoftLayer/transports/xmlrpc.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer/utils.py` & `softlayer-6.2.2/SoftLayer/utils.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/SoftLayer.egg-info/PKG-INFO` & `softlayer-6.2.2/SoftLayer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SoftLayer
-Version: 6.2.1
+Version: 6.2.2
 Summary: A library for SoftLayer's API
 Home-page: https://github.com/SoftLayer/softlayer-python
 Author: SoftLayer, Inc., an IBM Company
 Author-email: SLDNDeveloperRelations@wwpdl.vnet.ibm.com
 License: MIT
 Keywords: softlayer,cloud,slcli,ibmcloud
 Classifier: Environment :: Console
```

### Comparing `softlayer-6.2.1/SoftLayer.egg-info/SOURCES.txt` & `softlayer-6.2.2/SoftLayer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/setup.py` & `softlayer-6.2.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     with codecs.open('README.rst', 'r', 'utf-8') as readme_file:
         LONG_DESCRIPTION = readme_file.read()
 else:
     LONG_DESCRIPTION = DESCRIPTION
 
 setup(
     name='SoftLayer',
-    version='v6.2.1',
+    version='v6.2.2',
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type='text/x-rst',
     author='SoftLayer, Inc., an IBM Company',
     author_email='SLDNDeveloperRelations@wwpdl.vnet.ibm.com',
     packages=find_packages(exclude=['tests']),
     license='MIT',
```

### Comparing `softlayer-6.2.1/tests/CLI/core_tests.py` & `softlayer-6.2.2/tests/CLI/core_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/custom_types_tests.py` & `softlayer-6.2.2/tests/CLI/custom_types_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/environment_tests.py` & `softlayer-6.2.2/tests/CLI/environment_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/formatting_table_tests.py` & `softlayer-6.2.2/tests/CLI/formatting_table_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/helper_tests.py` & `softlayer-6.2.2/tests/CLI/helper_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/account_tests.py` & `softlayer-6.2.2/tests/CLI/modules/account_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/bandwidth_tests.py` & `softlayer-6.2.2/tests/CLI/modules/bandwidth_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/block_tests.py` & `softlayer-6.2.2/tests/CLI/modules/block_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/call_api_tests.py` & `softlayer-6.2.2/tests/CLI/modules/call_api_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/cdn_tests.py` & `softlayer-6.2.2/tests/CLI/modules/cdn_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/config_tests.py` & `softlayer-6.2.2/tests/CLI/modules/config_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/dedicatedhost_tests.py` & `softlayer-6.2.2/tests/CLI/modules/dedicatedhost_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/dns_tests.py` & `softlayer-6.2.2/tests/CLI/modules/dns_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/email_tests.py` & `softlayer-6.2.2/tests/CLI/modules/email_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/event_log_tests.py` & `softlayer-6.2.2/tests/CLI/modules/event_log_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/file_tests.py` & `softlayer-6.2.2/tests/CLI/modules/file_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/firewall_tests.py` & `softlayer-6.2.2/tests/CLI/modules/firewall_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/globalip_tests.py` & `softlayer-6.2.2/tests/CLI/modules/globalip_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/image_tests.py` & `softlayer-6.2.2/tests/CLI/modules/image_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/ipsec_tests.py` & `softlayer-6.2.2/tests/CLI/modules/ipsec_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/licenses_test.py` & `softlayer-6.2.2/tests/CLI/modules/licenses_test.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/loadbal_tests.py` & `softlayer-6.2.2/tests/CLI/modules/loadbal_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/nas_tests.py` & `softlayer-6.2.2/tests/CLI/modules/nas_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/object_storage_tests.py` & `softlayer-6.2.2/tests/CLI/modules/object_storage_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/order_tests.py` & `softlayer-6.2.2/tests/CLI/modules/order_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/report_tests.py` & `softlayer-6.2.2/tests/CLI/modules/report_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/search_tests.py` & `softlayer-6.2.2/tests/CLI/modules/search_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/security_tests.py` & `softlayer-6.2.2/tests/CLI/modules/security_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/securitygroup_tests.py` & `softlayer-6.2.2/tests/CLI/modules/securitygroup_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/sshkey_tests.py` & `softlayer-6.2.2/tests/CLI/modules/sshkey_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/ssl_tests.py` & `softlayer-6.2.2/tests/CLI/modules/ssl_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/subnet_tests.py` & `softlayer-6.2.2/tests/CLI/modules/subnet_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/summary_tests.py` & `softlayer-6.2.2/tests/CLI/modules/summary_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/tag_tests.py` & `softlayer-6.2.2/tests/CLI/modules/tag_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/ticket_tests.py` & `softlayer-6.2.2/tests/CLI/modules/ticket_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/user_tests.py` & `softlayer-6.2.2/tests/CLI/modules/user_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/vlan_tests.py` & `softlayer-6.2.2/tests/CLI/modules/vlan_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/vs/vs_capacity_tests.py` & `softlayer-6.2.2/tests/CLI/modules/vs/vs_capacity_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/vs/vs_create_tests.py` & `softlayer-6.2.2/tests/CLI/modules/vs/vs_create_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/vs/vs_placement_tests.py` & `softlayer-6.2.2/tests/CLI/modules/vs/vs_placement_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/CLI/modules/vs/vs_tests.py` & `softlayer-6.2.2/tests/CLI/modules/vs/vs_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/account_tests.py` & `softlayer-6.2.2/tests/managers/account_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/bandwidth_tests.py` & `softlayer-6.2.2/tests/managers/bandwidth_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/block_tests.py` & `softlayer-6.2.2/tests/managers/block_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/cdn_tests.py` & `softlayer-6.2.2/tests/managers/cdn_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/dedicated_host_tests.py` & `softlayer-6.2.2/tests/managers/dedicated_host_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/dns_tests.py` & `softlayer-6.2.2/tests/managers/dns_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/email_tests.py` & `softlayer-6.2.2/tests/managers/email_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/event_log_tests.py` & `softlayer-6.2.2/tests/managers/event_log_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/file_tests.py` & `softlayer-6.2.2/tests/managers/file_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/firewall_tests.py` & `softlayer-6.2.2/tests/managers/firewall_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/hardware_tests.py` & `softlayer-6.2.2/tests/managers/hardware_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/image_tests.py` & `softlayer-6.2.2/tests/managers/image_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/ipsec_tests.py` & `softlayer-6.2.2/tests/managers/ipsec_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/loadbal_tests.py` & `softlayer-6.2.2/tests/managers/loadbal_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/metadata_tests.py` & `softlayer-6.2.2/tests/managers/metadata_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/network_tests.py` & `softlayer-6.2.2/tests/managers/network_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/object_storage_tests.py` & `softlayer-6.2.2/tests/managers/object_storage_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/ordering_tests.py` & `softlayer-6.2.2/tests/managers/ordering_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/search_tests.py` & `softlayer-6.2.2/tests/managers/search_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/sshkey_tests.py` & `softlayer-6.2.2/tests/managers/sshkey_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/ssl_tests.py` & `softlayer-6.2.2/tests/managers/ssl_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/storage_generic_tests.py` & `softlayer-6.2.2/tests/managers/storage_generic_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/storage_utils_tests.py` & `softlayer-6.2.2/tests/managers/storage_utils_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/tag_tests.py` & `softlayer-6.2.2/tests/managers/tag_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/ticket_tests.py` & `softlayer-6.2.2/tests/managers/ticket_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/user_tests.py` & `softlayer-6.2.2/tests/managers/user_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/vs/vs_capacity_tests.py` & `softlayer-6.2.2/tests/managers/vs/vs_capacity_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/vs/vs_order_tests.py` & `softlayer-6.2.2/tests/managers/vs/vs_order_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/vs/vs_placement_tests.py` & `softlayer-6.2.2/tests/managers/vs/vs_placement_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/vs/vs_tests.py` & `softlayer-6.2.2/tests/managers/vs/vs_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/managers/vs/vs_waiting_for_ready_tests.py` & `softlayer-6.2.2/tests/managers/vs/vs_waiting_for_ready_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/transports/debug_tests.py` & `softlayer-6.2.2/tests/transports/debug_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/transports/rest_tests.py` & `softlayer-6.2.2/tests/transports/rest_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/transports/transport_tests.py` & `softlayer-6.2.2/tests/transports/transport_tests.py`

 * *Files identical despite different names*

### Comparing `softlayer-6.2.1/tests/transports/xmlrpc_tests.py` & `softlayer-6.2.2/tests/transports/xmlrpc_tests.py`

 * *Files identical despite different names*

