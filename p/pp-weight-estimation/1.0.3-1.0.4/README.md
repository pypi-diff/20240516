# Comparing `tmp/pp_weight_estimation-1.0.3.tar.gz` & `tmp/pp_weight_estimation-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pp_weight_estimation-1.0.3.tar", last modified: Thu May 16 12:26:46 2024, max compression
+gzip compressed data, was "pp_weight_estimation-1.0.4.tar", last modified: Thu May 16 12:52:16 2024, max compression
```

## Comparing `pp_weight_estimation-1.0.3.tar` & `pp_weight_estimation-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-05-16 12:26:46.673552 pp_weight_estimation-1.0.3/
--rw-r--r--   0 winnow    (1000) winnow    (1000)      245 2024-05-16 12:26:46.673552 pp_weight_estimation-1.0.3/PKG-INFO
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       56 2024-05-16 12:25:41.000000 pp_weight_estimation-1.0.3/README.md
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-05-16 12:26:46.673552 pp_weight_estimation-1.0.3/pp_weight_estimation/
--rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2024-05-16 11:09:18.000000 pp_weight_estimation-1.0.3/pp_weight_estimation/__init__.py
--rw-rw-r--   0 winnow    (1000) winnow    (1000)      206 2024-05-16 12:26:29.000000 pp_weight_estimation-1.0.3/pp_weight_estimation/version.py
-drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-05-16 12:26:46.673552 pp_weight_estimation-1.0.3/pp_weight_estimation.egg-info/
--rw-r--r--   0 winnow    (1000) winnow    (1000)      245 2024-05-16 12:26:46.000000 pp_weight_estimation-1.0.3/pp_weight_estimation.egg-info/PKG-INFO
--rw-rw-r--   0 winnow    (1000) winnow    (1000)      317 2024-05-16 12:26:46.000000 pp_weight_estimation-1.0.3/pp_weight_estimation.egg-info/SOURCES.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)        1 2024-05-16 12:26:46.000000 pp_weight_estimation-1.0.3/pp_weight_estimation.egg-info/dependency_links.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       27 2024-05-16 12:26:46.000000 pp_weight_estimation-1.0.3/pp_weight_estimation.egg-info/requires.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       21 2024-05-16 12:26:46.000000 pp_weight_estimation-1.0.3/pp_weight_estimation.egg-info/top_level.txt
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       81 2024-05-16 11:05:46.000000 pp_weight_estimation-1.0.3/pyproject.toml
--rw-rw-r--   0 winnow    (1000) winnow    (1000)       38 2024-05-16 12:26:46.673552 pp_weight_estimation-1.0.3/setup.cfg
--rw-rw-r--   0 winnow    (1000) winnow    (1000)      858 2024-05-16 11:07:18.000000 pp_weight_estimation-1.0.3/setup.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-05-16 12:52:16.311330 pp_weight_estimation-1.0.4/
+-rw-r--r--   0 winnow    (1000) winnow    (1000)      245 2024-05-16 12:52:16.307330 pp_weight_estimation-1.0.4/PKG-INFO
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       56 2024-05-16 12:25:41.000000 pp_weight_estimation-1.0.4/README.md
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-05-16 12:52:16.307330 pp_weight_estimation-1.0.4/pp_weight_estimation/
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        0 2024-05-16 11:09:18.000000 pp_weight_estimation-1.0.4/pp_weight_estimation/__init__.py
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      206 2024-05-16 12:51:55.000000 pp_weight_estimation-1.0.4/pp_weight_estimation/version.py
+drwxrwxr-x   0 winnow    (1000) winnow    (1000)        0 2024-05-16 12:52:16.307330 pp_weight_estimation-1.0.4/pp_weight_estimation.egg-info/
+-rw-r--r--   0 winnow    (1000) winnow    (1000)      245 2024-05-16 12:52:16.000000 pp_weight_estimation-1.0.4/pp_weight_estimation.egg-info/PKG-INFO
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      317 2024-05-16 12:52:16.000000 pp_weight_estimation-1.0.4/pp_weight_estimation.egg-info/SOURCES.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)        1 2024-05-16 12:52:16.000000 pp_weight_estimation-1.0.4/pp_weight_estimation.egg-info/dependency_links.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       27 2024-05-16 12:52:16.000000 pp_weight_estimation-1.0.4/pp_weight_estimation.egg-info/requires.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       21 2024-05-16 12:52:16.000000 pp_weight_estimation-1.0.4/pp_weight_estimation.egg-info/top_level.txt
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       81 2024-05-16 11:05:46.000000 pp_weight_estimation-1.0.4/pyproject.toml
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)       38 2024-05-16 12:52:16.311330 pp_weight_estimation-1.0.4/setup.cfg
+-rw-rw-r--   0 winnow    (1000) winnow    (1000)      858 2024-05-16 11:07:18.000000 pp_weight_estimation-1.0.4/setup.py
```

### Comparing `pp_weight_estimation-1.0.3/setup.py` & `pp_weight_estimation-1.0.4/setup.py`

 * *Files identical despite different names*

