# Comparing `tmp/chainbench-0.7.0.tar.gz` & `tmp/chainbench-0.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainbench-0.7.0.tar", max compression
+gzip compressed data, was "chainbench-0.7.1.tar", max compression
```

## Comparing `chainbench-0.7.0.tar` & `chainbench-0.7.1.tar`

### file list

```diff
@@ -1,59 +1,59 @@
--rw-r--r--   0        0        0    11357 2024-05-14 15:20:25.775396 chainbench-0.7.0/LICENSE
--rw-r--r--   0        0        0    12382 2024-05-14 15:20:25.775396 chainbench-0.7.0/README.md
--rw-r--r--   0        0        0        0 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/__init__.py
--rw-r--r--   0        0        0       39 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/__main__.py
--rw-r--r--   0        0        0    15901 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/main.py
--rw-r--r--   0        0        0        0 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/__init__.py
--rw-r--r--   0        0        0     1277 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/arbitrum/general.py
--rw-r--r--   0        0        0     1110 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/avalanche/archive.py
--rw-r--r--   0        0        0     1175 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/avalanche/general.py
--rw-r--r--   0        0        0     1010 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/base/archive.py
--rw-r--r--   0        0        0     1240 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/base/general.py
--rw-r--r--   0        0        0      846 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/bsc/general.py
--rw-r--r--   0        0        0     1212 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/ethereum/consensus.py
--rw-r--r--   0        0        0      935 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/ethereum/general.py
--rw-r--r--   0        0        0      425 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/evm/all.py
--rw-r--r--   0        0        0      903 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/evm/debug_trace.py
--rw-r--r--   0        0        0      281 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/evm/get_logs.py
--rw-r--r--   0        0        0      807 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/evm/heavy.py
--rw-r--r--   0        0        0      532 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/evm/light.py
--rw-r--r--   0        0        0      807 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/fantom/archive.py
--rw-r--r--   0        0        0      987 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/fantom/general.py
--rw-r--r--   0        0        0     2012 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/oasis/general.py
--rw-r--r--   0        0        0      949 2024-05-14 15:20:25.775396 chainbench-0.7.0/chainbench/profile/optimism/archive.py
--rw-r--r--   0        0        0     1205 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/profile/optimism/general.py
--rw-r--r--   0        0        0      998 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/profile/polygon/general.py
--rw-r--r--   0        0        0      899 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/profile/ronin/general.py
--rw-r--r--   0        0        0      452 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/profile/solana/all.py
--rw-r--r--   0        0        0     1204 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/profile/solana/general.py
--rw-r--r--   0        0        0     2223 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/profile/starknet/wallet.py
--rw-r--r--   0        0        0      599 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/test_data/__init__.py
--rw-r--r--   0        0        0     6484 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/test_data/blockchain.py
--rw-r--r--   0        0        0     5934 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/test_data/ethereum.py
--rw-r--r--   0        0        0    19240 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/test_data/evm.py
--rw-r--r--   0        0        0     6037 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/test_data/solana.py
--rw-r--r--   0        0        0     2284 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/test_data/starknet.py
--rw-r--r--   0        0        0       24 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/tools/__init__.py
--rw-r--r--   0        0        0       18 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/tools/discovery/__init__.py
--rw-r--r--   0        0        0      977 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/tools/discovery/clients.json
--rw-r--r--   0        0        0    55080 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/tools/discovery/methods.json
--rw-r--r--   0        0        0     5499 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/tools/discovery/rpc.py
--rw-r--r--   0        0        0      497 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/__init__.py
--rw-r--r--   0        0        0     1459 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/common.py
--rw-r--r--   0        0        0    10599 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/http.py
--rw-r--r--   0        0        0      216 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/protocol/__init__.py
--rw-r--r--   0        0        0    11937 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/protocol/ethereum.py
--rw-r--r--   0        0        0    21316 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/protocol/evm.py
--rw-r--r--   0        0        0    22218 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/protocol/solana.py
--rw-r--r--   0        0        0     3694 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/protocol/starknet.py
--rw-r--r--   0        0        0      573 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/user/tag.py
--rw-r--r--   0        0        0        0 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/__init__.py
--rw-r--r--   0        0        0     6480 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/cli.py
--rw-r--r--   0        0        0    13147 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/event.py
--rw-r--r--   0        0        0     6347 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/http.py
--rw-r--r--   0        0        0     2419 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/monitor.py
--rw-r--r--   0        0        0     3453 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/notify.py
--rw-r--r--   0        0        0      870 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/rng.py
--rw-r--r--   0        0        0      455 2024-05-14 15:20:25.779396 chainbench-0.7.0/chainbench/util/timer.py
--rw-r--r--   0        0        0      991 2024-05-14 15:20:25.783396 chainbench-0.7.0/pyproject.toml
--rw-r--r--   0        0        0    13054 1970-01-01 00:00:00.000000 chainbench-0.7.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-05-16 06:12:13.871475 chainbench-0.7.1/LICENSE
+-rw-r--r--   0        0        0    12382 2024-05-16 06:12:13.871475 chainbench-0.7.1/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/__init__.py
+-rw-r--r--   0        0        0       39 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/__main__.py
+-rw-r--r--   0        0        0    15901 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/main.py
+-rw-r--r--   0        0        0        0 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/__init__.py
+-rw-r--r--   0        0        0     1277 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/arbitrum/general.py
+-rw-r--r--   0        0        0     1110 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/avalanche/archive.py
+-rw-r--r--   0        0        0     1175 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/avalanche/general.py
+-rw-r--r--   0        0        0     1010 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/base/archive.py
+-rw-r--r--   0        0        0     1240 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/base/general.py
+-rw-r--r--   0        0        0      846 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/bsc/general.py
+-rw-r--r--   0        0        0     1212 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/ethereum/consensus.py
+-rw-r--r--   0        0        0      935 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/ethereum/general.py
+-rw-r--r--   0        0        0      425 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/evm/all.py
+-rw-r--r--   0        0        0      856 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/evm/debug_trace.py
+-rw-r--r--   0        0        0      281 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/evm/get_logs.py
+-rw-r--r--   0        0        0      807 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/evm/heavy.py
+-rw-r--r--   0        0        0      532 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/evm/light.py
+-rw-r--r--   0        0        0      807 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/fantom/archive.py
+-rw-r--r--   0        0        0      987 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/fantom/general.py
+-rw-r--r--   0        0        0     2012 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/oasis/general.py
+-rw-r--r--   0        0        0      949 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/optimism/archive.py
+-rw-r--r--   0        0        0     1205 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/optimism/general.py
+-rw-r--r--   0        0        0      998 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/polygon/general.py
+-rw-r--r--   0        0        0      899 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/ronin/general.py
+-rw-r--r--   0        0        0      452 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/solana/all.py
+-rw-r--r--   0        0        0     1204 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/solana/general.py
+-rw-r--r--   0        0        0     2223 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/profile/starknet/wallet.py
+-rw-r--r--   0        0        0      599 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/test_data/__init__.py
+-rw-r--r--   0        0        0     6484 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/test_data/blockchain.py
+-rw-r--r--   0        0        0     5934 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/test_data/ethereum.py
+-rw-r--r--   0        0        0    19240 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/test_data/evm.py
+-rw-r--r--   0        0        0     6037 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/test_data/solana.py
+-rw-r--r--   0        0        0     2284 2024-05-16 06:12:13.871475 chainbench-0.7.1/chainbench/test_data/starknet.py
+-rw-r--r--   0        0        0       24 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/tools/__init__.py
+-rw-r--r--   0        0        0       18 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/tools/discovery/__init__.py
+-rw-r--r--   0        0        0      977 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/tools/discovery/clients.json
+-rw-r--r--   0        0        0    55080 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/tools/discovery/methods.json
+-rw-r--r--   0        0        0     5499 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/tools/discovery/rpc.py
+-rw-r--r--   0        0        0      497 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/user/__init__.py
+-rw-r--r--   0        0        0     1459 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/user/common.py
+-rw-r--r--   0        0        0    10599 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/user/http.py
+-rw-r--r--   0        0        0      216 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/user/protocol/__init__.py
+-rw-r--r--   0        0        0    11937 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/user/protocol/ethereum.py
+-rw-r--r--   0        0        0    21316 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/user/protocol/evm.py
+-rw-r--r--   0        0        0    22218 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/user/protocol/solana.py
+-rw-r--r--   0        0        0     3694 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/user/protocol/starknet.py
+-rw-r--r--   0        0        0      573 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/user/tag.py
+-rw-r--r--   0        0        0        0 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/util/__init__.py
+-rw-r--r--   0        0        0     6480 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/util/cli.py
+-rw-r--r--   0        0        0    13147 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/util/event.py
+-rw-r--r--   0        0        0     6347 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/util/http.py
+-rw-r--r--   0        0        0     2419 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/util/monitor.py
+-rw-r--r--   0        0        0     3453 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/util/notify.py
+-rw-r--r--   0        0        0      870 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/util/rng.py
+-rw-r--r--   0        0        0      455 2024-05-16 06:12:13.875475 chainbench-0.7.1/chainbench/util/timer.py
+-rw-r--r--   0        0        0      991 2024-05-16 06:12:13.875475 chainbench-0.7.1/pyproject.toml
+-rw-r--r--   0        0        0    13054 1970-01-01 00:00:00.000000 chainbench-0.7.1/PKG-INFO
```

### Comparing `chainbench-0.7.0/LICENSE` & `chainbench-0.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/README.md` & `chainbench-0.7.1/README.md`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/main.py` & `chainbench-0.7.1/chainbench/main.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/arbitrum/general.py` & `chainbench-0.7.1/chainbench/profile/arbitrum/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/avalanche/archive.py` & `chainbench-0.7.1/chainbench/profile/avalanche/archive.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/avalanche/general.py` & `chainbench-0.7.1/chainbench/profile/avalanche/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/base/archive.py` & `chainbench-0.7.1/chainbench/profile/base/archive.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/base/general.py` & `chainbench-0.7.1/chainbench/profile/base/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/bsc/general.py` & `chainbench-0.7.1/chainbench/profile/bsc/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/ethereum/consensus.py` & `chainbench-0.7.1/chainbench/profile/ethereum/consensus.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/ethereum/general.py` & `chainbench-0.7.1/chainbench/profile/ethereum/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/evm/heavy.py` & `chainbench-0.7.1/chainbench/profile/evm/heavy.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/evm/light.py` & `chainbench-0.7.1/chainbench/profile/evm/light.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/fantom/archive.py` & `chainbench-0.7.1/chainbench/profile/fantom/archive.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/fantom/general.py` & `chainbench-0.7.1/chainbench/profile/fantom/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/oasis/general.py` & `chainbench-0.7.1/chainbench/profile/oasis/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/optimism/archive.py` & `chainbench-0.7.1/chainbench/profile/optimism/archive.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/optimism/general.py` & `chainbench-0.7.1/chainbench/profile/optimism/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/polygon/general.py` & `chainbench-0.7.1/chainbench/profile/polygon/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/ronin/general.py` & `chainbench-0.7.1/chainbench/profile/ronin/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/solana/general.py` & `chainbench-0.7.1/chainbench/profile/solana/general.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/profile/starknet/wallet.py` & `chainbench-0.7.1/chainbench/profile/starknet/wallet.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/test_data/__init__.py` & `chainbench-0.7.1/chainbench/test_data/__init__.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/test_data/blockchain.py` & `chainbench-0.7.1/chainbench/test_data/blockchain.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/test_data/ethereum.py` & `chainbench-0.7.1/chainbench/test_data/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/test_data/evm.py` & `chainbench-0.7.1/chainbench/test_data/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/test_data/solana.py` & `chainbench-0.7.1/chainbench/test_data/solana.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/test_data/starknet.py` & `chainbench-0.7.1/chainbench/test_data/starknet.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/tools/discovery/clients.json` & `chainbench-0.7.1/chainbench/tools/discovery/clients.json`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/tools/discovery/methods.json` & `chainbench-0.7.1/chainbench/tools/discovery/methods.json`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/tools/discovery/rpc.py` & `chainbench-0.7.1/chainbench/tools/discovery/rpc.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/user/common.py` & `chainbench-0.7.1/chainbench/user/common.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/user/http.py` & `chainbench-0.7.1/chainbench/user/http.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/user/protocol/ethereum.py` & `chainbench-0.7.1/chainbench/user/protocol/ethereum.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/user/protocol/evm.py` & `chainbench-0.7.1/chainbench/user/protocol/evm.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/user/protocol/solana.py` & `chainbench-0.7.1/chainbench/user/protocol/solana.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/user/protocol/starknet.py` & `chainbench-0.7.1/chainbench/user/protocol/starknet.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/user/tag.py` & `chainbench-0.7.1/chainbench/user/tag.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/util/cli.py` & `chainbench-0.7.1/chainbench/util/cli.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/util/event.py` & `chainbench-0.7.1/chainbench/util/event.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/util/http.py` & `chainbench-0.7.1/chainbench/util/http.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/util/monitor.py` & `chainbench-0.7.1/chainbench/util/monitor.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/util/notify.py` & `chainbench-0.7.1/chainbench/util/notify.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/chainbench/util/rng.py` & `chainbench-0.7.1/chainbench/util/rng.py`

 * *Files identical despite different names*

### Comparing `chainbench-0.7.0/pyproject.toml` & `chainbench-0.7.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "chainbench"
-version = "0.7.0"
+version = "0.7.1"
 description = ""
 authors = [
     "Egor Molodik <egor.molodik@chainstack.com>",
     "Erwin Wee <erwin.wee@chainstack.com>"
 ]
 maintainers = ["Erwin Wee <erwin.wee@chainstack.com>"]
 readme = "README.md"
```

### Comparing `chainbench-0.7.0/PKG-INFO` & `chainbench-0.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: chainbench
-Version: 0.7.0
+Version: 0.7.1
 Summary: 
 Author: Egor Molodik
 Author-email: egor.molodik@chainstack.com
 Maintainer: Erwin Wee
 Maintainer-email: erwin.wee@chainstack.com
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
```

