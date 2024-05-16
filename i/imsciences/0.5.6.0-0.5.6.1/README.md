# Comparing `tmp/imsciences-0.5.6.0.tar.gz` & `tmp/imsciences-0.5.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.6.0.tar", last modified: Wed May 15 17:36:41 2024, max compression
+gzip compressed data, was "imsciences-0.5.6.1.tar", last modified: Thu May 16 11:38:30 2024, max compression
```

## Comparing `imsciences-0.5.6.0.tar` & `imsciences-0.5.6.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 17:36:41.268648 imsciences-0.5.6.0/
--rw-rw-rw-   0        0        0     9470 2024-05-15 17:36:41.264537 imsciences-0.5.6.0/PKG-INFO
--rw-rw-rw-   0        0        0     8965 2024-05-15 17:36:32.000000 imsciences-0.5.6.0/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 17:36:41.234337 imsciences-0.5.6.0/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.6.0/imsciences/__init__.py
--rw-rw-rw-   0        0        0    60033 2024-05-15 17:36:31.000000 imsciences-0.5.6.0/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-15 17:36:41.260821 imsciences-0.5.6.0/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9470 2024-05-15 17:36:41.000000 imsciences-0.5.6.0/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-15 17:36:41.000000 imsciences-0.5.6.0/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 17:36:41.000000 imsciences-0.5.6.0/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-15 17:36:41.000000 imsciences-0.5.6.0/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 17:36:41.000000 imsciences-0.5.6.0/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 17:36:41.269156 imsciences-0.5.6.0/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-15 17:36:34.000000 imsciences-0.5.6.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:38:30.339733 imsciences-0.5.6.1/
+-rw-rw-rw-   0        0        0     9757 2024-05-16 11:38:30.336746 imsciences-0.5.6.1/PKG-INFO
+-rw-rw-rw-   0        0        0     9252 2024-05-16 11:38:25.000000 imsciences-0.5.6.1/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 11:38:30.312074 imsciences-0.5.6.1/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.6.1/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    65522 2024-05-16 11:36:52.000000 imsciences-0.5.6.1/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 11:38:30.332696 imsciences-0.5.6.1/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9757 2024-05-16 11:38:30.000000 imsciences-0.5.6.1/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-16 11:38:30.000000 imsciences-0.5.6.1/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 11:38:30.000000 imsciences-0.5.6.1/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 11:38:30.000000 imsciences-0.5.6.1/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 11:38:30.000000 imsciences-0.5.6.1/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 11:38:30.339733 imsciences-0.5.6.1/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-16 11:38:23.000000 imsciences-0.5.6.1/setup.py
```

### Comparing `imsciences-0.5.6.0/PKG-INFO` & `imsciences-0.5.6.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.6.0
+Version: 0.5.6.1
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -124,7 +124,11 @@
 ### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
 - **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
 - **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
 
 ### 28. `format_numbers_with_commas(df, decimal_length_chosen=2)`
 - **Description**: Converts data in numerical format into numbers with commas and a chosen decimal place length.
 - **Usage**: `format_numbers_with_commas(df,1)`
+
+### 29. `filter_df_on_multiple_conditions(df, filters_dict)`
+- **Description**: Filters dataframe on multiple conditions, which come in the form of a dictionary.
+- **Usage**: `filter_df_on_multiple_conditions(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''})`
```

### Comparing `imsciences-0.5.6.0/README.md` & `imsciences-0.5.6.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -108,8 +108,12 @@
 
 ### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
 - **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
 - **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
 
 ### 28. `format_numbers_with_commas(df, decimal_length_chosen=2)`
 - **Description**: Converts data in numerical format into numbers with commas and a chosen decimal place length.
-- **Usage**: `format_numbers_with_commas(df,1)`
+- **Usage**: `format_numbers_with_commas(df,1)`
+
+### 29. `filter_df_on_multiple_conditions(df, filters_dict)`
+- **Description**: Filters dataframe on multiple conditions, which come in the form of a dictionary.
+- **Usage**: `filter_df_on_multiple_conditions(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''})`
```

### Comparing `imsciences-0.5.6.0/imsciences/datafunctions.py` & `imsciences-0.5.6.1/imsciences/datafunctions.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,22 @@
 import plotly.graph_objs as go
 from dateutil.parser import parse
 import numpy as np
 from datetime import datetime
 import datetime
 import re
 from datetime import datetime, timedelta
