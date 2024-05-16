# Comparing `tmp/deropy-0.2.3.tar.gz` & `tmp/deropy-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deropy-0.2.3.tar", last modified: Fri May 10 13:09:46 2024, max compression
+gzip compressed data, was "deropy-0.3.0.tar", last modified: Thu May 16 09:16:13 2024, max compression
```

## Comparing `deropy-0.2.3.tar` & `deropy-0.3.0.tar`

### file list

```diff
@@ -1,121 +1,133 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:46.310083 deropy-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-05-10 13:09:42.000000 deropy-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-10 13:09:46.310083 deropy-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-10 13:09:42.000000 deropy-0.2.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:46.294083 deropy-0.2.3/deropy/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:46.294083 deropy-0.2.3/deropy/commands/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/commands/configure.py
--rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/commands/deploy.py
--rw-r--r--   0 runner    (1001) docker     (127)     9935 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/commands/generate.py
--rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/commands/simulate.py
--rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/commands/transpile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:46.294083 deropy-0.2.3/deropy/dvm/
--rw-r--r--   0 runner    (1001) docker     (127)     4536 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/Smartcontract.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:46.298083 deropy-0.2.3/deropy/dvm/dast/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/assignement.py
--rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/binaryOperator.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)     1100 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/dast_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/declaration.py
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/functionCall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/functionDef.py
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/goto.py
--rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/ifTest.py
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/name.py
--rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/returns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/variableDeclarationAdnAssignement.py
--rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/dast/whileLoop.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:46.306083 deropy-0.2.3/deropy/dvm/functions/
--rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/AddressRaw.py
--rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/AddressString.py
--rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/AssetValue.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Atoi.py
--rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Blid.py
--rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/BlockHeight.py
--rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/BlockTimestamp.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Delete.py
--rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Dero.py
--rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/DeroValue.py
--rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Exists.py
--rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Function.py
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Hex.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/HexDecode.py
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/IsAddressValid.py
--rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Itoa.py
--rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Keccak256.py
--rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Load.py
--rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/MapDelete.py
--rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/MapExists.py
--rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/MapGet.py
--rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/MapStore.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Panic.py
--rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Random.py
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Scid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/SendAssetToAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/SendDeroToAddress.py
--rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Sha256.py
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Sha3256.py
--rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Signer.py
--rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Store.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Strlen.py
--rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Substr.py
--rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/Txid.py
--rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/UpdateScCode.py
--rw-r--r--   0 runner    (1001) docker     (127)     1573 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/functions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:46.306083 deropy-0.2.3/deropy/dvm/iast/
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/IastNode.py
--rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/argument.py
--rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/assignement.py
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/binaryOperator.py
--rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/compare.py
--rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/constant.py
--rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/functionCall.py
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/functionDef.py
--rw-r--r--   0 runner    (1001) docker     (127)     2735 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/iast_converter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/ifTest.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/name.py
--rw-r--r--   0 runner    (1001) docker     (127)     2028 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/operator.py
--rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/returns.py
--rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/variableDeclarationAdnAssignement.py
--rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/iast/whileLoop.py
--rw-r--r--   0 runner    (1001) docker     (127)     4901 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/parser.py
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/tester.py
--rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/dvm/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/logger.py
--rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:46.310083 deropy-0.2.3/deropy/python_templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/python_templates/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2201 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/python_templates/lottery.py
--rw-r--r--   0 runner    (1001) docker     (127)      591 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/python_templates/minimum_sc.py
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/python_templates/nameservice.py
--rw-r--r--   0 runner    (1001) docker     (127)     1084 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/python_templates/token.py
--rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:46.310083 deropy-0.2.3/deropy/wallet/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/wallet/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3453 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/wallet/derohe_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1448 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/wallet/python_wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/wallet/wallet.py
--rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/wallet/wallet_factory.py
--rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-10 13:09:42.000000 deropy-0.2.3/deropy/wallet/wallet_simulator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:46.310083 deropy-0.2.3/deropy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-10 13:09:46.000000 deropy-0.2.3/deropy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3213 2024-05-10 13:09:46.000000 deropy-0.2.3/deropy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-10 13:09:46.000000 deropy-0.2.3/deropy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-10 13:09:46.000000 deropy-0.2.3/deropy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-10 13:09:46.000000 deropy-0.2.3/deropy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-10 13:09:46.000000 deropy-0.2.3/deropy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-10 13:09:46.310083 deropy-0.2.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      945 2024-05-10 13:09:42.000000 deropy-0.2.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-10 13:09:46.310083 deropy-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-10 13:09:42.000000 deropy-0.2.3/tests/test_compute_storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-10 13:09:42.000000 deropy-0.2.3/tests/test_map_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-10 13:09:42.000000 deropy-0.2.3/tests/test_storage_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:13.717410 deropy-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    34522 2024-05-16 09:16:03.000000 deropy-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-16 09:16:13.717410 deropy-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2671 2024-05-16 09:16:03.000000 deropy-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:13.697409 deropy-0.3.0/deropy/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:13.697409 deropy-0.3.0/deropy/commands/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1398 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/commands/configure.py
+-rw-r--r--   0 runner    (1001) docker     (127)      664 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/commands/deploy.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10633 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/commands/generate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4170 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/commands/simulate.py
+-rw-r--r--   0 runner    (1001) docker     (127)      424 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/commands/transpile.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:13.697409 deropy-0.3.0/deropy/dvm/
+-rw-r--r--   0 runner    (1001) docker     (127)     5053 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/Smartcontract.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:13.701409 deropy-0.3.0/deropy/dvm/dast/
+-rw-r--r--   0 runner    (1001) docker     (127)      564 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      666 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/assignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      979 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/binaryOperator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      561 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      508 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1155 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/dast_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)      823 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/declaration.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/functionCall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1150 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/functionDef.py
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/goto.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1390 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/ifTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)      512 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/returns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1222 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/variableDeclarationAdnAssignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/dast/whileLoop.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:13.709410 deropy-0.3.0/deropy/dvm/functions/
+-rw-r--r--   0 runner    (1001) docker     (127)      969 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/AddressRaw.py
+-rw-r--r--   0 runner    (1001) docker     (127)      883 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/AddressString.py
+-rw-r--r--   0 runner    (1001) docker     (127)      759 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/AssetValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Atoi.py
+-rw-r--r--   0 runner    (1001) docker     (127)      390 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Blid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      533 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/BlockHeight.py
+-rw-r--r--   0 runner    (1001) docker     (127)      472 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/BlockTimestamp.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Delete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      534 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Dero.py
+-rw-r--r--   0 runner    (1001) docker     (127)      557 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/DeroValue.py
+-rw-r--r--   0 runner    (1001) docker     (127)      539 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Exists.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1901 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Function.py
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Hex.py
+-rw-r--r--   0 runner    (1001) docker     (127)      493 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/HexDecode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/IsAddressValid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      577 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Itoa.py
+-rw-r--r--   0 runner    (1001) docker     (127)      596 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Keccak256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      885 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Load.py
+-rw-r--r--   0 runner    (1001) docker     (127)      510 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/MapDelete.py
+-rw-r--r--   0 runner    (1001) docker     (127)      514 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/MapExists.py
+-rw-r--r--   0 runner    (1001) docker     (127)      501 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/MapGet.py
+-rw-r--r--   0 runner    (1001) docker     (127)      663 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/MapStore.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Panic.py
+-rw-r--r--   0 runner    (1001) docker     (127)      574 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Random.py
+-rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Scid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1512 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/SendAssetToAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1358 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/SendDeroToAddress.py
+-rw-r--r--   0 runner    (1001) docker     (127)      524 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Sha256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Sha3256.py
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Signer.py
+-rw-r--r--   0 runner    (1001) docker     (127)      789 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Store.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Strlen.py
+-rw-r--r--   0 runner    (1001) docker     (127)      894 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Substr.py
+-rw-r--r--   0 runner    (1001) docker     (127)      452 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/Txid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      791 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/UpdateScCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/functions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:13.713410 deropy-0.3.0/deropy/dvm/iast/
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/IastNode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      698 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/argument.py
+-rw-r--r--   0 runner    (1001) docker     (127)      714 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/assignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      859 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/binaryOperator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      490 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/comment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      865 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/compare.py
+-rw-r--r--   0 runner    (1001) docker     (127)      506 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/constant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/functionCall.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/functionDef.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3137 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/iast_converter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1097 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/ifTest.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/name.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2185 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/operator.py
+-rw-r--r--   0 runner    (1001) docker     (127)      555 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/returns.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1135 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/variableDeclarationAdnAssignement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      817 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/iast/whileLoop.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6329 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:13.713410 deropy-0.3.0/deropy/dvm/std/
+-rw-r--r--   0 runner    (1001) docker     (127)      153 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/std/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:13.713410 deropy-0.3.0/deropy/dvm/std/basic/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/std/basic/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/std/basic/decrement.bas
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/std/basic/increment.bas
+-rw-r--r--   0 runner    (1001) docker     (127)      476 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/std/basic/updateCode.bas
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/std/decrement.py
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/std/increment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      801 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/std/updateCode.py
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/tester.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1605 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/dvm/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/logger.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:13.713410 deropy-0.3.0/deropy/python_templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/python_templates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2064 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/python_templates/lottery.py
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/python_templates/minimum_sc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      784 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/python_templates/nameservice.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/python_templates/token.py
+-rw-r--r--   0 runner    (1001) docker     (127)      404 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)      735 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:13.713410 deropy-0.3.0/deropy/wallet/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/wallet/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3814 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/wallet/derohe_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1527 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/wallet/python_wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1413 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/wallet/wallet.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1113 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/wallet/wallet_factory.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1594 2024-05-16 09:16:03.000000 deropy-0.3.0/deropy/wallet/wallet_simulator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:13.713410 deropy-0.3.0/deropy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3269 2024-05-16 09:16:13.000000 deropy-0.3.0/deropy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3518 2024-05-16 09:16:13.000000 deropy-0.3.0/deropy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 09:16:13.000000 deropy-0.3.0/deropy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-05-16 09:16:13.000000 deropy-0.3.0/deropy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      128 2024-05-16 09:16:13.000000 deropy-0.3.0/deropy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-05-16 09:16:13.000000 deropy-0.3.0/deropy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 09:16:13.717410 deropy-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      992 2024-05-16 09:16:03.000000 deropy-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 09:16:13.713410 deropy-0.3.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4150 2024-05-16 09:16:03.000000 deropy-0.3.0/tests/test_compute_storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-05-16 09:16:03.000000 deropy-0.3.0/tests/test_map_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1478 2024-05-16 09:16:03.000000 deropy-0.3.0/tests/test_storage_functions.py
```

### Comparing `deropy-0.2.3/LICENSE` & `deropy-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/PKG-INFO` & `deropy-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.2.3
+Version: 0.3.0
 Summary: A set of tool to help of DERO smart contract development
 Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deropy-0.2.3/README.md` & `deropy-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/commands/configure.py` & `deropy-0.3.0/deropy/commands/configure.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/commands/deploy.py` & `deropy-0.3.0/deropy/commands/deploy.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/commands/generate.py` & `deropy-0.3.0/deropy/commands/generate.py`

 * *Files 8% similar despite different names*

```diff
@@ -88,18 +88,19 @@
 
 def _generate_class(file: str, scid: str, output: str = None):
     file_content = _read_bas(file)
     functions = _parse_function(file_content)
 
     output_path = output if output is not None else 'SC.py'
 
