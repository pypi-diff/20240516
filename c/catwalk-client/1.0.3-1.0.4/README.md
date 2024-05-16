# Comparing `tmp/catwalk_client-1.0.3.tar.gz` & `tmp/catwalk_client-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "catwalk_client-1.0.3.tar", last modified: Mon Sep 25 14:11:49 2023, max compression
+gzip compressed data, was "catwalk_client-1.0.4.tar", last modified: Thu May 16 11:57:37 2024, max compression
```

## Comparing `catwalk_client-1.0.3.tar` & `catwalk_client-1.0.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwxr-x   0 marek     (1001) marek     (1001)        0 2023-09-25 14:11:49.146444 catwalk_client-1.0.3/
--rw-r--r--   0 marek     (1001) marek     (1001)     6848 2023-09-25 14:11:49.142444 catwalk_client-1.0.3/PKG-INFO
--rw-rw-r--   0 marek     (1001) marek     (1001)     6457 2023-09-25 14:10:29.000000 catwalk_client-1.0.3/README.md
-drwxrwxr-x   0 marek     (1001) marek     (1001)        0 2023-09-25 14:11:49.118443 catwalk_client-1.0.3/catwalk_client/
--rw-rw-r--   0 marek     (1001) marek     (1001)       34 2023-09-12 20:02:45.000000 catwalk_client-1.0.3/catwalk_client/__init__.py
--rw-rw-r--   0 marek     (1001) marek     (1001)    16350 2023-09-25 14:10:29.000000 catwalk_client-1.0.3/catwalk_client/client.py
-drwxrwxr-x   0 marek     (1001) marek     (1001)        0 2023-09-25 14:11:49.134444 catwalk_client-1.0.3/catwalk_client/common/
--rw-rw-r--   0 marek     (1001) marek     (1001)       51 2023-09-12 20:02:45.000000 catwalk_client-1.0.3/catwalk_client/common/__init__.py
--rw-rw-r--   0 marek     (1001) marek     (1001)    10039 2023-09-25 14:10:29.000000 catwalk_client-1.0.3/catwalk_client/common/_http_client.py
--rw-rw-r--   0 marek     (1001) marek     (1001)     1040 2023-09-25 14:10:29.000000 catwalk_client-1.0.3/catwalk_client/common/_session.py
--rw-rw-r--   0 marek     (1001) marek     (1001)     3145 2023-09-22 12:08:07.000000 catwalk_client-1.0.3/catwalk_client/common/catwalk_http_client.py
--rw-rw-r--   0 marek     (1001) marek     (1001)      814 2023-09-25 14:10:29.000000 catwalk_client-1.0.3/catwalk_client/common/constants.py
--rw-rw-r--   0 marek     (1001) marek     (1001)      355 2023-09-25 14:10:29.000000 catwalk_client-1.0.3/catwalk_client/common/exception.py
--rw-rw-r--   0 marek     (1001) marek     (1001)     1651 2023-09-25 14:10:29.000000 catwalk_client-1.0.3/catwalk_client/common/logger.py
-drwxrwxr-x   0 marek     (1001) marek     (1001)        0 2023-09-25 14:11:49.138444 catwalk_client-1.0.3/catwalk_client/tools/
--rw-rw-r--   0 marek     (1001) marek     (1001)      154 2023-09-12 20:02:45.000000 catwalk_client-1.0.3/catwalk_client/tools/__init__.py
--rw-rw-r--   0 marek     (1001) marek     (1001)     1675 2023-09-22 12:08:07.000000 catwalk_client-1.0.3/catwalk_client/tools/_case_builder.py
--rw-rw-r--   0 marek     (1001) marek     (1001)     3320 2023-09-25 14:10:29.000000 catwalk_client-1.0.3/catwalk_client/tools/_case_exporter.py
--rw-rw-r--   0 marek     (1001) marek     (1001)     5675 2023-09-25 14:10:29.000000 catwalk_client-1.0.3/catwalk_client/tools/_case_exporter_v2.py
-drwxrwxr-x   0 marek     (1001) marek     (1001)        0 2023-09-25 14:11:49.126443 catwalk_client-1.0.3/catwalk_client.egg-info/
--rw-r--r--   0 marek     (1001) marek     (1001)     6848 2023-09-25 14:11:49.000000 catwalk_client-1.0.3/catwalk_client.egg-info/PKG-INFO
--rw-rw-r--   0 marek     (1001) marek     (1001)      670 2023-09-25 14:11:49.000000 catwalk_client-1.0.3/catwalk_client.egg-info/SOURCES.txt
--rw-rw-r--   0 marek     (1001) marek     (1001)        1 2023-09-25 14:11:49.000000 catwalk_client-1.0.3/catwalk_client.egg-info/dependency_links.txt
--rw-rw-r--   0 marek     (1001) marek     (1001)       22 2023-09-25 14:11:49.000000 catwalk_client-1.0.3/catwalk_client.egg-info/requires.txt
--rw-rw-r--   0 marek     (1001) marek     (1001)       15 2023-09-25 14:11:49.000000 catwalk_client-1.0.3/catwalk_client.egg-info/top_level.txt
--rw-rw-r--   0 marek     (1001) marek     (1001)      442 2023-09-25 14:10:29.000000 catwalk_client-1.0.3/pyproject.toml
--rw-rw-r--   0 marek     (1001) marek     (1001)       38 2023-09-25 14:11:49.146444 catwalk_client-1.0.3/setup.cfg
+drwxr-xr-x   0 thokik    (1000) thokik    (1000)        0 2024-05-16 11:57:37.864432 catwalk_client-1.0.4/
+-rw-r--r--   0 thokik    (1000) thokik    (1000)     6882 2024-05-16 11:57:37.864432 catwalk_client-1.0.4/PKG-INFO
+-rw-r--r--   0 thokik    (1000) thokik    (1000)     6457 2024-05-14 13:09:32.000000 catwalk_client-1.0.4/README.md
+drwxr-xr-x   0 thokik    (1000) thokik    (1000)        0 2024-05-16 11:57:37.864432 catwalk_client-1.0.4/catwalk_client/
+-rw-r--r--   0 thokik    (1000) thokik    (1000)       34 2024-05-14 13:09:32.000000 catwalk_client-1.0.4/catwalk_client/__init__.py
+-rw-r--r--   0 thokik    (1000) thokik    (1000)    16367 2024-05-15 12:56:30.000000 catwalk_client-1.0.4/catwalk_client/client.py
+drwxr-xr-x   0 thokik    (1000) thokik    (1000)        0 2024-05-16 11:57:37.864432 catwalk_client-1.0.4/catwalk_client/common/
+-rw-r--r--   0 thokik    (1000) thokik    (1000)       51 2024-05-14 13:09:32.000000 catwalk_client-1.0.4/catwalk_client/common/__init__.py
+-rw-r--r--   0 thokik    (1000) thokik    (1000)    10039 2024-05-14 13:09:32.000000 catwalk_client-1.0.4/catwalk_client/common/_http_client.py
+-rw-r--r--   0 thokik    (1000) thokik    (1000)     1040 2024-05-14 13:09:32.000000 catwalk_client-1.0.4/catwalk_client/common/_session.py
+-rw-r--r--   0 thokik    (1000) thokik    (1000)     3145 2024-05-14 13:09:32.000000 catwalk_client-1.0.4/catwalk_client/common/catwalk_http_client.py
+-rw-r--r--   0 thokik    (1000) thokik    (1000)      814 2024-05-14 13:09:32.000000 catwalk_client-1.0.4/catwalk_client/common/constants.py
+-rw-r--r--   0 thokik    (1000) thokik    (1000)      355 2024-05-14 13:09:32.000000 catwalk_client-1.0.4/catwalk_client/common/exception.py
+-rw-r--r--   0 thokik    (1000) thokik    (1000)     1651 2024-05-14 13:09:32.000000 catwalk_client-1.0.4/catwalk_client/common/logger.py
+drwxr-xr-x   0 thokik    (1000) thokik    (1000)        0 2024-05-16 11:57:37.864432 catwalk_client-1.0.4/catwalk_client/tools/
+-rw-r--r--   0 thokik    (1000) thokik    (1000)      154 2024-05-14 13:09:32.000000 catwalk_client-1.0.4/catwalk_client/tools/__init__.py
+-rw-r--r--   0 thokik    (1000) thokik    (1000)     1675 2024-05-14 13:09:32.000000 catwalk_client-1.0.4/catwalk_client/tools/_case_builder.py
+-rw-r--r--   0 thokik    (1000) thokik    (1000)     3318 2024-05-15 12:56:30.000000 catwalk_client-1.0.4/catwalk_client/tools/_case_exporter.py
+-rw-r--r--   0 thokik    (1000) thokik    (1000)     5769 2024-05-15 12:56:30.000000 catwalk_client-1.0.4/catwalk_client/tools/_case_exporter_v2.py
+drwxr-xr-x   0 thokik    (1000) thokik    (1000)        0 2024-05-16 11:57:37.864432 catwalk_client-1.0.4/catwalk_client.egg-info/
+-rw-r--r--   0 thokik    (1000) thokik    (1000)     6882 2024-05-16 11:57:37.000000 catwalk_client-1.0.4/catwalk_client.egg-info/PKG-INFO
+-rw-r--r--   0 thokik    (1000) thokik    (1000)      670 2024-05-16 11:57:37.000000 catwalk_client-1.0.4/catwalk_client.egg-info/SOURCES.txt
+-rw-r--r--   0 thokik    (1000) thokik    (1000)        1 2024-05-16 11:57:37.000000 catwalk_client-1.0.4/catwalk_client.egg-info/dependency_links.txt
+-rw-r--r--   0 thokik    (1000) thokik    (1000)       22 2024-05-16 11:57:37.000000 catwalk_client-1.0.4/catwalk_client.egg-info/requires.txt
+-rw-r--r--   0 thokik    (1000) thokik    (1000)       15 2024-05-16 11:57:37.000000 catwalk_client-1.0.4/catwalk_client.egg-info/top_level.txt
+-rw-r--r--   0 thokik    (1000) thokik    (1000)      502 2024-05-16 11:55:17.000000 catwalk_client-1.0.4/pyproject.toml
+-rw-r--r--   0 thokik    (1000) thokik    (1000)       38 2024-05-16 11:57:37.864432 catwalk_client-1.0.4/setup.cfg
```

### Comparing `catwalk_client-1.0.3/PKG-INFO` & `catwalk_client-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: catwalk_client
-Version: 1.0.3
+Version: 1.0.4
 Summary: Client for Catwalk
