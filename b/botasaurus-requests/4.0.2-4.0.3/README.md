# Comparing `tmp/botasaurus_requests-4.0.2.tar.gz` & `tmp/botasaurus_requests-4.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "botasaurus_requests-4.0.2.tar", last modified: Thu May 16 12:30:42 2024, max compression
+gzip compressed data, was "botasaurus_requests-4.0.3.tar", last modified: Thu May 16 15:05:38 2024, max compression
```

## Comparing `botasaurus_requests-4.0.2.tar` & `botasaurus_requests-4.0.3.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2024-05-16 12:30:42.110888 botasaurus_requests-4.0.2/
--rw-rw-rw-   0        0        0    11558 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.2/LICENSE
--rw-rw-rw-   0        0        0       14 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.2/MANIFEST.in
--rw-rw-rw-   0        0        0    14535 2024-05-16 12:30:42.110554 botasaurus_requests-4.0.2/PKG-INFO
--rw-rw-rw-   0        0        0      609 2024-05-16 07:09:14.000000 botasaurus_requests-4.0.2/README.md
-drwxrwxrwx   0        0        0        0 2024-05-16 12:30:42.062419 botasaurus_requests-4.0.2/botasaurus_requests/
--rw-rw-rw-   0        0        0      700 2024-05-16 11:45:50.000000 botasaurus_requests-4.0.2/botasaurus_requests/__init__.py
--rw-rw-rw-   0        0        0     4939 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.2/botasaurus_requests/__main__.py
--rw-rw-rw-   0        0        0       21 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.2/botasaurus_requests/__version__.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:30:42.106170 botasaurus_requests-4.0.2/botasaurus_requests/bin/
--rw-rw-rw-   0        0        0        0 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.2/botasaurus_requests/bin/__init__.py
--rw-rw-rw-   0        0        0     6715 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.2/botasaurus_requests/cffi.py
--rw-rw-rw-   0        0        0    15963 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.2/botasaurus_requests/client.py
--rw-rw-rw-   0        0        0    16718 2024-05-16 06:48:02.000000 botasaurus_requests-4.0.2/botasaurus_requests/cookies.py
--rw-rw-rw-   0        0        0      767 2024-05-16 06:02:03.000000 botasaurus_requests-4.0.2/botasaurus_requests/exceptions.py
--rw-rw-rw-   0        0        0     6026 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.2/botasaurus_requests/headers.py
--rw-rw-rw-   0        0        0    16753 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.2/botasaurus_requests/parser.py
--rw-rw-rw-   0        0        0    19318 2024-05-16 11:31:13.000000 botasaurus_requests-4.0.2/botasaurus_requests/reqs.py
--rw-rw-rw-   0        0        0     8486 2024-05-16 11:43:30.000000 botasaurus_requests-4.0.2/botasaurus_requests/request_class.py
--rw-rw-rw-   0        0        0       19 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.2/botasaurus_requests/request_functions.py
--rw-rw-rw-   0        0        0     9875 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.2/botasaurus_requests/response.py
--rw-rw-rw-   0        0        0    12167 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.2/botasaurus_requests/session.py
--rw-rw-rw-   0        0        0     4692 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.2/botasaurus_requests/toolbelt.py
-drwxrwxrwx   0        0        0        0 2024-05-16 12:30:42.108779 botasaurus_requests-4.0.2/botasaurus_requests.egg-info/
--rw-rw-rw-   0        0        0    14535 2024-05-16 12:30:41.000000 botasaurus_requests-4.0.2/botasaurus_requests.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      797 2024-05-16 12:30:41.000000 botasaurus_requests-4.0.2/botasaurus_requests.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-05-16 12:30:41.000000 botasaurus_requests-4.0.2/botasaurus_requests.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-05-16 12:30:41.000000 botasaurus_requests-4.0.2/botasaurus_requests.egg-info/requires.txt
--rw-rw-rw-   0        0        0       20 2024-05-16 12:30:41.000000 botasaurus_requests-4.0.2/botasaurus_requests.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1008 2024-05-16 12:30:40.000000 botasaurus_requests-4.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       81 2024-05-16 12:30:42.120408 botasaurus_requests-4.0.2/setup.cfg
--rw-rw-rw-   0        0        0       39 2024-04-24 07:16:00.000000 botasaurus_requests-4.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:05:38.684731 botasaurus_requests-4.0.3/
+-rw-rw-rw-   0        0        0    11558 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.3/LICENSE
+-rw-rw-rw-   0        0        0       14 2024-05-16 05:34:38.000000 botasaurus_requests-4.0.3/MANIFEST.in
+-rw-rw-rw-   0        0        0    14535 2024-05-16 15:05:38.683715 botasaurus_requests-4.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2024-05-16 07:09:14.000000 botasaurus_requests-4.0.3/README.md
+drwxrwxrwx   0        0        0        0 2024-05-16 15:05:38.627621 botasaurus_requests-4.0.3/botasaurus_requests/
+-rw-rw-rw-   0        0        0      700 2024-05-16 11:45:50.000000 botasaurus_requests-4.0.3/botasaurus_requests/__init__.py
+-rw-rw-rw-   0        0        0     4939 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.3/botasaurus_requests/__main__.py
+-rw-rw-rw-   0        0        0       21 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.3/botasaurus_requests/__version__.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:05:38.678490 botasaurus_requests-4.0.3/botasaurus_requests/bin/
+-rw-rw-rw-   0        0        0        0 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.3/botasaurus_requests/bin/__init__.py
+-rw-rw-rw-   0        0        0     7338 2024-05-16 13:27:52.000000 botasaurus_requests-4.0.3/botasaurus_requests/cffi.py
+-rw-rw-rw-   0        0        0    15963 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.3/botasaurus_requests/client.py
+-rw-rw-rw-   0        0        0    16718 2024-05-16 06:48:02.000000 botasaurus_requests-4.0.3/botasaurus_requests/cookies.py
+-rw-rw-rw-   0        0        0      767 2024-05-16 06:02:03.000000 botasaurus_requests-4.0.3/botasaurus_requests/exceptions.py
+-rw-rw-rw-   0        0        0     6026 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.3/botasaurus_requests/headers.py
+-rw-rw-rw-   0        0        0    16753 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.3/botasaurus_requests/parser.py
+-rw-rw-rw-   0        0        0    19318 2024-05-16 11:31:13.000000 botasaurus_requests-4.0.3/botasaurus_requests/reqs.py
+-rw-rw-rw-   0        0        0     8486 2024-05-16 11:43:30.000000 botasaurus_requests-4.0.3/botasaurus_requests/request_class.py
+-rw-rw-rw-   0        0        0       19 2024-05-16 12:29:29.000000 botasaurus_requests-4.0.3/botasaurus_requests/request_functions.py
+-rw-rw-rw-   0        0        0     9871 2024-05-16 15:04:13.000000 botasaurus_requests-4.0.3/botasaurus_requests/response.py
+-rw-rw-rw-   0        0        0    12167 2024-05-16 06:58:22.000000 botasaurus_requests-4.0.3/botasaurus_requests/session.py
+-rw-rw-rw-   0        0        0     4692 2024-05-16 05:45:16.000000 botasaurus_requests-4.0.3/botasaurus_requests/toolbelt.py
+drwxrwxrwx   0        0        0        0 2024-05-16 15:05:38.681515 botasaurus_requests-4.0.3/botasaurus_requests.egg-info/
+-rw-rw-rw-   0        0        0    14535 2024-05-16 15:05:38.000000 botasaurus_requests-4.0.3/botasaurus_requests.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      797 2024-05-16 15:05:38.000000 botasaurus_requests-4.0.3/botasaurus_requests.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-05-16 15:05:38.000000 botasaurus_requests-4.0.3/botasaurus_requests.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-05-16 15:05:38.000000 botasaurus_requests-4.0.3/botasaurus_requests.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       20 2024-05-16 15:05:38.000000 botasaurus_requests-4.0.3/botasaurus_requests.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1008 2024-05-16 15:05:36.000000 botasaurus_requests-4.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       81 2024-05-16 15:05:38.688470 botasaurus_requests-4.0.3/setup.cfg
+-rw-rw-rw-   0        0        0       39 2024-04-24 07:16:00.000000 botasaurus_requests-4.0.3/setup.py
```

### Comparing `botasaurus_requests-4.0.2/LICENSE` & `botasaurus_requests-4.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.2/PKG-INFO` & `botasaurus_requests-4.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus_requests
-Version: 4.0.2
+Version: 4.0.3
 Summary: botasaurus_requests is a fork of the requests library with the playwright dependencies removed.
 Author-email: Chetan <chetan@omkar.cloud>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `botasaurus_requests-4.0.2/README.md` & `botasaurus_requests-4.0.3/README.md`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests/__init__.py` & `botasaurus_requests-4.0.3/botasaurus_requests/__init__.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests/__main__.py` & `botasaurus_requests-4.0.3/botasaurus_requests/__main__.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests/cffi.py` & `botasaurus_requests-4.0.3/botasaurus_requests/cffi.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,30 @@
     'armv7l': 'arm-7',
     'ppc64le': 'ppc64le',
     'riscv64': 'riscv64',
     's390x': 's390x',
 }
 
 
