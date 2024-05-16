# Comparing `tmp/lephare-0.1.7.tar.gz` & `tmp/lephare-0.1.8-cp312-cp312-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lephare-0.1.7.tar", last modified: Wed May 15 03:33:57 2024, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

