# Comparing `tmp/geneweaver_db-0.4.0a2.tar.gz` & `tmp/geneweaver_db-0.4.0a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_db-0.4.0a2.tar", max compression
+gzip compressed data, was "geneweaver_db-0.4.0a3.tar", max compression
```

## Comparing `geneweaver_db-0.4.0a2.tar` & `geneweaver_db-0.4.0a3.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11356 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/LICENSE
--rw-r--r--   0        0        0     2162 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/README.md
--rw-r--r--   0        0        0      955 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/pyproject.toml
--rw-r--r--   0        0        0      156 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/src/geneweaver/db/__init__.py
--rw-r--r--   0        0        0      132 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/src/geneweaver/db/aio/__init__.py
--rw-r--r--   0        0        0     3134 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/src/geneweaver/db/aio/gene.py
--rw-r--r--   0        0        0     5163 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/src/geneweaver/db/aio/geneset.py
--rw-r--r--   0        0        0     2189 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/src/geneweaver/db/aio/publication.py
--rw-r--r--   0        0        0     1310 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/src/geneweaver/db/aio/species.py
--rw-r--r--   0        0        0      809 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/src/geneweaver/db/aio/threshold.py
--rw-r--r--   0        0        0       56 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/core/__init__.py
--rw-r--r--   0        0        0      845 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/core/cursor.py
--rw-r--r--   0        0        0      145 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/core/settings.py
--rw-r--r--   0        0        0     1769 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/core/settings_class.py
--rw-r--r--   0        0        0      438 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/exceptions.py
--rw-r--r--   0        0        0    10316 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/gene.py
--rw-r--r--   0        0        0     8981 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/geneset.py
--rw-r--r--   0        0        0     7887 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/geneset_value.py
--rw-r--r--   0        0        0     2063 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/publication.py
--rw-r--r--   0        0        0       42 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/__init__.py
--rw-r--r--   0        0        0     5410 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/gene.py
--rw-r--r--   0        0        0      364 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/__init__.py
--rw-r--r--   0        0        0     1351 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/const.py
--rw-r--r--   0        0        0     5492 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/read.py
--rw-r--r--   0        0        0     4824 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/utils.py
--rw-r--r--   0        0        0     4014 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/write.py
--rw-r--r--   0        0        0      982 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/project.py
--rw-r--r--   0        0        0     4683 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/publication.py
--rw-r--r--   0        0        0       60 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/search/__init__.py
--rw-r--r--   0        0        0       50 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/search/search.py
--rw-r--r--   0        0        0     1571 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/search/utils.py
--rw-r--r--   0        0        0     1603 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/species.py
--rw-r--r--   0        0        0     2900 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/threshold.py
--rw-r--r--   0        0        0     1782 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/utils.py
--rw-r--r--   0        0        0     1249 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/species.py
--rw-r--r--   0        0        0      775 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/threshold.py
--rw-r--r--   0        0        0     6887 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/user.py
--rw-r--r--   0        0        0     3201 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/utils.py
--rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 geneweaver_db-0.4.0a2/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/LICENSE
+-rw-r--r--   0        0        0     2162 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/README.md
+-rw-r--r--   0        0        0      955 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/aio/__init__.py
+-rw-r--r--   0        0        0     3134 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/aio/gene.py
+-rw-r--r--   0        0        0     5163 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/aio/geneset.py
+-rw-r--r--   0        0        0     2189 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/aio/publication.py
+-rw-r--r--   0        0        0     1310 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/aio/species.py
+-rw-r--r--   0        0        0      809 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/aio/threshold.py
+-rw-r--r--   0        0        0       56 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/core/__init__.py
+-rw-r--r--   0        0        0      845 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/core/cursor.py
+-rw-r--r--   0        0        0      145 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/core/settings.py
+-rw-r--r--   0        0        0     1769 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/core/settings_class.py
+-rw-r--r--   0        0        0      438 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/exceptions.py
+-rw-r--r--   0        0        0    10316 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/gene.py
+-rw-r--r--   0        0        0     8981 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/geneset.py
+-rw-r--r--   0        0        0     7887 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/geneset_value.py
+-rw-r--r--   0        0        0     2063 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/publication.py
+-rw-r--r--   0        0        0       42 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/__init__.py
+-rw-r--r--   0        0        0     5410 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/gene.py
+-rw-r--r--   0        0        0      364 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/__init__.py
+-rw-r--r--   0        0        0     1351 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/const.py
+-rw-r--r--   0        0        0     5492 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/read.py
+-rw-r--r--   0        0        0     4824 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/utils.py
+-rw-r--r--   0        0        0     4014 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/write.py
+-rw-r--r--   0        0        0      982 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/project.py
+-rw-r--r--   0        0        0     4683 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/publication.py
+-rw-r--r--   0        0        0       60 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/search/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/search/search.py
+-rw-r--r--   0        0        0     1572 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/search/utils.py
+-rw-r--r--   0        0        0     1603 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/species.py
+-rw-r--r--   0        0        0     2900 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/threshold.py
+-rw-r--r--   0        0        0     1782 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/query/utils.py
+-rw-r--r--   0        0        0     1249 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/species.py
+-rw-r--r--   0        0        0      775 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/threshold.py
+-rw-r--r--   0        0        0     6887 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/user.py
+-rw-r--r--   0        0        0     3201 2024-05-16 19:46:23.051550 geneweaver_db-0.4.0a3/src/geneweaver/db/utils.py
+-rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 geneweaver_db-0.4.0a3/PKG-INFO
```

### Comparing `geneweaver_db-0.4.0a2/LICENSE` & `geneweaver_db-0.4.0a3/LICENSE`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/README.md` & `geneweaver_db-0.4.0a3/README.md`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/pyproject.toml` & `geneweaver_db-0.4.0a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geneweaver-db"
-version = "0.4.0a2"
+version = "0.4.0a3"
 description = "Database Interaction Services for GeneWeaver"
 authors = ["Jax Computational Sciences <cssc@jax.org>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://thejacksonlaboratory.github.io/geneweaver-docs/"
 repository = "https://github.com/TheJacksonLaboratory/geneweaver-db"
 packages = [
```

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/aio/gene.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/aio/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/aio/geneset.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/aio/geneset.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/aio/publication.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/aio/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/aio/species.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/aio/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/aio/threshold.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/aio/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/core/cursor.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/core/cursor.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/core/settings_class.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/core/settings_class.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/gene.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/geneset.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/geneset.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/geneset_value.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/geneset_value.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/publication.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/query/gene.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/query/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/const.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/const.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/read.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/read.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/utils.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/write.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/query/geneset/write.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/query/project.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/query/project.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/query/publication.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/query/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/query/search/utils.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/query/search/utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     QueryType.WEBSEARCH: SQL("@@ websearch_to_tsquery({search_config}, %(search)s)"),
 }
 
 
 def search_query(
     search_column: Composed,
     search_string: str,
-    search_config: SearchConfig = SearchConfig.SIMPLE,
+    search_config: SearchConfig = SearchConfig.ENGLISH,
     query_type: QueryType = QueryType.WEBSEARCH,
 ) -> Tuple[Composed, dict]:
     """Generate a search query.
 
     Works generically with any table that has a search column.
 
     :param search_column: The column to search.
```

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/query/species.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/query/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/query/threshold.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/query/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/query/utils.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/query/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/species.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/threshold.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/user.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/user.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/src/geneweaver/db/utils.py` & `geneweaver_db-0.4.0a3/src/geneweaver/db/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a2/PKG-INFO` & `geneweaver_db-0.4.0a3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneweaver-db
-Version: 0.4.0a2
+Version: 0.4.0a3
 Summary: Database Interaction Services for GeneWeaver
 Home-page: https://thejacksonlaboratory.github.io/geneweaver-docs/
 License: Apache-2.0
 Author: Jax Computational Sciences
 Author-email: cssc@jax.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

