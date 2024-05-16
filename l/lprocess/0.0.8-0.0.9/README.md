# Comparing `tmp/lprocess-0.0.8.tar.gz` & `tmp/lprocess-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lprocess-0.0.8.tar", last modified: Tue May 14 17:41:17 2024, max compression
+gzip compressed data, was "lprocess-0.0.9.tar", last modified: Thu May 16 04:49:06 2024, max compression
```

## Comparing `lprocess-0.0.8.tar` & `lprocess-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-14 17:41:17.943553 lprocess-0.0.8/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-14 17:41:17.943553 lprocess-0.0.8/PKG-INFO
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-14 17:41:17.943553 lprocess-0.0.8/lprocess/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)     5630 2024-05-14 17:40:52.000000 lprocess-0.0.8/lprocess/EDA.py
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       21 2024-05-11 11:47:06.000000 lprocess-0.0.8/lprocess/__init__.py
-drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-14 17:41:17.943553 lprocess-0.0.8/lprocess.egg-info/
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      505 2024-05-14 17:41:17.000000 lprocess-0.0.8/lprocess.egg-info/PKG-INFO
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      204 2024-05-14 17:41:17.000000 lprocess-0.0.8/lprocess.egg-info/SOURCES.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        1 2024-05-14 17:41:17.000000 lprocess-0.0.8/lprocess.egg-info/dependency_links.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       24 2024-05-14 17:41:17.000000 lprocess-0.0.8/lprocess.egg-info/requires.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        9 2024-05-14 17:41:17.000000 lprocess-0.0.8/lprocess.egg-info/top_level.txt
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       38 2024-05-14 17:41:17.943553 lprocess-0.0.8/setup.cfg
--rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      703 2024-05-14 17:41:01.000000 lprocess-0.0.8/setup.py
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-16 04:49:06.436724 lprocess-0.0.9/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      533 2024-05-16 04:49:06.436724 lprocess-0.0.9/PKG-INFO
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-16 04:49:06.436724 lprocess-0.0.9/lprocess/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)     5724 2024-05-16 04:41:09.000000 lprocess-0.0.9/lprocess/EDA.py
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       21 2024-05-11 11:47:06.000000 lprocess-0.0.9/lprocess/__init__.py
+drwxrwxr-x   0 lordpatil  (1000) lordpatil  (1000)        0 2024-05-16 04:49:06.436724 lprocess-0.0.9/lprocess.egg-info/
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      533 2024-05-16 04:49:06.000000 lprocess-0.0.9/lprocess.egg-info/PKG-INFO
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      204 2024-05-16 04:49:06.000000 lprocess-0.0.9/lprocess.egg-info/SOURCES.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        1 2024-05-16 04:49:06.000000 lprocess-0.0.9/lprocess.egg-info/dependency_links.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       24 2024-05-16 04:49:06.000000 lprocess-0.0.9/lprocess.egg-info/requires.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)        9 2024-05-16 04:49:06.000000 lprocess-0.0.9/lprocess.egg-info/top_level.txt
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)       38 2024-05-16 04:49:06.436724 lprocess-0.0.9/setup.cfg
+-rw-rw-r--   0 lordpatil  (1000) lordpatil  (1000)      731 2024-05-16 04:49:00.000000 lprocess-0.0.9/setup.py
```

### Comparing `lprocess-0.0.8/lprocess/EDA.py` & `lprocess-0.0.9/lprocess/EDA.py`

 * *Files 2% similar despite different names*

```diff
@@ -88,32 +88,34 @@
         codes = self.data[col].astype('category').cat.codes
         plt.hist(codes, density=True, histtype='stepfilled', alpha=0.5)
 
     def plot_numerical_hist(self, col):
         """
         Plot a histogram for a numerical column.
         """
-        plt.hist(self.data[col].dropna(), bins='auto', density=True, alpha=0.5)
+        plt.hist(self.data[col].dropna(),  density=True, alpha=0.5, ec="red")
 
     def plot_numerical_kde(self, col):
         """
         Plot a kernel density estimate for a numerical column.
         """
         values = self.data[col].dropna().values
         kde = self.calc_kde(values)
-        x_grid = np.linspace(values.min(), values.max(), 200)
-        plt.plot(x_grid, kde(x_grid))
+        x_grid = np.linspace(values.min(), values.max(), len(values))
+        y_grid = kde(x_grid)
+        plt.plot(x_grid, y_grid)
 
     def calc_kde(self, data):
         """
         Calculate the kernel density estimate for a given data array.
         """
         bandwidth = 1.06 * data.std() * len(data) ** (-1/5)
         kernel = self.gaussian_kernel(bandwidth)
-        return lambda x: np.mean(kernel((x - data[:, None])/bandwidth), axis=1)
+        data = data[:, np.newaxis]  # Add a new axis to make data 2D
+        return lambda x: np.mean(kernel((x - data) / bandwidth), axis=1)
 
     def gaussian_kernel(self, bandwidth):
         """
         Gaussian kernel function.
         """
         def kernel(x):
             return (1 / np.sqrt(2 * np.pi)) * np.exp(-0.5 * x**2)
@@ -145,7 +147,9 @@
         """
         print(f"Value Counts for {col}:")
         print(self.data[col].value_counts())
         plt.figure(figsize=(8, 6))
         self.plot_categorical_hist(col)
         plt.title(f"Distribution of {col}")
         plt.show()
+
+
```

### Comparing `lprocess-0.0.8/setup.py` & `lprocess-0.0.9/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
 
-VERSION = '0.0.8'
-DESCRIPTION = 'Data Preprocessing library'
+VERSION = '0.0.9'
+DESCRIPTION = 'Data Preprocessing library that makes EDA easy for all'
 
 
 # Setting up
 setup(
     name="lprocess",
     version=VERSION,
     author="Chirag Patil",
```

