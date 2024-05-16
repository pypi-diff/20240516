# Comparing `tmp/idms-0.2.4.tar.gz` & `tmp/idms-0.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idms-0.2.4.tar", last modified: Tue Sep 26 07:01:20 2023, max compression
+gzip compressed data, was "idms-0.2.6.tar", last modified: Thu May 16 14:00:59 2024, max compression
```

## Comparing `idms-0.2.4.tar` & `idms-0.2.6.tar`

### file list

```diff
@@ -1,28 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 07:01:20.133611 idms-0.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1079 2023-09-26 07:00:52.000000 idms-0.2.4/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2023-09-26 07:00:52.000000 idms-0.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2023-09-26 07:01:20.133611 idms-0.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1526 2023-09-26 07:00:52.000000 idms-0.2.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 07:01:20.129611 idms-0.2.4/data/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-26 07:00:52.000000 idms-0.2.4/data/data_file
--rw-r--r--   0 runner    (1001) docker     (127)      261 2023-09-26 07:00:52.000000 idms-0.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       78 2023-09-26 07:01:20.133611 idms-0.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     8676 2023-09-26 07:00:52.000000 idms-0.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 07:01:20.125611 idms-0.2.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 07:01:20.129611 idms-0.2.4/src/idms/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-26 07:00:52.000000 idms-0.2.4/src/idms/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 07:01:20.133611 idms-0.2.4/src/idms/api/
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-09-26 07:00:52.000000 idms-0.2.4/src/idms/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13125 2023-09-26 07:00:52.000000 idms-0.2.4/src/idms/api/contentserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      586 2023-09-26 07:00:52.000000 idms-0.2.4/src/idms/functions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 07:01:20.133611 idms-0.2.4/src/idms.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2611 2023-09-26 07:01:20.000000 idms-0.2.4/src/idms.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2023-09-26 07:01:20.000000 idms-0.2.4/src/idms.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-09-26 07:01:20.000000 idms-0.2.4/src/idms.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       39 2023-09-26 07:01:20.000000 idms-0.2.4/src/idms.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      101 2023-09-26 07:01:20.000000 idms-0.2.4/src/idms.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2023-09-26 07:01:20.000000 idms-0.2.4/src/idms.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-09-26 07:01:20.133611 idms-0.2.4/src/sample/
--rw-r--r--   0 runner    (1001) docker     (127)      111 2023-09-26 07:00:52.000000 idms-0.2.4/src/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)        9 2023-09-26 07:00:52.000000 idms-0.2.4/src/sample/package_data.dat
--rw-r--r--   0 runner    (1001) docker     (127)       43 2023-09-26 07:00:52.000000 idms-0.2.4/src/sample/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:00:59.675454 idms-0.2.6/
+-rw-r--r--   0 runner    (1001) docker     (127)     1079 2024-05-16 14:00:51.000000 idms-0.2.6/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      157 2024-05-16 14:00:51.000000 idms-0.2.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-16 14:00:59.675454 idms-0.2.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1526 2024-05-16 14:00:51.000000 idms-0.2.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:00:59.671454 idms-0.2.6/data/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 14:00:51.000000 idms-0.2.6/data/data_file
+-rw-r--r--   0 runner    (1001) docker     (127)     1401 2024-05-16 14:00:51.000000 idms-0.2.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-05-16 14:00:59.675454 idms-0.2.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     8677 2024-05-16 14:00:51.000000 idms-0.2.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:00:59.671454 idms-0.2.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:00:59.671454 idms-0.2.6/src/idms/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 14:00:51.000000 idms-0.2.6/src/idms/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:00:59.671454 idms-0.2.6/src/idms/api/
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-05-16 14:00:51.000000 idms-0.2.6/src/idms/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13276 2024-05-16 14:00:51.000000 idms-0.2.6/src/idms/api/contentserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4174 2024-05-16 14:00:51.000000 idms-0.2.6/src/idms/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:00:59.675454 idms-0.2.6/src/idms.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2868 2024-05-16 14:00:59.000000 idms-0.2.6/src/idms.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      485 2024-05-16 14:00:59.000000 idms-0.2.6/src/idms.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 14:00:59.000000 idms-0.2.6/src/idms.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-05-16 14:00:59.000000 idms-0.2.6/src/idms.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-05-16 14:00:59.000000 idms-0.2.6/src/idms.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-05-16 14:00:59.000000 idms-0.2.6/src/idms.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:00:59.671454 idms-0.2.6/src/sample/
+-rw-r--r--   0 runner    (1001) docker     (127)      111 2024-05-16 14:00:51.000000 idms-0.2.6/src/sample/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-05-16 14:00:51.000000 idms-0.2.6/src/sample/package_data.dat
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-05-16 14:00:51.000000 idms-0.2.6/src/sample/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 14:00:59.675454 idms-0.2.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      445 2024-05-16 14:00:51.000000 idms-0.2.6/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      416 2024-05-16 14:00:51.000000 idms-0.2.6/tests/test_simple.py
```

### Comparing `idms-0.2.4/LICENSE.txt` & `idms-0.2.6/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `idms-0.2.4/PKG-INFO` & `idms-0.2.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idms
-Version: 0.2.4
+Version: 0.2.6
 Summary: Python class to talk to idms REST and Search API, better known as iDMS.
 Home-page: https://github.com/Provincie-Zuid-Holland/idms
 Author: Daniel Overdevest, Michael de Winter
 Author-email: d.overdevest@pzh.nl, mr.de.winter@pzh.nl
 Project-URL: Bug Reports, https://github.com/ProvZH/idms/issues
 Project-URL: Source, https://github.com/ProvZH/idms
 Keywords: idms,contentserver,restapi,searchapi
@@ -16,17 +16,23 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.5, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: requests>=2.25.0
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
+Requires-Dist: python-dotenv>=0.15.0; extra == "dev"
+Requires-Dist: pandas>=1.1.4; extra == "dev"
+Requires-Dist: openpyxl; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE.txt
+Requires-Dist: coverage; extra == "test"
 
 # iDMS
 
 ![Upload Python Package](https://github.com/ProvZH/iDMS/workflows/Upload%20Python%20Package/badge.svg)
 
 
 Python class to talk to iDMS REST and Search API within Provincie Zuid-Holland.
```

