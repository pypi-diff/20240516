# Comparing `tmp/mlscat-0.0.8.tar.gz` & `tmp/mlscat-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlscat-0.0.8.tar", last modified: Wed May 15 13:37:44 2024, max compression
+gzip compressed data, was "mlscat-0.0.9.tar", last modified: Thu May 16 04:06:47 2024, max compression
```

## Comparing `mlscat-0.0.8.tar` & `mlscat-0.0.9.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-05-15 13:37:44.280662 mlscat-0.0.8/
--rw-r--r--   0 M0nk3y    (1021) M0nk3y    (1021)      776 2024-05-15 13:37:44.280662 mlscat-0.0.8/PKG-INFO
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      523 2024-04-17 06:13:37.000000 mlscat-0.0.8/README.md
-drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-05-15 13:37:44.280662 mlscat-0.0.8/mlscat/
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)       41 2024-05-15 13:35:57.000000 mlscat-0.0.8/mlscat/__init__.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     2972 2024-05-15 12:27:06.000000 mlscat-0.0.8/mlscat/attacks.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1573 2024-05-15 13:35:36.000000 mlscat-0.0.8/mlscat/data.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1024 2024-05-15 12:27:54.000000 mlscat-0.0.8/mlscat/leakage.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      986 2024-05-15 12:56:33.000000 mlscat-0.0.8/mlscat/preprocess.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1993 2024-05-15 12:07:34.000000 mlscat-0.0.8/mlscat/security.py
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)    25946 2024-05-15 12:35:40.000000 mlscat-0.0.8/mlscat/utils.py
-drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-05-15 13:37:44.280662 mlscat-0.0.8/mlscat.egg-info/
--rw-r--r--   0 M0nk3y    (1021) M0nk3y    (1021)      776 2024-05-15 13:37:44.000000 mlscat-0.0.8/mlscat.egg-info/PKG-INFO
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      293 2024-05-15 13:37:44.000000 mlscat-0.0.8/mlscat.egg-info/SOURCES.txt
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        1 2024-05-15 13:37:44.000000 mlscat-0.0.8/mlscat.egg-info/dependency_links.txt
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        6 2024-05-15 13:37:44.000000 mlscat-0.0.8/mlscat.egg-info/requires.txt
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        7 2024-05-15 13:37:44.000000 mlscat-0.0.8/mlscat.egg-info/top_level.txt
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)       38 2024-05-15 13:37:44.280662 mlscat-0.0.8/setup.cfg
--rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      590 2024-04-17 12:37:41.000000 mlscat-0.0.8/setup.py
+drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-05-16 04:06:47.445720 mlscat-0.0.9/
+-rw-r--r--   0 M0nk3y    (1021) M0nk3y    (1021)      820 2024-05-16 04:06:47.445720 mlscat-0.0.9/PKG-INFO
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      523 2024-04-17 06:13:37.000000 mlscat-0.0.9/README.md
+drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-05-16 04:06:47.441720 mlscat-0.0.9/mlscat/
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      102 2024-05-16 04:06:20.000000 mlscat-0.0.9/mlscat/__init__.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     2972 2024-05-15 13:48:29.000000 mlscat-0.0.9/mlscat/attacks.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1573 2024-05-15 13:35:36.000000 mlscat-0.0.9/mlscat/data.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1075 2024-05-16 04:06:35.000000 mlscat-0.0.9/mlscat/dpreprocess.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1024 2024-05-15 12:27:54.000000 mlscat-0.0.9/mlscat/leakage.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)     1993 2024-05-15 12:07:34.000000 mlscat-0.0.9/mlscat/security.py
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)    25946 2024-05-15 12:35:40.000000 mlscat-0.0.9/mlscat/utils.py
+drwxrwxr-x   0 M0nk3y    (1021) M0nk3y    (1021)        0 2024-05-16 04:06:47.445720 mlscat-0.0.9/mlscat.egg-info/
+-rw-r--r--   0 M0nk3y    (1021) M0nk3y    (1021)      820 2024-05-16 04:06:47.000000 mlscat-0.0.9/mlscat.egg-info/PKG-INFO
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      294 2024-05-16 04:06:47.000000 mlscat-0.0.9/mlscat.egg-info/SOURCES.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        1 2024-05-16 04:06:47.000000 mlscat-0.0.9/mlscat.egg-info/dependency_links.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        6 2024-05-16 04:06:47.000000 mlscat-0.0.9/mlscat.egg-info/requires.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)        7 2024-05-16 04:06:47.000000 mlscat-0.0.9/mlscat.egg-info/top_level.txt
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)       38 2024-05-16 04:06:47.445720 mlscat-0.0.9/setup.cfg
+-rw-rw-r--   0 M0nk3y    (1021) M0nk3y    (1021)      634 2024-05-16 03:34:02.000000 mlscat-0.0.9/setup.py
```

### Comparing `mlscat-0.0.8/PKG-INFO` & `mlscat-0.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: mlscat
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small cat help you enjoy your side channel attack journal!
+Home-page: https://github.com/i4mhmh/mlscat
 Author: i4mhmh
 Author-email: i4mhmh@outlook.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 
 # MLSCAT