+import pandas as pd
+from datetime import datetime
+from imsciences import *
+from fredapi import Fred
+import pandas as pd
+import datetime
+from datetime import timedelta
+import time
 
 class dataprocessing:
     
     def help(self):
         print("This is the help section. The functions in the package are as follows:")
 
         print("\n1. get_wd_levels")
@@ -152,14 +160,20 @@
         print("   - Example: keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')")      
 
         print("\n28. format_numbers_with_commas")
         print("   - Description: Converts data in numerical format into numbers with commas and a chosen decimal place length.")
         print("   - Usage: format_numbers_with_commas(df, decimal_length_chosen=2)")
         print("   - Example: format_numbers_with_commas(df,1)")         
     
+        print("\n29. filter_df_on_multiple_conditions")
+        print("   - Description: Filters dataframe on multiple conditions, which come in the form of a dictionary.")
+        print("   - Usage: filter_df_on_multiple_conditions(df, filters_dict)")
+        print("   - Example: filter_df_on_multiple_conditions(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''})")       
+    
+    
     def get_wd_levels(self, levels):
         """
         Gets the current wd of whoever is working on it and gives the options to move the number of levels up.
 
         Parameters:
         - data_frame: pandas DataFrame
             The input data frame.
@@ -618,42 +632,17 @@
             margins (bool, optional): Whether the pivot table needs a total rows and column. Defaults to False.
             margins_name (str, optional): The name of the Totals columns. Defaults to "Total".
             datetime_trans_needed (bool, optional): Whether the index column needs to be transformed into datetime format. Defaults to False.
 
         Returns:
             pandas.DataFrame: The pivot table specified
         """
-        mask = pd.Series(True, index=df.index)
-        for col, cond in filters_dict.items():
-            cond = cond.strip()
-            operator, value = cond.split(maxsplit=1)
-            
-            # If value is a string condition make sure to check if there are new lines
-            if "'" in value:
-                value = value.strip().strip("'\"")
-            # If not a string e.g. datetime or number condition you need to transform the string into a value
-            else:
-                value = eval(value)  
-
-            if operator == "==":
-                temp_mask = (df[col] == value)
-            elif operator == "!=":
-                temp_mask = (df[col] != value)
-            elif operator == ">=":
-                temp_mask = (df[col] >= value)
-            elif operator == "<=":
-                temp_mask = (df[col] <= value)
-            elif operator == ">":
-                temp_mask = (df[col] > value)
-            elif operator == "<":
-                temp_mask = (df[col] < value)                          
-            mask &= temp_mask
-
+        
         # Create the filtered df by applying the conditions
-        df_filtered = df[mask]
+        df_filtered = self.filter_df_on_multiple_conditions(df, filters_dict)
         
         # Ensure OBS is in datetime format for proper sorting
         df_filtered = df_filtered.copy()
         
         # If datetime transformation is needed
         if datetime_trans_needed is True:
             df_filtered.loc[:,index_col] = pd.to_datetime(df_filtered[index_col], dayfirst=True)
@@ -1039,43 +1028,16 @@
         if change_in_existing_df_col not in ["Yes", "No"]:
             raise ValueError("Invalid input value for change_in_existing_df_col. Allowed values are: ['Yes', 'No']")
         
         # Raises value error if input is invalid for add_notes_col
         if add_notes not in ["Yes", "No"]:
             raise ValueError("Invalid input value for add_notes. Allowed values are: ['Yes', 'No']")
 
-        # Create list of conditions 
-        mask = pd.Series(True, index=df.index)
-        for col, cond in filters_dict.items():
-            cond = cond.strip()
-            operator, value = cond.split(maxsplit=1)
-            
-            # If value is a string condition make sure to check if there are new lines
-            if "'" in value:
-                value = value.strip().strip("'\"")
-            # If not a string e.g. datetime or number condition you need to transform the string into a value
-            else:
-                value = eval(value)  
-
-            if operator == "==":
-                temp_mask = (df[col] == value)
-            elif operator == "!=":
-                temp_mask = (df[col] != value)
-            elif operator == ">=":
-                temp_mask = (df[col] >= value)
-            elif operator == "<=":
-                temp_mask = (df[col] <= value)
-            elif operator == ">":
-                temp_mask = (df[col] > value)
-            elif operator == "<":
-                temp_mask = (df[col] < value)                          
-            mask &= temp_mask
-
         # Create the filtered df by applying the conditions