-Author-email: Marek Połom <marek.polom@deepsense.ai>, Mateusz Hordyński <mateusz.hordynski@deepsense.ai>
+Author-email: Marek Połom <marek.polom@deepsense.ai>, Mateusz Hordyński <mateusz.hordynski@deepsense.ai>, Thor Kikkenborg <thokik@erst.dk>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: catwalk_common>=0.0.7
 
 # Catwalk Client
```

### Comparing `catwalk_client-1.0.3/README.md` & `catwalk_client-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `catwalk_client-1.0.3/catwalk_client/client.py` & `catwalk_client-1.0.4/catwalk_client/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -134,15 +134,15 @@
     def export_cases(
         self,
         from_datetime: datetime,
         to_datetime: datetime,
         submitter_name: str | None = None,
         submitter_version: str | None = None,
         max_retries: int = 5,
-        limit: int | None = None,
+        limit: int | None = 100,
     ):
         exporter = CaseExporter(
             http_client=self.http_client,
             from_datetime=from_datetime,
             to_datetime=to_datetime,
             submitter_name=submitter_name or self.submitter_name,
             submitter_version=submitter_version or self.submitter_version,
@@ -155,29 +155,29 @@
         self,
         submitter_name: str | None = None,
         submitter_version: str | None = None,
         datetime_from: datetime | None = None,
         datetime_to: datetime = datetime.now(),
         sort_by: list[str] | str | None = None,
         sort_order: list[SORT_ORDER] | SORT_ORDER = "desc",
-        limit: int = 100,
+        limit: int | None = 100,
         offset: int = 0,
         max_retries: int = 5,
     ):
         """Export cases using the v2 export endpoint.
 
         Args:
             submitter_name (Optional[str], optional): Name of submitter to export. Defaults to None.
             submitter_version (Optional[str], optional): Version of submitter to export. Defaults to None.
             datetime_from (Optional[datetime], optional): Lower boundary of case creation date. Defaults to None.
             datetime_to (datetime, optional): Upper boundary of case creation date. Defaults to current time.
             sort_by (Union[list[str], str, None], optional): Field(s) by which exported cases will be ordered. Defaults to None.
             sort_order (Union[list[SORT_ORDER], SORT_ORDER], optional): Order(s) by which exported cases will be ordered. Defaults to "desc".
             limit (int, optional): Size limit of a single batch fetched from the API (not overall limit).
-                                   Defaults to 100. Max is 1000, if the limit is higher than 1000 the API will return an error.
+                                   Defaults to 100. Must be a positive integer if not None. If a maximum limit is set, limit must obey it.
             offset (int, optional): Starting offset of fetched data. Defaults to 0.
             max_retries (int, optional): Maximum number of retries in case the request does not succeed. Defaults to 5.
 
         Yields:
             OpenCase: Cases returned by the API.
         """
         exporter = CaseExporterV2(
```