+    # retrieve the exact name of the class from the file
     class_name = os.path.basename(file)
     class_name = class_name.split('.')[0]
     class_name = class_name.capitalize()
-
+            
     lines = ['import requests']
     lines += ['import json\n']
     lines += [f'class {class_name}:']
     lines += [f'    SCID="{scid}"']
     lines += ['    def __init__(self):']
     lines += [f"        self.url = '{simulator_host}/json_rpc'"]
     lines += ["        self.headers = {'content-type': 'application/json'}"]
@@ -164,30 +165,43 @@
         '                "code": True,',
         '                "variables": True',
         '            }',
         '        }',
         '        response = requests.post(url, data=json.dumps(payload), headers=self.headers)',
         '        # keep only the `stringkeys` and `variables`',
         '        data = response.json()',
-        '        self.storage = data["result"]["stringkeys"]',
+        '        stringkeys = data["result"]["stringkeys"]',
+        '        # for each key, if it is a string, decode the hex string to a string',
+        '        for k, v in stringkeys.items():',
+        '            if k == "C":',
+        '                continue',
+        '            if isinstance(v, str):',
+        '                try:',
+        '                    stringkeys[k] = bytes.fromhex(v).decode("utf-8")',
+        '                except:',
+        '                    pass',
+        '        # store the result and overwrite C',
+        '        stringkeys["C"] = ""',
+        '        self.storage = stringkeys',
+
         '        return self.storage',
     ]
 
 
 def _generate_method_scinvoce(f_name, p, class_name):
     # create the method definition
     method_parameters = ''
     for k, v in p.items():
         method_parameters += f'{k}: {_SC_type_to_python_type(v)}, '
     method_parameters = method_parameters[:-2]
 
     if len(method_parameters) == 0:
-        lines = [f'\n    def {f_name}(self, dero_deposit: int = 0, asset_deposit: int = 0, host: str = None):']
+        lines = [f'\n    def {f_name}(self, dero_deposit: int = 0, asset_deposit: tuple = (0, ), host: str = None):']
     else:
-        lines = [f'\n    def {f_name}(self, {method_parameters}, dero_deposit: int = 0, asset_deposit: int = 0, host: str = None):']
+        lines = [f'\n    def {f_name}(self, {method_parameters}, dero_deposit: int = 0, asset_deposit: tuple = (0, ), host: str = None):']
 
     scrpc = [
         '                    "sc_rpc": [',
         '                        {',
         '                            "name": "entrypoint",',
         '                            "datatype": "S",',
         f'                            "value": "{f_name}"',
@@ -211,15 +225,15 @@
         '                "params": {',
         f'                    "scid": {class_name}.SCID,',
         '                    "ringsize": 2,',
     ]
     if f_name != 'Initialize':
         payload += [
             '                    "sc_dero_deposit": dero_deposit,',
-            '                    "sc_asset_deposit": asset_deposit,',
+            '                    "sc_token_deposit": asset_deposit[0] if asset_deposit is not None else 0,',
         ]
     payload += scrpc
     payload += [
         '                    ]',
         '                }',
         '            }',
     ]
```

### Comparing `deropy-0.2.3/deropy/commands/simulate.py` & `deropy-0.3.0/deropy/commands/simulate.py`

 * *Files 4% similar despite different names*

```diff
@@ -129,15 +129,19 @@
             print(line.decode(), end='')
             if expected in line.decode():
                 break
             if timeout == 0:
                 break
             timeout -= 0.1
 
+
 def read_until_empty(q):
+    print("\n\n\n")
+    print("Reading the output from the simulator")
+    print("\n\n\n")
     while True:
         try:
             line = q.get_nowait()
         except Empty:
             break
         else:
             print(line.decode(), end='')
```

### Comparing `deropy-0.2.3/deropy/dvm/Smartcontract.py` & `deropy-0.3.0/deropy/dvm/Smartcontract.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,34 +2,34 @@
 import functools
 import time
 
 from deropy.dvm.utils import print_red
 
 
 class SmartContract:
-    scid = None
+    SCID = None
     active_wallet = None
     public_functions = []
     max_compute_gaz = 10_000_000
     max_storage_gas = 20_000
     dero_value = None
     asset_value = None
 
     # Blockchain basic component simulation
     blocks = []
     transactions = []
-    scid = sha256(str(time.time()).encode()).hexdigest()
+    SCID = sha256(str(time.time()).encode()).hexdigest()
 
     def __new__(cls):
         if not hasattr(cls, 'instance'):
             cls.instance = super(SmartContract, cls).__new__(cls)
             cls.instance._initialize()
 
-        if SmartContract.scid is None:
-            SmartContract.scid = sha256(str(time.time()*2).encode()).hexdigest()
+        if SmartContract.SCID is None:
+            SmartContract.SCID = sha256(str(time.time()*2).encode()).hexdigest()
 
         return cls.instance
 
     @classmethod
     def get_instance(cls):
         if not hasattr(cls, 'instance'):
             cls.instance = super(SmartContract, cls).__new__(cls)
@@ -39,19 +39,39 @@
     def _initialize(self):
         SmartContract.storage = dict()
         SmartContract.memory = dict()
         SmartContract.gasStorage = []
         SmartContract.gasCompute = []
 
         # At first instanciaion, create the smart-contract Id
-        if SmartContract.scid is None:
-            SmartContract.scid = sha256(str(time.time()*2).encode()).hexdigest()
+        if SmartContract.SCID is None:
+            SmartContract.SCID = sha256(str(time.time()*2).encode()).hexdigest()
+
+    @staticmethod
+    def reset():
+        SmartContract.storage = dict()
+        SmartContract.memory = dict()
+        SmartContract.gasStorage = []
+        SmartContract.gasCompute = []
+        SmartContract.SCID = None
 
     def read(self):
-        return SmartContract.storage
+        storage = SmartContract.storage
+
+        for k, v in storage.items():
+            if k == "C":
+                continue
+            if isinstance(v, str):
+                try:
+                    storage[k] = bytes.fromhex(v).decode("utf-8")
+                except:
+                    pass
+        return storage
+
+        # return SmartContract.storage
 
     def store(self, key, value):
         SmartContract.storage[key] = value
 
     def load(self, key):
         return SmartContract.storage[key]
 
@@ -66,25 +86,24 @@
 
         SmartContract.asset_value[asset_id] = amount
 
 
 def isPublic(func):
     # A public method is one called during a transaction, therefore we should create a txid and store into a block
     def public_function(*args, **kwargs):
