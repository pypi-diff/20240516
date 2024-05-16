# Comparing `tmp/epubgrep-0.8.1.tar.gz` & `tmp/epubgrep-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "epubgrep-0.8.1.tar", last modified: Fri Jan 26 19:12:37 2024, max compression
+gzip compressed data, was "epubgrep-0.9.0.tar", last modified: Fri Jan 26 19:57:35 2024, max compression
```

## Comparing `epubgrep-0.8.1.tar` & `epubgrep-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 matej     (1000) matej     (1000)        0 2024-01-26 19:12:37.988620 epubgrep-0.8.1/
--rw-r--r--   0 matej     (1000) matej     (1000)      819 2024-01-26 19:12:37.988620 epubgrep-0.8.1/PKG-INFO
-drwxr-xr-x   0 matej     (1000) matej     (1000)        0 2024-01-26 19:12:37.988620 epubgrep-0.8.1/epubgrep.egg-info/
--rw-r--r--   0 matej     (1000) matej     (1000)      819 2024-01-26 19:12:37.000000 epubgrep-0.8.1/epubgrep.egg-info/PKG-INFO
--rw-r--r--   0 matej     (1000) matej     (1000)      260 2024-01-26 19:12:37.000000 epubgrep-0.8.1/epubgrep.egg-info/SOURCES.txt
--rw-r--r--   0 matej     (1000) matej     (1000)        1 2024-01-26 19:12:37.000000 epubgrep-0.8.1/epubgrep.egg-info/dependency_links.txt
--rw-r--r--   0 matej     (1000) matej     (1000)       43 2024-01-26 19:12:37.000000 epubgrep-0.8.1/epubgrep.egg-info/entry_points.txt
--rw-r--r--   0 matej     (1000) matej     (1000)       10 2024-01-26 19:12:37.000000 epubgrep-0.8.1/epubgrep.egg-info/requires.txt
--rw-r--r--   0 matej     (1000) matej     (1000)        9 2024-01-26 19:12:37.000000 epubgrep-0.8.1/epubgrep.egg-info/top_level.txt
--rwxr-xr-x   0 matej     (1000) matej     (1000)     8569 2022-09-06 22:26:00.000000 epubgrep-0.8.1/epubgrep.py
--rw-r--r--   0 matej     (1000) matej     (1000)      993 2024-01-26 19:12:28.000000 epubgrep-0.8.1/pyproject.toml
--rw-r--r--   0 matej     (1000) matej     (1000)       38 2024-01-26 19:12:37.988620 epubgrep-0.8.1/setup.cfg
-drwxr-xr-x   0 matej     (1000) matej     (1000)        0 2024-01-26 19:12:37.988620 epubgrep-0.8.1/tests/
--rw-r--r--   0 matej     (1000) matej     (1000)        0 2018-11-30 10:56:38.000000 epubgrep-0.8.1/tests/__init__.py
--rw-r--r--   0 matej     (1000) matej     (1000)      203 2018-11-30 10:54:40.000000 epubgrep-0.8.1/tests/test_epugrep.py
+drwxr-xr-x   0 matej     (1000) matej     (1000)        0 2024-01-26 19:57:35.387877 epubgrep-0.9.0/
+-rw-r--r--   0 matej     (1000) matej     (1000)      819 2024-01-26 19:57:35.387877 epubgrep-0.9.0/PKG-INFO
+drwxr-xr-x   0 matej     (1000) matej     (1000)        0 2024-01-26 19:57:35.387877 epubgrep-0.9.0/epubgrep.egg-info/
+-rw-r--r--   0 matej     (1000) matej     (1000)      819 2024-01-26 19:57:35.000000 epubgrep-0.9.0/epubgrep.egg-info/PKG-INFO
+-rw-r--r--   0 matej     (1000) matej     (1000)      260 2024-01-26 19:57:35.000000 epubgrep-0.9.0/epubgrep.egg-info/SOURCES.txt
+-rw-r--r--   0 matej     (1000) matej     (1000)        1 2024-01-26 19:57:35.000000 epubgrep-0.9.0/epubgrep.egg-info/dependency_links.txt
+-rw-r--r--   0 matej     (1000) matej     (1000)       43 2024-01-26 19:57:35.000000 epubgrep-0.9.0/epubgrep.egg-info/entry_points.txt
+-rw-r--r--   0 matej     (1000) matej     (1000)       10 2024-01-26 19:57:35.000000 epubgrep-0.9.0/epubgrep.egg-info/requires.txt
+-rw-r--r--   0 matej     (1000) matej     (1000)        9 2024-01-26 19:57:35.000000 epubgrep-0.9.0/epubgrep.egg-info/top_level.txt
+-rwxr-xr-x   0 matej     (1000) matej     (1000)     8557 2024-01-26 19:56:14.000000 epubgrep-0.9.0/epubgrep.py
+-rw-r--r--   0 matej     (1000) matej     (1000)      933 2024-01-26 19:57:15.000000 epubgrep-0.9.0/pyproject.toml
+-rw-r--r--   0 matej     (1000) matej     (1000)       38 2024-01-26 19:57:35.387877 epubgrep-0.9.0/setup.cfg
+drwxr-xr-x   0 matej     (1000) matej     (1000)        0 2024-01-26 19:57:35.387877 epubgrep-0.9.0/tests/
+-rw-r--r--   0 matej     (1000) matej     (1000)        0 2018-11-30 10:56:38.000000 epubgrep-0.9.0/tests/__init__.py
+-rw-r--r--   0 matej     (1000) matej     (1000)      203 2018-11-30 10:54:40.000000 epubgrep-0.9.0/tests/test_epugrep.py
```

### Comparing `epubgrep-0.8.1/PKG-INFO` & `epubgrep-0.9.0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubgrep
-Version: 0.8.1
+Version: 0.9.0
 Summary: Grep through EPub files
 Author-email: Matěj Cepl <mcepl@cepl.eu>
 Project-URL: Homepage, https://git.cepl.eu/cgit/epubgrep
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `epubgrep-0.8.1/epubgrep.egg-info/PKG-INFO` & `epubgrep-0.9.0/epubgrep.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: epubgrep
-Version: 0.8.1
+Version: 0.9.0
 Summary: Grep through EPub files
 Author-email: Matěj Cepl <mcepl@cepl.eu>
 Project-URL: Homepage, https://git.cepl.eu/cgit/epubgrep
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.3
 Classifier: Programming Language :: Python :: 3.4
 Classifier: Programming Language :: Python :: 3.5
```

