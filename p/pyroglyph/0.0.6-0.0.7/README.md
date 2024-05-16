# Comparing `tmp/pyroglyph-0.0.6.tar.gz` & `tmp/pyroglyph-0.0.7-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyroglyph-0.0.6.tar", last modified: Tue Dec 10 03:23:47 2019, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

