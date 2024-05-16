# Comparing `tmp/imsciences-0.5.5.9.tar.gz` & `tmp/imsciences-0.5.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.5.9.tar", last modified: Wed May 15 16:06:01 2024, max compression
+gzip compressed data, was "imsciences-0.5.6.0.tar", last modified: Wed May 15 17:36:41 2024, max compression
```

## Comparing `imsciences-0.5.5.9.tar` & `imsciences-0.5.6.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 16:06:01.336023 imsciences-0.5.5.9/
--rw-rw-rw-   0        0        0     8987 2024-05-15 16:06:01.331635 imsciences-0.5.5.9/PKG-INFO
--rw-rw-rw-   0        0        0     8482 2024-05-15 12:04:13.000000 imsciences-0.5.5.9/README.md
-drwxrwxrwx   0        0        0        0 2024-05-15 16:06:01.306528 imsciences-0.5.5.9/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.5.9/imsciences/__init__.py
--rw-rw-rw-   0        0        0    55701 2024-05-15 16:04:36.000000 imsciences-0.5.5.9/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-15 16:06:01.329636 imsciences-0.5.5.9/imsciences.egg-info/
--rw-rw-rw-   0        0        0     8987 2024-05-15 16:06:01.000000 imsciences-0.5.5.9/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-15 16:06:01.000000 imsciences-0.5.5.9/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 16:06:01.000000 imsciences-0.5.5.9/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-15 16:06:01.000000 imsciences-0.5.5.9/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-15 16:06:01.000000 imsciences-0.5.5.9/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-15 16:06:01.336023 imsciences-0.5.5.9/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-15 16:05:56.000000 imsciences-0.5.5.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:36:41.268648 imsciences-0.5.6.0/
+-rw-rw-rw-   0        0        0     9470 2024-05-15 17:36:41.264537 imsciences-0.5.6.0/PKG-INFO
+-rw-rw-rw-   0        0        0     8965 2024-05-15 17:36:32.000000 imsciences-0.5.6.0/README.md
+drwxrwxrwx   0        0        0        0 2024-05-15 17:36:41.234337 imsciences-0.5.6.0/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.6.0/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    60033 2024-05-15 17:36:31.000000 imsciences-0.5.6.0/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-15 17:36:41.260821 imsciences-0.5.6.0/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9470 2024-05-15 17:36:41.000000 imsciences-0.5.6.0/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-15 17:36:41.000000 imsciences-0.5.6.0/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-15 17:36:41.000000 imsciences-0.5.6.0/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-15 17:36:41.000000 imsciences-0.5.6.0/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-15 17:36:41.000000 imsciences-0.5.6.0/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-15 17:36:41.269156 imsciences-0.5.6.0/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-15 17:36:34.000000 imsciences-0.5.6.0/setup.py
```

### Comparing `imsciences-0.5.5.9/PKG-INFO` & `imsciences-0.5.6.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.5.9
+Version: 0.5.6.0
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
@@ -77,17 +77,17 @@
 - **Description**: Convert a DataFrame column with mixed date formats to datetime.
 - **Usage**: `convert_us_to_uk_dates(df, date_col)`
 
 ### 16. `combine_sheets(all_sheets)`
 - **Description**: Combines multiple DataFrames from a dictionary into a single DataFrame.
 - **Usage**: `combine_sheets({'Sheet1': df1, 'Sheet2': df2})`
 
-### 17. `dynamic_pivot(data_frame, index_col, columns, values_col, fill_value=0)`
+### 17. `pivot_table(df, filters_dict, index_col, columns, values_col, fill_value=0,aggfunc='sum',margins=False,margins_name='Total',datetime_trans_needed=True)`
 - **Description**: Dynamically pivots a DataFrame based on specified columns.
