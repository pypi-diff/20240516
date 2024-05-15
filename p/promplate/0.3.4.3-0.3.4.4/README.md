# Comparing `tmp/promplate-0.3.4.3.tar.gz` & `tmp/promplate-0.3.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "promplate-0.3.4.3.tar", max compression
+gzip compressed data, was "promplate-0.3.4.4.tar", max compression
```

## Comparing `promplate-0.3.4.3.tar` & `promplate-0.3.4.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0       45 2023-12-07 20:31:43.859313 promplate-0.3.4.3/promplate/__init__.py
--rw-r--r--   0        0        0      103 2024-02-05 14:52:39.251073 promplate-0.3.4.3/promplate/chain/__init__.py
--rw-r--r--   0        0        0     2309 2024-04-26 17:31:42.113544 promplate-0.3.4.3/promplate/chain/callback.py
--rw-r--r--   0        0        0    17376 2024-04-26 17:32:20.940322 promplate-0.3.4.3/promplate/chain/node.py
--rw-r--r--   0        0        0     1308 2024-04-18 10:26:42.315669 promplate-0.3.4.3/promplate/chain/utils.py
--rw-r--r--   0        0        0        0 2023-11-23 14:05:02.473815 promplate-0.3.4.3/promplate/llm/__init__.py
--rw-r--r--   0        0        0     1043 2024-04-18 10:26:42.319797 promplate-0.3.4.3/promplate/llm/base.py
--rw-r--r--   0        0        0      120 2023-12-17 20:48:44.211258 promplate-0.3.4.3/promplate/llm/openai/__init__.py
--rw-r--r--   0        0        0     4125 2024-04-18 10:26:42.326058 promplate-0.3.4.3/promplate/llm/openai/v0.py
--rw-r--r--   0        0        0     6002 2024-04-20 08:19:12.536648 promplate-0.3.4.3/promplate/llm/openai/v1.py
--rw-r--r--   0        0        0       87 2024-04-06 09:45:04.214579 promplate-0.3.4.3/promplate/prompt/__init__.py
--rw-r--r--   0        0        0     1633 2024-04-15 04:14:57.538290 promplate-0.3.4.3/promplate/prompt/builder.py
--rw-r--r--   0        0        0     3216 2024-04-26 17:31:42.143848 promplate-0.3.4.3/promplate/prompt/chat.py
--rw-r--r--   0        0        0     7400 2024-04-26 18:29:57.045553 promplate-0.3.4.3/promplate/prompt/template.py
--rw-r--r--   0        0        0     3285 2024-04-26 18:50:10.020121 promplate-0.3.4.3/promplate/prompt/utils.py
--rw-r--r--   0        0        0     1600 2024-04-26 18:53:42.104877 promplate-0.3.4.3/pyproject.toml
--rw-r--r--   0        0        0     1995 2024-04-15 04:14:57.536290 promplate-0.3.4.3/README.md
--rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 promplate-0.3.4.3/PKG-INFO
+-rw-r--r--   0        0        0       45 2023-12-07 20:31:43.859313 promplate-0.3.4.4/promplate/__init__.py
+-rw-r--r--   0        0        0      103 2024-02-05 14:52:39.251073 promplate-0.3.4.4/promplate/chain/__init__.py
+-rw-r--r--   0        0        0     2309 2024-04-26 17:31:42.113544 promplate-0.3.4.4/promplate/chain/callback.py
+-rw-r--r--   0        0        0    17376 2024-04-26 17:32:20.940322 promplate-0.3.4.4/promplate/chain/node.py
+-rw-r--r--   0        0        0     1308 2024-04-18 10:26:42.315669 promplate-0.3.4.4/promplate/chain/utils.py
+-rw-r--r--   0        0        0        0 2023-11-23 14:05:02.473815 promplate-0.3.4.4/promplate/llm/__init__.py
+-rw-r--r--   0        0        0     1043 2024-04-18 10:26:42.319797 promplate-0.3.4.4/promplate/llm/base.py
+-rw-r--r--   0        0        0      120 2023-12-17 20:48:44.211258 promplate-0.3.4.4/promplate/llm/openai/__init__.py
+-rw-r--r--   0        0        0     4125 2024-04-18 10:26:42.326058 promplate-0.3.4.4/promplate/llm/openai/v0.py
+-rw-r--r--   0        0        0     6002 2024-04-20 08:19:12.536648 promplate-0.3.4.4/promplate/llm/openai/v1.py
+-rw-r--r--   0        0        0       87 2024-04-06 09:45:04.214579 promplate-0.3.4.4/promplate/prompt/__init__.py
+-rw-r--r--   0        0        0     1633 2024-04-15 04:14:57.538290 promplate-0.3.4.4/promplate/prompt/builder.py
+-rw-r--r--   0        0        0     3216 2024-04-26 17:31:42.143848 promplate-0.3.4.4/promplate/prompt/chat.py
+-rw-r--r--   0        0        0     7362 2024-04-26 19:15:34.918440 promplate-0.3.4.4/promplate/prompt/template.py
+-rw-r--r--   0        0        0     3285 2024-04-26 18:50:10.020121 promplate-0.3.4.4/promplate/prompt/utils.py
+-rw-r--r--   0        0        0     1600 2024-04-26 19:15:52.361070 promplate-0.3.4.4/pyproject.toml
+-rw-r--r--   0        0        0     1995 2024-04-15 04:14:57.536290 promplate-0.3.4.4/README.md
+-rw-r--r--   0        0        0     3212 1970-01-01 00:00:00.000000 promplate-0.3.4.4/PKG-INFO
```

### Comparing `promplate-0.3.4.3/promplate/chain/callback.py` & `promplate-0.3.4.4/promplate/chain/callback.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.3/promplate/chain/node.py` & `promplate-0.3.4.4/promplate/chain/node.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.3/promplate/chain/utils.py` & `promplate-0.3.4.4/promplate/chain/utils.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.3/promplate/llm/base.py` & `promplate-0.3.4.4/promplate/llm/base.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.3/promplate/llm/openai/v0.py` & `promplate-0.3.4.4/promplate/llm/openai/v0.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.3/promplate/llm/openai/v1.py` & `promplate-0.3.4.4/promplate/llm/openai/v1.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.3/promplate/prompt/builder.py` & `promplate-0.3.4.4/promplate/prompt/builder.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.3/promplate/prompt/chat.py` & `promplate-0.3.4.4/promplate/prompt/chat.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.3/promplate/prompt/template.py` & `promplate-0.3.4.4/promplate/prompt/template.py`

 * *Files 0% similar despite different names*

```diff
@@ -92,15 +92,14 @@
     def compile(self, sync=True, indent_str="\t"):
         self._buffer = []
         self._ops_stack = []
         self._builder = get_base_builder(sync, indent_str)
 
         for token in split_template_tokens(self.text):
             if not token:
-                print(f"{token = }")
                 continue
             s_token = token.strip()
             if s_token.startswith("{{") and s_token.endswith("}}"):
                 self._on_eval_token(token)
             elif s_token.startswith("{#") and s_token.endswith("#}"):
                 self._on_exec_token(token)
             elif s_token.startswith("{%") and s_token.endswith("%}") and "\n" not in s_token:
```

### Comparing `promplate-0.3.4.3/promplate/prompt/utils.py` & `promplate-0.3.4.4/promplate/prompt/utils.py`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.3/pyproject.toml` & `promplate-0.3.4.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "promplate"
-version = "0.3.4.3"
+version = "0.3.4.4"
 description = "Prompt engineering framework for humans"
 homepage = "https://promplate.dev/"
 documentation = "https://docs.py.promplate.dev/"
 repository = "https://github.com/promplate/core"
 authors = ["Muspi Merol <me@promplate.dev>"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `promplate-0.3.4.3/README.md` & `promplate-0.3.4.4/README.md`

 * *Files identical despite different names*

### Comparing `promplate-0.3.4.3/PKG-INFO` & `promplate-0.3.4.4/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: promplate
-Version: 0.3.4.3
+Version: 0.3.4.4
 Summary: Prompt engineering framework for humans
 Home-page: https://promplate.dev/
 License: MIT
 Keywords: prompt,template,nlp,llm
 Author: Muspi Merol
 Author-email: me@promplate.dev
 Requires-Python: >=3.10,<4.0
```

