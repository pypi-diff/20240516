# Comparing `tmp/geneweaver_db-0.4.0a1.tar.gz` & `tmp/geneweaver_db-0.4.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geneweaver_db-0.4.0a1.tar", max compression
+gzip compressed data, was "geneweaver_db-0.4.0a2.tar", max compression
```

## Comparing `geneweaver_db-0.4.0a1.tar` & `geneweaver_db-0.4.0a2.tar`

### file list

```diff
@@ -1,39 +1,39 @@
--rw-r--r--   0        0        0    11356 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/LICENSE
--rw-r--r--   0        0        0     2162 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/README.md
--rw-r--r--   0        0        0      955 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/pyproject.toml
--rw-r--r--   0        0        0      156 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/__init__.py
--rw-r--r--   0        0        0      132 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/aio/__init__.py
--rw-r--r--   0        0        0     3134 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/aio/gene.py
--rw-r--r--   0        0        0     5009 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/aio/geneset.py
--rw-r--r--   0        0        0     2189 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/aio/publication.py
--rw-r--r--   0        0        0     1310 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/aio/species.py
--rw-r--r--   0        0        0      809 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/aio/threshold.py
--rw-r--r--   0        0        0       56 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/core/__init__.py
--rw-r--r--   0        0        0      845 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/core/cursor.py
--rw-r--r--   0        0        0      145 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/core/settings.py
--rw-r--r--   0        0        0     1769 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/core/settings_class.py
--rw-r--r--   0        0        0      438 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/exceptions.py
--rw-r--r--   0        0        0    10316 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/gene.py
--rw-r--r--   0        0        0     8827 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/geneset.py
--rw-r--r--   0        0        0     7887 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/geneset_value.py
--rw-r--r--   0        0        0     2063 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/publication.py
--rw-r--r--   0        0        0       42 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/__init__.py
--rw-r--r--   0        0        0     5410 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/gene.py
--rw-r--r--   0        0        0      364 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/geneset/__init__.py
--rw-r--r--   0        0        0     1351 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/geneset/const.py
--rw-r--r--   0        0        0     5287 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/geneset/read.py
--rw-r--r--   0        0        0     4824 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/geneset/utils.py
--rw-r--r--   0        0        0     4014 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/geneset/write.py
--rw-r--r--   0        0        0      982 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/project.py
--rw-r--r--   0        0        0     4683 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/publication.py
--rw-r--r--   0        0        0       60 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/search/__init__.py
--rw-r--r--   0        0        0       50 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/search/search.py
--rw-r--r--   0        0        0     1571 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/search/utils.py
--rw-r--r--   0        0        0     1603 2024-05-10 16:57:06.870767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/species.py
--rw-r--r--   0        0        0     2900 2024-05-10 16:57:06.874767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/threshold.py
--rw-r--r--   0        0        0     1782 2024-05-10 16:57:06.874767 geneweaver_db-0.4.0a1/src/geneweaver/db/query/utils.py
--rw-r--r--   0        0        0     1249 2024-05-10 16:57:06.874767 geneweaver_db-0.4.0a1/src/geneweaver/db/species.py
--rw-r--r--   0        0        0      775 2024-05-10 16:57:06.874767 geneweaver_db-0.4.0a1/src/geneweaver/db/threshold.py
--rw-r--r--   0        0        0     6887 2024-05-10 16:57:06.874767 geneweaver_db-0.4.0a1/src/geneweaver/db/user.py
--rw-r--r--   0        0        0     3201 2024-05-10 16:57:06.874767 geneweaver_db-0.4.0a1/src/geneweaver/db/utils.py
--rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 geneweaver_db-0.4.0a1/PKG-INFO
+-rw-r--r--   0        0        0    11356 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/LICENSE
+-rw-r--r--   0        0        0     2162 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/README.md
+-rw-r--r--   0        0        0      955 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/pyproject.toml
+-rw-r--r--   0        0        0      156 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/src/geneweaver/db/__init__.py
+-rw-r--r--   0        0        0      132 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/src/geneweaver/db/aio/__init__.py
+-rw-r--r--   0        0        0     3134 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/src/geneweaver/db/aio/gene.py
+-rw-r--r--   0        0        0     5163 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/src/geneweaver/db/aio/geneset.py
+-rw-r--r--   0        0        0     2189 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/src/geneweaver/db/aio/publication.py
+-rw-r--r--   0        0        0     1310 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/src/geneweaver/db/aio/species.py
+-rw-r--r--   0        0        0      809 2024-05-16 14:35:40.606760 geneweaver_db-0.4.0a2/src/geneweaver/db/aio/threshold.py
+-rw-r--r--   0        0        0       56 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/core/__init__.py
+-rw-r--r--   0        0        0      845 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/core/cursor.py
+-rw-r--r--   0        0        0      145 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/core/settings.py
+-rw-r--r--   0        0        0     1769 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/core/settings_class.py
+-rw-r--r--   0        0        0      438 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/exceptions.py
+-rw-r--r--   0        0        0    10316 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/gene.py
+-rw-r--r--   0        0        0     8981 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/geneset.py
+-rw-r--r--   0        0        0     7887 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/geneset_value.py
+-rw-r--r--   0        0        0     2063 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/publication.py
+-rw-r--r--   0        0        0       42 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/__init__.py
+-rw-r--r--   0        0        0     5410 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/gene.py
+-rw-r--r--   0        0        0      364 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/__init__.py
+-rw-r--r--   0        0        0     1351 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/const.py
+-rw-r--r--   0        0        0     5492 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/read.py
+-rw-r--r--   0        0        0     4824 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/utils.py
+-rw-r--r--   0        0        0     4014 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/write.py
+-rw-r--r--   0        0        0      982 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/project.py
+-rw-r--r--   0        0        0     4683 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/publication.py
+-rw-r--r--   0        0        0       60 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/search/__init__.py
+-rw-r--r--   0        0        0       50 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/search/search.py
+-rw-r--r--   0        0        0     1571 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/search/utils.py
+-rw-r--r--   0        0        0     1603 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/species.py
+-rw-r--r--   0        0        0     2900 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/threshold.py
+-rw-r--r--   0        0        0     1782 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/query/utils.py
+-rw-r--r--   0        0        0     1249 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/species.py
+-rw-r--r--   0        0        0      775 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/threshold.py
+-rw-r--r--   0        0        0     6887 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/user.py
+-rw-r--r--   0        0        0     3201 2024-05-16 14:35:40.610760 geneweaver_db-0.4.0a2/src/geneweaver/db/utils.py
+-rw-r--r--   0        0        0     2984 1970-01-01 00:00:00.000000 geneweaver_db-0.4.0a2/PKG-INFO
```

### Comparing `geneweaver_db-0.4.0a1/LICENSE` & `geneweaver_db-0.4.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/README.md` & `geneweaver_db-0.4.0a2/README.md`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/pyproject.toml` & `geneweaver_db-0.4.0a2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "geneweaver-db"
-version = "0.4.0a1"
+version = "0.4.0a2"
 description = "Database Interaction Services for GeneWeaver"
 authors = ["Jax Computational Sciences <cssc@jax.org>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://thejacksonlaboratory.github.io/geneweaver-docs/"
 repository = "https://github.com/TheJacksonLaboratory/geneweaver-db"
 packages = [
```

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/aio/gene.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/aio/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/aio/geneset.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/aio/geneset.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Async database interaction code relating to Genesets."""
 
 from typing import List, Optional
 
-from geneweaver.core.enum import GeneIdentifier, Species
+from geneweaver.core.enum import GeneIdentifier, ScoreType, Species
 from geneweaver.db.query import geneset as geneset_query
 from geneweaver.db.utils import GenesetTierOrTiers
 from psycopg import AsyncCursor
 from psycopg.rows import Row
 
 
 async def get(
@@ -22,14 +22,15 @@
     gene_id_type: Optional[GeneIdentifier] = None,
     search_text: Optional[str] = None,
     limit: Optional[int] = None,
     offset: Optional[int] = None,
     is_readable_by: Optional[int] = None,
     with_publication_info: bool = True,
     ontology_term: Optional[str] = None,
+    score_type: Optional[ScoreType] = None,
 ) -> List[Row]:
     """Get genesets from the database.
 
     :param cursor: An async database cursor.
     :param gs_id: Show only results with this geneset ID.
     :param owner_id: Show only results owned by this user ID.
     :param curation_tier: Show only results of this curation tier.