### Comparing `catwalk_client-1.0.3/catwalk_client/common/_http_client.py` & `catwalk_client-1.0.4/catwalk_client/common/_http_client.py`

 * *Files identical despite different names*

### Comparing `catwalk_client-1.0.3/catwalk_client/common/_session.py` & `catwalk_client-1.0.4/catwalk_client/common/_session.py`

 * *Files identical despite different names*

### Comparing `catwalk_client-1.0.3/catwalk_client/common/catwalk_http_client.py` & `catwalk_client-1.0.4/catwalk_client/common/catwalk_http_client.py`

 * *Files identical despite different names*

### Comparing `catwalk_client-1.0.3/catwalk_client/common/constants.py` & `catwalk_client-1.0.4/catwalk_client/common/constants.py`

 * *Files identical despite different names*

### Comparing `catwalk_client-1.0.3/catwalk_client/common/logger.py` & `catwalk_client-1.0.4/catwalk_client/common/logger.py`

 * *Files identical despite different names*

### Comparing `catwalk_client-1.0.3/catwalk_client/tools/_case_builder.py` & `catwalk_client-1.0.4/catwalk_client/tools/_case_builder.py`

 * *Files identical despite different names*

### Comparing `catwalk_client-1.0.3/catwalk_client/tools/_case_exporter.py` & `catwalk_client-1.0.4/catwalk_client/tools/_case_exporter.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
         http_client: CatwalkHTTPClient,
         from_datetime: datetime,
         to_datetime: datetime,
         submitter_name: str | None = None,
         submitter_version: str | None = None,
         max_retries: int = 5,
         batch: int = 1,
