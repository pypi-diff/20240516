# Comparing `tmp/ovsdbapp-2.6.0.tar.gz` & `tmp/ovsdbapp-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovsdbapp-2.6.0.tar", last modified: Thu Feb 22 15:11:45 2024, max compression
+gzip compressed data, was "ovsdbapp-2.7.0.tar", last modified: Thu May 16 13:07:06 2024, max compression
```

## Comparing `ovsdbapp-2.6.0.tar` & `ovsdbapp-2.7.0.tar`

### file list

```diff
@@ -1,197 +1,198 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.992421 ovsdbapp-2.6.0/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4111 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/.pylintrc
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3538 2024-02-22 15:11:45.000000 ovsdbapp-2.6.0/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/CONTRIBUTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17498 2024-02-22 15:11:45.000000 ovsdbapp-2.6.0/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/HACKING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1537 2024-02-22 15:11:45.992421 ovsdbapp-2.6.0/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2042 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/TESTING.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.948413 ovsdbapp-2.6.0/doc/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/doc/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.948413 ovsdbapp-2.6.0/doc/source/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     2670 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/doc/source/conf.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.952413 ovsdbapp-2.6.0/doc/source/contributor/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/doc/source/contributor/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/doc/source/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.952413 ovsdbapp-2.6.0/doc/source/install/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/doc/source/install/index.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.952413 ovsdbapp-2.6.0/doc/source/user/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/doc/source/user/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/doc/source/user/overview.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4840 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/doc/source/user/tutorial.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.952413 ovsdbapp-2.6.0/ovsdbapp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/CHANGES
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11910 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/api.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.956414 ovsdbapp-2.6.0/ovsdbapp/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.960415 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9342 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    14070 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/command.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.960415 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/common/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/common/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/common/base_connection_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8119 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2418 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    16687 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/idlutils.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.960415 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/linux/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/linux/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1316 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/linux/connection_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/rowview.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5256 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/transaction.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3320 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/vlog.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.960415 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/windows/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/windows/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/windows/connection_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1683 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/windows/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1304 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/constants.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6596 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1948 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/exceptions.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.960415 ovsdbapp-2.6.0/ovsdbapp/schema/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.964416 ovsdbapp-2.6.0/ovsdbapp/schema/hardware_vtep/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/hardware_vtep/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7885 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/hardware_vtep/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9755 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/hardware_vtep/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/hardware_vtep/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.964416 ovsdbapp-2.6.0/ovsdbapp/schema/open_vswitch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/open_vswitch/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8593 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/open_vswitch/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    13455 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/open_vswitch/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/open_vswitch/helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5614 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/open_vswitch/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.964416 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_ic_northbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_ic_northbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2179 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_ic_northbound/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2416 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_ic_northbound/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_ic_northbound/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.968417 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_northbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_northbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    60641 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_northbound/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    75575 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_northbound/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    18489 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_northbound/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.968417 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_southbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_southbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3022 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_southbound/api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4464 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_southbound/commands.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1772 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/schema/ovn_southbound/impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.968417 ovsdbapp-2.6.0/ovsdbapp/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.968417 ovsdbapp-2.6.0/ovsdbapp/tests/functional/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.968417 ovsdbapp-2.6.0/ovsdbapp/tests/functional/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/backend/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.968417 ovsdbapp-2.6.0/ovsdbapp/tests/functional/backend/ovs_idl/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/backend/ovs_idl/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2976 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/backend/ovs_idl/test_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2714 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/backend/ovs_idl/test_indexing.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2679 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.972417 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/fixtures.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.972417 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/hardware_vtep/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/hardware_vtep/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/hardware_vtep/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15722 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/hardware_vtep/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.972417 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/open_vswitch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/open_vswitch/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/open_vswitch/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6227 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/open_vswitch/test_common_db.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9049 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/open_vswitch/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.972417 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3976 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.976418 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_northbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_northbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1617 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_northbound/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)   115495 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_northbound/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.976418 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_southbound/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_southbound/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1598 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_southbound/event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_southbound/fixtures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7393 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_southbound/test_impl_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.976418 ovsdbapp-2.6.0/ovsdbapp/tests/unit/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/unit/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.976418 ovsdbapp-2.6.0/ovsdbapp/tests/unit/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/unit/backend/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.980419 ovsdbapp-2.6.0/ovsdbapp/tests/unit/backend/ovs_idl/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/unit/backend/ovs_idl/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/unit/backend/ovs_idl/test_connection.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/unit/backend/ovs_idl/test_helpers.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    12330 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/unit/backend/ovs_idl/test_idlutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2715 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/unit/backend/ovs_idl/test_vlog.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/unit/backend/test_ovs_idl.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.980419 ovsdbapp-2.6.0/ovsdbapp/tests/unit/schema/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/unit/schema/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.980419 ovsdbapp-2.6.0/ovsdbapp/tests/unit/schema/open_vswitch/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/unit/schema/open_vswitch/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/unit/schema/open_vswitch/test_impl_idl.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/unit/test_api.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3026 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/unit/test_event.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2855 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/unit/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2341 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/tests/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11749 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/ovsdbapp/venv.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.956414 ovsdbapp-2.6.0/ovsdbapp.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1537 2024-02-22 15:11:45.000000 ovsdbapp-2.6.0/ovsdbapp.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5968 2024-02-22 15:11:45.000000 ovsdbapp-2.6.0/ovsdbapp.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:11:45.000000 ovsdbapp-2.6.0/ovsdbapp.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-02-22 15:11:45.000000 ovsdbapp-2.6.0/ovsdbapp.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-02-22 15:11:45.000000 ovsdbapp-2.6.0/ovsdbapp.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-02-22 15:11:45.000000 ovsdbapp-2.6.0/ovsdbapp.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-02-22 15:11:45.000000 ovsdbapp-2.6.0/ovsdbapp.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.944412 ovsdbapp-2.6.0/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.984420 ovsdbapp-2.6.0/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/notes/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/notes/configure-ovsdb-manager-a29a148b241a125e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/notes/drop-py27-support-c426980520444bfa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/notes/drop-python-3-6-and-3-7-8ae8ccf16e422fc4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/notes/ovn-support-allow-stateless-01aed5acdcd1c0d1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/notes/ovn-support-discard-nexthop-cdb1d35aceaf4b63.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/notes/ovn-support-hw-vtep-ca8b3ee7a74df3fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/notes/ovn-support-ic-northbound-df557a866a1f411f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/notes/provide-address-set-api-3cb387b9e571d4ea.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/notes/provide-lb-hc-api-8ff13ccaf75f1eee.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/notes/provide-lrp-gateway-chassis-api-14e2948183f60cfa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/notes/provide-lrp-get-method-a33a99a7f86b827e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/notes/provide-lrp-networks-modifying-1af13589064c12c6.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.988420 ovsdbapp-2.6.0/releasenotes/source/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/2023.1.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/2023.2.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.988420 ovsdbapp-2.6.0/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7768 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      280 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/pike.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/queens.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/rocky.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/stein.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/train.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/ussuri.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      138 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/victoria.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      134 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/wallaby.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/xena.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/yoga.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/releasenotes/source/zed.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/requirements.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-02-22 15:11:45.992421 ovsdbapp-2.6.0/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.992421 ovsdbapp-2.6.0/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1863 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/tools/coding-checks.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1774 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/tools/debug_venv
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1735 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/tools/debug_venv.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      509 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/tools/setup-ovs.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      278 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/tools/test-setup.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2578 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/tox.ini
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-02-22 15:11:45.992421 ovsdbapp-2.6.0/zuul.d/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/zuul.d/ovsdbapp-jobs.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2024-02-22 15:11:10.000000 ovsdbapp-2.6.0/zuul.d/project.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.196385 ovsdbapp-2.7.0/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4111 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/.pylintrc
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       94 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3648 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      651 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/CONTRIBUTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18052 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      452 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/HACKING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    10143 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1537 2024-05-16 13:07:06.196385 ovsdbapp-2.7.0/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      534 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2042 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/TESTING.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.160364 ovsdbapp-2.7.0/doc/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      108 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.160364 ovsdbapp-2.7.0/doc/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2670 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/source/conf.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.160364 ovsdbapp-2.7.0/doc/source/contributor/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       78 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/source/contributor/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      273 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/source/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.160364 ovsdbapp-2.7.0/doc/source/install/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      193 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/source/install/index.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.160364 ovsdbapp-2.7.0/doc/source/user/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      298 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/source/user/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2122 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/source/user/overview.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4840 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/doc/source/user/tutorial.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.164367 ovsdbapp-2.7.0/ovsdbapp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/CHANGES
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      664 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11910 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/api.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.168369 ovsdbapp-2.7.0/ovsdbapp/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.172371 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9364 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    14070 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/command.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.172371 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/common/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/common/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1065 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/common/base_connection_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8119 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2418 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1097 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    16687 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/idlutils.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.172371 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/linux/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/linux/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1316 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/linux/connection_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1022 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/rowview.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5256 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/transaction.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3320 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/vlog.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.172371 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/windows/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/windows/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2162 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/windows/connection_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1683 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/windows/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1304 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/constants.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6596 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1948 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/exceptions.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.172371 ovsdbapp-2.7.0/ovsdbapp/schema/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.172371 ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7885 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9755 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3356 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.176374 ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8593 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    13455 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2244 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5614 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.176374 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2179 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2416 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1331 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.176374 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    60641 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    75757 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    18489 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.176374 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3022 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4648 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/commands.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1772 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.180376 ovsdbapp-2.7.0/ovsdbapp/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      940 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.180376 ovsdbapp-2.7.0/ovsdbapp/tests/functional/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.180376 ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.180376 ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/ovs_idl/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/ovs_idl/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2976 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/ovs_idl/test_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2714 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/ovs_idl/test_indexing.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2679 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.180376 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1829 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/fixtures.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.180376 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/hardware_vtep/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/hardware_vtep/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      968 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/hardware_vtep/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15722 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/hardware_vtep/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.184378 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      742 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6227 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/test_common_db.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9049 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.184378 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      873 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3976 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.184378 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_northbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_northbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1617 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_northbound/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)   116548 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_northbound/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.184378 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1598 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      868 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/fixtures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7393 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/test_impl_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.184378 ovsdbapp-2.7.0/ovsdbapp/tests/unit/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.184378 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.188381 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2363 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_connection.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1153 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_helpers.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    12330 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_idlutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2715 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_vlog.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1896 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/test_ovs_idl.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.188381 ovsdbapp-2.7.0/ovsdbapp/tests/unit/schema/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/schema/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.188381 ovsdbapp-2.7.0/ovsdbapp/tests/unit/schema/open_vswitch/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/schema/open_vswitch/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1971 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/schema/open_vswitch/test_impl_idl.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4027 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/test_api.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3026 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/test_event.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2855 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/unit/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2341 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/tests/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11749 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/ovsdbapp/venv.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.168369 ovsdbapp-2.7.0/ovsdbapp.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1537 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/ovsdbapp.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5999 2024-05-16 13:07:06.000000 ovsdbapp-2.7.0/ovsdbapp.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/ovsdbapp.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/ovsdbapp.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       46 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/ovsdbapp.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       63 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/ovsdbapp.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        9 2024-05-16 13:07:05.000000 ovsdbapp-2.7.0/ovsdbapp.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.156362 ovsdbapp-2.7.0/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.192383 ovsdbapp-2.7.0/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      442 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/configure-ovsdb-manager-a29a148b241a125e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/drop-py27-support-c426980520444bfa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/drop-python-3-6-and-3-7-8ae8ccf16e422fc4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       91 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/ovn-support-allow-stateless-01aed5acdcd1c0d1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      104 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/ovn-support-discard-nexthop-cdb1d35aceaf4b63.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      373 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/ovn-support-hw-vtep-ca8b3ee7a74df3fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      238 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/ovn-support-ic-northbound-df557a866a1f411f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/provide-address-set-api-3cb387b9e571d4ea.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      271 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/provide-lb-hc-api-8ff13ccaf75f1eee.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/provide-lrp-gateway-chassis-api-14e2948183f60cfa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       99 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/provide-lrp-get-method-a33a99a7f86b827e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       90 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/notes/provide-lrp-networks-modifying-1af13589064c12c6.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.196385 ovsdbapp-2.7.0/releasenotes/source/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/2023.1.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/2023.2.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/2024.1.rst
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.196385 ovsdbapp-2.7.0/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7768 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      290 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/pike.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      147 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/queens.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/rocky.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      145 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/stein.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      126 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/train.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      130 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/ussuri.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      144 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/victoria.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/wallaby.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/xena.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/yoga.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      118 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/releasenotes/source/zed.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      338 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/requirements.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      768 2024-05-16 13:07:06.200388 ovsdbapp-2.7.0/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1030 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      207 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.196385 ovsdbapp-2.7.0/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1863 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/tools/coding-checks.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1774 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/tools/debug_venv
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1735 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/tools/debug_venv.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      509 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/tools/setup-ovs.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      278 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/tools/test-setup.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2578 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-05-16 13:07:06.196385 ovsdbapp-2.7.0/zuul.d/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      335 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/zuul.d/ovsdbapp-jobs.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      336 2024-05-16 13:06:38.000000 ovsdbapp-2.7.0/zuul.d/project.yaml
```

### Comparing `ovsdbapp-2.6.0/.pylintrc` & `ovsdbapp-2.7.0/.pylintrc`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/AUTHORS` & `ovsdbapp-2.7.0/AUTHORS`

 * *Files 3% similar despite different names*

