# Comparing `tmp/abraham_md-0.1.1.tar.gz` & `tmp/abraham_md-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abraham_md-0.1.1.tar", max compression
+gzip compressed data, was "abraham_md-0.2.0.tar", max compression
```

## Comparing `abraham_md-0.1.1.tar` & `abraham_md-0.2.0.tar`

### file list

```diff
@@ -1,15 +1,29 @@
--rw-r--r--   0        0        0     1090 2024-05-07 14:41:06.608685 abraham_md-0.1.1/LICENSE
--rw-r--r--   0        0        0     2925 2024-05-07 14:42:58.193523 abraham_md-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1075 2024-05-07 14:41:06.652678 abraham_md-0.1.1/README.md
--rw-r--r--   0        0        0        0 2024-05-07 14:41:06.432425 abraham_md-0.1.1/source/abraham_md/__init__.py
--rw-r--r--   0        0        0        0 2024-05-07 14:41:06.300329 abraham_md-0.1.1/source/abraham_md/config/__init__.py
--rw-r--r--   0        0        0      603 2024-05-07 14:42:43.283256 abraham_md-0.1.1/source/abraham_md/config/constants.py
--rw-r--r--   0        0        0     1442 2024-05-07 14:42:43.284520 abraham_md-0.1.1/source/abraham_md/config/paths.py
--rw-r--r--   0        0        0        0 2024-05-07 14:41:06.344935 abraham_md-0.1.1/source/abraham_md/interface/__init__.py
--rw-r--r--   0        0        0      422 2024-05-07 14:42:43.285519 abraham_md-0.1.1/source/abraham_md/interface/command_line.py
--rw-r--r--   0        0        0        0 2024-05-07 14:41:06.369314 abraham_md-0.1.1/source/abraham_md/logs/__init__.py
--rw-r--r--   0        0        0     1879 2024-05-07 14:42:43.287841 abraham_md-0.1.1/source/abraham_md/logs/setup_logging.py
--rw-r--r--   0        0        0      538 2024-05-07 14:42:21.002478 abraham_md-0.1.1/source/abraham_md/main.py
--rw-r--r--   0        0        0        0 2024-05-07 14:41:06.494505 abraham_md-0.1.1/source/abraham_md/py.typed
--rw-r--r--   0        0        0        5 2024-05-07 14:41:06.506652 abraham_md-0.1.1/source/abraham_md/VERSION
--rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 abraham_md-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1090 2024-05-07 14:41:06.608685 abraham_md-0.2.0/LICENSE
+-rw-r--r--   0        0        0     2925 2024-05-16 21:58:47.533087 abraham_md-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1075 2024-05-07 14:44:41.642261 abraham_md-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-07 14:41:06.432425 abraham_md-0.2.0/source/abraham_md/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:41:06.300329 abraham_md-0.2.0/source/abraham_md/config/__init__.py
+-rw-r--r--   0        0        0     1732 2024-05-16 21:51:27.079863 abraham_md-0.2.0/source/abraham_md/config/constants.py
+-rw-r--r--   0        0        0     1978 2024-05-10 00:10:53.530487 abraham_md-0.2.0/source/abraham_md/config/dialogue.py
+-rw-r--r--   0        0        0     1440 2024-05-12 00:09:58.433088 abraham_md-0.2.0/source/abraham_md/config/paths.py
+-rw-r--r--   0        0        0     1622 2024-05-10 12:54:28.981922 abraham_md-0.2.0/source/abraham_md/config/structures.py
+-rw-r--r--   0        0        0      565 2024-05-10 13:28:57.245163 abraham_md-0.2.0/source/abraham_md/config/type_annotations.py
+-rw-r--r--   0        0        0        0 2024-05-09 23:32:06.524598 abraham_md-0.2.0/source/abraham_md/generation/__init__.py
+-rw-r--r--   0        0        0     9869 2024-05-10 20:34:56.661348 abraham_md-0.2.0/source/abraham_md/generation/module_data_structures.py
+-rw-r--r--   0        0        0     2951 2024-05-16 21:56:42.028592 abraham_md-0.2.0/source/abraham_md/generation/module_logic.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:41:06.344935 abraham_md-0.2.0/source/abraham_md/interface/__init__.py
+-rw-r--r--   0        0        0     1949 2024-05-10 00:11:03.134115 abraham_md-0.2.0/source/abraham_md/interface/command_line.py
+-rw-r--r--   0        0        0     3577 2024-05-09 12:21:57.286417 abraham_md-0.2.0/source/abraham_md/interface/graphical.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:41:06.369314 abraham_md-0.2.0/source/abraham_md/logs/__init__.py
+-rw-r--r--   0        0        0     1879 2024-05-07 14:42:43.287841 abraham_md-0.2.0/source/abraham_md/logs/setup_logging.py
+-rw-r--r--   0        0        0     2959 2024-05-12 00:33:34.027259 abraham_md-0.2.0/source/abraham_md/main.py
+-rw-r--r--   0        0        0        0 2024-05-08 16:27:23.861307 abraham_md-0.2.0/source/abraham_md/processing/__init__.py
+-rw-r--r--   0        0        0     4889 2024-05-12 00:17:54.669783 abraham_md-0.2.0/source/abraham_md/processing/file_conversion.py
+-rw-r--r--   0        0        0     4088 2024-05-11 23:47:12.880549 abraham_md-0.2.0/source/abraham_md/processing/file_interaction.py
+-rw-r--r--   0        0        0     2073 2024-05-09 22:55:16.874934 abraham_md-0.2.0/source/abraham_md/processing/llm_integration.py
+-rw-r--r--   0        0        0        0 2024-05-07 14:41:06.494505 abraham_md-0.2.0/source/abraham_md/py.typed
+-rw-r--r--   0        0        0     2064 2024-05-10 15:23:19.138279 abraham_md-0.2.0/source/abraham_md/templates/overview.md.j2
+-rw-r--r--   0        0        0        0 2024-05-08 10:59:22.408212 abraham_md-0.2.0/source/abraham_md/validation/__init__.py
+-rw-r--r--   0        0        0     2720 2024-05-10 12:29:31.229464 abraham_md-0.2.0/source/abraham_md/validation/path_validation.py
+-rw-r--r--   0        0        0        5 2024-05-07 14:41:06.506652 abraham_md-0.2.0/source/abraham_md/VERSION
+-rw-r--r--   0        0        0     2066 1970-01-01 00:00:00.000000 abraham_md-0.2.0/PKG-INFO
```

### Comparing `abraham_md-0.1.1/LICENSE` & `abraham_md-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `abraham_md-0.1.1/pyproject.toml` & `abraham_md-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "abraham_md"
-version = "0.1.1"
+version = "0.2.0"
 description = "Converts University of Lincoln module files into a useful Obsidian Vault for keeping notes throughout the academic year, as well as revising at the end of an academic year."
 authors = ["W. Fayers <wills@fayers.com>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "abraham_md", from = "source"}]
 homepage = "https://github.com/unkokaeru/abraham_md"
 repository = "https://github.com/unkokaeru/abraham_md"
```

