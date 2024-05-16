# Comparing `tmp/shaped-0.8.0.tar.gz` & `tmp/shaped-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/io/dist/.tmp-lok_txkm/shaped-0.8.0.tar", last modified: Wed Oct 25 22:31:21 2023, max compression
+gzip compressed data, was "shaped-0.9.0.tar", last modified: Fri Dec 15 20:19:17 2023, max compression
```

## Comparing `shaped-0.8.0.tar` & `shaped-0.9.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 22:31:21.000000 shaped-0.8.0/
--rw-r--r--   0 root         (0) root         (0)     2474 2023-10-25 22:31:21.000000 shaped-0.8.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1936 2023-03-29 16:19:37.000000 shaped-0.8.0/README.md
--rwxr-xr-x   0 root         (0) root         (0)       81 2023-03-07 19:31:59.000000 shaped-0.8.0/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-10-25 22:31:21.000000 shaped-0.8.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1254 2023-10-25 22:29:04.000000 shaped-0.8.0/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 22:31:21.000000 shaped-0.8.0/shaped.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2474 2023-10-25 22:31:20.000000 shaped-0.8.0/shaped.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      274 2023-10-25 22:31:20.000000 shaped-0.8.0/shaped.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-25 22:31:20.000000 shaped-0.8.0/shaped.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       46 2023-10-25 22:31:20.000000 shaped-0.8.0/shaped.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      107 2023-10-25 22:31:20.000000 shaped-0.8.0/shaped.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        4 2023-10-25 22:31:20.000000 shaped-0.8.0/shaped.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-23 19:25:57.000000 shaped-0.8.0/shaped.egg-info/zip-safe
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-25 22:31:21.000000 shaped-0.8.0/src/
--rw-r--r--   0 root         (0) root         (0)        0 2023-03-08 16:04:34.000000 shaped-0.8.0/src/__init__.py
--rw-r--r--   0 root         (0) root         (0)     9213 2023-10-25 22:28:26.000000 shaped-0.8.0/src/shaped_cli.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:19:16.996005 shaped-0.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2023-12-15 20:19:16.992005 shaped-0.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1936 2023-12-15 20:19:03.000000 shaped-0.9.0/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)       81 2023-12-15 20:19:03.000000 shaped-0.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-15 20:19:16.996005 shaped-0.9.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1254 2023-12-15 20:19:03.000000 shaped-0.9.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:19:16.992005 shaped-0.9.0/shaped.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2686 2023-12-15 20:19:16.000000 shaped-0.9.0/shaped.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      274 2023-12-15 20:19:16.000000 shaped-0.9.0/shaped.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 20:19:16.000000 shaped-0.9.0/shaped.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2023-12-15 20:19:16.000000 shaped-0.9.0/shaped.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2023-12-15 20:19:16.000000 shaped-0.9.0/shaped.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        4 2023-12-15 20:19:16.000000 shaped-0.9.0/shaped.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-15 20:19:16.000000 shaped-0.9.0/shaped.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-15 20:19:16.992005 shaped-0.9.0/src/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2023-12-15 20:19:03.000000 shaped-0.9.0/src/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9884 2023-12-15 20:19:03.000000 shaped-0.9.0/src/shaped_cli.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `shaped-0.8.0/PKG-INFO` & `shaped-0.9.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: shaped
-Version: 0.8.0
+Version: 0.9.0
 Summary: A CLI tool for interacting with the Shaped API.
 Home-page: https://github.com/shaped-ai/shaped-cli
 Author: Shaped Team
 Author-email: support@shaped.ai
 Keywords: shaped-ai
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: typer[all]>=0.7.0
+Requires-Dist: requests>=2.28.1
+Requires-Dist: pydantic>=1.10.2
+Requires-Dist: pyyaml>=6.0
+Requires-Dist: pyarrow==11.0.0
+Requires-Dist: pandas==1.5.3
+Requires-Dist: tqdm==4.65.0
 
 # Shaped CLI
 
 CLI for interactions with the Shaped API.
 
 ## Installing the Shaped CLI
```

### Comparing `shaped-0.8.0/README.md` & `shaped-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `shaped-0.8.0/setup.py` & `shaped-0.9.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import os
 
 from setuptools import find_packages, setup
 
 with open("README.md") as f:
     long_description = f.read()
 
