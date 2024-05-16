# Comparing `tmp/ecoinvent_interface-2.4.1.tar.gz` & `tmp/ecoinvent_interface-2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ecoinvent_interface-2.4.1.tar", last modified: Thu Dec  7 15:07:52 2023, max compression
+gzip compressed data, was "ecoinvent_interface-2.5.tar", last modified: Thu May 16 15:09:55 2024, max compression
```

## Comparing `ecoinvent_interface-2.4.1.tar` & `ecoinvent_interface-2.5.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:07:52.238407 ecoinvent_interface-2.4.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1091 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       82 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    13529 2023-12-07 15:07:52.234407 ecoinvent_interface-2.4.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    11983 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:07:52.222407 ecoinvent_interface-2.4.1/ecoinvent_interface/
--rw-r--r--   0 runner    (1001) docker     (127)      540 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/ecoinvent_interface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9683 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/ecoinvent_interface/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:07:52.222407 ecoinvent_interface-2.4.1/ecoinvent_interface/data/
--rw-r--r--   0 runner    (1001) docker     (127)  7759238 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/ecoinvent_interface/data/mappings.zip
--rw-r--r--   0 runner    (1001) docker     (127)     2476 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/ecoinvent_interface/mapping.py
--rw-r--r--   0 runner    (1001) docker     (127)     7381 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/ecoinvent_interface/process_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)    12978 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/ecoinvent_interface/release.py
--rw-r--r--   0 runner    (1001) docker     (127)     1218 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/ecoinvent_interface/settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1990 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/ecoinvent_interface/spold_versions.py
--rw-r--r--   0 runner    (1001) docker     (127)     2231 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/ecoinvent_interface/storage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3347 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/ecoinvent_interface/string_distance.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:07:52.234407 ecoinvent_interface-2.4.1/ecoinvent_interface.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13529 2023-12-07 15:07:52.000000 ecoinvent_interface-2.4.1/ecoinvent_interface.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      733 2023-12-07 15:07:52.000000 ecoinvent_interface-2.4.1/ecoinvent_interface.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-12-07 15:07:52.000000 ecoinvent_interface-2.4.1/ecoinvent_interface.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      199 2023-12-07 15:07:52.000000 ecoinvent_interface-2.4.1/ecoinvent_interface.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       20 2023-12-07 15:07:52.000000 ecoinvent_interface-2.4.1/ecoinvent_interface.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-12-07 15:07:52.238407 ecoinvent_interface-2.4.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-12-07 15:07:52.234407 ecoinvent_interface-2.4.1/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     5790 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/tests/test_process_interface.py
--rw-r--r--   0 runner    (1001) docker     (127)     4625 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/tests/test_release.py
--rw-r--r--   0 runner    (1001) docker     (127)      827 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/tests/test_release_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     2654 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (127)     1275 2023-12-07 15:07:39.000000 ecoinvent_interface-2.4.1/tests/test_spold_versions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:09:55.968442 ecoinvent_interface-2.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1091 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    13533 2024-05-16 15:09:55.968442 ecoinvent_interface-2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    11989 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:09:55.956442 ecoinvent_interface-2.5/ecoinvent_interface/
+-rw-r--r--   0 runner    (1001) docker     (127)      538 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/ecoinvent_interface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9793 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/ecoinvent_interface/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:09:55.956442 ecoinvent_interface-2.5/ecoinvent_interface/data/
+-rw-r--r--   0 runner    (1001) docker     (127)  7759238 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/ecoinvent_interface/data/mappings.zip
+-rw-r--r--   0 runner    (1001) docker     (127)     2476 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/ecoinvent_interface/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7432 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/ecoinvent_interface/process_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12978 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/ecoinvent_interface/release.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1218 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/ecoinvent_interface/settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1990 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/ecoinvent_interface/spold_versions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2231 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/ecoinvent_interface/storage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3347 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/ecoinvent_interface/string_distance.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:09:55.968442 ecoinvent_interface-2.5/ecoinvent_interface.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13533 2024-05-16 15:09:55.000000 ecoinvent_interface-2.5/ecoinvent_interface.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      733 2024-05-16 15:09:55.000000 ecoinvent_interface-2.5/ecoinvent_interface.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 15:09:55.000000 ecoinvent_interface-2.5/ecoinvent_interface.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      199 2024-05-16 15:09:55.000000 ecoinvent_interface-2.5/ecoinvent_interface.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       20 2024-05-16 15:09:55.000000 ecoinvent_interface-2.5/ecoinvent_interface.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 15:09:55.968442 ecoinvent_interface-2.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 15:09:55.968442 ecoinvent_interface-2.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     5790 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/tests/test_process_interface.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4625 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/tests/test_release.py
+-rw-r--r--   0 runner    (1001) docker     (127)      827 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/tests/test_release_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2654 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1275 2024-05-16 15:09:52.000000 ecoinvent_interface-2.5/tests/test_spold_versions.py
```

### Comparing `ecoinvent_interface-2.4.1/LICENSE` & `ecoinvent_interface-2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ecoinvent_interface-2.4.1/PKG-INFO` & `ecoinvent_interface-2.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: ecoinvent_interface
-Version: 2.4.1
+Version: 2.5
 Summary: Unofficial client for interfacing with ecoinvent database
 Author-email:  Chris Mutel <cmutel@gmail.com>
 Maintainer-email:  Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/brightway-lca/ecoinvent_interface
 Project-URL: homepage, https://github.com/brightway-lca/ecoinvent_interface
 Project-URL: tracker, https://github.com/brightway-lca/ecoinvent_interface/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: platformdirs
 Requires-Dist: py7zr
 Requires-Dist: pydantic-settings
 Requires-Dist: pyecospold
