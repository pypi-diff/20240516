# Comparing `tmp/contact_magic-0.9.0.tar.gz` & `tmp/contact_magic-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "contact_magic-0.9.0.tar", max compression
+gzip compressed data, was "contact_magic-0.9.1.tar", max compression
```

## Comparing `contact_magic-0.9.0.tar` & `contact_magic-0.9.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.9.0/README.md
--rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.9.0/contact_magic/__init__.py
--rw-r--r--   0        0        0     1159 2023-08-22 12:56:45.237444 contact_magic-0.9.0/contact_magic/asyncio.py
--rw-r--r--   0        0        0     1681 2023-09-14 12:32:13.496265 contact_magic-0.9.0/contact_magic/callbacks.py
--rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.9.0/contact_magic/conf/__init__.py
--rw-r--r--   0        0        0     3123 2023-09-08 12:50:16.549742 contact_magic-0.9.0/contact_magic/conf/all_technology_categories.py
--rw-r--r--   0        0        0     6239 2024-02-01 15:48:16.500972 contact_magic-0.9.0/contact_magic/conf/settings.py
--rw-r--r--   0        0        0     3014 2024-02-28 12:50:02.257075 contact_magic-0.9.0/contact_magic/dict_utils.py
--rw-r--r--   0        0        0     5983 2024-02-28 14:27:47.669823 contact_magic-0.9.0/contact_magic/helpers.py
--rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.9.0/contact_magic/integrations/__init__.py
--rw-r--r--   0        0        0     4385 2024-02-28 13:48:55.201326 contact_magic-0.9.0/contact_magic/integrations/copyfactory.py
--rw-r--r--   0        0        0     3970 2024-03-29 18:32:54.934655 contact_magic-0.9.0/contact_magic/integrations/sales_scrapers.py
--rw-r--r--   0        0        0     2376 2023-09-08 13:51:24.244648 contact_magic-0.9.0/contact_magic/integrations/sheets.py
--rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.9.0/contact_magic/logger.py
--rw-r--r--   0        0        0    23010 2024-03-29 18:35:51.296394 contact_magic-0.9.0/contact_magic/models.py
--rw-r--r--   0        0        0     3079 2023-09-07 15:20:51.788409 contact_magic-0.9.0/contact_magic/preprocessors.py
--rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.9.0/contact_magic/scripts/__init__.py
--rw-r--r--   0        0        0     1806 2023-07-09 10:19:06.127936 contact_magic-0.9.0/contact_magic/scripts/agency.py
--rw-r--r--   0        0        0      688 2024-03-28 10:03:31.101902 contact_magic-0.9.0/contact_magic/scripts/default_scraper_options.py
--rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.9.0/contact_magic/scripts/logger.py
--rw-r--r--   0        0        0     9381 2024-03-28 13:19:07.385491 contact_magic-0.9.0/contact_magic/scripts/run_workflows.py
--rw-r--r--   0        0        0     3192 2024-03-28 10:06:51.662914 contact_magic-0.9.0/contact_magic/scripts/sync_scraper_options_to_workersheets.py
--rw-r--r--   0        0        0     2542 2023-08-25 10:25:45.448025 contact_magic-0.9.0/contact_magic/scripts/update_workflow_approval_metrics.py
--rw-r--r--   0        0        0     3032 2024-03-28 11:10:56.451674 contact_magic-0.9.0/contact_magic/utils.py
--rw-r--r--   0        0        0     1925 2024-04-02 18:45:32.335586 contact_magic-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0     4514 2023-06-09 23:55:24.983205 contact_magic-0.9.1/README.md
+-rw-r--r--   0        0        0      280 2023-06-11 21:59:22.389422 contact_magic-0.9.1/contact_magic/__init__.py
+-rw-r--r--   0        0        0     1159 2023-08-22 12:56:45.237444 contact_magic-0.9.1/contact_magic/asyncio.py
+-rw-r--r--   0        0        0     1681 2023-09-14 12:32:13.496265 contact_magic-0.9.1/contact_magic/callbacks.py
+-rw-r--r--   0        0        0       51 2023-06-10 00:10:37.013402 contact_magic-0.9.1/contact_magic/conf/__init__.py
+-rw-r--r--   0        0        0     3123 2023-09-08 12:50:16.549742 contact_magic-0.9.1/contact_magic/conf/all_technology_categories.py
+-rw-r--r--   0        0        0     6239 2024-02-01 15:48:16.500972 contact_magic-0.9.1/contact_magic/conf/settings.py
+-rw-r--r--   0        0        0     3014 2024-02-28 12:50:02.257075 contact_magic-0.9.1/contact_magic/dict_utils.py
+-rw-r--r--   0        0        0     5983 2024-05-16 11:11:22.178723 contact_magic-0.9.1/contact_magic/helpers.py
+-rw-r--r--   0        0        0      121 2023-06-07 09:00:51.259272 contact_magic-0.9.1/contact_magic/integrations/__init__.py
+-rw-r--r--   0        0        0     4671 2024-05-16 11:14:36.009276 contact_magic-0.9.1/contact_magic/integrations/copyfactory.py
+-rw-r--r--   0        0        0     3986 2024-05-16 11:15:29.761496 contact_magic-0.9.1/contact_magic/integrations/sales_scrapers.py
+-rw-r--r--   0        0        0     2376 2024-04-06 10:46:58.295568 contact_magic-0.9.1/contact_magic/integrations/sheets.py
+-rw-r--r--   0        0        0       65 2023-06-08 09:44:27.736870 contact_magic-0.9.1/contact_magic/logger.py
+-rw-r--r--   0        0        0    23080 2024-05-16 11:10:08.606548 contact_magic-0.9.1/contact_magic/models.py
+-rw-r--r--   0        0        0     3079 2023-09-07 15:20:51.788409 contact_magic-0.9.1/contact_magic/preprocessors.py
+-rw-r--r--   0        0        0        0 2023-06-09 17:35:50.408715 contact_magic-0.9.1/contact_magic/scripts/__init__.py
+-rw-r--r--   0        0        0     1806 2023-07-09 10:19:06.127936 contact_magic-0.9.1/contact_magic/scripts/agency.py
+-rw-r--r--   0        0        0      688 2024-03-28 10:03:31.101902 contact_magic-0.9.1/contact_magic/scripts/default_scraper_options.py
+-rw-r--r--   0        0        0       61 2023-06-08 09:10:28.353224 contact_magic-0.9.1/contact_magic/scripts/logger.py
+-rw-r--r--   0        0        0     9381 2024-05-16 11:05:25.989706 contact_magic-0.9.1/contact_magic/scripts/run_workflows.py
+-rw-r--r--   0        0        0     3192 2024-04-06 10:46:45.939145 contact_magic-0.9.1/contact_magic/scripts/sync_scraper_options_to_workersheets.py
+-rw-r--r--   0        0        0     2542 2023-08-25 10:25:45.448025 contact_magic-0.9.1/contact_magic/scripts/update_workflow_approval_metrics.py
+-rw-r--r--   0        0        0     3032 2024-03-28 11:10:56.451674 contact_magic-0.9.1/contact_magic/utils.py
+-rw-r--r--   0        0        0     1925 2024-05-16 11:15:11.619858 contact_magic-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     6284 1970-01-01 00:00:00.000000 contact_magic-0.9.1/PKG-INFO
```

### Comparing `contact_magic-0.9.0/README.md` & `contact_magic-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/contact_magic/asyncio.py` & `contact_magic-0.9.1/contact_magic/asyncio.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/contact_magic/callbacks.py` & `contact_magic-0.9.1/contact_magic/callbacks.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/contact_magic/conf/all_technology_categories.py` & `contact_magic-0.9.1/contact_magic/conf/all_technology_categories.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/contact_magic/conf/settings.py` & `contact_magic-0.9.1/contact_magic/conf/settings.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/contact_magic/dict_utils.py` & `contact_magic-0.9.1/contact_magic/dict_utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/contact_magic/helpers.py` & `contact_magic-0.9.1/contact_magic/helpers.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/contact_magic/integrations/copyfactory.py` & `contact_magic-0.9.1/contact_magic/integrations/copyfactory.py`

 * *Files 17% similar despite different names*

```diff
@@ -30,14 +30,15 @@
     if not SETTINGS.COPYFACTORY_API_KEY:
         return None
     headers = {
         "Accept": "application/json",
         "Authorization": SETTINGS.COPYFACTORY_API_KEY,
     }
     variable_data = get_first_level_items(variables)