```diff
@@ -15,21 +15,23 @@
 Boden R <bodenvmw@gmail.com>
 Brian Haley <bhaley@redhat.com>
 Chuck Short <chucks@redhat.com>
 Corey Bryant <corey.bryant@canonical.com>
 Cyril Roelandt <cyril.roelandt@enovance.com>
 Daniel Alvarez <dalvarez@redhat.com>
 Davanum Srinivas <davanum@gmail.com>
+Dmitrii Skorykh <dskorykh@gmail.com>
 Dong Jun <dongj@dtdream.com>
 Doug Hellmann <doug@doughellmann.com>
 Doug Wiegley <dougw@a10networks.com>
 Elvira García <egarciar@redhat.com>
 Emma Foley <emma.l.foley@intel.com>
 Flavio Fernandes <flaviof@redhat.com>
 Frank Wang <wangpeihuixyz@126.com>
+Frode Nordahl <fnordahl@ubuntu.com>
 Frode Nordahl <frode.nordahl@canonical.com>
 Gal Sagie <gal.sagie@huawei.com>
 Gary Kotton <gkotton@vmware.com>
 Ghanshyam Mann <gmann@ghanshyammann.com>
 Guoshuai Li <ligs@dtdream.com>
 Henry Gessau <gessau@gmail.com>
 Hervé Beraud <hberaud@redhat.com>
@@ -55,14 +57,15 @@
 Omer Anson <omer.anson@toganetworks.com>
 OpenStack Release Bot <infra-root@openstack.org>
 Petr Horáček <phoracek@redhat.com>
 Richard Theis <rtheis@us.ibm.com>
 Rodolfo Alonso <ralonsoh@redhat.com>
 Rodolfo Alonso Hernandez <ralonsoh@redhat.com>
 Sean Mooney <sean.k.mooney@intel.com>
+Seena Fallah <seenafallah@gmail.com>
 Slawek Kaplonski <skaplons@redhat.com>
 Takashi Kajinami <kajinamit@oss.nttdata.com>
 Takashi Natsume <takanattie@gmail.com>
 Ted Elhourani <theodore.elhourani@gmail.com>
 Terry Wilson <terry@logivox.net>
 Terry Wilson <twilson@redhat.com>
 Vu Cong Tuan <tuanvc@vn.fujitsu.com>
```

