# Comparing `tmp/browserbase_haystack-0.0.3.tar.gz` & `tmp/browserbase_haystack-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserbase_haystack-0.0.3.tar", last modified: Mon May 13 10:30:07 2024, max compression
+gzip compressed data, was "browserbase_haystack-0.0.4.tar", last modified: Thu May 16 11:43:49 2024, max compression
```

## Comparing `browserbase_haystack-0.0.3.tar` & `browserbase_haystack-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-13 10:30:07.752153 browserbase_haystack-0.0.3/
--rw-r--r--   0 mish       (501) staff       (20)     1063 2024-04-18 21:20:37.000000 browserbase_haystack-0.0.3/LICENSE
--rw-r--r--   0 mish       (501) staff       (20)     2956 2024-05-13 10:30:07.751965 browserbase_haystack-0.0.3/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)     2343 2024-05-13 10:23:31.000000 browserbase_haystack-0.0.3/README.md
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-13 10:30:07.750963 browserbase_haystack-0.0.3/browserbase_haystack/
--rw-r--r--   0 mish       (501) staff       (20)     1004 2024-05-13 10:25:51.000000 browserbase_haystack-0.0.3/browserbase_haystack/__init__.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-13 10:30:07.751768 browserbase_haystack-0.0.3/browserbase_haystack.egg-info/
--rw-r--r--   0 mish       (501) staff       (20)     2956 2024-05-13 10:30:07.000000 browserbase_haystack-0.0.3/browserbase_haystack.egg-info/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      284 2024-05-13 10:30:07.000000 browserbase_haystack-0.0.3/browserbase_haystack.egg-info/SOURCES.txt
--rw-r--r--   0 mish       (501) staff       (20)        1 2024-05-13 10:30:07.000000 browserbase_haystack-0.0.3/browserbase_haystack.egg-info/dependency_links.txt
--rw-r--r--   0 mish       (501) staff       (20)       24 2024-05-13 10:30:07.000000 browserbase_haystack-0.0.3/browserbase_haystack.egg-info/requires.txt
--rw-r--r--   0 mish       (501) staff       (20)       21 2024-05-13 10:30:07.000000 browserbase_haystack-0.0.3/browserbase_haystack.egg-info/top_level.txt
--rw-r--r--   0 mish       (501) staff       (20)      672 2024-05-13 10:29:43.000000 browserbase_haystack-0.0.3/pyproject.toml
--rw-r--r--   0 mish       (501) staff       (20)       38 2024-05-13 10:30:07.752204 browserbase_haystack-0.0.3/setup.cfg
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-16 11:43:49.838698 browserbase_haystack-0.0.4/
+-rw-r--r--   0 mish       (501) staff       (20)     1063 2024-04-18 21:20:37.000000 browserbase_haystack-0.0.4/LICENSE
+-rw-r--r--   0 mish       (501) staff       (20)     2956 2024-05-16 11:43:49.838452 browserbase_haystack-0.0.4/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)     2343 2024-05-14 19:56:21.000000 browserbase_haystack-0.0.4/README.md
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-16 11:43:49.837237 browserbase_haystack-0.0.4/browserbase_haystack/
+-rw-r--r--   0 mish       (501) staff       (20)     1075 2024-05-14 19:57:06.000000 browserbase_haystack-0.0.4/browserbase_haystack/__init__.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-05-16 11:43:49.838188 browserbase_haystack-0.0.4/browserbase_haystack.egg-info/
+-rw-r--r--   0 mish       (501) staff       (20)     2956 2024-05-16 11:43:49.000000 browserbase_haystack-0.0.4/browserbase_haystack.egg-info/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      284 2024-05-16 11:43:49.000000 browserbase_haystack-0.0.4/browserbase_haystack.egg-info/SOURCES.txt
+-rw-r--r--   0 mish       (501) staff       (20)        1 2024-05-16 11:43:49.000000 browserbase_haystack-0.0.4/browserbase_haystack.egg-info/dependency_links.txt
+-rw-r--r--   0 mish       (501) staff       (20)       24 2024-05-16 11:43:49.000000 browserbase_haystack-0.0.4/browserbase_haystack.egg-info/requires.txt
+-rw-r--r--   0 mish       (501) staff       (20)       21 2024-05-16 11:43:49.000000 browserbase_haystack-0.0.4/browserbase_haystack.egg-info/top_level.txt
+-rw-r--r--   0 mish       (501) staff       (20)      672 2024-05-16 11:43:43.000000 browserbase_haystack-0.0.4/pyproject.toml
+-rw-r--r--   0 mish       (501) staff       (20)       38 2024-05-16 11:43:49.838773 browserbase_haystack-0.0.4/setup.cfg
```

### Comparing `browserbase_haystack-0.0.3/LICENSE` & `browserbase_haystack-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `browserbase_haystack-0.0.3/PKG-INFO` & `browserbase_haystack-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserbase-haystack
-Version: 0.0.3
+Version: 0.0.4
 Summary: Browserbase Haystack Fetcher
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Issues, https://github.com/browserbase/haystack/issues
 Project-URL: Source, https://github.com/browserbase/haystack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -72,10 +72,10 @@
 pipe.connect("prompt_builder.prompt", "llm.prompt")
 result = pipe.run(data={"fetcher": {"urls": ["https://example.com"]}})
 ```
 
 ### Parameters
 
 - `urls` Required. A list of URLs to fetch
