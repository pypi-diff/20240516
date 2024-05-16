# Comparing `tmp/vnerrant-1.0.1rc3.tar.gz` & `tmp/vnerrant-1.0.1rc4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vnerrant-1.0.1rc3.tar", last modified: Sun May 12 18:08:05 2024, max compression
+gzip compressed data, was "vnerrant-1.0.1rc4.tar", last modified: Thu May 16 03:16:45 2024, max compression
```

## Comparing `vnerrant-1.0.1rc3.tar` & `vnerrant-1.0.1rc4.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 18:08:05.355002 vnerrant-1.0.1rc3/
--rw-r--r--   0 manred1997   (501) staff       (20)      101 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/MANIFEST.in
--rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-05-12 18:08:05.354753 vnerrant-1.0.1rc3/PKG-INFO
--rw-r--r--   0 manred1997   (501) staff       (20)     9342 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc3/README.md
--rw-r--r--   0 manred1997   (501) staff       (20)       38 2024-05-12 18:08:05.355046 vnerrant-1.0.1rc3/setup.cfg
--rw-r--r--   0 manred1997   (501) staff       (20)     1527 2024-05-12 18:07:15.000000 vnerrant-1.0.1rc3/setup.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 18:08:05.337072 vnerrant-1.0.1rc3/tests/
--rw-r--r--   0 manred1997   (501) staff       (20)     6916 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc3/tests/test_vnerrant.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 18:08:05.338521 vnerrant-1.0.1rc3/vnerrant/
--rw-r--r--   0 manred1997   (501) staff       (20)     1079 2024-05-12 18:07:17.000000 vnerrant-1.0.1rc3/vnerrant/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    11976 2024-05-12 18:00:06.000000 vnerrant-1.0.1rc3/vnerrant/annotator.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 18:08:05.340035 vnerrant-1.0.1rc3/vnerrant/cli/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/cli/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10307 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/cli/convert.py
--rw-r--r--   0 manred1997   (501) staff       (20)     4512 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/cli/evaluate.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 18:08:05.342128 vnerrant-1.0.1rc3/vnerrant/components/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/components/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     9008 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/components/alignment.py
--rw-r--r--   0 manred1997   (501) staff       (20)      479 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/components/classifier.py
--rw-r--r--   0 manred1997   (501) staff       (20)     6382 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc3/vnerrant/components/converter.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 18:08:05.344114 vnerrant-1.0.1rc3/vnerrant/components/en/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/components/en/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    31652 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc3/vnerrant/components/en/classifier.py
--rw-r--r--   0 manred1997   (501) staff       (20)     3082 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/components/en/constants.py
--rw-r--r--   0 manred1997   (501) staff       (20)     1886 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc3/vnerrant/components/en/explainer.py
--rw-r--r--   0 manred1997   (501) staff       (20)    12286 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/components/en/lancaster.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10931 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc3/vnerrant/components/en/merger.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 18:08:05.345655 vnerrant-1.0.1rc3/vnerrant/components/en/resources/
--rw-r--r--   0 manred1997   (501) staff       (20)     1035 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/components/en/resources/README.md
--rw-r--r--   0 manred1997   (501) staff       (20)      394 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/components/en/resources/en-ptb_map
--rw-r--r--   0 manred1997   (501) staff       (20)  1839291 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/components/en/resources/en_GB-large.txt
--rw-r--r--   0 manred1997   (501) staff       (20)     1595 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/components/en/utils.py
--rw-r--r--   0 manred1997   (501) staff       (20)     9042 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/components/evaluater.py
--rw-r--r--   0 manred1997   (501) staff       (20)      200 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc3/vnerrant/components/explainer.py
--rw-r--r--   0 manred1997   (501) staff       (20)     3188 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc3/vnerrant/components/merger.py
--rw-r--r--   0 manred1997   (501) staff       (20)     2510 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/components/tokenizer.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 18:08:05.351333 vnerrant-1.0.1rc3/vnerrant/config/
--rw-r--r--   0 manred1997   (501) staff       (20)     2187 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc3/vnerrant/config/errant_verbose.json
--rw-r--r--   0 manred1997   (501) staff       (20)      532 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/config/mapping_type_error.yaml
--rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/config.py
--rw-r--r--   0 manred1997   (501) staff       (20)     1981 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc3/vnerrant/constants.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 18:08:05.351735 vnerrant-1.0.1rc3/vnerrant/metrics/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/metrics/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     2567 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/metrics/criteria.py
--rw-r--r--   0 manred1997   (501) staff       (20)      389 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/metrics/stats.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 18:08:05.352392 vnerrant-1.0.1rc3/vnerrant/model/
--rw-r--r--   0 manred1997   (501) staff       (20)       52 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc3/vnerrant/model/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)    10929 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc3/vnerrant/model/edit.py
--rw-r--r--   0 manred1997   (501) staff       (20)      556 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/run_cli.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 18:08:05.354282 vnerrant-1.0.1rc3/vnerrant/utils/
--rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/utils/__init__.py
--rw-r--r--   0 manred1997   (501) staff       (20)     7287 2024-05-12 18:05:36.000000 vnerrant-1.0.1rc3/vnerrant/utils/edit_utils.py
--rw-r--r--   0 manred1997   (501) staff       (20)      647 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/utils/helper.py
--rw-r--r--   0 manred1997   (501) staff       (20)     4516 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/utils/pretty_results.py
--rw-r--r--   0 manred1997   (501) staff       (20)     7720 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc3/vnerrant/utils/string_utils.py
--rw-r--r--   0 manred1997   (501) staff       (20)     1181 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc3/vnerrant/utils/utils.py
-drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-12 18:08:05.354521 vnerrant-1.0.1rc3/vnerrant.egg-info/
--rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-05-12 18:08:05.000000 vnerrant-1.0.1rc3/vnerrant.egg-info/PKG-INFO
--rw-r--r--   0 manred1997   (501) staff       (20)     1446 2024-05-12 18:08:05.000000 vnerrant-1.0.1rc3/vnerrant.egg-info/SOURCES.txt
--rw-r--r--   0 manred1997   (501) staff       (20)        1 2024-05-12 18:08:05.000000 vnerrant-1.0.1rc3/vnerrant.egg-info/dependency_links.txt
--rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-05-12 18:08:05.000000 vnerrant-1.0.1rc3/vnerrant.egg-info/entry_points.txt
--rw-r--r--   0 manred1997   (501) staff       (20)       26 2024-05-12 18:08:05.000000 vnerrant-1.0.1rc3/vnerrant.egg-info/requires.txt
--rw-r--r--   0 manred1997   (501) staff       (20)        9 2024-05-12 18:08:05.000000 vnerrant-1.0.1rc3/vnerrant.egg-info/top_level.txt
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.901372 vnerrant-1.0.1rc4/
+-rw-r--r--   0 manred1997   (501) staff       (20)      101 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/MANIFEST.in
+-rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-05-16 03:16:45.901085 vnerrant-1.0.1rc4/PKG-INFO
+-rw-r--r--   0 manred1997   (501) staff       (20)     9342 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/README.md
+-rw-r--r--   0 manred1997   (501) staff       (20)       38 2024-05-16 03:16:45.901422 vnerrant-1.0.1rc4/setup.cfg
+-rw-r--r--   0 manred1997   (501) staff       (20)     1527 2024-05-16 03:14:49.000000 vnerrant-1.0.1rc4/setup.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.883010 vnerrant-1.0.1rc4/tests/
+-rw-r--r--   0 manred1997   (501) staff       (20)     6916 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc4/tests/test_vnerrant.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.884563 vnerrant-1.0.1rc4/vnerrant/
+-rw-r--r--   0 manred1997   (501) staff       (20)     1079 2024-05-16 03:15:01.000000 vnerrant-1.0.1rc4/vnerrant/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    12029 2024-05-16 03:12:28.000000 vnerrant-1.0.1rc4/vnerrant/annotator.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.886062 vnerrant-1.0.1rc4/vnerrant/cli/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/cli/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10307 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/cli/convert.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     4512 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/cli/evaluate.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.888423 vnerrant-1.0.1rc4/vnerrant/components/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     9008 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/alignment.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      479 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/classifier.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     6382 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/components/converter.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.890421 vnerrant-1.0.1rc4/vnerrant/components/en/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/en/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    31652 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/components/en/classifier.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     3082 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/en/constants.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     1886 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/components/en/explainer.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    12286 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/en/lancaster.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10931 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/components/en/merger.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.891052 vnerrant-1.0.1rc4/vnerrant/components/en/resources/
+-rw-r--r--   0 manred1997   (501) staff       (20)     1035 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/en/resources/README.md
+-rw-r--r--   0 manred1997   (501) staff       (20)      394 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/en/resources/en-ptb_map
+-rw-r--r--   0 manred1997   (501) staff       (20)  1839291 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/en/resources/en_GB-large.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)     1595 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/en/utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     9042 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/evaluater.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      200 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/components/explainer.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     3188 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/components/merger.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     2510 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/components/tokenizer.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.896251 vnerrant-1.0.1rc4/vnerrant/config/
+-rw-r--r--   0 manred1997   (501) staff       (20)     2187 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/config/errant_verbose.json
+-rw-r--r--   0 manred1997   (501) staff       (20)      532 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/config/mapping_type_error.yaml
+-rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/config.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     1981 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/constants.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.896922 vnerrant-1.0.1rc4/vnerrant/metrics/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/metrics/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     2567 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/metrics/criteria.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      389 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/metrics/stats.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.898380 vnerrant-1.0.1rc4/vnerrant/model/
+-rw-r--r--   0 manred1997   (501) staff       (20)       52 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc4/vnerrant/model/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)    10929 2024-04-28 06:50:25.000000 vnerrant-1.0.1rc4/vnerrant/model/edit.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      556 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/run_cli.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.900581 vnerrant-1.0.1rc4/vnerrant/utils/
+-rw-r--r--   0 manred1997   (501) staff       (20)        0 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/utils/__init__.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     7243 2024-05-16 03:11:45.000000 vnerrant-1.0.1rc4/vnerrant/utils/edit_utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)      647 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/utils/helper.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     4516 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/utils/pretty_results.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     7720 2024-04-28 06:29:25.000000 vnerrant-1.0.1rc4/vnerrant/utils/string_utils.py
+-rw-r--r--   0 manred1997   (501) staff       (20)     1181 2024-02-24 03:34:08.000000 vnerrant-1.0.1rc4/vnerrant/utils/utils.py
+drwxr-xr-x   0 manred1997   (501) staff       (20)        0 2024-05-16 03:16:45.900793 vnerrant-1.0.1rc4/vnerrant.egg-info/
+-rw-r--r--   0 manred1997   (501) staff       (20)    10287 2024-05-16 03:16:45.000000 vnerrant-1.0.1rc4/vnerrant.egg-info/PKG-INFO
+-rw-r--r--   0 manred1997   (501) staff       (20)     1446 2024-05-16 03:16:45.000000 vnerrant-1.0.1rc4/vnerrant.egg-info/SOURCES.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)        1 2024-05-16 03:16:45.000000 vnerrant-1.0.1rc4/vnerrant.egg-info/dependency_links.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)       58 2024-05-16 03:16:45.000000 vnerrant-1.0.1rc4/vnerrant.egg-info/entry_points.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)       26 2024-05-16 03:16:45.000000 vnerrant-1.0.1rc4/vnerrant.egg-info/requires.txt
+-rw-r--r--   0 manred1997   (501) staff       (20)        9 2024-05-16 03:16:45.000000 vnerrant-1.0.1rc4/vnerrant.egg-info/top_level.txt
```

### Comparing `vnerrant-1.0.1rc3/PKG-INFO` & `vnerrant-1.0.1rc4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnerrant
-Version: 1.0.1rc3
+Version: 1.0.1rc4
 Summary: The ERRor ANnotation Toolkit (ERRANT).         Automatically extract and classify edits in parallel sentences.
 License: MIT
 Keywords: automatic annotation,grammatical errors,natural language processing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vnerrant-1.0.1rc3/README.md` & `vnerrant-1.0.1rc4/README.md`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/setup.py` & `vnerrant-1.0.1rc4/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 # Readme text for long description
 with open(base_dir / "README.md") as f:
     readme = f.read()
 
 setup(
     name="vnerrant",
-    version="1.0.1rc3",
+    version="1.0.1rc4",
     license="MIT",
     description="The ERRor ANnotation Toolkit (ERRANT). \
         Automatically extract and classify edits in parallel sentences.",
     long_description=readme,
     long_description_content_type="text/markdown",
     keywords=[
         "automatic annotation",
```