### Comparing `ovsdbapp-2.6.0/CONTRIBUTING.rst` & `ovsdbapp-2.7.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ChangeLog` & `ovsdbapp-2.7.0/ChangeLog`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,24 @@
 CHANGES
 =======
 
+2.7.0
+-----
+
+* Backend: always operate on (class level) ovsdb\_connection
+* Remove executable from python files which don't really needs it
+* Handle IPv6 addresses for LB IP port mappings
+* Fix BFD functional test, avoid comparing status column
+* ovn-sb: remove chassis from Chassis\_Private on ChassisDelCommand
+* Update master for stable/2024.1
+* reno: Update master for unmaintained/xena
+* reno: Update master for unmaintained/wallaby
+* reno: Update master for unmaintained/victoria
+* nb: commands: fix passing string to LSP attach/detach mirror API
+
 2.6.0
 -----
 
 * reno: Update master for unmaintained/yoga
 * tox: Drop envdir
 * Bump hacking
 * Support add/remove CIDR type address in Address\_Set cmds
```

### Comparing `ovsdbapp-2.6.0/LICENSE` & `ovsdbapp-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/PKG-INFO` & `ovsdbapp-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ovsdbapp
-Version: 2.6.0
+Version: 2.7.0
 Summary: A library for creating OVSDB applications
 Home-page: https://pypi.org/project/ovsdbapp/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========
         ovsdbapp
