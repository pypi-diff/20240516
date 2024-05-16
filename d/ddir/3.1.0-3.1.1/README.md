# Comparing `tmp/ddir-3.1.0-py3-none-any.whl.zip` & `tmp/ddir-3.1.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,15 +1,15 @@
-Zip file size: 14354 bytes, number of entries: 13
--rw-r--r--  2.0 unx     4924 b- defN 24-May-10 16:32 ddir/__init__.py
--rw-r--r--  2.0 unx     4445 b- defN 24-May-10 16:32 ddir/__main__.py
--rw-r--r--  2.0 unx      156 b- defN 24-May-10 16:32 ddir/__version__.py
--rw-r--r--  2.0 unx    11931 b- defN 24-May-10 16:32 ddir/diff.py
--rw-r--r--  2.0 unx      673 b- defN 24-May-10 16:32 ddir/initialize.py
--rw-r--r--  2.0 unx     2600 b- defN 24-May-10 16:32 ddir/legacy.py
--rw-r--r--  2.0 unx     5828 b- defN 24-May-10 16:32 ddir/target.py
--rw-r--r--  2.0 unx     1211 b- defN 24-May-10 16:32 ddir-3.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     3622 b- defN 24-May-10 16:32 ddir-3.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-May-10 16:32 ddir-3.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       44 b- defN 24-May-10 16:32 ddir-3.1.0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        5 b- defN 24-May-10 16:32 ddir-3.1.0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      969 b- defN 24-May-10 16:32 ddir-3.1.0.dist-info/RECORD
-13 files, 36500 bytes uncompressed, 12764 bytes compressed:  65.0%
+Zip file size: 15004 bytes, number of entries: 13
+-rw-r--r--  2.0 unx     4924 b- defN 24-May-16 14:58 ddir/__init__.py
+-rw-r--r--  2.0 unx     4445 b- defN 24-May-16 14:58 ddir/__main__.py
+-rw-r--r--  2.0 unx      156 b- defN 24-May-16 14:58 ddir/__version__.py
+-rw-r--r--  2.0 unx    12671 b- defN 24-May-16 14:58 ddir/diff.py
+-rw-r--r--  2.0 unx      673 b- defN 24-May-16 14:58 ddir/initialize.py
+-rw-r--r--  2.0 unx     2600 b- defN 24-May-16 14:58 ddir/legacy.py
+-rw-r--r--  2.0 unx     5828 b- defN 24-May-16 14:58 ddir/target.py
+-rw-r--r--  2.0 unx     1211 b- defN 24-May-16 14:58 ddir-3.1.1.dist-info/LICENSE
+-rw-r--r--  2.0 unx     4541 b- defN 24-May-16 14:58 ddir-3.1.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-May-16 14:58 ddir-3.1.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx       44 b- defN 24-May-16 14:58 ddir-3.1.1.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        5 b- defN 24-May-16 14:58 ddir-3.1.1.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      969 b- defN 24-May-16 14:58 ddir-3.1.1.dist-info/RECORD
+13 files, 38159 bytes uncompressed, 13414 bytes compressed:  64.8%
```

## zipnote {}

```diff
@@ -15,26 +15,26 @@
 
 Filename: ddir/legacy.py
 Comment: 
 
 Filename: ddir/target.py
 Comment: 
 
-Filename: ddir-3.1.0.dist-info/LICENSE
+Filename: ddir-3.1.1.dist-info/LICENSE
 Comment: 
 
-Filename: ddir-3.1.0.dist-info/METADATA
+Filename: ddir-3.1.1.dist-info/METADATA
 Comment: 
 
-Filename: ddir-3.1.0.dist-info/WHEEL
+Filename: ddir-3.1.1.dist-info/WHEEL
 Comment: 
 
-Filename: ddir-3.1.0.dist-info/entry_points.txt
+Filename: ddir-3.1.1.dist-info/entry_points.txt
 Comment: 
 
