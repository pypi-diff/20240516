# Comparing `tmp/docmesh_core-0.0.3.tar.gz` & `tmp/docmesh_core-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_core-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_core-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_core-0.0.3.tar` & `docmesh_core-0.0.4.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       10 2024-05-13 04:13:58.033801 docmesh_core-0.0.3/README.md
--rw-r--r--   0        0        0       22 2024-05-15 04:29:41.981399 docmesh_core-0.0.3/docmesh_core/__init__.py
--rw-r--r--   0        0        0     1234 2024-05-14 02:57:17.145280 docmesh_core-0.0.3/docmesh_core/db/__init__.py
--rw-r--r--   0        0        0     1325 2024-05-13 04:13:58.033801 docmesh_core-0.0.3/docmesh_core/db/auth.py
--rw-r--r--   0        0        0    10864 2024-05-15 04:29:14.393063 docmesh_core-0.0.3/docmesh_core/db/neo.py
--rw-r--r--   0        0        0      417 2024-05-13 10:34:53.297212 docmesh_core-0.0.3/docmesh_core/utils/__init__.py
--rw-r--r--   0        0        0      269 2024-05-13 04:13:58.037801 docmesh_core-0.0.3/docmesh_core/utils/graph_utils.py
--rw-r--r--   0        0        0     3857 2024-05-13 11:40:13.918990 docmesh_core-0.0.3/docmesh_core/utils/semantic_scholar.py
--rw-r--r--   0        0        0      750 2024-05-13 04:13:58.037801 docmesh_core-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 docmesh_core-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       10 2024-05-13 04:13:58.033801 docmesh_core-0.0.4/README.md
+-rw-r--r--   0        0        0       22 2024-05-16 05:07:40.528095 docmesh_core-0.0.4/docmesh_core/__init__.py
+-rw-r--r--   0        0        0     1244 2024-05-15 11:01:49.702507 docmesh_core-0.0.4/docmesh_core/db/__init__.py
+-rw-r--r--   0        0        0     1325 2024-05-13 04:13:58.033801 docmesh_core-0.0.4/docmesh_core/db/auth.py
+-rw-r--r--   0        0        0    10869 2024-05-15 11:28:37.262344 docmesh_core-0.0.4/docmesh_core/db/neo.py
+-rw-r--r--   0        0        0      417 2024-05-15 10:24:49.939048 docmesh_core-0.0.4/docmesh_core/utils/__init__.py
+-rw-r--r--   0        0        0      269 2024-05-13 04:13:58.037801 docmesh_core-0.0.4/docmesh_core/utils/graph_utils.py
+-rw-r--r--   0        0        0     3857 2024-05-13 11:40:13.918990 docmesh_core-0.0.4/docmesh_core/utils/semantic_scholar.py
+-rw-r--r--   0        0        0      750 2024-05-13 04:13:58.037801 docmesh_core-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 docmesh_core-0.0.4/PKG-INFO
```

### Comparing `docmesh_core-0.0.3/docmesh_core/db/__init__.py` & `docmesh_core-0.0.4/docmesh_core/db/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     list_follows,
     list_popular_entities,
     get_paper_from_id,
     get_paper_from_title,
     add_paper_from_title,
     add_paper_from_arxiv,
     update_papers,
-    read_paper,
+    mark_paper_read,
     list_latest_papers,
     list_unread_similar_papers,
     list_unread_semantic_papers,
     list_unread_follows_papers,
     list_unread_influential_papers,
     list_unembedded_papers,
     get_latest_citegraph,
@@ -37,15 +37,15 @@
     "list_follows",
     "list_popular_entities",
     "get_paper_from_id",
     "get_paper_from_title",
     "add_paper_from_title",
     "add_paper_from_arxiv",
     "update_papers",
-    "read_paper",
+    "mark_paper_read",
     "list_latest_papers",
     "list_unread_similar_papers",
     "list_unread_semantic_papers",
     "list_unread_follows_papers",
     "list_unread_influential_papers",
     "list_unembedded_papers",
     "get_latest_citegraph",
```

### Comparing `docmesh_core-0.0.3/docmesh_core/db/auth.py` & `docmesh_core-0.0.4/docmesh_core/db/auth.py`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.3/docmesh_core/db/neo.py` & `docmesh_core-0.0.4/docmesh_core/db/neo.py`

 * *Files 0% similar despite different names*

```diff
@@ -205,15 +205,15 @@
 @db.transaction
 def update_papers(papers: DataFrame) -> list[Paper]:
     papers: list[Paper] = Paper.create_or_update(*papers.to_dict(orient="records"))
     return papers
 
 
 @db.transaction
-def read_paper(entity_name: str, paper_id: str) -> None:
+def mark_paper_read(entity_name: str, paper_id: str) -> None:
     entity = get_entity(entity_name)
     paper = get_paper_from_id(paper_id=paper_id)
     # XXX: neomodel says that they can ensure relationship uniqueness
     # however, it doesn't
     if not entity.reads.is_connected(paper):
         entity.reads.connect(paper)
```

### Comparing `docmesh_core-0.0.3/docmesh_core/utils/semantic_scholar.py` & `docmesh_core-0.0.4/docmesh_core/utils/semantic_scholar.py`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.3/pyproject.toml` & `docmesh_core-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `docmesh_core-0.0.3/PKG-INFO` & `docmesh_core-0.0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docmesh_core
-Version: 0.0.3
+Version: 0.0.4
 Summary: Core components for docmesh.
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

