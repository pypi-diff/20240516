# Comparing `tmp/protein_turnover-0.3.7.tar.gz` & `tmp/protein_turnover-0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "protein_turnover-0.3.7.tar", max compression
+gzip compressed data, was "protein_turnover-0.3.8.tar", max compression
```

## Comparing `protein_turnover-0.3.7.tar` & `protein_turnover-0.3.8.tar`

### file list

```diff
@@ -1,45 +1,46 @@
--rw-r--r--   0        0        0     1068 2024-04-10 10:25:59.389801 protein_turnover-0.3.7/LICENSE
--rw-r--r--   0        0        0        0 2022-09-06 02:29:35.838848 protein_turnover-0.3.7/protein_turnover/__init__.py
--rw-r--r--   0        0        0      481 2024-04-12 09:19:03.438815 protein_turnover-0.3.7/protein_turnover/__main__.py
--rw-r--r--   0        0        0      142 2024-04-18 09:07:07.364073 protein_turnover-0.3.7/protein_turnover/api.py
--rw-r--r--   0        0        0     9778 2024-04-15 08:28:10.056355 protein_turnover-0.3.7/protein_turnover/background.py
--rw-r--r--   0        0        0     1594 2024-04-11 07:40:50.403214 protein_turnover-0.3.7/protein_turnover/background_ui.py
--rw-r--r--   0        0        0     6670 2024-04-11 05:21:49.849892 protein_turnover-0.3.7/protein_turnover/broken_api.py
--rw-r--r--   0        0        0     2745 2024-04-11 02:01:52.718758 protein_turnover-0.3.7/protein_turnover/cli.py
--rw-r--r--   0        0        0     1390 2024-04-18 06:46:32.496210 protein_turnover-0.3.7/protein_turnover/config.py
--rw-r--r--   0        0        0        0 2023-04-17 04:28:06.153132 protein_turnover-0.3.7/protein_turnover/dinosaur/__init__.py
--rw-r--r--   0        0        0     3062 2023-08-29 07:02:47.263592 protein_turnover-0.3.7/protein_turnover/dinosaur/cmd.py
--rw-r--r--   0        0        0     1918 2024-04-10 08:19:00.355662 protein_turnover-0.3.7/protein_turnover/dinosaur/dinosaur.py
--rw-r--r--   0        0        0     1691 2023-11-01 09:45:31.835472 protein_turnover-0.3.7/protein_turnover/filters.py
--rw-r--r--   0        0        0    19858 2024-03-28 01:40:54.972101 protein_turnover-0.3.7/protein_turnover/fitenvelopes.py
--rw-r--r--   0        0        0     7124 2024-04-15 08:28:10.056355 protein_turnover-0.3.7/protein_turnover/jobs.py
--rw-r--r--   0        0        0     1511 2023-10-31 22:36:14.534600 protein_turnover-0.3.7/protein_turnover/logger.py
--rw-r--r--   0        0        0      981 2023-08-28 10:18:07.794829 protein_turnover-0.3.7/protein_turnover/mailer.py
--rw-r--r--   0        0        0     2708 2024-04-11 05:19:39.944840 protein_turnover-0.3.7/protein_turnover/parallel_utils.py
--rw-r--r--   0        0        0    12680 2024-04-11 11:28:05.946176 protein_turnover-0.3.7/protein_turnover/pepxml.py
--rw-r--r--   0        0        0    29793 2023-11-06 13:19:24.639523 protein_turnover-0.3.7/protein_turnover/pepxml_reader.py
--rw-r--r--   0        0        0     4181 2024-04-11 03:10:41.293175 protein_turnover-0.3.7/protein_turnover/pepxml_ui.py
--rw-r--r--   0        0        0    18499 2023-10-31 22:36:18.510700 protein_turnover-0.3.7/protein_turnover/plotting.py
--rw-r--r--   0        0        0     3817 2024-02-06 08:48:02.313547 protein_turnover-0.3.7/protein_turnover/protxml.py
--rw-r--r--   0        0        0        0 2023-08-29 04:01:11.951477 protein_turnover-0.3.7/protein_turnover/py.typed
--rw-r--r--   0        0        0    26888 2024-04-26 00:23:46.745567 protein_turnover-0.3.7/protein_turnover/pymz.py
--rw-r--r--   0        0        0    10050 2024-04-24 05:27:48.262533 protein_turnover-0.3.7/protein_turnover/pymz_ui.py
--rw-r--r--   0        0        0     2571 2023-09-01 03:32:11.939419 protein_turnover-0.3.7/protein_turnover/settings.py
--rw-r--r--   0        0        0     2726 2023-11-05 07:06:29.593017 protein_turnover-0.3.7/protein_turnover/sns.py
--rw-r--r--   0        0        0        0 2022-11-02 03:43:40.908584 protein_turnover-0.3.7/protein_turnover/sqla/__init__.py
--rw-r--r--   0        0        0     4791 2024-04-02 05:33:08.127208 protein_turnover-0.3.7/protein_turnover/sqla/iso_peaks.py
--rw-r--r--   0        0        0     3982 2024-04-12 09:19:03.622817 protein_turnover-0.3.7/protein_turnover/sqla/iso_peaks_ui.py
--rw-r--r--   0        0        0    12901 2024-04-11 04:06:36.929908 protein_turnover-0.3.7/protein_turnover/sqla/model.py
--rw-r--r--   0        0        0    20036 2024-04-10 06:44:53.511669 protein_turnover-0.3.7/protein_turnover/sqla/query.py
--rw-r--r--   0        0        0     5249 2024-02-14 07:30:52.792197 protein_turnover-0.3.7/protein_turnover/sqla/utils.py
--rw-r--r--   0        0        0        0 2022-09-06 02:29:35.846848 protein_turnover-0.3.7/protein_turnover/types/__init__.py
--rw-r--r--   0        0        0     7955 2023-11-03 02:17:35.435401 protein_turnover-0.3.7/protein_turnover/types/checking.py
--rw-r--r--   0        0        0      956 2023-08-28 10:18:07.838829 protein_turnover-0.3.7/protein_turnover/types/mzmltypes.py
--rw-r--r--   0        0        0     1874 2023-08-28 10:18:07.806829 protein_turnover-0.3.7/protein_turnover/types/pepxmltypes.py
--rw-r--r--   0        0        0     2594 2023-08-28 10:18:07.838829 protein_turnover-0.3.7/protein_turnover/types/turnovertype.py
--rw-r--r--   0        0        0     7509 2023-11-05 22:47:34.227461 protein_turnover-0.3.7/protein_turnover/unimod.py
--rw-r--r--   0        0        0    20458 2024-04-18 12:12:35.320150 protein_turnover-0.3.7/protein_turnover/utils.py
--rw-r--r--   0        0        0     5798 2024-04-15 04:58:55.719116 protein_turnover-0.3.7/protein_turnover/web.py
--rw-r--r--   0        0        0     2614 2024-04-15 08:27:59.960224 protein_turnover-0.3.7/protein_turnover/web_ui.py
--rw-r--r--   0        0        0     1129 2024-04-24 05:33:56.862021 protein_turnover-0.3.7/pyproject.toml
--rw-r--r--   0        0        0     1285 1970-01-01 00:00:00.000000 protein_turnover-0.3.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-10 10:25:59.389801 protein_turnover-0.3.8/LICENSE
+-rw-r--r--   0        0        0       54 2024-04-26 05:23:38.437576 protein_turnover-0.3.8/prerelease.md
+-rw-r--r--   0        0        0        0 2022-09-06 02:29:35.838848 protein_turnover-0.3.8/protein_turnover/__init__.py
+-rw-r--r--   0        0        0      481 2024-04-12 09:19:03.438815 protein_turnover-0.3.8/protein_turnover/__main__.py
+-rw-r--r--   0        0        0      142 2024-04-18 09:07:07.364073 protein_turnover-0.3.8/protein_turnover/api.py
+-rw-r--r--   0        0        0     9778 2024-04-15 08:28:10.056355 protein_turnover-0.3.8/protein_turnover/background.py
+-rw-r--r--   0        0        0     1594 2024-04-11 07:40:50.403214 protein_turnover-0.3.8/protein_turnover/background_ui.py
+-rw-r--r--   0        0        0     6670 2024-04-11 05:21:49.849892 protein_turnover-0.3.8/protein_turnover/broken_api.py
+-rw-r--r--   0        0        0     2745 2024-04-11 02:01:52.718758 protein_turnover-0.3.8/protein_turnover/cli.py
+-rw-r--r--   0        0        0     1390 2024-04-18 06:46:32.496210 protein_turnover-0.3.8/protein_turnover/config.py
+-rw-r--r--   0        0        0        0 2023-04-17 04:28:06.153132 protein_turnover-0.3.8/protein_turnover/dinosaur/__init__.py
+-rw-r--r--   0        0        0     3062 2023-08-29 07:02:47.263592 protein_turnover-0.3.8/protein_turnover/dinosaur/cmd.py
+-rw-r--r--   0        0        0     1918 2024-04-10 08:19:00.355662 protein_turnover-0.3.8/protein_turnover/dinosaur/dinosaur.py
+-rw-r--r--   0        0        0     1691 2023-11-01 09:45:31.835472 protein_turnover-0.3.8/protein_turnover/filters.py
+-rw-r--r--   0        0        0    19858 2024-03-28 01:40:54.972101 protein_turnover-0.3.8/protein_turnover/fitenvelopes.py
+-rw-r--r--   0        0        0     7124 2024-04-15 08:28:10.056355 protein_turnover-0.3.8/protein_turnover/jobs.py
+-rw-r--r--   0        0        0     1511 2023-10-31 22:36:14.534600 protein_turnover-0.3.8/protein_turnover/logger.py
+-rw-r--r--   0        0        0      981 2023-08-28 10:18:07.794829 protein_turnover-0.3.8/protein_turnover/mailer.py
+-rw-r--r--   0        0        0     2708 2024-04-11 05:19:39.944840 protein_turnover-0.3.8/protein_turnover/parallel_utils.py
+-rw-r--r--   0        0        0    12680 2024-04-11 11:28:05.946176 protein_turnover-0.3.8/protein_turnover/pepxml.py
+-rw-r--r--   0        0        0    29793 2023-11-06 13:19:24.639523 protein_turnover-0.3.8/protein_turnover/pepxml_reader.py
+-rw-r--r--   0        0        0     4181 2024-04-11 03:10:41.293175 protein_turnover-0.3.8/protein_turnover/pepxml_ui.py
+-rw-r--r--   0        0        0    18499 2023-10-31 22:36:18.510700 protein_turnover-0.3.8/protein_turnover/plotting.py
+-rw-r--r--   0        0        0     3817 2024-02-06 08:48:02.313547 protein_turnover-0.3.8/protein_turnover/protxml.py
+-rw-r--r--   0        0        0        0 2023-08-29 04:01:11.951477 protein_turnover-0.3.8/protein_turnover/py.typed
+-rw-r--r--   0        0        0    26888 2024-04-26 00:23:46.745567 protein_turnover-0.3.8/protein_turnover/pymz.py
+-rw-r--r--   0        0        0    10050 2024-04-24 05:27:48.262533 protein_turnover-0.3.8/protein_turnover/pymz_ui.py
+-rw-r--r--   0        0        0     2571 2023-09-01 03:32:11.939419 protein_turnover-0.3.8/protein_turnover/settings.py
+-rw-r--r--   0        0        0     2726 2023-11-05 07:06:29.593017 protein_turnover-0.3.8/protein_turnover/sns.py
+-rw-r--r--   0        0        0        0 2022-11-02 03:43:40.908584 protein_turnover-0.3.8/protein_turnover/sqla/__init__.py
+-rw-r--r--   0        0        0     4791 2024-04-02 05:33:08.127208 protein_turnover-0.3.8/protein_turnover/sqla/iso_peaks.py
+-rw-r--r--   0        0        0     3982 2024-04-12 09:19:03.622817 protein_turnover-0.3.8/protein_turnover/sqla/iso_peaks_ui.py
+-rw-r--r--   0        0        0    12901 2024-04-11 04:06:36.929908 protein_turnover-0.3.8/protein_turnover/sqla/model.py
+-rw-r--r--   0        0        0    20036 2024-04-10 06:44:53.511669 protein_turnover-0.3.8/protein_turnover/sqla/query.py
+-rw-r--r--   0        0        0     5249 2024-02-14 07:30:52.792197 protein_turnover-0.3.8/protein_turnover/sqla/utils.py
+-rw-r--r--   0        0        0        0 2022-09-06 02:29:35.846848 protein_turnover-0.3.8/protein_turnover/types/__init__.py
+-rw-r--r--   0        0        0     7955 2023-11-03 02:17:35.435401 protein_turnover-0.3.8/protein_turnover/types/checking.py
+-rw-r--r--   0        0        0      956 2023-08-28 10:18:07.838829 protein_turnover-0.3.8/protein_turnover/types/mzmltypes.py
+-rw-r--r--   0        0        0     1874 2023-08-28 10:18:07.806829 protein_turnover-0.3.8/protein_turnover/types/pepxmltypes.py
+-rw-r--r--   0        0        0     2594 2023-08-28 10:18:07.838829 protein_turnover-0.3.8/protein_turnover/types/turnovertype.py
+-rw-r--r--   0        0        0     7509 2023-11-05 22:47:34.227461 protein_turnover-0.3.8/protein_turnover/unimod.py
+-rw-r--r--   0        0        0    20458 2024-04-18 12:12:35.320150 protein_turnover-0.3.8/protein_turnover/utils.py
+-rw-r--r--   0        0        0     5798 2024-04-15 04:58:55.719116 protein_turnover-0.3.8/protein_turnover/web.py
+-rw-r--r--   0        0        0     2614 2024-04-15 08:27:59.960224 protein_turnover-0.3.8/protein_turnover/web_ui.py
+-rw-r--r--   0        0        0     1154 2024-04-26 05:23:56.101740 protein_turnover-0.3.8/pyproject.toml
+-rw-r--r--   0        0        0     1381 1970-01-01 00:00:00.000000 protein_turnover-0.3.8/PKG-INFO
```

### Comparing `protein_turnover-0.3.7/LICENSE` & `protein_turnover-0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/background.py` & `protein_turnover-0.3.8/protein_turnover/background.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/background_ui.py` & `protein_turnover-0.3.8/protein_turnover/background_ui.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/broken_api.py` & `protein_turnover-0.3.8/protein_turnover/broken_api.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/cli.py` & `protein_turnover-0.3.8/protein_turnover/cli.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/config.py` & `protein_turnover-0.3.8/protein_turnover/config.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/dinosaur/cmd.py` & `protein_turnover-0.3.8/protein_turnover/dinosaur/cmd.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/dinosaur/dinosaur.py` & `protein_turnover-0.3.8/protein_turnover/dinosaur/dinosaur.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/filters.py` & `protein_turnover-0.3.8/protein_turnover/filters.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/fitenvelopes.py` & `protein_turnover-0.3.8/protein_turnover/fitenvelopes.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/jobs.py` & `protein_turnover-0.3.8/protein_turnover/jobs.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/logger.py` & `protein_turnover-0.3.8/protein_turnover/logger.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/mailer.py` & `protein_turnover-0.3.8/protein_turnover/mailer.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/parallel_utils.py` & `protein_turnover-0.3.8/protein_turnover/parallel_utils.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/pepxml.py` & `protein_turnover-0.3.8/protein_turnover/pepxml.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/pepxml_reader.py` & `protein_turnover-0.3.8/protein_turnover/pepxml_reader.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/pepxml_ui.py` & `protein_turnover-0.3.8/protein_turnover/pepxml_ui.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/plotting.py` & `protein_turnover-0.3.8/protein_turnover/plotting.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/protxml.py` & `protein_turnover-0.3.8/protein_turnover/protxml.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/pymz.py` & `protein_turnover-0.3.8/protein_turnover/pymz.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/pymz_ui.py` & `protein_turnover-0.3.8/protein_turnover/pymz_ui.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/settings.py` & `protein_turnover-0.3.8/protein_turnover/settings.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/sns.py` & `protein_turnover-0.3.8/protein_turnover/sns.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/sqla/iso_peaks.py` & `protein_turnover-0.3.8/protein_turnover/sqla/iso_peaks.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/sqla/iso_peaks_ui.py` & `protein_turnover-0.3.8/protein_turnover/sqla/iso_peaks_ui.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/sqla/model.py` & `protein_turnover-0.3.8/protein_turnover/sqla/model.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/sqla/query.py` & `protein_turnover-0.3.8/protein_turnover/sqla/query.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/sqla/utils.py` & `protein_turnover-0.3.8/protein_turnover/sqla/utils.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/types/checking.py` & `protein_turnover-0.3.8/protein_turnover/types/checking.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/types/mzmltypes.py` & `protein_turnover-0.3.8/protein_turnover/types/mzmltypes.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/types/pepxmltypes.py` & `protein_turnover-0.3.8/protein_turnover/types/pepxmltypes.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/types/turnovertype.py` & `protein_turnover-0.3.8/protein_turnover/types/turnovertype.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/unimod.py` & `protein_turnover-0.3.8/protein_turnover/unimod.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/utils.py` & `protein_turnover-0.3.8/protein_turnover/utils.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/web.py` & `protein_turnover-0.3.8/protein_turnover/web.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/protein_turnover/web_ui.py` & `protein_turnover-0.3.8/protein_turnover/web_ui.py`

 * *Files identical despite different names*

### Comparing `protein_turnover-0.3.7/pyproject.toml` & `protein_turnover-0.3.8/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 [tool.poetry]
 name = "protein-turnover"
