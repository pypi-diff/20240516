# Comparing `tmp/eth-tester-0.9.1b1.tar.gz` & `tmp/eth-tester-0.9.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eth-tester-0.9.1b1.tar", last modified: Wed Jul 26 16:27:58 2023, max compression
+gzip compressed data, was "eth-tester-0.9.1b2.tar", last modified: Fri Jan 26 20:45:27 2024, max compression
```

## Comparing `eth-tester-0.9.1b1.tar` & `eth-tester-0.9.1b2.tar`

### file list

```diff
@@ -1,65 +1,81 @@
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.462478 eth-tester-0.9.1b1/
--rw-r--r--   0 eve        (501) staff       (20)     1080 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/LICENSE
--rw-r--r--   0 eve        (501) staff       (20)      121 2022-08-25 19:50:54.000000 eth-tester-0.9.1b1/MANIFEST.in
--rw-r--r--   0 eve        (501) staff       (20)    35041 2023-07-26 16:27:58.462303 eth-tester-0.9.1b1/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)    34123 2023-04-27 21:21:30.000000 eth-tester-0.9.1b1/README.md
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.453862 eth-tester-0.9.1b1/eth_tester/
--rw-r--r--   0 eve        (501) staff       (20)      331 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/eth_tester/__init__.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.455057 eth-tester-0.9.1b1/eth_tester/backends/
--rw-r--r--   0 eve        (501) staff       (20)     1652 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/backends/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2889 2022-11-21 19:35:20.000000 eth-tester-0.9.1b1/eth_tester/backends/base.py
--rw-r--r--   0 eve        (501) staff       (20)      540 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/backends/common.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.456229 eth-tester-0.9.1b1/eth_tester/backends/mock/
--rw-r--r--   0 eve        (501) staff       (20)       53 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/eth_tester/backends/mock/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      304 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/backends/mock/common.py
--rw-r--r--   0 eve        (501) staff       (20)    13229 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/backends/mock/factory.py
--rw-r--r--   0 eve        (501) staff       (20)     9480 2022-11-21 19:35:20.000000 eth-tester-0.9.1b1/eth_tester/backends/mock/main.py
--rw-r--r--   0 eve        (501) staff       (20)     3068 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/backends/mock/serializers.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.457208 eth-tester-0.9.1b1/eth_tester/backends/pyevm/
--rw-r--r--   0 eve        (501) staff       (20)      173 2021-11-18 18:37:46.000000 eth-tester-0.9.1b1/eth_tester/backends/pyevm/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)    27687 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/backends/pyevm/main.py
--rw-r--r--   0 eve        (501) staff       (20)     8556 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/backends/pyevm/serializers.py
--rw-r--r--   0 eve        (501) staff       (20)      515 2021-11-18 18:37:46.000000 eth-tester-0.9.1b1/eth_tester/backends/pyevm/utils.py
--rw-r--r--   0 eve        (501) staff       (20)     1725 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/constants.py
--rw-r--r--   0 eve        (501) staff       (20)      413 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/eth_tester/exceptions.py
--rw-r--r--   0 eve        (501) staff       (20)    30564 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/main.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.458428 eth-tester-0.9.1b1/eth_tester/normalization/
--rw-r--r--   0 eve        (501) staff       (20)      702 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/normalization/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     3429 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/normalization/base.py
--rw-r--r--   0 eve        (501) staff       (20)      924 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/normalization/common.py
--rw-r--r--   0 eve        (501) staff       (20)     2869 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/normalization/default.py
--rw-r--r--   0 eve        (501) staff       (20)     3358 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/normalization/inbound.py
--rw-r--r--   0 eve        (501) staff       (20)     5748 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/normalization/outbound.py
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/eth_tester/rpc.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.458659 eth-tester-0.9.1b1/eth_tester/tools/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-11-10 19:15:57.000000 eth-tester-0.9.1b1/eth_tester/tools/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     2235 2022-11-21 19:35:20.000000 eth-tester-0.9.1b1/eth_tester/tools/gas_burner_contract.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.461003 eth-tester-0.9.1b1/eth_tester/utils/
--rw-r--r--   0 eve        (501) staff       (20)        0 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/eth_tester/utils/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)      152 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/eth_tester/utils/accounts.py
--rw-r--r--   0 eve        (501) staff       (20)      243 2021-03-31 18:03:15.000000 eth-tester-0.9.1b1/eth_tester/utils/address.py
--rw-r--r--   0 eve        (501) staff       (20)    65774 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/utils/backend_testing.py
--rw-r--r--   0 eve        (501) staff       (20)     9633 2022-11-21 19:35:20.000000 eth-tester-0.9.1b1/eth_tester/utils/emitter_contract.py
--rw-r--r--   0 eve        (501) staff       (20)      323 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/utils/encoding.py
--rw-r--r--   0 eve        (501) staff       (20)     5244 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/utils/filters.py
--rw-r--r--   0 eve        (501) staff       (20)     4324 2022-11-21 19:35:20.000000 eth-tester-0.9.1b1/eth_tester/utils/math_contract.py
--rw-r--r--   0 eve        (501) staff       (20)      906 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/utils/module_loading.py
--rw-r--r--   0 eve        (501) staff       (20)     5035 2022-11-21 19:35:20.000000 eth-tester-0.9.1b1/eth_tester/utils/throws_contract.py
--rw-r--r--   0 eve        (501) staff       (20)     1191 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/utils/transactions.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.462050 eth-tester-0.9.1b1/eth_tester/validation/
--rw-r--r--   0 eve        (501) staff       (20)      658 2022-08-31 17:39:35.000000 eth-tester-0.9.1b1/eth_tester/validation/__init__.py
--rw-r--r--   0 eve        (501) staff       (20)     3075 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/validation/base.py
--rw-r--r--   0 eve        (501) staff       (20)     5833 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/validation/common.py
--rw-r--r--   0 eve        (501) staff       (20)     3114 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/validation/default.py
--rw-r--r--   0 eve        (501) staff       (20)    11728 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/validation/inbound.py
--rw-r--r--   0 eve        (501) staff       (20)     9124 2023-07-20 17:32:32.000000 eth-tester-0.9.1b1/eth_tester/validation/outbound.py
-drwxr-xr-x   0 eve        (501) staff       (20)        0 2023-07-26 16:27:58.454489 eth-tester-0.9.1b1/eth_tester.egg-info/
--rw-r--r--   0 eve        (501) staff       (20)    35041 2023-07-26 16:27:58.000000 eth-tester-0.9.1b1/eth_tester.egg-info/PKG-INFO
--rw-r--r--   0 eve        (501) staff       (20)     1616 2023-07-26 16:27:58.000000 eth-tester-0.9.1b1/eth_tester.egg-info/SOURCES.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2023-07-26 16:27:58.000000 eth-tester-0.9.1b1/eth_tester.egg-info/dependency_links.txt
--rw-r--r--   0 eve        (501) staff       (20)        1 2023-07-26 16:27:58.000000 eth-tester-0.9.1b1/eth_tester.egg-info/not-zip-safe
--rw-r--r--   0 eve        (501) staff       (20)      988 2023-07-26 16:27:58.000000 eth-tester-0.9.1b1/eth_tester.egg-info/requires.txt
--rw-r--r--   0 eve        (501) staff       (20)       11 2023-07-26 16:27:58.000000 eth-tester-0.9.1b1/eth_tester.egg-info/top_level.txt
--rw-r--r--   0 eve        (501) staff       (20)     1055 2022-11-21 19:35:20.000000 eth-tester-0.9.1b1/pyproject.toml
--rw-r--r--   0 eve        (501) staff       (20)       38 2023-07-26 16:27:58.462519 eth-tester-0.9.1b1/setup.cfg
--rw-r--r--   0 eve        (501) staff       (20)     2529 2023-07-26 16:27:18.000000 eth-tester-0.9.1b1/setup.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:27.021786 eth-tester-0.9.1b2/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1080 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/LICENSE
+-rw-r--r--   0 fselmo     (501) staff       (20)      121 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/MANIFEST.in
+-rw-r--r--   0 fselmo     (501) staff       (20)    35399 2024-01-26 20:45:27.021147 eth-tester-0.9.1b2/PKG-INFO
+-rw-r--r--   0 fselmo     (501) staff       (20)    34501 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/README.md
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:26.981710 eth-tester-0.9.1b2/eth_tester/
+-rw-r--r--   0 fselmo     (501) staff       (20)      331 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/__init__.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:26.987085 eth-tester-0.9.1b2/eth_tester/backends/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1652 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/backends/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2889 2024-01-25 23:47:46.000000 eth-tester-0.9.1b2/eth_tester/backends/base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      540 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/backends/common.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:26.990902 eth-tester-0.9.1b2/eth_tester/backends/mock/
+-rw-r--r--   0 fselmo     (501) staff       (20)       53 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/backends/mock/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      304 2024-01-25 23:47:46.000000 eth-tester-0.9.1b2/eth_tester/backends/mock/common.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    13229 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/backends/mock/factory.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9741 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/backends/mock/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3068 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/backends/mock/serializers.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:26.993858 eth-tester-0.9.1b2/eth_tester/backends/pyevm/
+-rw-r--r--   0 fselmo     (501) staff       (20)      173 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/backends/pyevm/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    28758 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/backends/pyevm/main.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     8556 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/backends/pyevm/serializers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      515 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/backends/pyevm/utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1725 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/constants.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      413 2024-01-25 23:47:46.000000 eth-tester-0.9.1b2/eth_tester/exceptions.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    30855 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/main.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:26.997763 eth-tester-0.9.1b2/eth_tester/normalization/
+-rw-r--r--   0 fselmo     (501) staff       (20)      702 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/normalization/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3429 2024-01-25 23:47:46.000000 eth-tester-0.9.1b2/eth_tester/normalization/base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      924 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/normalization/common.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2869 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/normalization/default.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3322 2024-01-26 20:32:35.000000 eth-tester-0.9.1b2/eth_tester/normalization/inbound.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5748 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/normalization/outbound.py
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2024-01-25 23:47:46.000000 eth-tester-0.9.1b2/eth_tester/rpc.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:26.998593 eth-tester-0.9.1b2/eth_tester/tools/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2024-01-25 23:47:46.000000 eth-tester-0.9.1b2/eth_tester/tools/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     2235 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/tools/gas_burner_contract.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:27.006208 eth-tester-0.9.1b2/eth_tester/utils/
+-rw-r--r--   0 fselmo     (501) staff       (20)        0 2024-01-25 23:47:46.000000 eth-tester-0.9.1b2/eth_tester/utils/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      152 2024-01-25 23:47:46.000000 eth-tester-0.9.1b2/eth_tester/utils/accounts.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      243 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/utils/address.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    68674 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/utils/backend_testing.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9633 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/utils/emitter_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      323 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/utils/encoding.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5244 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/utils/filters.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     4324 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/utils/math_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      906 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/utils/module_loading.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5035 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/utils/throws_contract.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1191 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/utils/transactions.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:27.010322 eth-tester-0.9.1b2/eth_tester/validation/
+-rw-r--r--   0 fselmo     (501) staff       (20)      658 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/validation/__init__.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3075 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/validation/base.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     5833 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/validation/common.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     3114 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/validation/default.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    11728 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/validation/inbound.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     9124 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/eth_tester/validation/outbound.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:26.985040 eth-tester-0.9.1b2/eth_tester.egg-info/
+-rw-r--r--   0 fselmo     (501) staff       (20)    35399 2024-01-26 20:45:26.000000 eth-tester-0.9.1b2/eth_tester.egg-info/PKG-INFO
+-rw-r--r--   0 fselmo     (501) staff       (20)     2018 2024-01-26 20:45:26.000000 eth-tester-0.9.1b2/eth_tester.egg-info/SOURCES.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)        1 2024-01-26 20:45:26.000000 eth-tester-0.9.1b2/eth_tester.egg-info/dependency_links.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)        1 2022-11-21 22:09:50.000000 eth-tester-0.9.1b2/eth_tester.egg-info/not-zip-safe
+-rw-r--r--   0 fselmo     (501) staff       (20)      988 2024-01-26 20:45:26.000000 eth-tester-0.9.1b2/eth_tester.egg-info/requires.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)       11 2024-01-26 20:45:26.000000 eth-tester-0.9.1b2/eth_tester.egg-info/top_level.txt
+-rw-r--r--   0 fselmo     (501) staff       (20)     1055 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/pyproject.toml
+-rw-r--r--   0 fselmo     (501) staff       (20)       38 2024-01-26 20:45:27.021969 eth-tester-0.9.1b2/setup.cfg
+-rw-r--r--   0 fselmo     (501) staff       (20)     2529 2024-01-26 20:45:04.000000 eth-tester-0.9.1b2/setup.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:27.010927 eth-tester-0.9.1b2/tests/
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:27.011577 eth-tester-0.9.1b2/tests/backends/
+-rw-r--r--   0 fselmo     (501) staff       (20)    15879 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/tests/backends/test_pyevm.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:27.013630 eth-tester-0.9.1b2/tests/core/
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:27.015944 eth-tester-0.9.1b2/tests/core/filter-utils/
+-rw-r--r--   0 fselmo     (501) staff       (20)    17717 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/tests/core/filter-utils/test_filter_helpers.py
+-rw-r--r--   0 fselmo     (501) staff       (20)     1064 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/tests/core/filter-utils/test_filter_object.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:27.017060 eth-tester-0.9.1b2/tests/core/normalization/
+-rw-r--r--   0 fselmo     (501) staff       (20)     1067 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/tests/core/normalization/test_default_outbound_normalization.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      512 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/tests/core/test_account_utils.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      741 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/tests/core/test_mock_backend.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      729 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/tests/core/test_transaction_utils.py
+drwxr-xr-x   0 fselmo     (501) staff       (20)        0 2024-01-26 20:45:27.019541 eth-tester-0.9.1b2/tests/core/validation/
+-rw-r--r--   0 fselmo     (501) staff       (20)    23080 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/tests/core/validation/test_inbound_validation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)    17364 2024-01-26 20:32:23.000000 eth-tester-0.9.1b2/tests/core/validation/test_outbound_validation.py
+-rw-r--r--   0 fselmo     (501) staff       (20)      930 2024-01-25 23:47:47.000000 eth-tester-0.9.1b2/tests/utils.py
```

### Comparing `eth-tester-0.9.1b1/LICENSE` & `eth-tester-0.9.1b2/LICENSE`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/PKG-INFO` & `eth-tester-0.9.1b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: eth-tester
-Version: 0.9.1b1
+Version: 0.9.1b2
 Summary: Tools for testing Ethereum applications.
 Home-page: https://github.com/ethereum/eth-tester
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -619,14 +618,22 @@
 <a id="api-estimate_gas"></a>
 
 #### `EthereumTester.estimate_gas(transaction)`
 
 Executes the provided `transaction` object, measuring and returning the gas
 consumption.
 
+<a id="api-fee_history"></a>
+
+#### `EthereumTester.get_fee_history(block_count=1, newest_block='latest', reward_percentiles=[])`
+
+Return the historical gas information for the number of blocks specified as the `block_count` starting from `newest_block`.
+Note that specifying `reward_percentiles` has no effect on the response and so `reward` will always return an empty list.
+
+
 
 ### Logs and Filters
 
 <a id="api-create_block_filter"></a>
 
 #### `EthereumTester.create_block_filter() -> integer`
 
@@ -1033,9 +1040,7 @@
 
 
 # Use with Web3.py
 
 See the [web3.py documentation](http://web3py.readthedocs.io/en/latest/) for
 information on the `EthereumTester` provider which integrates with this
 library.
-
-
```