```

### Comparing `mlscat-0.0.8/README.md` & `mlscat-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `mlscat-0.0.8/mlscat/attacks.py` & `mlscat-0.0.9/mlscat/attacks.py`

 * *Files identical despite different names*

### Comparing `mlscat-0.0.8/mlscat/data.py` & `mlscat-0.0.9/mlscat/data.py`

 * *Files identical despite different names*

### Comparing `mlscat-0.0.8/mlscat/leakage.py` & `mlscat-0.0.9/mlscat/leakage.py`

 * *Files identical despite different names*

### Comparing `mlscat-0.0.8/mlscat/preprocess.py` & `mlscat-0.0.9/mlscat/dpreprocess.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,48 +1,48 @@
-import numpy as np
-from sklearn import preprocessing
+# import numpy as np
+# from sklearn import preprocessing
 
-'''
-This is data preprocess module.
-'''
-
-def minmax(x, y, data):
-    '''
-    ### minmax
+# '''
+# This is data preprocess module.
+# '''
+
+# def minmax(x, y, data) -> np.ndarray:
+#     '''
+#     ### minmax
     
-    `A function scale the data to x, y`
+#     `A function scale the data to x, y`
     
-    Args:
-    `x`: begain.
-    `y`: end.
-    `data`: scaled data.
+#     Args:
+#     `x`: begain.
+#     `y`: end.
+#     `data`: scaled data.
     
-    Returns:
-        data array.
-    '''
+#     Returns:
+#         data array.
+#     '''
 
-    scale = preprocessing.MinMaxScaler(feature_range=(x, y))
-    scaled_data = scale.fit_transform(data)
-    return scaled_data
+#     scale = preprocessing.MinMaxScaler(feature_range=(x, y))
+#     scaled_data = scale.fit_transform(data)
+#     return scaled_data
 
 
-def convert_bin_label(labels) -> np.ndarray:
-    '''
-    ### convert_bin_label   
+# def convert_bin_label(labels) -> np.ndarray:
+#     '''
+#     ### convert_bin_label   
 
-    Args:
-    `labels`: normal labels array.
+#     Args:
+#     `labels`: normal labels array.
 
-    Returns:
-        bin labels array.
+#     Returns:
+#         bin labels array.
         
-    Examples:
-    >>> convert_bin_label([10,2])
-    array[[0. 0. 0. 0. 1. 0. 1. 0.]
-          [0. 0. 0. 0. 0. 0. 1. 0.]]
-    '''
-    result = np.zeros(shape=(len(labels), 8))
-    for index, label in enumerate(labels):
-        bin_label = bin(int(label))[2:].zfill(8)
-        bin_arr_label = [int(x) for x in bin_label]
-        result[index] = bin_arr_label
-    return result
+#     Examples:
+#     >>> convert_bin_label([10,2])
+#     array[[0. 0. 0. 0. 1. 0. 1. 0.]
+#           [0. 0. 0. 0. 0. 0. 1. 0.]]
+#     '''
+#     result = np.zeros(shape=(len(labels), 8))
+#     for index, label in enumerate(labels):
+#         bin_label = bin(int(label))[2:].zfill(8)
+#         bin_arr_label = [int(x) for x in bin_label]
+#         result[index] = bin_arr_label
+#     return result
```

### Comparing `mlscat-0.0.8/mlscat/security.py` & `mlscat-0.0.9/mlscat/security.py`

 * *Files identical despite different names*

### Comparing `mlscat-0.0.8/mlscat/utils.py` & `mlscat-0.0.9/mlscat/utils.py`

 * *Files identical despite different names*

### Comparing `mlscat-0.0.8/mlscat.egg-info/PKG-INFO` & `mlscat-0.0.9/mlscat.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: mlscat
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small cat help you enjoy your side channel attack journal!
+Home-page: https://github.com/i4mhmh/mlscat
 Author: i4mhmh
 Author-email: i4mhmh@outlook.com
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: numpy
 
 # MLSCAT
```

### Comparing `mlscat-0.0.8/setup.py` & `mlscat-0.0.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,9 +15,10 @@
         'numpy',
     ],
     author="i4mhmh",
     author_email='i4mhmh@outlook.com',
     description='A small cat help you enjoy your side channel attack journal!',
     long_description=long_description,
     long_description_content_type="text/markdown",
+    url="https://github.com/i4mhmh/mlscat",
     python_requires = ">=3.8"
 )
```

