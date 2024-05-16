# Comparing `tmp/iam_builder-4.3.0.tar.gz` & `tmp/iam_builder-4.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "iam_builder-4.3.0.tar", max compression
+gzip compressed data, was "iam_builder-4.4.0.tar", max compression
```

## Comparing `iam_builder-4.3.0.tar` & `iam_builder-4.4.0.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     5365 2024-04-18 13:42:16.185654 iam_builder-4.3.0/README.md
--rw-r--r--   0        0        0        0 2024-04-18 13:42:16.185654 iam_builder-4.3.0/iam_builder/__init__.py
--rw-r--r--   0        0        0      803 2024-04-18 13:42:16.185654 iam_builder-4.3.0/iam_builder/command_line.py
--rw-r--r--   0        0        0       93 2024-04-18 13:42:16.185654 iam_builder-4.3.0/iam_builder/exceptions.py
--rw-r--r--   0        0        0     3414 2024-04-18 13:42:16.185654 iam_builder-4.3.0/iam_builder/iam_builder.py
--rw-r--r--   0        0        0      430 2024-04-18 13:42:16.185654 iam_builder-4.3.0/iam_builder/iam_schema.py
--rw-r--r--   0        0        0     3216 2024-04-18 13:42:16.185654 iam_builder-4.3.0/iam_builder/schemas/iam_schema.json
--rwxr-xr-x   0        0        0    11633 2024-04-18 13:42:16.185654 iam_builder-4.3.0/iam_builder/templates.py
--rw-r--r--   0        0        0      476 2024-04-18 13:42:16.185654 iam_builder-4.3.0/pyproject.toml
--rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 iam_builder-4.3.0/PKG-INFO
+-rw-r--r--   0        0        0     5365 2024-05-16 08:16:56.632107 iam_builder-4.4.0/README.md
+-rw-r--r--   0        0        0        0 2024-05-16 08:16:56.632107 iam_builder-4.4.0/iam_builder/__init__.py
+-rw-r--r--   0        0        0      803 2024-05-16 08:16:56.632107 iam_builder-4.4.0/iam_builder/command_line.py
+-rw-r--r--   0        0        0       93 2024-05-16 08:16:56.632107 iam_builder-4.4.0/iam_builder/exceptions.py
+-rw-r--r--   0        0        0     3414 2024-05-16 08:16:56.632107 iam_builder-4.4.0/iam_builder/iam_builder.py
+-rw-r--r--   0        0        0      430 2024-05-16 08:16:56.632107 iam_builder-4.4.0/iam_builder/iam_schema.py
+-rw-r--r--   0        0        0     3216 2024-05-16 08:16:56.636107 iam_builder-4.4.0/iam_builder/schemas/iam_schema.json
+-rwxr-xr-x   0        0        0    11681 2024-05-16 08:16:56.636107 iam_builder-4.4.0/iam_builder/templates.py
+-rw-r--r--   0        0        0      476 2024-05-16 08:16:56.636107 iam_builder-4.4.0/pyproject.toml
+-rw-r--r--   0        0        0     6151 1970-01-01 00:00:00.000000 iam_builder-4.4.0/PKG-INFO
```

### Comparing `iam_builder-4.3.0/README.md` & `iam_builder-4.4.0/README.md`

 * *Files identical despite different names*

### Comparing `iam_builder-4.3.0/iam_builder/command_line.py` & `iam_builder-4.4.0/iam_builder/command_line.py`

 * *Files identical despite different names*

### Comparing `iam_builder-4.3.0/iam_builder/iam_builder.py` & `iam_builder-4.4.0/iam_builder/iam_builder.py`

 * *Files identical despite different names*

### Comparing `iam_builder-4.3.0/iam_builder/schemas/iam_schema.json` & `iam_builder-4.4.0/iam_builder/schemas/iam_schema.json`

 * *Files identical despite different names*

### Comparing `iam_builder-4.3.0/iam_builder/templates.py` & `iam_builder-4.4.0/iam_builder/templates.py`

 * *Files 1% similar despite different names*

```diff
@@ -202,14 +202,15 @@
                     "athena:GetCatalogs",
                     "athena:GetExecutionEngine",
                     "athena:GetExecutionEngines",
                     "athena:GetNamespace",
                     "athena:GetNamespaces",
                     "athena:GetTable",
                     "athena:GetTables",
+                    "athena:GetTableMetadata",
                     "athena:RunQuery",
                     "glue:GetDatabase",
                     "glue:GetDatabases",
                     "glue:GetTable",
                     "glue:GetTables",
                     "glue:GetPartition",
                     "glue:GetPartitions",
@@ -382,8 +383,8 @@
             "kms:Encrypt",
             "kms:DescribeKey",
             "kms:Decrypt"
         ],
         "Effect": "Allow",
         "Resource": kms_arns,
     }
-    return policy
+    return policy
```

### Comparing `iam_builder-4.3.0/PKG-INFO` & `iam_builder-4.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: iam_builder
-Version: 4.3.0
+Version: 4.4.0
 Summary: A lil python package to generate iam policies
 License: MIT
 Author: Karik Isichei
 Author-email: karik.isichei@digital.justice.gov.uk
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

