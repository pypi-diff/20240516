# Comparing `tmp/ghostfolio-0.3.0.tar.gz` & `tmp/ghostfolio-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghostfolio-0.3.0.tar", last modified: Sat Oct 21 13:04:13 2023, max compression
+gzip compressed data, was "ghostfolio-0.4.0.tar", last modified: Thu May 16 20:35:21 2024, max compression
```

## Comparing `ghostfolio-0.3.0.tar` & `ghostfolio-0.4.0.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-10-21 13:04:13.262988 ghostfolio-0.3.0/
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)    11347 2023-07-02 18:34:37.000000 ghostfolio-0.3.0/LICENSE
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      281 2023-10-21 13:04:13.262988 ghostfolio-0.3.0/PKG-INFO
-drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-10-21 13:04:13.262988 ghostfolio-0.3.0/ghostfolio/
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)     3785 2023-10-21 12:10:03.000000 ghostfolio-0.3.0/ghostfolio/__init__.py
-drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2023-10-21 13:04:13.262988 ghostfolio-0.3.0/ghostfolio.egg-info/
--rw-r--r--   0 ms32035   (1000) ms32035   (1000)      281 2023-10-21 13:04:13.000000 ghostfolio-0.3.0/ghostfolio.egg-info/PKG-INFO
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)      214 2023-10-21 13:04:13.000000 ghostfolio-0.3.0/ghostfolio.egg-info/SOURCES.txt
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)        1 2023-10-21 13:04:13.000000 ghostfolio-0.3.0/ghostfolio.egg-info/dependency_links.txt
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)        9 2023-10-21 13:04:13.000000 ghostfolio-0.3.0/ghostfolio.egg-info/requires.txt
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)       16 2023-10-21 13:04:13.000000 ghostfolio-0.3.0/ghostfolio.egg-info/top_level.txt
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)      356 2023-10-21 12:10:48.000000 ghostfolio-0.3.0/pyproject.toml
--rw-rw-r--   0 ms32035   (1000) ms32035   (1000)       38 2023-10-21 13:04:13.262988 ghostfolio-0.3.0/setup.cfg
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2024-05-16 20:35:21.838755 ghostfolio-0.4.0/
+-rw-rw-r--   0 ms32035   (1000) ms32035   (1000)    11347 2023-07-02 18:34:37.000000 ghostfolio-0.4.0/LICENSE
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      281 2024-05-16 20:35:21.838755 ghostfolio-0.4.0/PKG-INFO
+-rw-rw-r--   0 ms32035   (1000) ms32035   (1000)      291 2023-07-02 18:34:37.000000 ghostfolio-0.4.0/README.md
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2024-05-16 20:35:21.837755 ghostfolio-0.4.0/ghostfolio/
+-rw-rw-r--   0 ms32035   (1000) ms32035   (1000)     3783 2024-05-16 18:05:52.000000 ghostfolio-0.4.0/ghostfolio/__init__.py
+drwxrwxr-x   0 ms32035   (1000) ms32035   (1000)        0 2024-05-16 20:35:21.838755 ghostfolio-0.4.0/ghostfolio.egg-info/
+-rw-r--r--   0 ms32035   (1000) ms32035   (1000)      281 2024-05-16 20:35:21.000000 ghostfolio-0.4.0/ghostfolio.egg-info/PKG-INFO
+-rw-rw-r--   0 ms32035   (1000) ms32035   (1000)      224 2024-05-16 20:35:21.000000 ghostfolio-0.4.0/ghostfolio.egg-info/SOURCES.txt
+-rw-rw-r--   0 ms32035   (1000) ms32035   (1000)        1 2024-05-16 20:35:21.000000 ghostfolio-0.4.0/ghostfolio.egg-info/dependency_links.txt
+-rw-rw-r--   0 ms32035   (1000) ms32035   (1000)        9 2024-05-16 20:35:21.000000 ghostfolio-0.4.0/ghostfolio.egg-info/requires.txt
+-rw-rw-r--   0 ms32035   (1000) ms32035   (1000)       22 2024-05-16 20:35:21.000000 ghostfolio-0.4.0/ghostfolio.egg-info/top_level.txt
+-rw-rw-r--   0 ms32035   (1000) ms32035   (1000)      356 2024-05-16 18:05:15.000000 ghostfolio-0.4.0/pyproject.toml
+-rw-rw-r--   0 ms32035   (1000) ms32035   (1000)       38 2024-05-16 20:35:21.838755 ghostfolio-0.4.0/setup.cfg
```

### Comparing `ghostfolio-0.3.0/LICENSE` & `ghostfolio-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ghostfolio-0.3.0/ghostfolio/__init__.py` & `ghostfolio-0.4.0/ghostfolio/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -63,16 +63,16 @@
         return self._get("order", params=params)
 
     def performance(self, date_range: str = "max") -> dict:
         return self._get(
             "portfolio/performance", params={"range": date_range}, api_version="v2"
         )
 
-    def positions(self, date_range: str = "max") -> dict:
-        return self._get("portfolio/positions", params={"range": date_range})
+    def holdings(self, date_range: str = "max") -> dict:
+        return self._get("portfolio/holdings", params={"range": date_range})
 
     def position(self, data_source: str, symbol: str):
         """Get position for a symbol from a data source."""
         return self._get(f"portfolio/position/{data_source}/{symbol}")
 
     def import_transactions(self, data: dict):
         """Import transactions."""
```