### Comparing `eth-tester-0.9.1b1/README.md` & `eth-tester-0.9.1b2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -590,14 +590,22 @@
 <a id="api-estimate_gas"></a>
 
 #### `EthereumTester.estimate_gas(transaction)`
 
 Executes the provided `transaction` object, measuring and returning the gas
 consumption.
 
+<a id="api-fee_history"></a>
+
+#### `EthereumTester.get_fee_history(block_count=1, newest_block='latest', reward_percentiles=[])`
+
+Return the historical gas information for the number of blocks specified as the `block_count` starting from `newest_block`.
+Note that specifying `reward_percentiles` has no effect on the response and so `reward` will always return an empty list.
+
+
 
 ### Logs and Filters
 
 <a id="api-create_block_filter"></a>
 
 #### `EthereumTester.create_block_filter() -> integer`
```

### Comparing `eth-tester-0.9.1b1/eth_tester/backends/__init__.py` & `eth-tester-0.9.1b2/eth_tester/backends/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/backends/base.py` & `eth-tester-0.9.1b2/eth_tester/backends/base.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/backends/common.py` & `eth-tester-0.9.1b2/eth_tester/backends/common.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/backends/mock/factory.py` & `eth-tester-0.9.1b2/eth_tester/backends/mock/factory.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/backends/mock/main.py` & `eth-tester-0.9.1b2/eth_tester/backends/mock/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -318,7 +318,17 @@
         return self.send_transaction(transaction)
 
     def estimate_gas(self, transaction):
         raise NotImplementedError("Must be implemented by subclasses")
 
     def call(self, transaction, block_number="latest"):
         raise NotImplementedError("Must be implemented by subclasses")