-        sc = SmartContract.get_instance()
 
         # Create a transaction id and block id
         txid = sha256(str(time.time()).encode()).hexdigest()
         blockid = sha256(str(time.time()).encode()).hexdigest()
 
         # Store the transaction and the block
         SmartContract.transactions.append({
             "txid": txid,
             "blockid": blockid,
-            "scid": sc.scid,
+            "scid": SmartContract.SCID,
             "func": func.__name__,
             "args": args,
             "kwargs": kwargs
         })
         SmartContract.blocks.append(blockid)
 
         # Call the function
```

### Comparing `deropy-0.2.3/deropy/dvm/dast/__init__.py` & `deropy-0.3.0/deropy/dvm/iast/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,15 +1,15 @@
-from .assignement import Assignment
-from .declaration import VariableDeclaration
+from .IastNode import IastNode
+from .returns import Return
+from .constant import Constant
+from .name import Name
 from .variableDeclarationAdnAssignement import VariableDeclarationAndAssignment
+from .assignement import Assignment
 from .functionCall import FunctionCall
 from .functionDef import FunctionDef
-from .constant import Constant
-from .name import Name
-from .returns import Return
 from .ifTest import IfTest
 from .compare import Compare
 from .operator import Operator
 from .binaryOperator import BinaryOperator
 from .argument import Argument
-from .goto import Goto
-from .whileLoop import WhileLoop
+from .whileLoop import WhileLoop
+from .comment import Comment
```

### Comparing `deropy-0.2.3/deropy/dvm/dast/argument.py` & `deropy-0.3.0/deropy/dvm/dast/argument.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/dast/assignement.py` & `deropy-0.3.0/deropy/dvm/dast/assignement.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/dast/binaryOperator.py` & `deropy-0.3.0/deropy/dvm/dast/binaryOperator.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/dast/compare.py` & `deropy-0.3.0/deropy/dvm/dast/compare.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/dast/dast_converter.py` & `deropy-0.3.0/deropy/dvm/dast/dast_converter.py`

 * *Files 14% similar despite different names*

```diff
@@ -14,13 +14,14 @@
         "IfTest": dast.IfTest.from_intermediate_ast,
         "Operator": dast.Operator.from_intermediate_ast,
         "Argument": dast.Argument.from_intermediate_ast,
         "BinaryOperator": dast.BinaryOperator.from_intermediate_ast,
         "Assignment": dast.Assignment.from_intermediate_ast,
         "Goto": dast.Goto.from_intermediate_ast,
         "WhileLoop": dast.WhileLoop.from_intermediate_ast,
+        "Comment": dast.Comment.from_intermediate_ast,
     }
     json_type = json_object["type"]
     if json_type in type_mapping:
         return type_mapping[json_type](json_object)
     else:
         raise Exception(f"Unknown type: {json_type}")
```

### Comparing `deropy-0.2.3/deropy/dvm/dast/declaration.py` & `deropy-0.3.0/deropy/dvm/dast/declaration.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/dast/functionCall.py` & `deropy-0.3.0/deropy/dvm/dast/functionCall.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import json, ast, inspect
 
+from deropy.dvm.functions import __all__ as all_functions
 import deropy.dvm.dast.dast_converter as dast_converter
 
 
 class FunctionCall():
     def __init__(self, name, args):
         self.name = name
         self.args = args
@@ -43,12 +44,15 @@
         for a in self.args:
             if isinstance(a, str):
                 str_args.append(f'"{a}"')
                 continue
         
             str_args.append(str(a))
         
-        return f"{self.name.upper()}({', '.join([a for a in str_args])})"
+        function_name = self.name
+        if function_name in all_functions:
+            function_name = self.name.upper()
+        return f"{function_name}({', '.join([a for a in str_args])})"
     
     def __repr__(self):
         return str(self)
```

### Comparing `deropy-0.2.3/deropy/dvm/dast/functionDef.py` & `deropy-0.3.0/deropy/dvm/dast/functionDef.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/dast/ifTest.py` & `deropy-0.3.0/deropy/dvm/dast/ifTest.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/dast/operator.py` & `deropy-0.3.0/deropy/dvm/dast/operator.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/dast/returns.py` & `deropy-0.3.0/deropy/dvm/dast/returns.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/dast/variableDeclarationAdnAssignement.py` & `deropy-0.3.0/deropy/dvm/dast/variableDeclarationAdnAssignement.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/dast/whileLoop.py` & `deropy-0.3.0/deropy/dvm/dast/whileLoop.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/AddressRaw.py` & `deropy-0.3.0/deropy/dvm/functions/AddressRaw.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/AddressString.py` & `deropy-0.3.0/deropy/dvm/functions/AddressString.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/AssetValue.py` & `deropy-0.3.0/deropy/dvm/functions/AssetValue.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/Atoi.py` & `deropy-0.3.0/deropy/dvm/functions/Atoi.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/BlockHeight.py` & `deropy-0.3.0/deropy/dvm/functions/BlockHeight.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/Dero.py` & `deropy-0.3.0/deropy/dvm/functions/Dero.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/DeroValue.py` & `deropy-0.3.0/deropy/dvm/functions/DeroValue.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/Exists.py` & `deropy-0.3.0/deropy/dvm/functions/Exists.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/Function.py` & `deropy-0.3.0/deropy/dvm/functions/Function.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/IsAddressValid.py` & `deropy-0.3.0/deropy/dvm/functions/IsAddressValid.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/Itoa.py` & `deropy-0.3.0/deropy/dvm/functions/Itoa.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/Keccak256.py` & `deropy-0.3.0/deropy/dvm/functions/Keccak256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/Load.py` & `deropy-0.3.0/deropy/dvm/functions/Load.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/MapExists.py` & `deropy-0.3.0/deropy/dvm/functions/MapExists.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/MapStore.py` & `deropy-0.3.0/deropy/dvm/functions/MapStore.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/Random.py` & `deropy-0.3.0/deropy/dvm/functions/Random.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/Scid.py` & `deropy-0.3.0/deropy/dvm/functions/Sha3256.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 from deropy.dvm.functions.Function import Function
-from deropy.dvm.Smartcontract import SmartContract
+import hashlib
 
 
-class Scid(Function):
+class Sha3256(Function):
     def __init__(self):
         func_parameters = {
-            'value': {"type": "int", "value": None},
+            "s": {"type": "str", "value": None},
         }
