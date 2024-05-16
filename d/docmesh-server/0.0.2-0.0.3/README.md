# Comparing `tmp/docmesh_server-0.0.2.tar.gz` & `tmp/docmesh_server-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_server-0.0.2.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_server-0.0.3.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_server-0.0.2.tar` & `docmesh_server-0.0.3.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       16 2024-05-14 04:58:32.409536 docmesh_server-0.0.2/README.md
--rw-r--r--   0        0        0       64 2024-05-15 03:22:41.491751 docmesh_server-0.0.2/docmesh_server/__init__.py
--rw-r--r--   0        0        0     6382 2024-05-15 03:21:46.043064 docmesh_server-0.0.2/docmesh_server/main.py
--rw-r--r--   0        0        0      673 2024-05-15 03:21:52.387143 docmesh_server-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 docmesh_server-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       16 2024-05-14 04:58:32.409536 docmesh_server-0.0.3/README.md
+-rw-r--r--   0        0        0       64 2024-05-16 05:16:57.517248 docmesh_server-0.0.3/docmesh_server/__init__.py
+-rw-r--r--   0        0        0     6397 2024-05-15 11:05:11.588961 docmesh_server-0.0.3/docmesh_server/main.py
+-rw-r--r--   0        0        0      673 2024-05-16 05:17:24.217304 docmesh_server-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      585 1970-01-01 00:00:00.000000 docmesh_server-0.0.3/PKG-INFO
```

### Comparing `docmesh_server-0.0.2/docmesh_server/main.py` & `docmesh_server-0.0.3/docmesh_server/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 from neomodel import config
 from sqlalchemy import create_engine
 from fastapi import status, Depends, HTTPException, Response, FastAPI
 from fastapi.security import HTTPBearer, HTTPAuthorizationCredentials
 
 from docmesh_core.utils.semantic_scholar import get_paper_id
-from docmesh_core.db.neo import add_entity, _add_paper, read_paper, DuplicateEntity
+from docmesh_core.db.neo import add_entity, _add_paper, mark_paper_read, DuplicateEntity
 from docmesh_core.db.auth import get_entity_from_auth, add_auth_for_entity
 from docmesh_agent.agent import execute_docmesh_agent
 from docmesh_agent.embeddings.embeddings import update_paper_embeddings
 
 if (neo4j_url := os.getenv("NEO4J_URL")) is None:
     raise ValueError("You have not set neo4j database url using environment `NEO4J_URL`.")
 else:
@@ -159,24 +159,24 @@
             data = {
                 "msg": f"Failed to add a new paper {body.paper}, with error: {e}.",
             }
 
     return {"data": data}
 
 
-@app.post("/read_paper")
-def read_paper_api(
+@app.post("/mark_paper")
+def mark_paper_read_api(
     body: ReadPaperBody,
     response: Response,
     token: HTTPAuthorizationCredentials = Depends(auth_scheme),
 ) -> dict[str, Any]:
     entity_name = _check_access_token(token.credentials)
 
     try:
-        read_paper(entity_name=entity_name, paper_id=body.paper_id)
+        mark_paper_read(entity_name=entity_name, paper_id=body.paper_id)
         data = {
             "msg": f"Successfully mark paper {body.paper_id} read for {entity_name}.",
         }
     except Exception as e:
         response.status_code = status.HTTP_500_INTERNAL_SERVER_ERROR
         data = {
             "msg": f"Failed to mark paper {body.paper_id} with error: {e}.",
```

### Comparing `docmesh_server-0.0.2/pyproject.toml` & `docmesh_server-0.0.3/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -14,16 +14,16 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Operating System :: OS Independent"
 ]
 requires-python = ">=3.8"
 dependencies = [
-    "docmesh_core>=0.0.2",
-    "docmesh_agent>=0.0.3",
+    "docmesh-core>=0.0.4",
+    "docmesh-agent>=0.0.5",
     "fastapi==0.111.0",
     "uvicorn==0.29.0",
     "gunicorn==19.3.0",
 ]
 
 [tool.flake8]
 max-line-length = 120
```

### Comparing `docmesh_server-0.0.2/PKG-INFO` & `docmesh_server-0.0.3/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: docmesh_server
-Version: 0.0.2
+Version: 0.0.3
 Summary: Server of docmesh.
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Dist: docmesh_core>=0.0.2
-Requires-Dist: docmesh_agent>=0.0.3
+Requires-Dist: docmesh-core>=0.0.4
+Requires-Dist: docmesh-agent>=0.0.5
 Requires-Dist: fastapi==0.111.0
 Requires-Dist: uvicorn==0.29.0
 Requires-Dist: gunicorn==19.3.0
 
 # docemsh server
```

