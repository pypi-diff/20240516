# Comparing `tmp/streamlit_octostar_utils-0.0.3.tar.gz` & `tmp/streamlit_octostar_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "streamlit_octostar_utils-0.0.3.tar", max compression
+gzip compressed data, was "streamlit_octostar_utils-0.0.4.tar", max compression
```

## Comparing `streamlit_octostar_utils-0.0.3.tar` & `streamlit_octostar_utils-0.0.4.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     1073 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/LICENSE
--rw-r--r--   0        0        0      324 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/README.md
--rw-r--r--   0        0        0      741 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/pyproject.toml
--rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/__init__.py
--rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/api_crafter/__init__.py
--rw-r--r--   0        0        0     4996 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/api_crafter/fastapi.py
--rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/core/__init__.py
--rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/core/threading/__init__.py
--rw-r--r--   0        0        0     2224 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/core/threading/key_queue.py
--rw-r--r--   0        0        0       68 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/hello.py
--rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/octostar/__init__.py
--rw-r--r--   0        0        0     1690 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/octostar/client.py
--rw-r--r--   0        0        0      210 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/octostar/context.py
--rw-r--r--   0        0        0     1149 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/octostar/permissions.py
--rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/ontology/__init__.py
--rw-r--r--   0        0        0      137 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/ontology/inheritance.py
--rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/style/__init__.py
--rw-r--r--   0        0        0      605 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/style/common.py
--rw-r--r--   0        0        0        1 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/threading/__init__.py
--rw-r--r--   0        0        0     4591 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/threading/async_task_manager.py
--rw-r--r--   0        0        0     4001 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/threading/session_callback_manager.py
--rw-r--r--   0        0        0      809 2024-05-09 16:24:25.699144 streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/threading/session_state_hot_swapper.py
--rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 streamlit_octostar_utils-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-05-16 12:16:15.594064 streamlit_octostar_utils-0.0.4/LICENSE
+-rw-r--r--   0        0        0      324 2024-05-16 12:16:15.594064 streamlit_octostar_utils-0.0.4/README.md
+-rw-r--r--   0        0        0      741 2024-05-16 12:16:15.594064 streamlit_octostar_utils-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0        1 2024-05-16 12:16:15.594064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-16 12:16:15.594064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/api_crafter/__init__.py
+-rw-r--r--   0        0        0     4996 2024-05-16 12:16:15.594064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/api_crafter/fastapi.py
+-rw-r--r--   0        0        0        1 2024-05-16 12:16:15.594064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/core/__init__.py
+-rw-r--r--   0        0        0        1 2024-05-16 12:16:15.594064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/core/threading/__init__.py
+-rw-r--r--   0        0        0     2224 2024-05-16 12:16:15.598064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/core/threading/key_queue.py
+-rw-r--r--   0        0        0       68 2024-05-16 12:16:15.598064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/hello.py
+-rw-r--r--   0        0        0        1 2024-05-16 12:16:15.598064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/octostar/__init__.py
+-rw-r--r--   0        0        0     1690 2024-05-16 12:16:15.598064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/octostar/client.py
+-rw-r--r--   0        0        0      210 2024-05-16 12:16:15.598064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/octostar/context.py
+-rw-r--r--   0        0        0     1149 2024-05-16 12:16:15.598064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/octostar/permissions.py
+-rw-r--r--   0        0        0        1 2024-05-16 12:16:15.598064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/ontology/__init__.py
+-rw-r--r--   0        0        0      137 2024-05-16 12:16:15.598064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/ontology/inheritance.py
+-rw-r--r--   0        0        0        1 2024-05-16 12:16:15.598064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/style/__init__.py
+-rw-r--r--   0        0        0     1492 2024-05-16 12:16:15.598064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/style/common.py
+-rw-r--r--   0        0        0        1 2024-05-16 12:16:15.598064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/threading/__init__.py
+-rw-r--r--   0        0        0     4591 2024-05-16 12:16:15.598064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/threading/async_task_manager.py
+-rw-r--r--   0        0        0     3757 2024-05-16 12:16:15.598064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/threading/session_callback_manager.py
+-rw-r--r--   0        0        0      809 2024-05-16 12:16:15.598064 streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/threading/session_state_hot_swapper.py
+-rw-r--r--   0        0        0      978 1970-01-01 00:00:00.000000 streamlit_octostar_utils-0.0.4/PKG-INFO
```

### Comparing `streamlit_octostar_utils-0.0.3/LICENSE` & `streamlit_octostar_utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `streamlit_octostar_utils-0.0.3/pyproject.toml` & `streamlit_octostar_utils-0.0.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "streamlit-octostar-utils"
-version = "0.0.3"
+version = "0.0.4"
 description = ""
 license = "MIT"
 authors = ["Valerio Tonelli <tonellivalerio97@gmail.com>"]
 readme = "README.md"
 include = [
     "streamlit-octostar-utils/**/*"
 ]
```

