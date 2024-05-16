# Comparing `tmp/perian_cli-0.0.26.tar.gz` & `tmp/perian_cli-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perian_cli-0.0.26.tar", max compression
+gzip compressed data, was "perian_cli-0.1.1.tar", max compression
```

## Comparing `perian_cli-0.0.26.tar` & `perian_cli-0.1.1.tar`

### file list

```diff
@@ -1,28 +1,29 @@
--rw-r--r--   0        0        0     1220 2024-05-02 07:42:40.320695 perian_cli-0.0.26/pcli/__init__.py
--rw-r--r--   0        0        0        0 2024-05-02 07:42:40.320764 perian_cli-0.0.26/pcli/api/__init__.py
--rw-r--r--   0        0        0     3607 2024-05-02 07:42:40.320850 perian_cli-0.0.26/pcli/api/accelerator_type.py
--rw-r--r--   0        0        0     1452 2024-05-02 07:42:40.320918 perian_cli-0.0.26/pcli/api/billing.py
--rw-r--r--   0        0        0     3200 2024-05-02 07:42:40.320995 perian_cli-0.0.26/pcli/api/instance_type.py
--rw-r--r--   0        0        0     3670 2024-05-08 19:41:47.993678 perian_cli-0.0.26/pcli/api/job.py
--rw-r--r--   0        0        0     1020 2024-05-08 19:38:12.714322 perian_cli-0.0.26/pcli/api/organization.py
--rw-r--r--   0        0        0     4950 2024-05-07 11:53:55.387135 perian_cli-0.0.26/pcli/cli.py
--rw-r--r--   0        0        0      133 2024-05-02 07:42:40.321188 perian_cli-0.0.26/pcli/colors.py
--rw-r--r--   0        0        0        0 2024-05-02 07:42:40.321250 perian_cli-0.0.26/pcli/commands/__init__.py
--rw-r--r--   0        0        0     3036 2024-05-02 07:42:40.321328 perian_cli-0.0.26/pcli/commands/accelerator_type.py
--rw-r--r--   0        0        0     1846 2024-05-02 07:42:40.321388 perian_cli-0.0.26/pcli/commands/billing.py
--rw-r--r--   0        0        0      344 2024-05-02 07:42:40.321449 perian_cli-0.0.26/pcli/commands/config.py
--rw-r--r--   0        0        0      898 2024-05-02 07:42:40.321513 perian_cli-0.0.26/pcli/commands/currency.py
--rw-r--r--   0        0        0     3526 2024-05-02 07:42:40.321588 perian_cli-0.0.26/pcli/commands/instance_type.py
--rw-r--r--   0        0        0     9529 2024-05-14 12:34:40.416195 perian_cli-0.0.26/pcli/commands/job.py
--rw-r--r--   0        0        0     4523 2024-05-07 11:53:55.388603 perian_cli-0.0.26/pcli/commands/registry.py
--rw-r--r--   0        0        0     5756 2024-05-08 19:41:47.994564 perian_cli-0.0.26/pcli/responses.py
--rw-r--r--   0        0        0      446 2024-05-07 14:19:49.243150 perian_cli-0.0.26/pcli/settings.py
--rw-r--r--   0        0        0     4452 2024-05-07 11:53:55.389921 perian_cli-0.0.26/pcli/util/__init__.py
--rw-r--r--   0        0        0     3688 2024-05-02 07:42:40.322636 perian_cli-0.0.26/pcli/util/currencies.py
--rw-r--r--   0        0        0     1086 2024-05-02 07:42:40.322715 perian_cli-0.0.26/pcli/util/db.py
--rw-r--r--   0        0        0    18983 2024-05-15 13:00:01.635606 perian_cli-0.0.26/pcli/util/formatter.py
--rw-r--r--   0        0        0      566 2024-05-02 07:42:40.322935 perian_cli-0.0.26/pcli/util/organization.py
--rw-r--r--   0        0        0    24293 2024-05-02 07:42:40.323042 perian_cli-0.0.26/pcli/util/rich_utils.py
--rw-r--r--   0        0        0     1185 2024-05-07 11:53:55.390884 perian_cli-0.0.26/pcli/util/setup.py
--rw-r--r--   0        0        0      635 2024-05-02 07:42:40.323434 perian_cli-0.0.26/pyproject.toml
--rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 perian_cli-0.0.26/PKG-INFO
+-rw-r--r--   0        0        0      238 2024-05-16 08:33:28.069526 perian_cli-0.1.1/README.md
+-rw-r--r--   0        0        0     1220 2024-05-02 07:42:40.320695 perian_cli-0.1.1/pcli/__init__.py
+-rw-r--r--   0        0        0        0 2024-05-02 07:42:40.320764 perian_cli-0.1.1/pcli/api/__init__.py
+-rw-r--r--   0        0        0     3607 2024-05-02 07:42:40.320850 perian_cli-0.1.1/pcli/api/accelerator_type.py
+-rw-r--r--   0        0        0     1452 2024-05-02 07:42:40.320918 perian_cli-0.1.1/pcli/api/billing.py
+-rw-r--r--   0        0        0     3200 2024-05-02 07:42:40.320995 perian_cli-0.1.1/pcli/api/instance_type.py
+-rw-r--r--   0        0        0     3670 2024-05-08 19:41:47.993678 perian_cli-0.1.1/pcli/api/job.py
+-rw-r--r--   0        0        0     1020 2024-05-08 19:38:12.714322 perian_cli-0.1.1/pcli/api/organization.py
+-rw-r--r--   0        0        0     4950 2024-05-07 11:53:55.387135 perian_cli-0.1.1/pcli/cli.py
+-rw-r--r--   0        0        0      133 2024-05-02 07:42:40.321188 perian_cli-0.1.1/pcli/colors.py
+-rw-r--r--   0        0        0        0 2024-05-02 07:42:40.321250 perian_cli-0.1.1/pcli/commands/__init__.py
+-rw-r--r--   0        0        0     3036 2024-05-02 07:42:40.321328 perian_cli-0.1.1/pcli/commands/accelerator_type.py
+-rw-r--r--   0        0        0     1846 2024-05-02 07:42:40.321388 perian_cli-0.1.1/pcli/commands/billing.py
+-rw-r--r--   0        0        0      344 2024-05-02 07:42:40.321449 perian_cli-0.1.1/pcli/commands/config.py
+-rw-r--r--   0        0        0      898 2024-05-02 07:42:40.321513 perian_cli-0.1.1/pcli/commands/currency.py
+-rw-r--r--   0        0        0     3526 2024-05-02 07:42:40.321588 perian_cli-0.1.1/pcli/commands/instance_type.py
+-rw-r--r--   0        0        0     9529 2024-05-16 06:57:29.587333 perian_cli-0.1.1/pcli/commands/job.py
+-rw-r--r--   0        0        0     4523 2024-05-07 11:53:55.388603 perian_cli-0.1.1/pcli/commands/registry.py
+-rw-r--r--   0        0        0     5756 2024-05-08 19:41:47.994564 perian_cli-0.1.1/pcli/responses.py
+-rw-r--r--   0        0        0      446 2024-05-07 14:19:49.243150 perian_cli-0.1.1/pcli/settings.py
+-rw-r--r--   0        0        0     4452 2024-05-07 11:53:55.389921 perian_cli-0.1.1/pcli/util/__init__.py
+-rw-r--r--   0        0        0     3688 2024-05-02 07:42:40.322636 perian_cli-0.1.1/pcli/util/currencies.py
+-rw-r--r--   0        0        0     1086 2024-05-02 07:42:40.322715 perian_cli-0.1.1/pcli/util/db.py
+-rw-r--r--   0        0        0    18983 2024-05-15 13:00:01.635606 perian_cli-0.1.1/pcli/util/formatter.py
+-rw-r--r--   0        0        0      566 2024-05-02 07:42:40.322935 perian_cli-0.1.1/pcli/util/organization.py
+-rw-r--r--   0        0        0    24293 2024-05-02 07:42:40.323042 perian_cli-0.1.1/pcli/util/rich_utils.py
+-rw-r--r--   0        0        0     1185 2024-05-07 11:53:55.390884 perian_cli-0.1.1/pcli/util/setup.py
+-rw-r--r--   0        0        0      654 2024-05-16 08:38:36.522919 perian_cli-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 perian_cli-0.1.1/PKG-INFO
```

### Comparing `perian_cli-0.0.26/pcli/__init__.py` & `perian_cli-0.1.1/pcli/__init__.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/api/accelerator_type.py` & `perian_cli-0.1.1/pcli/api/accelerator_type.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/api/billing.py` & `perian_cli-0.1.1/pcli/api/billing.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/api/instance_type.py` & `perian_cli-0.1.1/pcli/api/instance_type.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/api/job.py` & `perian_cli-0.1.1/pcli/api/job.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/api/organization.py` & `perian_cli-0.1.1/pcli/api/organization.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/cli.py` & `perian_cli-0.1.1/pcli/cli.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/commands/accelerator_type.py` & `perian_cli-0.1.1/pcli/commands/accelerator_type.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/commands/billing.py` & `perian_cli-0.1.1/pcli/commands/billing.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/commands/currency.py` & `perian_cli-0.1.1/pcli/commands/currency.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/commands/instance_type.py` & `perian_cli-0.1.1/pcli/commands/instance_type.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/commands/job.py` & `perian_cli-0.1.1/pcli/commands/job.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     InvalidJobManifestException,
     InvalidParametersException,
     InvalidInstanceTypeIdException,
     InsufficientQuotaException
 )
 from pcli.util import load_instance_type_filter_from_values, load_job_manifest_from_json
 from pcli.util.formatter import print_jobs_list, print_job_description, format_instance_type_query
