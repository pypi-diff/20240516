# Comparing `tmp/docmesh_agent-0.0.4.tar.gz` & `tmp/docmesh_agent-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "docmesh_agent-0.0.4.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "docmesh_agent-0.0.5.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `docmesh_agent-0.0.4.tar` & `docmesh_agent-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0       15 2024-05-10 12:01:09.706198 docmesh_agent-0.0.4/README.md
--rw-r--r--   0        0        0       22 2024-05-15 03:04:04.129896 docmesh_agent-0.0.4/docmesh_agent/__init__.py
--rw-r--r--   0        0        0     1799 2024-05-15 02:56:58.892615 docmesh_agent-0.0.4/docmesh_agent/agent.py
--rw-r--r--   0        0        0      136 2024-05-14 03:33:52.820396 docmesh_agent-0.0.4/docmesh_agent/embeddings/__init__.py
--rw-r--r--   0        0        0     1404 2024-05-14 03:33:17.744088 docmesh_agent-0.0.4/docmesh_agent/embeddings/embeddings.py
--rw-r--r--   0        0        0       88 2024-05-10 11:02:39.301355 docmesh_agent-0.0.4/docmesh_agent/parser/__init__.py
--rw-r--r--   0        0        0      788 2024-05-10 11:14:17.156634 docmesh_agent-0.0.4/docmesh_agent/parser/output_parser.py
--rw-r--r--   0        0        0      186 2024-05-10 11:02:39.301355 docmesh_agent-0.0.4/docmesh_agent/toolkit/__init__.py
--rw-r--r--   0        0        0      531 2024-05-10 11:17:03.765428 docmesh_agent-0.0.4/docmesh_agent/toolkit/entity.py
--rw-r--r--   0        0        0      787 2024-05-11 04:38:52.647986 docmesh_agent-0.0.4/docmesh_agent/toolkit/paper.py
--rw-r--r--   0        0        0      625 2024-05-13 03:31:55.262732 docmesh_agent-0.0.4/docmesh_agent/toolkit/recommend.py
--rw-r--r--   0        0        0      741 2024-05-13 03:31:34.698480 docmesh_agent-0.0.4/docmesh_agent/tools/__init__.py
--rw-r--r--   0        0        0     1104 2024-05-10 11:02:39.301355 docmesh_agent-0.0.4/docmesh_agent/tools/base.py
--rw-r--r--   0        0        0     2304 2024-05-13 04:13:58.029801 docmesh_agent-0.0.4/docmesh_agent/tools/entity.py
--rw-r--r--   0        0        0     3936 2024-05-13 04:13:58.033801 docmesh_agent-0.0.4/docmesh_agent/tools/graph_tools.py
--rw-r--r--   0        0        0     5760 2024-05-14 06:38:24.001928 docmesh_agent-0.0.4/docmesh_agent/tools/paper.py
--rw-r--r--   0        0        0     4384 2024-05-14 03:34:39.156802 docmesh_agent-0.0.4/docmesh_agent/tools/recommend.py
--rw-r--r--   0        0        0      680 2024-05-14 06:51:11.184595 docmesh_agent-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      583 1970-01-01 00:00:00.000000 docmesh_agent-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       15 2024-05-10 12:01:09.706198 docmesh_agent-0.0.5/README.md
+-rw-r--r--   0        0        0       22 2024-05-16 05:02:55.471515 docmesh_agent-0.0.5/docmesh_agent/__init__.py
+-rw-r--r--   0        0        0     1799 2024-05-15 02:56:58.892615 docmesh_agent-0.0.5/docmesh_agent/agent.py
+-rw-r--r--   0        0        0      136 2024-05-14 03:33:52.820396 docmesh_agent-0.0.5/docmesh_agent/embeddings/__init__.py
+-rw-r--r--   0        0        0     1404 2024-05-14 03:33:17.744088 docmesh_agent-0.0.5/docmesh_agent/embeddings/embeddings.py
+-rw-r--r--   0        0        0       88 2024-05-10 11:02:39.301355 docmesh_agent-0.0.5/docmesh_agent/parser/__init__.py
+-rw-r--r--   0        0        0      788 2024-05-10 11:14:17.156634 docmesh_agent-0.0.5/docmesh_agent/parser/output_parser.py
+-rw-r--r--   0        0        0      186 2024-05-10 11:02:39.301355 docmesh_agent-0.0.5/docmesh_agent/toolkit/__init__.py
+-rw-r--r--   0        0        0      531 2024-05-10 11:17:03.765428 docmesh_agent-0.0.5/docmesh_agent/toolkit/entity.py
+-rw-r--r--   0        0        0     1035 2024-05-16 03:38:06.823760 docmesh_agent-0.0.5/docmesh_agent/toolkit/paper.py
+-rw-r--r--   0        0        0      625 2024-05-13 03:31:55.262732 docmesh_agent-0.0.5/docmesh_agent/toolkit/recommend.py
+-rw-r--r--   0        0        0      881 2024-05-16 03:36:36.235578 docmesh_agent-0.0.5/docmesh_agent/tools/__init__.py
+-rw-r--r--   0        0        0     1104 2024-05-10 11:02:39.301355 docmesh_agent-0.0.5/docmesh_agent/tools/base.py
+-rw-r--r--   0        0        0     2304 2024-05-13 04:13:58.029801 docmesh_agent-0.0.5/docmesh_agent/tools/entity.py
+-rw-r--r--   0        0        0     3936 2024-05-13 04:13:58.033801 docmesh_agent-0.0.5/docmesh_agent/tools/graph_tools.py
+-rw-r--r--   0        0        0     8856 2024-05-16 03:35:20.727428 docmesh_agent-0.0.5/docmesh_agent/tools/paper.py
+-rw-r--r--   0        0        0     4384 2024-05-16 02:53:38.522240 docmesh_agent-0.0.5/docmesh_agent/tools/recommend.py
+-rw-r--r--   0        0        0      727 2024-05-15 11:38:47.189942 docmesh_agent-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      646 1970-01-01 00:00:00.000000 docmesh_agent-0.0.5/PKG-INFO
```

### Comparing `docmesh_agent-0.0.4/docmesh_agent/agent.py` & `docmesh_agent-0.0.5/docmesh_agent/agent.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.4/docmesh_agent/embeddings/embeddings.py` & `docmesh_agent-0.0.5/docmesh_agent/embeddings/embeddings.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.4/docmesh_agent/parser/output_parser.py` & `docmesh_agent-0.0.5/docmesh_agent/parser/output_parser.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.4/docmesh_agent/toolkit/entity.py` & `docmesh_agent-0.0.5/docmesh_agent/toolkit/entity.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.4/docmesh_agent/toolkit/paper.py` & `docmesh_agent-0.0.5/docmesh_agent/toolkit/paper.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,31 @@
 from langchain_core.tools import BaseToolkit
 
 from docmesh_agent.tools.base import BaseAgentTool
 from docmesh_agent.tools.paper import (
     AddPaperFromTitleTool,
     AddPaperFromArxivTool,
     GetPaperIdTool,
+    GetPaperPDFTool,
     MarkPaperReadTool,
+    ReadWholePDFTool,
+    ReadPartialPDFTool,
     PaperSummaryTool,
     ListLatestPaperTool,
 )
 
 
 class PaperToolkit(BaseToolkit):
     entity_name: str
 
     def get_tools(self) -> list[BaseAgentTool]:
         return [
             AddPaperFromTitleTool(entity_name=self.entity_name),
             AddPaperFromArxivTool(entity_name=self.entity_name),
             GetPaperIdTool(entity_name=self.entity_name),
+            GetPaperPDFTool(entity_name=self.entity_name),
             MarkPaperReadTool(entity_name=self.entity_name),
+            ReadWholePDFTool(entity_name=self.entity_name),
+            ReadPartialPDFTool(entity_name=self.entity_name),
             PaperSummaryTool(entity_name=self.entity_name),
             ListLatestPaperTool(entity_name=self.entity_name),
         ]
