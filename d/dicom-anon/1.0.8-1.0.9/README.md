# Comparing `tmp/dicom-anon-1.0.8.tar.gz` & `tmp/dicom-anon-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dicom-anon-1.0.8.tar", last modified: Fri Mar  1 17:19:00 2024, max compression
+gzip compressed data, was "dicom-anon-1.0.9.tar", last modified: Fri Mar  1 19:56:02 2024, max compression
```

## Comparing `dicom-anon-1.0.8.tar` & `dicom-anon-1.0.9.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1459 2021-05-08 13:12:20.530786 dicom-anon-1.0.8/LICENSE
--rw-r--r--   0        0        0     9457 2021-05-08 20:33:49.995842 dicom-anon-1.0.8/README.md
--rw-r--r--   0        0        0        0 2024-03-01 17:16:10.631166 dicom-anon-1.0.8/dicomanonymizer/__init__.py
--rw-r--r--   0        0        0     6133 2024-03-01 16:43:30.217386 dicom-anon-1.0.8/dicomanonymizer/anonymizer.py
--rw-r--r--   0        0        0    13206 2024-03-01 16:43:22.497430 dicom-anon-1.0.8/dicomanonymizer/dicomfields.py
--rw-r--r--   0        0        0    10930 2024-03-01 16:43:32.897371 dicom-anon-1.0.8/dicomanonymizer/simpledicomanonymizer.py
--rw-r--r--   0        0        0       22 2024-03-01 17:16:10.631166 dicom-anon-1.0.8/dicomanonymizer/version.py
--rw-r--r--   0        0        0     1787 2024-03-01 17:16:17.547255 dicom-anon-1.0.8/pyproject.toml
--rw-r--r--   0        0        0       34 2024-03-01 17:16:10.631166 dicom-anon-1.0.8/tests/test.py
--rw-r--r--   0        0        0     9795 1970-01-01 00:00:00.000000 dicom-anon-1.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1459 2024-03-01 19:55:42.543957 dicom-anon-1.0.9/LICENSE
+-rw-r--r--   0        0        0     9457 2024-03-01 19:55:42.543957 dicom-anon-1.0.9/README.md
+-rw-r--r--   0        0        0        0 2024-03-01 19:55:42.543957 dicom-anon-1.0.9/dicomanonymizer/__init__.py
+-rw-r--r--   0        0        0     6133 2024-03-01 19:55:42.543957 dicom-anon-1.0.9/dicomanonymizer/anonymizer.py
+-rw-r--r--   0        0        0    13206 2024-03-01 19:55:42.543957 dicom-anon-1.0.9/dicomanonymizer/dicomfields.py
+-rw-r--r--   0        0        0    10930 2024-03-01 19:55:42.543957 dicom-anon-1.0.9/dicomanonymizer/simpledicomanonymizer.py
+-rw-r--r--   0        0        0       22 2024-03-01 19:55:42.543957 dicom-anon-1.0.9/dicomanonymizer/version.py
+-rw-r--r--   0        0        0     1787 2024-03-01 19:55:42.543957 dicom-anon-1.0.9/pyproject.toml
+-rw-r--r--   0        0        0       34 2024-03-01 19:55:42.543957 dicom-anon-1.0.9/tests/test.py
+-rw-r--r--   0        0        0     9795 1970-01-01 00:00:00.000000 dicom-anon-1.0.9/PKG-INFO
```

### Comparing `dicom-anon-1.0.8/LICENSE` & `dicom-anon-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dicom-anon-1.0.8/README.md` & `dicom-anon-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `dicom-anon-1.0.8/dicomanonymizer/anonymizer.py` & `dicom-anon-1.0.9/dicomanonymizer/anonymizer.py`

 * *Files identical despite different names*

### Comparing `dicom-anon-1.0.8/dicomanonymizer/dicomfields.py` & `dicom-anon-1.0.9/dicomanonymizer/dicomfields.py`

 * *Files identical despite different names*

### Comparing `dicom-anon-1.0.8/dicomanonymizer/simpledicomanonymizer.py` & `dicom-anon-1.0.9/dicomanonymizer/simpledicomanonymizer.py`

 * *Files identical despite different names*

### Comparing `dicom-anon-1.0.8/pyproject.toml` & `dicom-anon-1.0.9/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "pydicom",
     "tqdm",
     "setuptools>=69.0.2",
 ]
 requires-python = ">=3.8"
 readme = "README.md"
 dynamic = []
-version = "1.0.8"
+version = "1.0.9"
 
 [project.license]
 text = "Apache"
 
 [project.scripts]
 dicom-anonymizer = "dicomanonymizer.anonymizer:main"
```

### Comparing `dicom-anon-1.0.8/PKG-INFO` & `dicom-anon-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dicom-anon
-Version: 1.0.8
+Version: 1.0.9
 Summary: Program to anonymize dicom files with default and custom rules
 License: Apache
 Author-email: Laurenn Lam <laurenn.lam@kitware.com>,Scott Chase Waggener <chase@medcognetics.com>,Tim Cogan <tim@medcognetics.com>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # DicomAnonymizer
```

