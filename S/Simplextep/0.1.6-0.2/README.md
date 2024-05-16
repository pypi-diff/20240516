# Comparing `tmp/simplextep-0.1.6.tar.gz` & `tmp/Simplextep-0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplextep-0.1.6.tar", last modified: Thu May 16 07:33:55 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

