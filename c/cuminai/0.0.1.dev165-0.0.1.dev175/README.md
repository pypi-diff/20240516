# Comparing `tmp/cuminai-0.0.1.dev165.tar.gz` & `tmp/cuminai-0.0.1.dev175.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cuminai-0.0.1.dev165.tar", max compression
+gzip compressed data, was "cuminai-0.0.1.dev175.tar", max compression
```

## Comparing `cuminai-0.0.1.dev165.tar` & `cuminai-0.0.1.dev175.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       75 2024-05-12 07:46:46.527637 cuminai-0.0.1.dev165/cuminai/__init__.py
--rw-r--r--   0        0        0      691 2024-05-15 18:12:16.655249 cuminai-0.0.1.dev165/cuminai/constants.py
--rw-r--r--   0        0        0     2466 2024-05-15 10:54:39.551320 cuminai-0.0.1.dev165/cuminai/contextstores.py
--rw-r--r--   0        0        0    12061 2024-05-16 05:54:42.498882 cuminai-0.0.1.dev165/cuminai/creator.py
--rw-r--r--   0        0        0      520 2024-05-15 10:40:50.032155 cuminai-0.0.1.dev165/cuminai/validator.py
--rw-r--r--   0        0        0    11558 2024-05-11 18:16:30.219425 cuminai-0.0.1.dev165/LICENSE
--rw-r--r--   0        0        0      569 2024-05-16 05:51:20.992730 cuminai-0.0.1.dev165/pyproject.toml
--rw-r--r--   0        0        0     1350 2024-05-16 05:53:31.413774 cuminai-0.0.1.dev165/README.md
--rw-r--r--   0        0        0     2036 1970-01-01 00:00:00.000000 cuminai-0.0.1.dev165/PKG-INFO
+-rw-r--r--   0        0        0       75 2024-05-12 07:46:46.527637 cuminai-0.0.1.dev175/cuminai/__init__.py
+-rw-r--r--   0        0        0      691 2024-05-15 18:12:16.655249 cuminai-0.0.1.dev175/cuminai/constants.py
+-rw-r--r--   0        0        0     2466 2024-05-15 10:54:39.551320 cuminai-0.0.1.dev175/cuminai/contextstores.py
+-rw-r--r--   0        0        0    12718 2024-05-16 19:49:15.267475 cuminai-0.0.1.dev175/cuminai/creator.py
+-rw-r--r--   0        0        0      575 2024-05-16 19:30:39.564649 cuminai-0.0.1.dev175/cuminai/validator.py
+-rw-r--r--   0        0        0    11558 2024-05-11 18:16:30.219425 cuminai-0.0.1.dev175/LICENSE
+-rw-r--r--   0        0        0      569 2024-05-16 19:34:50.032171 cuminai-0.0.1.dev175/pyproject.toml
+-rw-r--r--   0        0        0     3135 2024-05-16 19:58:36.161593 cuminai-0.0.1.dev175/README.md
+-rw-r--r--   0        0        0     3754 1970-01-01 00:00:00.000000 cuminai-0.0.1.dev175/PKG-INFO
```

### Comparing `cuminai-0.0.1.dev165/cuminai/constants.py` & `cuminai-0.0.1.dev175/cuminai/constants.py`

 * *Files identical despite different names*

### Comparing `cuminai-0.0.1.dev165/cuminai/contextstores.py` & `cuminai-0.0.1.dev175/cuminai/contextstores.py`

 * *Files identical despite different names*

### Comparing `cuminai-0.0.1.dev165/cuminai/creator.py` & `cuminai-0.0.1.dev175/cuminai/creator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import os
 import click
 from pathlib import Path
