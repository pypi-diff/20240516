# Comparing `tmp/imsciences-0.5.6.4.tar.gz` & `tmp/imsciences-0.5.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.6.4.tar", last modified: Thu May 16 18:38:05 2024, max compression
+gzip compressed data, was "imsciences-0.5.6.5.tar", last modified: Thu May 16 18:44:36 2024, max compression
```

## Comparing `imsciences-0.5.6.4.tar` & `imsciences-0.5.6.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 18:38:05.015606 imsciences-0.5.6.4/
--rw-rw-rw-   0        0        0     9757 2024-05-16 18:38:05.010823 imsciences-0.5.6.4/PKG-INFO
--rw-rw-rw-   0        0        0     9252 2024-05-16 11:38:25.000000 imsciences-0.5.6.4/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 18:38:04.975458 imsciences-0.5.6.4/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.6.4/imsciences/__init__.py
--rw-rw-rw-   0        0        0    79221 2024-05-16 18:37:35.000000 imsciences-0.5.6.4/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:38:05.007674 imsciences-0.5.6.4/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9757 2024-05-16 18:38:04.000000 imsciences-0.5.6.4/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-16 18:38:04.000000 imsciences-0.5.6.4/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 18:38:04.000000 imsciences-0.5.6.4/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 18:38:04.000000 imsciences-0.5.6.4/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 18:38:04.000000 imsciences-0.5.6.4/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 18:38:05.015606 imsciences-0.5.6.4/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-16 18:37:50.000000 imsciences-0.5.6.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:44:36.143924 imsciences-0.5.6.5/
+-rw-rw-rw-   0        0        0     9757 2024-05-16 18:44:36.137928 imsciences-0.5.6.5/PKG-INFO
+-rw-rw-rw-   0        0        0     9252 2024-05-16 11:38:25.000000 imsciences-0.5.6.5/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 18:44:36.096930 imsciences-0.5.6.5/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.6.5/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    79375 2024-05-16 18:44:21.000000 imsciences-0.5.6.5/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:44:36.134925 imsciences-0.5.6.5/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9757 2024-05-16 18:44:35.000000 imsciences-0.5.6.5/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-16 18:44:35.000000 imsciences-0.5.6.5/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 18:44:35.000000 imsciences-0.5.6.5/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 18:44:35.000000 imsciences-0.5.6.5/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 18:44:35.000000 imsciences-0.5.6.5/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 18:44:36.144932 imsciences-0.5.6.5/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-16 18:43:55.000000 imsciences-0.5.6.5/setup.py
```

### Comparing `imsciences-0.5.6.4/PKG-INFO` & `imsciences-0.5.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.6.4
+Version: 0.5.6.5
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.6.4/README.md` & `imsciences-0.5.6.5/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.6.4/imsciences/datafunctions.py` & `imsciences-0.5.6.5/imsciences/datafunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import requests
 import os
 import plotly.express as px
 import plotly.graph_objs as go
 import numpy as np
 import datetime
 import re
+import warnings
 import pandas as pd
 from imsciences import *
 from fredapi import Fred
 import time
 
 class dataprocessing:
     
@@ -277,56 +278,60 @@
             grouped = df_copy.groupby(['week_start'] + group_columns)[sum_columns].sum().reset_index()
 
         # Rename 'week_start' column to 'OBS'
         grouped = grouped.rename(columns={'week_start': 'OBS'})
 
         return grouped
     
-    def convert_monthly_to_daily(self, df, date_column, divide=True):
+    def convert_monthly_to_daily(df, date_column, divide=True):
         """
         Convert a DataFrame with monthly data to daily data.
         This function takes a DataFrame and a date column, then it expands each
         monthly record into daily records by dividing the numeric values by the number of days in that month.
 
         :param df: DataFrame with monthly data.
         :param date_column: The name of the column containing the date.
         :param divide: boolean divide by the number of days in a month (default True)
         :return: A new DataFrame with daily data.
         """
 
-        # Convert date_column to datetime with explicit format
-        df[date_column] = pd.to_datetime(df[date_column], format='%d/%m/%Y')
+        # Suppress warnings
+        with warnings.catch_warnings():
+            warnings.simplefilter("ignore")
+
+            # Convert date_column to datetime
+            df[date_column] = pd.to_datetime(df[date_column])
+
+            # Initialize an empty list to hold the daily records
+            daily_records = []
+
+            # Iterate over each row in the DataFrame
+            for _, row in df.iterrows():
+                # Calculate the number of days in the month
+                num_days = calendar.monthrange(row[date_column].year, row[date_column].month)[1]
+
+                # Create a new record for each day of the month
+                for day in range(1, num_days + 1):
+                    daily_row = row.copy()
+                    daily_row[date_column] = row[date_column].replace(day=day)
+
+                    # Divide each numeric value by the number of days in the month
+                    for col in df.columns:
+                        if pd.api.types.is_numeric_dtype(df[col]) and col != date_column:
+                            if divide:
+                                daily_row[col] = row[col] / num_days
+                            else: 
+                                daily_row[col] = row[col]
+                    daily_records.append(daily_row)
 
-        # Initialize an empty list to hold the daily records
-        daily_records = []
+            # Convert the list of daily records into a DataFrame
+            daily_df = pd.DataFrame(daily_records)
 
-        # Iterate over each row in the DataFrame
-        for _, row in df.iterrows():
-            # Calculate the number of days in the month
-            num_days = calendar.monthrange(row[date_column].year, row[date_column].month)[1]
-
-            # Create a new record for each day of the month
-            for day in range(1, num_days + 1):
-                daily_row = row.copy()
-                daily_row[date_column] = row[date_column].replace(day=day)
-
-                # Divide each numeric value by the number of days in the month if divide is True
-                for col in df.columns:
-                    if pd.api.types.is_numeric_dtype(df[col]) and col != date_column:
-                        if divide:
-                            daily_row[col] = row[col] / num_days
-                        else: 
-                            daily_row[col] = row[col]
-                daily_records.append(daily_row)
-
-        # Convert the list of daily records into a DataFrame
-        daily_df = pd.DataFrame(daily_records)
-        
         return daily_df
-    
+        
     def plot_two(self, df1, col1, df2, col2, date_column, same_axis=True):
         """
         Plots specified columns from two different dataframes with both different and the same lengths,
         using a specified date column as the X-axis, and charting on either the same or separate y axes.
 
         :param df1: First DataFrame
         :param col1: Column name from the first DataFrame
```

### Comparing `imsciences-0.5.6.4/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.6.5/imsciences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.6.4
+Version: 0.5.6.5
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.6.4/setup.py` & `imsciences-0.5.6.5/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.6.4'
+VERSION = '0.5.6.5'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