@@ -42,14 +43,15 @@
     :param search_text: Return genesets that match this search text (using PostgreSQL
                         full-text search).
     :param limit: Limit the number of results.
     :param offset: Offset the results.
     :param is_readable_by: A user ID to check if the user can read the results.
     :param with_publication_info: Include publication info in the return.
     :param ontology_term: Show only results associated with this ontology term.
+    :param score_type: Show only results with given score type.
 
     :return: list of results using `.fetchall()`
     """
     await cursor.execute(
         *geneset_query.get(
             is_readable_by=is_readable_by,
             gs_id=gs_id,
@@ -62,14 +64,15 @@
             pubmed_id=pubmed_id,
             gene_id_type=gene_id_type,
             search_text=search_text,
             limit=limit,
             offset=offset,
             with_publication_info=with_publication_info,
             ontology_term=ontology_term,
+            score_type=score_type,
         )
     )
 
     return await cursor.fetchall()
 
 
 async def by_id(
```

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/aio/publication.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/aio/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/aio/species.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/aio/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/aio/threshold.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/aio/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/core/cursor.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/core/cursor.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/core/settings_class.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/core/settings_class.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/gene.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/geneset.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/geneset.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """Geneset database functions."""
 
 from typing import List, Optional
 
-from geneweaver.core.enum import GeneIdentifier, Species
+from geneweaver.core.enum import GeneIdentifier, ScoreType, Species
 from geneweaver.db.query import geneset as geneset_query
 from geneweaver.db.utils import GenesetTierOrTiers, temp_override_row_factory
 from psycopg import Cursor, rows
 from psycopg.rows import Row
 
 
 def get(
@@ -22,14 +22,15 @@
     pubmed_id: Optional[int] = None,
     gene_id_type: Optional[GeneIdentifier] = None,
     search_text: Optional[str] = None,
     limit: Optional[int] = None,
     offset: Optional[int] = None,
     with_publication_info: bool = True,
     ontology_term: Optional[str] = None,
+    score_type: Optional[ScoreType] = None,
 ) -> List[Row]:
     """Get genesets from the database.
 
     :param cursor: An async database cursor.
     :param is_readable_by: A user ID to check if the user can read the results.
     :param gs_id: Show only results with this geneset ID.
     :param owner_id: Show only results owned by this user ID.
