# Comparing `tmp/klspy-2.0.2.tar.gz` & `tmp/klspy-2.0.3-cp312-cp312-macosx_11_0_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "klspy-2.0.2.tar", last modified: Fri Sep  8 06:16:42 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