### Comparing `vnerrant-1.0.1rc3/tests/test_vnerrant.py` & `vnerrant-1.0.1rc4/tests/test_vnerrant.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/__init__.py` & `vnerrant-1.0.1rc4/vnerrant/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from typing import Any
 
 import spacy
 
 from vnerrant.annotator import Annotator
 from vnerrant.utils.utils import get_spacy_models_for_language
 
-__version__ = "v1.0.1rc3"
+__version__ = "v1.0.1rc4"
 
 
 def load(
     lang: str = "en",
     model_name: str = "en_core_web_sm",
     nlp: Any = None,
 ) -> Annotator:
```

### Comparing `vnerrant-1.0.1rc3/vnerrant/annotator.py` & `vnerrant-1.0.1rc4/vnerrant/annotator.py`

 * *Files 1% similar despite different names*

```diff
@@ -267,15 +267,15 @@
 
         processed_text = " ".join([token for token in text.split() if token.strip()])
         if not merged_token_with_ws_texts[0].strip():
             processed_text = merged_token_with_ws_texts[0] + processed_text
 
         return processed_text, merged_token_with_ws_texts
 
-    def postprocess(self, edit_collection: EditCollection):
+    def postprocess(self, edit_collection: EditCollection, is_update_span: bool = True):
         """
         Postprocess the edit collection.
         :param edit_collection: An EditCollection object
         :return: None
         """
         edit_utils.update_edits(edit_collection.orig_doc, edit_collection.cor_doc, edit_collection.edits)
         edit_utils.update_edits(edit_collection.orig_doc, edit_collection.cor_doc, edit_collection.match_edits)
