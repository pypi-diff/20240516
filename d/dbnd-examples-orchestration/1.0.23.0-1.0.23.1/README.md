# Comparing `tmp/dbnd-examples-orchestration-1.0.23.0.tar.gz` & `tmp/dbnd_examples_orchestration-1.0.23.1-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbnd-examples-orchestration-1.0.23.0.tar", last modified: Tue May  7 15:42:12 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

