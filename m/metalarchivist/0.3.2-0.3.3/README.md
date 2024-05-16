# Comparing `tmp/metalarchivist-0.3.2.tar.gz` & `tmp/metalarchivist-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metalarchivist-0.3.2.tar", last modified: Wed May 15 22:00:16 2024, max compression
+gzip compressed data, was "metalarchivist-0.3.3.tar", last modified: Wed May 15 23:40:10 2024, max compression
```

## Comparing `metalarchivist-0.3.2.tar` & `metalarchivist-0.3.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:00:16.934857 metalarchivist-0.3.2/
--rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/LICENSE
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-15 22:00:16.934857 metalarchivist-0.3.2/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/README.md
--rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 22:00:16.934857 metalarchivist-0.3.2/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:00:16.926857 metalarchivist-0.3.2/src/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:00:16.927857 metalarchivist-0.3.2/src/metalarchivist/
--rwxrwxrwx   0 root         (0) root         (0)      107 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:00:16.930857 metalarchivist-0.3.2/src/metalarchivist/export/
--rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/export/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     4225 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/export/album.py
--rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/export/band.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:00:16.930857 metalarchivist-0.3.2/src/metalarchivist/export/data/
--rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/export/data/user-agents.json
--rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/export/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     9505 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/export/label.py
--rwxrwxrwx   0 root         (0) root         (0)     7075 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/export/util.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:00:16.932857 metalarchivist-0.3.2/src/metalarchivist/interface/
--rwxrwxrwx   0 root         (0) root         (0)     1378 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/interface/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     6842 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/interface/album.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:00:16.932857 metalarchivist-0.3.2/src/metalarchivist/interface/api/
--rw-rw-rw-   0 root         (0) root         (0)     3092 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/interface/api/base.py
--rw-rw-rw-   0 root         (0) root         (0)     4836 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/interface/api/page.py
--rwxrwxrwx   0 root         (0) root         (0)     8469 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/interface/band.py
--rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/interface/genre.py
--rw-rw-rw-   0 root         (0) root         (0)     6191 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/interface/label.py
--rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/interface/search.py
--rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/interface/theme.py
--rwxrwxrwx   0 root         (0) root         (0)     3645 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/metalarchivist/report.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:00:16.934857 metalarchivist-0.3.2/src/metalarchivist.egg-info/
--rw-r--r--   0 root         (0) root         (0)      702 2024-05-15 22:00:16.000000 metalarchivist-0.3.2/src/metalarchivist.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1030 2024-05-15 22:00:16.000000 metalarchivist-0.3.2/src/metalarchivist.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 22:00:16.000000 metalarchivist-0.3.2/src/metalarchivist.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-05-15 22:00:16.000000 metalarchivist-0.3.2/src/metalarchivist.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       20 2024-05-15 22:00:16.000000 metalarchivist-0.3.2/src/metalarchivist.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 22:00:16.933857 metalarchivist-0.3.2/src/test/
--rwxrwxrwx   0 root         (0) root         (0)    10013 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/test/test_albums.py
--rwxrwxrwx   0 root         (0) root         (0)     5029 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/test/test_bands.py
--rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/test/test_genres.py
--rw-rw-rw-   0 root         (0) root         (0)     4731 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/test/test_labels.py
--rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-15 22:00:03.000000 metalarchivist-0.3.2/src/test/test_themes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.399529 metalarchivist-0.3.3/
+-rwxrwxrwx   0 root         (0) root         (0)      693 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-15 23:40:10.399529 metalarchivist-0.3.3/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      113 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/README.md
+-rwxrwxrwx   0 root         (0) root         (0)      677 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2024-05-15 23:40:10.399529 metalarchivist-0.3.3/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.391529 metalarchivist-0.3.3/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.392529 metalarchivist-0.3.3/src/metalarchivist/
+-rwxrwxrwx   0 root         (0) root         (0)      107 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.395529 metalarchivist-0.3.3/src/metalarchivist/export/
+-rwxrwxrwx   0 root         (0) root         (0)      257 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/export/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     4225 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/export/album.py
+-rwxrwxrwx   0 root         (0) root         (0)     3679 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/export/band.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.395529 metalarchivist-0.3.3/src/metalarchivist/export/data/
+-rw-rw-rw-   0 root         (0) root         (0)     1754 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/export/data/user-agents.json
+-rw-rw-rw-   0 root         (0) root         (0)     2685 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/export/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     9505 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/export/label.py
+-rwxrwxrwx   0 root         (0) root         (0)     7075 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/export/util.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.397529 metalarchivist-0.3.3/src/metalarchivist/interface/
+-rwxrwxrwx   0 root         (0) root         (0)     1378 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     6842 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/album.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.397529 metalarchivist-0.3.3/src/metalarchivist/interface/api/
+-rw-rw-rw-   0 root         (0) root         (0)     3092 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/api/base.py
+-rw-rw-rw-   0 root         (0) root         (0)     4836 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/api/page.py
+-rwxrwxrwx   0 root         (0) root         (0)     8469 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/band.py
+-rw-rw-rw-   0 root         (0) root         (0)     7975 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/genre.py
+-rw-rw-rw-   0 root         (0) root         (0)     6225 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/label.py
+-rwxrwxrwx   0 root         (0) root         (0)      380 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/search.py
+-rw-rw-rw-   0 root         (0) root         (0)     7235 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/interface/theme.py
+-rwxrwxrwx   0 root         (0) root         (0)     3645 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/metalarchivist/report.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.399529 metalarchivist-0.3.3/src/metalarchivist.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      702 2024-05-15 23:40:10.000000 metalarchivist-0.3.3/src/metalarchivist.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-05-15 23:40:10.000000 metalarchivist-0.3.3/src/metalarchivist.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-05-15 23:40:10.000000 metalarchivist-0.3.3/src/metalarchivist.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-05-15 23:40:10.000000 metalarchivist-0.3.3/src/metalarchivist.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       20 2024-05-15 23:40:10.000000 metalarchivist-0.3.3/src/metalarchivist.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-05-15 23:40:10.398529 metalarchivist-0.3.3/src/test/
+-rwxrwxrwx   0 root         (0) root         (0)    10013 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/test/test_albums.py
+-rwxrwxrwx   0 root         (0) root         (0)     5029 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/test/test_bands.py
+-rwxrwxrwx   0 root         (0) root         (0)     8506 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/test/test_genres.py
+-rw-rw-rw-   0 root         (0) root         (0)     4731 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/test/test_labels.py
+-rw-rw-rw-   0 root         (0) root         (0)     4108 2024-05-15 23:39:56.000000 metalarchivist-0.3.3/src/test/test_themes.py
```

### Comparing `metalarchivist-0.3.2/LICENSE` & `metalarchivist-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/PKG-INFO` & `metalarchivist-0.3.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.3.2
+Version: 0.3.3
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.3.2/pyproject.toml` & `metalarchivist-0.3.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "metalarchivist"
-version = "0.3.2"
+version = "0.3.3"
 authors = [ { name = "z3c0", email = "z3c0@21337.tech" } ]
 description = "A package for extracting data from metal-archives.com"
 readme = "README.md"
 requires-python = ">=3.11"
 dependencies = [ "rich", "lxml", "urllib3", "pycryptodome" ]
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `metalarchivist-0.3.2/src/metalarchivist/export/album.py` & `metalarchivist-0.3.3/src/metalarchivist/export/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/metalarchivist/export/band.py` & `metalarchivist-0.3.3/src/metalarchivist/export/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/metalarchivist/export/data/user-agents.json` & `metalarchivist-0.3.3/src/metalarchivist/export/data/user-agents.json`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/metalarchivist/export/genre.py` & `metalarchivist-0.3.3/src/metalarchivist/export/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/metalarchivist/export/label.py` & `metalarchivist-0.3.3/src/metalarchivist/export/label.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/metalarchivist/export/util.py` & `metalarchivist-0.3.3/src/metalarchivist/export/util.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/metalarchivist/interface/__init__.py` & `metalarchivist-0.3.3/src/metalarchivist/interface/__init__.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/metalarchivist/interface/album.py` & `metalarchivist-0.3.3/src/metalarchivist/interface/album.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/metalarchivist/interface/api/base.py` & `metalarchivist-0.3.3/src/metalarchivist/interface/api/base.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/metalarchivist/interface/api/page.py` & `metalarchivist-0.3.3/src/metalarchivist/interface/api/page.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/metalarchivist/interface/band.py` & `metalarchivist-0.3.3/src/metalarchivist/interface/band.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/metalarchivist/interface/genre.py` & `metalarchivist-0.3.3/src/metalarchivist/interface/genre.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/metalarchivist/interface/label.py` & `metalarchivist-0.3.3/src/metalarchivist/interface/label.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,17 +13,18 @@
 @dataclass
 class LabelRosterMember:
     metallum_id: int
     band: BandLink
     subgenres: Subgenres
     country_of_origin: str
 