-version = "0.3.7"
+version = "0.3.8"
 description = "protein turnover pipeline"
 authors = ["Ian Castleden <ian.castleden@uwa.edu.au>"]
 license = "MIT"
+readme = "prerelease.md"
 exclude = ["oldcode/**", "tests/**"]
 packages = [{ include = "protein_turnover" }]
 repository = "https://github.com/arabidopsis/protein_turnover.git"
 
 classifiers =[
     "Development Status :: 4 - Beta",
     "Intended Audience :: Science/Research",
```

### Comparing `protein_turnover-0.3.7/PKG-INFO` & `protein_turnover-0.3.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: protein-turnover
-Version: 0.3.7
+Version: 0.3.8
 Summary: protein turnover pipeline
 Home-page: https://github.com/arabidopsis/protein_turnover.git
 License: MIT
 Author: Ian Castleden
 Author-email: ian.castleden@uwa.edu.au
 Requires-Python: >=3.10
 Classifier: Development Status :: 4 - Beta
@@ -25,7 +25,13 @@
 Requires-Dist: pyarrow (>=15.0.0,<16.0.0)
 Requires-Dist: pymzml (>=2.5.2,<3.0.0)
 Requires-Dist: pyteomics (>=4.5.3,<5.0.0)
 Requires-Dist: scipy (>=1.8.1,<2.0.0)
 Requires-Dist: tomli (>=2.0.1,<3.0.0)
 Requires-Dist: tomli-w (>=1.0.0,<2.0.0)
 Project-URL: Repository, https://github.com/arabidopsis/protein_turnover.git
+Description-Content-Type: text/markdown
+
+# Protein Turnover Pipeline
+
+More documentation soon.
+
```

