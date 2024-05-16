# Comparing `tmp/mypy-boto3-mwaa-1.34.30.tar.gz` & `tmp/mypy-boto3-mwaa-1.34.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy-boto3-mwaa-1.34.30.tar", last modified: Mon Jan 29 20:47:49 2024, max compression
+gzip compressed data, was "mypy-boto3-mwaa-1.34.57.tar", last modified: Wed Mar  6 21:33:27 2024, max compression
```

## Comparing `mypy-boto3-mwaa-1.34.30.tar` & `mypy-boto3-mwaa-1.34.57.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 20:47:49.714680 mypy-boto3-mwaa-1.34.30/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-29 20:47:24.000000 mypy-boto3-mwaa-1.34.30/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    12532 2024-01-29 20:47:49.714680 mypy-boto3-mwaa-1.34.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-01-29 20:47:24.000000 mypy-boto3-mwaa-1.34.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 20:47:49.714680 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-29 20:47:25.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      566 2024-01-29 20:47:25.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      907 2024-01-29 20:47:25.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-01-29 20:47:25.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-01-29 20:47:25.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-01-29 20:47:25.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)     9794 2024-01-29 20:47:25.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-01-29 20:47:25.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-01-29 20:47:25.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-29 20:47:25.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-01-29 20:47:25.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    12394 2024-01-29 20:47:25.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-29 20:47:24.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-29 20:47:49.714680 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    12532 2024-01-29 20:47:49.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      623 2024-01-29 20:47:49.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 20:47:49.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-29 20:47:49.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-29 20:47:49.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-01-29 20:47:49.000000 mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-29 20:47:49.714680 mypy-boto3-mwaa-1.34.30/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-01-29 20:47:24.000000 mypy-boto3-mwaa-1.34.30/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:27.652249 mypy-boto3-mwaa-1.34.57/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-06 21:32:58.000000 mypy-boto3-mwaa-1.34.57/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    12532 2024-03-06 21:33:27.652249 mypy-boto3-mwaa-1.34.57/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    10989 2024-03-06 21:32:58.000000 mypy-boto3-mwaa-1.34.57/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:27.652249 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-06 21:32:58.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      566 2024-03-06 21:32:58.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      907 2024-03-06 21:32:58.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11191 2024-03-06 21:32:58.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11188 2024-03-06 21:32:58.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-03-06 21:32:59.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9825 2024-03-06 21:32:59.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1795 2024-03-06 21:32:58.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1793 2024-03-06 21:32:58.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-06 21:32:58.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    12407 2024-03-06 21:32:59.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12407 2024-03-06 21:32:59.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-06 21:32:58.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-06 21:33:27.652249 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    12532 2024-03-06 21:33:27.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      623 2024-03-06 21:33:27.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 21:33:27.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-06 21:33:27.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-06 21:33:27.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-03-06 21:33:27.000000 mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-06 21:33:27.652249 mypy-boto3-mwaa-1.34.57/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-03-06 21:32:58.000000 mypy-boto3-mwaa-1.34.57/setup.py
```

### Comparing `mypy-boto3-mwaa-1.34.30/LICENSE` & `mypy-boto3-mwaa-1.34.57/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.34.30/PKG-INFO` & `mypy-boto3-mwaa-1.34.57/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mwaa
-Version: 1.34.30
-Summary: Type annotations for boto3.MWAA 1.34.30 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.57
+Summary: Type annotations for boto3.MWAA 1.34.57 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mwaa)](https://pepy.tech/project/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.34.30](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.34.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mwaa-1.34.30/README.md` & `mypy-boto3-mwaa-1.34.57/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mwaa)](https://pepy.tech/project/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.34.30](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.34.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/__init__.py` & `mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/__init__.pyi` & `mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/__main__.py` & `mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/__main__.py`

 * *Files 15% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.MWAA 1.34.30\n"
-        "Version:         1.34.30\n"
-        "Builder version: 7.23.1\n"
+        "Type annotations for boto3.MWAA 1.34.57\n"
+        "Version:         1.34.57\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.30")
+    print("1.34.57")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/client.py` & `mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/client.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/client.pyi` & `mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/client.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/literals.py` & `mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -123,14 +124,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
```

### Comparing `mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/literals.pyi` & `mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -105,14 +105,15 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
+    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -123,14 +124,15 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
+    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
```

### Comparing `mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/paginator.py` & `mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/paginator.py`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/paginator.pyi` & `mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/paginator.pyi`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/type_defs.py` & `mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/type_defs.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,18 +77,18 @@
         "Name": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "SecurityGroupIds": NotRequired[Sequence[str]],
         "SubnetIds": NotRequired[Sequence[str]],
```

### Comparing `mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa/type_defs.pyi` & `mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa/type_defs.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -77,18 +77,18 @@
         "Name": str,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
-        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
+        "HostId": NotRequired[str],
     },
 )
 NetworkConfigurationTypeDef = TypedDict(
     "NetworkConfigurationTypeDef",
     {
         "SecurityGroupIds": NotRequired[Sequence[str]],
         "SubnetIds": NotRequired[Sequence[str]],
```

### Comparing `mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa.egg-info/PKG-INFO` & `mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-mwaa
-Version: 1.34.30
-Summary: Type annotations for boto3.MWAA 1.34.30 service generated with mypy-boto3-builder 7.23.1
+Version: 1.34.57
+Summary: Type annotations for boto3.MWAA 1.34.57 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-mwaa.svg?color=blue)](https://pypi.org/project/mypy-boto3-mwaa)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-mwaa)](https://pepy.tech/project/mypy-boto3-mwaa)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.MWAA 1.34.30](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
+[boto3.MWAA 1.34.57](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/mwaa.html#MWAA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-mwaa docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_mwaa/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy-boto3-mwaa-1.34.30/mypy_boto3_mwaa.egg-info/SOURCES.txt` & `mypy-boto3-mwaa-1.34.57/mypy_boto3_mwaa.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy-boto3-mwaa-1.34.30/setup.py` & `mypy-boto3-mwaa-1.34.57/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-mwaa",
-    version="1.34.30",
+    version="1.34.57",
     packages=["mypy_boto3_mwaa"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.MWAA 1.34.30 service generated with mypy-boto3-builder 7.23.1",
+    description="Type annotations for boto3.MWAA 1.34.57 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