```

### Comparing `ovsdbapp-2.6.0/README.rst` & `ovsdbapp-2.7.0/README.rst`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/TESTING.rst` & `ovsdbapp-2.7.0/TESTING.rst`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/doc/source/conf.py` & `ovsdbapp-2.7.0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/doc/source/user/overview.rst` & `ovsdbapp-2.7.0/doc/source/user/overview.rst`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/doc/source/user/tutorial.rst` & `ovsdbapp-2.7.0/doc/source/user/tutorial.rst`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/__init__.py` & `ovsdbapp-2.7.0/ovsdbapp/__init__.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/api.py` & `ovsdbapp-2.7.0/ovsdbapp/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/__init__.py` & `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,20 +28,20 @@
     lookup_table = {}
     _ovsdb_connection = None
 
     def __init__(self, connection, start=True, auto_index=True, **kwargs):
         super().__init__(**kwargs)
         self.ovsdb_connection = connection
         if auto_index:
-            if connection.is_running:
+            if self.ovsdb_connection.is_running:
                 LOG.debug("Connection already started, not creating indices")
             else:
                 self.autocreate_indices()
         if start:
-            self.start_connection(connection)
+            self.start_connection(self.ovsdb_connection)
 
     @property
     def ovsdb_connection(self):
         return self.__class__._ovsdb_connection
 
     @ovsdb_connection.setter
     def ovsdb_connection(self, connection):