-- **Usage**: `dynamic_pivot(df, 'Date', ['Category1', 'Category2'], ['Value1'])`
+- **Usage**: `pivot_table(df, {'Master Include':' == 1','OBS':' >= datetime(2019,9,9)','Metric Short Names':' == 'spd''}, 'OBS', 'Channel Short Names', 'Value', fill_value=0,aggfunc='sum',margins=False,margins_name='Total',datetime_trans_needed=True)`
 
 ### 18. `apply_lookup_table_for_columns(df, col_names, to_find_dict, if_not_in_country_dict='Other'), new_column_name='Mapping')`
 - **Description**: Equivalent of xlookup in excel. Allows you to map a dictionary of substrings within a column. If multiple columns are need for the LUT then a | seperator is needed.
 - **Usage**: `classify_within_column(df, ['campaign type','media type'], {'France Paid Social FB|paid social': 'facebook','France Paid Social TW|paid social': 'twitter'}, 'other','mapping')`
 
 ### 19. `aggregate_daily_to_wc_wide(df, date_column, group_columns, sum_columns, wc, aggregation='sum', include_totals=False)`
 - **Description**: Aggregates daily data into weekly data, grouping and summing specified columns, starting on a specified day of the week. In the wide format.
@@ -120,7 +120,11 @@
 ### 26. `convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')`
 - **Description**: Changes a dataframe from wide to long format.
 - **Usage**: `keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')`
 
 ### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
 - **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
 - **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
+
+### 28. `format_numbers_with_commas(df, decimal_length_chosen=2)`
+- **Description**: Converts data in numerical format into numbers with commas and a chosen decimal place length.
+- **Usage**: `format_numbers_with_commas(df,1)`
```

### Comparing `imsciences-0.5.5.9/README.md` & `imsciences-0.5.6.0/imsciences.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,22 @@
+Metadata-Version: 2.1
+Name: imsciences
+Version: 0.5.6.0
+Summary: IMS Data Processing Package
+Author: IMS
+Author-email: cam@im-sciences.com
+Keywords: python,data processing
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: Unix
+Classifier: Operating System :: MacOS :: MacOS X
+Classifier: Operating System :: Microsoft :: Windows
+Description-Content-Type: text/markdown
+
 # IMS Package Documentation
 
 The IMS package is a python library for processing incoming data into a format that can be used for projects. IMS processing offers a variety of functions to manipulate and analyze data efficiently. Here are the functionalities provided by the package:
 
 ### 1. `get_wd_levels(levels)`
 - **Description**: Get the working directory with the option of moving up parents.
 - **Usage**: `get_wd_levels(levels)`
@@ -62,17 +77,17 @@
 - **Description**: Convert a DataFrame column with mixed date formats to datetime.
 - **Usage**: `convert_us_to_uk_dates(df, date_col)`
 
 ### 16. `combine_sheets(all_sheets)`
 - **Description**: Combines multiple DataFrames from a dictionary into a single DataFrame.
 - **Usage**: `combine_sheets({'Sheet1': df1, 'Sheet2': df2})`
 
-### 17. `dynamic_pivot(data_frame, index_col, columns, values_col, fill_value=0)`
+### 17. `pivot_table(df, filters_dict, index_col, columns, values_col, fill_value=0,aggfunc='sum',margins=False,margins_name='Total',datetime_trans_needed=True)`
 - **Description**: Dynamically pivots a DataFrame based on specified columns.
-- **Usage**: `dynamic_pivot(df, 'Date', ['Category1', 'Category2'], ['Value1'])`
+- **Usage**: `pivot_table(df, {'Master Include':' == 1','OBS':' >= datetime(2019,9,9)','Metric Short Names':' == 'spd''}, 'OBS', 'Channel Short Names', 'Value', fill_value=0,aggfunc='sum',margins=False,margins_name='Total',datetime_trans_needed=True)`
 
 ### 18. `apply_lookup_table_for_columns(df, col_names, to_find_dict, if_not_in_country_dict='Other'), new_column_name='Mapping')`
 - **Description**: Equivalent of xlookup in excel. Allows you to map a dictionary of substrings within a column. If multiple columns are need for the LUT then a | seperator is needed.
 - **Usage**: `classify_within_column(df, ['campaign type','media type'], {'France Paid Social FB|paid social': 'facebook','France Paid Social TW|paid social': 'twitter'}, 'other','mapping')`
 
 ### 19. `aggregate_daily_to_wc_wide(df, date_column, group_columns, sum_columns, wc, aggregation='sum', include_totals=False)`
 - **Description**: Aggregates daily data into weekly data, grouping and summing specified columns, starting on a specified day of the week. In the wide format.
@@ -104,8 +119,12 @@
 
 ### 26. `convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')`
 - **Description**: Changes a dataframe from wide to long format.
 - **Usage**: `keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')`
 
 ### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
 - **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
