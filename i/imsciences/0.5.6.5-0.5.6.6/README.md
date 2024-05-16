# Comparing `tmp/imsciences-0.5.6.5.tar.gz` & `tmp/imsciences-0.5.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsciences-0.5.6.5.tar", last modified: Thu May 16 18:44:36 2024, max compression
+gzip compressed data, was "imsciences-0.5.6.6.tar", last modified: Thu May 16 18:47:10 2024, max compression
```

## Comparing `imsciences-0.5.6.5.tar` & `imsciences-0.5.6.6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 18:44:36.143924 imsciences-0.5.6.5/
--rw-rw-rw-   0        0        0     9757 2024-05-16 18:44:36.137928 imsciences-0.5.6.5/PKG-INFO
--rw-rw-rw-   0        0        0     9252 2024-05-16 11:38:25.000000 imsciences-0.5.6.5/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 18:44:36.096930 imsciences-0.5.6.5/imsciences/
--rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.6.5/imsciences/__init__.py
--rw-rw-rw-   0        0        0    79375 2024-05-16 18:44:21.000000 imsciences-0.5.6.5/imsciences/datafunctions.py
-drwxrwxrwx   0        0        0        0 2024-05-16 18:44:36.134925 imsciences-0.5.6.5/imsciences.egg-info/
--rw-rw-rw-   0        0        0     9757 2024-05-16 18:44:35.000000 imsciences-0.5.6.5/imsciences.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      238 2024-05-16 18:44:35.000000 imsciences-0.5.6.5/imsciences.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 18:44:35.000000 imsciences-0.5.6.5/imsciences.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2024-05-16 18:44:35.000000 imsciences-0.5.6.5/imsciences.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-05-16 18:44:35.000000 imsciences-0.5.6.5/imsciences.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 18:44:36.144932 imsciences-0.5.6.5/setup.cfg
--rw-rw-rw-   0        0        0     1093 2024-05-16 18:43:55.000000 imsciences-0.5.6.5/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:47:09.994930 imsciences-0.5.6.6/
+-rw-rw-rw-   0        0        0     9757 2024-05-16 18:47:09.990922 imsciences-0.5.6.6/PKG-INFO
+-rw-rw-rw-   0        0        0     9252 2024-05-16 11:38:25.000000 imsciences-0.5.6.6/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 18:47:09.948387 imsciences-0.5.6.6/imsciences/
+-rw-rw-rw-   0        0        0       78 2024-05-15 13:56:33.000000 imsciences-0.5.6.6/imsciences/__init__.py
+-rw-rw-rw-   0        0        0    79381 2024-05-16 18:46:52.000000 imsciences-0.5.6.6/imsciences/datafunctions.py
+drwxrwxrwx   0        0        0        0 2024-05-16 18:47:09.985919 imsciences-0.5.6.6/imsciences.egg-info/
+-rw-rw-rw-   0        0        0     9757 2024-05-16 18:47:09.000000 imsciences-0.5.6.6/imsciences.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      238 2024-05-16 18:47:09.000000 imsciences-0.5.6.6/imsciences.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 18:47:09.000000 imsciences-0.5.6.6/imsciences.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2024-05-16 18:47:09.000000 imsciences-0.5.6.6/imsciences.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-05-16 18:47:09.000000 imsciences-0.5.6.6/imsciences.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 18:47:09.995942 imsciences-0.5.6.6/setup.cfg
+-rw-rw-rw-   0        0        0     1093 2024-05-16 18:47:00.000000 imsciences-0.5.6.6/setup.py
```

### Comparing `imsciences-0.5.6.5/PKG-INFO` & `imsciences-0.5.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.6.5
+Version: 0.5.6.6
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.6.5/README.md` & `imsciences-0.5.6.6/README.md`

 * *Files identical despite different names*

### Comparing `imsciences-0.5.6.5/imsciences/datafunctions.py` & `imsciences-0.5.6.6/imsciences/datafunctions.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,15 @@
             grouped = df_copy.groupby(['week_start'] + group_columns)[sum_columns].sum().reset_index()
 
         # Rename 'week_start' column to 'OBS'
         grouped = grouped.rename(columns={'week_start': 'OBS'})
 
         return grouped
     
-    def convert_monthly_to_daily(df, date_column, divide=True):
+    def convert_monthly_to_daily(self, df, date_column, divide=True):
         """
         Convert a DataFrame with monthly data to daily data.
         This function takes a DataFrame and a date column, then it expands each
         monthly record into daily records by dividing the numeric values by the number of days in that month.
 
         :param df: DataFrame with monthly data.
         :param date_column: The name of the column containing the date.
```

### Comparing `imsciences-0.5.6.5/imsciences.egg-info/PKG-INFO` & `imsciences-0.5.6.6/imsciences.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsciences
-Version: 0.5.6.5
+Version: 0.5.6.6
 Summary: IMS Data Processing Package
 Author: IMS
 Author-email: cam@im-sciences.com
 Keywords: python,data processing
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `imsciences-0.5.6.5/setup.py` & `imsciences-0.5.6.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Function to read the contents of the README file
 def read_md(file_name):
     if os.path.isfile(file_name):
         with open(file_name, 'r', encoding='utf-8') as f:
             return f.read()
     return ''
 
-VERSION = '0.5.6.5'
+VERSION = '0.5.6.6'
 DESCRIPTION = 'IMS Data Processing Package'
 LONG_DESCRIPTION = read_md('README.md')  # Reading from README.md
 
 # Setting up
 setup(
     name="imsciences",
     version=VERSION,
```

