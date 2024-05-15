# Comparing `tmp/plone.distribution-1.0.0b4.tar.gz` & `tmp/plone.distribution-2.0.0a1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.distribution-1.0.0b4.tar", last modified: Wed Apr  3 10:04:16 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