### Comparing `streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/api_crafter/fastapi.py` & `streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/api_crafter/fastapi.py`

 * *Files identical despite different names*

### Comparing `streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/core/threading/key_queue.py` & `streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/core/threading/key_queue.py`

 * *Files identical despite different names*

### Comparing `streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/octostar/client.py` & `streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/octostar/client.py`

 * *Files identical despite different names*

### Comparing `streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/octostar/permissions.py` & `streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/octostar/permissions.py`

 * *Files identical despite different names*

### Comparing `streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/threading/async_task_manager.py` & `streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/threading/async_task_manager.py`

 * *Files identical despite different names*

### Comparing `streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/threading/session_callback_manager.py` & `streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/threading/session_callback_manager.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,18 +30,15 @@
         return SessionCallbackManager.instance
 
     def heartbeat(self):
         inactive_sessions = []
         for session_id, session_info in list(self.active_sessions.items()):
             if session_info['runtime'].is_active_session(session_id=session_info['context'].session_id):
                 heartbeat_fn = session_info.get('on_heartbeat')
-                heartbeat_fn(
-                    session_info['session_id'],
-                    session_info['context']
-                )
+                heartbeat_fn(session_info['context'])
             else:
                 inactive_sessions.append(session_id)
         for session_id in inactive_sessions:
             self.on_session_end(session_id)
 
     def monitoring_thread(self):
         while self.monitoring_thread_active:
@@ -68,28 +65,26 @@
             self.active_sessions[session_id]['on_session_start'] = SessionCallbackManager.callback_wrapper(on_session_start)
             self.active_sessions[session_id]['on_heartbeat'] = SessionCallbackManager.callback_wrapper(on_heartbeat)
             self.active_sessions[session_id]['on_session_end'] = SessionCallbackManager.callback_wrapper(on_session_end)
         self.on_session_start(session_id)
         return session_id
     
     def callback_wrapper(callback_fn):
-        def _callback(session_id, st_context):
+        def _callback(st_context):
             if callback_fn:
                 with SessionStateHotSwapper(st_context):
-                    callback_fn(session_id)
+                    callback_fn()
         return _callback
     
     def on_session_start(self, session_id):
         start_fn = self.active_sessions[session_id].get('on_session_start')
-        start_fn(self.active_sessions[session_id]['session_id'],
-                 self.active_sessions[session_id]['context'])
+        start_fn(self.active_sessions[session_id]['context'])
         self.start_monitoring()
 
     def on_session_end(self, session_id):
         with self.monitoring_thread_lock:
             if session_id in self.active_sessions:
                 end_fn = self.active_sessions[session_id].get('on_session_end')
-                end_fn(self.active_sessions[session_id]['session_id'],
-                       self.active_sessions[session_id]['context'])
+                end_fn(self.active_sessions[session_id]['context'])
                 self.active_sessions.pop(session_id, None)
                 if not self.active_sessions:
                     self.monitoring_thread_active = False
```

### Comparing `streamlit_octostar_utils-0.0.3/streamlit_octostar_utils/threading/session_state_hot_swapper.py` & `streamlit_octostar_utils-0.0.4/streamlit_octostar_utils/threading/session_state_hot_swapper.py`

 * *Files identical despite different names*

### Comparing `streamlit_octostar_utils-0.0.3/PKG-INFO` & `streamlit_octostar_utils-0.0.4/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: streamlit-octostar-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: 
 License: MIT
 Author: Valerio Tonelli
 Author-email: tonellivalerio97@gmail.com
 Requires-Python: >=3.9, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*, !=3.8.*
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

