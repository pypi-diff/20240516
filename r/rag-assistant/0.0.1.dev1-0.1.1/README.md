# Comparing `tmp/rag_assistant-0.0.1.dev1.tar.gz` & `tmp/rag_assistant-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rag_assistant-0.0.1.dev1.tar", last modified: Wed May 15 21:29:02 2024, max compression
+gzip compressed data, was "rag_assistant-0.1.1.tar", last modified: Wed May 15 21:43:26 2024, max compression
```

## Comparing `rag_assistant-0.0.1.dev1.tar` & `rag_assistant-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:29:02.404209 rag_assistant-0.0.1.dev1/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-15 21:29:02.404209 rag_assistant-0.0.1.dev1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 21:28:51.000000 rag_assistant-0.0.1.dev1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:29:02.404209 rag_assistant-0.0.1.dev1/rag_assistant/
--rw-r--r--   0 runner    (1001) docker     (127)    20792 2024-05-15 21:28:51.000000 rag_assistant-0.0.1.dev1/rag_assistant/RagAssistant.py
--rw-r--r--   0 runner    (1001) docker     (127)      204 2024-05-15 21:28:51.000000 rag_assistant-0.0.1.dev1/rag_assistant/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:29:02.404209 rag_assistant-0.0.1.dev1/rag_assistant.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      535 2024-05-15 21:29:02.000000 rag_assistant-0.0.1.dev1/rag_assistant.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-15 21:29:02.000000 rag_assistant-0.0.1.dev1/rag_assistant.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 21:29:02.000000 rag_assistant-0.0.1.dev1/rag_assistant.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 21:29:02.000000 rag_assistant-0.0.1.dev1/rag_assistant.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       25 2024-05-15 21:29:02.000000 rag_assistant-0.0.1.dev1/rag_assistant.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 21:29:02.000000 rag_assistant-0.0.1.dev1/rag_assistant.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:29:02.404209 rag_assistant-0.0.1.dev1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      879 2024-05-15 21:28:51.000000 rag_assistant-0.0.1.dev1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:43:26.087994 rag_assistant-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-15 21:43:26.087994 rag_assistant-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 21:43:15.000000 rag_assistant-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:43:26.087994 rag_assistant-0.1.1/rag_assistant/
+-rw-r--r--   0 runner    (1001) docker     (127)    18763 2024-05-15 21:43:15.000000 rag_assistant-0.1.1/rag_assistant/RagAssistant.py
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-15 21:43:15.000000 rag_assistant-0.1.1/rag_assistant/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 21:43:26.087994 rag_assistant-0.1.1/rag_assistant.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      552 2024-05-15 21:43:26.000000 rag_assistant-0.1.1/rag_assistant.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      298 2024-05-15 21:43:26.000000 rag_assistant-0.1.1/rag_assistant.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 21:43:26.000000 rag_assistant-0.1.1/rag_assistant.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-05-15 21:43:26.000000 rag_assistant-0.1.1/rag_assistant.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-05-15 21:43:26.000000 rag_assistant-0.1.1/rag_assistant.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-05-15 21:43:26.000000 rag_assistant-0.1.1/rag_assistant.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 21:43:26.087994 rag_assistant-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      897 2024-05-15 21:43:15.000000 rag_assistant-0.1.1/setup.py
```

### Comparing `rag_assistant-0.0.1.dev1/PKG-INFO` & `rag_assistant-0.1.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: rag_assistant
-Version: 0.0.1.dev1
+Version: 0.1.1
 Summary: The Swarmauri Rag Assistant is part of the swarmaURI framework.
 Home-page: http://github.com/swarmauri/rag_assistant
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Requires-Dist: gradio
 Requires-Dist: swarmauri[full]==0.1.127
 
 # Swarmauri Rag Assistant
 
 ## Overview
 The Swarmauri Rag Assistant