### Comparing `abraham_md-0.1.1/README.md` & `abraham_md-0.2.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # abraham_md
 
-![Continuous Integration (CI) Tests](https://github.com/unkokaeru/abraham_md/actions/workflows/continuous_integration.yml/badge.svg)
+![Continuous Integration (CI) Tests](https://github.com/unkokaeru/abraham-md/actions/workflows/continuous_integration.yml/badge.svg)
 
 Converts University of Lincoln module files into a useful Obsidian Vault for keeping notes throughout the academic year, as well as revising at the end of an academic year.
 
 ## Installation
 
 To install abraham_md, simply run:
```

### Comparing `abraham_md-0.1.1/source/abraham_md/config/paths.py` & `abraham_md-0.2.0/source/abraham_md/config/paths.py`

 * *Files 4% similar despite different names*

```diff
@@ -45,8 +45,8 @@
             if file.is_file():
                 shutil.copy(str(file), str(cls.temp_dir))
 
     TEMPLATES_PATH = temp_dir
 
 
 # Clone the templates directory to a temporary directory if rendering templates
-# Paths.temporary_clone("abraham_md.templates")
+Paths.temporary_clone("abraham_md.templates")
```

### Comparing `abraham_md-0.1.1/source/abraham_md/logs/setup_logging.py` & `abraham_md-0.2.0/source/abraham_md/logs/setup_logging.py`

 * *Files identical despite different names*

### Comparing `abraham_md-0.1.1/PKG-INFO` & `abraham_md-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abraham_md
-Version: 0.1.1
+Version: 0.2.0
 Summary: Converts University of Lincoln module files into a useful Obsidian Vault for keeping notes throughout the academic year, as well as revising at the end of an academic year.
 Home-page: https://github.com/unkokaeru/abraham_md
 License: MIT
 Author: W. Fayers
 Author-email: wills@fayers.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
@@ -23,15 +23,15 @@
 Provides-Extra: types
 Requires-Dist: rich (>=12.0.0,<13.0.0)
 Project-URL: Repository, https://github.com/unkokaeru/abraham_md
 Description-Content-Type: text/markdown
 
 # abraham_md
 
-![Continuous Integration (CI) Tests](https://github.com/unkokaeru/abraham_md/actions/workflows/continuous_integration.yml/badge.svg)
+![Continuous Integration (CI) Tests](https://github.com/unkokaeru/abraham-md/actions/workflows/continuous_integration.yml/badge.svg)
 
 Converts University of Lincoln module files into a useful Obsidian Vault for keeping notes throughout the academic year, as well as revising at the end of an academic year.
 
 ## Installation
 
 To install abraham_md, simply run:
```