-        super().__init__("scid", 2000, 0, func_parameters)
+        super().__init__("sha3256", 25_000, 0, func_parameters)
 
     def _exec(self, *args, **kwargs):
-        value = SmartContract.scid
-        self.parameters['value']['value'] = value
-        return value
+        self.parameters["s"]["value"] = kwargs["s"]
+        return hashlib.sha3_256(kwargs["s"].encode()).hexdigest()
 
     def _computeGasStorageCost(self):
         return 0
 
 
-def scid():
-    return Scid()()
+def sha3256(s: str):
+    return Sha3256()(s=s)
```

### Comparing `deropy-0.2.3/deropy/dvm/functions/SendAssetToAddress.py` & `deropy-0.3.0/deropy/dvm/functions/SendAssetToAddress.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/SendDeroToAddress.py` & `deropy-0.3.0/deropy/dvm/functions/SendDeroToAddress.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/Sha256.py` & `deropy-0.3.0/deropy/dvm/functions/Sha256.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/Sha3256.py` & `deropy-0.3.0/deropy/dvm/functions/UpdateScCode.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 from deropy.dvm.functions.Function import Function
-import hashlib
 
 
-class Sha3256(Function):
+class UpdateScCode(Function):
     def __init__(self):
         func_parameters = {
-            "s": {"type": "str", "value": None},
+            "sc_code": {"type": "str", "value": None},
         }
-        super().__init__("sha3256", 25_000, 0, func_parameters)
-
-    def _exec(self, *args, **kwargs):
-        self.parameters["s"]["value"] = kwargs["s"]
-        return hashlib.sha3_256(kwargs["s"].encode()).hexdigest()
+        super().__init__("update_sc_code", 5000, 0, func_parameters)
 
     def _computeGasStorageCost(self):
+        if isinstance(self.parameters["sc_code"]["value"], int):
+            return 1
+        else:
+            size = len(self.parameters["sc_code"]["value"])
+            return size * 2  # 2 gas per byte (1 for tx, 1 for storage)
+
+    def _exec(self, *args, **kwargs):
+        self.parameters["sc_code"]["value"] = kwargs["sc_code"]
+        self.sc.storage["code"] = kwargs["sc_code"]
         return 0
 
 
-def sha3256(s: str):
-    return Sha3256()(s=s)
+def update_sc_code(sc_code: str):
+    return UpdateScCode()(sc_code=sc_code)
```

### Comparing `deropy-0.2.3/deropy/dvm/functions/Signer.py` & `deropy-0.3.0/deropy/dvm/functions/Signer.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/Store.py` & `deropy-0.3.0/deropy/dvm/functions/Store.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/Substr.py` & `deropy-0.3.0/deropy/dvm/functions/Substr.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/functions/__init__.py` & `deropy-0.3.0/deropy/dvm/functions/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,16 +23,16 @@
 from .DeroValue import derovalue
 from .AssetValue import assetvalue
 from .Atoi import atoi
 from .Itoa import itoa
 from .Sha256 import sha256
 from .Sha3256 import sha3256
 from .Keccak256 import keccak256
-from .Hex import _hex
-from .HexDecode import hex_decode
+from .Hex import hex
+from .HexDecode import hexdecode
 from .Strlen import strlen
 from .Substr import substr
 from .Panic import panic
 
 __all__ = [
     delete,
     exists,
@@ -59,13 +59,13 @@
     derovalue,
     assetvalue,
     atoi,
     itoa,
     sha256,
     sha3256,
     keccak256,
-    _hex,
-    hex_decode,
+    hex,
+    hexdecode,
     strlen,
     substr,
     panic,
 ]
```

### Comparing `deropy-0.2.3/deropy/dvm/iast/argument.py` & `deropy-0.3.0/deropy/dvm/iast/argument.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/iast/assignement.py` & `deropy-0.3.0/deropy/dvm/iast/assignement.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/iast/binaryOperator.py` & `deropy-0.3.0/deropy/dvm/iast/binaryOperator.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/iast/compare.py` & `deropy-0.3.0/deropy/dvm/iast/compare.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/iast/functionCall.py` & `deropy-0.3.0/deropy/dvm/iast/functionCall.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/iast/functionDef.py` & `deropy-0.3.0/deropy/dvm/iast/functionDef.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/iast/iast_converter.py` & `deropy-0.3.0/deropy/dvm/iast/iast_converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 import ast
 
 import deropy.dvm.iast as iast
 
 
 def to_iast(node):
-    if isinstance(node, list):
-        return [to_iast(n) for n in node]
-
     if isinstance(node, ast.ClassDef):
         pass
 
+    if isinstance(node, list):
+        return [to_iast(n) for n in node]
+
     if isinstance(node, ast.If):
         return iast.IfTest.from_python_ast("if", node)
 
     if isinstance(node, ast.While):
         return iast.WhileLoop.from_python_ast(node)
 
     if isinstance(node, ast.Compare):
@@ -34,14 +34,17 @@
 
     if isinstance(node, ast.Call):
         return iast.FunctionCall.from_python_ast(node)
 
     if isinstance(node, ast.Expr):
         if isinstance(node.value, ast.Call):
             return iast.FunctionCall.from_python_ast(node.value)
+        if isinstance(node.value, ast.Constant):
+            if isinstance(node.value.value, str):
+                return iast.Comment.from_python_ast(node)
 
     if isinstance(node, ast.FunctionDef):
         body = []
         for b in node.body:
             p = to_iast(b)
             if p is not None:
                 body.append(p)