+import http.client
 import yaml
 from cuminai.constants import (
     _CUMINAI_CONFIG_DIR,
     _CUMINAI_CONFIG_FILE,
     _CUMINAI_CREATOR_HOST,
     _CUMIN_FILE_NAME,
     _CUMINAI_DUMMY_TENANT_NAME,
@@ -32,38 +33,52 @@
 
 @executor.command(help='Log in to a Cumin AI managed knowledge store')
 @click.option('-u', '--username',  help='username', required=True)
 @click.option('-k', '--apikey', help='api key', required=True)
 def login(username, apikey):
     username = username.strip()
     apikey = apikey.strip()
+    
+    if not validator.UsernameValidator.match(username):
+        click.echo("username must be an alphanumeric between 6 and 36 characters")
+        return
+
+    if apikey == "":
+        click.echo("apikey can't be empty")
+        return
+
+    # validate the client credentials from Cumin AI
+    connection = http.client.HTTPSConnection("api.creator.cuminai.com", timeout=10)
+    connection.request("GET", "/v1/creator/auth/verify", headers={
+        "CUMINAI-API-KEY": apikey,
+        "CUMINAI-CLIENT-ID": username
+    })
+    response = connection.getresponse()
+    if response.status != 200:
+        click.echo("Login failed: invalid client credentials. please try again with correct username and apikey combination.")
+        return
 
     if not os.path.exists(Path.home() / _CUMINAI_CONFIG_DIR):
         os.makedirs(Path.home() / _CUMINAI_CONFIG_DIR)
         with open(Path.home() / _CUMINAI_CONFIG_DIR / _CUMINAI_CONFIG_FILE, 'x') as f:
             yaml.dump(None, f)
-    
-    if username == "":
-        click.echo("username can't be empty")
-    if apikey == "":
-        click.echo("apikey can't be empty")
 
     data = {}
     with open(Path.home() / _CUMINAI_CONFIG_DIR / _CUMINAI_CONFIG_FILE, 'r') as f:
         data = yaml.safe_load(f)
         if data is None:
             data = {}
 
     data["username"] = username
     data["apikey"] = apikey
         
     with open(Path.home() / _CUMINAI_CONFIG_DIR / _CUMINAI_CONFIG_FILE, 'w') as f:
         yaml.dump(data, f)
 
-    click.echo(f'Cumin AI login Successful for Creator {username}')
+    click.echo(f'Cumin AI login Successful for creator:{username}')
 
 @executor.command(help='Log out from Cumin AI managed knowledge store')
 def logout():
     if not os.path.exists(Path.home() / _CUMINAI_CONFIG_DIR):
         click.echo(f'Creator not logged in yet. "cuminai login" first before logging out')
         return
 
@@ -260,15 +275,15 @@
         any('link' not in source for source in data['knowledge']) or \
         any(not validator.LinkValidator.match(source['link']) for source in data['knowledge']):
         raise ValueError("::invalid knowledge source: 'knowledge' is required, and should be a list of valid knowledge sources of the particular kind to ingest")
     
     if any('metadata' in source and 'tags' in source['metadata'] and not isinstance(source['metadata']['tags'], list) for source in data['knowledge']):
         raise ValueError("::invalid knowledge:metadata:tags: metadata tags should be a list of string tags")
     
-    if any(any(not isinstance(tag, str) for tag in source['metadata']['tags']) for source in data['knowledge']):
+    if any('metadata' in source and any(not isinstance(tag, str) for tag in source['metadata']['tags']) for source in data['knowledge']):
         raise ValueError("::invalid knowledge:metadata:tags: metadata tags should be a list of string tags")
     
     if 'chunkstrategy' in data and not isinstance(data['chunkstrategy'], dict):
         raise ValueError("::invalid chunkstrategy: chunk strategy is optional, but if defined, must be a dict containing size and overlap")
     
     if 'chunkstrategy' in data:
         if 'size' not in data['chunkstrategy'] or not isinstance(data['chunkstrategy']['size'], int) or \
```

### Comparing `cuminai-0.0.1.dev165/cuminai/validator.py` & `cuminai-0.0.1.dev175/cuminai/validator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import re
 
+UsernameValidator = re.compile('^[0-9a-zA-Z]{6,36}$')
 NameValidator = re.compile('^[0-9a-zA-Z]+$')
 
 OllamaEmbeddingValidator = re.compile('^ollama/(mxbai-embed-large|nomic-embed-text|all-minilm)(latest|(:v[0-9a-zA-Z-_.]+))?$')
 
 LinkValidator = re.compile('^(https://www.|https://)[a-zA-Z]{2,}(.[a-zA-Z]{2,})(.[a-zA-Z]{2,})?/[a-zA-Z0-9]{2,}|((https://www.|https://)[a-zA-Z]{2,}(.[a-zA-Z]{2,})(.[a-zA-Z]{2,})?)|(https://www.|https://)[a-zA-Z0-9]{2,}.[a-zA-Z0-9]{2,}.[a-zA-Z0-9]{2,}(.[a-zA-Z0-9]{2,})?$')
 
 OllamaEmbeddingFetcher = re.compile('^ollama/(.*)$')
```

### Comparing `cuminai-0.0.1.dev165/LICENSE` & `cuminai-0.0.1.dev175/LICENSE`

 * *Files identical despite different names*

### Comparing `cuminai-0.0.1.dev165/pyproject.toml` & `cuminai-0.0.1.dev175/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cuminai"
-version = "0.0.1dev165"
+version = "0.0.1dev175"
 description = ""
 authors = ["Harshal Priyadarshi <harshal@cuminai.com>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<3.13"
 numpy = "^1"
```

