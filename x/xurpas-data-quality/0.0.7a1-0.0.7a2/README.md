# Comparing `tmp/xurpas_data_quality-0.0.7a1.tar.gz` & `tmp/xurpas_data_quality-0.0.7a2-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xurpas_data_quality-0.0.7a1.tar", last modified: Thu May 16 07:00:02 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