@@ -79,9 +82,15 @@
         return iast.Operator.from_python_ast(node)
     if isinstance(node, ast.Sub):
         return iast.Operator.from_python_ast(node)
     if isinstance(node, ast.Mult):
         return iast.Operator.from_python_ast(node)
     if isinstance(node, ast.Div):
         return iast.Operator.from_python_ast(node)
+    if isinstance(node, ast.BitAnd):
+        return iast.Operator.from_python_ast(node)
+    if isinstance(node, ast.BitOr):
+        return iast.Operator.from_python_ast(node)
 
+    print('Unknown node type:', type(node))
+    print(ast.dump(node))
     raise Exception(f'Unknown node type: {type(node)}')
```

### Comparing `deropy-0.2.3/deropy/dvm/iast/ifTest.py` & `deropy-0.3.0/deropy/dvm/iast/ifTest.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/iast/operator.py` & `deropy-0.3.0/deropy/dvm/iast/operator.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,14 +30,18 @@
             return cls("+")._invert()
         if isinstance(node, ast.Sub):
             return cls("-")._invert()
         if isinstance(node, ast.Mult):
             return cls("*")._invert()
         if isinstance(node, ast.Div):
             return cls("/")._invert()
+        if isinstance(node, ast.BitAnd):
+            return cls("&")._invert()
+        if isinstance(node, ast.BitOr):
+            return cls("|")._invert()
         else:
             raise ValueError(f"Unknown operator: {node}")
         
     def _invert(self):
         if self.value == "==":
             self.value = "!="
         elif self.value == "!=":
```

### Comparing `deropy-0.2.3/deropy/dvm/iast/returns.py` & `deropy-0.3.0/deropy/dvm/iast/returns.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/iast/variableDeclarationAdnAssignement.py` & `deropy-0.3.0/deropy/dvm/iast/variableDeclarationAdnAssignement.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/iast/whileLoop.py` & `deropy-0.3.0/deropy/dvm/iast/whileLoop.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/parser.py` & `deropy-0.3.0/deropy/dvm/parser.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,59 @@
 import inspect
 import json
 import ast
 import sys
+import os
+
 
 import deropy.dvm.iast.iast_converter as iast_converter
 import deropy.dvm.dast as dast
+import deropy.dvm.std as std
 from deropy.dvm.dast import *
 from deropy.dvm.utils import flatten_list
 
 
+standard_library_functions = []
+header_comment = []
+
+
 def load_dast(str_func_name, obj):
     return globals()[str_func_name].from_intermediate_ast(obj)
 
 
+def load_std_function(import_line):
+    function_names = import_line.split("import ")[1]
+    function_names = function_names.replace('\n', '')
+
+    if ',' in function_names:
+        function_names = function_names.split(',')
+    else:
+        function_names = [function_names]
+
+    for func in function_names:
+        func = func.strip()
+        root_directory = os.path.dirname(inspect.getfile(std))
+        std_basic_path = os.path.join(root_directory, 'basic')
+
+        with open(os.path.join(std_basic_path, f'{func}.bas'), 'r') as fi:
+            code = fi.readlines()
+            code.append('\n')
+
+        standard_library_functions.append(code)
+
+
 def file_to_iast(path):
     with open(path, "r") as f:
         code = f.readlines()
 
+    # Collect all the standard library functions
+    for line in code:
+        if "deropy.dvm.std" in line:
+            load_std_function(line)
+
     # remove all lines that are comments, or imports
     code = [line for line in code if not line.startswith("#") and not line.startswith("import") and not line.startswith("from")]
     code = [line for line in code if line.strip() != ""]
 
     # remove all str( ... ) call but keep what's inside the parenthesis
     i = 0
     while i < len(code):
@@ -28,14 +61,17 @@
         if 'str(' in line:
             start = line.index('str(')
             end = line.index(')', start)
             inside = line[start+4:end]
             code[i] = line[:start] + inside + line[end+1:]
         i += 1
 
+    # remove all the self. from the code
+    code = [line.replace('self.', '') for line in code]
+
     code = "".join(code)
     tree = ast.parse(code)
 
     return tree_to_iast(tree)
 
 
 def code_to_iast(code):
@@ -52,25 +88,29 @@
 
     return parsed
 
 
 def parse(path, output_path=None):
     parsed = file_to_iast(path)
 
-    # if output_path exists, overwrite it
-    if output_path is not None:
-        with open(output_path, 'w') as f:
-            f.write('')
+    if output_path is None:
+        output_path = path.replace(".py", ".bas")
 
-    for f in parsed:
-        func_dvm = []
+    all_functions = []
 
+    for f in parsed:
+            
         json_function = json.loads(f.to_json())
 
         func = load_dast(json_function["type"], json_function)
+
+        if isinstance(func, Comment):
+            header_comment.append(str(func))
+            continue
+
         flatten_func_body = []
         for b in func.body:
             if isinstance(b, list):
                 for l in b:
                     flatten_func_body.append(l)
                 continue
             flatten_func_body.append(b)
@@ -120,30 +160,44 @@
                 before_while.extend(flatten_list(b["body"]))
                 before_while.append(if_json_iast)
                 before_while.extend(after_while)
                 flatten_func_body = before_while
 
             i += 1
 
-        # print the DVM-BASIC code
-        print(func)
-        for i, b in enumerate(flatten_func_body):
+        all_functions.append((func, flatten_func_body))
+
+    # print the DVM-BASIC code
+    # first the header comment
+    for hc in header_comment:
+        print(hc)
+
+    for func_name, func_body in all_functions:
+        print(func_name)
+        for i, b in enumerate(func_body):
             print(f'{i+1} {load_dast(b["type"], b)}')
         print('End Function\n')
 