-Filename: ddir-3.1.0.dist-info/top_level.txt
+Filename: ddir-3.1.1.dist-info/top_level.txt
 Comment: 
 
-Filename: ddir-3.1.0.dist-info/RECORD
+Filename: ddir-3.1.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## ddir/__version__.py

```diff
@@ -1,7 +1,7 @@
 """
 This module holds the version of ddir.
 
 It contains a placeholder for the version number, which is replaced by the build script.
 """
 
-VERSION = '3.1.0'
+VERSION = '3.1.1'
```

## ddir/diff.py

```diff
@@ -260,31 +260,54 @@
     else:
         source_last_changed = stat(source).st_mtime
         target_last_changed = stat(target).st_mtime
 
         source_last_changed_str = datetime.fromtimestamp(source_last_changed).isoformat()
         target_last_changed_str = datetime.fromtimestamp(target_last_changed).isoformat()
 
-        if source_last_changed > target_last_changed:
+        if not _float_sneaky_equals(source_last_changed, target_last_changed) and source_last_changed > target_last_changed:
             print(f'[metadata] files differ: {source} is newer than {target} ({source_last_changed_str} > {target_last_changed_str})')
             diff.add_diff(Diff(DiffType.NEWER, 'f', source, target))
-        elif target_last_changed > source_last_changed:
+        elif not _float_sneaky_equals(source_last_changed, target_last_changed) and target_last_changed > source_last_changed:
             print(f'[metadata] files differ: {target} is newer than {source} ({target_last_changed_str} > {source_last_changed_str})')
             diff.add_diff(Diff(DiffType.OLDER, 'f', source, target))
         elif not fast:
             with open(source, 'rb', encoding=ENCODING) as source_file, \
                     open(target, 'rb', encoding=ENCODING) as target_file:
                 source_md5 = md5(source_file.read()).hexdigest()
                 target_md5 = md5(target_file.read()).hexdigest()
 
                 if source_md5 != target_md5:
                     print(f'[content ] files differ: {source}')
                     diff.add_diff(Diff(DiffType.UNKNOWN, 'f', source, target))
 
 
+def _float_sneaky_equals(a: float, b: float) -> bool:
+    a_len_d = len(str(a).split('.')[1])
+    b_len_d = len(str(b).split('.')[1])
+
+    if a_len_d == b_len_d:
+        return 0 if a == b else 1
+
+    if a_len_d < b_len_d:
+        return a == _truncate_float(b, a_len_d)
+
+    return _truncate_float(a, b_len_d) == b
+
+
+def _truncate_float(f: float, n: int) -> float:
+    """Truncates/pads a float f to n decimal places without rounding"""
+    s = str(f)
+    if 'e' in s or 'E' in s:
+        return float(f'{0:.{f}f}')
+
+    i, _, d = s.partition('.')
+    return float('.'.join([i, (d+'0'*n)[:n]]))
+
+
 def resolve(reader: DiffFileReader, modes=(0, 0, 0, 0, 0)) -> None:
     """Resolves all diffs from a given diff file.
 
     The modes work like this: for each type (the order is "+", "-", ">", "<", "?")
     a number in the tuple indicates how to handle diffs of that type. There are
     the following modes:
         - 0: skip
```

## Comparing `ddir-3.1.0.dist-info/LICENSE` & `ddir-3.1.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ddir-3.1.0.dist-info/METADATA` & `ddir-3.1.1.dist-info/METADATA`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ddir
-Version: 3.1.0
+Version: 3.1.1
 Summary: Diff a directory and sync changes.
 License: Public Domain
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # ddir
 
