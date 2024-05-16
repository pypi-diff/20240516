# Comparing `tmp/vbpy-1.1.tar.gz` & `tmp/vbpy-2.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vbpy-1.1.tar", last modified: Wed May 15 08:47:10 2024, max compression
+gzip compressed data, was "vbpy-2.0.2.tar", last modified: Thu May 16 09:08:24 2024, max compression
```

## Comparing `vbpy-1.1.tar` & `vbpy-2.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-15 08:47:10.350000 vbpy-1.1/
--rw-rw-rw-   0        0        0      120 2024-05-15 08:47:12.000000 vbpy-1.1/PKG-INFO
--rw-rw-rw-   0        0        0       42 2024-05-15 08:47:12.000000 vbpy-1.1/setup.cfg
--rw-rw-rw-   0        0        0      534 2024-05-15 08:46:58.000000 vbpy-1.1/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-15 08:47:10.390000 vbpy-1.1/vbpy/
--rw-rw-rw-   0        0        0      134 2024-05-15 08:43:06.000000 vbpy-1.1/vbpy/__init__.py
--rw-rw-rw-   0        0        0     2553 2024-05-15 08:43:08.000000 vbpy-1.1/vbpy/combine_data.py
--rw-rw-rw-   0        0        0    18131 2024-05-15 08:27:34.000000 vbpy-1.1/vbpy/load_claim_auto.py
--rw-rw-rw-   0        0        0    13907 2024-05-15 08:19:46.000000 vbpy-1.1/vbpy/load_revenue_auto.py
-drwxrwxrwx   0        0        0        0 2024-05-15 08:47:10.430000 vbpy-1.1/vbpy.egg-info/
--rw-rw-rw-   0        0        0      120 2024-05-15 08:47:12.000000 vbpy-1.1/vbpy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      208 2024-05-15 08:47:12.000000 vbpy-1.1/vbpy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-15 08:47:12.000000 vbpy-1.1/vbpy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-05-15 08:47:12.000000 vbpy-1.1/vbpy.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-05-16 09:08:24.310000 vbpy-2.0.2/
+-rw-rw-rw-   0        0        0      122 2024-05-16 09:08:26.000000 vbpy-2.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2024-05-16 09:08:26.000000 vbpy-2.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      536 2024-05-16 09:07:58.000000 vbpy-2.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:08:24.350000 vbpy-2.0.2/vbpy/
+-rw-rw-rw-   0        0        0      149 2024-05-15 08:58:38.000000 vbpy-2.0.2/vbpy/__init__.py
+-rw-rw-rw-   0        0        0     2553 2024-05-16 07:09:16.000000 vbpy-2.0.2/vbpy/combine_data_file.py
+-rw-rw-rw-   0        0        0    18171 2024-05-16 09:07:32.000000 vbpy-2.0.2/vbpy/load_claim_auto_file.py
+-rw-rw-rw-   0        0        0    14001 2024-05-16 09:07:50.000000 vbpy-2.0.2/vbpy/load_revenue_auto_file.py
+drwxrwxrwx   0        0        0        0 2024-05-16 09:08:24.380000 vbpy-2.0.2/vbpy.egg-info/
+-rw-rw-rw-   0        0        0      122 2024-05-16 09:08:26.000000 vbpy-2.0.2/vbpy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      223 2024-05-16 09:08:26.000000 vbpy-2.0.2/vbpy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 09:08:26.000000 vbpy-2.0.2/vbpy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-05-16 09:08:26.000000 vbpy-2.0.2/vbpy.egg-info/top_level.txt
```

### Comparing `vbpy-1.1/setup.py` & `vbpy-2.0.2/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 setup(
     
     name='vbpy',
-    version='1.1',
+    version='2.0.2',
     packages=find_packages(),
     # description='Your library description',
     # long_description=open('README.md').read(),
     # long_description_content_type='text/markdown',
     author='Nguyen Ha Tuan Long',
     author_email='tuanlongnguyenha@gmail.com',
     # url='https://github.com/yourusername/your_library_name',
```

### Comparing `vbpy-1.1/vbpy/combine_data.py` & `vbpy-2.0.2/vbpy/combine_data_file.py`

 * *Files identical despite different names*

### Comparing `vbpy-1.1/vbpy/load_claim_auto.py` & `vbpy-2.0.2/vbpy/load_claim_auto_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -91,16 +91,15 @@
                     }
 
                     df.rename(columns={col: df_clm_dict[col] for col in df.columns if col in df_clm_dict}, inplace=True)
 
                     
                     """ SEPARATE SO MAY and SO KHUNG"""
                     print("--------------------------------------------------------------------------\nSeparating SO MAY/SO KHUNG:")