+
+    def get_fee_history(
+        self, block_count=1, newest_block="latest", reward_percentiles=[]
+    ):
+        return {
+            "oldest_block": 1,
+            "base_fee_per_gas": [],
+            "gas_used_ratio": [],
+            "reward": [],
+        }
```

### Comparing `eth-tester-0.9.1b1/eth_tester/backends/mock/serializers.py` & `eth-tester-0.9.1b2/eth_tester/backends/mock/serializers.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/backends/pyevm/main.py` & `eth-tester-0.9.1b2/eth_tester/backends/pyevm/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -552,14 +552,43 @@
             block,
             block_receipts,
             transaction,
             transaction_index,
             is_pending,
         )
 
+    def get_fee_history(
+        self, block_count=1, newest_block="latest", reward_percentiles: List[int] = []
+    ):
+        if isinstance(block_count, int) and not 1 <= block_count <= 1024:
+            raise ValidationError("block_count must be between 1 and 1024")
+
+        if newest_block == "pending":
+            newest_block = "latest"
+
+        block = self.get_block_by_number(newest_block)
+        block_header = self.chain.get_canonical_block_header_by_number(block["number"])
+
+        ancestors = self.chain.get_ancestors(block_count, header=block_header)
+
+        base_fee_per_gas = []
+        gas_used_ratio = []
+        reward = []  # always return empty reward array for now
+
+        for ancestor in ancestors:
+            base_fee_per_gas.append(ancestor.header.base_fee_per_gas)
+            gas_used_ratio.append(ancestor.header.gas_used / ancestor.header.gas_limit)
+
+        return {
+            "oldest_block": 1,
+            "base_fee_per_gas": base_fee_per_gas,
+            "gas_used_ratio": gas_used_ratio,
+            "reward": reward,
+        }
+
     #
     # Account state
     #
     def get_nonce(self, account, block_number="latest"):
         vm = _get_vm_for_block_number(self.chain, block_number)
         return vm.state.get_nonce(account)