-        df_filtered = df[mask]
+        df_filtered = self.filter_df_on_multiple_conditions(df, filters_dict)
 
         # Create a new column to add the changes if desired, else edit in the current chosen column
         col_to_update = col_to_change if change_in_existing_df_col == "Yes" else new_col_to_change_name
         if change_in_existing_df_col == "No" and new_col_to_change_name not in df.columns:
             df = df.copy()
             df[new_col_to_change_name] = df[col_to_change]
             
@@ -1124,9 +1086,158 @@
 
 
         # Apply the function across several columns using applymap()
         formatted_df = df.applymap(format_number_with_commas)
 
         return formatted_df
     
+    def filter_df_on_multiple_conditions(self, df, filters_dict):
+        """
+        Filter a dataframe based on mulitple conditions
+
+        Args:
+            df (pandas.DatFrame): Dataframe to filter on
+            filters_dict (dict): Dictionary with strings as conditions
+
+        Returns:
+            pandas.DatFrame: Filtered Da
+        """
+        mask = pd.Series(True, index=df.index)
+        for col, cond in filters_dict.items():
+            cond = cond.strip()
+            operator, value = cond.split(maxsplit=1)
+            
+            # If value is a string condition make sure to check if there are new lines
+            if "'" in value:
+                value = value.strip().strip("'\"")
+            # If not a string e.g. datetime or number condition you need to transform the string into a value
+            else:
+                value = eval(value)  
+
+            if operator == "==":
+                temp_mask = (df[col] == value)
+            elif operator == "!=":
+                temp_mask = (df[col] != value)
+            elif operator == ">=":
+                temp_mask = (df[col] >= value)
+            elif operator == "<=":
+                temp_mask = (df[col] <= value)
+            elif operator == ">":
+                temp_mask = (df[col] > value)
+            elif operator == "<":
+                temp_mask = (df[col] < value)                          
+            mask &= temp_mask
+
+        # Create the filtered df by applying the conditions
+        df_filtered = df[mask]
+    
+        return df_filtered
+
 class datapull:
-    print("hello")
+
+    def pull_fred_data(self, week_commencing: str = 'sun', series_id_list: list[str] = ["GPDIC1", "Y057RX1Q020SBEA", "GCEC1", "ND000333Q", "Y006RX1Q020SBEA"]) -> pd.DataFrame:
+        '''
+        Parameters
+        ----------
+        week_commencing : str
+            specify the day for the week commencing, the default is 'sun' (e.g., 'mon', 'tue', 'wed', 'thu', 'fri', 'sat', 'sun')
+
+        series_id_list : list[str]
+            provide a list with IDs to download data series from FRED (link: https://fred.stlouisfed.org/tags/series?t=id). Default list is 
+            ["GPDIC1", "Y057RX1Q020SBEA", "GCEC1", "ND000333Q", "Y006RX1Q020SBEA"]
+        
+        Returns
+        ----------
+        pd.DataFrame
+            Return a data frame with FRED data according to the series IDs provided
+
+        Example
+        ----------
+        pull_fred_data("mon", ["GCEC1", "SP500"])
+        '''
+        # Fred API
+        fred = Fred(api_key='76f5f8156145fdb8fbaf66f1eb944f8a')
+
+        # Fetch the metadata for each series to get the full names
+        series_names = {series_id: fred.get_series_info(series_id).title for series_id in series_id_list}
+
+        # Download data from series id list
+        fred_series = {series_id: fred.get_series(series_id) for series_id in series_id_list}
+
+        # Data processing
+        date_range = {'OBS': pd.date_range("1950-01-01", datetime.today().strftime('%Y-%m-%d'), freq='d')}
+        fred_series_df = pd.DataFrame(date_range)
+
+        for series_id, series_data in fred_series.items():
+            series_data = series_data.reset_index()
+            series_data.columns = ['OBS', series_names[series_id]]  # Use the series name as the column header
+            fred_series_df = pd.merge_asof(fred_series_df, series_data, on='OBS', direction='backward')
+
+        # Handle duplicate columns
+        for col in fred_series_df.columns:
+            if '_x' in col:
+                base_col = col.replace('_x', '')
+                fred_series_df[base_col] = fred_series_df[col].combine_first(fred_series_df[base_col + '_y'])
+                fred_series_df.drop([col, base_col + '_y'], axis=1, inplace=True)
+
+        # Ensure sum_columns are present in the DataFrame
+        sum_columns = [series_names[series_id] for series_id in series_id_list if series_names[series_id] in fred_series_df.columns]
+
+        # Aggregate results by week
+        fred_df_final = dataprocessing.aggregate_daily_to_wc_wide(df=fred_series_df, 
+                                                    date_column="OBS", 
+                                                    group_columns=[], 
+                                                    sum_columns=sum_columns,
+                                                    wc=week_commencing,
+                                                    aggregation="average")
+
+        # Remove anything after the instance of any ':' in the column names and rename
+        fred_df_final.columns = ['macro_' + col.lower().split(':')[0].replace(' ', '_') for col in fred_df_final.columns]
+
+        return fred_df_final
+    
+    def pull_boe_data(week_commencing="mon", max_retries=30, delay=5):
+        # Week commencing dictionary
+        day_dict = {"mon": 0, "tue": 1, "wed": 2, "thur": 3, "fri": 4, "sat": 5, "sun": 6}
+        
+        # Function to fetch the data with retries
+        def fetch_data_with_retries(url, max_retries, delay):
+            for attempt in range(max_retries):
+                try:
+                    html_table = pd.read_html(url)[0]
+                    return html_table
+                except Exception as e:
+                    print(f"Attempt {attempt + 1} failed: {e}")
+                    if attempt < max_retries - 1:
+                        time.sleep(delay)
+                    else:
+                        raise
+        
+        # Import HTML data from Bank of England rate
+        url = 'https://www.bankofengland.co.uk/boeapps/database/Bank-Rate.asp'
+        html_table = fetch_data_with_retries(url, max_retries, delay)
+        
+        df = pd.DataFrame(html_table)
+        df.rename(columns={"Date Changed": "OBS", "Rate": "macro_boe_intr_rate"}, inplace=True)
+        
+        # Change date column to datetime and find the corresponding week to the date
+        df["OBS"] = pd.to_datetime(df["OBS"], format="%d %b %y")
+        df.sort_values("OBS", axis=0, inplace=True)
+        
+        # Create a daily date range and find the week commencing for that day
+        date_range = pd.date_range(df["OBS"].iloc[0], datetime.date.today(), freq="d")
+        df_daily = pd.DataFrame(date_range, columns=["OBS"])
+        
+        # Find the start of the week for each day
+        df_daily['OBS'] = df_daily["OBS"].apply(lambda x: x - pd.Timedelta(days=(x.weekday() - day_dict[week_commencing]) % 7))
+        
+        # Outer merge the daily date range on the boe dataframe and forward fill in the blanks
+        df_final = df_daily.merge(df, on='OBS', how="left")
+        df_final.ffill(inplace=True)
+        
+        # Group by the week start date and get the mean of the interest rates for each week
+        df_final = df_final.groupby('OBS')['macro_boe_intr_rate'].mean().reset_index()
+        
+        # Format the dates in the final dataframe
+        df_final['OBS'] = df_final['OBS'].dt.strftime('%d/%m/%Y')
+        
+        return df_final
```

### Comparing `imsciences-0.5.6.0/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.6.1/imsciences.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.6.0
+Version: 0.5.6.1
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -124,7 +124,11 @@
 ### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
 - **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
 - **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
 
 ### 28. `format_numbers_with_commas(df, decimal_length_chosen=2)`
 - **Description**: Converts data in numerical format into numbers with commas and a chosen decimal place length.
 - **Usage**: `format_numbers_with_commas(df,1)`
+
+### 29. `filter_df_on_multiple_conditions(df, filters_dict)`
+- **Description**: Filters dataframe on multiple conditions, which come in the form of a dictionary.
+- **Usage**: `filter_df_on_multiple_conditions(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''})`
```

### Comparing `imsciences-0.5.6.0/setup.py` & `imsciences-0.5.6.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.6.0'
+VERSION = '0.5.6.1'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

