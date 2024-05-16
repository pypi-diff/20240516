# Comparing `tmp/bitcoin_qrreader-0.8.7.tar.gz` & `tmp/bitcoin_qrreader-0.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitcoin_qrreader-0.8.7.tar", max compression
+gzip compressed data, was "bitcoin_qrreader-0.8.8.tar", max compression
```

## Comparing `bitcoin_qrreader-0.8.7.tar` & `bitcoin_qrreader-0.8.8.tar`

### file list

```diff
@@ -1,44 +1,44 @@
--rw-r--r--   0        0        0    35149 2023-06-09 17:54:40.000000 bitcoin_qrreader-0.8.7/LICENSE
--rw-r--r--   0        0        0     1474 2024-02-08 11:20:06.244073 bitcoin_qrreader-0.8.7/README.md
--rw-r--r--   0        0        0        0 2023-07-20 11:25:47.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/__init__.py
--rw-r--r--   0        0        0    29516 2024-04-19 13:35:12.623277 bitcoin_qrreader-0.8.7/bitcoin_qrreader/bitcoin_qr.py
--rw-r--r--   0        0        0     3757 2024-04-19 15:03:46.357699 bitcoin_qrreader-0.8.7/bitcoin_qrreader/bitcoin_qr_gui.py
--rw-r--r--   0        0        0     4182 2024-04-19 13:35:23.375455 bitcoin_qrreader-0.8.7/bitcoin_qrreader/multipath_descriptor.py
--rw-r--r--   0        0        0     7740 2024-04-19 14:36:46.472651 bitcoin_qrreader-0.8.7/bitcoin_qrreader/qr_qui.py
--rw-r--r--   0        0        0     2854 2023-07-21 11:50:05.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/LICENSE
--rw-r--r--   0        0        0        0 2023-07-21 11:50:05.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/__init__.py
--rw-r--r--   0        0        0     4940 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/bytewords.py
--rw-r--r--   0        0        0    11219 2024-01-07 18:00:24.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/cbor_lite.py
--rw-r--r--   0        0        0      179 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/constants.py
--rw-r--r--   0        0        0      729 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/crc32.py
--rw-r--r--   0        0        0     9747 2024-04-19 13:37:39.509769 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/fountain_decoder.py
--rw-r--r--   0        0        0     4972 2024-04-19 13:37:45.293870 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/fountain_encoder.py
--rw-r--r--   0        0        0     1604 2024-04-19 13:37:50.969969 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/fountain_utils.py
--rw-r--r--   0        0        0     1568 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/random_sampler.py
--rw-r--r--   0        0        0      491 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/ur.py
--rw-r--r--   0        0        0     5091 2024-04-19 13:38:18.494450 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/ur_decoder.py
--rw-r--r--   0        0        0     2016 2024-04-19 13:38:11.454326 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/ur_encoder.py
--rw-r--r--   0        0        0     1638 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/utils.py
--rw-r--r--   0        0        0     4422 2024-04-19 13:38:01.210147 bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/xoshiro256.py
--rw-r--r--   0        0        0     1076 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/LICENSE.md
--rw-r--r--   0        0        0      318 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/README.md
--rw-r--r--   0        0        0     1157 2024-04-19 13:39:40.239899 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/__init__.py
--rw-r--r--   0        0        0     1582 2024-04-19 13:39:03.135238 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/bytes.py
--rw-r--r--   0        0        0     1119 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/cbor/COPYING
--rw-r--r--   0        0        0     1247 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/cbor/__init__.py
--rw-r--r--   0        0        0     2165 2024-01-07 18:00:24.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/cbor/data.py
--rw-r--r--   0        0        0     6630 2024-04-19 13:37:30.765618 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/cbor/decoder.py
--rw-r--r--   0        0        0     4831 2024-04-19 13:37:25.453526 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/cbor/encoder.py
--rw-r--r--   0        0        0     1315 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/__init__.py
--rw-r--r--   0        0        0     2343 2024-04-19 13:37:19.453422 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/account.py
--rw-r--r--   0        0        0     1845 2024-04-19 13:37:13.077312 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/bip39.py
--rw-r--r--   0        0        0     1954 2024-04-19 13:37:07.525216 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/coin_info.py
--rw-r--r--   0        0        0     2194 2024-04-19 13:37:02.105123 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/ec_key.py
--rw-r--r--   0        0        0     8882 2024-04-19 13:36:56.321024 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/hd_key.py
--rw-r--r--   0        0        0     3686 2024-04-19 13:36:50.728928 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/keypath.py
--rw-r--r--   0        0        0     2425 2024-04-19 13:36:44.668825 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/multi_key.py
--rw-r--r--   0        0        0     6339 2024-04-19 13:36:38.828725 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/output.py
--rw-r--r--   0        0        0     1296 2024-04-19 13:36:32.280614 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/psbt.py
--rw-r--r--   0        0        0     2291 2024-04-19 13:36:17.748367 bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/registry.py
--rw-r--r--   0        0        0      779 2024-04-19 15:04:10.166161 bitcoin_qrreader-0.8.7/pyproject.toml
--rw-r--r--   0        0        0     2434 1970-01-01 00:00:00.000000 bitcoin_qrreader-0.8.7/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-09 17:54:40.000000 bitcoin_qrreader-0.8.8/LICENSE
+-rw-r--r--   0        0        0     1474 2024-02-08 11:20:06.244073 bitcoin_qrreader-0.8.8/README.md
+-rw-r--r--   0        0        0        0 2023-07-20 11:25:47.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/__init__.py
+-rw-r--r--   0        0        0    29516 2024-04-19 13:35:12.623277 bitcoin_qrreader-0.8.8/bitcoin_qrreader/bitcoin_qr.py
+-rw-r--r--   0        0        0     3757 2024-04-19 15:03:46.357699 bitcoin_qrreader-0.8.8/bitcoin_qrreader/bitcoin_qr_gui.py
+-rw-r--r--   0        0        0     4182 2024-04-19 13:35:23.375455 bitcoin_qrreader-0.8.8/bitcoin_qrreader/multipath_descriptor.py
+-rw-r--r--   0        0        0     7740 2024-05-16 16:10:40.131165 bitcoin_qrreader-0.8.8/bitcoin_qrreader/qr_qui.py
+-rw-r--r--   0        0        0     2854 2023-07-21 11:50:05.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/LICENSE
+-rw-r--r--   0        0        0        0 2023-07-21 11:50:05.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/__init__.py
+-rw-r--r--   0        0        0     4940 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/bytewords.py
+-rw-r--r--   0        0        0    11219 2024-01-07 18:00:24.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/cbor_lite.py
+-rw-r--r--   0        0        0      179 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/constants.py
+-rw-r--r--   0        0        0      729 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/crc32.py
+-rw-r--r--   0        0        0     9747 2024-04-19 13:37:39.509769 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/fountain_decoder.py
+-rw-r--r--   0        0        0     4972 2024-04-19 13:37:45.293870 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/fountain_encoder.py
+-rw-r--r--   0        0        0     1604 2024-04-19 13:37:50.969969 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/fountain_utils.py
+-rw-r--r--   0        0        0     1568 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/random_sampler.py
+-rw-r--r--   0        0        0      491 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/ur.py
+-rw-r--r--   0        0        0     5091 2024-04-19 13:38:18.494450 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/ur_decoder.py
+-rw-r--r--   0        0        0     2016 2024-04-19 13:38:11.454326 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/ur_encoder.py
+-rw-r--r--   0        0        0     1638 2023-07-21 17:21:38.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/utils.py
+-rw-r--r--   0        0        0     4422 2024-04-19 13:38:01.210147 bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/xoshiro256.py
+-rw-r--r--   0        0        0     1076 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/LICENSE.md
+-rw-r--r--   0        0        0      318 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/README.md
+-rw-r--r--   0        0        0     1157 2024-04-19 13:39:40.239899 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/__init__.py
+-rw-r--r--   0        0        0     1582 2024-04-19 13:39:03.135238 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/bytes.py
+-rw-r--r--   0        0        0     1119 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/cbor/COPYING
+-rw-r--r--   0        0        0     1247 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/cbor/__init__.py
+-rw-r--r--   0        0        0     2165 2024-01-07 18:00:24.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/cbor/data.py
+-rw-r--r--   0        0        0     6630 2024-04-19 13:37:30.765618 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/cbor/decoder.py
+-rw-r--r--   0        0        0     4831 2024-04-19 13:37:25.453526 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/cbor/encoder.py
+-rw-r--r--   0        0        0     1315 2023-07-21 18:01:30.000000 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/__init__.py
+-rw-r--r--   0        0        0     2343 2024-04-19 13:37:19.453422 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/account.py
+-rw-r--r--   0        0        0     1845 2024-04-19 13:37:13.077312 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/bip39.py
+-rw-r--r--   0        0        0     1954 2024-04-19 13:37:07.525216 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/coin_info.py
+-rw-r--r--   0        0        0     2194 2024-04-19 13:37:02.105123 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/ec_key.py
+-rw-r--r--   0        0        0     8882 2024-04-19 13:36:56.321024 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/hd_key.py
+-rw-r--r--   0        0        0     3686 2024-04-19 13:36:50.728928 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/keypath.py
+-rw-r--r--   0        0        0     2425 2024-04-19 13:36:44.668825 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/multi_key.py
+-rw-r--r--   0        0        0     6339 2024-04-19 13:36:38.828725 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/output.py
+-rw-r--r--   0        0        0     1296 2024-04-19 13:36:32.280614 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/psbt.py
+-rw-r--r--   0        0        0     2291 2024-04-19 13:36:17.748367 bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/registry.py
+-rw-r--r--   0        0        0      787 2024-05-16 16:11:21.572207 bitcoin_qrreader-0.8.8/pyproject.toml
+-rw-r--r--   0        0        0     2436 1970-01-01 00:00:00.000000 bitcoin_qrreader-0.8.8/PKG-INFO
```

### Comparing `bitcoin_qrreader-0.8.7/LICENSE` & `bitcoin_qrreader-0.8.8/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/README.md` & `bitcoin_qrreader-0.8.8/README.md`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/bitcoin_qr.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/bitcoin_qr.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/bitcoin_qr_gui.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/bitcoin_qr_gui.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/multipath_descriptor.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/multipath_descriptor.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/qr_qui.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/qr_qui.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/LICENSE` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/LICENSE`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/bytewords.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/bytewords.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/cbor_lite.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/cbor_lite.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/crc32.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/crc32.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/fountain_decoder.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/fountain_decoder.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/fountain_encoder.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/fountain_encoder.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/fountain_utils.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/fountain_utils.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/random_sampler.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/random_sampler.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/ur_decoder.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/ur_decoder.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/ur_encoder.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/ur_encoder.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/utils.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/utils.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/ur/xoshiro256.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/ur/xoshiro256.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/LICENSE.md` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/LICENSE.md`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/__init__.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/__init__.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/bytes.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/bytes.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/cbor/COPYING` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/cbor/COPYING`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/cbor/__init__.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/cbor/__init__.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/cbor/data.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/cbor/data.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/cbor/decoder.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/cbor/decoder.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/cbor/encoder.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/cbor/encoder.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/__init__.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/__init__.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/account.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/account.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/bip39.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/bip39.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/coin_info.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/coin_info.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/ec_key.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/ec_key.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/hd_key.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/hd_key.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/keypath.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/keypath.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/multi_key.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/multi_key.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/output.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/output.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/crypto/psbt.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/crypto/psbt.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/bitcoin_qrreader/urtypes/registry.py` & `bitcoin_qrreader-0.8.8/bitcoin_qrreader/urtypes/registry.py`

 * *Files identical despite different names*