```

### Comparing `eth-tester-0.9.1b1/eth_tester/backends/pyevm/serializers.py` & `eth-tester-0.9.1b2/eth_tester/backends/pyevm/serializers.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/backends/pyevm/utils.py` & `eth-tester-0.9.1b2/eth_tester/backends/pyevm/utils.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/constants.py` & `eth-tester-0.9.1b2/eth_tester/constants.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/main.py` & `eth-tester-0.9.1b2/eth_tester/main.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 from __future__ import unicode_literals
 
 import collections
 import itertools
 import operator
 import time
 import functools
+from typing import List
 
 from eth_typing import (
     HexAddress,
     HexStr,
 )
 from eth_utils import (
     is_integer,
@@ -359,14 +360,22 @@
             transaction_hash,
         )
         raw_receipt = self.backend.get_transaction_receipt(raw_transaction_hash)
         self.validator.validate_outbound_receipt(raw_receipt)
         receipt = self.normalizer.normalize_outbound_receipt(raw_receipt)
         return receipt
 
+    def get_fee_history(
+        self, block_count=1, newest_block="latest", reward_percentiles: List[int] = []
+    ):
+        fee_history = self.backend.get_fee_history(
+            block_count, newest_block, reward_percentiles
+        )
+        return fee_history
+
     #
     # Mining
     #
     def enable_auto_mine_transactions(self):
         self.auto_mine_transactions = True
         sent_transaction_hashes = self._pop_pending_transactions_to_pending_block()
         self.mine_block()