```

### Comparing `ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/command.py` & `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/command.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/common/base_connection_utils.py` & `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/common/base_connection_utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/connection.py` & `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/connection.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/event.py` & `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/event.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/fixtures.py` & `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/idlutils.py` & `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/idlutils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/linux/connection_utils.py` & `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/linux/connection_utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/rowview.py` & `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/rowview.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/transaction.py` & `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/transaction.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/vlog.py` & `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/vlog.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/windows/connection_utils.py` & `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/windows/connection_utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/backend/ovs_idl/windows/utils.py` & `ovsdbapp-2.7.0/ovsdbapp/backend/ovs_idl/windows/utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/constants.py` & `ovsdbapp-2.7.0/ovsdbapp/constants.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/event.py` & `ovsdbapp-2.7.0/ovsdbapp/event.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/exceptions.py` & `ovsdbapp-2.7.0/ovsdbapp/exceptions.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/hardware_vtep/api.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/hardware_vtep/commands.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/commands.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/hardware_vtep/impl_idl.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/hardware_vtep/impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/open_vswitch/api.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/open_vswitch/commands.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/commands.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/open_vswitch/helpers.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/helpers.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/open_vswitch/impl_idl.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/open_vswitch/impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/ovn_ic_northbound/api.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/ovn_ic_northbound/commands.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/commands.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/ovn_ic_northbound/impl_idl.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_ic_northbound/impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/ovn_northbound/api.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/ovn_northbound/commands.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/commands.py`

 * *Files 1% similar despite different names*

```diff
@@ -1219,15 +1219,15 @@
         try:
             lsp = self.api.lookup('Logical_Switch_Port', self.port)
             mirror = self.api.lookup('Mirror', self.mirror)
             if mirror in lsp.mirror_rules and not self.may_exist:
                 msg = "Mirror Rule %s is already set on LSP %s" % (self.mirror,
                                                                    self.port)
                 raise RuntimeError(msg)
-            lsp.addvalue('mirror_rules', self.mirror)
+            lsp.addvalue('mirror_rules', mirror)
         except idlutils.RowNotFound as e:
             raise RuntimeError("LSP %s not found" % self.port) from e
 
 
 class LspDetachMirror(cmd.BaseCommand):
     def __init__(self, api, port, mirror, if_exist=False):
         super().__init__(api)
@@ -1239,15 +1239,15 @@
         try:
             lsp = self.api.lookup('Logical_Switch_Port', self.port)
             mirror = self.api.lookup('Mirror', self.mirror)
             if mirror not in lsp.mirror_rules and not self.if_exist:
                 msg = "Mirror Rule %s doesn't exist on LSP %s" % (self.mirror,
                                                                   self.port)
                 raise RuntimeError(msg)