### Comparing `idms-0.2.4/README.md` & `idms-0.2.6/README.md`

 * *Files identical despite different names*

### Comparing `idms-0.2.4/setup.py` & `idms-0.2.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,17 +2,18 @@
 
 See:
 https://packaging.python.org/guides/distributing-packages-using-setuptools/
 https://github.com/pypa/sampleproject
 """
 
 # Always prefer setuptools over distutils
-from setuptools import setup, find_packages
 import pathlib
 
+from setuptools import find_packages, setup
+
 here = pathlib.Path(__file__).parent.resolve()
 
 # Get the long description from the README file
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
@@ -32,15 +33,15 @@
     name="idms",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/en/latest/single_source_version.html
-    version="0.2.4",  # Required
+    version="0.2.6",  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="Python class to talk to idms REST and Search API, better known as iDMS.",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `idms-0.2.4/src/idms/api/contentserver.py` & `idms-0.2.6/src/idms/api/contentserver.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-import requests
-import urllib
-import logging
-import json
-import datetime, time
 import copy
-import idms.functions as otfunc
-from requests.adapters import HTTPAdapter
-from requests.packages.urllib3.util.retry import Retry
-from urllib.parse import urlparse, urlunparse, parse_qs
-from functools import reduce
+import datetime
+import json
+import logging
 import os
-import uuid
 import time
-import random
+from functools import reduce
+from urllib.parse import parse_qs, urlparse, urlunparse
+from urllib.request import pathname2url
+
+import numpy as np
+import requests
+from requests.adapters import HTTPAdapter
+from requests.packages.urllib3.util.retry import Retry
+
+import idms.functions as otfunc
 
 
 def dotfield(input_dict: dict, input_key: str, notFound=None) -> str:
     """
     Magic function to get nested properties from dictionary writen as level1.level2.level3.
 
     Example:
@@ -36,35 +37,36 @@
         self,
         baseUrl: str,
         username: str = None,
         password: str = None,
         ticket: str = None,
         verifySSL: bool = True,
         maxErrorRetry: int = 10,
+        post_error_retries: int = 10,
     ):
         # Settings for retry and auto retry if error code 500 is given
         retry = Retry(
-            total=10,
-            read=10,
-            connect=10,
+            total=post_error_retries,
+            read=post_error_retries,
+            connect=post_error_retries,
             backoff_factor=1,
             status_forcelist=(500, 502, 503, 504),
         )
 
         # Mounts a session for re-use authorization
         self.baseUrl = baseUrl
         self.session = requests.Session()
         self.session.verify = verifySSL
         self.session.mount(baseUrl, HTTPAdapter(max_retries=retry))
 
         # Safety measures to not to overload the server.
         self.maxCallsPerFolder = 10000
         self.gracefulSleepSeconds = 0.01
 
-        # Type 0 is always a folder, 751 is for ProvZH an E-mailmap and 136 for Samengesteld document and 298 for a Collectie.
+        # Type 0 is always a folder, 751 is for ProvZH and E-mailmap and 136 for Samengesteld document and 298 for a Collectie.
         self.folderTypes = [0, 751, 136, 298]
         self.folderTypesStopRecursive = [136, 298]
 
         self.includeParentsPath = True
         self.outputColumns = [
             "properties.parent_id",
             "properties.id",
@@ -79,15 +81,15 @@
             "properties.type_name",
             "properties.summary",
             "properties.description_multilingual.nl",
             "regions.OTLocation",
             "systemattributes.Dossiernummer",
         ]
 
-        self.debugJson = False
+        self.debugJson = True
 
         # Retry faulty urls, extra fall back when it's not a HTTP code.
         self.maxErrorRetry = maxErrorRetry
 
         if ticket:
             self.ticket = ticket
         else:
@@ -226,32 +228,32 @@
 
     def search(
         self,
         complexQuery: str,
         limit: int = 10,
         metadata: str = "true",
         slice: str = None,
-        resume_last_position = True
+        resume_last_position=True,
     ) -> list:
         """
         Search API endpoint
         Example: {self.baseUrl}/api/v2/search?where=`complexQuery`&limit=`limit`&metadata=`metadata`
 
         :param str `complexQuery`:  See documentation for search options for a complexQuery: https://docs2.cer-rec.gc.ca/ll-eng/llisapi.dll?func=help.index&keyword=LL.Search%20Broker.Category
         """
-    
-        file_path_resume = os.getcwd()+"/"+str(complexQuery)+"_last_position.txt"
 
-        results = []
+        file_path_resume = os.getcwd() + "/" + pathname2url(complexQuery)[0:15] + "_last_position.txt"
+
+        results = np.array([])
         headers = {"otcsticket": self.ticket}
         counter = 0
 
-        if os.path.exists(file_path_resume) and resume_last_position is True:       
+        if os.path.exists(file_path_resume) and resume_last_position is True:
             with open(file_path_resume, "r") as file:
-                url  = file.read()
+                url = file.read()
         else:
             url = self.baseUrl + "/api/v2/search"
 
         max_error_retries = 0
 
         base_data = {"where": complexQuery, "limit": limit, "metadata": metadata}
         if slice:
@@ -293,41 +295,44 @@
                     dataRow = result.get("data")
                     row = self.parseNodeColumns(dataRow)
 
                     ancestorsList = dotfield(result, "links.ancestors", [])
                     ancestorsStr = " > ".join([a.get("name") for a in ancestorsList])
                     row["locationPathString"] = ancestorsStr
                     row["complexQuery"] = complexQuery
-                    results.append(row)
+                    results = np.append(results, row)
 
                 # Determine if there is a next page and prepare for next while-loop.
                 # nextUrl contains a GET url to retrieve the next page.
                 nextUrl = dotfield(search_results, "collection.paging.links.next.href")
 
                 logging.debug(f" > nextUrl: {nextUrl}")
 
                 if nextUrl:
                     url = self.baseUrl + nextUrl
-                    with open(file_path_resume, "w") as file:              
+                    with open(file_path_resume, "w") as file:
                         file.write(str(url))
                 else:
                     url = ""
 
             except Exception as e:
                 max_error_retries = max_error_retries + 1
                 print(e)
                 logging.debug("Error: " + str(e))
 
         # Inform the user that the max error retries has been met.
         if max_error_retries >= self.maxErrorRetry:
-            logging.warning(f"Stopped due max error tries: ({max_error_retries}) reached the max error retry ({self.maxErrorRetry}) limit!")
-            with open(file_path_resume, "w") as file:              
+            logging.warning(
+                f"Stopped due max error tries: ({max_error_retries}) reached the max error retry ({self.maxErrorRetry}) limit!"
+            )
+            with open(file_path_resume, "w") as file:
                 file.write(str(url))
 
-        
         # Inform user if stopped earlier due maxCallsPerFolder variable
         if counter >= self.maxCallsPerFolder:
-            logging.warning(f"Stopped due counter ({counter}) reached the maxCallsPerFolder ({self.maxCallsPerFolder}) limit!")
-            with open(file_path_resume, "w") as file:              
+            logging.warning(
+                f"Stopped due counter ({counter}) reached the maxCallsPerFolder ({self.maxCallsPerFolder}) limit!"
+            )
+            with open(file_path_resume, "w") as file:
                 file.write(str(url))
 
-        return results
+        return results.tolist()
```

### Comparing `idms-0.2.4/src/idms.egg-info/PKG-INFO` & `idms-0.2.6/src/idms.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idms
-Version: 0.2.4
+Version: 0.2.6
 Summary: Python class to talk to idms REST and Search API, better known as iDMS.
 Home-page: https://github.com/Provincie-Zuid-Holland/idms
 Author: Daniel Overdevest, Michael de Winter
 Author-email: d.overdevest@pzh.nl, mr.de.winter@pzh.nl
 Project-URL: Bug Reports, https://github.com/ProvZH/idms/issues
 Project-URL: Source, https://github.com/ProvZH/idms
 Keywords: idms,contentserver,restapi,searchapi
@@ -16,17 +16,23 @@
 Classifier: Programming Language :: Python :: 3.5
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Requires-Python: >=3.5, <4
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+Requires-Dist: requests>=2.25.0
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
+Requires-Dist: python-dotenv>=0.15.0; extra == "dev"
+Requires-Dist: pandas>=1.1.4; extra == "dev"
+Requires-Dist: openpyxl; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE.txt
+Requires-Dist: coverage; extra == "test"
 
 # iDMS
 
 ![Upload Python Package](https://github.com/ProvZH/iDMS/workflows/Upload%20Python%20Package/badge.svg)
 
 
 Python class to talk to iDMS REST and Search API within Provincie Zuid-Holland.
```