-        # Write the DVM-BASIC code to a file
-        if output_path is None:
-            output_path = path.split('.')[0] + '.bas'
-
-        with open(output_path, 'a') as f:
-            f.write(f'{func}\n')
-            for i, b in enumerate(flatten_func_body):
+    for std_func in standard_library_functions:
+        print(''.join(std_func))
+
+    with open(output_path, 'w') as f:
+        # first the header comment
+        for hc in header_comment:
+            f.write(hc)
+        f.write('\n')
+        for func_name, func_body in all_functions:
+            f.write(f'{func_name}\n')
+            for i, b in enumerate(func_body):
                 f.write(f'{i+1} {load_dast(b["type"], b)}\n')
             f.write('End Function\n\n')
 
+        for std_func in standard_library_functions:
+            f.write(''.join(std_func))
+
 
 if __name__ == "__main__":
     if len(sys.argv) < 2:
         print("Usage: python parser.py <path_to_file>")
         sys.exit(1)
 
     print('\n')
```

### Comparing `deropy-0.2.3/deropy/dvm/tester.py` & `deropy-0.3.0/deropy/dvm/tester.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/dvm/utils.py` & `deropy-0.3.0/deropy/dvm/utils.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/main.py` & `deropy-0.3.0/deropy/main.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/python_templates/lottery.py` & `deropy-0.3.0/deropy/python_templates/lottery.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
-from deropy.dvm.functions import exists, store, derovalue, load, signer, random, send_dero_to_address, address_raw, update_sc_code
+from deropy.dvm.functions import exists, store, derovalue, load, signer, random, send_dero_to_address, address_raw
 from deropy.dvm.Smartcontract import SmartContract, logger, sc_logger
+from deropy.dvm.std import updateCode
 
 
 @sc_logger(logger)
 class Lottery(SmartContract):
     def Initialize(self) -> int:
         if exists('owner') == 0:
             store('owner', signer())
@@ -59,14 +60,7 @@
 
     def Withdraw(self, amount: int) -> int:
         if load('owner') != signer():
             return 1
 
         send_dero_to_address(signer(), amount)
         return 0
-
-    def UpdateCode(self, new_code: str) -> int:
-        if load('owner') != signer():
-            return 1
-
-        update_sc_code(new_code)
-        return 0
```

### Comparing `deropy-0.2.3/deropy/python_templates/minimum_sc.py` & `deropy-0.3.0/deropy/python_templates/minimum_sc.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from deropy.dvm.functions import store, load, signer, exists, update_sc_code
 from deropy.dvm.Smartcontract import SmartContract, logger, sc_logger
+from deropy.dvm.std import updateCode
 
 
 @sc_logger(logger)
 class Minimal(SmartContract):
     def Initialize(self) -> int:
         print(exists("owner"))
         if exists("owner") == 0:
```

### Comparing `deropy-0.2.3/deropy/python_templates/nameservice.py` & `deropy-0.3.0/deropy/python_templates/nameservice.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from deropy.dvm.functions import exists, store, load, strlen, signer, address_raw
 from deropy.dvm.Smartcontract import SmartContract, logger, sc_logger
+from deropy.dvm.std import updateCode
 
 
 @sc_logger(logger)
 class NameService(SmartContract):
     def Initialize(self) -> int:
         return 0
```

### Comparing `deropy-0.2.3/deropy/python_templates/token.py` & `deropy-0.3.0/deropy/python_templates/token.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from deropy.dvm.functions import exists, store, load, derovalue, assetvalue, signer, address_raw, send_dero_to_address
 from deropy.dvm.functions import send_asset_to_address, scid
 from deropy.dvm.Smartcontract import SmartContract, logger, sc_logger
+from deropy.dvm.std import updateCode
 
 
 @sc_logger(logger)
 class Token(SmartContract):
     def InitializePrivate(self) -> int:
         if exists("owner") == 0:
             store("owner", signer())
```

### Comparing `deropy-0.2.3/deropy/utils.py` & `deropy-0.3.0/deropy/utils.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/wallet/derohe_wallet.py` & `deropy-0.3.0/deropy/wallet/derohe_wallet.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,21 +4,21 @@
 
 from deropy.utils import active_waiting
 from deropy.wallet.wallet import Wallet
 
 
 class DeroheWallet(Wallet):
     def __init__(self, name, id):
-        super().__init__(self, name, id)
+        super().__init__(name, id)
 
     def _init(self):
         wallet_port = 30000 + self.id
         self.rpc_host = f'http://127.0.0.1:{wallet_port}/json_rpc'
 
-    def _simulator_init(self):
+        self.logger.info(f'Fetching wallet information for "{self.name}"')
         self.string_address = self._get_string_address()
         self.raw_address = self._get_raw_address()
 
         self.logger.info(f'Wallet "{self.name}" created: {self.string_address} - {self.raw_address} - "{self.name}')
         self.balance = {}
 
     def _get_string_address(self):
@@ -26,14 +26,17 @@
             "jsonrpc": "2.0",
             "id": "1",
             "method": "GetAddress"
         }
         response = requests.post(self.rpc_host, json=payload).json()
         return response['result']['address']
 