```

### Comparing `rag_assistant-0.0.1.dev1/rag_assistant/RagAssistant.py` & `rag_assistant-0.1.1/rag_assistant/RagAssistant.py`

 * *Files 15% similar despite different names*

```diff
@@ -22,17 +22,14 @@
 from swarmauri.standard.documents.concrete.Document import Document
 from swarmauri.standard.documents.concrete.EmbeddedDocument import EmbeddedDocument
 from swarmauri.standard.messages.concrete import (HumanMessage, 
                                                   SystemMessage,
                                                   AgentMessage)
 from swarmauri.standard.utils.load_documents_from_json import load_documents_from_json_file
 
-#head="""<link rel="icon" href="data:image/png;base64,iVBORw0KGgoAAAANSUhEUgAAACAAAAAgCAYAAABzenr0AAAAAXNSR0IArs4c6QAABWFJREFUWEe1V2tsFFUU/s7M7KO77Ra2LRisUArasLjbLqVdaRfQkACCNISgUQJCiCHGfyaYEIMSfIQY/K3GEAUkqNHwUJ6JEoht7ZZuu92uaCktILUJpSy0233PzNU7SClNu9MWvX8ms+ec7/vOuefMvUsYxypxu2dYgHRLS8utcbhjrttdIMJiaG+p69HzJz0Hl8dTKMLYwRiIMeW11ov1hzLFlFZUbSQS93EfNZGaGwz6ujP56wpwOCoeM2abrhOREUBCluXKNv+vbaOBOssXOSVJagRgZgxJOZaaFQr5bj6SAB7sqvS+KoA+J4KJqawucLHWOxpoWaW3joiqOLmqsm3BptqDehXWrcB9gPlub6lkwGcEeAC8xxgjgmDhdgY1xp9E9A7AGmRZfj3U7AvqkWsx43G67+NaWLVeFMVvAIhjxCmKorwcbKr/fry4ExJQ5vFeI9CsTOCMsauBxtri/1yAy+WyCmZbhIgyimaMsd7ueHZPj1/bFr01gQqUG9yerBhAUmZQJrfIcQv8/rQe+YR7oKzS20ZET+tsQSjQWOscD7muAN7p5wOBXAuZp0GQ8g4fPrgjMhCpUWQZ4XAYf3Xf+8Y8XlgIu90OUZJgs9mOv7Jh00dGSehTTOgtLy4eICI2liBtC862tlrzJOtWEK0gYDZAFkbMAgYbANPwaWGMIRpPIJVKI3zrpjZH9vzpMBoNsGaZ+SgO5+LESRAGiFEMYDEGXCWiM32pyJcrSkuj1NDaUSgahJ8JeCpT2RRFwZ2BCG6F7yIWT2iuT0yza88bvWHtackyo8A+BVNtORDFsSZ1iKU9lZKXUdOlK98C9NJo5IqiIhKNItw/gP7IIFT1XiVzrBZMy5uKntbvtIxnuF7EzdthRKL3Gl8QCLk52bDn2pCTbYUoCKPmxsC+oabfO/t5qXlpeZaxRBLRWFwDG4zFwX/nyyBJGmC+PRdmkwn1F85i3ewTmu3otTVYtGQ5Eskk+sL9muC0LGs2LjDbmoUciwXZlixkmU1adbStYrhLvlBH/HLXdXMilYaqqg8pNRoMyM2xYootR8uaB3FBZ06dgDfvDJ51GTT/88E06u+swvKVq4Z8eAJ3ByLoj0SRSj88kYIgwGw0oGROUYIaQx117V1/VimqAk5oNhm1veSE/H14U8XjcXy1fz8W5Aewrpr35oN1pC6JQNiNjZu3wGw2Dxm4YC4gMhhDLJFAIpnS3kVBREnxrHpq/qOrRlXZsUznAgf5LRTCoQMHcPt2X6ZeRX5BATZt3oJ5DsfIiRgZx5iqrtVmpulS5xsA7QWYdroNX52dV3Dyhx/RFmzNSDzS6Corwws1NSgqmj2aEN6t2xc65nw6NLQNbV3TRUFdCyInAWZFUbs+2L3r3e4bNx6u9YRkADNnFiV37t71PhgVCwL/FqAtLUePP+N0aheVjGfB1g1L/YudxgXi6FOkK0VRgV+CqZYvvr6wYCznjAKSDav3GiVhuy5TBgdZVT82VJ58a1ICButWlVlNQjOf5smJYCwWVcqtS0+3TEoAD0o1rD5nkITnJiNAVtg5g+fEskyxupm5K6sXgoSGDNewsfAVQsrT7PP5H0kADy6tqN4jCMKOiVRBYezDYGPtTr0Y3Qr8CyCWVniPCgKt0QPkdsbYsUBj7XoAip7/eAXA4XAYXfMK9lU8KW1kY9wLiTHm75APtF8b3Ob/P65kPJven55fb7MIu0xGmv9gOhhLy2iLJtnuqUtPHtHLerh93BUYCdp1emXJJ8eS5xlAb9ZkLSlcferyRIjv+05aAAco8yz28UM94Kvl/5YmtR5JgKuy+m0wsODFuj2TYv8n6G+wcRzTJW9piwAAAABJRU5ErkJggg==" type="image/png">"""
-head=""
-
 class RagAssistant:
     def __init__(self, 
                  api_key: str = "", 
                  system_context: str = "You are a helpful assistant.",
                  model_name = "openai_gpt-4o",
                  db_path='prompt_responses.db'):
         print('Initializing... this will take a moment.')
