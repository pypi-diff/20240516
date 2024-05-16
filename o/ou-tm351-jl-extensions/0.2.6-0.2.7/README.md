# Comparing `tmp/ou_tm351_jl_extensions-0.2.6.tar.gz` & `tmp/ou_tm351_jl_extensions-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ou_tm351_jl_extensions-0.2.6.tar", max compression
+gzip compressed data, was "ou_tm351_jl_extensions-0.2.7.tar", max compression
```

## Comparing `ou_tm351_jl_extensions-0.2.6.tar` & `ou_tm351_jl_extensions-0.2.7.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1074 2023-05-04 10:46:43.497008 ou_tm351_jl_extensions-0.2.6/LICENSE
--rw-r--r--   0        0        0     1226 2023-07-21 20:49:34.016848 ou_tm351_jl_extensions-0.2.6/README.md
--rw-r--r--   0        0        0     2388 2023-05-04 15:50:37.140962 ou_tm351_jl_extensions-0.2.6/ou_tm351_jl_extensions/__init__.py
--rw-r--r--   0        0        0     1775 2024-05-08 15:12:02.057289 ou_tm351_jl_extensions-0.2.6/pyproject.toml
--rw-r--r--   0        0        0     2836 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.2.6/PKG-INFO
+-rw-r--r--   0        0        0     1074 2023-05-04 10:46:43.497008 ou_tm351_jl_extensions-0.2.7/LICENSE
+-rw-r--r--   0        0        0     1950 2024-05-15 12:55:07.442996 ou_tm351_jl_extensions-0.2.7/README.md
+-rw-r--r--   0        0        0     2388 2023-05-04 15:50:37.140962 ou_tm351_jl_extensions-0.2.7/ou_tm351_jl_extensions/__init__.py
+-rw-r--r--   0        0        0     1832 2024-05-15 14:32:28.287918 ou_tm351_jl_extensions-0.2.7/pyproject.toml
+-rw-r--r--   0        0        0     3569 1970-01-01 00:00:00.000000 ou_tm351_jl_extensions-0.2.7/PKG-INFO
```

### Comparing `ou_tm351_jl_extensions-0.2.6/LICENSE` & `ou_tm351_jl_extensions-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.6/ou_tm351_jl_extensions/__init__.py` & `ou_tm351_jl_extensions-0.2.7/ou_tm351_jl_extensions/__init__.py`

 * *Files identical despite different names*

### Comparing `ou_tm351_jl_extensions-0.2.6/pyproject.toml` & `ou_tm351_jl_extensions-0.2.7/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 [tool.poetry]
 name = "ou-tm351-jl-extensions"
-version = "0.2.6"
+version = "0.2.7"
 description = ""
 authors = ["Tony Hirst <tony.hirst@gmail.com>"]
 readme = "README.md"
 packages = [{include = "ou_tm351_jl_extensions"}]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.13"
 jupyterlab = ">=4.1"
 
 # Branding and OU extensions
-jupyterlab-ou-brand-extension = "^0.2.0" # OU brand extension (faviocon.logo)
+jupyterlab-ou-brand-extension = "^0.2.0" # OU brand extension (favicon, logo)
 
 # Notebook cell tools
-jupyterlab-cell-status-extension = "^0.1.3" # cell execution status; accessibility tools
-jupyterlab-empinken-extension = "^0.5.0" # cell background styling
+jupyterlab-cell-status-extension = "^0.2.2" # cell execution status; accessibility tools
+jupyterlab-empinken-extension = "^0.5.2" # cell background styling
 jupyterlab-skip-traceback = "^5.1.0" # skip trackeback / error reporting
 jupyterlab-myst = "^2.4.0" ## MyST parser and styling (markdown cells)
 jupyterlab-spellchecker = "^0.8.4" ## Spellchecker
 
 # Code support
-jupyterlab-lsp = "^5.1.0" # language server protocol
+#jupyterlab-lsp = "^5.1.0" # language server protocol
 jupyterlab-code-formatter = "^2.2.1" # Code formatter
 black = "^24.4.2" # code formatting
 isort = "^5.13.2" # code formatting
 
 # Language packs
 jupyterlab-language-pack-fr-fr = "^4.1.post2" # French
 jupyterlab-language-pack-zh-cn = "^4.1.post2" # Chinese
@@ -38,15 +38,16 @@
 jupytext = "^1.16.0" # text notebook formats
 
 # Renderers
 jupyterlab-geojson = "^3.3.1" # geojson renderer
 jupyter-compare-view = "^0.2.4" # compare images
 
 # Resource monitoring
-jupyter-resource-usage = "^1.0.2" # memorry/CPU
+jupyter-resource-usage = "^1.0.2" # memory/CPU
+jupyterlab_execute_time = "^3.1.2" # cell execution time
 
 # Misc, evaluation, etc
 #stickyland = "^0.2.1" # sticky notes - BROKEN?
 #jupyterlab-tour = "^3.1.4" # Jupyterlab tour (irritating!)
 
 
 [build-system]
```

