# Comparing `tmp/TsingPig_Lab-0.1.3.tar.gz` & `tmp/TsingPig_Lab-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TsingPig_Lab-0.1.3.tar", last modified: Thu May 16 07:30:16 2024, max compression
+gzip compressed data, was "dist\TsingPig_Lab-0.1.4.tar", last modified: Thu May 16 07:56:17 2024, max compression
```

## Comparing `TsingPig_Lab-0.1.3.tar` & `TsingPig_Lab-0.1.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 07:30:16.058025 TsingPig_Lab-0.1.3/
--rw-rw-rw-   0        0        0     1489 2024-05-16 07:30:16.057021 TsingPig_Lab-0.1.3/PKG-INFO
--rw-rw-rw-   0        0        0      723 2024-05-16 07:30:04.000000 TsingPig_Lab-0.1.3/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 07:30:16.051967 TsingPig_Lab-0.1.3/TsingPig_Lab.egg-info/
--rw-rw-rw-   0        0        0     1489 2024-05-16 07:30:15.000000 TsingPig_Lab-0.1.3/TsingPig_Lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2024-05-16 07:30:16.000000 TsingPig_Lab-0.1.3/TsingPig_Lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 07:30:15.000000 TsingPig_Lab-0.1.3/TsingPig_Lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-16 07:30:15.000000 TsingPig_Lab-0.1.3/TsingPig_Lab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 07:30:16.058025 TsingPig_Lab-0.1.3/setup.cfg
--rw-rw-rw-   0        0        0      941 2024-05-16 06:31:47.000000 TsingPig_Lab-0.1.3/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:30:16.056018 TsingPig_Lab-0.1.3/tsingpig_lab/
--rw-rw-rw-   0        0        0     3124 2024-05-16 07:19:47.000000 TsingPig_Lab-0.1.3/tsingpig_lab/Algorithms.py
--rw-rw-rw-   0        0        0     1101 2024-05-16 06:23:09.000000 TsingPig_Lab-0.1.3/tsingpig_lab/DataStructures.py
--rw-rw-rw-   0        0        0      449 2024-05-16 07:19:58.000000 TsingPig_Lab-0.1.3/tsingpig_lab/__init__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:56:17.433478 TsingPig_Lab-0.1.4/
+-rw-rw-rw-   0        0        0     2592 2024-05-16 07:56:17.433478 TsingPig_Lab-0.1.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1674 2024-05-16 07:42:18.000000 TsingPig_Lab-0.1.4/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 07:56:17.427475 TsingPig_Lab-0.1.4/TsingPig_Lab.egg-info/
+-rw-rw-rw-   0        0        0     2592 2024-05-16 07:56:17.000000 TsingPig_Lab-0.1.4/TsingPig_Lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-05-16 07:56:17.000000 TsingPig_Lab-0.1.4/TsingPig_Lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 07:56:17.000000 TsingPig_Lab-0.1.4/TsingPig_Lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-16 07:56:17.000000 TsingPig_Lab-0.1.4/TsingPig_Lab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 07:56:17.433478 TsingPig_Lab-0.1.4/setup.cfg
+-rw-rw-rw-   0        0        0      941 2024-05-16 06:31:47.000000 TsingPig_Lab-0.1.4/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:56:17.431477 TsingPig_Lab-0.1.4/tsingpig_lab/
+-rw-rw-rw-   0        0        0     3124 2024-05-16 07:19:47.000000 TsingPig_Lab-0.1.4/tsingpig_lab/Algorithms.py
+-rw-rw-rw-   0        0        0     1322 2024-05-16 07:56:09.000000 TsingPig_Lab-0.1.4/tsingpig_lab/DataStructures.py
+-rw-rw-rw-   0        0        0      449 2024-05-16 07:56:09.000000 TsingPig_Lab-0.1.4/tsingpig_lab/__init__.py
```

### Comparing `TsingPig_Lab-0.1.3/PKG-INFO` & `TsingPig_Lab-0.1.4/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TsingPig_Lab
-Version: 0.1.3
+Version: 0.1.4
 Summary: TsingPig_Lab is a package for algorithm.
 Home-page: https://gitlab.com/tsingpig-code/tsingpig_lab
 Author: TsingPig
 Author-email: 1114196607@qq.com
 License: UNKNOWN
 Description: # TsingPig - Lab
         ## 1. Introduction
@@ -21,25 +21,44 @@
         Thanks for your support!
         
         
         
         ## 2. Functions
         ### 2.1. DataStructures
         
-        **Sparse Table (ST)**
+        #### 2.1.1 Sparse Table (ST)
         
         A data structure ST table (Sparse Table) that supports interval contribution problem queries.
         
+        **Usage**
+        
+        | Method                                               | Description                                                  |
+        | ---------------------------------------------------- | ------------------------------------------------------------ |
+        | `__init__(nums: List, opt = lambda a, b: max(a, b))` | Initialize the Sparse Table (ST) data structure with the given list of numbers and an optional comparison function. |
+        | `qry(L: int, R: int)`                                | Query the opt value within the range [L, R].                 |
+        
+        **Simple**
+        
         ``` python
-        from tsingpig_lab import DataStructures
-        st = DataStructures.ST([1, 2, 3])
-        print(st.qry(0, 2))  # 3
+        from tsingpig_lab.DataStructures import ST as ST
+        st = ST([1, 9, 0, 2, 4, 5])
+        print(st.qry(1, 3))	# 9
         ```
         
