# Comparing `tmp/sphinxcontrib-katex-0.9.8.tar.gz` & `tmp/sphinxcontrib-katex-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sphinxcontrib-katex-0.9.8.tar", last modified: Thu Oct 12 14:14:32 2023, max compression
+gzip compressed data, was "sphinxcontrib-katex-0.9.9.tar", last modified: Mon Oct 16 07:30:08 2023, max compression
```

## Comparing `sphinxcontrib-katex-0.9.8.tar` & `sphinxcontrib-katex-0.9.9.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 14:14:32.065748 sphinxcontrib-katex-0.9.8/
--rw-r--r--   0 runner    (1001) docker     (127)     5132 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3759 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      171 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2023-10-12 14:14:32.065748 sphinxcontrib-katex-0.9.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5596 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 14:14:32.065748 sphinxcontrib-katex-0.9.8/docs/
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       66 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (127)      775 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/docs/definitions.py
--rw-r--r--   0 runner    (1001) docker     (127)     4953 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/docs/examples.rst
--rw-r--r--   0 runner    (1001) docker     (127)      571 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/docs/macros.rst
--rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (127)     3874 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-12 14:14:32.065748 sphinxcontrib-katex-0.9.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 14:14:32.065748 sphinxcontrib-katex-0.9.8/sphinxcontrib/
--rw-r--r--   0 runner    (1001) docker     (127)     3478 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/sphinxcontrib/auto-render.min.js
--rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/sphinxcontrib/katex-math.css
--rw-r--r--   0 runner    (1001) docker     (127)     4365 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/sphinxcontrib/katex-server.js
--rw-r--r--   0 runner    (1001) docker     (127)   277038 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/sphinxcontrib/katex.min.js
--rw-r--r--   0 runner    (1001) docker     (127)    19069 2023-10-12 14:14:12.000000 sphinxcontrib-katex-0.9.8/sphinxcontrib/katex.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-12 14:14:32.065748 sphinxcontrib-katex-0.9.8/sphinxcontrib_katex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8036 2023-10-12 14:14:32.000000 sphinxcontrib-katex-0.9.8/sphinxcontrib_katex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      654 2023-10-12 14:14:32.000000 sphinxcontrib-katex-0.9.8/sphinxcontrib_katex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-12 14:14:32.000000 sphinxcontrib-katex-0.9.8/sphinxcontrib_katex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-12 14:14:32.000000 sphinxcontrib-katex-0.9.8/sphinxcontrib_katex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-12 14:14:32.000000 sphinxcontrib-katex-0.9.8/sphinxcontrib_katex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:30:08.239453 sphinxcontrib-katex-0.9.9/
+-rw-r--r--   0 runner    (1001) docker     (127)     5242 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3759 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      171 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2023-10-16 07:30:08.239453 sphinxcontrib-katex-0.9.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5596 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:30:08.231453 sphinxcontrib-katex-0.9.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      775 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/docs/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4953 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/docs/examples.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       61 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/docs/macros.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     3874 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)        5 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2023-10-16 07:30:08.239453 sphinxcontrib-katex-0.9.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:30:08.235453 sphinxcontrib-katex-0.9.9/sphinxcontrib/
+-rw-r--r--   0 runner    (1001) docker     (127)     3478 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/sphinxcontrib/auto-render.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)     1132 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/sphinxcontrib/katex-math.css
+-rw-r--r--   0 runner    (1001) docker     (127)     4365 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/sphinxcontrib/katex-server.js
+-rw-r--r--   0 runner    (1001) docker     (127)   277038 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/sphinxcontrib/katex.min.js
+-rw-r--r--   0 runner    (1001) docker     (127)    19069 2023-10-16 07:29:52.000000 sphinxcontrib-katex-0.9.9/sphinxcontrib/katex.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-10-16 07:30:08.239453 sphinxcontrib-katex-0.9.9/sphinxcontrib_katex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8036 2023-10-16 07:30:08.000000 sphinxcontrib-katex-0.9.9/sphinxcontrib_katex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      654 2023-10-16 07:30:08.000000 sphinxcontrib-katex-0.9.9/sphinxcontrib_katex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2023-10-16 07:30:08.000000 sphinxcontrib-katex-0.9.9/sphinxcontrib_katex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2023-10-16 07:30:08.000000 sphinxcontrib-katex-0.9.9/sphinxcontrib_katex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2023-10-16 07:30:08.000000 sphinxcontrib-katex-0.9.9/sphinxcontrib_katex.egg-info/top_level.txt
```

### Comparing `sphinxcontrib-katex-0.9.8/CHANGELOG.rst` & `sphinxcontrib-katex-0.9.9/CHANGELOG.rst`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,20 @@
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
 
+Version 0.9.9 (2023-10-16)
+--------------------------
+
+* Fixed: building of documentation on Read The Docs.
+
+
 Version 0.9.8 (2023-10-12)
 --------------------------
 
 * Added: support for Python 3.12
 * Changed: use KaTeX 0.16.9
```