@@ -42,14 +43,15 @@
     :param gene_id_type: Show only results with this gene ID type.
     :param search_text: Return genesets that match this search text (using PostgreSQL
                         full-text search).
     :param limit: Limit the number of results.
     :param offset: Offset the results.
     :param with_publication_info: Include publication info in the return.
     :param ontology_term: Show only results associated with this ontology term.
+    :param score_type: Show only results with given score type.
 
     :return: list of results using `.fetchall()`
     """
     cursor.execute(
         *geneset_query.get(
             is_readable_by=is_readable_by,
             gs_id=gs_id,
@@ -62,14 +64,15 @@
             pubmed_id=pubmed_id,
             gene_id_type=gene_id_type,
             search_text=search_text,
             limit=limit,
             offset=offset,
             with_publication_info=with_publication_info,
             ontology_term=ontology_term,
+            score_type=score_type,
         )
     )
 
     return cursor.fetchall()
 
 
 def by_id(
```

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/geneset_value.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/geneset_value.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/publication.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/query/gene.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/query/gene.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/query/geneset/const.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/const.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/query/geneset/read.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/read.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 """SQL query generation code for reading genesets."""
 
 from typing import Optional, Tuple
 
-from geneweaver.core.enum import GeneIdentifier, Species
+from geneweaver.core.enum import GeneIdentifier, ScoreType, Species
 from geneweaver.db.query.geneset.utils import (
     add_ontology_parameter,
     add_ontology_query,
     format_select_query,
     is_readable,
     restrict_tier,
     search,
@@ -29,14 +29,15 @@
     search_text: Optional[str] = None,
     status: Optional[str] = "normal",
     limit: Optional[int] = None,
     offset: Optional[int] = None,
     is_readable_by: Optional[int] = None,
     with_publication_info: bool = True,
     ontology_term: Optional[str] = None,
+    score_type: Optional[ScoreType] = None,
 ) -> Tuple[Composed, dict]:
     """Get genesets.
 
     :param gs_id: Show only results with this geneset ID.
     :param owner_id: Show only results owned by this user ID.
     :param curation_tier: Show only results of this curation tier.
     :param species: Show only results associated with this species.
@@ -49,14 +50,15 @@
                         full-text search).
     :param status: Show only results with this status. Default is "normal".
     :param limit: Limit the number of results.
     :param offset: Offset the results.
     :param is_readable_by: A user ID to check if the user can read the results.
     :param with_publication_info: Include publication info in the return.
     :param ontology_term: Show only results associated with this ontology term.
+    :param score_type: Show only results with given score type.
     """
     params = {}
     filtering = []
     query = format_select_query(
         with_publication_info=with_publication_info,
         with_publication_join=pubmed_id is not None,
     )
@@ -83,14 +85,15 @@
             "sp_id": int(species) if species is not None else None,
             "gs_name": name,
             "gs_abbreviation": abbreviation,
             "pub_id": publication_id,
             "pub_pubmed": str(pubmed_id) if pubmed_id is not None else None,
             "gs_gene_id_type": int(gene_id_type) if gene_id_type is not None else None,
             "gs_status": status,
+            "gs_threshold_type": int(score_type) if score_type is not None else None,
         },
     )
 
     if len(filtering) > 0:
         query += SQL("WHERE") + SQL("AND").join(filtering)
 
     query = limit_and_offset(query, limit, offset).join(" ")
```

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/query/geneset/utils.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/query/geneset/write.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/query/geneset/write.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/query/project.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/query/project.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/query/publication.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/query/publication.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/query/search/utils.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/query/search/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/query/species.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/query/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/query/threshold.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/query/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/query/utils.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/query/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/species.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/species.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/threshold.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/threshold.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/user.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/user.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/src/geneweaver/db/utils.py` & `geneweaver_db-0.4.0a2/src/geneweaver/db/utils.py`

 * *Files identical despite different names*

### Comparing `geneweaver_db-0.4.0a1/PKG-INFO` & `geneweaver_db-0.4.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geneweaver-db
-Version: 0.4.0a1
+Version: 0.4.0a2
 Summary: Database Interaction Services for GeneWeaver
 Home-page: https://thejacksonlaboratory.github.io/geneweaver-docs/
 License: Apache-2.0
 Author: Jax Computational Sciences
 Author-email: cssc@jax.org
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
```