```

### Comparing `docmesh_agent-0.0.4/docmesh_agent/toolkit/recommend.py` & `docmesh_agent-0.0.5/docmesh_agent/toolkit/recommend.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.4/docmesh_agent/tools/__init__.py` & `docmesh_agent-0.0.5/docmesh_agent/tools/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,15 +3,18 @@
     ListFollowsTool,
     ListPopularEntitiesTool,
 )
 from .paper import (
     AddPaperFromTitleTool,
     AddPaperFromArxivTool,
     GetPaperIdTool,
+    GetPaperPDFTool,
     MarkPaperReadTool,
+    ReadWholePDFTool,
+    ReadPartialPDFTool,
     PaperSummaryTool,
     ListLatestPaperTool,
 )
 from .recommend import (
     UnreadFollowsTool,
     UnreadInfluentialTool,
     UnreadSimilarTool,
@@ -21,15 +24,18 @@
 __all__ = [
     "FollowEntityTool",
     "ListFollowsTool",
     "ListPopularEntitiesTool",
     "AddPaperFromTitleTool",
     "AddPaperFromArxivTool",
     "GetPaperIdTool",
+    "GetPaperPDFTool",
     "MarkPaperReadTool",
+    "ReadWholePDFTool",
+    "ReadPartialPDFTool",
     "PaperSummaryTool",
     "ListLatestPaperTool",
     "UnreadFollowsTool",
     "UnreadInfluentialTool",
     "UnreadSimilarTool",
     "UnreadSemanticTool",
 ]
```

### Comparing `docmesh_agent-0.0.4/docmesh_agent/tools/base.py` & `docmesh_agent-0.0.5/docmesh_agent/tools/base.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.4/docmesh_agent/tools/entity.py` & `docmesh_agent-0.0.5/docmesh_agent/tools/entity.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.4/docmesh_agent/tools/graph_tools.py` & `docmesh_agent-0.0.5/docmesh_agent/tools/graph_tools.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.4/docmesh_agent/tools/recommend.py` & `docmesh_agent-0.0.5/docmesh_agent/tools/recommend.py`

 * *Files identical despite different names*

### Comparing `docmesh_agent-0.0.4/PKG-INFO` & `docmesh_agent-0.0.5/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 Metadata-Version: 2.1
 Name: docmesh_agent
-Version: 0.0.4
+Version: 0.0.5
 Summary: Agent helps you dig the paper connection!
 Author-email: Zhengkai Yang <kyle.yang1995@gmail.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Operating System :: OS Independent
-Requires-Dist: docmesh_core>=0.0.2
+Requires-Dist: docmesh-core>=0.0.2
+Requires-Dist: pymupdf>=1.24.3
+Requires-Dist: faiss-cpu>=1.8.0
 Requires-Dist: langchain>=0.1.15
 Requires-Dist: langchain-openai>=0.1.3
 Requires-Dist: langchainhub>=0.1.15
 
 # docmesh agent
```

