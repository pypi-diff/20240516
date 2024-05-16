# Comparing `tmp/fintoolsap-1.7.2.tar.gz` & `tmp/fintoolsap-1.7.3.tar.gz`

## Comparing `fintoolsap-1.7.2.tar` & `fintoolsap-1.7.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/FinToolsAP.code-workspace
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/FinToolsAP.yaml
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/todo.txt
--rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/src/FinToolsAP/Decorators.py
--rw-r--r--   0        0        0    19279 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/src/FinToolsAP/LaTeXBuilder.py
--rw-r--r--   0        0        0    77642 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/src/FinToolsAP/LocalDatabase.py
--rw-r--r--   0        0        0    32188 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/src/FinToolsAP/PortfolioSorts.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/src/FinToolsAP/ResultsClasses.py
--rw-r--r--   0        0        0    51220 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/src/FinToolsAP/UtilityFunctions.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/src/FinToolsAP/__init__.py
--rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/src/FinToolsAP/_config.py
--rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/src/FinToolsAP/_download_script.py
--rw-r--r--   0        0        0     4420 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/src/FinToolsAP/_util_funcs.py
--rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/src/FinToolsAP/base_files/DatabaseParameters.py
--rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/src/FinToolsAP/base_files/ExampleCreateTable.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/src/FinToolsAP/base_files/ExampleExtraScript.py
--rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_BMME_sorts.py
--rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_Bond.py
--rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_DB_construction.py
--rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_FF_factors.py
--rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_bloom_cds.py
--rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_breakpoint_construction.py
--rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_create_all_factors.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_csv_import.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_csv_to_sql.py
--rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_dbp_file_print.py
--rw-r--r--   0        0        0    27112 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_martin_output.py
--rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_pca.py
--rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_query_BTDS.py
--rw-r--r--   0        0        0    30780 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_query_Bank.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_query_CRSP.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_query_CRSPMF.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_query_Factors.py
--rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_query_IBES.py
--rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_query_IH.py
--rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_query_MF.py
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_query_MFCH.py
--rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_query_MFHoldings.py
--rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_query_MFLinks.py
--rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_raw_query.py
--rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_score_characteristics.py
--rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_sorting.py
--rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_univariate_sorts.py
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/TEST_virtual_environment.py
--rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/test.py
--rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/tests/test_dbp.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/LICENSE
--rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/README.md
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/pyproject.toml
--rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 fintoolsap-1.7.2/PKG-INFO
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/FinToolsAP.code-workspace
+-rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/FinToolsAP.yaml
+-rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/todo.txt
+-rw-r--r--   0        0        0     3287 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/src/FinToolsAP/Decorators.py
+-rw-r--r--   0        0        0    19279 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/src/FinToolsAP/LaTeXBuilder.py
+-rw-r--r--   0        0        0    77593 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/src/FinToolsAP/LocalDatabase.py
+-rw-r--r--   0        0        0    32188 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/src/FinToolsAP/PortfolioSorts.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/src/FinToolsAP/ResultsClasses.py
+-rw-r--r--   0        0        0    51220 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/src/FinToolsAP/UtilityFunctions.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/src/FinToolsAP/__init__.py
+-rw-r--r--   0        0        0     8808 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/src/FinToolsAP/_config.py
+-rw-r--r--   0        0        0     1079 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/src/FinToolsAP/_download_script.py
+-rw-r--r--   0        0        0     6385 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/src/FinToolsAP/_util_funcs.py
+-rw-r--r--   0        0        0     2006 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/src/FinToolsAP/base_files/DatabaseParameters.py
+-rw-r--r--   0        0        0     3463 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/src/FinToolsAP/base_files/ExampleCreateTable.py
+-rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/src/FinToolsAP/base_files/ExampleExtraScript.py
+-rw-r--r--   0        0        0    11131 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_BMME_sorts.py
+-rw-r--r--   0        0        0      324 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_Bond.py
+-rw-r--r--   0        0        0      317 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_DB_construction.py
+-rw-r--r--   0        0        0     4890 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_FF_factors.py
+-rw-r--r--   0        0        0      964 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_bloom_cds.py
+-rw-r--r--   0        0        0     9352 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_breakpoint_construction.py
+-rw-r--r--   0        0        0     1303 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_create_all_factors.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_csv_import.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_csv_to_sql.py
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_dbp_file_print.py
+-rw-r--r--   0        0        0    27112 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_martin_output.py
+-rw-r--r--   0        0        0      856 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_pca.py
+-rw-r--r--   0        0        0     1155 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_query_BTDS.py
+-rw-r--r--   0        0        0    30780 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_query_Bank.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_query_CRSP.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_query_CRSPMF.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_query_Factors.py
+-rw-r--r--   0        0        0     2549 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_query_IBES.py
+-rw-r--r--   0        0        0     3056 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_query_IH.py
+-rw-r--r--   0        0        0     2510 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_query_MF.py
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_query_MFCH.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_query_MFHoldings.py
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_query_MFLinks.py
+-rw-r--r--   0        0        0     1314 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_raw_query.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_score_characteristics.py
+-rw-r--r--   0        0        0     5925 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_sorting.py
+-rw-r--r--   0        0        0    11343 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_univariate_sorts.py
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/TEST_virtual_environment.py
+-rw-r--r--   0        0        0      718 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/test.py
+-rw-r--r--   0        0        0      256 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/tests/test_dbp.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/LICENSE
+-rw-r--r--   0        0        0     3309 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/README.md
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/pyproject.toml
+-rw-r--r--   0        0        0     3887 2020-02-02 00:00:00.000000 fintoolsap-1.7.3/PKG-INFO
```

### Comparing `fintoolsap-1.7.2/src/FinToolsAP/Decorators.py` & `fintoolsap-1.7.3/src/FinToolsAP/Decorators.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/src/FinToolsAP/LaTeXBuilder.py` & `fintoolsap-1.7.3/src/FinToolsAP/LaTeXBuilder.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/src/FinToolsAP/LocalDatabase.py` & `fintoolsap-1.7.3/src/FinToolsAP/LocalDatabase.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,18 +63,14 @@
 import itertools
 import sqlalchemy
 import connectorx
 import subprocess
 import importlib.util
 import pandas.tseries.offsets
 