### Comparing `bitcoin_qrreader-0.8.7/pyproject.toml` & `bitcoin_qrreader-0.8.8/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -7,32 +7,32 @@
 show_error_codes = true 
 disable_error_code = "assignment"
 
 
 
 [tool.poetry]
 name = "bitcoin-qrreader"
-version = "0.8.7"
+version = "0.8.8"
 authors = ["andreasgriffin <andreasgriffin@proton.me>"]
 license = "GPL-3.0"
 readme = "README.md"
 description = "A python bitcoin qr reader"
 homepage = "https://github.com/andreasgriffin/bitcoin-qrreader"
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.12"
-pyqt6 = "^6.6.1"
+pyqt6 = "^6.7.0"
 base58 = "2.1.1"
 bdkpython ="0.31.0"
-pygame ="2.5.0"
+pygame ="2.5.2"
 numpy = "^1.21.0"
 mss ="9.0.1"
 hwi = "2.3.1"
-opencv-python = "^4.9.0.80"
-pyzbar = "^0.1.9"
+pyzbar = "0.1.9"
+opencv-python-headless = "^4.9.0.80"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^6.0"
 
 [build-system]
 requires = ["poetry-core"]
```

### Comparing `bitcoin_qrreader-0.8.7/PKG-INFO` & `bitcoin_qrreader-0.8.8/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitcoin-qrreader
-Version: 0.8.7
+Version: 0.8.8
 Summary: A python bitcoin qr reader
 Home-page: https://github.com/andreasgriffin/bitcoin-qrreader
 License: GPL-3.0
 Author: andreasgriffin
 Author-email: andreasgriffin@proton.me
 Requires-Python: >=3.8,<3.12
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -14,18 +14,18 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: base58 (==2.1.1)
 Requires-Dist: bdkpython (==0.31.0)
 Requires-Dist: hwi (==2.3.1)
 Requires-Dist: mss (==9.0.1)
 Requires-Dist: numpy (>=1.21.0,<2.0.0)
-Requires-Dist: opencv-python (>=4.9.0.80,<5.0.0.0)
-Requires-Dist: pygame (==2.5.0)
-Requires-Dist: pyqt6 (>=6.6.1,<7.0.0)
-Requires-Dist: pyzbar (>=0.1.9,<0.2.0)
+Requires-Dist: opencv-python-headless (>=4.9.0.80,<5.0.0.0)
+Requires-Dist: pygame (==2.5.2)
+Requires-Dist: pyqt6 (>=6.7.0,<7.0.0)
+Requires-Dist: pyzbar (==0.1.9)
 Description-Content-Type: text/markdown
 
 # A python bitcoin qr reader
 
 * Recognizes (and classifies)
   * Addresses  (also BIP21 with amount)
   * Transactions (also base43 electrum encoding)
```