-        limit: int | None = None,
+        limit: int | None = 100,
     ):
         self.http_client = http_client
 
         self.from_datetime = from_datetime
         self.to_datetime = to_datetime
 
         self.filters = self._build_filters(
@@ -79,15 +79,15 @@
 
     @staticmethod
     def _build_filters(
         submitter_name: str,
         submitter_version: str,
         from_datetime: datetime,
         to_datetime: datetime,
-        limit: int | None = None,
+        limit: int | None = 100,
     ):
         filters = {
             "submitter_name": submitter_name,
             "submitter_version": submitter_version,
             "from_timestamp": from_datetime.isoformat(),
             "to_timestamp": to_datetime.isoformat(),
             "limit": limit,
```

### Comparing `catwalk_client-1.0.3/catwalk_client/tools/_case_exporter_v2.py` & `catwalk_client-1.0.4/catwalk_client/tools/_case_exporter_v2.py`

 * *Files 3% similar despite different names*

```diff
@@ -22,29 +22,29 @@
         http_client: CatwalkHTTPClient,
         submitter_name: str | None = None,
         submitter_version: str | None = None,
         datetime_from: datetime | None = None,
         datetime_to: datetime = datetime.now(),
         sort_by: list[str] | str | None = None,
         sort_order: list[SORT_ORDER] | SORT_ORDER = "desc",
-        limit: int = 100,
+        limit: int | None = 100,
         offset: int = 0,
         max_retries: int = 5,
     ):
         """Create CaseExporter object (EXPORT V2).
 
         Args:
             submitter_name (Optional[str], optional): Name of submitter to export. Defaults to None.
             submitter_version (Optional[str], optional): Version of submitter to export. Defaults to None.
             datetime_from (Optional[datetime], optional): Lower boundary of case creation date. Defaults to None.
             datetime_to (datetime, optional): Upper boundary of case creation date. Defaults to current time.
             sort_by (Union[list[str], str, None], optional): Field(s) by which exported cases will be ordered. Defaults to None.
             sort_order (Union[list[SORT_ORDER], SORT_ORDER], optional): Order(s) by which exported cases will be ordered. Defaults to "desc".
             limit (int, optional): Limit of a single batch fetched from the API (not overall limit).
-                                   Defaults to 100. Max is 1000, if the limit is higher than 1000 the API will return an error.
+                                   Defaults to 100. Must be a postitive integer if not None. If a maximum limit is set, limit must obey it.
             offset (int, optional): Starting offset of fetched data. Defaults to 0.
             max_retries (int, optional): Maximum number of retries in case the request does not succeed. Defaults to 5.
         """
         self.path = "/api/v2/cases/export"
         self.http_client = http_client
         self.max_retries = max_retries
 
@@ -79,15 +79,18 @@
 
             current_retry = 0
             data = loads(response)
 
             for case in data["cases"]:
                 yield OpenCase.parse_obj(case)
 
-            if len(data["cases"]) < self.limit:
+            if self.limit:
+                if len(data["cases"]) < self.limit:
+                    break
+            else:
                 break
 
             self.offset += self.limit
 
     def _handle_retry(self, retry: int, response: str):
         """Check if the unsuccessful call can be retried and apply delay to the next call.
```

### Comparing `catwalk_client-1.0.3/catwalk_client.egg-info/PKG-INFO` & `catwalk_client-1.0.4/catwalk_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
-Name: catwalk-client
-Version: 1.0.3
+Name: catwalk_client
+Version: 1.0.4
 Summary: Client for Catwalk
-Author-email: Marek Połom <marek.polom@deepsense.ai>, Mateusz Hordyński <mateusz.hordynski@deepsense.ai>
+Author-email: Marek Połom <marek.polom@deepsense.ai>, Mateusz Hordyński <mateusz.hordynski@deepsense.ai>, Thor Kikkenborg <thokik@erst.dk>
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8.0
 Description-Content-Type: text/markdown
 Requires-Dist: catwalk_common>=0.0.7
 
 # Catwalk Client
```

### Comparing `catwalk_client-1.0.3/catwalk_client.egg-info/SOURCES.txt` & `catwalk_client-1.0.4/catwalk_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

