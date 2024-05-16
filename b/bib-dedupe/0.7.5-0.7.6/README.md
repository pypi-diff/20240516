# Comparing `tmp/bib_dedupe-0.7.5.tar.gz` & `tmp/bib_dedupe-0.7.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bib_dedupe-0.7.5.tar", max compression
+gzip compressed data, was "bib_dedupe-0.7.6.tar", max compression
```

## Comparing `bib_dedupe-0.7.5.tar` & `bib_dedupe-0.7.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1070 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/LICENSE
--rw-r--r--   0        0        0     3867 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/README.md
--rw-r--r--   0        0        0      411 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/__init__.py
--rw-r--r--   0        0        0     6496 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/bib_dedupe.py
--rw-r--r--   0        0        0     8465 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/block.py
--rw-r--r--   0        0        0      269 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/cli.py
--rw-r--r--   0        0        0     2795 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/cluster.py
--rw-r--r--   0        0        0      253 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/constants/__init__.py
--rw-r--r--   0        0        0      191 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/constants/colors.py
--rw-r--r--   0        0        0      490 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/constants/entrytypes.py
--rw-r--r--   0        0        0     1033 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/constants/fields.py
--rw-r--r--   0        0        0     2212 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/debug.py
--rw-r--r--   0        0        0    19504 2024-05-07 10:50:56.598713 bib_dedupe-0.7.5/bib_dedupe/dedupe_benchmark.py
--rw-r--r--   0        0        0   109747 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/journal_variants.csv
--rw-r--r--   0        0        0     5852 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/match.py
--rw-r--r--   0        0        0     5683 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/match_conditions.py
--rw-r--r--   0        0        0     5789 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/maybe_cases.py
--rw-r--r--   0        0        0     7871 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/merge.py
--rw-r--r--   0        0        0     7191 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep.py
--rw-r--r--   0        0        0     2071 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_abstract.py
--rw-r--r--   0        0        0     9428 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_author.py
--rw-r--r--   0        0        0     5719 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_container_title.py
--rw-r--r--   0        0        0     1220 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_doi.py
--rw-r--r--   0        0        0      817 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_number.py
--rw-r--r--   0        0        0     2516 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_pages.py
--rw-r--r--   0        0        0     5010 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_title.py
--rw-r--r--   0        0        0     1374 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_volume.py
--rw-r--r--   0        0        0      573 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/prep_year.py
--rw-r--r--   0        0        0    15071 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/sim.py
--rw-r--r--   0        0        0      836 2024-05-07 10:50:56.602713 bib_dedupe-0.7.5/bib_dedupe/util.py
--rw-r--r--   0        0        0     2230 2024-05-07 10:50:57.746723 bib_dedupe-0.7.5/pyproject.toml
--rw-r--r--   0        0        0     5604 1970-01-01 00:00:00.000000 bib_dedupe-0.7.5/PKG-INFO
+-rw-r--r--   0        0        0     1070 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/LICENSE
+-rw-r--r--   0        0        0     3867 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/README.md
+-rw-r--r--   0        0        0      411 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/__init__.py
+-rw-r--r--   0        0        0     6496 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/bib_dedupe.py
+-rw-r--r--   0        0        0     8465 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/block.py
+-rw-r--r--   0        0        0      269 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/cli.py
+-rw-r--r--   0        0        0     2795 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/cluster.py
+-rw-r--r--   0        0        0      253 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/constants/__init__.py
+-rw-r--r--   0        0        0      191 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/constants/colors.py
+-rw-r--r--   0        0        0      490 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/constants/entrytypes.py
+-rw-r--r--   0        0        0     1033 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/constants/fields.py
+-rw-r--r--   0        0        0     2212 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/debug.py
+-rw-r--r--   0        0        0    19504 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/dedupe_benchmark.py
+-rw-r--r--   0        0        0   109747 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/journal_variants.csv
+-rw-r--r--   0        0        0     5852 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/match.py
+-rw-r--r--   0        0        0     5683 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/match_conditions.py
+-rw-r--r--   0        0        0     5789 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/maybe_cases.py
+-rw-r--r--   0        0        0     7871 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/merge.py
+-rw-r--r--   0        0        0     7189 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/prep.py
+-rw-r--r--   0        0        0     2071 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/prep_abstract.py
+-rw-r--r--   0        0        0     9428 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/prep_author.py
+-rw-r--r--   0        0        0     5719 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/prep_container_title.py
+-rw-r--r--   0        0        0     1220 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/prep_doi.py
+-rw-r--r--   0        0        0      817 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/prep_number.py
+-rw-r--r--   0        0        0     2516 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/prep_pages.py
+-rw-r--r--   0        0        0     5010 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/prep_title.py
+-rw-r--r--   0        0        0     1374 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/prep_volume.py
+-rw-r--r--   0        0        0      573 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/prep_year.py
+-rw-r--r--   0        0        0    15071 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/sim.py
+-rw-r--r--   0        0        0      836 2024-05-16 15:17:10.479834 bib_dedupe-0.7.6/bib_dedupe/util.py
+-rw-r--r--   0        0        0     2230 2024-05-16 15:17:11.627839 bib_dedupe-0.7.6/pyproject.toml
+-rw-r--r--   0        0        0     5604 1970-01-01 00:00:00.000000 bib_dedupe-0.7.6/PKG-INFO
```

### Comparing `bib_dedupe-0.7.5/LICENSE` & `bib_dedupe-0.7.6/LICENSE`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/README.md` & `bib_dedupe-0.7.6/README.md`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/bib_dedupe.py` & `bib_dedupe-0.7.6/bib_dedupe/bib_dedupe.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/block.py` & `bib_dedupe-0.7.6/bib_dedupe/block.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/cluster.py` & `bib_dedupe-0.7.6/bib_dedupe/cluster.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/constants/fields.py` & `bib_dedupe-0.7.6/bib_dedupe/constants/fields.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/debug.py` & `bib_dedupe-0.7.6/bib_dedupe/debug.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/dedupe_benchmark.py` & `bib_dedupe-0.7.6/bib_dedupe/dedupe_benchmark.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/journal_variants.csv` & `bib_dedupe-0.7.6/bib_dedupe/journal_variants.csv`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/match.py` & `bib_dedupe-0.7.6/bib_dedupe/match.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/match_conditions.py` & `bib_dedupe-0.7.6/bib_dedupe/match_conditions.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/maybe_cases.py` & `bib_dedupe-0.7.6/bib_dedupe/maybe_cases.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/merge.py` & `bib_dedupe-0.7.6/bib_dedupe/merge.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/prep.py` & `bib_dedupe-0.7.6/bib_dedupe/prep.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,14 +119,16 @@
     Returns:
         The prepared dataframe.
     """
     records_df = records_df.copy()
 
     if ID not in records_df.columns:
         records_df.loc[:, ID] = range(1, len(records_df) + 1)
+    if not records_df[ID].is_unique:
+        raise ValueError("ID column in records_df must be unique.")
 
     if ENTRYTYPE not in records_df.columns:
         records_df[ENTRYTYPE] = "article"
 
     missing_fields = [f for f in REQUIRED_FIELDS if f not in records_df.columns]
     assert len(missing_fields) == 0, f"Missing required fields: {missing_fields}"
 
@@ -191,16 +193,14 @@
     Args:
         records_df: The records dataframe.
         cpu: The number of CPUs to use. If -1, use all available CPUs.
 
     Returns:
         The prepared records dataframe.
     """
-    if not records_df["ID"].is_unique:
-        raise ValueError("ID column in records_df must be unique.")
 
     now = datetime.now().strftime("%Y-%m-%d %H:%M:%S")
     verbose_print.print(f"Loaded {records_df.shape[0]:,} records")
     verbose_print.print(f"Prep started at {now}")
     start_time = time.time()
 
     if 0 == records_df.shape[0]:
```

