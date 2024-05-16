# Comparing `tmp/ctidb-1.1.8.tar.gz` & `tmp/ctidb-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctidb-1.1.8.tar", last modified: Tue Jan 23 08:52:32 2024, max compression
+gzip compressed data, was "ctidb-1.1.9.tar", last modified: Tue Mar 26 07:15:37 2024, max compression
```

## Comparing `ctidb-1.1.8.tar` & `ctidb-1.1.9.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwx------   0 root         (0) root         (0)        0 2024-01-23 08:52:32.901704 ctidb-1.1.8/
--rw-------   0 root         (0) root         (0)    11560 2024-01-23 01:39:39.000000 ctidb-1.1.8/LICENSE
--rw-r--r--   0 root         (0) root         (0)     2410 2024-01-23 08:52:32.900704 ctidb-1.1.8/PKG-INFO
--rw-------   0 root         (0) root         (0)     1705 2024-01-23 01:39:38.000000 ctidb-1.1.8/README.rst
-drwx------   0 root         (0) root         (0)        0 2024-01-23 08:52:32.899704 ctidb-1.1.8/ctidb/
--rw-------   0 root         (0) root         (0)      273 2024-01-23 01:39:39.000000 ctidb-1.1.8/ctidb/__init__.py
--rw-------   0 root         (0) root         (0)      581 2024-01-23 01:39:39.000000 ctidb-1.1.8/ctidb/custom.py
--rw-------   0 root         (0) root         (0)     7116 2024-01-23 01:39:39.000000 ctidb-1.1.8/ctidb/decoder.py
--rw-------   0 root         (0) root         (0)    17821 2024-01-23 01:39:39.000000 ctidb-1.1.8/ctidb/reader.py
-drwx------   0 root         (0) root         (0)        0 2024-01-23 08:52:32.900704 ctidb-1.1.8/ctidb.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2410 2024-01-23 08:52:32.000000 ctidb-1.1.8/ctidb.egg-info/PKG-INFO
--rw-------   0 root         (0) root         (0)      238 2024-01-23 08:52:32.000000 ctidb-1.1.8/ctidb.egg-info/SOURCES.txt
--rw-------   0 root         (0) root         (0)        1 2024-01-23 08:52:32.000000 ctidb-1.1.8/ctidb.egg-info/dependency_links.txt
--rw-------   0 root         (0) root         (0)        2 2024-01-23 01:39:39.000000 ctidb-1.1.8/ctidb.egg-info/not-zip-safe
--rw-------   0 root         (0) root         (0)        6 2024-01-23 08:52:32.000000 ctidb-1.1.8/ctidb.egg-info/top_level.txt
--rw-------   0 root         (0) root         (0)       38 2024-01-23 08:52:32.901704 ctidb-1.1.8/setup.cfg
--rw-------   0 root         (0) root         (0)     1816 2024-01-23 01:39:38.000000 ctidb-1.1.8/setup.py
+drwx------   0 root         (0) root         (0)        0 2024-03-26 07:15:37.723858 ctidb-1.1.9/
+-rw-------   0 root         (0) root         (0)    11560 2024-01-30 03:35:06.000000 ctidb-1.1.9/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-03-26 07:15:37.723858 ctidb-1.1.9/PKG-INFO
+-rw-------   0 root         (0) root         (0)     1705 2024-01-30 03:35:05.000000 ctidb-1.1.9/README.rst
+drwx------   0 root         (0) root         (0)        0 2024-03-26 07:15:37.720858 ctidb-1.1.9/ctidb/
+-rw-------   0 root         (0) root         (0)      273 2024-03-26 07:14:29.000000 ctidb-1.1.9/ctidb/__init__.py
+-rw-------   0 root         (0) root         (0)      581 2024-03-26 07:14:29.000000 ctidb-1.1.9/ctidb/custom.py
+-rw-------   0 root         (0) root         (0)     7116 2024-03-26 07:14:29.000000 ctidb-1.1.9/ctidb/decoder.py
+-rw-------   0 root         (0) root         (0)    17959 2024-03-26 07:14:29.000000 ctidb-1.1.9/ctidb/reader.py
+drwx------   0 root         (0) root         (0)        0 2024-03-26 07:15:37.722858 ctidb-1.1.9/ctidb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2410 2024-03-26 07:15:37.000000 ctidb-1.1.9/ctidb.egg-info/PKG-INFO
+-rw-------   0 root         (0) root         (0)      238 2024-03-26 07:15:37.000000 ctidb-1.1.9/ctidb.egg-info/SOURCES.txt
+-rw-------   0 root         (0) root         (0)        1 2024-03-26 07:15:37.000000 ctidb-1.1.9/ctidb.egg-info/dependency_links.txt
+-rw-------   0 root         (0) root         (0)        2 2024-01-23 01:39:39.000000 ctidb-1.1.9/ctidb.egg-info/not-zip-safe
+-rw-------   0 root         (0) root         (0)        6 2024-03-26 07:15:37.000000 ctidb-1.1.9/ctidb.egg-info/top_level.txt
+-rw-------   0 root         (0) root         (0)       38 2024-03-26 07:15:37.723858 ctidb-1.1.9/setup.cfg
+-rw-------   0 root         (0) root         (0)     1816 2024-01-30 03:35:05.000000 ctidb-1.1.9/setup.py
```

### Comparing `ctidb-1.1.8/LICENSE` & `ctidb-1.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `ctidb-1.1.8/PKG-INFO` & `ctidb-1.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctidb
-Version: 1.1.8
+Version: 1.1.9
 Summary: criminalip.ctidb reader
 Home-page: https://github.com/aispera/ctidb
 Author: aispera
 Author-email: infra@aispera.com
 License: Apache License, Version 2.0
 Keywords: aispera,ctidb,criminalip
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ctidb-1.1.8/README.rst` & `ctidb-1.1.9/README.rst`

 * *Files identical despite different names*