-            lsp.delvalue('mirror_rules', self.mirror)
+            lsp.delvalue('mirror_rules', mirror)
         except idlutils.RowNotFound as e:
             if self.if_exists:
                 return
             msg = "LSP %s doesn't exist" % self.port
             raise RuntimeError(msg) from e
 
 
@@ -1666,37 +1666,44 @@
                 return
         if not self.if_exists:
             msg = "Health check '%s' on lb %s does not exist" % (
                 self.hc_uuid, self.lb)
             raise RuntimeError(msg)
 
 
-class LbAddIpPortMappingCommand(cmd.BaseCommand):
+class LbIpPortMappingCommand(cmd.BaseCommand):
+    @staticmethod
+    def normalize_ip(ip_str):
+        ip = netaddr.IPAddress(ip_str)
+        return f"[{ip}]" if ip.version == 6 else str(ip)
+
+
+class LbAddIpPortMappingCommand(LbIpPortMappingCommand):
     table = 'Load_Balancer'
 
     def __init__(self, api, lb, endpoint_ip, port_name, source_ip):
         super().__init__(api)
         self.lb = lb
-        self.endpoint_ip = str(netaddr.IPAddress(endpoint_ip))
+        self.endpoint_ip = self.normalize_ip(endpoint_ip)
         self.port_name = port_name
-        self.source_ip = str(netaddr.IPAddress(source_ip))
+        self.source_ip = self.normalize_ip(source_ip)
 
     def run_idl(self, txn):
         lb = self.api.lookup(self.table, self.lb)
         lb.setkey('ip_port_mappings', self.endpoint_ip,
                   '%s:%s' % (self.port_name, self.source_ip))
 
 
-class LbDelIpPortMappingCommand(cmd.BaseCommand):
+class LbDelIpPortMappingCommand(LbIpPortMappingCommand):
     table = 'Load_Balancer'
 
     def __init__(self, api, lb, endpoint_ip):
         super().__init__(api)
         self.lb = lb
-        self.endpoint_ip = str(netaddr.IPAddress(endpoint_ip))
+        self.endpoint_ip = self.normalize_ip(endpoint_ip)
 
     def run_idl(self, txn):
         lb = self.api.lookup(self.table, self.lb)
         lb.delkey('ip_port_mappings', self.endpoint_ip)
 
 
 class HealthCheckAddCommand(cmd.AddCommand):
```

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/ovn_northbound/impl_idl.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_northbound/impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/ovn_southbound/api.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/ovn_southbound/commands.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/commands.py`

 * *Files 3% similar despite different names*

```diff
@@ -70,14 +70,20 @@
             if self.if_exists:
                 return
             raise
         for encap in getattr(chassis, 'encaps', []):
             encap.delete()
         chassis.delete()
 
+        try:
+            chassis_private = self.api.lookup('Chassis_Private', self.chassis)
+            chassis_private.delete()
+        except idlutils.RowNotFound:
+            pass
+
 
 class ChassisListCommand(cmd.ReadOnlyCommand):
     def run_idl(self, txn):
         self.result = [rowview.RowView(r)
                        for r in self.api.tables['Chassis'].rows.values()]
```

### Comparing `ovsdbapp-2.6.0/ovsdbapp/schema/ovn_southbound/impl_idl.py` & `ovsdbapp-2.7.0/ovsdbapp/schema/ovn_southbound/impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/base.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/base.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/backend/ovs_idl/test_connection.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/ovs_idl/test_connection.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/backend/ovs_idl/test_indexing.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/backend/ovs_idl/test_indexing.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/base.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/base.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/fixtures.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/hardware_vtep/fixtures.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/hardware_vtep/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/hardware_vtep/test_impl_idl.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/hardware_vtep/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/open_vswitch/fixtures.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/open_vswitch/test_common_db.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/test_common_db.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/open_vswitch/test_impl_idl.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/open_vswitch/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/fixtures.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/test_impl_idl.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_ic_northbound/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_northbound/fixtures.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_northbound/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_northbound/test_impl_idl.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_northbound/test_impl_idl.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 
 import netaddr
 import testscenarios
+import types
 import uuid
 
 from ovsdbapp.backend.ovs_idl import idlutils
 from ovsdbapp import constants as const
 from ovsdbapp.tests.functional import base
 from ovsdbapp.tests.functional.schema.ovn_northbound import fixtures
 from ovsdbapp.tests import utils