+- `text_content` Optional. Only return page text content
 - `session_id` Optional. The Session ID
 - `proxy` Optional. Enable Proxy
-- `text_content` Optional. Only return page text content
```

### Comparing `browserbase_haystack-0.0.3/README.md` & `browserbase_haystack-0.0.4/README.md`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -55,10 +55,10 @@
 pipe.connect("prompt_builder.prompt", "llm.prompt")
 result = pipe.run(data={"fetcher": {"urls": ["https://example.com"]}})
 ```
 
 ### Parameters
 
 - `urls` Required. A list of URLs to fetch
+- `text_content` Optional. Only return page text content
 - `session_id` Optional. The Session ID
 - `proxy` Optional. Enable Proxy
-- `text_content` Optional. Only return page text content
```

### Comparing `browserbase_haystack-0.0.3/browserbase_haystack/__init__.py` & `browserbase_haystack-0.0.4/browserbase_haystack/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 from haystack.dataclasses import Document
 from browserbase import Browserbase
 from typing import Optional, List, Sequence
 
 
 @component
 class BrowserbaseFetcher:
-    def __init__(self, api_key: Optional[str] = None) -> None:
-        self.browserbase = Browserbase(api_key=api_key)
+    def __init__(
+        self, api_key: Optional[str] = None, project_id: Optional[str] = None
+    ) -> None:
+        self.browserbase = Browserbase(api_key=api_key, project_id=project_id)
 
     @component.output_types(documents=List[Document])
     def run(
         self,
         urls: Sequence[str],
         text_content: bool = False,
         session_id: Optional[str] = None,
```

### Comparing `browserbase_haystack-0.0.3/browserbase_haystack.egg-info/PKG-INFO` & `browserbase_haystack-0.0.4/browserbase_haystack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserbase-haystack
-Version: 0.0.3
+Version: 0.0.4
 Summary: Browserbase Haystack Fetcher
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://browserbase.com
 Project-URL: Issues, https://github.com/browserbase/haystack/issues
 Project-URL: Source, https://github.com/browserbase/haystack
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -72,10 +72,10 @@
 pipe.connect("prompt_builder.prompt", "llm.prompt")
 result = pipe.run(data={"fetcher": {"urls": ["https://example.com"]}})
 ```
 
 ### Parameters
 
 - `urls` Required. A list of URLs to fetch
+- `text_content` Optional. Only return page text content
 - `session_id` Optional. The Session ID
 - `proxy` Optional. Enable Proxy
-- `text_content` Optional. Only return page text content
```

### Comparing `browserbase_haystack-0.0.3/pyproject.toml` & `browserbase_haystack-0.0.4/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "browserbase-haystack"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Browserbase", email="info@browserbase.com" },
 ]
 description = "Browserbase Haystack Fetcher"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