@@ -40,16 +40,16 @@
 
 # ecoinvent_interface
 
 [![PyPI](https://img.shields.io/pypi/v/ecoinvent_interface.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/ecoinvent_interface.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/ecoinvent_interface)][pypi status]
 
-[pypi status]: https://pypi.org/project/bw_hestia_bridge/
-[tests]: https://github.com/brightway-lca/bw_hestia_bridge/actions?workflow=Tests
+[pypi status]: https://pypi.org/project/ecoinvent-interface/
+[tests]: https://github.com/brightway-lca/ecoinvent_interface/actions?workflow=Tests
 
 This is an **unofficial and unsupported** Python library to get ecoinvent data.
 
 # Quickstart
 
 ```python
 from ecoinvent_interface import Settings, EcoinventRelease, ReleaseType
```

### Comparing `ecoinvent_interface-2.4.1/README.md` & `ecoinvent_interface-2.5/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # ecoinvent_interface
 
 [![PyPI](https://img.shields.io/pypi/v/ecoinvent_interface.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/ecoinvent_interface.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/ecoinvent_interface)][pypi status]
 
-[pypi status]: https://pypi.org/project/bw_hestia_bridge/
-[tests]: https://github.com/brightway-lca/bw_hestia_bridge/actions?workflow=Tests
+[pypi status]: https://pypi.org/project/ecoinvent-interface/
+[tests]: https://github.com/brightway-lca/ecoinvent_interface/actions?workflow=Tests
 
 This is an **unofficial and unsupported** Python library to get ecoinvent data.
 
 # Quickstart
 
 ```python
 from ecoinvent_interface import Settings, EcoinventRelease, ReleaseType
```

### Comparing `ecoinvent_interface-2.4.1/ecoinvent_interface/__init__.py` & `ecoinvent_interface-2.5/ecoinvent_interface/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,14 @@
     "ProcessFileType",
     "ProcessMapping",
     "ReleaseType",
     "Settings",
     "get_excel_lcia_file_for_version",
 ]
 
-__version__ = "2.4.1"
+__version__ = "2.5"
 
 from .storage import CachedStorage
 from .settings import Settings, permanent_setting
 from .release import EcoinventRelease, ReleaseType, get_excel_lcia_file_for_version
 from .process_interface import EcoinventProcess, ProcessFileType
 from .mapping import ProcessMapping
```

### Comparing `ecoinvent_interface-2.4.1/ecoinvent_interface/core.py` & `ecoinvent_interface-2.5/ecoinvent_interface/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,15 +123,16 @@
         logger.debug(message)
 
     def _get_credentials(self, post_data: dict) -> None:
         sso_url = self.urls["sso"]
         headers = {
             "ecoinvent-api-client-library": "ecoinvent_interface",
             "ecoinvent-api-client-library-version": __version__,
-        } | self.custom_headers
+        }
+        headers.update(self.custom_headers)
         response = requests.post(sso_url, post_data, headers=headers, timeout=20)
 
         if response.ok:
             tokens = json.loads(response.text)
             self.last_refresh = time()
             self.access_token = tokens["access_token"]
             self.refresh_token = tokens["refresh_token"]
@@ -144,15 +145,16 @@
     @fresh_login
     def _get_all_reports(self) -> dict:
         reports_url = self.urls["api"] + "files/reports"
         headers = {
             "Authorization": f"Bearer {self.access_token}",
             "ecoinvent-api-client-library": "ecoinvent_interface",
             "ecoinvent-api-client-library-version": __version__,
-        } | self.custom_headers
+        }
+        headers.update(self.custom_headers)
         message = """Requesting URL.
     URL: {reports_url}
     Class: {self.__class__.__name__}
     Instance ID: {id(self)}
     Version: {__version__}
     User: {self.username}
         """
@@ -162,15 +164,16 @@
     @fresh_login
     def _get_all_files(self) -> dict:
         files_url = self.urls["api"] + "files"
         headers = {
             "Authorization": f"Bearer {self.access_token}",
             "ecoinvent-api-client-library": "ecoinvent_interface",
             "ecoinvent-api-client-library-version": __version__,
-        } | self.custom_headers
+        }
+        headers.update(self.custom_headers)
         message = """Requesting URL.
     URL: {files_url}
     Class: {self.__class__.__name__}
     Instance ID: {id(self)}
     Version: {__version__}
     User: {self.username}
         """