@@ -285,15 +285,16 @@
             if edit.original.text == edit.corrected.text:
                 continue
 
             space_edits.append(edit_utils.process_space_edit(edit))
 
         edit_utils.merge_edit_collection_with_space_edits(edit_collection, space_edits)
         edit_utils.update_operator(edit_collection.edits)
-        edit_utils.update_replace_operator(edit_collection.edits)
+        if is_update_span:
+            edit_utils.upadte_span_edit(edit_collection.edits)
 
     def import_edit(
         self,
         orig: Doc,
         cor: Doc,
         edit: list,
         min: bool = True,
```

### Comparing `vnerrant-1.0.1rc3/vnerrant/cli/convert.py` & `vnerrant-1.0.1rc4/vnerrant/cli/convert.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/cli/evaluate.py` & `vnerrant-1.0.1rc4/vnerrant/cli/evaluate.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/components/alignment.py` & `vnerrant-1.0.1rc4/vnerrant/components/alignment.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/components/converter.py` & `vnerrant-1.0.1rc4/vnerrant/components/converter.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/components/en/classifier.py` & `vnerrant-1.0.1rc4/vnerrant/components/en/classifier.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/components/en/constants.py` & `vnerrant-1.0.1rc4/vnerrant/components/en/constants.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/components/en/explainer.py` & `vnerrant-1.0.1rc4/vnerrant/components/en/explainer.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/components/en/lancaster.py` & `vnerrant-1.0.1rc4/vnerrant/components/en/lancaster.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/components/en/merger.py` & `vnerrant-1.0.1rc4/vnerrant/components/en/merger.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/components/en/resources/README.md` & `vnerrant-1.0.1rc4/vnerrant/components/en/resources/README.md`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/components/en/resources/en_GB-large.txt` & `vnerrant-1.0.1rc4/vnerrant/components/en/resources/en_GB-large.txt`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/components/en/utils.py` & `vnerrant-1.0.1rc4/vnerrant/components/en/utils.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/components/evaluater.py` & `vnerrant-1.0.1rc4/vnerrant/components/evaluater.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/components/merger.py` & `vnerrant-1.0.1rc4/vnerrant/components/merger.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/components/tokenizer.py` & `vnerrant-1.0.1rc4/vnerrant/components/tokenizer.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/config/errant_verbose.json` & `vnerrant-1.0.1rc4/vnerrant/config/errant_verbose.json`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/config/mapping_type_error.yaml` & `vnerrant-1.0.1rc4/vnerrant/config/mapping_type_error.yaml`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/constants.py` & `vnerrant-1.0.1rc4/vnerrant/constants.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/metrics/criteria.py` & `vnerrant-1.0.1rc4/vnerrant/metrics/criteria.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/model/edit.py` & `vnerrant-1.0.1rc4/vnerrant/model/edit.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/run_cli.py` & `vnerrant-1.0.1rc4/vnerrant/run_cli.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/utils/edit_utils.py` & `vnerrant-1.0.1rc4/vnerrant/utils/edit_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -124,26 +124,25 @@
         if orig_text and cor_text:
             edit.edit_type = "R" + edit.edit_type[1:]
         elif not orig_text and cor_text:
             edit.edit_type = "M" + edit.edit_type[1:]
         else:
             edit.edit_type = "U" + edit.edit_type[1:]
 
-def update_replace_operator(edits: List[Edit]):
+def upadte_span_edit(edits: List[Edit]): # noqa D103
     """
     Update the replace operator of the edits.
     Args:
         edits (list[Edit]): A list of Edit objects to be updated.
     """
     for edit in edits:
-        if edit.edit_type[0] == "R":
-            edit.original.text = edit.original.text[:-1]
-            edit.original.end_char = edit.original.start_char + len(edit.original.text)
-            edit.corrected.text = edit.corrected.text[:-1]
-            edit.corrected.end_char = edit.corrected.start_char + len(edit.corrected.text)
+        edit.original.text = edit.original.tokens.text
+        edit.original.end_char = edit.original.start_char + len(edit.original.text)
+        edit.corrected.text = edit.corrected.tokens.text
+        edit.corrected.end_char = edit.corrected.start_char + len(edit.corrected.text)
             
 def process_space_edit(edit: Edit) -> Edit:
     """
     Process the space edit.
     Args:
         edit (Edit): An Edit object to be processed.
```

### Comparing `vnerrant-1.0.1rc3/vnerrant/utils/helper.py` & `vnerrant-1.0.1rc4/vnerrant/utils/helper.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/utils/pretty_results.py` & `vnerrant-1.0.1rc4/vnerrant/utils/pretty_results.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/utils/string_utils.py` & `vnerrant-1.0.1rc4/vnerrant/utils/string_utils.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant/utils/utils.py` & `vnerrant-1.0.1rc4/vnerrant/utils/utils.py`

 * *Files identical despite different names*

### Comparing `vnerrant-1.0.1rc3/vnerrant.egg-info/PKG-INFO` & `vnerrant-1.0.1rc4/vnerrant.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vnerrant
-Version: 1.0.1rc3
+Version: 1.0.1rc4
 Summary: The ERRor ANnotation Toolkit (ERRANT).         Automatically extract and classify edits in parallel sentences.
 License: MIT
 Keywords: automatic annotation,grammatical errors,natural language processing
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Education
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `vnerrant-1.0.1rc3/vnerrant.egg-info/SOURCES.txt` & `vnerrant-1.0.1rc4/vnerrant.egg-info/SOURCES.txt`

 * *Files identical despite different names*

