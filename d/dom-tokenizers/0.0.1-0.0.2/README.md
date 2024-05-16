# Comparing `tmp/dom_tokenizers-0.0.1.tar.gz` & `tmp/dom_tokenizers-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dom_tokenizers-0.0.1.tar", last modified: Wed May 15 19:15:13 2024, max compression
+gzip compressed data, was "dom_tokenizers-0.0.2.tar", last modified: Thu May 16 00:40:32 2024, max compression
```

## Comparing `dom_tokenizers-0.0.1.tar` & `dom_tokenizers-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:15:13.081043 dom_tokenizers-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-05-15 19:14:51.000000 dom_tokenizers-0.0.1/.flake8
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-15 19:14:51.000000 dom_tokenizers-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-15 19:14:51.000000 dom_tokenizers-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    14476 2024-05-15 19:15:13.077043 dom_tokenizers-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      288 2024-05-15 19:14:51.000000 dom_tokenizers-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-05-15 19:14:51.000000 dom_tokenizers-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-15 19:15:13.081043 dom_tokenizers-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:15:13.077043 dom_tokenizers-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:15:13.077043 dom_tokenizers-0.0.1/src/dom_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-15 19:14:51.000000 dom_tokenizers-0.0.1/src/dom_tokenizers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:15:13.077043 dom_tokenizers-0.0.1/src/dom_tokenizers/pre_tokenizers/
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-15 19:14:51.000000 dom_tokenizers-0.0.1/src/dom_tokenizers/pre_tokenizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9367 2024-05-15 19:14:51.000000 dom_tokenizers-0.0.1/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
--rw-r--r--   0 runner    (1001) docker     (127)     3190 2024-05-15 19:14:51.000000 dom_tokenizers-0.0.1/src/dom_tokenizers/train.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-15 19:15:13.077043 dom_tokenizers-0.0.1/src/dom_tokenizers.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14476 2024-05-15 19:15:13.000000 dom_tokenizers-0.0.1/src/dom_tokenizers.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-15 19:15:13.000000 dom_tokenizers-0.0.1/src/dom_tokenizers.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-15 19:15:13.000000 dom_tokenizers-0.0.1/src/dom_tokenizers.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-15 19:15:13.000000 dom_tokenizers-0.0.1/src/dom_tokenizers.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-15 19:15:13.000000 dom_tokenizers-0.0.1/src/dom_tokenizers.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-15 19:15:13.000000 dom_tokenizers-0.0.1/src/dom_tokenizers.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:40:32.796277 dom_tokenizers-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      329 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/.flake8
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-16 00:40:32.796277 dom_tokenizers-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      841 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1475 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 00:40:32.796277 dom_tokenizers-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:40:32.792277 dom_tokenizers-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:40:32.792277 dom_tokenizers-0.0.2/src/dom_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/src/dom_tokenizers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:40:32.792277 dom_tokenizers-0.0.2/src/dom_tokenizers/pre_tokenizers/
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/src/dom_tokenizers/pre_tokenizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9367 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5266 2024-05-16 00:40:11.000000 dom_tokenizers-0.0.2/src/dom_tokenizers/train.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 00:40:32.792277 dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2244 2024-05-16 00:40:32.000000 dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      461 2024-05-16 00:40:32.000000 dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 00:40:32.000000 dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-05-16 00:40:32.000000 dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 00:40:32.000000 dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-05-16 00:40:32.000000 dom_tokenizers-0.0.2/src/dom_tokenizers.egg-info/top_level.txt
```

### Comparing `dom_tokenizers-0.0.1/LICENSE` & `dom_tokenizers-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `dom_tokenizers-0.0.1/pyproject.toml` & `dom_tokenizers-0.0.2/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,36 +1,41 @@
 [project]
 name = "dom-tokenizers"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "Gary Benson" }]
-description = "HTML DOM-aware tokenizers for Hugging Face language models"
+description = "DOM-aware tokenizers for Hugging Face language models"
 readme = "README.md"
-license = { file = "LICENSE" }
+license = { text = "Apache Software License (Apache-2.0)" }
 requires-python = ">=3.10"  # match..case
 classifiers = [
-    "Programming Language :: Python :: 3",
+    "Development Status :: 4 - Beta",
+    "Intended Audience :: Developers",
+    "Intended Audience :: Education",
+    "Intended Audience :: Science/Research",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
-    "Development Status :: 4 - Beta",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Programming Language :: Python :: 3.12",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
     "Topic :: Scientific/Engineering :: Information Analysis",
     "Topic :: Text Processing :: Markup :: HTML",
 ]
 dependencies = [
     "python-magic",
     "tokenizers",
     "transformers",
 ]
 
 [project.urls]
 Homepage = "https://github.com/gbenson/dom-tokenizers"
-Repository = "https://github.com/gbenson/dom-tokenizers"
-"Bug Tracker" = "https://github.com/gbenson/dom-tokenizers/issues"
+#Source = "https://github.com/gbenson/dom-tokenizers"
 
 [project.optional-dependencies]
 dev = [
     "build",
     "flake8",
 ]
 train = [
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `dom_tokenizers-0.0.1/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py` & `dom_tokenizers-0.0.2/src/dom_tokenizers/pre_tokenizers/dom_snapshot.py`

 * *Files identical despite different names*