@@ -250,15 +253,16 @@
         self, url: str, filename: str, directory: Path, params: Optional[dict] = {}
     ) -> Path:
         url = self.urls["api"] + url
         headers = {
             "Authorization": f"Bearer {self.access_token}",
             "ecoinvent-api-client-library": "ecoinvent_interface",
             "ecoinvent-api-client-library-version": __version__,
-        } | self.custom_headers
+        }
+        headers.update(self.custom_headers)
         self._streaming_download(
             url=url,
             params=params,
             directory=directory,
             headers=headers,
             filename=filename,
         )
@@ -269,15 +273,16 @@
         self, uuid: str, filename: str, url_namespace: str, directory: Path
     ) -> Path:
         url = self.urls["api"] + f"files/{url_namespace}/{uuid}"
         headers = {
             "Authorization": f"Bearer {self.access_token}",
             "ecoinvent-api-client-library": "ecoinvent_interface",
             "ecoinvent-api-client-library-version": __version__,
-        } | self.custom_headers
+        }
+        headers.update(self.custom_headers)
         s3_link = requests.get(url, headers=headers, timeout=20).json()["download_url"]
         self._streaming_download(
             url=s3_link, params={}, directory=directory, filename=filename
         )
         return directory / filename
 
     def list_versions(self) -> list:
```

### Comparing `ecoinvent_interface-2.4.1/ecoinvent_interface/data/mappings.zip` & `ecoinvent_interface-2.5/ecoinvent_interface/data/mappings.zip`

 * *Files identical despite different names*

### Comparing `ecoinvent_interface-2.4.1/ecoinvent_interface/mapping.py` & `ecoinvent_interface-2.5/ecoinvent_interface/mapping.py`

 * *Files identical despite different names*

### Comparing `ecoinvent_interface-2.4.1/ecoinvent_interface/process_interface.py` & `ecoinvent_interface-2.5/ecoinvent_interface/process_interface.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import io
 import json
 import logging
 import zipfile
 from enum import Enum
 from functools import lru_cache
 from pathlib import Path
-from typing import Optional, Union
+from typing import Optional, Tuple, Union
 from urllib.parse import parse_qsl, urlparse
 
 import requests
 
 from . import __version__
 from .core import SYSTEM_MODELS, InterfaceBase, fresh_login
 
@@ -49,15 +49,15 @@
         if not hasattr(self, "dataset_id"):
             raise MissingProcess("Must call `.select_process()` first")
         return f(self, *args, **kwargs)
 
     return wrapper
 
 
-def split_url(url: str) -> tuple[str, dict]:
+def split_url(url: str) -> Tuple[str, dict]:
     """Split a URL with params into a base path and a params dict"""
     nt = urlparse(url)
     return nt.path, dict(parse_qsl(nt.query))
 
 
 class ProcessFileType(Enum):
     upr = "Unit Process"
@@ -144,15 +144,16 @@
     @selected_process
     @fresh_login
     def _json_request(self, url: str) -> Union[dict, list]:
         headers = {
             "Authorization": f"Bearer {self.access_token}",
             "ecoinvent-api-client-library": "ecoinvent_interface",
             "ecoinvent-api-client-library-version": __version__,
-        } | self.custom_headers
+        }
+        headers.update(self.custom_headers)
         message = """Requesting URL.
     URL: {url}
     Class: {self.__class__.__name__}
     Instance ID: {id(self)}
     Version: {__version__}
     User: {self.username}
         """
