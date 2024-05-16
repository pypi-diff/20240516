# Comparing `tmp/answerrocket_client-0.2.2.tar.gz` & `tmp/answerrocket_client-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "answerrocket_client-0.2.2.tar", last modified: Thu May  9 15:53:20 2024, max compression
+gzip compressed data, was "answerrocket_client-0.2.3.tar", last modified: Wed May 15 18:48:45 2024, max compression
```

## Comparing `answerrocket_client-0.2.2.tar` & `answerrocket_client-0.2.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:20.716432 answerrocket_client-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-09 15:53:20.716432 answerrocket_client-0.2.2/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:20.712432 answerrocket_client-0.2.2/answer_rocket/
--rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/answer_rocket/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/answer_rocket/auth.py
--rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/answer_rocket/chat.py
--rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/answer_rocket/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    13046 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/answer_rocket/config.py
--rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/answer_rocket/data.py
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/answer_rocket/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:20.712432 answerrocket_client-0.2.2/answer_rocket/graphql/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/answer_rocket/graphql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/answer_rocket/graphql/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    46982 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/answer_rocket/graphql/schema.py
--rw-r--r--   0 runner    (1001) docker     (127)     4597 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/answer_rocket/graphql/sdk_operations.py
--rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/answer_rocket/output.py
--rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/answer_rocket/skill.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/answer_rocket/types.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:20.712432 answerrocket_client-0.2.2/answerrocket_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-09 15:53:20.000000 answerrocket_client-0.2.2/answerrocket_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-09 15:53:20.000000 answerrocket_client-0.2.2/answerrocket_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-09 15:53:20.000000 answerrocket_client-0.2.2/answerrocket_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-09 15:53:20.000000 answerrocket_client-0.2.2/answerrocket_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-09 15:53:20.000000 answerrocket_client-0.2.2/answerrocket_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/readme.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-09 15:53:20.716432 answerrocket_client-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-09 15:53:20.712432 answerrocket_client-0.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-09 15:53:16.000000 answerrocket_client-0.2.2/test/test_client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:48:45.992315 answerrocket_client-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-15 18:48:45.992315 answerrocket_client-0.2.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:48:45.988315 answerrocket_client-0.2.3/answer_rocket/
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/answer_rocket/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1418 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/answer_rocket/auth.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16137 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/answer_rocket/chat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1469 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/answer_rocket/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13046 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/answer_rocket/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18507 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/answer_rocket/data.py
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/answer_rocket/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:48:45.988315 answerrocket_client-0.2.3/answer_rocket/graphql/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/answer_rocket/graphql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1107 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/answer_rocket/graphql/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    46982 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/answer_rocket/graphql/schema.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4747 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/answer_rocket/graphql/sdk_operations.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7170 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/answer_rocket/output.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2663 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/answer_rocket/skill.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/answer_rocket/types.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:48:45.992315 answerrocket_client-0.2.3/answerrocket_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3907 2024-05-15 18:48:45.000000 answerrocket_client-0.2.3/answerrocket_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      629 2024-05-15 18:48:45.000000 answerrocket_client-0.2.3/answerrocket_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 18:48:45.000000 answerrocket_client-0.2.3/answerrocket_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       60 2024-05-15 18:48:45.000000 answerrocket_client-0.2.3/answerrocket_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 18:48:45.000000 answerrocket_client-0.2.3/answerrocket_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      488 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     3543 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/readme.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 18:48:45.992315 answerrocket_client-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 18:48:45.992315 answerrocket_client-0.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      471 2024-05-15 18:48:27.000000 answerrocket_client-0.2.3/test/test_client.py
```

### Comparing `answerrocket_client-0.2.2/PKG-INFO` & `answerrocket_client-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
```

### Comparing `answerrocket_client-0.2.2/answer_rocket/auth.py` & `answerrocket_client-0.2.3/answer_rocket/auth.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.2/answer_rocket/chat.py` & `answerrocket_client-0.2.3/answer_rocket/chat.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.2/answer_rocket/client.py` & `answerrocket_client-0.2.3/answer_rocket/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.2/answer_rocket/config.py` & `answerrocket_client-0.2.3/answer_rocket/config.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.2/answer_rocket/data.py` & `answerrocket_client-0.2.3/answer_rocket/data.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.2/answer_rocket/graphql/client.py` & `answerrocket_client-0.2.3/answer_rocket/graphql/client.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.2/answer_rocket/graphql/schema.py` & `answerrocket_client-0.2.3/answer_rocket/graphql/schema.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.2/answer_rocket/graphql/sdk_operations.py` & `answerrocket_client-0.2.3/answer_rocket/graphql/sdk_operations.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,15 +89,18 @@
     _op = sgqlc.operation.Operation(_schema_root.query_type, name='ChatThread', variables=dict(id=sgqlc.types.Arg(sgqlc.types.non_null(_schema.UUID))))
     _op_chat_thread = _op.chat_thread(id=sgqlc.types.Variable('id'))
     _op_chat_thread.id()
     _op_chat_thread.entry_count()
     _op_chat_thread.title()
     _op_chat_thread.copilot_id()
     _op_chat_thread_entries = _op_chat_thread.entries()
-    _op_chat_thread_entries.__fragment__(fragment_chat_result_fragment())
+    _op_chat_thread_entries.id()
+    _op_chat_thread_entries.thread_id()
+    _op_chat_thread_entries_answer = _op_chat_thread_entries.answer()
+    _op_chat_thread_entries_answer.__fragment__(fragment_chat_result_fragment())
     return _op
 
 
 class Query:
     chat_entry = query_chat_entry()
     chat_thread = query_chat_thread()
```

### Comparing `answerrocket_client-0.2.2/answer_rocket/output.py` & `answerrocket_client-0.2.3/answer_rocket/output.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.2/answer_rocket/skill.py` & `answerrocket_client-0.2.3/answer_rocket/skill.py`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.2/answerrocket_client.egg-info/PKG-INFO` & `answerrocket_client-0.2.3/answerrocket_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: answerrocket-client
-Version: 0.2.2
+Version: 0.2.3
 Summary: Python client for interacting with AnswerRocket's skill API
 Requires-Python: >=3.10.7
 Description-Content-Type: text/markdown
 Requires-Dist: sgqlc
 Requires-Dist: openai
 Requires-Dist: pandas>=1.5.1
 Requires-Dist: typing-extensions
```

### Comparing `answerrocket_client-0.2.2/answerrocket_client.egg-info/SOURCES.txt` & `answerrocket_client-0.2.3/answerrocket_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `answerrocket_client-0.2.2/readme.md` & `answerrocket_client-0.2.3/readme.md`

 * *Files identical despite different names*

