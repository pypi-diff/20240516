# Comparing `tmp/browserbase-0.1.2.tar.gz` & `tmp/browserbase-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserbase-0.1.2.tar", last modified: Mon May 13 10:27:51 2024, max compression
+gzip compressed data, was "browserbase-0.1.3.tar", last modified: Thu May 16 14:17:32 2024, max compression
```

## Comparing `browserbase-0.1.2.tar` & `browserbase-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-13 10:27:51.546739 browserbase-0.1.2/
--rw-r--r--   0 mish       (501) staff       (20)     1064 2024-04-09 17:45:47.000000 browserbase-0.1.2/LICENSE
--rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-13 10:27:51.546489 browserbase-0.1.2/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      933 2024-04-19 10:57:22.000000 browserbase-0.1.2/README.md
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-13 10:27:51.544720 browserbase-0.1.2/browserbase/
--rw-r--r--   0 mish       (501) staff       (20)    10721 2024-05-13 10:27:05.000000 browserbase-0.1.2/browserbase/__init__.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-13 10:27:51.545786 browserbase-0.1.2/browserbase/helpers/
--rw-r--r--   0 mish       (501) staff       (20)      301 2024-04-16 18:32:01.000000 browserbase-0.1.2/browserbase/helpers/anthropic.py
--rw-r--r--   0 mish       (501) staff       (20)      503 2024-04-15 12:54:51.000000 browserbase-0.1.2/browserbase/helpers/gpt4.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-13 10:27:51.546189 browserbase-0.1.2/browserbase.egg-info/
--rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-13 10:27:51.000000 browserbase-0.1.2/browserbase.egg-info/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      291 2024-05-13 10:27:51.000000 browserbase-0.1.2/browserbase.egg-info/SOURCES.txt
--rw-r--r--   0 mish       (501) staff       (20)        1 2024-05-13 10:27:51.000000 browserbase-0.1.2/browserbase.egg-info/dependency_links.txt
--rw-r--r--   0 mish       (501) staff       (20)       49 2024-05-13 10:27:51.000000 browserbase-0.1.2/browserbase.egg-info/requires.txt
--rw-r--r--   0 mish       (501) staff       (20)       12 2024-05-13 10:27:51.000000 browserbase-0.1.2/browserbase.egg-info/top_level.txt
--rw-r--r--   0 mish       (501) staff       (20)      697 2024-05-13 10:27:39.000000 browserbase-0.1.2/pyproject.toml
--rw-r--r--   0 mish       (501) staff       (20)       38 2024-05-13 10:27:51.546793 browserbase-0.1.2/setup.cfg
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-16 14:17:32.346690 browserbase-0.1.3/
+-rw-r--r--   0 mish       (501) staff       (20)     1064 2024-04-09 17:45:47.000000 browserbase-0.1.3/LICENSE
+-rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-16 14:17:32.346409 browserbase-0.1.3/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      933 2024-04-19 10:57:22.000000 browserbase-0.1.3/README.md
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-16 14:17:32.344583 browserbase-0.1.3/browserbase/
+-rw-r--r--   0 mish       (501) staff       (20)    10720 2024-05-16 14:16:11.000000 browserbase-0.1.3/browserbase/__init__.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-16 14:17:32.345845 browserbase-0.1.3/browserbase/helpers/
+-rw-r--r--   0 mish       (501) staff       (20)      301 2024-04-16 18:32:01.000000 browserbase-0.1.3/browserbase/helpers/anthropic.py
+-rw-r--r--   0 mish       (501) staff       (20)      503 2024-04-15 12:54:51.000000 browserbase-0.1.3/browserbase/helpers/gpt4.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-16 14:17:32.346166 browserbase-0.1.3/browserbase.egg-info/
+-rw-r--r--   0 mish       (501) staff       (20)     1575 2024-05-16 14:17:32.000000 browserbase-0.1.3/browserbase.egg-info/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      291 2024-05-16 14:17:32.000000 browserbase-0.1.3/browserbase.egg-info/SOURCES.txt
+-rw-r--r--   0 mish       (501) staff       (20)        1 2024-05-16 14:17:32.000000 browserbase-0.1.3/browserbase.egg-info/dependency_links.txt
+-rw-r--r--   0 mish       (501) staff       (20)       49 2024-05-16 14:17:32.000000 browserbase-0.1.3/browserbase.egg-info/requires.txt
+-rw-r--r--   0 mish       (501) staff       (20)       12 2024-05-16 14:17:32.000000 browserbase-0.1.3/browserbase.egg-info/top_level.txt
+-rw-r--r--   0 mish       (501) staff       (20)      697 2024-05-16 14:17:21.000000 browserbase-0.1.3/pyproject.toml
+-rw-r--r--   0 mish       (501) staff       (20)       38 2024-05-16 14:17:32.346742 browserbase-0.1.3/setup.cfg
```

### Comparing `browserbase-0.1.2/LICENSE` & `browserbase-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `browserbase-0.1.2/PKG-INFO` & `browserbase-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserbase
-Version: 0.1.2
+Version: 0.1.3
 Summary: Browserbase Python SDK
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Source, https://github.com/browserbase/python-sdk
 Project-URL: Issues, https://github.com/browserbase/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `browserbase-0.1.2/README.md` & `browserbase-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `browserbase-0.1.2/browserbase/__init__.py` & `browserbase-0.1.3/browserbase/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
             return html
 
     def load_urls(
         self,
         urls: Sequence[str],
         text_content: bool = False,
         session_id: Optional[str] = None,
-        proxy: Optional[bool] = False,
+        proxy: Optional[bool] = None,
     ):
         """Load multiple pages in a headless browser and return the contents"""
         if not urls:
             raise ValueError("Page URL was not provided")
 
         with sync_playwright() as p:
             browser = p.chromium.connect_over_cdp(
```

### Comparing `browserbase-0.1.2/browserbase.egg-info/PKG-INFO` & `browserbase-0.1.3/browserbase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserbase
-Version: 0.1.2
+Version: 0.1.3
 Summary: Browserbase Python SDK
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Source, https://github.com/browserbase/python-sdk
 Project-URL: Issues, https://github.com/browserbase/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `browserbase-0.1.2/pyproject.toml` & `browserbase-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "browserbase"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Browserbase", email="info@browserbase.com" },
 ]
 description = "Browserbase Python SDK"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

