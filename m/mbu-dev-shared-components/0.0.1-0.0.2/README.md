# Comparing `tmp/mbu_dev_shared_components-0.0.1.tar.gz` & `tmp/mbu_dev_shared_components-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mbu_dev_shared_components-0.0.1.tar", last modified: Thu May 16 15:30:52 2024, max compression
+gzip compressed data, was "mbu_dev_shared_components-0.0.2.tar", last modified: Thu May 16 19:19:47 2024, max compression
```

## Comparing `mbu_dev_shared_components-0.0.1.tar` & `mbu_dev_shared_components-0.0.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 15:30:52.784467 mbu_dev_shared_components-0.0.1/
--rw-rw-rw-   0        0        0     1085 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      957 2024-05-16 15:30:52.781839 mbu_dev_shared_components-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      498 2024-05-16 15:19:15.000000 mbu_dev_shared_components-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 15:30:52.693278 mbu_dev_shared_components-0.0.1/mbu_dev_shared_components/
-drwxrwxrwx   0        0        0        0 2024-05-16 15:30:52.752771 mbu_dev_shared_components-0.0.1/mbu_dev_shared_components/office365_api/
--rw-rw-rw-   0        0        0        0 2024-05-16 14:20:13.000000 mbu_dev_shared_components-0.0.1/mbu_dev_shared_components/office365_api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:30:52.770177 mbu_dev_shared_components-0.0.1/mbu_dev_shared_components/office365_api/sharepoint_api/
--rw-rw-rw-   0        0        0        0 2024-05-16 14:20:46.000000 mbu_dev_shared_components-0.0.1/mbu_dev_shared_components/office365_api/sharepoint_api/__init__.py
--rw-rw-rw-   0        0        0     8970 2024-05-16 15:09:46.000000 mbu_dev_shared_components-0.0.1/mbu_dev_shared_components/office365_api/sharepoint_api/sharepoint_files.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:30:52.772935 mbu_dev_shared_components-0.0.1/mbu_dev_shared_components/os2forms_api/
--rw-rw-rw-   0        0        0        0 2024-05-16 15:12:48.000000 mbu_dev_shared_components-0.0.1/mbu_dev_shared_components/os2forms_api/__init__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 15:30:52.775414 mbu_dev_shared_components-0.0.1/mbu_dev_shared_components.egg-info/
--rw-rw-rw-   0        0        0      957 2024-05-16 15:30:52.000000 mbu_dev_shared_components-0.0.1/mbu_dev_shared_components.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      521 2024-05-16 15:30:52.000000 mbu_dev_shared_components-0.0.1/mbu_dev_shared_components.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 15:30:52.000000 mbu_dev_shared_components-0.0.1/mbu_dev_shared_components.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       36 2024-05-16 15:30:52.000000 mbu_dev_shared_components-0.0.1/mbu_dev_shared_components.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2024-05-16 15:30:52.000000 mbu_dev_shared_components-0.0.1/mbu_dev_shared_components.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      549 2024-05-16 15:28:33.000000 mbu_dev_shared_components-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-05-16 15:30:52.784970 mbu_dev_shared_components-0.0.1/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-05-16 19:19:47.296642 mbu_dev_shared_components-0.0.2/
+-rw-rw-rw-   0        0        0     1085 2024-05-16 14:14:30.000000 mbu_dev_shared_components-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0      957 2024-05-16 19:19:47.291942 mbu_dev_shared_components-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-05-16 15:19:15.000000 mbu_dev_shared_components-0.0.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 19:19:47.240482 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/
+drwxrwxrwx   0        0        0        0 2024-05-16 19:19:47.275358 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/office365/
+-rw-rw-rw-   0        0        0        0 2024-05-16 14:20:13.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/office365/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 19:19:47.278444 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/office365/sharepoint_api/
+-rw-rw-rw-   0        0        0        0 2024-05-16 14:20:46.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/office365/sharepoint_api/__init__.py
+-rw-rw-rw-   0        0        0     8970 2024-05-16 15:09:46.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/office365/sharepoint_api/files.py
+drwxrwxrwx   0        0        0        0 2024-05-16 19:19:47.280591 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/os2forms_api/
+-rw-rw-rw-   0        0        0        0 2024-05-16 15:12:48.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/os2forms_api/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 19:19:47.290229 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components.egg-info/
+-rw-rw-rw-   0        0        0      957 2024-05-16 19:19:47.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      498 2024-05-16 19:19:47.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 19:19:47.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       36 2024-05-16 19:19:47.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2024-05-16 19:19:47.000000 mbu_dev_shared_components-0.0.2/mbu_dev_shared_components.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      549 2024-05-16 19:18:30.000000 mbu_dev_shared_components-0.0.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-05-16 19:19:47.297143 mbu_dev_shared_components-0.0.2/setup.cfg
```

### Comparing `mbu_dev_shared_components-0.0.1/LICENSE` & `mbu_dev_shared_components-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.1/PKG-INFO` & `mbu_dev_shared_components-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbu_dev_shared_components
-Version: 0.0.1
+Version: 0.0.2
 Summary: Shared components to use in RPA projects
 Author-email: MBU <rpa@mbu.aarhus.dk>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mbu_dev_shared_components-0.0.1/mbu_dev_shared_components/office365_api/sharepoint_api/sharepoint_files.py` & `mbu_dev_shared_components-0.0.2/mbu_dev_shared_components/office365/sharepoint_api/files.py`

 * *Files identical despite different names*

### Comparing `mbu_dev_shared_components-0.0.1/mbu_dev_shared_components.egg-info/PKG-INFO` & `mbu_dev_shared_components-0.0.2/mbu_dev_shared_components.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mbu_dev_shared_components
-Version: 0.0.1
+Version: 0.0.2
 Summary: Shared components to use in RPA projects
 Author-email: MBU <rpa@mbu.aarhus.dk>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: Microsoft :: Windows
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
```

### Comparing `mbu_dev_shared_components-0.0.1/pyproject.toml` & `mbu_dev_shared_components-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=65.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mbu_dev_shared_components"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="MBU", email="rpa@mbu.aarhus.dk" },
 ]
 description = "Shared components to use in RPA projects"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

