# Comparing `tmp/calling_rate-0.3.1.tar.gz` & `tmp/calling_rate-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "calling_rate-0.3.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "calling_rate-0.4.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `calling_rate-0.3.1.tar` & `calling_rate-0.4.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1037 2023-09-19 19:58:50.376750 calling_rate-0.3.1/README.md
--rw-r--r--   0        0        0      212 2023-09-19 19:58:50.376750 calling_rate-0.3.1/calling_rate/__init__.py
--rw-r--r--   0        0        0      623 2023-09-19 19:58:50.376750 calling_rate-0.3.1/calling_rate/curator.py
--rw-r--r--   0        0        0     3252 2023-09-19 19:58:50.376750 calling_rate-0.3.1/calling_rate/number_of_burrows_from_call_rates.py
--rw-r--r--   0        0        0     1512 2023-09-19 19:58:50.376750 calling_rate-0.3.1/calling_rate/raw_data_to_tdp.py
--rw-r--r--   0        0        0      618 2023-09-19 19:58:50.376750 calling_rate-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1605 1970-01-01 00:00:00.000000 calling_rate-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0      833 2024-02-20 19:27:01.246735 calling_rate-0.4.0/README.md
+-rw-r--r--   0        0        0      212 2024-02-20 19:27:01.250735 calling_rate-0.4.0/calling_rate/__init__.py
+-rw-r--r--   0        0        0      623 2024-02-20 19:27:01.250735 calling_rate-0.4.0/calling_rate/curator.py
+-rw-r--r--   0        0        0     4349 2024-02-20 19:27:01.250735 calling_rate-0.4.0/calling_rate/number_of_burrows_from_call_rates.py
+-rw-r--r--   0        0        0     1512 2024-02-20 19:27:01.250735 calling_rate-0.4.0/calling_rate/raw_data_to_tdp.py
+-rw-r--r--   0        0        0      618 2024-02-20 19:27:01.250735 calling_rate-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     1401 1970-01-01 00:00:00.000000 calling_rate-0.4.0/PKG-INFO
```

### Comparing `calling_rate-0.3.1/calling_rate/curator.py` & `calling_rate-0.4.0/calling_rate/curator.py`

 * *Files identical despite different names*

### Comparing `calling_rate-0.3.1/calling_rate/raw_data_to_tdp.py` & `calling_rate-0.4.0/calling_rate/raw_data_to_tdp.py`

 * *Files identical despite different names*

### Comparing `calling_rate-0.3.1/pyproject.toml` & `calling_rate-0.4.0/pyproject.toml`

 * *Files identical despite different names*

