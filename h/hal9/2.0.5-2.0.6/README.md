# Comparing `tmp/hal9-2.0.5.tar.gz` & `tmp/hal9-2.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hal9-2.0.5.tar", max compression
+gzip compressed data, was "hal9-2.0.6.tar", max compression
```

## Comparing `hal9-2.0.5.tar` & `hal9-2.0.6.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     2951 2024-05-13 20:08:58.664846 hal9-2.0.5/README.md
--rw-r--r--   0        0        0       86 2024-05-13 20:08:58.596845 hal9-2.0.5/hal9/__init__.py
--rw-r--r--   0        0        0     1127 2024-05-13 20:08:58.596845 hal9-2.0.5/hal9/cli.py
--rw-r--r--   0        0        0      634 2024-05-13 20:08:58.596845 hal9-2.0.5/hal9/create.py
--rw-r--r--   0        0        0      482 2024-05-13 20:08:58.596845 hal9-2.0.5/hal9/deploy.py
--rw-r--r--   0        0        0      531 2024-05-13 20:08:58.596845 hal9-2.0.5/hal9/run.py
--rw-r--r--   0        0        0      342 2024-05-13 20:08:58.596845 hal9-2.0.5/hal9/targets/docker.py
--rw-r--r--   0        0        0      467 2024-05-13 20:08:58.600845 hal9-2.0.5/hal9/targets/hal9.py
--rw-r--r--   0        0        0       42 2024-05-13 20:08:58.600845 hal9-2.0.5/hal9/templates/docker/Dockerfile
--rw-r--r--   0        0        0       70 2024-05-13 20:08:58.600845 hal9-2.0.5/hal9/templates/openai/app.py
--rw-r--r--   0        0        0      434 2024-05-13 20:08:58.600845 hal9-2.0.5/pyproject.toml
--rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 hal9-2.0.5/PKG-INFO
+-rw-r--r--   0        0        0     2951 2024-05-15 03:40:34.327792 hal9-2.0.6/README.md
+-rw-r--r--   0        0        0       86 2024-05-15 03:40:34.255791 hal9-2.0.6/hal9/__init__.py
+-rw-r--r--   0        0        0     1220 2024-05-15 03:40:34.255791 hal9-2.0.6/hal9/cli.py
+-rw-r--r--   0        0        0      634 2024-05-15 03:40:34.255791 hal9-2.0.6/hal9/create.py
+-rw-r--r--   0        0        0      574 2024-05-15 03:40:34.255791 hal9-2.0.6/hal9/deploy.py
+-rw-r--r--   0        0        0      531 2024-05-15 03:40:34.259791 hal9-2.0.6/hal9/run.py
+-rw-r--r--   0        0        0      352 2024-05-15 03:40:34.259791 hal9-2.0.6/hal9/targets/docker.py
+-rw-r--r--   0        0        0     2061 2024-05-15 03:40:34.259791 hal9-2.0.6/hal9/targets/hal9.py
+-rw-r--r--   0        0        0       42 2024-05-15 03:40:34.259791 hal9-2.0.6/hal9/templates/docker/Dockerfile
+-rw-r--r--   0        0        0       70 2024-05-15 03:40:34.259791 hal9-2.0.6/hal9/templates/openai/app.py
+-rw-r--r--   0        0        0      434 2024-05-15 03:40:34.259791 hal9-2.0.6/pyproject.toml
+-rw-r--r--   0        0        0     3589 1970-01-01 00:00:00.000000 hal9-2.0.6/PKG-INFO
```

### Comparing `hal9-2.0.5/README.md` & `hal9-2.0.6/README.md`

 * *Files identical despite different names*

### Comparing `hal9-2.0.5/hal9/cli.py` & `hal9-2.0.6/hal9/cli.py`

 * *Files 18% similar despite different names*

```diff
@@ -33,21 +33,22 @@
     PATH: The path to the project. Required argument.
     """
     api_run(path)
 
 @click.command()
 @click.argument('path')
 @click.option('--target', default="hal9", help='Deployment target')
-def deploy(path :str, target :str):
+@click.option('--url', default="https://api.hal9.com", help='Deployment url')
+def deploy(path :str, target :str, url :str):
     """
     Deploy Project
 
     PATH: The path to the project. Required argument.
     """
-    api_deploy(path, target)
+    api_deploy(path, target, url)
 
 cli.add_command(create)
 cli.add_command(run)
 cli.add_command(deploy)
 
 if __name__ == "__main__":
     cli()
```

### Comparing `hal9-2.0.5/hal9/create.py` & `hal9-2.0.6/hal9/create.py`

 * *Files identical despite different names*

### Comparing `hal9-2.0.5/hal9/run.py` & `hal9-2.0.6/hal9/run.py`

 * *Files identical despite different names*

### Comparing `hal9-2.0.5/PKG-INFO` & `hal9-2.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hal9
-Version: 2.0.5
+Version: 2.0.6
 Summary: 
 Author: Javier Luraschi
 Author-email: javier@hal9.ai
 Requires-Python: >=3.8, !=2.7.*, !=3.0.*, !=3.1.*, !=3.2.*, !=3.3.*, !=3.4.*, !=3.5.*, !=3.6.*, !=3.7.*
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