### Comparing `sphinxcontrib-katex-0.9.8/CONTRIBUTING.rst` & `sphinxcontrib-katex-0.9.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.8/LICENSE` & `sphinxcontrib-katex-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.8/PKG-INFO` & `sphinxcontrib-katex-0.9.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-katex
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Sphinx extension for rendering math in HTML pages
 Author-email: Hagen Wierstorf <hagenw@posteo.de>
 License: The MIT License
         
         Copyright (c) 2017 Hagen Wierstorf 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sphinxcontrib-katex-0.9.8/README.rst` & `sphinxcontrib-katex-0.9.9/README.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.8/docs/conf.py` & `sphinxcontrib-katex-0.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.8/docs/definitions.py` & `sphinxcontrib-katex-0.9.9/docs/definitions.py`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.8/docs/examples.rst` & `sphinxcontrib-katex-0.9.9/docs/examples.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.8/docs/index.rst` & `sphinxcontrib-katex-0.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.8/pyproject.toml` & `sphinxcontrib-katex-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.8/sphinxcontrib/auto-render.min.js` & `sphinxcontrib-katex-0.9.9/sphinxcontrib/auto-render.min.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.8/sphinxcontrib/katex-math.css` & `sphinxcontrib-katex-0.9.9/sphinxcontrib/katex-math.css`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.8/sphinxcontrib/katex-server.js` & `sphinxcontrib-katex-0.9.9/sphinxcontrib/katex-server.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.8/sphinxcontrib/katex.min.js` & `sphinxcontrib-katex-0.9.9/sphinxcontrib/katex.min.js`

 * *Files identical despite different names*

### Comparing `sphinxcontrib-katex-0.9.8/sphinxcontrib/katex.py` & `sphinxcontrib-katex-0.9.9/sphinxcontrib/katex.py`

 * *Files 1% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
 from docutils import nodes
 from sphinx.errors import ExtensionError
 from sphinx.locale import _
 from sphinx.util.osutil import copyfile
 
 
-__version__ = '0.9.8'
+__version__ = '0.9.9'
 katex_version = '0.16.9'
 filename_css = 'katex-math.css'
 filename_autorenderer = 'katex_autorenderer.js'
 SRC_DIR = Path(__file__).parent
 SCRIPT_PATH = str(SRC_DIR / "katex-server.js")
 
 ONE_MILLISECOND = 0.001
```

### Comparing `sphinxcontrib-katex-0.9.8/sphinxcontrib_katex.egg-info/PKG-INFO` & `sphinxcontrib-katex-0.9.9/sphinxcontrib_katex.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sphinxcontrib-katex
-Version: 0.9.8
+Version: 0.9.9
 Summary: A Sphinx extension for rendering math in HTML pages
 Author-email: Hagen Wierstorf <hagenw@posteo.de>
 License: The MIT License
         
         Copyright (c) 2017 Hagen Wierstorf 
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `sphinxcontrib-katex-0.9.8/sphinxcontrib_katex.egg-info/SOURCES.txt` & `sphinxcontrib-katex-0.9.9/sphinxcontrib_katex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

