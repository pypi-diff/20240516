# Comparing `tmp/imsciences-0.5.6.1.tar.gz` & `tmp/imsciences-0.5.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.6.1.tar", last modified: Thu May 16 11:38:30 2024, max compression
+gzip compressed data, was "imsciences-0.5.6.2.tar", last modified: Thu May 16 12:54:21 2024, max compression
```

## Comparing `imsciences-0.5.6.1.tar` & `imsciences-0.5.6.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 11:38:30.339733 imsciences-0.5.6.1/
--rw-rw-rw-   0        0        0     9757 2024-05-16 11:38:30.336746 imsciences-0.5.6.1/PKG-INFO
--rw-rw-rw-   0        0        0     9252 2024-05-16 11:38:25.000000 imsciences-0.5.6.1/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 11:38:30.312074 imsciences-0.5.6.1/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.6.1/imsciences/__init__.py
--rw-rw-rw-   0        0        0    65522 2024-05-16 11:36:52.000000 imsciences-0.5.6.1/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-16 11:38:30.332696 imsciences-0.5.6.1/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9757 2024-05-16 11:38:30.000000 imsciences-0.5.6.1/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-16 11:38:30.000000 imsciences-0.5.6.1/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 11:38:30.000000 imsciences-0.5.6.1/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 11:38:30.000000 imsciences-0.5.6.1/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 11:38:30.000000 imsciences-0.5.6.1/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 11:38:30.339733 imsciences-0.5.6.1/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-16 11:38:23.000000 imsciences-0.5.6.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:54:21.437730 imsciences-0.5.6.2/
+-rw-rw-rw-   0        0        0     9757 2024-05-16 12:54:21.434729 imsciences-0.5.6.2/PKG-INFO
+-rw-rw-rw-   0        0        0     9252 2024-05-16 11:38:25.000000 imsciences-0.5.6.2/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 12:54:21.401003 imsciences-0.5.6.2/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.6.2/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    65305 2024-05-16 12:52:34.000000 imsciences-0.5.6.2/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 12:54:21.431090 imsciences-0.5.6.2/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9757 2024-05-16 12:54:21.000000 imsciences-0.5.6.2/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-16 12:54:21.000000 imsciences-0.5.6.2/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 12:54:21.000000 imsciences-0.5.6.2/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 12:54:21.000000 imsciences-0.5.6.2/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 12:54:21.000000 imsciences-0.5.6.2/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 12:54:21.437730 imsciences-0.5.6.2/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-16 12:53:41.000000 imsciences-0.5.6.2/setup.py
```

### Comparing `imsciences-0.5.6.1/PKG-INFO` & `imsciences-0.5.6.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.6.1
+Version: 0.5.6.2
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.6.1/README.md` & `imsciences-0.5.6.2/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.6.1/imsciences/datafunctions.py` & `imsciences-0.5.6.2/imsciences/datafunctions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 import pandas as pd
 import calendar
 import os
 import plotly.express as px
 import plotly.graph_objs as go
-from dateutil.parser import parse
 import numpy as np
-from datetime import datetime
 import datetime
 import re
-from datetime import datetime, timedelta
 import pandas as pd
-from datetime import datetime
 from imsciences import *
 from fredapi import Fred
-import pandas as pd
-import datetime
-from datetime import timedelta
 import time
 
 class dataprocessing:
     
     def help(self):
         print("This is the help section. The functions in the package are as follows:")
 
@@ -408,38 +401,38 @@
                 rangemode='tozero'  # Setting Y-axis to start at 0 if suitable
             )
         )
 
         return fig
 
     def week_of_year_mapping(self, df, week_col, start_day_str):
-        from datetime import datetime, timedelta
+
         # Mapping of string day names to day numbers (1 for Monday, 7 for Sunday)
         day_mapping = {
             'mon': 1, 'tue': 2, 'wed': 3, 'thu': 4, 'fri': 5, 'sat': 6, 'sun': 7
         }
 
         # Convert the day string to a number, or raise an error if not valid
         start_day = day_mapping.get(start_day_str.lower())
         if start_day is None:
             raise ValueError(f"Invalid day input: '{start_day_str}'. Please use one of 'mon', 'tue', 'wed', 'thu', 'fri', 'sat', 'sun'.")
 
         # Function to convert week number to start date of the week
         def week_to_startdate(week_str, start_day):
             year, week = map(int, week_str.split('-W'))
-            first_day_of_year = datetime(year, 1, 1)
+            first_day_of_year = datetime.datetime(year, 1, 1)
             day_of_week = first_day_of_year.isocalendar()[2]
             days_to_add = (7 - day_of_week + 1) if day_of_week > 4 else (1 - day_of_week)
