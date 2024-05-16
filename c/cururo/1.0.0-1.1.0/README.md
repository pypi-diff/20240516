# Comparing `tmp/cururo-1.0.0.tar.gz` & `tmp/cururo-1.1.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cururo-1.0.0.tar", last modified: Tue May 14 20:13:34 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