-- **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
+- **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
+
+### 28. `format_numbers_with_commas(df, decimal_length_chosen=2)`
+- **Description**: Converts data in numerical format into numbers with commas and a chosen decimal place length.
+- **Usage**: `format_numbers_with_commas(df,1)`
```

### Comparing `imsciences-0.5.5.9/imsciences/datafunctions.py` & `imsciences-0.5.6.0/imsciences/datafunctions.py`

 * *Files 3% similar despite different names*

```diff
@@ -92,18 +92,18 @@
         print("    - Example: convert_us_to_uk_dates(df, 'date')")
         
         print("\n16. combine_sheets")
         print("    - Description: Combines multiple DataFrames from a dictionary into a single DataFrame.")
         print("    - Usage: combine_sheets(all_sheets)")
         print("    - Example: combine_sheets({'Sheet1': df1, 'Sheet2': df2})")
         
-        print("\n17. dynamic_pivot")
+        print("\n17. pivot_table")
         print("    - Description: Dynamically pivots a DataFrame based on specified columns.")
-        print("    - Usage: dynamic_pivot(data_frame, index_col, columns, values_col, fill_value=0)")
-        print("    - Example: dynamic_pivot(df, 'Date', ['Category1', 'Category2'], ['Value1'])")
+        print("    - Usage: pivot_table(df, filters_dict, index_col, columns, values_col, fill_value=0,aggfunc='sum',margins=False,margins_name='Total',datetime_trans_needed=True)")
+        print("    - Example: pivot_table(df, {'Master Include':' == 1','OBS':' >= datetime(2019,9,9)','Metric Short Names':' == 'spd''}, 'OBS', 'Channel Short Names', 'Value', fill_value=0,aggfunc='sum',margins=False,margins_name='Total',datetime_trans_needed=True)")
         
         print("\n18. apply_lookup_table_for_columns")
         print("    - Description: Equivalent of xlookup in excel. Allows you to map a dictionary of substrings within a column. If multiple columns are need for the LUT then a | seperator is needed.")
         print("    - Usage: classify_within_column(df, col_names, to_find_dict, if_not_in_country_dict='Other'), new_column_name='Mapping'")
         print("    - Example: classify_within_column(df, ['campaign type','media type'], {'France Paid Social FB|paid social': 'facebook','France Paid Social TW|paid social': 'twitter'}, 'other','mapping')")
 
         print("\n19. aggregate_daily_to_wc_wide")
@@ -146,15 +146,20 @@
         print("   - Usage: convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')")
         print("   - Example: keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')") 
         
         print("\n27. manually_edit_data")
         print("   - Description: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.")
         print("   - Usage: manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)")
         print("   - Example: keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')")      
-        
+
+        print("\n28. format_numbers_with_commas")
+        print("   - Description: Converts data in numerical format into numbers with commas and a chosen decimal place length.")
+        print("   - Usage: format_numbers_with_commas(df, decimal_length_chosen=2)")
+        print("   - Example: format_numbers_with_commas(df,1)")         
+    
     def get_wd_levels(self, levels):
         """
         Gets the current wd of whoever is working on it and gives the options to move the number of levels up.
 
         Parameters:
         - data_frame: pandas DataFrame
             The input data frame.
@@ -594,41 +599,92 @@
 
         for sheet_name, df in all_sheets.items():
             df['SheetName'] = sheet_name 
             combined_df = pd.concat([combined_df, df], ignore_index=True)
 
         return combined_df
     
-    def dynamic_pivot(self, data_frame, index_col, columns, values_col, fill_value=0):
+    def pivot_table(self, df, filters_dict, index_col, columns, values_col, fill_value=0,aggfunc='sum',margins=False,margins_name="Total",datetime_trans_needed=True):
+        """
+        Provides the ability to create pivot tables, filtering the data to get to data you want and then pivoting on certain columns
+
+        Args:
+            df (pandas.DataFrame): The DataFrame containing the data.
+            filters_dict (dict): Dictionary of conditions for the boolean mask i.e. what to filter your df on to get to your chosen cell
+            index_col (str): Name of Column for your pivot table to index on
+            columns (str): Name of Columns for your pivot table.
+            values_col (str): Name of Values Columns for your pivot table.
+            fill_value (int, optional): The value to replace nan with. Defaults to 0.
+            aggfunc (str, optional): The method on which to aggregate the values column. Defaults to sum.
+            margins (bool, optional): Whether the pivot table needs a total rows and column. Defaults to False.
+            margins_name (str, optional): The name of the Totals columns. Defaults to "Total".
+            datetime_trans_needed (bool, optional): Whether the index column needs to be transformed into datetime format. Defaults to False.
+
+        Returns:
+            pandas.DataFrame: The pivot table specified
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
         # Ensure OBS is in datetime format for proper sorting