### Comparing `epubgrep-0.8.1/epubgrep.py` & `epubgrep-0.9.0/epubgrep.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 
     for auth in authors:
         res = sre.search(auth)
         if res:
             if not title:
                 title = f'{fname}:'
             out += ' ' + _colorize_found(auth, res, col)
-            
+
     return title + out
 
 
 def grep_book(filename: str, opts: argparse.Namespace,
               re_flags: int) -> Optional[str]:
     assert os.path.isfile(filename), f'{filename} is not a file.'
     sought_RE = re.compile('(' + opts.pattern + ')', re_flags)
```

### Comparing `epubgrep-0.8.1/pyproject.toml` & `epubgrep-0.9.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "epubgrep"
-version = "0.8.1"
+version = "0.9.0"
 authors = [{name = "Matěj Cepl", email = "mcepl@cepl.eu"}]
 description = "Grep through EPub files"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Programming Language :: Python :: 3.3",
     "Programming Language :: Python :: 3.4",
     "Programming Language :: Python :: 3.5",
@@ -22,10 +22,7 @@
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 urls = {Homepage = "https://git.cepl.eu/cgit/epubgrep"}
 dependencies = ["epub_meta"]
 
 [project.scripts]
 epubgrep = "epubgrep:main"
-
-# [tool.setuptools.packages]
-# find = {namespaces = false}
```

