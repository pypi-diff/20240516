# Comparing `tmp/TsingPig_Lab-0.1.2.tar.gz` & `tmp/TsingPig_Lab-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\TsingPig_Lab-0.1.2.tar", last modified: Thu May 16 07:10:23 2024, max compression
+gzip compressed data, was "dist\TsingPig_Lab-0.1.3.tar", last modified: Thu May 16 07:30:16 2024, max compression
```

## Comparing `TsingPig_Lab-0.1.2.tar` & `TsingPig_Lab-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 07:10:23.698287 TsingPig_Lab-0.1.2/
--rw-rw-rw-   0        0        0      804 2024-05-16 07:10:23.697286 TsingPig_Lab-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      255 2024-05-16 06:23:09.000000 TsingPig_Lab-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 07:10:23.689801 TsingPig_Lab-0.1.2/TsingPig_Lab.egg-info/
--rw-rw-rw-   0        0        0      804 2024-05-16 07:10:23.000000 TsingPig_Lab-0.1.2/TsingPig_Lab.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      285 2024-05-16 07:10:23.000000 TsingPig_Lab-0.1.2/TsingPig_Lab.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 07:10:23.000000 TsingPig_Lab-0.1.2/TsingPig_Lab.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       13 2024-05-16 07:10:23.000000 TsingPig_Lab-0.1.2/TsingPig_Lab.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-05-16 07:10:23.698287 TsingPig_Lab-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0      941 2024-05-16 06:31:47.000000 TsingPig_Lab-0.1.2/setup.py
-drwxrwxrwx   0        0        0        0 2024-05-16 07:10:23.696287 TsingPig_Lab-0.1.2/tsingpig_lab/
--rw-rw-rw-   0        0        0     2075 2024-05-16 07:06:31.000000 TsingPig_Lab-0.1.2/tsingpig_lab/BaseConverter.py
--rw-rw-rw-   0        0        0      413 2024-05-16 07:06:31.000000 TsingPig_Lab-0.1.2/tsingpig_lab/Bin.py
--rw-rw-rw-   0        0        0     1101 2024-05-16 06:23:09.000000 TsingPig_Lab-0.1.2/tsingpig_lab/ST.py
--rw-rw-rw-   0        0        0      260 2024-05-16 07:10:16.000000 TsingPig_Lab-0.1.2/tsingpig_lab/__init__.py
--rw-rw-rw-   0        0        0      195 2024-05-16 07:09:51.000000 TsingPig_Lab-0.1.2/tsingpig_lab/tsingpig_lab.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:30:16.058025 TsingPig_Lab-0.1.3/
+-rw-rw-rw-   0        0        0     1489 2024-05-16 07:30:16.057021 TsingPig_Lab-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2024-05-16 07:30:04.000000 TsingPig_Lab-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 07:30:16.051967 TsingPig_Lab-0.1.3/TsingPig_Lab.egg-info/
+-rw-rw-rw-   0        0        0     1489 2024-05-16 07:30:15.000000 TsingPig_Lab-0.1.3/TsingPig_Lab.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2024-05-16 07:30:16.000000 TsingPig_Lab-0.1.3/TsingPig_Lab.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 07:30:15.000000 TsingPig_Lab-0.1.3/TsingPig_Lab.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       13 2024-05-16 07:30:15.000000 TsingPig_Lab-0.1.3/TsingPig_Lab.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-05-16 07:30:16.058025 TsingPig_Lab-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0      941 2024-05-16 06:31:47.000000 TsingPig_Lab-0.1.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 07:30:16.056018 TsingPig_Lab-0.1.3/tsingpig_lab/
+-rw-rw-rw-   0        0        0     3124 2024-05-16 07:19:47.000000 TsingPig_Lab-0.1.3/tsingpig_lab/Algorithms.py
+-rw-rw-rw-   0        0        0     1101 2024-05-16 06:23:09.000000 TsingPig_Lab-0.1.3/tsingpig_lab/DataStructures.py
+-rw-rw-rw-   0        0        0      449 2024-05-16 07:19:58.000000 TsingPig_Lab-0.1.3/tsingpig_lab/__init__.py
```

### Comparing `TsingPig_Lab-0.1.2/setup.py` & `TsingPig_Lab-0.1.3/setup.py`

 * *Files identical despite different names*

### Comparing `TsingPig_Lab-0.1.2/tsingpig_lab/BaseConverter.py` & `TsingPig_Lab-0.1.3/tsingpig_lab/Algorithms.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+
+
+# 进制转换器
 class BaseConverter:
     def __init__(self, a: int, b: int):
         """
         将a进制的数字转换为b进制的数字
         :param a: 原数是a进制
         :param b: 转换后为b进制
         """
@@ -66,9 +69,45 @@
         """
         if n < 10:
             return str(n)
         else:
             return chr(ord('A') + n - 10)
 
 
-# baseCon = BaseConverter(2, 10)
-# print(baseCon.convert('-111'))
+# 二进制码转换器
+class Bin():
+    def __init__(self, num: str, b: int = 2):
+        """
+        :param num: 数字字符串
+        :param base: num的进制，默认为10
+        """
+        if b != 2:
+            num = BaseConverter(b, 2).convert(num)
+        self.num = num
+
+    def grey_to_bin(self) -> str:
+        """
+        将当前的二进制码视为格雷码，求解其对应的二进制码
+        :return: 对应的二进制码
+        """
+        num = self.num
+        if num[0] == '-': num = num[1:]
+        res = num[0]
+        n = len(num)
+        for i in range(1, n):
+            res += str(int(res[-1]) ^ int(num[i]))
+        return res
+
+
+    def bin_to_grey(self) -> str:
+        """
+        将当前的二进制码视为二进制码，求解其对应的格雷码
+        :return: 对应的格雷码
+        """
+        num = self.num
+        if num[0] == '-': num = num[1:]
+        n = len(num)
+        res = num[0]
+        for i in range(1, n):
+            res += str(int(num[i - 1]) ^ int(num[i]))
+        return res
+
```

### Comparing `TsingPig_Lab-0.1.2/tsingpig_lab/ST.py` & `TsingPig_Lab-0.1.3/tsingpig_lab/DataStructures.py`

 * *Files identical despite different names*