-            start_of_iso_week = first_day_of_year + timedelta(days=days_to_add)
+            start_of_iso_week = first_day_of_year + datetime.timedelta(days=days_to_add)
 
             # Adjust start day
             days_to_shift = (start_day - 1) % 7
-            start_of_week = start_of_iso_week + timedelta(days=days_to_shift)
+            start_of_week = start_of_iso_week + datetime.timedelta(days=days_to_shift)
 
-            return start_of_week + timedelta(weeks=week - 1)
+            return start_of_week + datetime.timedelta(weeks=week - 1)
 
         # Apply the function to each row in the specified week column
         df['OBS'] = df[week_col].apply(lambda x: week_to_startdate(x, start_day)).dt.strftime('%d/%m/%Y')
         return df
     
     def exclude_rows(self, df, col_to_filter, list_of_filters):
         # This line filters the DataFrame based on whether the values in the specified column are not in the list_of_filters
@@ -566,15 +559,15 @@
 
         # Handle null values (optional, can be adjusted as needed)
         merged_df.fillna(0, inplace=True)
 
         return merged_df
     
     def convert_us_to_uk_dates(self, df, date_col):
-        import datetime
+
         def fix_date(d):
             # Convert datetime objects to string
             if isinstance(d, pd.Timestamp) or isinstance(d, datetime.datetime):
                 d = d.strftime('%m/%d/%Y')
             
             # Split date string into components
             parts = d.split('/')
@@ -867,15 +860,15 @@
         combined_FY_and_H (str, optional): String used to specify is a combined half year and FY column is desired. Defaults to "No".
 
         Returns:
         pandas.DataFrame: DataFrame with a new column 'FY' containing the FY as well as, if desired, a half year column and a combined FY half year column.
         """
         
         try:
-            start_date = datetime.strptime(start_date, '%Y-%m-%d')
+            start_date = datetime.datetime.strptime(start_date, '%Y-%m-%d')
         except ValueError:
             print("Error: Date must be of format yyyy-mm-dd")
             return df
         
         df["OBS"] = pd.to_datetime(df[index_col])
         df["OBS as string"] = df["OBS"].dt.strftime("%Y-%m-%d")
 
@@ -1160,15 +1153,15 @@
         # Fetch the metadata for each series to get the full names
         series_names = {series_id: fred.get_series_info(series_id).title for series_id in series_id_list}
 
         # Download data from series id list
         fred_series = {series_id: fred.get_series(series_id) for series_id in series_id_list}
 
         # Data processing
-        date_range = {'OBS': pd.date_range("1950-01-01", datetime.today().strftime('%Y-%m-%d'), freq='d')}
+        date_range = {'OBS': pd.date_range("1950-01-01", datetime.datetime.today().strftime('%Y-%m-%d'), freq='d')}
         fred_series_df = pd.DataFrame(date_range)
 
         for series_id, series_data in fred_series.items():
             series_data = series_data.reset_index()
             series_data.columns = ['OBS', series_names[series_id]]  # Use the series name as the column header
             fred_series_df = pd.merge_asof(fred_series_df, series_data, on='OBS', direction='backward')
 
@@ -1220,15 +1213,15 @@
         df.rename(columns={"Date Changed": "OBS", "Rate": "macro_boe_intr_rate"}, inplace=True)
         
         # Change date column to datetime and find the corresponding week to the date
         df["OBS"] = pd.to_datetime(df["OBS"], format="%d %b %y")
         df.sort_values("OBS", axis=0, inplace=True)
         
         # Create a daily date range and find the week commencing for that day
-        date_range = pd.date_range(df["OBS"].iloc[0], datetime.date.today(), freq="d")
+        date_range = pd.date_range(df["OBS"].iloc[0], datetime.datetime.date.today(), freq="d")
         df_daily = pd.DataFrame(date_range, columns=["OBS"])
         
         # Find the start of the week for each day
         df_daily['OBS'] = df_daily["OBS"].apply(lambda x: x - pd.Timedelta(days=(x.weekday() - day_dict[week_commencing]) % 7))
         
         # Outer merge the daily date range on the boe dataframe and forward fill in the blanks
         df_final = df_daily.merge(df, on='OBS', how="left")
```

### Comparing `imsciences-0.5.6.1/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.6.2/imsciences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.6.1
+Version: 0.5.6.2
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.6.1/setup.py` & `imsciences-0.5.6.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.6.1'
+VERSION = '0.5.6.2'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

