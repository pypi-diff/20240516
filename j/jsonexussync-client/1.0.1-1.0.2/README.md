# Comparing `tmp/jsonexussync-client-1.0.1.tar.gz` & `tmp/jsonexussync_client-1.0.2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonexussync-client-1.0.1.tar", last modified: Sun Mar 10 13:39:42 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

