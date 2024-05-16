# Comparing `tmp/mypy_boto3_acm_pca-1.34.107.tar.gz` & `tmp/mypy-boto3-acm-pca-1.34.28.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_acm_pca-1.34.107.tar", last modified: Thu May 16 19:34:29 2024, max compression
+gzip compressed data, was "mypy-boto3-acm-pca-1.34.28.tar", last modified: Thu Jan 25 20:47:02 2024, max compression
```

## Comparing `mypy_boto3_acm_pca-1.34.107.tar` & `mypy-boto3-acm-pca-1.34.28.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:34:29.521034 mypy_boto3_acm_pca-1.34.107/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-05-16 19:34:29.521034 mypy_boto3_acm_pca-1.34.107/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12311 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:34:29.517034 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      920 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22329 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    22326 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    11984 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     4087 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)     4083 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    26576 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    26576 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/version.py
--rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/waiter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/waiter.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:34:29.521034 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13867 2024-05-16 19:34:29.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      739 2024-05-16 19:34:29.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:34:29.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:34:29.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 19:34:29.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       19 2024-05-16 19:34:29.000000 mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:34:29.521034 mypy_boto3_acm_pca-1.34.107/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1975 2024-05-16 19:31:52.000000 mypy_boto3_acm_pca-1.34.107/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:47:02.662944 mypy-boto3-acm-pca-1.34.28/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-01-25 20:46:45.000000 mypy-boto3-acm-pca-1.34.28/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-01-25 20:47:02.662944 mypy-boto3-acm-pca-1.34.28/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12310 2024-01-25 20:46:45.000000 mypy-boto3-acm-pca-1.34.28/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:47:02.662944 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-01-25 20:46:45.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1706 2024-01-25 20:46:45.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      906 2024-01-25 20:46:45.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22319 2024-01-25 20:46:45.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22316 2024-01-25 20:46:45.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11847 2024-01-25 20:46:46.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11847 2024-01-25 20:46:46.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     4105 2024-01-25 20:46:45.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-01-25 20:46:45.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-01-25 20:46:45.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    25494 2024-01-25 20:46:46.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25494 2024-01-25 20:46:46.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-01-25 20:46:45.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/version.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3584 2024-01-25 20:46:45.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3581 2024-01-25 20:46:45.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/waiter.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-01-25 20:47:02.662944 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13864 2024-01-25 20:47:02.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      739 2024-01-25 20:47:02.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 20:47:02.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-01-25 20:47:02.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-01-25 20:47:02.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       19 2024-01-25 20:47:02.000000 mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-01-25 20:47:02.662944 mypy-boto3-acm-pca-1.34.28/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-01-25 20:46:45.000000 mypy-boto3-acm-pca-1.34.28/setup.py
```

### Comparing `mypy_boto3_acm_pca-1.34.107/LICENSE` & `mypy-boto3-acm-pca-1.34.28/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_acm_pca-1.34.107/PKG-INFO` & `mypy-boto3-acm-pca-1.34.28/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm-pca
-Version: 1.34.107
-Summary: Type annotations for boto3.ACMPCA 1.34.107 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.28
+Summary: Type annotations for boto3.ACMPCA 1.34.28 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm-pca)](https://pepy.tech/project/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.34.107](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.34.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_acm_pca-1.34.107/README.md` & `mypy-boto3-acm-pca-1.34.28/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm-pca)](https://pepy.tech/project/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.34.107](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.34.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/__init__.py` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/__init__.pyi` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/__main__.py` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/__main__.py`

 * *Files 24% similar despite different names*

```diff
@@ -6,29 +6,28 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.ACMPCA 1.34.107\n"
-        "Version:         1.34.107\n"
-        "Builder version: 7.24.0\n"
-        "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca//\n"
-        "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA\n"
-        "Other services:  https://pypi.org/project/boto3-stubs/\n"
-        "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
+        "Type annotations for boto3.ACMPCA 1.34.28\nVersion:         1.34.28\nBuilder version:"
+        " 7.23.1\nDocs:           "
+        " https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca//\nBoto3 docs:     "
+        " https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA\nOther"
+        " services:  https://pypi.org/project/boto3-stubs/\nChangelog:      "
+        " https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.107")
+    print("1.34.28")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/client.py` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     ListCertificateAuthoritiesPaginator,
     ListPermissionsPaginator,
     ListTagsPaginator,
 )
 from .type_defs import (
     ApiPassthroughTypeDef,
     BlobTypeDef,
-    CertificateAuthorityConfigurationUnionTypeDef,
+    CertificateAuthorityConfigurationTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
@@ -133,15 +133,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/client/#close)
         """
 
     def create_certificate_authority(
         self,
         *,
-        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationUnionTypeDef,
+        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationTypeDef,
         CertificateAuthorityType: CertificateAuthorityTypeType,
         RevocationConfiguration: RevocationConfigurationTypeDef = ...,
         IdempotencyToken: str = ...,
         KeyStorageSecurityStandard: KeyStorageSecurityStandardType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         UsageMode: CertificateAuthorityUsageModeType = ...,
     ) -> CreateCertificateAuthorityResponseTypeDef:
```

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/client.pyi` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -34,15 +34,15 @@
     ListCertificateAuthoritiesPaginator,
     ListPermissionsPaginator,
     ListTagsPaginator,
 )
 from .type_defs import (
     ApiPassthroughTypeDef,
     BlobTypeDef,
-    CertificateAuthorityConfigurationUnionTypeDef,
+    CertificateAuthorityConfigurationTypeDef,
     CreateCertificateAuthorityAuditReportResponseTypeDef,
     CreateCertificateAuthorityResponseTypeDef,
     DescribeCertificateAuthorityAuditReportResponseTypeDef,
     DescribeCertificateAuthorityResponseTypeDef,
     EmptyResponseMetadataTypeDef,
     GetCertificateAuthorityCertificateResponseTypeDef,
     GetCertificateAuthorityCsrResponseTypeDef,
@@ -130,15 +130,15 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/client/#close)
         """
 
     def create_certificate_authority(
         self,
         *,
-        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationUnionTypeDef,
+        CertificateAuthorityConfiguration: CertificateAuthorityConfigurationTypeDef,
         CertificateAuthorityType: CertificateAuthorityTypeType,
         RevocationConfiguration: RevocationConfigurationTypeDef = ...,
         IdempotencyToken: str = ...,
         KeyStorageSecurityStandard: KeyStorageSecurityStandardType = ...,
         Tags: Sequence[TagTypeDef] = ...,
         UsageMode: CertificateAuthorityUsageModeType = ...,
     ) -> CreateCertificateAuthorityResponseTypeDef:
```

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/literals.py` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/literals.py`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,14 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
-    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -146,15 +145,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -172,15 +170,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -193,26 +190,24 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -273,14 +268,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -409,15 +405,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -461,15 +456,14 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -515,15 +509,14 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
-    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/literals.pyi` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/literals.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -127,15 +127,14 @@
     "application-insights",
     "applicationcostprofiler",
     "appmesh",
     "apprunner",
     "appstream",
     "appsync",
     "arc-zonal-shift",
-    "artifact",
     "athena",
     "auditmanager",
     "autoscaling",
     "autoscaling-plans",
     "b2bi",
     "backup",
     "backup-gateway",
@@ -146,15 +145,14 @@
     "bedrock-agent",
     "bedrock-agent-runtime",
     "bedrock-runtime",
     "billingconductor",
     "braket",
     "budgets",
     "ce",
-    "chatbot",
     "chime",
     "chime-sdk-identity",
     "chime-sdk-media-pipelines",
     "chime-sdk-meetings",
     "chime-sdk-messaging",
     "chime-sdk-voice",
     "cleanrooms",
@@ -172,15 +170,14 @@
     "cloudtrail",
     "cloudtrail-data",
     "cloudwatch",
     "codeartifact",
     "codebuild",
     "codecatalyst",
     "codecommit",
-    "codeconnections",
     "codedeploy",
     "codeguru-reviewer",
     "codeguru-security",
     "codeguruprofiler",
     "codepipeline",
     "codestar",
     "codestar-connections",
@@ -193,26 +190,24 @@
     "compute-optimizer",
     "config",
     "connect",
     "connect-contact-lens",
     "connectcampaigns",
     "connectcases",
     "connectparticipant",
-    "controlcatalog",
     "controltower",
     "cost-optimization-hub",
     "cur",
     "customer-profiles",
     "databrew",
     "dataexchange",
     "datapipeline",
     "datasync",
     "datazone",
     "dax",
-    "deadline",
     "detective",
     "devicefarm",
     "devops-guru",
     "directconnect",
     "discovery",
     "dlm",
     "dms",
@@ -273,14 +268,15 @@
     "inspector",
     "inspector-scan",
     "inspector2",
     "internetmonitor",
     "iot",
     "iot-data",
     "iot-jobs-data",
+    "iot-roborunner",
     "iot1click-devices",
     "iot1click-projects",
     "iotanalytics",
     "iotdeviceadvisor",
     "iotevents",
     "iotevents-data",
     "iotfleethub",
@@ -409,15 +405,14 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
-    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
@@ -461,15 +456,14 @@
     "sts",
     "supplychain",
     "support",
     "support-app",
     "swf",
     "synthetics",
     "textract",
-    "timestream-influxdb",
     "timestream-query",
     "timestream-write",
     "tnb",
     "transcribe",
     "transfer",
     "translate",
     "trustedadvisor",
@@ -515,15 +509,14 @@
     "ap-south-1",
     "ap-south-2",
     "ap-southeast-1",
     "ap-southeast-2",
     "ap-southeast-3",
     "ap-southeast-4",
     "ca-central-1",
-    "ca-west-1",
     "eu-central-1",
     "eu-central-2",
     "eu-north-1",
     "eu-south-1",
     "eu-south-2",
     "eu-west-1",
     "eu-west-2",
```

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/paginator.py` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -26,65 +26,61 @@
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ResourceOwnerType
 from .type_defs import (
-    ListCertificateAuthoritiesResponseTypeDef,
+    ListCertificateAuthoritiesResponsePaginatorTypeDef,
     ListPermissionsResponseTypeDef,
     ListTagsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListCertificateAuthoritiesPaginator", "ListPermissionsPaginator", "ListTagsPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
-
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
-
 class ListCertificateAuthoritiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListCertificateAuthorities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/paginators/#listcertificateauthoritiespaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceOwner: ResourceOwnerType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListCertificateAuthoritiesResponseTypeDef]:
+    ) -> _PageIterator[ListCertificateAuthoritiesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListCertificateAuthorities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/paginators/#listcertificateauthoritiespaginator)
         """
 
-
 class ListPermissionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListPermissions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/paginators/#listpermissionspaginator)
     """
 
     def paginate(
         self, *, CertificateAuthorityArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/paginators/#listpermissionspaginator)
         """
 
-
 class ListTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/paginators/#listtagspaginator)
     """
 
     def paginate(
```

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/paginator.pyi` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/paginator.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,61 +26,65 @@
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .literals import ResourceOwnerType
 from .type_defs import (
-    ListCertificateAuthoritiesResponseTypeDef,
+    ListCertificateAuthoritiesResponsePaginatorTypeDef,
     ListPermissionsResponseTypeDef,
     ListTagsResponseTypeDef,
     PaginatorConfigTypeDef,
 )
 
 __all__ = ("ListCertificateAuthoritiesPaginator", "ListPermissionsPaginator", "ListTagsPaginator")
 
 _ItemTypeDef = TypeVar("_ItemTypeDef")
 
+
 class _PageIterator(Generic[_ItemTypeDef], PageIterator):
     def __iter__(self) -> Iterator[_ItemTypeDef]:
         """
         Proxy method to specify iterator item type.
         """
 
+
 class ListCertificateAuthoritiesPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListCertificateAuthorities)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/paginators/#listcertificateauthoritiespaginator)
     """
 
     def paginate(
         self,
         *,
         ResourceOwner: ResourceOwnerType = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListCertificateAuthoritiesResponseTypeDef]:
+    ) -> _PageIterator[ListCertificateAuthoritiesResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListCertificateAuthorities.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/paginators/#listcertificateauthoritiespaginator)
         """
 
+
 class ListPermissionsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListPermissions)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/paginators/#listpermissionspaginator)
     """
 
     def paginate(
         self, *, CertificateAuthorityArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
     ) -> _PageIterator[ListPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/paginators/#listpermissionspaginator)
         """
 
+
 class ListTagsPaginator(Paginator):
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA.Paginator.ListTags)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/paginators/#listtagspaginator)
     """
 
     def paginate(
```

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/type_defs.py` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/type_defs.py`

 * *Files 4% similar despite different names*

```diff
@@ -81,16 +81,15 @@
     "PermissionTypeDef",
     "ListTagsRequestRequestTypeDef",
     "OcspConfigurationTypeDef",
     "QualifierTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "RestoreCertificateAuthorityRequestRequestTypeDef",
     "RevokeCertificateRequestRequestTypeDef",
-    "ASN1SubjectExtraOutputTypeDef",
-    "ASN1SubjectOutputTypeDef",
+    "ASN1SubjectPaginatorTypeDef",
     "ASN1SubjectTypeDef",
     "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "CreateCertificateAuthorityAuditReportResponseTypeDef",
     "CreateCertificateAuthorityResponseTypeDef",
     "DescribeCertificateAuthorityAuditReportResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCertificateAuthorityCertificateResponseTypeDef",
@@ -106,35 +105,32 @@
     "GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef",
     "GetCertificateRequestCertificateIssuedWaitTypeDef",
     "ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListPermissionsResponseTypeDef",
     "PolicyQualifierInfoTypeDef",
-    "GeneralNameExtraOutputTypeDef",
-    "GeneralNameOutputTypeDef",
+    "GeneralNamePaginatorTypeDef",
     "GeneralNameTypeDef",
     "RevocationConfigurationTypeDef",
     "PolicyInformationTypeDef",
-    "AccessDescriptionExtraOutputTypeDef",
-    "AccessDescriptionOutputTypeDef",
+    "AccessDescriptionPaginatorTypeDef",
     "AccessDescriptionTypeDef",
     "UpdateCertificateAuthorityRequestRequestTypeDef",
     "ExtensionsTypeDef",
-    "CsrExtensionsExtraOutputTypeDef",
-    "CsrExtensionsOutputTypeDef",
+    "CsrExtensionsPaginatorTypeDef",
     "CsrExtensionsTypeDef",
     "ApiPassthroughTypeDef",
-    "CertificateAuthorityConfigurationExtraOutputTypeDef",
-    "CertificateAuthorityConfigurationOutputTypeDef",
+    "CertificateAuthorityConfigurationPaginatorTypeDef",
     "CertificateAuthorityConfigurationTypeDef",
     "IssueCertificateRequestRequestTypeDef",
+    "CertificateAuthorityPaginatorTypeDef",
     "CertificateAuthorityTypeDef",
-    "CertificateAuthorityConfigurationUnionTypeDef",
     "CreateCertificateAuthorityRequestRequestTypeDef",
+    "ListCertificateAuthoritiesResponsePaginatorTypeDef",
     "DescribeCertificateAuthorityResponseTypeDef",
     "ListCertificateAuthoritiesResponseTypeDef",
 )
 
 CustomAttributeTypeDef = TypedDict(
     "CustomAttributeTypeDef",
     {
@@ -158,18 +154,18 @@
         "AuditReportResponseFormat": AuditReportResponseFormatType,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
+        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
-        "HostId": NotRequired[str],
     },
 )
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": NotRequired[str],
@@ -379,36 +375,16 @@
     "RevokeCertificateRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "CertificateSerial": str,
         "RevocationReason": RevocationReasonType,
     },
 )
-ASN1SubjectExtraOutputTypeDef = TypedDict(
-    "ASN1SubjectExtraOutputTypeDef",
-    {
-        "Country": NotRequired[str],
-        "Organization": NotRequired[str],
-        "OrganizationalUnit": NotRequired[str],
-        "DistinguishedNameQualifier": NotRequired[str],
-        "State": NotRequired[str],
-        "CommonName": NotRequired[str],
-        "SerialNumber": NotRequired[str],
-        "Locality": NotRequired[str],
-        "Title": NotRequired[str],
-        "Surname": NotRequired[str],
-        "GivenName": NotRequired[str],
-        "Initials": NotRequired[str],
-        "Pseudonym": NotRequired[str],
-        "GenerationQualifier": NotRequired[str],
-        "CustomAttributes": NotRequired[List[CustomAttributeTypeDef]],
-    },
-)
-ASN1SubjectOutputTypeDef = TypedDict(
-    "ASN1SubjectOutputTypeDef",
+ASN1SubjectPaginatorTypeDef = TypedDict(
+    "ASN1SubjectPaginatorTypeDef",
     {
         "Country": NotRequired[str],
         "Organization": NotRequired[str],
         "OrganizationalUnit": NotRequired[str],
         "DistinguishedNameQualifier": NotRequired[str],
         "State": NotRequired[str],
         "CommonName": NotRequired[str],
@@ -519,16 +495,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 TagCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "TagCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Tags": Sequence[TagTypeDef],
@@ -598,45 +574,32 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "Permissions": List[PermissionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 PolicyQualifierInfoTypeDef = TypedDict(
     "PolicyQualifierInfoTypeDef",
     {
         "PolicyQualifierId": Literal["CPS"],
         "Qualifier": QualifierTypeDef,
     },
 )
-GeneralNameExtraOutputTypeDef = TypedDict(
-    "GeneralNameExtraOutputTypeDef",
+GeneralNamePaginatorTypeDef = TypedDict(
+    "GeneralNamePaginatorTypeDef",
     {
         "OtherName": NotRequired[OtherNameTypeDef],
         "Rfc822Name": NotRequired[str],
         "DnsName": NotRequired[str],
-        "DirectoryName": NotRequired[ASN1SubjectExtraOutputTypeDef],
-        "EdiPartyName": NotRequired[EdiPartyNameTypeDef],
-        "UniformResourceIdentifier": NotRequired[str],
-        "IpAddress": NotRequired[str],
-        "RegisteredId": NotRequired[str],
-    },
-)
-GeneralNameOutputTypeDef = TypedDict(
-    "GeneralNameOutputTypeDef",
-    {
-        "OtherName": NotRequired[OtherNameTypeDef],
-        "Rfc822Name": NotRequired[str],
-        "DnsName": NotRequired[str],
-        "DirectoryName": NotRequired[ASN1SubjectOutputTypeDef],
+        "DirectoryName": NotRequired[ASN1SubjectPaginatorTypeDef],
         "EdiPartyName": NotRequired[EdiPartyNameTypeDef],
         "UniformResourceIdentifier": NotRequired[str],
         "IpAddress": NotRequired[str],
         "RegisteredId": NotRequired[str],
     },
 )
 GeneralNameTypeDef = TypedDict(
@@ -662,26 +625,19 @@
 PolicyInformationTypeDef = TypedDict(
     "PolicyInformationTypeDef",
     {
         "CertPolicyId": str,
         "PolicyQualifiers": NotRequired[Sequence[PolicyQualifierInfoTypeDef]],
     },
 )
-AccessDescriptionExtraOutputTypeDef = TypedDict(
-    "AccessDescriptionExtraOutputTypeDef",
-    {
-        "AccessMethod": AccessMethodTypeDef,
-        "AccessLocation": GeneralNameExtraOutputTypeDef,
-    },
-)
-AccessDescriptionOutputTypeDef = TypedDict(
-    "AccessDescriptionOutputTypeDef",
+AccessDescriptionPaginatorTypeDef = TypedDict(
+    "AccessDescriptionPaginatorTypeDef",
     {
         "AccessMethod": AccessMethodTypeDef,
-        "AccessLocation": GeneralNameOutputTypeDef,
+        "AccessLocation": GeneralNamePaginatorTypeDef,
     },
 )
 AccessDescriptionTypeDef = TypedDict(
     "AccessDescriptionTypeDef",
     {
         "AccessMethod": AccessMethodTypeDef,
         "AccessLocation": GeneralNameTypeDef,
@@ -701,26 +657,19 @@
         "CertificatePolicies": NotRequired[Sequence[PolicyInformationTypeDef]],
         "ExtendedKeyUsage": NotRequired[Sequence[ExtendedKeyUsageTypeDef]],
         "KeyUsage": NotRequired[KeyUsageTypeDef],
         "SubjectAlternativeNames": NotRequired[Sequence[GeneralNameTypeDef]],
         "CustomExtensions": NotRequired[Sequence[CustomExtensionTypeDef]],
     },
 )
-CsrExtensionsExtraOutputTypeDef = TypedDict(
-    "CsrExtensionsExtraOutputTypeDef",
+CsrExtensionsPaginatorTypeDef = TypedDict(
+    "CsrExtensionsPaginatorTypeDef",
     {
         "KeyUsage": NotRequired[KeyUsageTypeDef],
-        "SubjectInformationAccess": NotRequired[List[AccessDescriptionExtraOutputTypeDef]],
-    },
-)
-CsrExtensionsOutputTypeDef = TypedDict(
-    "CsrExtensionsOutputTypeDef",
-    {
-        "KeyUsage": NotRequired[KeyUsageTypeDef],
-        "SubjectInformationAccess": NotRequired[List[AccessDescriptionOutputTypeDef]],
+        "SubjectInformationAccess": NotRequired[List[AccessDescriptionPaginatorTypeDef]],
     },
 )
 CsrExtensionsTypeDef = TypedDict(
     "CsrExtensionsTypeDef",
     {
         "KeyUsage": NotRequired[KeyUsageTypeDef],
         "SubjectInformationAccess": NotRequired[Sequence[AccessDescriptionTypeDef]],
@@ -729,30 +678,21 @@
 ApiPassthroughTypeDef = TypedDict(
     "ApiPassthroughTypeDef",
     {
         "Extensions": NotRequired[ExtensionsTypeDef],
         "Subject": NotRequired[ASN1SubjectTypeDef],
     },
 )
-CertificateAuthorityConfigurationExtraOutputTypeDef = TypedDict(
-    "CertificateAuthorityConfigurationExtraOutputTypeDef",
+CertificateAuthorityConfigurationPaginatorTypeDef = TypedDict(
+    "CertificateAuthorityConfigurationPaginatorTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "SigningAlgorithm": SigningAlgorithmType,
-        "Subject": ASN1SubjectExtraOutputTypeDef,
-        "CsrExtensions": NotRequired[CsrExtensionsExtraOutputTypeDef],
-    },
-)
-CertificateAuthorityConfigurationOutputTypeDef = TypedDict(
-    "CertificateAuthorityConfigurationOutputTypeDef",
-    {
-        "KeyAlgorithm": KeyAlgorithmType,
-        "SigningAlgorithm": SigningAlgorithmType,
-        "Subject": ASN1SubjectOutputTypeDef,
-        "CsrExtensions": NotRequired[CsrExtensionsOutputTypeDef],
+        "Subject": ASN1SubjectPaginatorTypeDef,
+        "CsrExtensions": NotRequired[CsrExtensionsPaginatorTypeDef],
     },
 )
 CertificateAuthorityConfigurationTypeDef = TypedDict(
     "CertificateAuthorityConfigurationTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "SigningAlgorithm": SigningAlgorithmType,
@@ -769,59 +709,84 @@
         "Validity": ValidityTypeDef,
         "ApiPassthrough": NotRequired[ApiPassthroughTypeDef],
         "TemplateArn": NotRequired[str],
         "ValidityNotBefore": NotRequired[ValidityTypeDef],
         "IdempotencyToken": NotRequired[str],
     },
 )
-CertificateAuthorityTypeDef = TypedDict(
-    "CertificateAuthorityTypeDef",
+CertificateAuthorityPaginatorTypeDef = TypedDict(
+    "CertificateAuthorityPaginatorTypeDef",
     {
         "Arn": NotRequired[str],
         "OwnerAccount": NotRequired[str],
         "CreatedAt": NotRequired[datetime],
         "LastStateChangeAt": NotRequired[datetime],
         "Type": NotRequired[CertificateAuthorityTypeType],
         "Serial": NotRequired[str],
         "Status": NotRequired[CertificateAuthorityStatusType],
         "NotBefore": NotRequired[datetime],
         "NotAfter": NotRequired[datetime],
         "FailureReason": NotRequired[FailureReasonType],
         "CertificateAuthorityConfiguration": NotRequired[
-            CertificateAuthorityConfigurationOutputTypeDef
+            CertificateAuthorityConfigurationPaginatorTypeDef
         ],
         "RevocationConfiguration": NotRequired[RevocationConfigurationTypeDef],
         "RestorableUntil": NotRequired[datetime],
         "KeyStorageSecurityStandard": NotRequired[KeyStorageSecurityStandardType],
         "UsageMode": NotRequired[CertificateAuthorityUsageModeType],
     },
 )
-CertificateAuthorityConfigurationUnionTypeDef = Union[
-    CertificateAuthorityConfigurationTypeDef, CertificateAuthorityConfigurationExtraOutputTypeDef
-]
+CertificateAuthorityTypeDef = TypedDict(
+    "CertificateAuthorityTypeDef",
+    {
+        "Arn": NotRequired[str],
+        "OwnerAccount": NotRequired[str],
+        "CreatedAt": NotRequired[datetime],
+        "LastStateChangeAt": NotRequired[datetime],
+        "Type": NotRequired[CertificateAuthorityTypeType],
+        "Serial": NotRequired[str],
+        "Status": NotRequired[CertificateAuthorityStatusType],
+        "NotBefore": NotRequired[datetime],
+        "NotAfter": NotRequired[datetime],
+        "FailureReason": NotRequired[FailureReasonType],
+        "CertificateAuthorityConfiguration": NotRequired[CertificateAuthorityConfigurationTypeDef],
+        "RevocationConfiguration": NotRequired[RevocationConfigurationTypeDef],
+        "RestorableUntil": NotRequired[datetime],
+        "KeyStorageSecurityStandard": NotRequired[KeyStorageSecurityStandardType],
+        "UsageMode": NotRequired[CertificateAuthorityUsageModeType],
+    },
+)
 CreateCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "CreateCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationTypeDef,
         "CertificateAuthorityType": CertificateAuthorityTypeType,
         "RevocationConfiguration": NotRequired[RevocationConfigurationTypeDef],
         "IdempotencyToken": NotRequired[str],
         "KeyStorageSecurityStandard": NotRequired[KeyStorageSecurityStandardType],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "UsageMode": NotRequired[CertificateAuthorityUsageModeType],
     },
 )
+ListCertificateAuthoritiesResponsePaginatorTypeDef = TypedDict(
+    "ListCertificateAuthoritiesResponsePaginatorTypeDef",
+    {
+        "CertificateAuthorities": List[CertificateAuthorityPaginatorTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DescribeCertificateAuthorityResponseTypeDef = TypedDict(
     "DescribeCertificateAuthorityResponseTypeDef",
     {
         "CertificateAuthority": CertificateAuthorityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListCertificateAuthoritiesResponseTypeDef = TypedDict(
     "ListCertificateAuthoritiesResponseTypeDef",
     {
         "CertificateAuthorities": List[CertificateAuthorityTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/type_defs.pyi` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/type_defs.pyi`

 * *Files 4% similar despite different names*

```diff
@@ -81,16 +81,15 @@
     "PermissionTypeDef",
     "ListTagsRequestRequestTypeDef",
     "OcspConfigurationTypeDef",
     "QualifierTypeDef",
     "PutPolicyRequestRequestTypeDef",
     "RestoreCertificateAuthorityRequestRequestTypeDef",
     "RevokeCertificateRequestRequestTypeDef",
-    "ASN1SubjectExtraOutputTypeDef",
-    "ASN1SubjectOutputTypeDef",
+    "ASN1SubjectPaginatorTypeDef",
     "ASN1SubjectTypeDef",
     "ImportCertificateAuthorityCertificateRequestRequestTypeDef",
     "CreateCertificateAuthorityAuditReportResponseTypeDef",
     "CreateCertificateAuthorityResponseTypeDef",
     "DescribeCertificateAuthorityAuditReportResponseTypeDef",
     "EmptyResponseMetadataTypeDef",
     "GetCertificateAuthorityCertificateResponseTypeDef",
@@ -106,35 +105,32 @@
     "GetCertificateAuthorityCsrRequestCertificateAuthorityCSRCreatedWaitTypeDef",
     "GetCertificateRequestCertificateIssuedWaitTypeDef",
     "ListCertificateAuthoritiesRequestListCertificateAuthoritiesPaginateTypeDef",
     "ListPermissionsRequestListPermissionsPaginateTypeDef",
     "ListTagsRequestListTagsPaginateTypeDef",
     "ListPermissionsResponseTypeDef",
     "PolicyQualifierInfoTypeDef",
-    "GeneralNameExtraOutputTypeDef",
-    "GeneralNameOutputTypeDef",
+    "GeneralNamePaginatorTypeDef",
     "GeneralNameTypeDef",
     "RevocationConfigurationTypeDef",
     "PolicyInformationTypeDef",
-    "AccessDescriptionExtraOutputTypeDef",
-    "AccessDescriptionOutputTypeDef",
+    "AccessDescriptionPaginatorTypeDef",
     "AccessDescriptionTypeDef",
     "UpdateCertificateAuthorityRequestRequestTypeDef",
     "ExtensionsTypeDef",
-    "CsrExtensionsExtraOutputTypeDef",
-    "CsrExtensionsOutputTypeDef",
+    "CsrExtensionsPaginatorTypeDef",
     "CsrExtensionsTypeDef",
     "ApiPassthroughTypeDef",
-    "CertificateAuthorityConfigurationExtraOutputTypeDef",
-    "CertificateAuthorityConfigurationOutputTypeDef",
+    "CertificateAuthorityConfigurationPaginatorTypeDef",
     "CertificateAuthorityConfigurationTypeDef",
     "IssueCertificateRequestRequestTypeDef",
+    "CertificateAuthorityPaginatorTypeDef",
     "CertificateAuthorityTypeDef",
-    "CertificateAuthorityConfigurationUnionTypeDef",
     "CreateCertificateAuthorityRequestRequestTypeDef",
+    "ListCertificateAuthoritiesResponsePaginatorTypeDef",
     "DescribeCertificateAuthorityResponseTypeDef",
     "ListCertificateAuthoritiesResponseTypeDef",
 )
 
 CustomAttributeTypeDef = TypedDict(
     "CustomAttributeTypeDef",
     {
@@ -158,18 +154,18 @@
         "AuditReportResponseFormat": AuditReportResponseFormatType,
     },
 )
 ResponseMetadataTypeDef = TypedDict(
     "ResponseMetadataTypeDef",
     {
         "RequestId": str,
+        "HostId": str,
         "HTTPStatusCode": int,
         "HTTPHeaders": Dict[str, str],
         "RetryAttempts": int,
-        "HostId": NotRequired[str],
     },
 )
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": NotRequired[str],
@@ -379,36 +375,16 @@
     "RevokeCertificateRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "CertificateSerial": str,
         "RevocationReason": RevocationReasonType,
     },
 )
-ASN1SubjectExtraOutputTypeDef = TypedDict(
-    "ASN1SubjectExtraOutputTypeDef",
-    {
-        "Country": NotRequired[str],
-        "Organization": NotRequired[str],
-        "OrganizationalUnit": NotRequired[str],
-        "DistinguishedNameQualifier": NotRequired[str],
-        "State": NotRequired[str],
-        "CommonName": NotRequired[str],
-        "SerialNumber": NotRequired[str],
-        "Locality": NotRequired[str],
-        "Title": NotRequired[str],
-        "Surname": NotRequired[str],
-        "GivenName": NotRequired[str],
-        "Initials": NotRequired[str],
-        "Pseudonym": NotRequired[str],
-        "GenerationQualifier": NotRequired[str],
-        "CustomAttributes": NotRequired[List[CustomAttributeTypeDef]],
-    },
-)
-ASN1SubjectOutputTypeDef = TypedDict(
-    "ASN1SubjectOutputTypeDef",
+ASN1SubjectPaginatorTypeDef = TypedDict(
+    "ASN1SubjectPaginatorTypeDef",
     {
         "Country": NotRequired[str],
         "Organization": NotRequired[str],
         "OrganizationalUnit": NotRequired[str],
         "DistinguishedNameQualifier": NotRequired[str],
         "State": NotRequired[str],
         "CommonName": NotRequired[str],
@@ -519,16 +495,16 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListTagsResponseTypeDef = TypedDict(
     "ListTagsResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 TagCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "TagCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityArn": str,
         "Tags": Sequence[TagTypeDef],
@@ -598,45 +574,32 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListPermissionsResponseTypeDef = TypedDict(
     "ListPermissionsResponseTypeDef",
     {
         "Permissions": List[PermissionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 PolicyQualifierInfoTypeDef = TypedDict(
     "PolicyQualifierInfoTypeDef",
     {
         "PolicyQualifierId": Literal["CPS"],
         "Qualifier": QualifierTypeDef,
     },
 )
-GeneralNameExtraOutputTypeDef = TypedDict(
-    "GeneralNameExtraOutputTypeDef",
+GeneralNamePaginatorTypeDef = TypedDict(
+    "GeneralNamePaginatorTypeDef",
     {
         "OtherName": NotRequired[OtherNameTypeDef],
         "Rfc822Name": NotRequired[str],
         "DnsName": NotRequired[str],
-        "DirectoryName": NotRequired[ASN1SubjectExtraOutputTypeDef],
-        "EdiPartyName": NotRequired[EdiPartyNameTypeDef],
-        "UniformResourceIdentifier": NotRequired[str],
-        "IpAddress": NotRequired[str],
-        "RegisteredId": NotRequired[str],
-    },
-)
-GeneralNameOutputTypeDef = TypedDict(
-    "GeneralNameOutputTypeDef",
-    {
-        "OtherName": NotRequired[OtherNameTypeDef],
-        "Rfc822Name": NotRequired[str],
-        "DnsName": NotRequired[str],
-        "DirectoryName": NotRequired[ASN1SubjectOutputTypeDef],
+        "DirectoryName": NotRequired[ASN1SubjectPaginatorTypeDef],
         "EdiPartyName": NotRequired[EdiPartyNameTypeDef],
         "UniformResourceIdentifier": NotRequired[str],
         "IpAddress": NotRequired[str],
         "RegisteredId": NotRequired[str],
     },
 )
 GeneralNameTypeDef = TypedDict(
@@ -662,26 +625,19 @@
 PolicyInformationTypeDef = TypedDict(
     "PolicyInformationTypeDef",
     {
         "CertPolicyId": str,
         "PolicyQualifiers": NotRequired[Sequence[PolicyQualifierInfoTypeDef]],
     },
 )
-AccessDescriptionExtraOutputTypeDef = TypedDict(
-    "AccessDescriptionExtraOutputTypeDef",
-    {
-        "AccessMethod": AccessMethodTypeDef,
-        "AccessLocation": GeneralNameExtraOutputTypeDef,
-    },
-)
-AccessDescriptionOutputTypeDef = TypedDict(
-    "AccessDescriptionOutputTypeDef",
+AccessDescriptionPaginatorTypeDef = TypedDict(
+    "AccessDescriptionPaginatorTypeDef",
     {
         "AccessMethod": AccessMethodTypeDef,
-        "AccessLocation": GeneralNameOutputTypeDef,
+        "AccessLocation": GeneralNamePaginatorTypeDef,
     },
 )
 AccessDescriptionTypeDef = TypedDict(
     "AccessDescriptionTypeDef",
     {
         "AccessMethod": AccessMethodTypeDef,
         "AccessLocation": GeneralNameTypeDef,
@@ -701,26 +657,19 @@
         "CertificatePolicies": NotRequired[Sequence[PolicyInformationTypeDef]],
         "ExtendedKeyUsage": NotRequired[Sequence[ExtendedKeyUsageTypeDef]],
         "KeyUsage": NotRequired[KeyUsageTypeDef],
         "SubjectAlternativeNames": NotRequired[Sequence[GeneralNameTypeDef]],
         "CustomExtensions": NotRequired[Sequence[CustomExtensionTypeDef]],
     },
 )
-CsrExtensionsExtraOutputTypeDef = TypedDict(
-    "CsrExtensionsExtraOutputTypeDef",
+CsrExtensionsPaginatorTypeDef = TypedDict(
+    "CsrExtensionsPaginatorTypeDef",
     {
         "KeyUsage": NotRequired[KeyUsageTypeDef],
-        "SubjectInformationAccess": NotRequired[List[AccessDescriptionExtraOutputTypeDef]],
-    },
-)
-CsrExtensionsOutputTypeDef = TypedDict(
-    "CsrExtensionsOutputTypeDef",
-    {
-        "KeyUsage": NotRequired[KeyUsageTypeDef],
-        "SubjectInformationAccess": NotRequired[List[AccessDescriptionOutputTypeDef]],
+        "SubjectInformationAccess": NotRequired[List[AccessDescriptionPaginatorTypeDef]],
     },
 )
 CsrExtensionsTypeDef = TypedDict(
     "CsrExtensionsTypeDef",
     {
         "KeyUsage": NotRequired[KeyUsageTypeDef],
         "SubjectInformationAccess": NotRequired[Sequence[AccessDescriptionTypeDef]],
@@ -729,30 +678,21 @@
 ApiPassthroughTypeDef = TypedDict(
     "ApiPassthroughTypeDef",
     {
         "Extensions": NotRequired[ExtensionsTypeDef],
         "Subject": NotRequired[ASN1SubjectTypeDef],
     },
 )
-CertificateAuthorityConfigurationExtraOutputTypeDef = TypedDict(
-    "CertificateAuthorityConfigurationExtraOutputTypeDef",
+CertificateAuthorityConfigurationPaginatorTypeDef = TypedDict(
+    "CertificateAuthorityConfigurationPaginatorTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "SigningAlgorithm": SigningAlgorithmType,
-        "Subject": ASN1SubjectExtraOutputTypeDef,
-        "CsrExtensions": NotRequired[CsrExtensionsExtraOutputTypeDef],
-    },
-)
-CertificateAuthorityConfigurationOutputTypeDef = TypedDict(
-    "CertificateAuthorityConfigurationOutputTypeDef",
-    {
-        "KeyAlgorithm": KeyAlgorithmType,
-        "SigningAlgorithm": SigningAlgorithmType,
-        "Subject": ASN1SubjectOutputTypeDef,
-        "CsrExtensions": NotRequired[CsrExtensionsOutputTypeDef],
+        "Subject": ASN1SubjectPaginatorTypeDef,
+        "CsrExtensions": NotRequired[CsrExtensionsPaginatorTypeDef],
     },
 )
 CertificateAuthorityConfigurationTypeDef = TypedDict(
     "CertificateAuthorityConfigurationTypeDef",
     {
         "KeyAlgorithm": KeyAlgorithmType,
         "SigningAlgorithm": SigningAlgorithmType,
@@ -769,59 +709,84 @@
         "Validity": ValidityTypeDef,
         "ApiPassthrough": NotRequired[ApiPassthroughTypeDef],
         "TemplateArn": NotRequired[str],
         "ValidityNotBefore": NotRequired[ValidityTypeDef],
         "IdempotencyToken": NotRequired[str],
     },
 )
-CertificateAuthorityTypeDef = TypedDict(
-    "CertificateAuthorityTypeDef",
+CertificateAuthorityPaginatorTypeDef = TypedDict(
+    "CertificateAuthorityPaginatorTypeDef",
     {
         "Arn": NotRequired[str],
         "OwnerAccount": NotRequired[str],
         "CreatedAt": NotRequired[datetime],
         "LastStateChangeAt": NotRequired[datetime],
         "Type": NotRequired[CertificateAuthorityTypeType],
         "Serial": NotRequired[str],
         "Status": NotRequired[CertificateAuthorityStatusType],
         "NotBefore": NotRequired[datetime],
         "NotAfter": NotRequired[datetime],
         "FailureReason": NotRequired[FailureReasonType],
         "CertificateAuthorityConfiguration": NotRequired[
-            CertificateAuthorityConfigurationOutputTypeDef
+            CertificateAuthorityConfigurationPaginatorTypeDef
         ],
         "RevocationConfiguration": NotRequired[RevocationConfigurationTypeDef],
         "RestorableUntil": NotRequired[datetime],
         "KeyStorageSecurityStandard": NotRequired[KeyStorageSecurityStandardType],
         "UsageMode": NotRequired[CertificateAuthorityUsageModeType],
     },
 )
-CertificateAuthorityConfigurationUnionTypeDef = Union[
-    CertificateAuthorityConfigurationTypeDef, CertificateAuthorityConfigurationExtraOutputTypeDef
-]
+CertificateAuthorityTypeDef = TypedDict(
+    "CertificateAuthorityTypeDef",
+    {
+        "Arn": NotRequired[str],
+        "OwnerAccount": NotRequired[str],
+        "CreatedAt": NotRequired[datetime],
+        "LastStateChangeAt": NotRequired[datetime],
+        "Type": NotRequired[CertificateAuthorityTypeType],
+        "Serial": NotRequired[str],
+        "Status": NotRequired[CertificateAuthorityStatusType],
+        "NotBefore": NotRequired[datetime],
+        "NotAfter": NotRequired[datetime],
+        "FailureReason": NotRequired[FailureReasonType],
+        "CertificateAuthorityConfiguration": NotRequired[CertificateAuthorityConfigurationTypeDef],
+        "RevocationConfiguration": NotRequired[RevocationConfigurationTypeDef],
+        "RestorableUntil": NotRequired[datetime],
+        "KeyStorageSecurityStandard": NotRequired[KeyStorageSecurityStandardType],
+        "UsageMode": NotRequired[CertificateAuthorityUsageModeType],
+    },
+)
 CreateCertificateAuthorityRequestRequestTypeDef = TypedDict(
     "CreateCertificateAuthorityRequestRequestTypeDef",
     {
         "CertificateAuthorityConfiguration": CertificateAuthorityConfigurationTypeDef,
         "CertificateAuthorityType": CertificateAuthorityTypeType,
         "RevocationConfiguration": NotRequired[RevocationConfigurationTypeDef],
         "IdempotencyToken": NotRequired[str],
         "KeyStorageSecurityStandard": NotRequired[KeyStorageSecurityStandardType],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "UsageMode": NotRequired[CertificateAuthorityUsageModeType],
     },
 )
+ListCertificateAuthoritiesResponsePaginatorTypeDef = TypedDict(
+    "ListCertificateAuthoritiesResponsePaginatorTypeDef",
+    {
+        "CertificateAuthorities": List[CertificateAuthorityPaginatorTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DescribeCertificateAuthorityResponseTypeDef = TypedDict(
     "DescribeCertificateAuthorityResponseTypeDef",
     {
         "CertificateAuthority": CertificateAuthorityTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListCertificateAuthoritiesResponseTypeDef = TypedDict(
     "ListCertificateAuthoritiesResponseTypeDef",
     {
         "CertificateAuthorities": List[CertificateAuthorityTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
```

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/waiter.py` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/waiter.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca/waiter.pyi` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca/waiter.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca.egg-info/PKG-INFO` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-acm-pca
-Version: 1.34.107
-Summary: Type annotations for boto3.ACMPCA 1.34.107 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.28
+Summary: Type annotations for boto3.ACMPCA 1.34.28 service generated with mypy-boto3-builder 7.23.1
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-acm-pca.svg?color=blue)](https://pypi.org/project/mypy-boto3-acm-pca)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-acm-pca)](https://pepy.tech/project/mypy-boto3-acm-pca)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.ACMPCA 1.34.107](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
+[boto3.ACMPCA 1.34.28](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/acm-pca.html#ACMPCA)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.1](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-acm-pca docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_acm_pca/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_acm_pca-1.34.107/mypy_boto3_acm_pca.egg-info/SOURCES.txt` & `mypy-boto3-acm-pca-1.34.28/mypy_boto3_acm_pca.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_acm_pca-1.34.107/setup.py` & `mypy-boto3-acm-pca-1.34.28/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -7,21 +7,23 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-acm-pca",
-    version="1.34.107",
+    version="1.34.28",
     packages=["mypy_boto3_acm_pca"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.ACMPCA 1.34.107 service generated with mypy-boto3-builder 7.24.0",
+    description=(
+        "Type annotations for boto3.ACMPCA 1.34.28 service generated with mypy-boto3-builder 7.23.1"
+    ),
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