-    def to_dict(self):
+    def to_dict(self) -> dict:
         dictionary = asdict(self)
         dictionary['subgenres'] = self.subgenres.to_dict()
+        return dictionary
 
 
 @dataclass
 class LabelRoster:
     current: list[LabelRosterMember]
     past: list[LabelRosterMember]
```

### Comparing `metalarchivist-0.3.2/src/metalarchivist/interface/theme.py` & `metalarchivist-0.3.3/src/metalarchivist/interface/theme.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/metalarchivist/report.py` & `metalarchivist-0.3.3/src/metalarchivist/report.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/metalarchivist.egg-info/PKG-INFO` & `metalarchivist-0.3.3/src/metalarchivist.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: metalarchivist
-Version: 0.3.2
+Version: 0.3.3
 Summary: A package for extracting data from metal-archives.com
 Author-email: z3c0 <z3c0@21337.tech>
 Project-URL: Homepage, https://gitlab.com/black-metal-book-club/metallum
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.11
```

### Comparing `metalarchivist-0.3.2/src/metalarchivist.egg-info/SOURCES.txt` & `metalarchivist-0.3.3/src/metalarchivist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/test/test_albums.py` & `metalarchivist-0.3.3/src/test/test_albums.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/test/test_bands.py` & `metalarchivist-0.3.3/src/test/test_bands.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/test/test_genres.py` & `metalarchivist-0.3.3/src/test/test_genres.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/test/test_labels.py` & `metalarchivist-0.3.3/src/test/test_labels.py`

 * *Files identical despite different names*

### Comparing `metalarchivist-0.3.2/src/test/test_themes.py` & `metalarchivist-0.3.3/src/test/test_themes.py`

 * *Files identical despite different names*