@@ -185,15 +186,16 @@
             available = list(files)
             raise KeyError(f"Can't find {file_type} in available options: {available}")
 
         headers = {
             "Authorization": f"Bearer {self.access_token}",
             "ecoinvent-api-client-library": "ecoinvent_interface",
             "ecoinvent-api-client-library-version": __version__,
-        } | self.custom_headers
+        }
+        headers.update(self.custom_headers)
         if meta.get("type").lower() == "xml":
             headers["Accept"] = "text/plain"
 
         url, params = split_url(meta["url"])
         suffix = meta["type"].lower()
         filename = (
             f"ecoinvent-{self.version}-{self.system_model}-{file_type.name}-"
```

### Comparing `ecoinvent_interface-2.4.1/ecoinvent_interface/release.py` & `ecoinvent_interface-2.5/ecoinvent_interface/release.py`

 * *Files identical despite different names*

### Comparing `ecoinvent_interface-2.4.1/ecoinvent_interface/settings.py` & `ecoinvent_interface-2.5/ecoinvent_interface/settings.py`

 * *Files identical despite different names*

### Comparing `ecoinvent_interface-2.4.1/ecoinvent_interface/spold_versions.py` & `ecoinvent_interface-2.5/ecoinvent_interface/spold_versions.py`

 * *Files identical despite different names*

### Comparing `ecoinvent_interface-2.4.1/ecoinvent_interface/storage.py` & `ecoinvent_interface-2.5/ecoinvent_interface/storage.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import hashlib
 import json
 import shutil
-from collections.abc import Iterable, MutableMapping
+from collections.abc import MutableMapping
 from pathlib import Path
-from typing import Union
+from typing import Iterable, Union
 
 import platformdirs
 
 base_dir = Path(
     platformdirs.user_data_dir(appname="EcoinventInterface", appauthor="pylca")
 )
 cache_dir_platformdirs = base_dir / "cache"
```

### Comparing `ecoinvent_interface-2.4.1/ecoinvent_interface/string_distance.py` & `ecoinvent_interface-2.5/ecoinvent_interface/string_distance.py`

 * *Files identical despite different names*

### Comparing `ecoinvent_interface-2.4.1/ecoinvent_interface.egg-info/PKG-INFO` & `ecoinvent_interface-2.5/ecoinvent_interface.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
-Name: ecoinvent-interface
-Version: 2.4.1
+Name: ecoinvent_interface
+Version: 2.5
 Summary: Unofficial client for interfacing with ecoinvent database
 Author-email:  Chris Mutel <cmutel@gmail.com>
 Maintainer-email:  Chris Mutel <cmutel@gmail.com>
 Project-URL: source, https://github.com/brightway-lca/ecoinvent_interface
 Project-URL: homepage, https://github.com/brightway-lca/ecoinvent_interface
 Project-URL: tracker, https://github.com/brightway-lca/ecoinvent_interface/issues
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering
-Requires-Python: >=3.9
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: lxml
 Requires-Dist: platformdirs
 Requires-Dist: py7zr
 Requires-Dist: pydantic-settings
 Requires-Dist: pyecospold
@@ -40,16 +40,16 @@
 
 # ecoinvent_interface
 
 [![PyPI](https://img.shields.io/pypi/v/ecoinvent_interface.svg)][pypi status]
 [![Status](https://img.shields.io/pypi/status/ecoinvent_interface.svg)][pypi status]
 [![Python Version](https://img.shields.io/pypi/pyversions/ecoinvent_interface)][pypi status]
 
-[pypi status]: https://pypi.org/project/bw_hestia_bridge/
-[tests]: https://github.com/brightway-lca/bw_hestia_bridge/actions?workflow=Tests
+[pypi status]: https://pypi.org/project/ecoinvent-interface/
+[tests]: https://github.com/brightway-lca/ecoinvent_interface/actions?workflow=Tests
 
 This is an **unofficial and unsupported** Python library to get ecoinvent data.
 
 # Quickstart
 
 ```python
 from ecoinvent_interface import Settings, EcoinventRelease, ReleaseType
```

### Comparing `ecoinvent_interface-2.4.1/ecoinvent_interface.egg-info/SOURCES.txt` & `ecoinvent_interface-2.5/ecoinvent_interface.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ecoinvent_interface-2.4.1/pyproject.toml` & `ecoinvent_interface-2.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     "Intended Audience :: Science/Research",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
     "Topic :: Scientific/Engineering",
 ]
-requires-python = ">=3.9"
+requires-python = ">=3.8"
 dependencies = [
     "lxml",
     "platformdirs",
     "py7zr",
     "pydantic-settings",
     "pyecospold",
     "requests",
```

### Comparing `ecoinvent_interface-2.4.1/tests/test_process_interface.py` & `ecoinvent_interface-2.5/tests/test_process_interface.py`

 * *Files identical despite different names*

### Comparing `ecoinvent_interface-2.4.1/tests/test_release.py` & `ecoinvent_interface-2.5/tests/test_release.py`

 * *Files identical despite different names*

### Comparing `ecoinvent_interface-2.4.1/tests/test_release_utils.py` & `ecoinvent_interface-2.5/tests/test_release_utils.py`

 * *Files identical despite different names*

### Comparing `ecoinvent_interface-2.4.1/tests/test_settings.py` & `ecoinvent_interface-2.5/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `ecoinvent_interface-2.4.1/tests/test_spold_versions.py` & `ecoinvent_interface-2.5/tests/test_spold_versions.py`

 * *Files identical despite different names*