-from perian import InstanceTypeQueryInput, CreateJobRequest
+from perian import InstanceTyperQueryView, CreateJobRequest
 from pcli import db
 from urllib.parse import urlparse
 from perian.models import DockerRegistryCredentials
 
 job_command = PerianTyper(
     no_args_is_help=True,
     rich_markup_mode="rich",
@@ -136,15 +136,15 @@
 
             # no specific instance type id, we need to find a suitable one first
             else:
                 selecting_instance_type_task = progress.add_task(description="Selecting optimal instance type",
                                                                  total=None)
 
                 # creating instance type query
-                instance_type_query = InstanceTypeQueryInput(**instance_type_filters)
+                instance_type_query = InstanceTyperQueryView(**instance_type_filters)
                 instance_types = get_instance_type_by_requirements(instance_type_query, 1)
                 job_description['instance_type_id'] = instance_types[0].id
 
                 # this is just for the user experience and the progress spinner
                 time.sleep(0.3)
                 progress.remove_task(selecting_instance_type_task)
```

### Comparing `perian_cli-0.0.26/pcli/commands/registry.py` & `perian_cli-0.1.1/pcli/commands/registry.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/responses.py` & `perian_cli-0.1.1/pcli/responses.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/util/__init__.py` & `perian_cli-0.1.1/pcli/util/__init__.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/util/currencies.py` & `perian_cli-0.1.1/pcli/util/currencies.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/util/db.py` & `perian_cli-0.1.1/pcli/util/db.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/util/formatter.py` & `perian_cli-0.1.1/pcli/util/formatter.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/util/organization.py` & `perian_cli-0.1.1/pcli/util/organization.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/util/rich_utils.py` & `perian_cli-0.1.1/pcli/util/rich_utils.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pcli/util/setup.py` & `perian_cli-0.1.1/pcli/util/setup.py`

 * *Files identical despite different names*

### Comparing `perian_cli-0.0.26/pyproject.toml` & `perian_cli-0.1.1/pyproject.toml`

 * *Files 26% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [tool.poetry]
 name = "perian-cli"
-version = "0.0.26"
+version = "0.1.1"
 description = "Perian Sky Platform CLI"
 authors = ["Perian <info@perian.io>"]
 homepage = "https://perian.io"
 documentation = "https://perian.io"
 packages = [{include = "pcli"}]
+readme = "README.md"
 
 [tool.poetry.scripts]
 perian = "pcli.cli:pcli"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 typer = "0.12.3"
 validators = "0.28.1"
 pydantic = "2.7.0"
 click = "8.1.7"
 rich = "13.7.1"
 toml = "0.10.2"
-perian = "0.1.25"
+perian = "0.2.0"
 requests = "2.31.0"
 pydantic-settings = "2.2.1"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
```

### Comparing `perian_cli-0.0.26/PKG-INFO` & `perian_cli-0.1.1/PKG-INFO`

 * *Files 27% similar despite different names*

```diff
@@ -1,22 +1,32 @@
 Metadata-Version: 2.1
 Name: perian-cli
-Version: 0.0.26
+Version: 0.1.1
 Summary: Perian Sky Platform CLI
 Home-page: https://perian.io
 Author: Perian
 Author-email: info@perian.io
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: click (==8.1.7)
-Requires-Dist: perian (==0.1.25)
+Requires-Dist: perian (==0.2.0)
 Requires-Dist: pydantic (==2.7.0)
 Requires-Dist: pydantic-settings (==2.2.1)
 Requires-Dist: requests (==2.31.0)
 Requires-Dist: rich (==13.7.1)
 Requires-Dist: toml (==0.10.2)
 Requires-Dist: typer (==0.12.3)
 Requires-Dist: validators (==0.28.1)
 Project-URL: Documentation, https://perian.io
+Description-Content-Type: text/markdown
+
+# Perian Sky Platform CLI
+
+### Getting Started
+To get started on our platform, follow [our guide](https://perian.io/assets/files/Perian_Sky_Platform_Getting_Started.pdf) that will walk you through all the necessary setup and features.
+
+
+
+
```