-# custom imports 
-import UtilityFunctions
-
-
 # Testing Flags
 
 # used to ignore a table when testing initialization of the database
 # the data is never deleted from disk but the database will believe its
 # missing
 TESTING_FLAGS = {}
 
@@ -324,15 +320,15 @@
                 tables_added.append(table)
                 self.db_modified = True
 
         # ---------------------------------------------------
                 
         ### 2. Load tables from file in Database/FILEtoDB
         added_files_to_db_flag = False
-        FILEStoDB_contents = UtilityFunctions.list_dir(self._path_to_files_to_load)
+        FILEStoDB_contents = _util_funcs.list_dir(self._path_to_files_to_load)
         FILEStoDB_contents = [f[:-4] for f in FILEStoDB_contents] # remove extension
         for table in self.DBP.Tables.FILES_TABLES:
             if(table not in self.curr_tables):
 
                 if(table not in FILEStoDB_contents):
                     print(_config.Messages.NO_DATA_FILE.format(color = _config.bcolors.WARNING,
                                                                tab = table
```

### Comparing `fintoolsap-1.7.2/src/FinToolsAP/PortfolioSorts.py` & `fintoolsap-1.7.3/src/FinToolsAP/PortfolioSorts.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/src/FinToolsAP/UtilityFunctions.py` & `fintoolsap-1.7.3/src/FinToolsAP/UtilityFunctions.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/src/FinToolsAP/_config.py` & `fintoolsap-1.7.3/src/FinToolsAP/_config.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/src/FinToolsAP/_download_script.py` & `fintoolsap-1.7.3/src/FinToolsAP/_download_script.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/src/FinToolsAP/base_files/DatabaseParameters.py` & `fintoolsap-1.7.3/src/FinToolsAP/base_files/DatabaseParameters.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/src/FinToolsAP/base_files/ExampleCreateTable.py` & `fintoolsap-1.7.3/src/FinToolsAP/base_files/ExampleCreateTable.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/src/FinToolsAP/base_files/ExampleExtraScript.py` & `fintoolsap-1.7.3/src/FinToolsAP/base_files/ExampleExtraScript.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_BMME_sorts.py` & `fintoolsap-1.7.3/tests/TEST_BMME_sorts.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_FF_factors.py` & `fintoolsap-1.7.3/tests/TEST_FF_factors.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_bloom_cds.py` & `fintoolsap-1.7.3/tests/TEST_bloom_cds.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_breakpoint_construction.py` & `fintoolsap-1.7.3/tests/TEST_breakpoint_construction.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_create_all_factors.py` & `fintoolsap-1.7.3/tests/TEST_create_all_factors.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_csv_import.py` & `fintoolsap-1.7.3/tests/TEST_csv_import.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_csv_to_sql.py` & `fintoolsap-1.7.3/tests/TEST_csv_to_sql.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_dbp_file_print.py` & `fintoolsap-1.7.3/tests/TEST_dbp_file_print.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_martin_output.py` & `fintoolsap-1.7.3/tests/TEST_martin_output.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_pca.py` & `fintoolsap-1.7.3/tests/TEST_pca.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_query_BTDS.py` & `fintoolsap-1.7.3/tests/TEST_query_BTDS.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_query_Bank.py` & `fintoolsap-1.7.3/tests/TEST_query_Bank.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_query_CRSP.py` & `fintoolsap-1.7.3/tests/TEST_query_CRSP.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_query_CRSPMF.py` & `fintoolsap-1.7.3/tests/TEST_query_CRSPMF.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_query_Factors.py` & `fintoolsap-1.7.3/tests/TEST_query_Factors.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_query_IBES.py` & `fintoolsap-1.7.3/tests/TEST_query_IBES.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_query_IH.py` & `fintoolsap-1.7.3/tests/TEST_query_IH.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_query_MF.py` & `fintoolsap-1.7.3/tests/TEST_query_MF.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_query_MFCH.py` & `fintoolsap-1.7.3/tests/TEST_query_MFCH.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_query_MFHoldings.py` & `fintoolsap-1.7.3/tests/TEST_query_MFHoldings.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_query_MFLinks.py` & `fintoolsap-1.7.3/tests/TEST_query_MFLinks.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_raw_query.py` & `fintoolsap-1.7.3/tests/TEST_raw_query.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_score_characteristics.py` & `fintoolsap-1.7.3/tests/TEST_score_characteristics.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_sorting.py` & `fintoolsap-1.7.3/tests/TEST_sorting.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_univariate_sorts.py` & `fintoolsap-1.7.3/tests/TEST_univariate_sorts.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/TEST_virtual_environment.py` & `fintoolsap-1.7.3/tests/TEST_virtual_environment.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/tests/test.py` & `fintoolsap-1.7.3/tests/test.py`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/LICENSE` & `fintoolsap-1.7.3/LICENSE`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/README.md` & `fintoolsap-1.7.3/README.md`

 * *Files identical despite different names*

### Comparing `fintoolsap-1.7.2/pyproject.toml` & `fintoolsap-1.7.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "FinToolsAP"
-version = "1.7.2"
+version = "1.7.3"
 authors = [
   { name="Andrew Maurice Perry", email="andrewpe@berkeley.edu" },
 ]
 description = "Package that includes many tools commonly used in finance. Also includes a local database."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
```

### Comparing `fintoolsap-1.7.2/PKG-INFO` & `fintoolsap-1.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: FinToolsAP
-Version: 1.7.2
+Version: 1.7.3
 Summary: Package that includes many tools commonly used in finance. Also includes a local database.
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Author-email: Andrew Maurice Perry <andrewpe@berkeley.edu>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