+        You can also customize comparison methods by passing function parameters. In default condition, the maximum value will be returned.
+        
+        ```python
+        from tsingpig_lab.DataStructures import ST as ST
+        st = ST([1, 9, -99, 2, 4, 5], lambda a, b: min(a, b))
+        print(st.qry(1, 4)) # -99
+        ```
+        
+        
         
+        > Please note that the issue of contribution needs to be met. It means $Opt (x, x)=x$
         
         ### 2.2. Algorithms
         
         #### 2.2.1 BaseConverter 
         
         ```python
```

### Comparing `TsingPig_Lab-0.1.3/TsingPig_Lab.egg-info/PKG-INFO` & `TsingPig_Lab-0.1.4/TsingPig_Lab.egg-info/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TsingPig-Lab
-Version: 0.1.3
+Version: 0.1.4
 Summary: TsingPig_Lab is a package for algorithm.
 Home-page: https://gitlab.com/tsingpig-code/tsingpig_lab
 Author: TsingPig
 Author-email: 1114196607@qq.com
 License: UNKNOWN
 Description: # TsingPig - Lab
         ## 1. Introduction
@@ -21,25 +21,44 @@
         Thanks for your support!
         
         
         
         ## 2. Functions
         ### 2.1. DataStructures
         
-        **Sparse Table (ST)**
+        #### 2.1.1 Sparse Table (ST)
         
         A data structure ST table (Sparse Table) that supports interval contribution problem queries.
         
+        **Usage**
+        
+        | Method                                               | Description                                                  |
+        | ---------------------------------------------------- | ------------------------------------------------------------ |
+        | `__init__(nums: List, opt = lambda a, b: max(a, b))` | Initialize the Sparse Table (ST) data structure with the given list of numbers and an optional comparison function. |
+        | `qry(L: int, R: int)`                                | Query the opt value within the range [L, R].                 |
+        
+        **Simple**
+        
         ``` python
-        from tsingpig_lab import DataStructures
-        st = DataStructures.ST([1, 2, 3])
-        print(st.qry(0, 2))  # 3
+        from tsingpig_lab.DataStructures import ST as ST
+        st = ST([1, 9, 0, 2, 4, 5])
+        print(st.qry(1, 3))	# 9
         ```
         
+        You can also customize comparison methods by passing function parameters. In default condition, the maximum value will be returned.
+        
+        ```python
+        from tsingpig_lab.DataStructures import ST as ST
+        st = ST([1, 9, -99, 2, 4, 5], lambda a, b: min(a, b))
+        print(st.qry(1, 4)) # -99
+        ```
+        
+        
         
+        > Please note that the issue of contribution needs to be met. It means $Opt (x, x)=x$
         
         ### 2.2. Algorithms
         
         #### 2.2.1 BaseConverter 
         
         ```python
```

### Comparing `TsingPig_Lab-0.1.3/setup.py` & `TsingPig_Lab-0.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `TsingPig_Lab-0.1.3/tsingpig_lab/Algorithms.py` & `TsingPig_Lab-0.1.4/tsingpig_lab/Algorithms.py`

 * *Files identical despite different names*

### Comparing `TsingPig_Lab-0.1.3/tsingpig_lab/DataStructures.py` & `TsingPig_Lab-0.1.4/tsingpig_lab/DataStructures.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import math
 from math import ceil
 from typing import List
 
 class ST:
     def __init__(self, nums: List, opt = lambda a, b: max(a, b)):
         """
-        在 O(nlogn) 的时间内预处理数组 nums，使得查询区间[L, R]opt的时间复杂度为 O(1)。
-        :param nums: 数组
-        :param opt: 比较函数，默认为最值
+        Initialize the Sparse Table (ST) data structure with the given list of numbers and an optional comparison function.
+
+        :param nums: The list of numbers to preprocess.
+        :param opt: The comparison function to use for queries. Default is max.
         """
         n = len(nums)
         log = [0] * (n + 1)
         for i in range(2, n + 1):
             log[i] = log[i >> 1] + 1
         lenj = ceil(math.log(n, 2)) + 1
         f = [[0] * lenj for _ in range(n)]
@@ -22,13 +23,17 @@
         self.f = f
         self.log = log
         self.opt = opt
 
 
     def qry(self, L: int, R: int):
         """
-        查询区间 [L, R] 的最值（时间复杂度：O(1)）
+        Query the maximum value within the range [L, R].
+
+        :param L: The left index of the range.
+        :param R: The right index of the range.
+        :return: The maximum value within the range [L, R].
         :rtype: object
         """
         k = self.log[R - L + 1]
         return self.opt(self.f[L][k], self.f[R - (1 << k) + 1][k])
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