@@ -14,14 +14,29 @@
 [![GitHub release](https://img.shields.io/github/release/yannickkirschen/ddir.svg)](https://github.com/yannickkirschen/ddir/releases/)
 
 `ddir` is a command line tool to calculate diffs between two directories and
 resolve them.
 
 Check out the [diff file format](#the-diff-file-format) as well.
 
+> [!IMPORTANT]
+> `ddir` uses `shutil.copy2` to copy files and directories. This function tries
+> to copy the metadata like timestamps as well. When copying data to an external
+> storage device with a different file system, there is an issue with the
+> accuracy of those timestamps:
+>
+> To determine if a file is newer or older, `ddir` uses the `st_mtime` property,
+> which is the UNIX timestamp as float. This float happens to be of a different
+> accuracy depending on the storage device and file system. On all my internal
+> devices (SSD and NVMe, APFS and ext4), the float has an accuracy of 6 decimal
+> places, but on my external devices (SSD, exFAT) it only has an accuracy of 2
+> decimal places. This causes all comparisons to be not equal and thus a file is
+> marked as modified though it isn't. This is why I implemented a sneaky
+> comparison, that cuts of the overlapping decimal places without rounding them.
+
 ## Installation
 
 `pip install ddir`
 
 This will install a binary called `ddir` on your `PATH` that you can execute.
 Depending on your system, you may need sudo/admin permissions.
```

## Comparing `ddir-3.1.0.dist-info/RECORD` & `ddir-3.1.1.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 ddir/__init__.py,sha256=hhcbMVrBNnaITOn7qp9LtkF6cXaZcwIxGh9ew2IKgsA,4924
 ddir/__main__.py,sha256=oV1gLrsOBY4j91BquC-W3m6CDSTJ-dXpICrZrjKQMgk,4445
-ddir/__version__.py,sha256=GsbCdKMqLSXfuahJcWyput_5Q6SPPkZr_1QpPqc8O7I,156
-ddir/diff.py,sha256=slS6qn1k5wJO0yrMlZdoKvzz-S_6E-qPdmc79fA8K54,11931
+ddir/__version__.py,sha256=I_Yi3h702ANpgAIAp7MxgB9Vd10cnwlnVUSyVbU0f80,156
+ddir/diff.py,sha256=6a-v1Hw8RUyhzsf8KJmvdVsH3pUelWBBj4_6gq2IJjk,12671
 ddir/initialize.py,sha256=XbgoD4YBxEsLfP5zabvuGIcOd2hAzHAYuBaPgeCY260,673
 ddir/legacy.py,sha256=shoCl9H9ZEO7Z_hh6urAyrUWzWnfgpygJsE7NIiBfGo,2600
 ddir/target.py,sha256=DK4riv1VBpjkomsulZeoc6JjPPcVL4Gp731y_ey9Oqo,5828
-ddir-3.1.0.dist-info/LICENSE,sha256=fhLl30uuEsshWBuhV87SDhmGoFCN0Q0Oikq5pM-U6Fw,1211
-ddir-3.1.0.dist-info/METADATA,sha256=yxYPMsUTPxYEtznFCPCyxk8a37l-s2zkQjISQEFXL3A,3622
-ddir-3.1.0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-ddir-3.1.0.dist-info/entry_points.txt,sha256=uEQJqxm8H6cL_TYsi1-Vd7vdRnesOSVPbnr4noyXnwE,44
-ddir-3.1.0.dist-info/top_level.txt,sha256=F7NGOmHjOI4UseDtkAR3bTsbwIxLi4Gy8KaMMpIl6Ws,5
-ddir-3.1.0.dist-info/RECORD,,
+ddir-3.1.1.dist-info/LICENSE,sha256=fhLl30uuEsshWBuhV87SDhmGoFCN0Q0Oikq5pM-U6Fw,1211
+ddir-3.1.1.dist-info/METADATA,sha256=nOLx4x_JtC5_X_4MR2CAj8k5ZCPx4SALefg1FxlZeKs,4541
+ddir-3.1.1.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+ddir-3.1.1.dist-info/entry_points.txt,sha256=uEQJqxm8H6cL_TYsi1-Vd7vdRnesOSVPbnr4noyXnwE,44
+ddir-3.1.1.dist-info/top_level.txt,sha256=F7NGOmHjOI4UseDtkAR3bTsbwIxLi4Gy8KaMMpIl6Ws,5
+ddir-3.1.1.dist-info/RECORD,,
```