+    variable_data = {k.replace("df.", "").strip(): v for k, v in variable_data.items()}
     data = {
         "premise_id": premise_id,
         "variables": variable_data,
     }
     try:
         async with httpx.AsyncClient(timeout=httpx.Timeout(DEFAULT_TIMEOUT)) as session:
             retries = 0
@@ -69,14 +70,18 @@
                             if item := list(
                                 get_values_in_object_by_key(variables, req_var)
                             ):
                                 if item[0]:
                                     data["variables"][req_var] = str(item[0])
                         if not data["variables"].get("company_organization_name"):
                             data["variables"]["company_organization_name"] = ""
+                        data["variables"] = {
+                            k.replace("df.", "").strip(): v
+                            for k, v in data["variables"].items()
+                        }
 
                 retries += 1
         return None
     except Exception:
         return None
```

### Comparing `contact_magic-0.9.0/contact_magic/integrations/sales_scrapers.py` & `contact_magic-0.9.1/contact_magic/integrations/sales_scrapers.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 
 base_url = "https://datafactory.run/api/"
 
 
 async def make_sales_scraper_request(endpoint, data: dict, max_retries=3):
     if not SETTINGS.SALES_SCRAPERS_API_KEY:
         return None
+    return None
     headers = {
         "Accept": "application/json",
         "X-API-Key": SETTINGS.SALES_SCRAPERS_API_KEY,
     }
 
     url = f"{base_url}{endpoint}"
     try:
```

### Comparing `contact_magic-0.9.0/contact_magic/integrations/sheets.py` & `contact_magic-0.9.1/contact_magic/integrations/sheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/contact_magic/models.py` & `contact_magic-0.9.1/contact_magic/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -338,14 +338,16 @@
     )
     sentence_wizards: list[SentenceWizard]
     keys_added: set = set()
     successful_scraper_name: str = ""
 
     @property
     def has_successful_sentence(self):
+        if not self.successful_scraper_name:
+            return False
         return len(self.successful_scraper_name) > 0
 
     @property
     def get_col_name_as_source(self) -> str:
         return f"source__{self.col_name}"
 
     async def build_datapoint(
```

### Comparing `contact_magic-0.9.0/contact_magic/preprocessors.py` & `contact_magic-0.9.1/contact_magic/preprocessors.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/contact_magic/scripts/agency.py` & `contact_magic-0.9.1/contact_magic/scripts/agency.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/contact_magic/scripts/default_scraper_options.py` & `contact_magic-0.9.1/contact_magic/scripts/default_scraper_options.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/contact_magic/scripts/run_workflows.py` & `contact_magic-0.9.1/contact_magic/scripts/run_workflows.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/contact_magic/scripts/sync_scraper_options_to_workersheets.py` & `contact_magic-0.9.1/contact_magic/scripts/sync_scraper_options_to_workersheets.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/contact_magic/scripts/update_workflow_approval_metrics.py` & `contact_magic-0.9.1/contact_magic/scripts/update_workflow_approval_metrics.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/contact_magic/utils.py` & `contact_magic-0.9.1/contact_magic/utils.py`

 * *Files identical despite different names*

### Comparing `contact_magic-0.9.0/pyproject.toml` & `contact_magic-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "contact-magic"
-version = "0.9.0"
+version = "0.9.1"
 description = "Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point."
 authors = ["Copyfactory <dev@copyfactory.io>"]
 readme = "README.md"
 packages = [
     { include = "contact_magic"}
 ]
 license = "MIT"
```

### Comparing `contact_magic-0.9.0/PKG-INFO` & `contact_magic-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: contact-magic
-Version: 0.9.0
+Version: 0.9.1
 Summary: Quickly set up workflows for retrieving hard-to-find contact information and composing personalized messages based on any data point.
 License: MIT
 Author: Copyfactory
 Author-email: dev@copyfactory.io
 Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Web Environment
```