+def move_file(src_path: Path, dst_path: Path):
+    import shutil
+    try:
+        # Check if the source file exists
+        if src_path.is_file():
+            # Create the destination directory if it doesn't exist
+            dst_path.parent.mkdir(parents=True, exist_ok=True)
+            
+            # Move the file
+            shutil.move(str(src_path), str(dst_path))
+        else:
+            print(f"Source file not found: {src_path}")
+    except Exception as e:
+        print(f"Error occurred: {e}")
+
+
 class LibraryManager:
     def __init__(self) -> None:
         self.parent_path: Path = root_dir / 'bin'
         self.file_cont, self.file_ext = self.get_name()
         self.file_pref = f'hrequests-cgo-{BRIDGE_VERSION}'
         filename = self.check_library()
         self.full_path: str = str(self.parent_path / filename)
@@ -92,16 +108,20 @@
             asset = self.check_assets(release['assets'])
             if asset:
                 url, name = asset
                 break
         else:
             raise IOError('Could not find a matching binary for your system.')
         # download file
-        file = self.parent_path / name
+        # file = self.parent_path / name
+        file = self.parent_path / 'temp'
         self.download_file(file, url)
+        move_file(file, self.parent_path / name)
+
+
 
     def download_file(self, file, url):
         # handle download_exec
         try:
             with open(file, 'wb') as fstream:
                 self.download_exec(fstream, url)
         except KeyboardInterrupt as e:
```

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests/client.py` & `botasaurus_requests-4.0.3/botasaurus_requests/client.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests/cookies.py` & `botasaurus_requests-4.0.3/botasaurus_requests/cookies.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests/exceptions.py` & `botasaurus_requests-4.0.3/botasaurus_requests/exceptions.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests/headers.py` & `botasaurus_requests-4.0.3/botasaurus_requests/headers.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests/parser.py` & `botasaurus_requests-4.0.3/botasaurus_requests/parser.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests/reqs.py` & `botasaurus_requests-4.0.3/botasaurus_requests/reqs.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests/request_class.py` & `botasaurus_requests-4.0.3/botasaurus_requests/request_class.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests/response.py` & `botasaurus_requests-4.0.3/botasaurus_requests/response.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
+from requests.utils import get_encoding_from_headers
 import re
 from dataclasses import dataclass
 from datetime import datetime, timedelta
 from http.client import responses as status_codes
 from typing import List, Literal, Optional, Union
 
-import cchardet as chardet
 from orjson import dumps, loads
 from requests.exceptions import HTTPError
 
 import botasaurus_requests
 from botasaurus_requests.cffi import library
 from botasaurus_requests.exceptions import ClientException
 
@@ -153,17 +153,16 @@
     browser: Optional[Literal['firefox', 'chrome']] = None
     elapsed: Optional[timedelta] = None
     encoding: str = 'UTF-8'
     is_utf8: bool = True
     proxy: Optional[str] = None
 
     def __post_init__(self) -> None:
-        if type(self.raw) is bytes:
-            self.encoding = chardet.detect(self.raw)['encoding']
-
+        self.encoding = get_encoding_from_headers(self.headers)
+        
     @property
     def reason(self) -> str:
         return status_codes[self.status_code]
 
     def json(self, **kwargs) -> Union[dict, list]:
         return loads(self.content, **kwargs)
```

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests/session.py` & `botasaurus_requests-4.0.3/botasaurus_requests/session.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests/toolbelt.py` & `botasaurus_requests-4.0.3/botasaurus_requests/toolbelt.py`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests.egg-info/PKG-INFO` & `botasaurus_requests-4.0.3/botasaurus_requests.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: botasaurus_requests
-Version: 4.0.2
+Version: 4.0.3
 Summary: botasaurus_requests is a fork of the requests library with the playwright dependencies removed.
 Author-email: Chetan <chetan@omkar.cloud>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
```

### Comparing `botasaurus_requests-4.0.2/botasaurus_requests.egg-info/SOURCES.txt` & `botasaurus_requests-4.0.3/botasaurus_requests.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `botasaurus_requests-4.0.2/pyproject.toml` & `botasaurus_requests-4.0.3/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "botasaurus_requests"
-version="4.0.2"
+version="4.0.3"
 description = "botasaurus_requests is a fork of the requests library with the playwright dependencies removed."
 authors = [
   {name = "Chetan", email = "chetan@omkar.cloud" } # Optional
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 keywords = [
```