-        data_frame[index_col] = pd.to_datetime(data_frame[index_col], dayfirst=True)
+        df_filtered = df_filtered.copy()
         
-        # Check if values_col is a single column or a list and pivot accordingly
-        if isinstance(values_col, list):
-            # If values_col is a list, use .pivot_table() to accommodate multiple values columns
-            pivoted_df = data_frame.pivot_table(index=index_col, columns=columns, values=values_col, aggfunc='sum')
-        else:
-            # For a single value column, use .pivot()
-            pivoted_df = data_frame.pivot(index=index_col, columns=columns, values=values_col)
+        # If datetime transformation is needed
+        if datetime_trans_needed is True:
+            df_filtered.loc[:,index_col] = pd.to_datetime(df_filtered[index_col], dayfirst=True)
         
+        # Create the pivot table
+        pivoted_df = df_filtered.pivot_table(index=index_col, columns=columns, values=values_col, aggfunc=aggfunc,margins=margins,margins_name=margins_name)
+            
         # Handling MultiIndex columns if present, making them a flat structure
         if isinstance(pivoted_df.columns, pd.MultiIndex):
             pivoted_df.columns = ['_'.join(map(str, col)).strip() for col in pivoted_df.columns.values]
         else:
             pivoted_df.columns = pivoted_df.columns.map(str)
         
         # Reset the pivot before returning
         pivoted_df = pivoted_df.reset_index()
         
         # Sort by OBS from oldest to newest
-        pivoted_df[index_col] = pd.to_datetime(pivoted_df[index_col])  # Ensure sorting works correctly
-        pivoted_df = pivoted_df.sort_values(by=index_col)
+        if datetime_trans_needed is True:
+            # pivoted_df = pivoted_df.reset_index()
+            pivoted_df[index_col] = pd.to_datetime(pivoted_df[index_col])  # Ensure sorting works correctly
+            pivoted_df = pivoted_df.sort_values(by=index_col)
         
-        # Convert OBS back to a string in YYYY-MM-DD format for display purposes
-        pivoted_df[index_col] = pivoted_df[index_col].dt.strftime('%Y-%m-%d')
+            # Convert OBS back to a string in YYYY-MM-DD format for display purposes
+            pivoted_df[index_col] = pivoted_df[index_col].dt.strftime('%Y-%m-%d')
+            
+            # Set index back to date column
+            # pivoted_df.set_index(index_col,inplace=True)
         
         # Fill in any NaNs
         pivoted_df = pivoted_df.fillna(fill_value)
         
         return pivoted_df
 
     def apply_lookup_table_for_columns(self, df, col_names, to_find_dict, if_not_in_dict="Other", new_column_name="Mapping"):
@@ -1040,9 +1096,37 @@
             note_col = existing_note_col_name if existing_note_col_name else 'Notes'
             if note_col not in df.columns:
                 df[note_col] = None
             df.loc[df_filtered.index, note_col] = note
 
         return df
     
+    def format_numbers_with_commas(self, df, decimal_length_chosen=2):
+        """
+        Converts data in numerical format into numbers with commas and a chosen decimal place length
+
+        Args:
+            df (pandas.DataFrame): The DataFrame containing the data.
+            decimal_length_chosen (int, optional): _description_. Defaults to 2.
+            
+        Returns:
+            pandas.DataFrame: The dataframe with the chosen updated format
+        """
+        def format_number_with_commas(x, decimal_length=decimal_length_chosen):
+            if isinstance(x, (int, float)):
+                if decimal_length is not None:
+                    format_str = "{:,.{}f}".format(x, decimal_length)
+                    formatted_number = format_str.format(x)
+                else:
+                    formatted_number = "{:,}".format(x)
+                return formatted_number
+            else:
+                return x  # Return unchanged if not a number
+
+
+        # Apply the function across several columns using applymap()
+        formatted_df = df.applymap(format_number_with_commas)
+
+        return formatted_df
+    
 class datapull:
     print("hello")