+    def get_raw_address(self):
+        return self.raw_address
+
     def _get_raw_address(self):
         def register(self, timeout=0):
             payload = {
                 "jsonrpc": "2.0",
                 "id": "1",
                 "method": "scinvoke",
                 "params": {
@@ -77,15 +80,24 @@
             response = requests.post(url, json=payload).json()
             return response['result']['stringkeys'][self.name]
 
         register(self)
         return get_raw_address(self)
 
     def get_balance(self, token):
-        return self.balance.get(token, 0)
+        payload = {
+            "jsonrpc": "2.0",
+            "id": "1",
+            "method": "GetBalance",
+            "params": {
+                "scid": token
+            }
+        }
+        response = requests.post(self.rpc_host, json=payload).json()
+        return response['result']['balance']
 
     def set_balance(self, token, amount):
         self.balance[token] = amount
 
     def invoke_sc_function(self, func, func_args: tuple = None, dero_deposit: int = None, asset_deposit: tuple = None):
         super().invoke_sc_function(func, func_args, dero_deposit, asset_deposit)
         args = [] if func_args is None else (func_args, ) if isinstance(func_args, (int, str)) else func_args
```

### Comparing `deropy-0.2.3/deropy/wallet/python_wallet.py` & `deropy-0.3.0/deropy/wallet/python_wallet.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,31 +13,32 @@
         self.string_address = hashlib.sha256(str(self.name).encode()).hexdigest()
         self.raw_address = self.string_address[:33]
         self.balance = {}
 
     def _get_string_address(self):
         return self.string_address
 
-    def _get_raw_address(self):
-        return self.raw_address
+    def get_raw_address(self):
+        # return self.raw_address
+        return "".join("{:02x}".format(c) for c in self.raw_address.encode())
 
     def get_balance(self, token):
         return self.balance.get(token, 0)
 
     def set_balance(self, token, amount):
         self.balance[token] = amount
 
     def invoke_sc_function(self, func, func_args: tuple = None, dero_deposit: int = None, asset_deposit: tuple = None):
         super().invoke_sc_function(func, func_args, dero_deposit, asset_deposit)
 
         # Wallet balance is consumed the dero or / and asset deposit
         # if dero_deposit is not None:
         #     self.balance["DERO"] -= dero_deposit
         if asset_deposit is not None:
-            self.balance[SmartContract.scid] -= asset_deposit[0]
+            self.balance[SmartContract.SCID] -= asset_deposit[0]
 
         args = [] if func_args is None else (func_args, ) if isinstance(func_args, (int, str)) else func_args
         result = func(*args)
 
         # deposit is burned by the smart-contract
         SmartContract.dero_value = None
         SmartContract.asset_value = None
```

### Comparing `deropy-0.2.3/deropy/wallet/wallet.py` & `deropy-0.3.0/deropy/wallet/wallet.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/wallet/wallet_factory.py` & `deropy-0.3.0/deropy/wallet/wallet_factory.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy/wallet/wallet_simulator.py` & `deropy-0.3.0/deropy/wallet/wallet_simulator.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/deropy.egg-info/PKG-INFO` & `deropy-0.3.0/deropy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deropy
-Version: 0.2.3
+Version: 0.3.0
 Summary: A set of tool to help of DERO smart contract development
 Home-page: https://github.com/dero-hyperbolic/deropy.git
 Author-email: leocances@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `deropy-0.2.3/deropy.egg-info/SOURCES.txt` & `deropy-0.3.0/deropy.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 deropy/dvm/parser.py
 deropy/dvm/tester.py
 deropy/dvm/utils.py
 deropy/dvm/dast/__init__.py
 deropy/dvm/dast/argument.py
 deropy/dvm/dast/assignement.py
 deropy/dvm/dast/binaryOperator.py
+deropy/dvm/dast/comment.py
 deropy/dvm/dast/compare.py
 deropy/dvm/dast/constant.py
 deropy/dvm/dast/dast_converter.py
 deropy/dvm/dast/declaration.py
 deropy/dvm/dast/functionCall.py
 deropy/dvm/dast/functionDef.py
 deropy/dvm/dast/goto.py
@@ -77,25 +78,34 @@
 deropy/dvm/functions/UpdateScCode.py
 deropy/dvm/functions/__init__.py
 deropy/dvm/iast/IastNode.py
 deropy/dvm/iast/__init__.py
 deropy/dvm/iast/argument.py
 deropy/dvm/iast/assignement.py
 deropy/dvm/iast/binaryOperator.py
+deropy/dvm/iast/comment.py
 deropy/dvm/iast/compare.py
 deropy/dvm/iast/constant.py
 deropy/dvm/iast/functionCall.py
 deropy/dvm/iast/functionDef.py
 deropy/dvm/iast/iast_converter.py
 deropy/dvm/iast/ifTest.py
 deropy/dvm/iast/name.py
 deropy/dvm/iast/operator.py
 deropy/dvm/iast/returns.py
 deropy/dvm/iast/variableDeclarationAdnAssignement.py
 deropy/dvm/iast/whileLoop.py
+deropy/dvm/std/__init__.py
+deropy/dvm/std/decrement.py
+deropy/dvm/std/increment.py
+deropy/dvm/std/updateCode.py
+deropy/dvm/std/basic/__init__.py
+deropy/dvm/std/basic/decrement.bas
+deropy/dvm/std/basic/increment.bas
+deropy/dvm/std/basic/updateCode.bas
 deropy/python_templates/__init__.py
 deropy/python_templates/lottery.py
 deropy/python_templates/minimum_sc.py
 deropy/python_templates/nameservice.py
 deropy/python_templates/token.py
 deropy/wallet/__init__.py
 deropy/wallet/derohe_wallet.py
```

### Comparing `deropy-0.2.3/setup.py` & `deropy-0.3.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from setuptools import setup, find_packages
 
 setup(
     name='deropy',
-    version=os.getenv('DEROPY_VERSION') or '0.2.3',
+    version=os.getenv('DEROPY_VERSION') or '0.3.0',
     url='https://github.com/dero-hyperbolic/deropy.git',
     author_email='leocances@gmail.com',
     description='A set of tool to help of DERO smart contract development',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     packages=find_packages(),
     install_requires=[
@@ -16,15 +16,17 @@
         'coloredlogs==15.0.1',
         'pyperclip==1.8.2',
         'python-dotenv==0.20.0',
         'InquirerPy==0.3.4',
         'pycryptodome==3.20.0',
     ],
     include_package_data=True,
-    package_data={},
+    package_data={
+        'deropy': ['dvm/std/basic/*.bas']
+    },
     classifiers=[
         'Programming Language :: Python :: 3',
         'Operating System :: OS Independent',
     ],
     entry_points={
         'console_scripts': [
             'deropy=deropy.main:deropy'
```

### Comparing `deropy-0.2.3/tests/test_compute_storage.py` & `deropy-0.3.0/tests/test_compute_storage.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/tests/test_map_functions.py` & `deropy-0.3.0/tests/test_map_functions.py`

 * *Files identical despite different names*

### Comparing `deropy-0.2.3/tests/test_storage_functions.py` & `deropy-0.3.0/tests/test_storage_functions.py`

 * *Files identical despite different names*