### Comparing `ctidb-1.1.8/ctidb/custom.py` & `ctidb-1.1.9/ctidb/custom.py`

 * *Files identical despite different names*

### Comparing `ctidb-1.1.8/ctidb/decoder.py` & `ctidb-1.1.9/ctidb/decoder.py`

 * *Files identical despite different names*

### Comparing `ctidb-1.1.8/ctidb/reader.py` & `ctidb-1.1.9/ctidb/reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -110,15 +110,17 @@
         langdata_start = self._buffer.rfind(
             self._LANGDATA_START_MARKER, max(0, self._buffer_size - int(self._buffer_size / 2))
         )
         self._metadata_lange = None
         self._metadata_cache = dict()
         self._metadata_cache_tmp = dict()
         if -1 != langdata_start:
-            self._metadata_lange = json.loads(self._buffer[langdata_start + len(self._LANGDATA_START_MARKER):])
+            self._metadata_lange_tmp = json.loads(self._buffer[langdata_start + len(self._LANGDATA_START_MARKER):])
+            self._metadata_lange = dict(zip(self._metadata_lange_tmp.values(),self._metadata_lange_tmp.keys()))
+            self._metadata_lange_tmp.clear()
 
         self._decoder = Decoder(
             self._buffer,
             self._metadata.search_tree_size + self._DATA_SECTION_SEPARATOR_SIZE,
         )
 
         tmp_description = self._metadata.description.get('description', '')
@@ -309,15 +311,15 @@
                     if idx in self._metadata_cache:
                         value = self._metadata_cache[idx]
                     else:
                         if idx not in self._metadata_cache_tmp:
                             self._metadata_cache_tmp[idx] = 0
                         self._metadata_cache_tmp[idx] = self._metadata_cache_tmp[idx] + 1
 
-                        value = [k for k, v in self._metadata_lange.items() if v == idx]
+                        value = [self._metadata_lange.get(idx)]
                         if 3 <= self._metadata_cache_tmp[idx]:
                             self._metadata_cache[idx] = value
                             del self._metadata_cache_tmp[idx]
 
                         if 100 <= len(self._metadata_cache_tmp):
                             self._metadata_cache_tmp.clear()
```

### Comparing `ctidb-1.1.8/ctidb.egg-info/PKG-INFO` & `ctidb-1.1.9/ctidb.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ctidb
-Version: 1.1.8
+Version: 1.1.9
 Summary: criminalip.ctidb reader
 Home-page: https://github.com/aispera/ctidb
 Author: aispera
 Author-email: infra@aispera.com
 License: Apache License, Version 2.0
 Keywords: aispera,ctidb,criminalip
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `ctidb-1.1.8/setup.py` & `ctidb-1.1.9/setup.py`

 * *Files identical despite different names*