@@ -1902,38 +1903,51 @@
 
     def test_lb_del_health_check_if_exists(self):
         lb = self._lb_add(utils.get_rand_device_name(),
                           '192.0.0.1', ['10.0.0.1'])
         self.api.lb_del_health_check(lb.name, uuid.uuid4(),
                                      if_exists=True).execute(check_error=True)
 
-    def _test_lb_add_del_ip_port_mapping(self, col):
-        endpoint_ip = '172.31.0.4'
+    def _test_lb_add_del_ip_port_mapping(self, col, input, expected):
+        endpoint_ip, source_ip = input
+        expected_endpoint_ip, expected_source_ip = expected
         port_name = 'sw1-p1'
-        source_ip = '172.31.0.6'
+
         lb = self._lb_add(utils.get_rand_device_name(),
                           '192.0.0.1', ['10.0.0.1'])
         self.assertEqual(lb.ip_port_mappings, {})
         val = getattr(lb, col)
         self.api.lb_add_ip_port_mapping(val,
                                         endpoint_ip,
                                         port_name,
                                         source_ip).execute(check_error=True)
-        self.assertEqual(lb.ip_port_mappings[endpoint_ip],
-                         '%s:%s' % (port_name, source_ip))
+        self.assertEqual(lb.ip_port_mappings[expected_endpoint_ip],
+                         '%s:%s' % (port_name, expected_source_ip))
 
         self.api.lb_del_ip_port_mapping(val,
                                         endpoint_ip).execute(check_error=True)
         self.assertEqual(lb.ip_port_mappings, {})
 
     def test_lb_add_del_ip_port_mapping_uuid(self):
-        self._test_lb_add_del_ip_port_mapping('uuid')
+        input = ('172.31.0.3', '172.31.0.6')
+        self._test_lb_add_del_ip_port_mapping('uuid', input, input)
+
+    def test_lb_add_del_ip_port_mapping_uuid_v6(self):
+        input = ('2001:db8::1', '2001:db8::2')
+        expected = (f"[{input[0]}]", f"[{input[1]}]")
+        self._test_lb_add_del_ip_port_mapping('uuid', input, expected)
 
     def test_lb_add_del_ip_port_mapping_name(self):
-        self._test_lb_add_del_ip_port_mapping('name')
+        input = ('172.31.0.3', '172.31.0.6')
+        self._test_lb_add_del_ip_port_mapping('name', input, input)
+
+    def test_lb_add_del_ip_port_mapping_name_v6(self):
+        input = ('2001:db8::1', '2001:db8::2')
+        expected = (f"[{input[0]}]", f"[{input[1]}]")
+        self._test_lb_add_del_ip_port_mapping('name', input, expected)
 
     def test_hc_get_set_options(self):
         hc_options = {
             'interval': '2',
             'timeout': '10',
             'success_count': '3',
             'failure_count': '3',
@@ -2538,28 +2552,35 @@
 
 class TestBFDOps(OvnNorthboundTest):
 
     def setUp(self):
         super(TestBFDOps, self).setUp()
         self.table = self.api.tables['BFD']
 
+    @staticmethod
+    def _freeze_and_filter_row(row, filter_columns):
+        return types.SimpleNamespace(
+            **{k: v
+               for k, v in idlutils.frozen_row(row)._asdict().items()
+               if k not in filter_columns})
+
     def _bfd_add(self, *args, **kwargs):
         cmd = self.api.bfd_add(*args, **kwargs)
         row = cmd.execute(check_error=True)
         self.assertEqual(cmd.logical_port, row.logical_port)
         self.assertEqual(cmd.dst_ip, row.dst_ip)
         self.assertEqual(cmd.columns['min_tx'] if cmd.columns[
             'min_tx'] else [], row.min_tx)
         self.assertEqual(cmd.columns['min_rx'] if cmd.columns[
             'min_rx'] else [], row.min_rx)
         self.assertEqual(cmd.columns['detect_mult'] if cmd.columns[
             'detect_mult'] else [], row.detect_mult)
         self.assertEqual(cmd.columns['external_ids'] or {}, row.external_ids)
         self.assertEqual(cmd.columns['options'] or {}, row.options)
-        return idlutils.frozen_row(row)
+        return self._freeze_and_filter_row(row, ('status',))
 
     def test_bfd_add(self):
         name = utils.get_rand_name()
         self._bfd_add(name, name)
 
     def test_bfd_add_non_defaults(self):
         name = utils.get_rand_name()
@@ -2629,16 +2650,20 @@
                 ('_uuid', 'status')):
             self.assertEqual(
                 getattr(b1, col),
                 getattr(found[0], col))
 
     def test_bfd_get(self):
         name = utils.get_rand_name()