### Comparing `bib_dedupe-0.7.5/bib_dedupe/prep_abstract.py` & `bib_dedupe-0.7.6/bib_dedupe/prep_abstract.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/prep_author.py` & `bib_dedupe-0.7.6/bib_dedupe/prep_author.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/prep_container_title.py` & `bib_dedupe-0.7.6/bib_dedupe/prep_container_title.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/prep_doi.py` & `bib_dedupe-0.7.6/bib_dedupe/prep_doi.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/prep_number.py` & `bib_dedupe-0.7.6/bib_dedupe/prep_number.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/prep_pages.py` & `bib_dedupe-0.7.6/bib_dedupe/prep_pages.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/prep_title.py` & `bib_dedupe-0.7.6/bib_dedupe/prep_title.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/prep_volume.py` & `bib_dedupe-0.7.6/bib_dedupe/prep_volume.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/prep_year.py` & `bib_dedupe-0.7.6/bib_dedupe/prep_year.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/sim.py` & `bib_dedupe-0.7.6/bib_dedupe/sim.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/bib_dedupe/util.py` & `bib_dedupe-0.7.6/bib_dedupe/util.py`

 * *Files identical despite different names*

### Comparing `bib_dedupe-0.7.5/pyproject.toml` & `bib_dedupe-0.7.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "bib-dedupe"
-version = "0.7.5"
+version = "0.7.6"
 description = "Identify and merge duplicates in bibliographic records"
 authors = ["Gerit Wagner <gerit.wagner@uni-bamberg.de>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/CoLRev-Environment/bib-dedupe"
 documentation = "https://colrev-environment.github.io/bib-dedupe/"
 keywords = ["de-duplication", "duplicate", "meta-analysis", "research", "reproducible research", "open science", "literature", "literature review", "systematic review", "systematic literature review"]
```

### Comparing `bib_dedupe-0.7.5/PKG-INFO` & `bib_dedupe-0.7.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bib-dedupe
-Version: 0.7.5
+Version: 0.7.6
 Summary: Identify and merge duplicates in bibliographic records
 Home-page: https://github.com/CoLRev-Environment/bib-dedupe
 License: MIT
 Keywords: de-duplication,duplicate,meta-analysis,research,reproducible research,open science,literature,literature review,systematic review,systematic literature review
 Author: Gerit Wagner
 Author-email: gerit.wagner@uni-bamberg.de
 Requires-Python: >=3.9,<4.0
```