```

### Comparing `imsciences-0.5.5.9/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.6.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: imsciences
-Version: 0.5.5.9
-Summary: IMS Data Processing Package
-Author: IMS
-Author-email: cam@im-sciences.com
-Keywords: python,data processing
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: Unix
-Classifier: Operating System :: MacOS :: MacOS X
-Classifier: Operating System :: Microsoft :: Windows
-Description-Content-Type: text/markdown
-
 # IMS Package Documentation
 
 The IMS package is a python library for processing incoming data into a format that can be used for projects. IMS processing offers a variety of functions to manipulate and analyze data efficiently. Here are the functionalities provided by the package:
 
 ### 1. `get_wd_levels(levels)`
 - **Description**: Get the working directory with the option of moving up parents.
 - **Usage**: `get_wd_levels(levels)`
@@ -77,17 +62,17 @@
 - **Description**: Convert a DataFrame column with mixed date formats to datetime.
 - **Usage**: `convert_us_to_uk_dates(df, date_col)`
 
 ### 16. `combine_sheets(all_sheets)`
 - **Description**: Combines multiple DataFrames from a dictionary into a single DataFrame.
 - **Usage**: `combine_sheets({'Sheet1': df1, 'Sheet2': df2})`
 
-### 17. `dynamic_pivot(data_frame, index_col, columns, values_col, fill_value=0)`
+### 17. `pivot_table(df, filters_dict, index_col, columns, values_col, fill_value=0,aggfunc='sum',margins=False,margins_name='Total',datetime_trans_needed=True)`
 - **Description**: Dynamically pivots a DataFrame based on specified columns.
-- **Usage**: `dynamic_pivot(df, 'Date', ['Category1', 'Category2'], ['Value1'])`
+- **Usage**: `pivot_table(df, {'Master Include':' == 1','OBS':' >= datetime(2019,9,9)','Metric Short Names':' == 'spd''}, 'OBS', 'Channel Short Names', 'Value', fill_value=0,aggfunc='sum',margins=False,margins_name='Total',datetime_trans_needed=True)`
 
 ### 18. `apply_lookup_table_for_columns(df, col_names, to_find_dict, if_not_in_country_dict='Other'), new_column_name='Mapping')`
 - **Description**: Equivalent of xlookup in excel. Allows you to map a dictionary of substrings within a column. If multiple columns are need for the LUT then a | seperator is needed.
 - **Usage**: `classify_within_column(df, ['campaign type','media type'], {'France Paid Social FB|paid social': 'facebook','France Paid Social TW|paid social': 'twitter'}, 'other','mapping')`
 
 ### 19. `aggregate_daily_to_wc_wide(df, date_column, group_columns, sum_columns, wc, aggregation='sum', include_totals=False)`
 - **Description**: Aggregates daily data into weekly data, grouping and summing specified columns, starting on a specified day of the week. In the wide format.
@@ -120,7 +105,11 @@
 ### 26. `convert_df_wide_2_long(df,value_cols,variable_col_name='Stacked',value_col_name='Value')`
 - **Description**: Changes a dataframe from wide to long format.
 - **Usage**: `keyword_lookup_replacement(df, ['Media Cost','Impressions','Clicks'],variable_col_name='Metric')`
 
 ### 27. `manually_edit_data(df, filters_dict, col_to_change, new_value, change_in_existing_df_col='No', new_col_to_change_name='New', manual_edit_col_name=None, add_notes='No', existing_note_col_name=None, note=None)`
 - **Description**: Allows the capability to manually update any cell in dataframe by applying filters and chosing a column to edit in dataframe.
 - **Usage**: `keyword_lookup_replacement(df, {'OBS':' <= datetime(2023,1,23)','File_Name':' == 'France media''},'Master Include',1,change_in_existing_df_col = 'Yes',new_col_to_change_name = 'Master Include',manual_edit_col_name = 'Manual Changes')`
+
+### 28. `format_numbers_with_commas(df, decimal_length_chosen=2)`
+- **Description**: Converts data in numerical format into numbers with commas and a chosen decimal place length.
+- **Usage**: `format_numbers_with_commas(df,1)`
```

### Comparing `imsciences-0.5.5.9/setup.py` & `imsciences-0.5.6.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.5.9'
+VERSION = '0.5.6.0'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