-        b1 = self.api.bfd_add(name, name).execute(check_error=True)
-        b2 = self.api.bfd_get(b1.uuid).execute(check_error=True)
+        b1 = self._freeze_and_filter_row(
+            self.api.bfd_add(name, name).execute(check_error=True),
+            ('status',))
+        b2 = self._freeze_and_filter_row(
+            self.api.bfd_get(b1.uuid).execute(check_error=True),
+            ('status',))
         self.assertEqual(b1, b2)
 
 
 class TestMirrorOps(OvnNorthboundTest):
 
     def setUp(self):
         super(TestMirrorOps, self).setUp()
```

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_southbound/event.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/event.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_southbound/fixtures.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/fixtures.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/functional/schema/ovn_southbound/test_impl_idl.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/functional/schema/ovn_southbound/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/unit/backend/ovs_idl/test_connection.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_connection.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/unit/backend/ovs_idl/test_helpers.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_helpers.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/unit/backend/ovs_idl/test_idlutils.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_idlutils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/unit/backend/ovs_idl/test_vlog.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/ovs_idl/test_vlog.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/unit/backend/test_ovs_idl.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/unit/backend/test_ovs_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/unit/schema/open_vswitch/test_impl_idl.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/unit/schema/open_vswitch/test_impl_idl.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/unit/test_api.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/unit/test_api.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/unit/test_event.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/unit/test_event.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/unit/test_utils.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/unit/test_utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/tests/utils.py` & `ovsdbapp-2.7.0/ovsdbapp/tests/utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/utils.py` & `ovsdbapp-2.7.0/ovsdbapp/utils.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp/venv.py` & `ovsdbapp-2.7.0/ovsdbapp/venv.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/ovsdbapp.egg-info/PKG-INFO` & `ovsdbapp-2.7.0/ovsdbapp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.2
 Name: ovsdbapp
-Version: 2.6.0
+Version: 2.7.0
 Summary: A library for creating OVSDB applications
 Home-page: https://pypi.org/project/ovsdbapp/
 Author: OpenStack
 Author-email: openstack-discuss@lists.openstack.org
 License: UNKNOWN
 Description: ========
         ovsdbapp
```

### Comparing `ovsdbapp-2.6.0/ovsdbapp.egg-info/SOURCES.txt` & `ovsdbapp-2.7.0/ovsdbapp.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -128,14 +128,15 @@
 releasenotes/notes/provide-address-set-api-3cb387b9e571d4ea.yaml
 releasenotes/notes/provide-lb-hc-api-8ff13ccaf75f1eee.yaml
 releasenotes/notes/provide-lrp-gateway-chassis-api-14e2948183f60cfa.yaml
 releasenotes/notes/provide-lrp-get-method-a33a99a7f86b827e.yaml
 releasenotes/notes/provide-lrp-networks-modifying-1af13589064c12c6.yaml
 releasenotes/source/2023.1.rst
 releasenotes/source/2023.2.rst
+releasenotes/source/2024.1.rst
 releasenotes/source/conf.py
 releasenotes/source/index.rst
 releasenotes/source/pike.rst
 releasenotes/source/queens.rst
 releasenotes/source/rocky.rst
 releasenotes/source/stein.rst
 releasenotes/source/train.rst
```

### Comparing `ovsdbapp-2.6.0/releasenotes/source/conf.py` & `ovsdbapp-2.7.0/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/setup.cfg` & `ovsdbapp-2.7.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/setup.py` & `ovsdbapp-2.7.0/setup.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/tools/coding-checks.sh` & `ovsdbapp-2.7.0/tools/coding-checks.sh`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/tools/debug_venv` & `ovsdbapp-2.7.0/tools/debug_venv`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/tools/debug_venv.py` & `ovsdbapp-2.7.0/tools/debug_venv.py`

 * *Files identical despite different names*

### Comparing `ovsdbapp-2.6.0/tox.ini` & `ovsdbapp-2.7.0/tox.ini`

 * *Files identical despite different names*