```

### Comparing `eth-tester-0.9.1b1/eth_tester/normalization/__init__.py` & `eth-tester-0.9.1b2/eth_tester/normalization/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/normalization/base.py` & `eth-tester-0.9.1b2/eth_tester/normalization/base.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/normalization/common.py` & `eth-tester-0.9.1b2/eth_tester/normalization/common.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/normalization/default.py` & `eth-tester-0.9.1b2/eth_tester/normalization/default.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/normalization/inbound.py` & `eth-tester-0.9.1b2/eth_tester/normalization/inbound.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 from __future__ import absolute_import
 
 from eth_utils import (
-    remove_0x_prefix,
     to_bytes,
 )
 from eth_utils.curried import (
     apply_one_of_formatters,
     decode_hex,
     is_address,
     is_list_like,
@@ -89,15 +88,15 @@
 
 def _normalize_inbound_access_list(access_list):
     return tuple(
         [
             tuple(
                 [
                     to_bytes(hexstr=entry["address"]),
-                    tuple([int(remove_0x_prefix(k)) for k in entry["storage_keys"]]),
+                    tuple([int(k, 16) for k in entry["storage_keys"]]),
                 ]
             )
             for entry in access_list
         ]
     )
```

### Comparing `eth-tester-0.9.1b1/eth_tester/normalization/outbound.py` & `eth-tester-0.9.1b2/eth_tester/normalization/outbound.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/tools/gas_burner_contract.py` & `eth-tester-0.9.1b2/eth_tester/tools/gas_burner_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/utils/backend_testing.py` & `eth-tester-0.9.1b2/eth_tester/utils/backend_testing.py`

 * *Files 2% similar despite different names*

```diff
@@ -238,14 +238,116 @@
         for account in eth_tester.get_accounts():
             nonce = eth_tester.get_nonce(account)
         assert is_integer(nonce)
         assert nonce >= UINT256_MIN
         assert nonce <= UINT256_MAX
 
     #
+    # Fee History
+    #
+    @pytest.mark.parametrize(
+        "block_count,newest_block,reward_percentiles,expected",
+        [
+            [
+                3,
+                "latest",
+                [],
+                {
+                    "base_fee_per_gas": [300657803, 343608917, 392695905],
+                    "gas_used_ratio": [0.0, 0.0, 0.0],
+                    "reward": [],
+                },
+            ],
+            [
+                1,
+                "safe",
+                [],
+                {
+                    "base_fee_per_gas": [300657803],
+                    "gas_used_ratio": [0.0],
+                    "reward": [],
+                },
+            ],
+            [
+                1,
+                "finalized",
+                [],
+                {
+                    "base_fee_per_gas": [300657803],
+                    "gas_used_ratio": [0.0],
+                    "reward": [],
+                },
+            ],
+            [
+                1,
+                "earliest",
+                [],
+                {
+                    "base_fee_per_gas": [],
+                    "gas_used_ratio": [],
+                    "reward": [],
+                },
+            ],
+            [
+                1,
+                "pending",
+                [],
+                {
+                    "base_fee_per_gas": [300657803],
+                    "gas_used_ratio": [0.0],
+                    "reward": [],
+                },
+            ],
+        ],
+    )
+    def test_get_fee_history(
+        self, eth_tester, block_count, newest_block, reward_percentiles, expected
+    ):
+        self.skip_if_no_evm_execution()
+
+        eth_tester.mine_blocks(10)
+        fee_history = eth_tester.get_fee_history(
+            block_count, newest_block, reward_percentiles
+        )
+
+        assert fee_history["oldest_block"] == 1
+        assert fee_history["base_fee_per_gas"] == expected["base_fee_per_gas"]
+        assert fee_history["gas_used_ratio"] == expected["gas_used_ratio"]
+        assert fee_history["reward"] == expected["reward"]
+
+    @pytest.mark.parametrize(
+        "block_count,newest_block,reward_percentiles,error,message",
+        [
+            [
+                1,
+                None,
+                None,
+                BlockNotFound,
+                "No block found for block number: None",
+            ],
+            [
+                0,
+                None,
+                None,
+                ValidationError,
+                "block_count must be between 1 and 1024",
+            ],
+        ],
+    )
+    def test_get_fee_history_fails(
+        self, eth_tester, block_count, newest_block, reward_percentiles, error, message
+    ):
+        self.skip_if_no_evm_execution()
+
+        eth_tester.mine_blocks(10)
+
+        with pytest.raises(error, match=message):
+            eth_tester.get_fee_history(block_count, newest_block, reward_percentiles)
+
+    #
     # Mining
     #
     def test_mine_block_single(self, eth_tester):
         eth_tester.mine_blocks()
         before_block_number = eth_tester.get_block_by_number("latest")["number"]
         eth_tester.mine_blocks()
         after_block_number = eth_tester.get_block_by_number("latest")["number"]
```

### Comparing `eth-tester-0.9.1b1/eth_tester/utils/emitter_contract.py` & `eth-tester-0.9.1b2/eth_tester/utils/emitter_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/utils/filters.py` & `eth-tester-0.9.1b2/eth_tester/utils/filters.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/utils/math_contract.py` & `eth-tester-0.9.1b2/eth_tester/utils/math_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/utils/module_loading.py` & `eth-tester-0.9.1b2/eth_tester/utils/module_loading.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/utils/throws_contract.py` & `eth-tester-0.9.1b2/eth_tester/utils/throws_contract.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/utils/transactions.py` & `eth-tester-0.9.1b2/eth_tester/utils/transactions.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/validation/__init__.py` & `eth-tester-0.9.1b2/eth_tester/validation/__init__.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/validation/base.py` & `eth-tester-0.9.1b2/eth_tester/validation/base.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/validation/common.py` & `eth-tester-0.9.1b2/eth_tester/validation/common.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/validation/default.py` & `eth-tester-0.9.1b2/eth_tester/validation/default.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/validation/inbound.py` & `eth-tester-0.9.1b2/eth_tester/validation/inbound.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester/validation/outbound.py` & `eth-tester-0.9.1b2/eth_tester/validation/outbound.py`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/eth_tester.egg-info/PKG-INFO` & `eth-tester-0.9.1b2/eth_tester.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 Metadata-Version: 2.1
 Name: eth-tester
-Version: 0.9.1b1
+Version: 0.9.1b2
 Summary: Tools for testing Ethereum applications.
 Home-page: https://github.com/ethereum/eth-tester
 Author: Piper Merriam
 Author-email: pipermerriam@gmail.com
 License: MIT
 Keywords: ethereum
-Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -619,14 +618,22 @@
 <a id="api-estimate_gas"></a>
 
 #### `EthereumTester.estimate_gas(transaction)`
 
 Executes the provided `transaction` object, measuring and returning the gas
 consumption.
 
+<a id="api-fee_history"></a>
+
+#### `EthereumTester.get_fee_history(block_count=1, newest_block='latest', reward_percentiles=[])`
+
+Return the historical gas information for the number of blocks specified as the `block_count` starting from `newest_block`.
+Note that specifying `reward_percentiles` has no effect on the response and so `reward` will always return an empty list.
+
+
 
 ### Logs and Filters
 
 <a id="api-create_block_filter"></a>
 
 #### `EthereumTester.create_block_filter() -> integer`
 
@@ -1033,9 +1040,7 @@
 
 
 # Use with Web3.py
 
 See the [web3.py documentation](http://web3py.readthedocs.io/en/latest/) for
 information on the `EthereumTester` provider which integrates with this
 library.
-
-
```

### Comparing `eth-tester-0.9.1b1/eth_tester.egg-info/SOURCES.txt` & `eth-tester-0.9.1b2/eth_tester.egg-info/SOURCES.txt`

 * *Files 24% similar despite different names*

```diff
@@ -46,8 +46,18 @@
 eth_tester/utils/throws_contract.py
 eth_tester/utils/transactions.py
 eth_tester/validation/__init__.py
 eth_tester/validation/base.py
 eth_tester/validation/common.py
 eth_tester/validation/default.py
 eth_tester/validation/inbound.py
-eth_tester/validation/outbound.py
+eth_tester/validation/outbound.py
+tests/utils.py
+tests/backends/test_pyevm.py
+tests/core/test_account_utils.py
+tests/core/test_mock_backend.py
+tests/core/test_transaction_utils.py
+tests/core/filter-utils/test_filter_helpers.py
+tests/core/filter-utils/test_filter_object.py
+tests/core/normalization/test_default_outbound_normalization.py
+tests/core/validation/test_inbound_validation.py
+tests/core/validation/test_outbound_validation.py
```

### Comparing `eth-tester-0.9.1b1/eth_tester.egg-info/requires.txt` & `eth-tester-0.9.1b2/eth_tester.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/pyproject.toml` & `eth-tester-0.9.1b2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `eth-tester-0.9.1b1/setup.py` & `eth-tester-0.9.1b2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 with open("./README.md") as readme:
     long_description = readme.read()
 
 setup(
     name="eth-tester",
     # *IMPORTANT*: Don't manually change the version here. Use the 'bumpversion' utility.
-    version="0.9.1-beta.1",
+    version="0.9.1-beta.2",
     description="""Tools for testing Ethereum applications.""",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Piper Merriam",
     author_email="pipermerriam@gmail.com",
     url="https://github.com/ethereum/eth-tester",
     include_package_data=True,
```