-version = "0.8.0"
+version = "0.9.0"
 circleci_build_number = os.getenv("CIRCLE_BUILD_NUM", "")
 if circleci_build_number != "":
     version = f"{version}.dev{circleci_build_number}"
 
 setup(
     name="shaped",
     version=version,
```

### Comparing `shaped-0.8.0/shaped.egg-info/PKG-INFO` & `shaped-0.9.0/shaped.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,29 @@
 Metadata-Version: 2.1
 Name: shaped
-Version: 0.8.0
+Version: 0.9.0
 Summary: A CLI tool for interacting with the Shaped API.
 Home-page: https://github.com/shaped-ai/shaped-cli
 Author: Shaped Team
 Author-email: support@shaped.ai
 Keywords: shaped-ai
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Programming Language :: Python :: 3
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
+Requires-Dist: typer[all]>=0.7.0
+Requires-Dist: requests>=2.28.1
+Requires-Dist: pydantic>=1.10.2
+Requires-Dist: pyyaml>=6.0
+Requires-Dist: pyarrow==11.0.0
+Requires-Dist: pandas==1.5.3
+Requires-Dist: tqdm==4.65.0
 
 # Shaped CLI
 
 CLI for interactions with the Shaped API.
 
 ## Installing the Shaped CLI
```

### Comparing `shaped-0.8.0/src/shaped_cli.py` & `shaped-0.9.0/src/shaped_cli.py`

 * *Files 4% similar despite different names*

```diff
@@ -119,37 +119,54 @@
 
 @app.command()
 def rank(
     model_name: str = typer.Option(...),
     user_id = typer.Option(None),
     limit=typer.Option(15),
     filter_predicate=typer.Option(None),
-    search: str = typer.Option(None),
+    text_query: str = typer.Option(None),
     return_metadata: bool = typer.Option(False),
+    flush_paginations: bool = typer.Option(False),
     exploration_factor: float = typer.Option(0.0),
+    diversity_factor: float = typer.Option(0.0),
+    extra_query_args: str = typer.Option(None)
 ):
     config = _read_config()
     url = f"{_get_shaped_url(config)}/models/{model_name}/rank"
     headers = {"accept": "application/json", "x-api-key": config.api_key}
     if exploration_factor < 0.0 or exploration_factor > 1.0:
         raise typer.BadParameter("`exploration_factor` must be between 0.0 and 1.0")
-    query_args = {"exploration_factor": exploration_factor}
+
+    if diversity_factor < 0.0:
+        raise typer.BadParameter("`diversity_factor` must be greater than 0.0")
+
+    query_args = {
+        "exploration_factor": exploration_factor,
+        "diversity_factor": diversity_factor,
+        "limit": str(limit)
+    }
+
     if user_id is not None:
         query_args |= {"user_id": user_id}
     if filter_predicate is not None:
         query_args |= {"filter_predicate": filter_predicate}
     if return_metadata is not None:
         query_args |= {"return_metadata": bool(return_metadata)}
-    if search is not None:
-        query_args |= {"search": search}
+    if text_query is not None:
+        query_args |= {"text_query": text_query}
+    if flush_paginations is not None:
+        query_args |= {"flush_paginations": flush_paginations}
+    if extra_query_args is not None:
+        extra_query_args = json.loads(extra_query_args)
+        query_args |= extra_query_args
 
     response = requests.post(
         url,
         headers=headers,
-        json={"limit": str(limit), **query_args},
+        json=query_args
     )
     typer.echo(_parse_response_as_yaml(response.text))
 
 
 @app.command()
 def similar(
     model_name: str = typer.Option(...),
@@ -235,14 +252,18 @@
     headers = {"accept": "application/json", "x-api-key": config.api_key}
     bar = tqdm(unit=" Records")
 
     def _write_chunk(chunk: pd.DataFrame):
         bar.update(len(chunk))
         payload = json.dumps({"data": json.loads(chunk.to_json(orient="records"))})
         response = requests.post(url, headers=headers, data=payload)
+        if response.status_code != 200:
+            typer.echo(response.text)
+            return
+
         _parse_response_as_yaml(response.text)
 
     # Chunk read and upload.
     chunk_size = 1000
     if type == "parquet":
 
         # Note this only works for parquet partitions (i.e. single binary files).
```

