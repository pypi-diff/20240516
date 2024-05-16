# Comparing `tmp/oppe-0.2.1-py3-none-any.whl.zip` & `tmp/oppe-0.2.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 5455 bytes, number of entries: 10
--rw-r--r--  2.0 unx      108 b- defN 23-Sep-17 20:39 oppe/__init__.py
--rw-r--r--  2.0 unx      643 b- defN 23-Sep-17 20:39 oppe/config.py
--rw-r--r--  2.0 unx      582 b- defN 23-Sep-17 20:39 oppe/exceptions.py
--rw-r--r--  2.0 unx     2766 b- defN 23-Sep-17 20:39 oppe/oppe.py
--rw-r--r--  2.0 unx     1641 b- defN 23-Sep-17 20:39 oppe/utils.py
--rw-r--r--  2.0 unx     1068 b- defN 23-Sep-17 20:39 oppe-0.2.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1789 b- defN 23-Sep-17 20:39 oppe-0.2.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Sep-17 20:39 oppe-0.2.1.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-Sep-17 20:39 oppe-0.2.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      725 b- defN 23-Sep-17 20:39 oppe-0.2.1.dist-info/RECORD
-10 files, 9419 bytes uncompressed, 4239 bytes compressed:  55.0%
+Zip file size: 5458 bytes, number of entries: 10
+-rw-r--r--  2.0 unx      108 b- defN 23-Dec-10 19:58 oppe/__init__.py
+-rw-r--r--  2.0 unx      643 b- defN 23-Dec-10 19:58 oppe/config.py
+-rw-r--r--  2.0 unx      582 b- defN 23-Dec-10 19:58 oppe/exceptions.py
+-rw-r--r--  2.0 unx     2766 b- defN 23-Dec-10 19:58 oppe/oppe.py
+-rw-r--r--  2.0 unx     1641 b- defN 23-Dec-10 19:58 oppe/utils.py
+-rw-r--r--  2.0 unx     1068 b- defN 23-Dec-10 19:58 oppe-0.2.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1789 b- defN 23-Dec-10 19:58 oppe-0.2.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-Dec-10 19:58 oppe-0.2.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-Dec-10 19:58 oppe-0.2.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      725 b- defN 23-Dec-10 19:58 oppe-0.2.2.dist-info/RECORD
+10 files, 9419 bytes uncompressed, 4242 bytes compressed:  55.0%
```

## zipnote {}

```diff
@@ -9,23 +9,23 @@
 
 Filename: oppe/oppe.py
 Comment: 
 
 Filename: oppe/utils.py
 Comment: 
 
-Filename: oppe-0.2.1.dist-info/LICENSE
+Filename: oppe-0.2.2.dist-info/LICENSE
 Comment: 
 
-Filename: oppe-0.2.1.dist-info/METADATA
+Filename: oppe-0.2.2.dist-info/METADATA
 Comment: 
 
-Filename: oppe-0.2.1.dist-info/WHEEL
+Filename: oppe-0.2.2.dist-info/WHEEL
 Comment: 
 
-Filename: oppe-0.2.1.dist-info/top_level.txt
+Filename: oppe-0.2.2.dist-info/top_level.txt
 Comment: 
 
-Filename: oppe-0.2.1.dist-info/RECORD
+Filename: oppe-0.2.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## oppe/__init__.py

```diff
@@ -1,6 +1,6 @@
 """Init file for oppe"""
 
 from oppe.oppe import Oppe  # noqa: F401
 
 __name__ = 'oppe'
-__version__ = '0.2.1'
+__version__ = '0.2.2'
```

## Comparing `oppe-0.2.1.dist-info/LICENSE` & `oppe-0.2.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `oppe-0.2.1.dist-info/METADATA` & `oppe-0.2.2.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oppe
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python API Wrapper for Oppe
 Home-page: https://github.com/kilobyteno/oppe-for-python
 Author: Kilobyte AS
 License: MIT
 Project-URL: Homepage, https://oppe.app
 Project-URL: Documentation, https://docs.oppe.app
 Project-URL: Github, https://github.com/kilobyteno/oppe-for-python
```

