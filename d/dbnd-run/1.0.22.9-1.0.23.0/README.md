# Comparing `tmp/dbnd-run-1.0.22.9.tar.gz` & `tmp/dbnd_run-1.0.23.0-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-run-1.0.22.9.tar", last modified: Thu Mar 14 15:33:33 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