@@ -343,15 +340,15 @@
             with gr.Row():
                 self.save_button = gr.Button("save")
                 
             self.vectorizer.change(self.change_vectorizer, inputs=[self.vectorizer], outputs=self.data_frame)
             self.load_button.click(self.load_and_filter_json, inputs=[self.file], outputs=self.data_frame)
             self.save_button.click(self.save_df, inputs=[self.data_frame])
 
-        with gr.Blocks(css = self.css, title="Swarmauri Rag Agent", head=head) as self.app:
+        with gr.Blocks(css = self.css, title="Swarmauri Rag Agent") as self.app:
             gr.TabbedInterface(interface_list=[self.chat, self.retrieval_table, self.document_table], 
                                       tab_names=["chat", "retrieval", "documents"])
 
     
     def launch(self, share: bool = False, server_name: Optional[str] = None, favicon_path: Optional[str] = None):
         kwargs = {}
         kwargs.update({'share': share})
```

### Comparing `rag_assistant-0.0.1.dev1/rag_assistant.egg-info/PKG-INFO` & `rag_assistant-0.1.1/rag_assistant.egg-info/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: rag_assistant
-Version: 0.0.1.dev1
+Version: 0.1.1
 Summary: The Swarmauri Rag Assistant is part of the swarmaURI framework.
 Home-page: http://github.com/swarmauri/rag_assistant
 Author: Jacob Stewart
 Author-email: corporate@swarmauri.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
+Requires-Dist: gradio
 Requires-Dist: swarmauri[full]==0.1.127
 
 # Swarmauri Rag Assistant
 
 ## Overview
 The Swarmauri Rag Assistant
```

### Comparing `rag_assistant-0.0.1.dev1/setup.py` & `rag_assistant-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,15 +14,16 @@
     packages=find_packages(include=['rag_assistant']),
     entry_points={
         'console_scripts': [
             'rag_assistant = rag_assistant.RagAssistant:main',
         ]
     },
     include_package_data=True,
-    install_requires=['swarmauri[full]==0.1.127'],
+    install_requires=['gradio',
+        'swarmauri[full]==0.1.127'],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3.10'
     ],
     python_requires='>=3.10',
     setup_requires=["wheel"]
 )
```