-                    df['SO_MAY'] = df['SO_KHUNG/SO_MAY'].str.split('/')[1]
-                    df['SO_KHUNG'] = df['SO_KHUNG/SO_MAY'].str.split('/')[0]
+                    df[['SO_KHUNG', 'SO_MAY']] = df['SO_KHUNG/SO_MAY'].str.split('/', expand=True)
                     df.drop('SO_KHUNG/SO_MAY', axis = 1, inplace = True)
                     
                         
                     """ REMOVE UNNECESSARY COLUMNS"""
                     print("--------------------------------------------------------------------------\nRemoving Unneeded Columns:")
                     removed_cols = [
                         'Lĩnh vực kinh doanh',
@@ -268,20 +267,22 @@
                     rows_b4 = df.shape[0]    
                     df = df[df['NGAY_HL'].notna()]
                     print(f'   Removed: {(rows_b4 - df.shape[0]):,.0f} Rows, ({((rows_b4 - df.shape[0])/rows_b4*100):.2f}%)')
                     
                     
                     " STANDARDIZE PLATE IDs"
                     print("--------------------------------------------------------------------------\nStandardizing SO_BIEN_XE:")    
-                    pattern = r'^\d+\d+[A-Za-z].*$' #Number-Number-Letter... (eg, 29A)
+                    pattern = r'^\d{2}[A-Za-z]\d{4,5}$' 
                     _copy = df['SO_BIEN_XE'].copy()
-                    df['SO_BIEN_XE'][~df['SO_BIEN_XE'].str.match(pattern, na = False)] = np.nan # Converted 7253 Inccorect values to NaN
-                    df['SO_BIEN_XE'] = df['SO_BIEN_XE'].str.replace('[^a-zA-Z0-9]', '', regex=True).upper()
+                    df.loc[:,'SO_BIEN_XE'] = df['SO_BIEN_XE'].str.replace('[^a-zA-Z0-9]', '', regex=True)
+                    df.loc[:,'SO_BIEN_XE'] = df['SO_BIEN_XE'].str.strip().str.upper()
+                    df.loc[df['SO_BIEN_XE'] == '', 'SO_BIEN_XE'] = pd.NA
+                    df.loc[~df['SO_BIEN_XE'].str.match(pattern, na = False), 'SO_BIEN_XE'] = pd.NA
                     
-                    print(f'   Changed: {(df['SO_BIEN_XE'] == _copy)} values')
+                    print(f'   Changed: {sum(df['SO_BIEN_XE'] == _copy)} values')
                     print(f'   Converted: {df['SO_BIEN_XE'].isna().sum() - _copy.isna().sum()} to NAs')
                     del _copy
                     
                     
                     """ PRINT EFF_YEAR COUNTS IN EACH DF"""
                     print("--------------------------------------------------------------------------\nEff Year Count:")
                     df['NAM_HL'] = df['NGAY_HL'].dt.year
```

### Comparing `vbpy-1.1/vbpy/load_revenue_auto.py` & `vbpy-2.0.2/vbpy/load_revenue_auto_file.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,20 +192,22 @@
                     rows_b4 = df.shape[0]    
                     df = df[df['NGAY_HL'].notna()]
                     print(f'   Removed: {(rows_b4 - df.shape[0]):,.0f} Rows, ({((rows_b4 - df.shape[0])/rows_b4*100):.2f}%)')
                     
                     
                     " STANDARDIZE PLATE IDs"
                     print("--------------------------------------------------------------------------\nStandardizing SO_BIEN_XE:")    
-                    pattern = r'^\d+\d+[A-Za-z].*$' #Number-Number-Letter... (eg, 29A)
+                    pattern = r'^\d{2}[A-Za-z]\d{4,5}$' 
                     _copy = df['SO_BIEN_XE'].copy()
-                    df['SO_BIEN_XE'][~df['SO_BIEN_XE'].str.match(pattern, na = False)] = np.nan # Converted 7253 Inccorect values to NaN
-                    df['SO_BIEN_XE'] = df['SO_BIEN_XE'].str.replace('[^a-zA-Z0-9]', '', regex=True).upper()
+                    df.loc[:,'SO_BIEN_XE'] = df['SO_BIEN_XE'].str.replace('[^a-zA-Z0-9]', '', regex=True)
+                    df.loc[:,'SO_BIEN_XE'] = df['SO_BIEN_XE'].str.strip().str.upper()
+                    df.loc[df['SO_BIEN_XE'] == '', 'SO_BIEN_XE'] = pd.NA
+                    df.loc[~df['SO_BIEN_XE'].str.match(pattern, na = False), 'SO_BIEN_XE'] = pd.NA
                     
-                    print(f'   Changed: {(df['SO_BIEN_XE'] == _copy)} values')
+                    print(f'   Changed: {sum(df['SO_BIEN_XE'] == _copy)} values')
                     print(f'   Converted: {df['SO_BIEN_XE'].isna().sum() - _copy.isna().sum()} to NAs')
                     del _copy
                     
                     
                     """ PRINT EFF_YEAR COUNTS IN EACH DF"""
                     print("--------------------------------------------------------------------------\nEff Year Count:")
                     df['NAM_HL'] = df['NGAY_HL'].dt.year
```

