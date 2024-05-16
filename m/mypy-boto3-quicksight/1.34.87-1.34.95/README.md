# Comparing `tmp/mypy_boto3_quicksight-1.34.87.tar.gz` & `tmp/mypy_boto3_quicksight-1.34.95.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_quicksight-1.34.87.tar", last modified: Thu Apr 18 19:34:22 2024, max compression
+gzip compressed data, was "mypy_boto3_quicksight-1.34.95.tar", last modified: Tue Apr 30 19:34:53 2024, max compression
```

## Comparing `mypy_boto3_quicksight-1.34.87.tar` & `mypy_boto3_quicksight-1.34.95.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:22.200633 mypy_boto3_quicksight-1.34.87/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-18 19:34:22.200633 mypy_boto3_quicksight-1.34.87/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15494 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:22.200633 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)   135105 2024-04-18 19:33:31.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/client.py
--rw-r--r--   0 runner    (1001) docker     (127)   135102 2024-04-18 19:33:31.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    39714 2024-04-18 19:33:32.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    39714 2024-04-18 19:33:32.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    36169 2024-04-18 19:33:32.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    36137 2024-04-18 19:33:32.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)   386207 2024-04-18 19:33:42.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)   386207 2024-04-18 19:33:36.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 19:34:22.200633 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-18 19:34:22.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-18 19:34:22.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:34:22.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 19:34:22.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-18 19:34:22.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-18 19:34:22.000000 mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 19:34:22.200633 mypy_boto3_quicksight-1.34.87/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-18 19:33:30.000000 mypy_boto3_quicksight-1.34.87/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:53.871056 mypy_boto3_quicksight-1.34.95/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-04-30 19:33:55.000000 mypy_boto3_quicksight-1.34.95/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-30 19:34:53.871056 mypy_boto3_quicksight-1.34.95/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15494 2024-04-30 19:33:55.000000 mypy_boto3_quicksight-1.34.95/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:53.867056 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-30 19:33:55.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6956 2024-04-30 19:33:55.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      931 2024-04-30 19:33:55.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136370 2024-04-30 19:33:56.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)   136367 2024-04-30 19:33:56.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    39932 2024-04-30 19:34:00.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39932 2024-04-30 19:34:00.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    36115 2024-04-30 19:33:56.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    36083 2024-04-30 19:33:56.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-30 19:33:55.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)   526578 2024-04-30 19:34:09.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)   526578 2024-04-30 19:34:07.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-30 19:33:55.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-30 19:34:53.871056 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    17061 2024-04-30 19:34:53.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-30 19:34:53.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:53.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-30 19:34:53.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-04-30 19:34:53.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-30 19:34:53.000000 mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-30 19:34:53.871056 mypy_boto3_quicksight-1.34.95/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1995 2024-04-30 19:33:55.000000 mypy_boto3_quicksight-1.34.95/setup.py
```

### Comparing `mypy_boto3_quicksight-1.34.87/LICENSE` & `mypy_boto3_quicksight-1.34.95/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_quicksight-1.34.87/PKG-INFO` & `mypy_boto3_quicksight-1.34.95/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-quicksight
-Version: 1.34.87
-Summary: Type annotations for boto3.QuickSight 1.34.87 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.95
+Summary: Type annotations for boto3.QuickSight 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-quicksight)](https://pepy.tech/project/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-quicksight docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_quicksight-1.34.87/README.md` & `mypy_boto3_quicksight-1.34.95/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-quicksight)](https://pepy.tech/project/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-quicksight docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/__init__.py` & `mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/__init__.pyi` & `mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/client.py` & `mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     DataSourceTypeType,
     EditionType,
     EmbeddingIdentityTypeType,
     FolderTypeType,
     IdentityTypeType,
     IngestionTypeType,
     MemberTypeType,
+    PurchaseModeType,
     RoleType,
     SharingModelType,
     ThemeTypeType,
     UserRoleType,
 )
 from .paginator import (
     DescribeFolderPermissionsPaginator,
@@ -68,28 +69,28 @@
     SearchDataSetsPaginator,
     SearchDataSourcesPaginator,
     SearchFoldersPaginator,
     SearchGroupsPaginator,
 )
 from .type_defs import (
     AccountCustomizationTypeDef,
-    AnalysisDefinitionTypeDef,
+    AnalysisDefinitionUnionTypeDef,
     AnalysisSearchFilterTypeDef,
     AnalysisSourceEntityTypeDef,
     AnonymousUserEmbeddingExperienceConfigurationTypeDef,
-    AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
+    AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef,
     AssetBundleExportJobValidationStrategyTypeDef,
-    AssetBundleImportJobOverrideParametersTypeDef,
-    AssetBundleImportJobOverridePermissionsTypeDef,
-    AssetBundleImportJobOverrideTagsTypeDef,
+    AssetBundleImportJobOverrideParametersUnionTypeDef,
+    AssetBundleImportJobOverridePermissionsUnionTypeDef,
+    AssetBundleImportJobOverrideTagsUnionTypeDef,
     AssetBundleImportJobOverrideValidationStrategyTypeDef,
     AssetBundleImportSourceTypeDef,
     CancelIngestionResponseTypeDef,
-    ColumnGroupTypeDef,
-    ColumnLevelPermissionRuleTypeDef,
+    ColumnGroupUnionTypeDef,
+    ColumnLevelPermissionRuleUnionTypeDef,
     CreateAccountCustomizationResponseTypeDef,
     CreateAccountSubscriptionResponseTypeDef,
     CreateAnalysisResponseTypeDef,
     CreateDashboardResponseTypeDef,
     CreateDataSetResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateFolderMembershipResponseTypeDef,
@@ -107,21 +108,21 @@
     CreateThemeResponseTypeDef,
     CreateTopicRefreshScheduleResponseTypeDef,
     CreateTopicResponseTypeDef,
     CreateVPCConnectionResponseTypeDef,
     DashboardPublishOptionsTypeDef,
     DashboardSearchFilterTypeDef,
     DashboardSourceEntityTypeDef,
-    DashboardVersionDefinitionTypeDef,
-    DatasetParameterTypeDef,
+    DashboardVersionDefinitionUnionTypeDef,
+    DatasetParameterUnionTypeDef,
     DataSetRefreshPropertiesTypeDef,
     DataSetSearchFilterTypeDef,
     DataSetUsageConfigurationTypeDef,
     DataSourceCredentialsTypeDef,
-    DataSourceParametersTypeDef,
+    DataSourceParametersUnionTypeDef,
     DataSourceSearchFilterTypeDef,
     DeleteAccountCustomizationResponseTypeDef,
     DeleteAccountSubscriptionResponseTypeDef,
     DeleteAnalysisResponseTypeDef,
     DeleteDashboardResponseTypeDef,
     DeleteDataSetRefreshPropertiesResponseTypeDef,
     DeleteDataSetResponseTypeDef,
@@ -183,22 +184,22 @@
     DescribeThemeResponseTypeDef,
     DescribeTopicPermissionsResponseTypeDef,
     DescribeTopicRefreshResponseTypeDef,
     DescribeTopicRefreshScheduleResponseTypeDef,
     DescribeTopicResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeVPCConnectionResponseTypeDef,
-    FieldFolderTypeDef,
+    FieldFolderUnionTypeDef,
     FolderSearchFilterTypeDef,
     GenerateEmbedUrlForAnonymousUserResponseTypeDef,
     GenerateEmbedUrlForRegisteredUserResponseTypeDef,
     GetDashboardEmbedUrlResponseTypeDef,
     GetSessionEmbedUrlResponseTypeDef,
     GroupSearchFilterTypeDef,
-    LinkSharingConfigurationTypeDef,
+    LinkSharingConfigurationUnionTypeDef,
     ListAnalysesResponseTypeDef,
     ListAssetBundleExportJobsResponseTypeDef,
     ListAssetBundleImportJobsResponseTypeDef,
     ListDashboardsResponseTypeDef,
     ListDashboardVersionsResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDataSourcesResponseTypeDef,
@@ -221,45 +222,45 @@
     ListThemesResponseTypeDef,
     ListThemeVersionsResponseTypeDef,
     ListTopicRefreshSchedulesResponseTypeDef,
     ListTopicsResponseTypeDef,
     ListUserGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
     ListVPCConnectionsResponseTypeDef,
-    LogicalTableTypeDef,
-    ParametersTypeDef,
-    PhysicalTableTypeDef,
+    LogicalTableUnionTypeDef,
+    ParametersUnionTypeDef,
+    PhysicalTableUnionTypeDef,
     PutDataSetRefreshPropertiesResponseTypeDef,
-    RefreshScheduleTypeDef,
+    RefreshScheduleUnionTypeDef,
     RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     RegisterUserResponseTypeDef,
-    ResourcePermissionTypeDef,
+    ResourcePermissionUnionTypeDef,
     RestoreAnalysisResponseTypeDef,
     RowLevelPermissionDataSetTypeDef,
-    RowLevelPermissionTagConfigurationTypeDef,
+    RowLevelPermissionTagConfigurationUnionTypeDef,
     SearchAnalysesResponseTypeDef,
     SearchDashboardsResponseTypeDef,
     SearchDataSetsResponseTypeDef,
     SearchDataSourcesResponseTypeDef,
     SearchFoldersResponseTypeDef,
     SearchGroupsResponseTypeDef,
     SessionTagTypeDef,
-    SnapshotConfigurationTypeDef,
+    SnapshotConfigurationUnionTypeDef,
     SnapshotUserConfigurationTypeDef,
     SslPropertiesTypeDef,
     StartAssetBundleExportJobResponseTypeDef,
     StartAssetBundleImportJobResponseTypeDef,
     StartDashboardSnapshotJobResponseTypeDef,
     TagResourceResponseTypeDef,
     TagTypeDef,
     TemplateSourceEntityTypeDef,
-    TemplateVersionDefinitionTypeDef,
-    ThemeConfigurationTypeDef,
-    TopicDetailsTypeDef,
-    TopicRefreshScheduleTypeDef,
+    TemplateVersionDefinitionUnionTypeDef,
+    ThemeConfigurationUnionTypeDef,
+    TopicDetailsUnionTypeDef,
+    TopicRefreshScheduleUnionTypeDef,
     UntagResourceResponseTypeDef,
     UpdateAccountCustomizationResponseTypeDef,
     UpdateAccountSettingsResponseTypeDef,
     UpdateAnalysisPermissionsResponseTypeDef,
     UpdateAnalysisResponseTypeDef,
     UpdateDashboardLinksResponseTypeDef,
     UpdateDashboardPermissionsResponseTypeDef,
@@ -274,14 +275,15 @@
     UpdateGroupResponseTypeDef,
     UpdateIAMPolicyAssignmentResponseTypeDef,
     UpdateIdentityPropagationConfigResponseTypeDef,
     UpdateIpRestrictionResponseTypeDef,
     UpdatePublicSharingSettingsResponseTypeDef,
     UpdateRefreshScheduleResponseTypeDef,
     UpdateRoleCustomPermissionResponseTypeDef,
+    UpdateSPICECapacityConfigurationResponseTypeDef,
     UpdateTemplateAliasResponseTypeDef,
     UpdateTemplatePermissionsResponseTypeDef,
     UpdateTemplateResponseTypeDef,
     UpdateThemeAliasResponseTypeDef,
     UpdateThemePermissionsResponseTypeDef,
     UpdateThemeResponseTypeDef,
     UpdateTopicPermissionsResponseTypeDef,
@@ -390,25 +392,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_account_customization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_account_customization)
         """
 
     def create_account_subscription(
         self,
         *,
-        Edition: EditionType,
         AuthenticationMethod: AuthenticationMethodOptionType,
         AwsAccountId: str,
         AccountName: str,
         NotificationEmail: str,
+        Edition: EditionType = ...,
         ActiveDirectoryName: str = ...,
         Realm: str = ...,
         DirectoryId: str = ...,
         AdminGroup: Sequence[str] = ...,
         AuthorGroup: Sequence[str] = ...,
         ReaderGroup: Sequence[str] = ...,
+        AdminProGroup: Sequence[str] = ...,
+        AuthorProGroup: Sequence[str] = ...,
+        ReaderProGroup: Sequence[str] = ...,
         FirstName: str = ...,
         LastName: str = ...,
         EmailAddress: str = ...,
         ContactNumber: str = ...,
         IAMIdentityCenterInstanceArn: str = ...,
     ) -> CreateAccountSubscriptionResponseTypeDef:
         """
@@ -420,20 +425,20 @@
 
     def create_analysis(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         Name: str,
-        Parameters: ParametersTypeDef = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Parameters: ParametersUnionTypeDef = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Definition: AnalysisDefinitionTypeDef = ...,
+        Definition: AnalysisDefinitionUnionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
         FolderArns: Sequence[str] = ...,
     ) -> CreateAnalysisResponseTypeDef:
         """
         Creates an analysis in Amazon QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_analysis)
@@ -442,25 +447,25 @@
 
     def create_dashboard(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         Name: str,
-        Parameters: ParametersTypeDef = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Parameters: ParametersUnionTypeDef = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         SourceEntity: DashboardSourceEntityTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: DashboardVersionDefinitionTypeDef = ...,
+        Definition: DashboardVersionDefinitionUnionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
         FolderArns: Sequence[str] = ...,
-        LinkSharingConfiguration: LinkSharingConfigurationTypeDef = ...,
+        LinkSharingConfiguration: LinkSharingConfigurationUnionTypeDef = ...,
         LinkEntities: Sequence[str] = ...,
     ) -> CreateDashboardResponseTypeDef:
         """
         Creates a dashboard from either a template or directly with a
         `DashboardDefinition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_dashboard)
@@ -469,26 +474,26 @@
 
     def create_data_set(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
         Name: str,
-        PhysicalTableMap: Mapping[str, PhysicalTableTypeDef],
+        PhysicalTableMap: Mapping[str, PhysicalTableUnionTypeDef],
         ImportMode: DataSetImportModeType,
-        LogicalTableMap: Mapping[str, LogicalTableTypeDef] = ...,
-        ColumnGroups: Sequence[ColumnGroupTypeDef] = ...,
-        FieldFolders: Mapping[str, FieldFolderTypeDef] = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        LogicalTableMap: Mapping[str, LogicalTableUnionTypeDef] = ...,
+        ColumnGroups: Sequence[ColumnGroupUnionTypeDef] = ...,
+        FieldFolders: Mapping[str, FieldFolderUnionTypeDef] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
-        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationTypeDef = ...,
-        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleTypeDef] = ...,
+        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationUnionTypeDef = ...,
+        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
-        DatasetParameters: Sequence[DatasetParameterTypeDef] = ...,
+        DatasetParameters: Sequence[DatasetParameterUnionTypeDef] = ...,
         FolderArns: Sequence[str] = ...,
     ) -> CreateDataSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_data_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_data_set)
@@ -497,17 +502,17 @@
     def create_data_source(
         self,
         *,
         AwsAccountId: str,
         DataSourceId: str,
         Name: str,
         Type: DataSourceTypeType,
-        DataSourceParameters: DataSourceParametersTypeDef = ...,
+        DataSourceParameters: DataSourceParametersUnionTypeDef = ...,
         Credentials: DataSourceCredentialsTypeDef = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,
         SslProperties: SslPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FolderArns: Sequence[str] = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source.
@@ -520,15 +525,15 @@
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Name: str = ...,
         FolderType: FolderTypeType = ...,
         ParentFolderArn: str = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SharingModel: SharingModelType = ...,
     ) -> CreateFolderResponseTypeDef:
         """
         Creates an empty shared folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_folder)
@@ -612,15 +617,15 @@
         QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_namespace)
         """
 
     def create_refresh_schedule(
-        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleTypeDef
+        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleUnionTypeDef
     ) -> CreateRefreshScheduleResponseTypeDef:
         """
         Creates a refresh schedule for a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_refresh_schedule)
         """
@@ -639,19 +644,19 @@
 
     def create_template(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
         Name: str = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
-        Definition: TemplateVersionDefinitionTypeDef = ...,
+        Definition: TemplateVersionDefinitionUnionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates a template either from a `TemplateDefinition` or from an existing
         Amazon QuickSight analysis or
         template.
 
@@ -672,17 +677,17 @@
     def create_theme(
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         Name: str,
         BaseThemeId: str,
-        Configuration: ThemeConfigurationTypeDef,
+        Configuration: ThemeConfigurationUnionTypeDef,
         VersionDescription: str = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateThemeResponseTypeDef:
         """
         Creates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_theme)
@@ -699,15 +704,15 @@
         """
 
     def create_topic(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
-        Topic: TopicDetailsTypeDef,
+        Topic: TopicDetailsUnionTypeDef,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTopicResponseTypeDef:
         """
         Creates a new Q topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_topic)
@@ -715,15 +720,15 @@
 
     def create_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetArn: str,
-        RefreshSchedule: TopicRefreshScheduleTypeDef,
+        RefreshSchedule: TopicRefreshScheduleUnionTypeDef,
         DatasetName: str = ...,
     ) -> CreateTopicRefreshScheduleResponseTypeDef:
         """
         Creates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_topic_refresh_schedule)
@@ -2041,15 +2046,15 @@
         self,
         *,
         AwsAccountId: str,
         AssetBundleExportJobId: str,
         ResourceArns: Sequence[str],
         ExportFormat: AssetBundleExportFormatType,
         IncludeAllDependencies: bool = ...,
-        CloudFormationOverridePropertyConfiguration: AssetBundleCloudFormationOverridePropertyConfigurationTypeDef = ...,
+        CloudFormationOverridePropertyConfiguration: AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef = ...,
         IncludePermissions: bool = ...,
         IncludeTags: bool = ...,
         ValidationStrategy: AssetBundleExportJobValidationStrategyTypeDef = ...,
     ) -> StartAssetBundleExportJobResponseTypeDef:
         """
         Starts an Asset Bundle export job.
 
@@ -2059,18 +2064,18 @@
 
     def start_asset_bundle_import_job(
         self,
         *,
         AwsAccountId: str,
         AssetBundleImportJobId: str,
         AssetBundleImportSource: AssetBundleImportSourceTypeDef,
-        OverrideParameters: AssetBundleImportJobOverrideParametersTypeDef = ...,
+        OverrideParameters: AssetBundleImportJobOverrideParametersUnionTypeDef = ...,
         FailureAction: AssetBundleImportFailureActionType = ...,
-        OverridePermissions: AssetBundleImportJobOverridePermissionsTypeDef = ...,
-        OverrideTags: AssetBundleImportJobOverrideTagsTypeDef = ...,
+        OverridePermissions: AssetBundleImportJobOverridePermissionsUnionTypeDef = ...,
+        OverrideTags: AssetBundleImportJobOverrideTagsUnionTypeDef = ...,
         OverrideValidationStrategy: AssetBundleImportJobOverrideValidationStrategyTypeDef = ...,
     ) -> StartAssetBundleImportJobResponseTypeDef:
         """
         Starts an Asset Bundle import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_asset_bundle_import_job)
@@ -2079,15 +2084,15 @@
     def start_dashboard_snapshot_job(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         SnapshotJobId: str,
         UserConfiguration: SnapshotUserConfigurationTypeDef,
-        SnapshotConfiguration: SnapshotConfigurationTypeDef,
+        SnapshotConfiguration: SnapshotConfigurationUnionTypeDef,
     ) -> StartDashboardSnapshotJobResponseTypeDef:
         """
         Starts an asynchronous job that generates a snapshot of a dashboard's output.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_dashboard_snapshot_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_dashboard_snapshot_job)
         """
@@ -2145,18 +2150,18 @@
 
     def update_analysis(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         Name: str,
-        Parameters: ParametersTypeDef = ...,
+        Parameters: ParametersUnionTypeDef = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: AnalysisDefinitionTypeDef = ...,
+        Definition: AnalysisDefinitionUnionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> UpdateAnalysisResponseTypeDef:
         """
         Updates an analysis in Amazon QuickSight See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/quicksight-2018-04-01/UpdateAnalysis).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis)
@@ -2164,16 +2169,16 @@
         """
 
     def update_analysis_permissions(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateAnalysisPermissionsResponseTypeDef:
         """
         Updates the read and write permissions for an analysis.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_analysis_permissions)
         """
@@ -2181,19 +2186,19 @@
     def update_dashboard(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         Name: str,
         SourceEntity: DashboardSourceEntityTypeDef = ...,
-        Parameters: ParametersTypeDef = ...,
+        Parameters: ParametersUnionTypeDef = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: DashboardVersionDefinitionTypeDef = ...,
+        Definition: DashboardVersionDefinitionUnionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> UpdateDashboardResponseTypeDef:
         """
         Updates a dashboard in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_dashboard)
@@ -2210,18 +2215,18 @@
         """
 
     def update_dashboard_permissions(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        GrantLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokeLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        GrantLinkPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokeLinkPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateDashboardPermissionsResponseTypeDef:
         """
         Updates read and write permissions on a dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_dashboard_permissions)
         """
@@ -2238,54 +2243,54 @@
 
     def update_data_set(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
         Name: str,
-        PhysicalTableMap: Mapping[str, PhysicalTableTypeDef],
+        PhysicalTableMap: Mapping[str, PhysicalTableUnionTypeDef],
         ImportMode: DataSetImportModeType,
-        LogicalTableMap: Mapping[str, LogicalTableTypeDef] = ...,
-        ColumnGroups: Sequence[ColumnGroupTypeDef] = ...,
-        FieldFolders: Mapping[str, FieldFolderTypeDef] = ...,
+        LogicalTableMap: Mapping[str, LogicalTableUnionTypeDef] = ...,
+        ColumnGroups: Sequence[ColumnGroupUnionTypeDef] = ...,
+        FieldFolders: Mapping[str, FieldFolderUnionTypeDef] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
-        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationTypeDef = ...,
-        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleTypeDef] = ...,
+        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationUnionTypeDef = ...,
+        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleUnionTypeDef] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
-        DatasetParameters: Sequence[DatasetParameterTypeDef] = ...,
+        DatasetParameters: Sequence[DatasetParameterUnionTypeDef] = ...,
     ) -> UpdateDataSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_set)
         """
 
     def update_data_set_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateDataSetPermissionsResponseTypeDef:
         """
         Updates the permissions on a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_set_permissions)
         """
 
     def update_data_source(
         self,
         *,
         AwsAccountId: str,
         DataSourceId: str,
         Name: str,
-        DataSourceParameters: DataSourceParametersTypeDef = ...,
+        DataSourceParameters: DataSourceParametersUnionTypeDef = ...,
         Credentials: DataSourceCredentialsTypeDef = ...,
         VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,
         SslProperties: SslPropertiesTypeDef = ...,
     ) -> UpdateDataSourceResponseTypeDef:
         """
         Updates a data source.
 
@@ -2294,16 +2299,16 @@
         """
 
     def update_data_source_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSourceId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateDataSourcePermissionsResponseTypeDef:
         """
         Updates the permissions to a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_source_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_source_permissions)
         """
@@ -2319,16 +2324,16 @@
         """
 
     def update_folder_permissions(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateFolderPermissionsResponseTypeDef:
         """
         Updates permissions of a folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_folder_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_folder_permissions)
         """
@@ -2401,15 +2406,15 @@
         dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_public_sharing_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_public_sharing_settings)
         """
 
     def update_refresh_schedule(
-        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleTypeDef
+        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleUnionTypeDef
     ) -> UpdateRefreshScheduleResponseTypeDef:
         """
         Updates a refresh schedule for a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_refresh_schedule)
         """
@@ -2420,23 +2425,33 @@
         """
         Updates the custom permissions that are associated with a role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_role_custom_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_role_custom_permission)
         """
 
+    def update_spice_capacity_configuration(
+        self, *, AwsAccountId: str, PurchaseMode: PurchaseModeType
+    ) -> UpdateSPICECapacityConfigurationResponseTypeDef:
+        """
+        Updates the SPICE capacity configuration for a Amazon QuickSight account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_spice_capacity_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_spice_capacity_configuration)
+        """
+
     def update_template(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         VersionDescription: str = ...,
         Name: str = ...,
-        Definition: TemplateVersionDefinitionTypeDef = ...,
+        Definition: TemplateVersionDefinitionUnionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> UpdateTemplateResponseTypeDef:
         """
         Updates a template from an existing Amazon QuickSight analysis or another
         template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template)
@@ -2454,16 +2469,16 @@
         """
 
     def update_template_permissions(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateTemplatePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_template_permissions)
         """
@@ -2472,15 +2487,15 @@
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         BaseThemeId: str,
         Name: str = ...,
         VersionDescription: str = ...,
-        Configuration: ThemeConfigurationTypeDef = ...,
+        Configuration: ThemeConfigurationUnionTypeDef = ...,
     ) -> UpdateThemeResponseTypeDef:
         """
         Updates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_theme)
         """
@@ -2496,56 +2511,56 @@
         """
 
     def update_theme_permissions(
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateThemePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_theme_permissions)
         """
 
     def update_topic(
-        self, *, AwsAccountId: str, TopicId: str, Topic: TopicDetailsTypeDef
+        self, *, AwsAccountId: str, TopicId: str, Topic: TopicDetailsUnionTypeDef
     ) -> UpdateTopicResponseTypeDef:
         """
         Updates a topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic)
         """
 
     def update_topic_permissions(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateTopicPermissionsResponseTypeDef:
         """
         Updates the permissions of a topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic_permissions)
         """
 
     def update_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetId: str,
-        RefreshSchedule: TopicRefreshScheduleTypeDef,
+        RefreshSchedule: TopicRefreshScheduleUnionTypeDef,
     ) -> UpdateTopicRefreshScheduleResponseTypeDef:
         """
         Updates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic_refresh_schedule)
         """
```

### Comparing `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/client.pyi` & `mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/client.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
     DataSourceTypeType,
     EditionType,
     EmbeddingIdentityTypeType,
     FolderTypeType,
     IdentityTypeType,
     IngestionTypeType,
     MemberTypeType,
+    PurchaseModeType,
     RoleType,
     SharingModelType,
     ThemeTypeType,
     UserRoleType,
 )
 from .paginator import (
     DescribeFolderPermissionsPaginator,
@@ -68,28 +69,28 @@
     SearchDataSetsPaginator,
     SearchDataSourcesPaginator,
     SearchFoldersPaginator,
     SearchGroupsPaginator,
 )
 from .type_defs import (
     AccountCustomizationTypeDef,
-    AnalysisDefinitionTypeDef,
+    AnalysisDefinitionUnionTypeDef,
     AnalysisSearchFilterTypeDef,
     AnalysisSourceEntityTypeDef,
     AnonymousUserEmbeddingExperienceConfigurationTypeDef,
-    AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
+    AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef,
     AssetBundleExportJobValidationStrategyTypeDef,
-    AssetBundleImportJobOverrideParametersTypeDef,
-    AssetBundleImportJobOverridePermissionsTypeDef,
-    AssetBundleImportJobOverrideTagsTypeDef,
+    AssetBundleImportJobOverrideParametersUnionTypeDef,
+    AssetBundleImportJobOverridePermissionsUnionTypeDef,
+    AssetBundleImportJobOverrideTagsUnionTypeDef,
     AssetBundleImportJobOverrideValidationStrategyTypeDef,
     AssetBundleImportSourceTypeDef,
     CancelIngestionResponseTypeDef,
-    ColumnGroupTypeDef,
-    ColumnLevelPermissionRuleTypeDef,
+    ColumnGroupUnionTypeDef,
+    ColumnLevelPermissionRuleUnionTypeDef,
     CreateAccountCustomizationResponseTypeDef,
     CreateAccountSubscriptionResponseTypeDef,
     CreateAnalysisResponseTypeDef,
     CreateDashboardResponseTypeDef,
     CreateDataSetResponseTypeDef,
     CreateDataSourceResponseTypeDef,
     CreateFolderMembershipResponseTypeDef,
@@ -107,21 +108,21 @@
     CreateThemeResponseTypeDef,
     CreateTopicRefreshScheduleResponseTypeDef,
     CreateTopicResponseTypeDef,
     CreateVPCConnectionResponseTypeDef,
     DashboardPublishOptionsTypeDef,
     DashboardSearchFilterTypeDef,
     DashboardSourceEntityTypeDef,
-    DashboardVersionDefinitionTypeDef,
-    DatasetParameterTypeDef,
+    DashboardVersionDefinitionUnionTypeDef,
+    DatasetParameterUnionTypeDef,
     DataSetRefreshPropertiesTypeDef,
     DataSetSearchFilterTypeDef,
     DataSetUsageConfigurationTypeDef,
     DataSourceCredentialsTypeDef,
-    DataSourceParametersTypeDef,
+    DataSourceParametersUnionTypeDef,
     DataSourceSearchFilterTypeDef,
     DeleteAccountCustomizationResponseTypeDef,
     DeleteAccountSubscriptionResponseTypeDef,
     DeleteAnalysisResponseTypeDef,
     DeleteDashboardResponseTypeDef,
     DeleteDataSetRefreshPropertiesResponseTypeDef,
     DeleteDataSetResponseTypeDef,
@@ -183,22 +184,22 @@
     DescribeThemeResponseTypeDef,
     DescribeTopicPermissionsResponseTypeDef,
     DescribeTopicRefreshResponseTypeDef,
     DescribeTopicRefreshScheduleResponseTypeDef,
     DescribeTopicResponseTypeDef,
     DescribeUserResponseTypeDef,
     DescribeVPCConnectionResponseTypeDef,
-    FieldFolderTypeDef,
+    FieldFolderUnionTypeDef,
     FolderSearchFilterTypeDef,
     GenerateEmbedUrlForAnonymousUserResponseTypeDef,
     GenerateEmbedUrlForRegisteredUserResponseTypeDef,
     GetDashboardEmbedUrlResponseTypeDef,
     GetSessionEmbedUrlResponseTypeDef,
     GroupSearchFilterTypeDef,
-    LinkSharingConfigurationTypeDef,
+    LinkSharingConfigurationUnionTypeDef,
     ListAnalysesResponseTypeDef,
     ListAssetBundleExportJobsResponseTypeDef,
     ListAssetBundleImportJobsResponseTypeDef,
     ListDashboardsResponseTypeDef,
     ListDashboardVersionsResponseTypeDef,
     ListDataSetsResponseTypeDef,
     ListDataSourcesResponseTypeDef,
@@ -221,45 +222,45 @@
     ListThemesResponseTypeDef,
     ListThemeVersionsResponseTypeDef,
     ListTopicRefreshSchedulesResponseTypeDef,
     ListTopicsResponseTypeDef,
     ListUserGroupsResponseTypeDef,
     ListUsersResponseTypeDef,
     ListVPCConnectionsResponseTypeDef,
-    LogicalTableTypeDef,
-    ParametersTypeDef,
-    PhysicalTableTypeDef,
+    LogicalTableUnionTypeDef,
+    ParametersUnionTypeDef,
+    PhysicalTableUnionTypeDef,
     PutDataSetRefreshPropertiesResponseTypeDef,
-    RefreshScheduleTypeDef,
+    RefreshScheduleUnionTypeDef,
     RegisteredUserEmbeddingExperienceConfigurationTypeDef,
     RegisterUserResponseTypeDef,
-    ResourcePermissionTypeDef,
+    ResourcePermissionUnionTypeDef,
     RestoreAnalysisResponseTypeDef,
     RowLevelPermissionDataSetTypeDef,
-    RowLevelPermissionTagConfigurationTypeDef,
+    RowLevelPermissionTagConfigurationUnionTypeDef,
     SearchAnalysesResponseTypeDef,
     SearchDashboardsResponseTypeDef,
     SearchDataSetsResponseTypeDef,
     SearchDataSourcesResponseTypeDef,
     SearchFoldersResponseTypeDef,
     SearchGroupsResponseTypeDef,
     SessionTagTypeDef,
-    SnapshotConfigurationTypeDef,
+    SnapshotConfigurationUnionTypeDef,
     SnapshotUserConfigurationTypeDef,
     SslPropertiesTypeDef,
     StartAssetBundleExportJobResponseTypeDef,
     StartAssetBundleImportJobResponseTypeDef,
     StartDashboardSnapshotJobResponseTypeDef,
     TagResourceResponseTypeDef,
     TagTypeDef,
     TemplateSourceEntityTypeDef,
-    TemplateVersionDefinitionTypeDef,
-    ThemeConfigurationTypeDef,
-    TopicDetailsTypeDef,
-    TopicRefreshScheduleTypeDef,
+    TemplateVersionDefinitionUnionTypeDef,
+    ThemeConfigurationUnionTypeDef,
+    TopicDetailsUnionTypeDef,
+    TopicRefreshScheduleUnionTypeDef,
     UntagResourceResponseTypeDef,
     UpdateAccountCustomizationResponseTypeDef,
     UpdateAccountSettingsResponseTypeDef,
     UpdateAnalysisPermissionsResponseTypeDef,
     UpdateAnalysisResponseTypeDef,
     UpdateDashboardLinksResponseTypeDef,
     UpdateDashboardPermissionsResponseTypeDef,
@@ -274,14 +275,15 @@
     UpdateGroupResponseTypeDef,
     UpdateIAMPolicyAssignmentResponseTypeDef,
     UpdateIdentityPropagationConfigResponseTypeDef,
     UpdateIpRestrictionResponseTypeDef,
     UpdatePublicSharingSettingsResponseTypeDef,
     UpdateRefreshScheduleResponseTypeDef,
     UpdateRoleCustomPermissionResponseTypeDef,
+    UpdateSPICECapacityConfigurationResponseTypeDef,
     UpdateTemplateAliasResponseTypeDef,
     UpdateTemplatePermissionsResponseTypeDef,
     UpdateTemplateResponseTypeDef,
     UpdateThemeAliasResponseTypeDef,
     UpdateThemePermissionsResponseTypeDef,
     UpdateThemeResponseTypeDef,
     UpdateTopicPermissionsResponseTypeDef,
@@ -387,25 +389,28 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_account_customization)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_account_customization)
         """
 
     def create_account_subscription(
         self,
         *,
-        Edition: EditionType,
         AuthenticationMethod: AuthenticationMethodOptionType,
         AwsAccountId: str,
         AccountName: str,
         NotificationEmail: str,
+        Edition: EditionType = ...,
         ActiveDirectoryName: str = ...,
         Realm: str = ...,
         DirectoryId: str = ...,
         AdminGroup: Sequence[str] = ...,
         AuthorGroup: Sequence[str] = ...,
         ReaderGroup: Sequence[str] = ...,
+        AdminProGroup: Sequence[str] = ...,
+        AuthorProGroup: Sequence[str] = ...,
+        ReaderProGroup: Sequence[str] = ...,
         FirstName: str = ...,
         LastName: str = ...,
         EmailAddress: str = ...,
         ContactNumber: str = ...,
         IAMIdentityCenterInstanceArn: str = ...,
     ) -> CreateAccountSubscriptionResponseTypeDef:
         """
@@ -417,20 +422,20 @@
 
     def create_analysis(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         Name: str,
-        Parameters: ParametersTypeDef = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Parameters: ParametersUnionTypeDef = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
         Tags: Sequence[TagTypeDef] = ...,
-        Definition: AnalysisDefinitionTypeDef = ...,
+        Definition: AnalysisDefinitionUnionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
         FolderArns: Sequence[str] = ...,
     ) -> CreateAnalysisResponseTypeDef:
         """
         Creates an analysis in Amazon QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_analysis)
@@ -439,25 +444,25 @@
 
     def create_dashboard(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         Name: str,
-        Parameters: ParametersTypeDef = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Parameters: ParametersUnionTypeDef = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         SourceEntity: DashboardSourceEntityTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: DashboardVersionDefinitionTypeDef = ...,
+        Definition: DashboardVersionDefinitionUnionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
         FolderArns: Sequence[str] = ...,
-        LinkSharingConfiguration: LinkSharingConfigurationTypeDef = ...,
+        LinkSharingConfiguration: LinkSharingConfigurationUnionTypeDef = ...,
         LinkEntities: Sequence[str] = ...,
     ) -> CreateDashboardResponseTypeDef:
         """
         Creates a dashboard from either a template or directly with a
         `DashboardDefinition`.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_dashboard)
@@ -466,26 +471,26 @@
 
     def create_data_set(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
         Name: str,
-        PhysicalTableMap: Mapping[str, PhysicalTableTypeDef],
+        PhysicalTableMap: Mapping[str, PhysicalTableUnionTypeDef],
         ImportMode: DataSetImportModeType,
-        LogicalTableMap: Mapping[str, LogicalTableTypeDef] = ...,
-        ColumnGroups: Sequence[ColumnGroupTypeDef] = ...,
-        FieldFolders: Mapping[str, FieldFolderTypeDef] = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        LogicalTableMap: Mapping[str, LogicalTableUnionTypeDef] = ...,
+        ColumnGroups: Sequence[ColumnGroupUnionTypeDef] = ...,
+        FieldFolders: Mapping[str, FieldFolderUnionTypeDef] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
-        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationTypeDef = ...,
-        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleTypeDef] = ...,
+        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationUnionTypeDef = ...,
+        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
-        DatasetParameters: Sequence[DatasetParameterTypeDef] = ...,
+        DatasetParameters: Sequence[DatasetParameterUnionTypeDef] = ...,
         FolderArns: Sequence[str] = ...,
     ) -> CreateDataSetResponseTypeDef:
         """
         Creates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_data_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_data_set)
@@ -494,17 +499,17 @@
     def create_data_source(
         self,
         *,
         AwsAccountId: str,
         DataSourceId: str,
         Name: str,
         Type: DataSourceTypeType,
-        DataSourceParameters: DataSourceParametersTypeDef = ...,
+        DataSourceParameters: DataSourceParametersUnionTypeDef = ...,
         Credentials: DataSourceCredentialsTypeDef = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,
         SslProperties: SslPropertiesTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         FolderArns: Sequence[str] = ...,
     ) -> CreateDataSourceResponseTypeDef:
         """
         Creates a data source.
@@ -517,15 +522,15 @@
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Name: str = ...,
         FolderType: FolderTypeType = ...,
         ParentFolderArn: str = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
         SharingModel: SharingModelType = ...,
     ) -> CreateFolderResponseTypeDef:
         """
         Creates an empty shared folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_folder)
@@ -609,15 +614,15 @@
         QuickSight.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_namespace)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_namespace)
         """
 
     def create_refresh_schedule(
-        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleTypeDef
+        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleUnionTypeDef
     ) -> CreateRefreshScheduleResponseTypeDef:
         """
         Creates a refresh schedule for a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_refresh_schedule)
         """
@@ -636,19 +641,19 @@
 
     def create_template(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
         Name: str = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         Tags: Sequence[TagTypeDef] = ...,
         VersionDescription: str = ...,
-        Definition: TemplateVersionDefinitionTypeDef = ...,
+        Definition: TemplateVersionDefinitionUnionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> CreateTemplateResponseTypeDef:
         """
         Creates a template either from a `TemplateDefinition` or from an existing
         Amazon QuickSight analysis or
         template.
 
@@ -669,17 +674,17 @@
     def create_theme(
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         Name: str,
         BaseThemeId: str,
-        Configuration: ThemeConfigurationTypeDef,
+        Configuration: ThemeConfigurationUnionTypeDef,
         VersionDescription: str = ...,
-        Permissions: Sequence[ResourcePermissionTypeDef] = ...,
+        Permissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateThemeResponseTypeDef:
         """
         Creates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_theme)
@@ -696,15 +701,15 @@
         """
 
     def create_topic(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
-        Topic: TopicDetailsTypeDef,
+        Topic: TopicDetailsUnionTypeDef,
         Tags: Sequence[TagTypeDef] = ...,
     ) -> CreateTopicResponseTypeDef:
         """
         Creates a new Q topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_topic)
@@ -712,15 +717,15 @@
 
     def create_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetArn: str,
-        RefreshSchedule: TopicRefreshScheduleTypeDef,
+        RefreshSchedule: TopicRefreshScheduleUnionTypeDef,
         DatasetName: str = ...,
     ) -> CreateTopicRefreshScheduleResponseTypeDef:
         """
         Creates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.create_topic_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#create_topic_refresh_schedule)
@@ -2038,15 +2043,15 @@
         self,
         *,
         AwsAccountId: str,
         AssetBundleExportJobId: str,
         ResourceArns: Sequence[str],
         ExportFormat: AssetBundleExportFormatType,
         IncludeAllDependencies: bool = ...,
-        CloudFormationOverridePropertyConfiguration: AssetBundleCloudFormationOverridePropertyConfigurationTypeDef = ...,
+        CloudFormationOverridePropertyConfiguration: AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef = ...,
         IncludePermissions: bool = ...,
         IncludeTags: bool = ...,
         ValidationStrategy: AssetBundleExportJobValidationStrategyTypeDef = ...,
     ) -> StartAssetBundleExportJobResponseTypeDef:
         """
         Starts an Asset Bundle export job.
 
@@ -2056,18 +2061,18 @@
 
     def start_asset_bundle_import_job(
         self,
         *,
         AwsAccountId: str,
         AssetBundleImportJobId: str,
         AssetBundleImportSource: AssetBundleImportSourceTypeDef,
-        OverrideParameters: AssetBundleImportJobOverrideParametersTypeDef = ...,
+        OverrideParameters: AssetBundleImportJobOverrideParametersUnionTypeDef = ...,
         FailureAction: AssetBundleImportFailureActionType = ...,
-        OverridePermissions: AssetBundleImportJobOverridePermissionsTypeDef = ...,
-        OverrideTags: AssetBundleImportJobOverrideTagsTypeDef = ...,
+        OverridePermissions: AssetBundleImportJobOverridePermissionsUnionTypeDef = ...,
+        OverrideTags: AssetBundleImportJobOverrideTagsUnionTypeDef = ...,
         OverrideValidationStrategy: AssetBundleImportJobOverrideValidationStrategyTypeDef = ...,
     ) -> StartAssetBundleImportJobResponseTypeDef:
         """
         Starts an Asset Bundle import job.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_asset_bundle_import_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_asset_bundle_import_job)
@@ -2076,15 +2081,15 @@
     def start_dashboard_snapshot_job(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         SnapshotJobId: str,
         UserConfiguration: SnapshotUserConfigurationTypeDef,
-        SnapshotConfiguration: SnapshotConfigurationTypeDef,
+        SnapshotConfiguration: SnapshotConfigurationUnionTypeDef,
     ) -> StartDashboardSnapshotJobResponseTypeDef:
         """
         Starts an asynchronous job that generates a snapshot of a dashboard's output.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.start_dashboard_snapshot_job)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#start_dashboard_snapshot_job)
         """
@@ -2142,18 +2147,18 @@
 
     def update_analysis(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
         Name: str,
-        Parameters: ParametersTypeDef = ...,
+        Parameters: ParametersUnionTypeDef = ...,
         SourceEntity: AnalysisSourceEntityTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: AnalysisDefinitionTypeDef = ...,
+        Definition: AnalysisDefinitionUnionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> UpdateAnalysisResponseTypeDef:
         """
         Updates an analysis in Amazon QuickSight See also: [AWS API
         Documentation](https://docs.aws.amazon.com/goto/WebAPI/quicksight-2018-04-01/UpdateAnalysis).
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis)
@@ -2161,16 +2166,16 @@
         """
 
     def update_analysis_permissions(
         self,
         *,
         AwsAccountId: str,
         AnalysisId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateAnalysisPermissionsResponseTypeDef:
         """
         Updates the read and write permissions for an analysis.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_analysis_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_analysis_permissions)
         """
@@ -2178,19 +2183,19 @@
     def update_dashboard(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
         Name: str,
         SourceEntity: DashboardSourceEntityTypeDef = ...,
-        Parameters: ParametersTypeDef = ...,
+        Parameters: ParametersUnionTypeDef = ...,
         VersionDescription: str = ...,
         DashboardPublishOptions: DashboardPublishOptionsTypeDef = ...,
         ThemeArn: str = ...,
-        Definition: DashboardVersionDefinitionTypeDef = ...,
+        Definition: DashboardVersionDefinitionUnionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> UpdateDashboardResponseTypeDef:
         """
         Updates a dashboard in an Amazon Web Services account.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_dashboard)
@@ -2207,18 +2212,18 @@
         """
 
     def update_dashboard_permissions(
         self,
         *,
         AwsAccountId: str,
         DashboardId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        GrantLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokeLinkPermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        GrantLinkPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokeLinkPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateDashboardPermissionsResponseTypeDef:
         """
         Updates read and write permissions on a dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_dashboard_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_dashboard_permissions)
         """
@@ -2235,54 +2240,54 @@
 
     def update_data_set(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
         Name: str,
-        PhysicalTableMap: Mapping[str, PhysicalTableTypeDef],
+        PhysicalTableMap: Mapping[str, PhysicalTableUnionTypeDef],
         ImportMode: DataSetImportModeType,
-        LogicalTableMap: Mapping[str, LogicalTableTypeDef] = ...,
-        ColumnGroups: Sequence[ColumnGroupTypeDef] = ...,
-        FieldFolders: Mapping[str, FieldFolderTypeDef] = ...,
+        LogicalTableMap: Mapping[str, LogicalTableUnionTypeDef] = ...,
+        ColumnGroups: Sequence[ColumnGroupUnionTypeDef] = ...,
+        FieldFolders: Mapping[str, FieldFolderUnionTypeDef] = ...,
         RowLevelPermissionDataSet: RowLevelPermissionDataSetTypeDef = ...,
-        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationTypeDef = ...,
-        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleTypeDef] = ...,
+        RowLevelPermissionTagConfiguration: RowLevelPermissionTagConfigurationUnionTypeDef = ...,
+        ColumnLevelPermissionRules: Sequence[ColumnLevelPermissionRuleUnionTypeDef] = ...,
         DataSetUsageConfiguration: DataSetUsageConfigurationTypeDef = ...,
-        DatasetParameters: Sequence[DatasetParameterTypeDef] = ...,
+        DatasetParameters: Sequence[DatasetParameterUnionTypeDef] = ...,
     ) -> UpdateDataSetResponseTypeDef:
         """
         Updates a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_set)
         """
 
     def update_data_set_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSetId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateDataSetPermissionsResponseTypeDef:
         """
         Updates the permissions on a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_set_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_set_permissions)
         """
 
     def update_data_source(
         self,
         *,
         AwsAccountId: str,
         DataSourceId: str,
         Name: str,
-        DataSourceParameters: DataSourceParametersTypeDef = ...,
+        DataSourceParameters: DataSourceParametersUnionTypeDef = ...,
         Credentials: DataSourceCredentialsTypeDef = ...,
         VpcConnectionProperties: VpcConnectionPropertiesTypeDef = ...,
         SslProperties: SslPropertiesTypeDef = ...,
     ) -> UpdateDataSourceResponseTypeDef:
         """
         Updates a data source.
 
@@ -2291,16 +2296,16 @@
         """
 
     def update_data_source_permissions(
         self,
         *,
         AwsAccountId: str,
         DataSourceId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateDataSourcePermissionsResponseTypeDef:
         """
         Updates the permissions to a data source.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_data_source_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_data_source_permissions)
         """
@@ -2316,16 +2321,16 @@
         """
 
     def update_folder_permissions(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateFolderPermissionsResponseTypeDef:
         """
         Updates permissions of a folder.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_folder_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_folder_permissions)
         """
@@ -2398,15 +2403,15 @@
         dashboard.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_public_sharing_settings)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_public_sharing_settings)
         """
 
     def update_refresh_schedule(
-        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleTypeDef
+        self, *, DataSetId: str, AwsAccountId: str, Schedule: RefreshScheduleUnionTypeDef
     ) -> UpdateRefreshScheduleResponseTypeDef:
         """
         Updates a refresh schedule for a dataset.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_refresh_schedule)
         """
@@ -2417,23 +2422,33 @@
         """
         Updates the custom permissions that are associated with a role.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_role_custom_permission)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_role_custom_permission)
         """
 
+    def update_spice_capacity_configuration(
+        self, *, AwsAccountId: str, PurchaseMode: PurchaseModeType
+    ) -> UpdateSPICECapacityConfigurationResponseTypeDef:
+        """
+        Updates the SPICE capacity configuration for a Amazon QuickSight account.
+
+        [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_spice_capacity_configuration)
+        [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_spice_capacity_configuration)
+        """
+
     def update_template(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
         SourceEntity: TemplateSourceEntityTypeDef = ...,
         VersionDescription: str = ...,
         Name: str = ...,
-        Definition: TemplateVersionDefinitionTypeDef = ...,
+        Definition: TemplateVersionDefinitionUnionTypeDef = ...,
         ValidationStrategy: ValidationStrategyTypeDef = ...,
     ) -> UpdateTemplateResponseTypeDef:
         """
         Updates a template from an existing Amazon QuickSight analysis or another
         template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template)
@@ -2451,16 +2466,16 @@
         """
 
     def update_template_permissions(
         self,
         *,
         AwsAccountId: str,
         TemplateId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateTemplatePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a template.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_template_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_template_permissions)
         """
@@ -2469,15 +2484,15 @@
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
         BaseThemeId: str,
         Name: str = ...,
         VersionDescription: str = ...,
-        Configuration: ThemeConfigurationTypeDef = ...,
+        Configuration: ThemeConfigurationUnionTypeDef = ...,
     ) -> UpdateThemeResponseTypeDef:
         """
         Updates a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_theme)
         """
@@ -2493,56 +2508,56 @@
         """
 
     def update_theme_permissions(
         self,
         *,
         AwsAccountId: str,
         ThemeId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateThemePermissionsResponseTypeDef:
         """
         Updates the resource permissions for a theme.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_theme_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_theme_permissions)
         """
 
     def update_topic(
-        self, *, AwsAccountId: str, TopicId: str, Topic: TopicDetailsTypeDef
+        self, *, AwsAccountId: str, TopicId: str, Topic: TopicDetailsUnionTypeDef
     ) -> UpdateTopicResponseTypeDef:
         """
         Updates a topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic)
         """
 
     def update_topic_permissions(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
-        GrantPermissions: Sequence[ResourcePermissionTypeDef] = ...,
-        RevokePermissions: Sequence[ResourcePermissionTypeDef] = ...,
+        GrantPermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
+        RevokePermissions: Sequence[ResourcePermissionUnionTypeDef] = ...,
     ) -> UpdateTopicPermissionsResponseTypeDef:
         """
         Updates the permissions of a topic.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_permissions)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic_permissions)
         """
 
     def update_topic_refresh_schedule(
         self,
         *,
         AwsAccountId: str,
         TopicId: str,
         DatasetId: str,
-        RefreshSchedule: TopicRefreshScheduleTypeDef,
+        RefreshSchedule: TopicRefreshScheduleUnionTypeDef,
     ) -> UpdateTopicRefreshScheduleResponseTypeDef:
         """
         Updates a topic refresh schedule.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Client.update_topic_refresh_schedule)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/client/#update_topic_refresh_schedule)
         """
```

### Comparing `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/literals.py` & `mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,15 @@
     "PivotTableFieldCollapseStateType",
     "PivotTableMetricPlacementType",
     "PivotTableRowsLayoutType",
     "PivotTableSubtotalLevelType",
     "PrimaryValueDisplayTypeType",
     "PropertyRoleType",
     "PropertyUsageType",
+    "PurchaseModeType",
     "RadarChartAxesRangeScaleType",
     "RadarChartShapeType",
     "ReferenceLineLabelHorizontalPositionType",
     "ReferenceLineLabelVerticalPositionType",
     "ReferenceLinePatternTypeType",
     "ReferenceLineSeriesTypeType",
     "ReferenceLineValueLabelRelativePositionType",
@@ -740,14 +741,15 @@
 PivotTableFieldCollapseStateType = Literal["COLLAPSED", "EXPANDED"]
 PivotTableMetricPlacementType = Literal["COLUMN", "ROW"]
 PivotTableRowsLayoutType = Literal["HIERARCHY", "TABULAR"]
 PivotTableSubtotalLevelType = Literal["ALL", "CUSTOM", "LAST"]
 PrimaryValueDisplayTypeType = Literal["ACTUAL", "COMPARISON", "HIDDEN"]
 PropertyRoleType = Literal["ID", "PRIMARY"]
 PropertyUsageType = Literal["DIMENSION", "INHERIT", "MEASURE"]
+PurchaseModeType = Literal["AUTO_PURCHASE", "MANUAL"]
 RadarChartAxesRangeScaleType = Literal["AUTO", "INDEPENDENT", "SHARED"]
 RadarChartShapeType = Literal["CIRCLE", "POLYGON"]
 ReferenceLineLabelHorizontalPositionType = Literal["CENTER", "LEFT", "RIGHT"]
 ReferenceLineLabelVerticalPositionType = Literal["ABOVE", "BELOW"]
 ReferenceLinePatternTypeType = Literal["DASHED", "DOTTED", "SOLID"]
 ReferenceLineSeriesTypeType = Literal["BAR", "LINE"]
 ReferenceLineValueLabelRelativePositionType = Literal["AFTER_CUSTOM_LABEL", "BEFORE_CUSTOM_LABEL"]
@@ -760,15 +762,15 @@
     "CREATION_IN_PROGRESS",
     "CREATION_SUCCESSFUL",
     "DELETED",
     "UPDATE_FAILED",
     "UPDATE_IN_PROGRESS",
     "UPDATE_SUCCESSFUL",
 ]
-RoleType = Literal["ADMIN", "AUTHOR", "READER"]
+RoleType = Literal["ADMIN", "ADMIN_PRO", "AUTHOR", "AUTHOR_PRO", "READER", "READER_PRO"]
 RowLevelPermissionFormatVersionType = Literal["VERSION_1", "VERSION_2"]
 RowLevelPermissionPolicyType = Literal["DENY_ACCESS", "GRANT_ACCESS"]
 SearchAnalysesPaginatorName = Literal["search_analyses"]
 SearchDashboardsPaginatorName = Literal["search_dashboards"]
 SearchDataSetsPaginatorName = Literal["search_data_sets"]
 SearchDataSourcesPaginatorName = Literal["search_data_sources"]
 SearchFoldersPaginatorName = Literal["search_folders"]
@@ -838,15 +840,24 @@
 TopicScheduleTypeType = Literal["DAILY", "HOURLY", "MONTHLY", "WEEKLY"]
 TopicTimeGranularityType = Literal[
     "DAY", "HOUR", "MINUTE", "MONTH", "QUARTER", "SECOND", "WEEK", "YEAR"
 ]
 TopicUserExperienceVersionType = Literal["LEGACY", "NEW_READER_EXPERIENCE"]
 URLTargetConfigurationType = Literal["NEW_TAB", "NEW_WINDOW", "SAME_TAB"]
 UndefinedSpecifiedValueTypeType = Literal["LEAST", "MOST"]
-UserRoleType = Literal["ADMIN", "AUTHOR", "READER", "RESTRICTED_AUTHOR", "RESTRICTED_READER"]
+UserRoleType = Literal[
+    "ADMIN",
+    "ADMIN_PRO",
+    "AUTHOR",
+    "AUTHOR_PRO",
+    "READER",
+    "READER_PRO",
+    "RESTRICTED_AUTHOR",
+    "RESTRICTED_READER",
+]
 VPCConnectionAvailabilityStatusType = Literal["AVAILABLE", "PARTIALLY_AVAILABLE", "UNAVAILABLE"]
 VPCConnectionResourceStatusType = Literal[
     "CREATION_FAILED",
     "CREATION_IN_PROGRESS",
     "CREATION_SUCCESSFUL",
     "DELETED",
     "DELETION_FAILED",
@@ -1171,14 +1182,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/literals.pyi` & `mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -171,14 +171,15 @@
     "PivotTableFieldCollapseStateType",
     "PivotTableMetricPlacementType",
     "PivotTableRowsLayoutType",
     "PivotTableSubtotalLevelType",
     "PrimaryValueDisplayTypeType",
     "PropertyRoleType",
     "PropertyUsageType",
+    "PurchaseModeType",
     "RadarChartAxesRangeScaleType",
     "RadarChartShapeType",
     "ReferenceLineLabelHorizontalPositionType",
     "ReferenceLineLabelVerticalPositionType",
     "ReferenceLinePatternTypeType",
     "ReferenceLineSeriesTypeType",
     "ReferenceLineValueLabelRelativePositionType",
@@ -740,14 +741,15 @@
 PivotTableFieldCollapseStateType = Literal["COLLAPSED", "EXPANDED"]
 PivotTableMetricPlacementType = Literal["COLUMN", "ROW"]
 PivotTableRowsLayoutType = Literal["HIERARCHY", "TABULAR"]
 PivotTableSubtotalLevelType = Literal["ALL", "CUSTOM", "LAST"]
 PrimaryValueDisplayTypeType = Literal["ACTUAL", "COMPARISON", "HIDDEN"]
 PropertyRoleType = Literal["ID", "PRIMARY"]
 PropertyUsageType = Literal["DIMENSION", "INHERIT", "MEASURE"]
+PurchaseModeType = Literal["AUTO_PURCHASE", "MANUAL"]
 RadarChartAxesRangeScaleType = Literal["AUTO", "INDEPENDENT", "SHARED"]
 RadarChartShapeType = Literal["CIRCLE", "POLYGON"]
 ReferenceLineLabelHorizontalPositionType = Literal["CENTER", "LEFT", "RIGHT"]
 ReferenceLineLabelVerticalPositionType = Literal["ABOVE", "BELOW"]
 ReferenceLinePatternTypeType = Literal["DASHED", "DOTTED", "SOLID"]
 ReferenceLineSeriesTypeType = Literal["BAR", "LINE"]
 ReferenceLineValueLabelRelativePositionType = Literal["AFTER_CUSTOM_LABEL", "BEFORE_CUSTOM_LABEL"]
@@ -760,15 +762,15 @@
     "CREATION_IN_PROGRESS",
     "CREATION_SUCCESSFUL",
     "DELETED",
     "UPDATE_FAILED",
     "UPDATE_IN_PROGRESS",
     "UPDATE_SUCCESSFUL",
 ]
-RoleType = Literal["ADMIN", "AUTHOR", "READER"]
+RoleType = Literal["ADMIN", "ADMIN_PRO", "AUTHOR", "AUTHOR_PRO", "READER", "READER_PRO"]
 RowLevelPermissionFormatVersionType = Literal["VERSION_1", "VERSION_2"]
 RowLevelPermissionPolicyType = Literal["DENY_ACCESS", "GRANT_ACCESS"]
 SearchAnalysesPaginatorName = Literal["search_analyses"]
 SearchDashboardsPaginatorName = Literal["search_dashboards"]
 SearchDataSetsPaginatorName = Literal["search_data_sets"]
 SearchDataSourcesPaginatorName = Literal["search_data_sources"]
 SearchFoldersPaginatorName = Literal["search_folders"]
@@ -838,15 +840,24 @@
 TopicScheduleTypeType = Literal["DAILY", "HOURLY", "MONTHLY", "WEEKLY"]
 TopicTimeGranularityType = Literal[
     "DAY", "HOUR", "MINUTE", "MONTH", "QUARTER", "SECOND", "WEEK", "YEAR"
 ]
 TopicUserExperienceVersionType = Literal["LEGACY", "NEW_READER_EXPERIENCE"]
 URLTargetConfigurationType = Literal["NEW_TAB", "NEW_WINDOW", "SAME_TAB"]
 UndefinedSpecifiedValueTypeType = Literal["LEAST", "MOST"]
-UserRoleType = Literal["ADMIN", "AUTHOR", "READER", "RESTRICTED_AUTHOR", "RESTRICTED_READER"]
+UserRoleType = Literal[
+    "ADMIN",
+    "ADMIN_PRO",
+    "AUTHOR",
+    "AUTHOR_PRO",
+    "READER",
+    "READER_PRO",
+    "RESTRICTED_AUTHOR",
+    "RESTRICTED_READER",
+]
 VPCConnectionAvailabilityStatusType = Literal["AVAILABLE", "PARTIALLY_AVAILABLE", "UNAVAILABLE"]
 VPCConnectionResourceStatusType = Literal[
     "CREATION_FAILED",
     "CREATION_IN_PROGRESS",
     "CREATION_SUCCESSFUL",
     "DELETED",
     "DELETION_FAILED",
@@ -1171,14 +1182,15 @@
     "robomaker",
     "rolesanywhere",
     "route53",
     "route53-recovery-cluster",
     "route53-recovery-control-config",
     "route53-recovery-readiness",
     "route53domains",
+    "route53profiles",
     "route53resolver",
     "rum",
     "s3",
     "s3control",
     "s3outposts",
     "sagemaker",
     "sagemaker-a2i-runtime",
```

### Comparing `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/paginator.py` & `mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/paginator.py`

 * *Files 0% similar despite different names*

```diff
@@ -86,25 +86,25 @@
 
 from .literals import AssignmentStatusType, RoleType, ThemeTypeType
 from .type_defs import (
     AnalysisSearchFilterTypeDef,
     DashboardSearchFilterTypeDef,
     DataSetSearchFilterTypeDef,
     DataSourceSearchFilterTypeDef,
-    DescribeFolderPermissionsResponsePaginatorTypeDef,
-    DescribeFolderResolvedPermissionsResponsePaginatorTypeDef,
+    DescribeFolderPermissionsResponseTypeDef,
+    DescribeFolderResolvedPermissionsResponseTypeDef,
     FolderSearchFilterTypeDef,
     GroupSearchFilterTypeDef,
     ListAnalysesResponseTypeDef,
     ListAssetBundleExportJobsResponseTypeDef,
     ListAssetBundleImportJobsResponseTypeDef,
     ListDashboardsResponseTypeDef,
     ListDashboardVersionsResponseTypeDef,
     ListDataSetsResponseTypeDef,
-    ListDataSourcesResponsePaginatorTypeDef,
+    ListDataSourcesResponseTypeDef,
     ListFolderMembersResponseTypeDef,
     ListFoldersResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListIAMPolicyAssignmentsForUserResponseTypeDef,
     ListIAMPolicyAssignmentsResponseTypeDef,
     ListIngestionsResponseTypeDef,
@@ -179,15 +179,15 @@
     def paginate(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Namespace: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[DescribeFolderPermissionsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[DescribeFolderPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.DescribeFolderPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/paginators/#describefolderpermissionspaginator)
         """
 
 
 class DescribeFolderResolvedPermissionsPaginator(Paginator):
@@ -199,15 +199,15 @@
     def paginate(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Namespace: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[DescribeFolderResolvedPermissionsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[DescribeFolderResolvedPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.DescribeFolderResolvedPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/paginators/#describefolderresolvedpermissionspaginator)
         """
 
 
 class ListAnalysesPaginator(Paginator):
@@ -304,15 +304,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListDataSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/paginators/#listdatasourcespaginator)
     """
 
     def paginate(
         self, *, AwsAccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListDataSourcesResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListDataSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListDataSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/paginators/#listdatasourcespaginator)
         """
 
 
 class ListFolderMembersPaginator(Paginator):
```

### Comparing `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/paginator.pyi` & `mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -86,25 +86,25 @@
 
 from .literals import AssignmentStatusType, RoleType, ThemeTypeType
 from .type_defs import (
     AnalysisSearchFilterTypeDef,
     DashboardSearchFilterTypeDef,
     DataSetSearchFilterTypeDef,
     DataSourceSearchFilterTypeDef,
-    DescribeFolderPermissionsResponsePaginatorTypeDef,
-    DescribeFolderResolvedPermissionsResponsePaginatorTypeDef,
+    DescribeFolderPermissionsResponseTypeDef,
+    DescribeFolderResolvedPermissionsResponseTypeDef,
     FolderSearchFilterTypeDef,
     GroupSearchFilterTypeDef,
     ListAnalysesResponseTypeDef,
     ListAssetBundleExportJobsResponseTypeDef,
     ListAssetBundleImportJobsResponseTypeDef,
     ListDashboardsResponseTypeDef,
     ListDashboardVersionsResponseTypeDef,
     ListDataSetsResponseTypeDef,
-    ListDataSourcesResponsePaginatorTypeDef,
+    ListDataSourcesResponseTypeDef,
     ListFolderMembersResponseTypeDef,
     ListFoldersResponseTypeDef,
     ListGroupMembershipsResponseTypeDef,
     ListGroupsResponseTypeDef,
     ListIAMPolicyAssignmentsForUserResponseTypeDef,
     ListIAMPolicyAssignmentsResponseTypeDef,
     ListIngestionsResponseTypeDef,
@@ -177,15 +177,15 @@
     def paginate(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Namespace: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[DescribeFolderPermissionsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[DescribeFolderPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.DescribeFolderPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/paginators/#describefolderpermissionspaginator)
         """
 
 class DescribeFolderResolvedPermissionsPaginator(Paginator):
     """
@@ -196,15 +196,15 @@
     def paginate(
         self,
         *,
         AwsAccountId: str,
         FolderId: str,
         Namespace: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[DescribeFolderResolvedPermissionsResponsePaginatorTypeDef]:
+    ) -> _PageIterator[DescribeFolderResolvedPermissionsResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.DescribeFolderResolvedPermissions.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/paginators/#describefolderresolvedpermissionspaginator)
         """
 
 class ListAnalysesPaginator(Paginator):
     """
@@ -294,15 +294,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListDataSources)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/paginators/#listdatasourcespaginator)
     """
 
     def paginate(
         self, *, AwsAccountId: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListDataSourcesResponsePaginatorTypeDef]:
+    ) -> _PageIterator[ListDataSourcesResponseTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight.Paginator.ListDataSources.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/paginators/#listdatasourcespaginator)
         """
 
 class ListFolderMembersPaginator(Paginator):
     """
```

### Comparing `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/type_defs.py` & `mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/type_defs.py`

 * *Files 17% similar despite different names*

```diff
@@ -132,14 +132,15 @@
     PivotTableFieldCollapseStateType,
     PivotTableMetricPlacementType,
     PivotTableRowsLayoutType,
     PivotTableSubtotalLevelType,
     PrimaryValueDisplayTypeType,
     PropertyRoleType,
     PropertyUsageType,
+    PurchaseModeType,
     RadarChartAxesRangeScaleType,
     RadarChartShapeType,
     ReferenceLineLabelHorizontalPositionType,
     ReferenceLineLabelVerticalPositionType,
     ReferenceLinePatternTypeType,
     ReferenceLineSeriesTypeType,
     ReferenceLineValueLabelRelativePositionType,
@@ -238,44 +239,55 @@
     "AnalysisSearchFilterTypeDef",
     "DataSetReferenceTypeDef",
     "AnalysisSummaryTypeDef",
     "SheetTypeDef",
     "AnchorDateConfigurationTypeDef",
     "AnonymousUserDashboardEmbeddingConfigurationTypeDef",
     "DashboardVisualIdTypeDef",
+    "AnonymousUserGenerativeQnAEmbeddingConfigurationTypeDef",
     "AnonymousUserQSearchBarEmbeddingConfigurationTypeDef",
     "ArcAxisDisplayRangeTypeDef",
     "ArcConfigurationTypeDef",
     "ArcOptionsTypeDef",
+    "AssetBundleExportJobAnalysisOverridePropertiesOutputTypeDef",
+    "AssetBundleExportJobDashboardOverridePropertiesOutputTypeDef",
+    "AssetBundleExportJobDataSetOverridePropertiesOutputTypeDef",
+    "AssetBundleExportJobDataSourceOverridePropertiesOutputTypeDef",
+    "AssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef",
+    "AssetBundleExportJobResourceIdOverrideConfigurationTypeDef",
+    "AssetBundleExportJobThemeOverridePropertiesOutputTypeDef",
+    "AssetBundleExportJobVPCConnectionOverridePropertiesOutputTypeDef",
     "AssetBundleExportJobAnalysisOverridePropertiesTypeDef",
     "AssetBundleExportJobDashboardOverridePropertiesTypeDef",
     "AssetBundleExportJobDataSetOverridePropertiesTypeDef",
     "AssetBundleExportJobDataSourceOverridePropertiesTypeDef",
     "AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef",
-    "AssetBundleExportJobResourceIdOverrideConfigurationTypeDef",
     "AssetBundleExportJobThemeOverridePropertiesTypeDef",
     "AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef",
     "AssetBundleExportJobErrorTypeDef",
     "AssetBundleExportJobSummaryTypeDef",
     "AssetBundleExportJobValidationStrategyTypeDef",
     "AssetBundleExportJobWarningTypeDef",
     "AssetBundleImportJobAnalysisOverrideParametersTypeDef",
+    "AssetBundleResourcePermissionsOutputTypeDef",
     "AssetBundleResourcePermissionsTypeDef",
     "TagTypeDef",
     "AssetBundleImportJobDashboardOverrideParametersTypeDef",
     "AssetBundleImportJobDataSetOverrideParametersTypeDef",
     "AssetBundleImportJobDataSourceCredentialPairTypeDef",
     "SslPropertiesTypeDef",
     "VpcConnectionPropertiesTypeDef",
     "AssetBundleImportJobErrorTypeDef",
-    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
+    "AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef",
     "AssetBundleImportJobResourceIdOverrideConfigurationTypeDef",
     "AssetBundleImportJobThemeOverrideParametersTypeDef",
+    "AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef",
     "AssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
     "AssetBundleImportJobOverrideValidationStrategyTypeDef",
+    "TimestampTypeDef",
     "AssetBundleImportJobSummaryTypeDef",
     "AssetBundleImportJobWarningTypeDef",
     "AssetBundleImportSourceDescriptionTypeDef",
     "BlobTypeDef",
     "AthenaParametersTypeDef",
     "AuroraParametersTypeDef",
     "AuroraPostgreSqlParametersTypeDef",
@@ -295,38 +307,43 @@
     "PaginationConfigurationTypeDef",
     "CalculatedColumnTypeDef",
     "CalculatedMeasureFieldTypeDef",
     "CancelIngestionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CastColumnTypeOperationTypeDef",
     "CustomFilterConfigurationTypeDef",
+    "CustomFilterListConfigurationOutputTypeDef",
+    "FilterListConfigurationOutputTypeDef",
     "CustomFilterListConfigurationTypeDef",
     "FilterListConfigurationTypeDef",
+    "CellValueSynonymOutputTypeDef",
     "CellValueSynonymTypeDef",
     "SimpleClusterMarkerTypeDef",
+    "CollectiveConstantOutputTypeDef",
     "CollectiveConstantTypeDef",
     "DataColorTypeDef",
     "CustomColorTypeDef",
     "ColumnDescriptionTypeDef",
     "ColumnGroupColumnSchemaTypeDef",
+    "GeoSpatialColumnGroupOutputTypeDef",
     "GeoSpatialColumnGroupTypeDef",
+    "ColumnLevelPermissionRuleOutputTypeDef",
     "ColumnLevelPermissionRuleTypeDef",
     "ColumnSchemaTypeDef",
+    "ComparativeOrderOutputTypeDef",
     "ComparativeOrderTypeDef",
     "ConditionalFormattingSolidColorTypeDef",
     "ConditionalFormattingCustomIconOptionsTypeDef",
     "ConditionalFormattingIconDisplayConfigurationTypeDef",
     "ConditionalFormattingIconSetTypeDef",
     "ContextMenuOptionTypeDef",
     "CreateAccountSubscriptionRequestRequestTypeDef",
     "SignupResponseTypeDef",
-    "ResourcePermissionTypeDef",
     "ValidationStrategyTypeDef",
     "DataSetUsageConfigurationTypeDef",
-    "FieldFolderTypeDef",
     "RowLevelPermissionDataSetTypeDef",
     "CreateFolderMembershipRequestRequestTypeDef",
     "FolderMemberTypeDef",
     "CreateGroupMembershipRequestRequestTypeDef",
     "GroupMemberTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "GroupTypeDef",
@@ -339,15 +356,15 @@
     "ThemeAliasTypeDef",
     "DecimalPlacesConfigurationTypeDef",
     "NegativeValueConfigurationTypeDef",
     "NullValueFormatConfigurationTypeDef",
     "LocalNavigationConfigurationTypeDef",
     "CustomActionURLOperationTypeDef",
     "CustomNarrativeOptionsTypeDef",
-    "TimestampTypeDef",
+    "CustomParameterValuesOutputTypeDef",
     "InputColumnTypeDef",
     "DataPointDrillUpDownOptionTypeDef",
     "DataPointMenuLabelOptionTypeDef",
     "DataPointTooltipOptionTypeDef",
     "ExportToCSVOptionTypeDef",
     "ExportWithHiddenFieldsOptionTypeDef",
     "SheetControlsOptionTypeDef",
@@ -356,22 +373,24 @@
     "VisualMenuOptionTypeDef",
     "DashboardSearchFilterTypeDef",
     "DashboardSummaryTypeDef",
     "DashboardVersionSummaryTypeDef",
     "ExportHiddenFieldsOptionTypeDef",
     "DataAggregationTypeDef",
     "DataBarsOptionsTypeDef",
+    "DataColorPaletteOutputTypeDef",
     "DataColorPaletteTypeDef",
     "DataPathLabelTypeTypeDef",
     "FieldLabelTypeTypeDef",
     "MaximumLabelTypeTypeDef",
     "MinimumLabelTypeTypeDef",
     "RangeEndsLabelTypeTypeDef",
     "DataPathTypeTypeDef",
     "DataSetSearchFilterTypeDef",
+    "FieldFolderOutputTypeDef",
     "OutputColumnTypeDef",
     "DataSourceErrorInfoTypeDef",
     "DatabricksParametersTypeDef",
     "ExasolParametersTypeDef",
     "JiraParametersTypeDef",
     "MariaDbParametersTypeDef",
     "MySqlParametersTypeDef",
@@ -385,20 +404,26 @@
     "SqlServerParametersTypeDef",
     "StarburstParametersTypeDef",
     "TeradataParametersTypeDef",
     "TrinoParametersTypeDef",
     "TwitterParametersTypeDef",
     "DataSourceSearchFilterTypeDef",
     "DataSourceSummaryTypeDef",
+    "DateTimeDatasetParameterDefaultValuesOutputTypeDef",
     "RollingDateConfigurationTypeDef",
+    "DateTimeValueWhenUnsetConfigurationOutputTypeDef",
     "MappedDataSetParameterTypeDef",
+    "DateTimeParameterOutputTypeDef",
     "SheetControlInfoIconLabelOptionsTypeDef",
+    "DecimalDatasetParameterDefaultValuesOutputTypeDef",
     "DecimalDatasetParameterDefaultValuesTypeDef",
     "DecimalValueWhenUnsetConfigurationTypeDef",
+    "DecimalParameterOutputTypeDef",
     "DecimalParameterTypeDef",
+    "FilterSelectableValuesOutputTypeDef",
     "FilterSelectableValuesTypeDef",
     "DeleteAccountCustomizationRequestRequestTypeDef",
     "DeleteAccountSubscriptionRequestRequestTypeDef",
     "DeleteAnalysisRequestRequestTypeDef",
     "DeleteDashboardRequestRequestTypeDef",
     "DeleteDataSetRefreshPropertiesRequestRequestTypeDef",
     "DeleteDataSetRequestRequestTypeDef",
@@ -423,14 +448,15 @@
     "DeleteUserRequestRequestTypeDef",
     "DeleteVPCConnectionRequestRequestTypeDef",
     "DescribeAccountCustomizationRequestRequestTypeDef",
     "DescribeAccountSettingsRequestRequestTypeDef",
     "DescribeAccountSubscriptionRequestRequestTypeDef",
     "DescribeAnalysisDefinitionRequestRequestTypeDef",
     "DescribeAnalysisPermissionsRequestRequestTypeDef",
+    "ResourcePermissionOutputTypeDef",
     "DescribeAnalysisRequestRequestTypeDef",
     "DescribeAssetBundleExportJobRequestRequestTypeDef",
     "DescribeAssetBundleImportJobRequestRequestTypeDef",
     "DescribeDashboardDefinitionRequestRequestTypeDef",
     "DescribeDashboardPermissionsRequestRequestTypeDef",
     "DescribeDashboardRequestRequestTypeDef",
     "DescribeDashboardSnapshotJobRequestRequestTypeDef",
@@ -439,15 +465,15 @@
     "DescribeDataSetPermissionsRequestRequestTypeDef",
     "DescribeDataSetRefreshPropertiesRequestRequestTypeDef",
     "DescribeDataSetRequestRequestTypeDef",
     "DescribeDataSourcePermissionsRequestRequestTypeDef",
     "DescribeDataSourceRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeFolderPermissionsRequestRequestTypeDef",
-    "ResourcePermissionPaginatorTypeDef",
+    "ResourcePermissionExtraOutputTypeDef",
     "DescribeFolderRequestRequestTypeDef",
     "DescribeFolderResolvedPermissionsRequestRequestTypeDef",
     "FolderTypeDef",
     "DescribeGroupMembershipRequestRequestTypeDef",
     "DescribeGroupRequestRequestTypeDef",
     "DescribeIAMPolicyAssignmentRequestRequestTypeDef",
     "IAMPolicyAssignmentTypeDef",
@@ -463,38 +489,44 @@
     "DescribeThemeAliasRequestRequestTypeDef",
     "DescribeThemePermissionsRequestRequestTypeDef",
     "DescribeThemeRequestRequestTypeDef",
     "DescribeTopicPermissionsRequestRequestTypeDef",
     "DescribeTopicRefreshRequestRequestTypeDef",
     "TopicRefreshDetailsTypeDef",
     "DescribeTopicRefreshScheduleRequestRequestTypeDef",
+    "TopicRefreshScheduleOutputTypeDef",
     "DescribeTopicRequestRequestTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "UserTypeDef",
     "DescribeVPCConnectionRequestRequestTypeDef",
     "NegativeFormatTypeDef",
     "DonutCenterOptionsTypeDef",
     "ListControlSelectAllOptionsTypeDef",
     "ErrorInfoTypeDef",
     "ExcludePeriodConfigurationTypeDef",
+    "FieldFolderTypeDef",
     "FieldSortTypeDef",
     "FieldTooltipItemTypeDef",
     "GeospatialMapStyleOptionsTypeDef",
+    "SameSheetTargetVisualConfigurationOutputTypeDef",
     "SameSheetTargetVisualConfigurationTypeDef",
     "FilterOperationTypeDef",
     "FolderSearchFilterTypeDef",
     "FolderSummaryTypeDef",
     "FontSizeTypeDef",
     "FontWeightTypeDef",
     "FontTypeDef",
     "TimeBasedForecastPropertiesTypeDef",
+    "WhatIfPointScenarioOutputTypeDef",
+    "WhatIfRangeScenarioOutputTypeDef",
     "FreeFormLayoutScreenCanvasSizeOptionsTypeDef",
     "FreeFormLayoutElementBackgroundStyleTypeDef",
     "FreeFormLayoutElementBorderStyleTypeDef",
     "LoadingAnimationTypeDef",
+    "GaugeChartColorConfigurationTypeDef",
     "SessionTagTypeDef",
     "GeospatialCoordinateBoundsTypeDef",
     "GeospatialHeatmapDataColorTypeDef",
     "GetDashboardEmbedUrlRequestRequestTypeDef",
     "GetSessionEmbedUrlRequestRequestTypeDef",
     "TableBorderOptionsTypeDef",
     "GradientStopTypeDef",
@@ -503,26 +535,29 @@
     "GroupSearchFilterTypeDef",
     "GutterStyleTypeDef",
     "IAMPolicyAssignmentSummaryTypeDef",
     "IdentityCenterConfigurationTypeDef",
     "LookbackWindowTypeDef",
     "QueueInfoTypeDef",
     "RowInfoTypeDef",
+    "IntegerDatasetParameterDefaultValuesOutputTypeDef",
     "IntegerDatasetParameterDefaultValuesTypeDef",
     "IntegerValueWhenUnsetConfigurationTypeDef",
+    "IntegerParameterOutputTypeDef",
     "IntegerParameterTypeDef",
     "JoinKeyPropertiesTypeDef",
     "KPISparklineOptionsTypeDef",
     "ProgressBarOptionsTypeDef",
     "SecondaryValueOptionsTypeDef",
     "TrendArrowOptionsTypeDef",
     "KPIVisualStandardLayoutTypeDef",
     "LineChartLineStyleSettingsTypeDef",
     "LineChartMarkerStyleSettingsTypeDef",
     "MissingDataConfigurationTypeDef",
+    "ResourcePermissionTypeDef",
     "ListAnalysesRequestRequestTypeDef",
     "ListAssetBundleExportJobsRequestRequestTypeDef",
     "ListAssetBundleImportJobsRequestRequestTypeDef",
     "ListControlSearchOptionsTypeDef",
     "ListDashboardVersionsRequestRequestTypeDef",
     "ListDashboardsRequestRequestTypeDef",
     "ListDataSetsRequestRequestTypeDef",
@@ -555,133 +590,177 @@
     "TopicSummaryTypeDef",
     "ListUserGroupsRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVPCConnectionsRequestRequestTypeDef",
     "LongFormatTextTypeDef",
     "ManifestFileLocationTypeDef",
     "MarginStyleTypeDef",
+    "NamedEntityDefinitionMetricOutputTypeDef",
     "NamedEntityDefinitionMetricTypeDef",
     "NamespaceErrorTypeDef",
     "NetworkInterfaceTypeDef",
+    "NewDefaultValuesOutputTypeDef",
     "NumericRangeFilterValueTypeDef",
     "ThousandSeparatorOptionsTypeDef",
     "PercentileAggregationTypeDef",
+    "StringParameterOutputTypeDef",
     "StringParameterTypeDef",
     "PercentVisibleRangeTypeDef",
     "PivotTableConditionalFormattingScopeTypeDef",
     "PivotTablePaginatedReportOptionsTypeDef",
     "PivotTableFieldOptionTypeDef",
     "PivotTableFieldSubtotalOptionsTypeDef",
     "PivotTableRowsLabelOptionsTypeDef",
+    "RowAlternateColorOptionsOutputTypeDef",
     "RowAlternateColorOptionsTypeDef",
+    "ProjectOperationOutputTypeDef",
     "ProjectOperationTypeDef",
     "RadarChartAreaStyleSettingsTypeDef",
     "RangeConstantTypeDef",
-    "RedshiftIAMParametersPaginatorTypeDef",
+    "RedshiftIAMParametersExtraOutputTypeDef",
+    "RedshiftIAMParametersOutputTypeDef",
     "RedshiftIAMParametersTypeDef",
     "ReferenceLineCustomLabelConfigurationTypeDef",
     "ReferenceLineStaticDataConfigurationTypeDef",
     "ReferenceLineStyleConfigurationTypeDef",
     "ScheduleRefreshOnEntityTypeDef",
     "StatePersistenceConfigurationsTypeDef",
+    "RegisteredUserGenerativeQnAEmbeddingConfigurationTypeDef",
     "RegisteredUserQSearchBarEmbeddingConfigurationTypeDef",
     "RenameColumnOperationTypeDef",
     "RestoreAnalysisRequestRequestTypeDef",
     "RowLevelPermissionTagRuleTypeDef",
     "S3BucketConfigurationTypeDef",
     "UploadSettingsTypeDef",
     "SectionAfterPageBreakTypeDef",
     "SpacingTypeDef",
+    "SheetVisualScopingConfigurationOutputTypeDef",
     "SheetVisualScopingConfigurationTypeDef",
+    "SemanticEntityTypeOutputTypeDef",
     "SemanticEntityTypeTypeDef",
+    "SemanticTypeOutputTypeDef",
     "SemanticTypeTypeDef",
     "SheetTextBoxTypeDef",
     "SheetElementConfigurationOverridesTypeDef",
     "ShortFormatTextTypeDef",
     "YAxisOptionsTypeDef",
     "SmallMultiplesAxisPropertiesTypeDef",
     "SnapshotAnonymousUserRedactedTypeDef",
+    "SnapshotFileSheetSelectionOutputTypeDef",
     "SnapshotFileSheetSelectionTypeDef",
     "SnapshotJobResultErrorInfoTypeDef",
+    "StringDatasetParameterDefaultValuesOutputTypeDef",
     "StringDatasetParameterDefaultValuesTypeDef",
     "StringValueWhenUnsetConfigurationTypeDef",
     "TableStyleTargetTypeDef",
     "TableCellImageSizingConfigurationTypeDef",
     "TablePaginatedReportOptionsTypeDef",
     "TableFieldCustomIconContentTypeDef",
+    "TablePinnedFieldOptionsOutputTypeDef",
     "TablePinnedFieldOptionsTypeDef",
     "TemplateSourceTemplateTypeDef",
     "TextControlPlaceholderOptionsTypeDef",
     "UIColorPaletteTypeDef",
     "ThemeErrorTypeDef",
     "TopicSingularFilterConstantTypeDef",
     "TotalAggregationFunctionTypeDef",
+    "UntagColumnOperationOutputTypeDef",
     "UntagColumnOperationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccountSettingsRequestRequestTypeDef",
     "UpdateDashboardLinksRequestRequestTypeDef",
     "UpdateDashboardPublishedVersionRequestRequestTypeDef",
     "UpdateFolderRequestRequestTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateIAMPolicyAssignmentRequestRequestTypeDef",
     "UpdateIdentityPropagationConfigRequestRequestTypeDef",
     "UpdateIpRestrictionRequestRequestTypeDef",
     "UpdatePublicSharingSettingsRequestRequestTypeDef",
     "UpdateRoleCustomPermissionRequestRequestTypeDef",
+    "UpdateSPICECapacityConfigurationRequestRequestTypeDef",
     "UpdateTemplateAliasRequestRequestTypeDef",
     "UpdateThemeAliasRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateVPCConnectionRequestRequestTypeDef",
     "WaterfallChartGroupColorConfigurationTypeDef",
     "WaterfallChartOptionsTypeDef",
     "WordCloudOptionsTypeDef",
     "UpdateAccountCustomizationRequestRequestTypeDef",
     "AxisLabelReferenceOptionsTypeDef",
     "CascadingControlSourceTypeDef",
+    "CategoryDrillDownFilterOutputTypeDef",
     "CategoryDrillDownFilterTypeDef",
+    "ContributionAnalysisDefaultOutputTypeDef",
     "ContributionAnalysisDefaultTypeDef",
     "DynamicDefaultValueTypeDef",
+    "FilterOperationSelectedFieldsConfigurationOutputTypeDef",
     "FilterOperationSelectedFieldsConfigurationTypeDef",
     "NumericEqualityDrillDownFilterTypeDef",
+    "ParameterSelectableValuesOutputTypeDef",
     "ParameterSelectableValuesTypeDef",
+    "TimeRangeDrillDownFilterOutputTypeDef",
     "AnalysisErrorTypeDef",
     "DashboardErrorTypeDef",
     "TemplateErrorTypeDef",
     "SearchAnalysesRequestRequestTypeDef",
     "AnalysisSourceTemplateTypeDef",
     "DashboardSourceTemplateTypeDef",
     "TemplateSourceAnalysisTypeDef",
     "AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef",
     "RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef",
     "ArcAxisConfigurationTypeDef",
+    "AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef",
     "AssetBundleCloudFormationOverridePropertyConfigurationTypeDef",
+    "AssetBundleImportJobAnalysisOverridePermissionsOutputTypeDef",
+    "AssetBundleImportJobDataSetOverridePermissionsOutputTypeDef",
+    "AssetBundleImportJobDataSourceOverridePermissionsOutputTypeDef",
+    "AssetBundleImportJobThemeOverridePermissionsOutputTypeDef",
+    "AssetBundleResourceLinkSharingConfigurationOutputTypeDef",
     "AssetBundleImportJobAnalysisOverridePermissionsTypeDef",
     "AssetBundleImportJobDataSetOverridePermissionsTypeDef",
     "AssetBundleImportJobDataSourceOverridePermissionsTypeDef",
     "AssetBundleImportJobThemeOverridePermissionsTypeDef",
     "AssetBundleResourceLinkSharingConfigurationTypeDef",
+    "AssetBundleImportJobAnalysisOverrideTagsOutputTypeDef",
     "AssetBundleImportJobAnalysisOverrideTagsTypeDef",
+    "AssetBundleImportJobDashboardOverrideTagsOutputTypeDef",
     "AssetBundleImportJobDashboardOverrideTagsTypeDef",
+    "AssetBundleImportJobDataSetOverrideTagsOutputTypeDef",
     "AssetBundleImportJobDataSetOverrideTagsTypeDef",
+    "AssetBundleImportJobDataSourceOverrideTagsOutputTypeDef",
     "AssetBundleImportJobDataSourceOverrideTagsTypeDef",
+    "AssetBundleImportJobThemeOverrideTagsOutputTypeDef",
     "AssetBundleImportJobThemeOverrideTagsTypeDef",
+    "AssetBundleImportJobVPCConnectionOverrideTagsOutputTypeDef",
     "AssetBundleImportJobVPCConnectionOverrideTagsTypeDef",
     "CreateAccountCustomizationRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateVPCConnectionRequestRequestTypeDef",
     "RegisterUserRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssetBundleImportJobDataSourceCredentialsTypeDef",
+    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
+    "CustomParameterValuesTypeDef",
+    "DateTimeDatasetParameterDefaultValuesTypeDef",
+    "DateTimeParameterTypeDef",
+    "DateTimeValueWhenUnsetConfigurationTypeDef",
+    "NewDefaultValuesTypeDef",
+    "TimeRangeDrillDownFilterTypeDef",
+    "TopicRefreshScheduleTypeDef",
+    "WhatIfPointScenarioTypeDef",
+    "WhatIfRangeScenarioTypeDef",
     "AssetBundleImportSourceTypeDef",
+    "AxisDisplayRangeOutputTypeDef",
     "AxisDisplayRangeTypeDef",
     "AxisScaleTypeDef",
     "ScatterPlotSortConfigurationTypeDef",
     "HistogramBinOptionsTypeDef",
     "TileStyleTypeDef",
     "BoxPlotOptionsTypeDef",
+    "CreateColumnsOperationOutputTypeDef",
     "CreateColumnsOperationTypeDef",
     "CancelIngestionResponseTypeDef",
     "CreateAccountCustomizationResponseTypeDef",
     "CreateAnalysisResponseTypeDef",
     "CreateDashboardResponseTypeDef",
     "CreateDataSetResponseTypeDef",
     "CreateDataSourceResponseTypeDef",
@@ -759,53 +838,39 @@
     "UpdateFolderResponseTypeDef",
     "UpdateIAMPolicyAssignmentResponseTypeDef",
     "UpdateIdentityPropagationConfigResponseTypeDef",
     "UpdateIpRestrictionResponseTypeDef",
     "UpdatePublicSharingSettingsResponseTypeDef",
     "UpdateRefreshScheduleResponseTypeDef",
     "UpdateRoleCustomPermissionResponseTypeDef",
+    "UpdateSPICECapacityConfigurationResponseTypeDef",
     "UpdateTemplateResponseTypeDef",
     "UpdateThemeResponseTypeDef",
     "UpdateTopicRefreshScheduleResponseTypeDef",
     "UpdateTopicResponseTypeDef",
     "UpdateVPCConnectionResponseTypeDef",
+    "CategoryFilterConfigurationOutputTypeDef",
     "CategoryFilterConfigurationTypeDef",
     "ClusterMarkerTypeDef",
+    "TopicCategoryFilterConstantOutputTypeDef",
     "TopicCategoryFilterConstantTypeDef",
+    "ColorScaleOutputTypeDef",
     "ColorScaleTypeDef",
+    "ColorsConfigurationOutputTypeDef",
     "ColorsConfigurationTypeDef",
     "ColumnTagTypeDef",
+    "ColumnGroupSchemaOutputTypeDef",
     "ColumnGroupSchemaTypeDef",
+    "ColumnGroupOutputTypeDef",
     "ColumnGroupTypeDef",
+    "ColumnLevelPermissionRuleUnionTypeDef",
+    "DataSetSchemaOutputTypeDef",
     "DataSetSchemaTypeDef",
     "ConditionalFormattingCustomIconConditionTypeDef",
     "CreateAccountSubscriptionResponseTypeDef",
-    "CreateFolderRequestRequestTypeDef",
-    "DescribeAnalysisPermissionsResponseTypeDef",
-    "DescribeDataSetPermissionsResponseTypeDef",
-    "DescribeDataSourcePermissionsResponseTypeDef",
-    "DescribeFolderPermissionsResponseTypeDef",
-    "DescribeFolderResolvedPermissionsResponseTypeDef",
-    "DescribeTemplatePermissionsResponseTypeDef",
-    "DescribeThemePermissionsResponseTypeDef",
-    "DescribeTopicPermissionsResponseTypeDef",
-    "LinkSharingConfigurationTypeDef",
-    "UpdateAnalysisPermissionsRequestRequestTypeDef",
-    "UpdateAnalysisPermissionsResponseTypeDef",
-    "UpdateDashboardPermissionsRequestRequestTypeDef",
-    "UpdateDataSetPermissionsRequestRequestTypeDef",
-    "UpdateDataSourcePermissionsRequestRequestTypeDef",
-    "UpdateFolderPermissionsRequestRequestTypeDef",
-    "UpdateFolderPermissionsResponseTypeDef",
-    "UpdateTemplatePermissionsRequestRequestTypeDef",
-    "UpdateTemplatePermissionsResponseTypeDef",
-    "UpdateThemePermissionsRequestRequestTypeDef",
-    "UpdateThemePermissionsResponseTypeDef",
-    "UpdateTopicPermissionsRequestRequestTypeDef",
-    "UpdateTopicPermissionsResponseTypeDef",
     "DataSetSummaryTypeDef",
     "CreateFolderMembershipResponseTypeDef",
     "CreateGroupMembershipResponseTypeDef",
     "DescribeGroupMembershipResponseTypeDef",
     "ListGroupMembershipsResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "DescribeGroupResponseTypeDef",
@@ -818,39 +883,49 @@
     "ListTemplateAliasesResponseTypeDef",
     "UpdateTemplateAliasResponseTypeDef",
     "CreateThemeAliasResponseTypeDef",
     "DescribeThemeAliasResponseTypeDef",
     "ListThemeAliasesResponseTypeDef",
     "UpdateThemeAliasResponseTypeDef",
     "CustomActionNavigationOperationTypeDef",
-    "CustomParameterValuesTypeDef",
-    "DateTimeDatasetParameterDefaultValuesTypeDef",
-    "DateTimeParameterTypeDef",
-    "DateTimeValueWhenUnsetConfigurationTypeDef",
-    "NewDefaultValuesTypeDef",
-    "TimeRangeDrillDownFilterTypeDef",
-    "TopicRefreshScheduleTypeDef",
-    "WhatIfPointScenarioTypeDef",
-    "WhatIfRangeScenarioTypeDef",
+    "CustomValuesConfigurationOutputTypeDef",
+    "CustomSqlOutputTypeDef",
     "CustomSqlTypeDef",
+    "RelationalTableOutputTypeDef",
     "RelationalTableTypeDef",
     "VisualInteractionOptionsTypeDef",
     "SearchDashboardsRequestRequestTypeDef",
     "ListDashboardsResponseTypeDef",
     "SearchDashboardsResponseTypeDef",
     "ListDashboardVersionsResponseTypeDef",
     "DashboardVisualPublishOptionsTypeDef",
     "TableInlineVisualizationTypeDef",
     "DataLabelTypeTypeDef",
     "DataPathValueTypeDef",
     "SearchDataSetsRequestRequestTypeDef",
     "SearchDataSourcesRequestRequestTypeDef",
     "SearchDataSourcesResponseTypeDef",
+    "DateTimeDatasetParameterOutputTypeDef",
+    "TimeRangeFilterValueOutputTypeDef",
     "TimeRangeFilterValueTypeDef",
+    "DecimalDatasetParameterOutputTypeDef",
     "DecimalDatasetParameterTypeDef",
+    "DescribeAnalysisPermissionsResponseTypeDef",
+    "DescribeDataSetPermissionsResponseTypeDef",
+    "DescribeDataSourcePermissionsResponseTypeDef",
+    "DescribeFolderResolvedPermissionsResponseTypeDef",
+    "DescribeTemplatePermissionsResponseTypeDef",
+    "DescribeThemePermissionsResponseTypeDef",
+    "DescribeTopicPermissionsResponseTypeDef",
+    "LinkSharingConfigurationOutputTypeDef",
+    "UpdateAnalysisPermissionsResponseTypeDef",
+    "UpdateFolderPermissionsResponseTypeDef",
+    "UpdateTemplatePermissionsResponseTypeDef",
+    "UpdateThemePermissionsResponseTypeDef",
+    "UpdateTopicPermissionsResponseTypeDef",
     "DescribeFolderPermissionsRequestDescribeFolderPermissionsPaginateTypeDef",
     "DescribeFolderResolvedPermissionsRequestDescribeFolderResolvedPermissionsPaginateTypeDef",
     "ListAnalysesRequestListAnalysesPaginateTypeDef",
     "ListAssetBundleExportJobsRequestListAssetBundleExportJobsPaginateTypeDef",
     "ListAssetBundleImportJobsRequestListAssetBundleImportJobsPaginateTypeDef",
     "ListDashboardVersionsRequestListDashboardVersionsPaginateTypeDef",
     "ListDashboardsRequestListDashboardsPaginateTypeDef",
@@ -872,323 +947,459 @@
     "ListThemesRequestListThemesPaginateTypeDef",
     "ListUserGroupsRequestListUserGroupsPaginateTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "SearchAnalysesRequestSearchAnalysesPaginateTypeDef",
     "SearchDashboardsRequestSearchDashboardsPaginateTypeDef",
     "SearchDataSetsRequestSearchDataSetsPaginateTypeDef",
     "SearchDataSourcesRequestSearchDataSourcesPaginateTypeDef",
-    "DescribeFolderPermissionsResponsePaginatorTypeDef",
-    "DescribeFolderResolvedPermissionsResponsePaginatorTypeDef",
+    "DescribeFolderPermissionsResponseTypeDef",
     "DescribeFolderResponseTypeDef",
     "DescribeIAMPolicyAssignmentResponseTypeDef",
     "DescribeTopicRefreshResponseTypeDef",
+    "DescribeTopicRefreshScheduleResponseTypeDef",
+    "TopicRefreshScheduleSummaryTypeDef",
     "DescribeUserResponseTypeDef",
     "ListUsersResponseTypeDef",
     "RegisterUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
     "DisplayFormatOptionsTypeDef",
     "DonutOptionsTypeDef",
+    "FieldFolderUnionTypeDef",
+    "FilterOperationTargetVisualsConfigurationOutputTypeDef",
     "FilterOperationTargetVisualsConfigurationTypeDef",
     "SearchFoldersRequestRequestTypeDef",
     "SearchFoldersRequestSearchFoldersPaginateTypeDef",
     "ListFoldersResponseTypeDef",
     "SearchFoldersResponseTypeDef",
     "FontConfigurationTypeDef",
+    "TypographyOutputTypeDef",
     "TypographyTypeDef",
+    "ForecastScenarioOutputTypeDef",
     "FreeFormLayoutCanvasSizeOptionsTypeDef",
     "SnapshotAnonymousUserTypeDef",
     "GeospatialWindowOptionsTypeDef",
+    "GeospatialHeatmapColorScaleOutputTypeDef",
     "GeospatialHeatmapColorScaleTypeDef",
     "TableSideBorderOptionsTypeDef",
+    "GradientColorOutputTypeDef",
     "GradientColorTypeDef",
     "GridLayoutCanvasSizeOptionsTypeDef",
     "SearchGroupsRequestRequestTypeDef",
     "SearchGroupsRequestSearchGroupsPaginateTypeDef",
     "ListIAMPolicyAssignmentsResponseTypeDef",
     "IncrementalRefreshTypeDef",
     "IngestionTypeDef",
+    "IntegerDatasetParameterOutputTypeDef",
     "IntegerDatasetParameterTypeDef",
     "JoinInstructionTypeDef",
     "KPIVisualLayoutOptionsTypeDef",
     "LineChartDefaultSeriesSettingsTypeDef",
     "LineChartSeriesSettingsTypeDef",
+    "LinkSharingConfigurationTypeDef",
+    "ResourcePermissionUnionTypeDef",
     "ListFolderMembersResponseTypeDef",
     "ListTemplateVersionsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "ListThemeVersionsResponseTypeDef",
     "ListThemesResponseTypeDef",
     "ListTopicsResponseTypeDef",
     "VisualSubtitleLabelOptionsTypeDef",
     "S3ParametersTypeDef",
     "TileLayoutStyleTypeDef",
+    "NamedEntityDefinitionOutputTypeDef",
     "NamedEntityDefinitionTypeDef",
     "NamespaceInfoV2TypeDef",
     "VPCConnectionSummaryTypeDef",
     "VPCConnectionTypeDef",
+    "OverrideDatasetParameterOperationOutputTypeDef",
     "NumericSeparatorConfigurationTypeDef",
     "NumericalAggregationFunctionTypeDef",
+    "ParametersOutputTypeDef",
     "VisibleRangeOptionsTypeDef",
     "RadarChartSeriesSettingsTypeDef",
     "TopicRangeFilterConstantTypeDef",
-    "RedshiftParametersPaginatorTypeDef",
+    "RedshiftParametersExtraOutputTypeDef",
+    "RedshiftParametersOutputTypeDef",
     "RedshiftParametersTypeDef",
     "RefreshFrequencyTypeDef",
     "RegisteredUserConsoleFeatureConfigurationsTypeDef",
     "RegisteredUserDashboardFeatureConfigurationsTypeDef",
+    "RowLevelPermissionTagConfigurationOutputTypeDef",
     "RowLevelPermissionTagConfigurationTypeDef",
     "SnapshotS3DestinationConfigurationTypeDef",
+    "S3SourceOutputTypeDef",
     "S3SourceTypeDef",
     "SectionPageBreakConfigurationTypeDef",
     "SectionBasedLayoutPaperCanvasSizeOptionsTypeDef",
     "SectionStyleTypeDef",
+    "SelectedSheetsFilterScopeConfigurationOutputTypeDef",
     "SelectedSheetsFilterScopeConfigurationTypeDef",
     "SheetElementRenderingRuleTypeDef",
     "VisualTitleLabelOptionsTypeDef",
     "SingleAxisOptionsTypeDef",
     "SnapshotUserConfigurationRedactedTypeDef",
+    "SnapshotFileOutputTypeDef",
     "SnapshotFileTypeDef",
+    "StringDatasetParameterOutputTypeDef",
     "StringDatasetParameterTypeDef",
     "TableFieldImageConfigurationTypeDef",
     "TopicNumericEqualityFilterTypeDef",
     "TopicRelativeDateFilterTypeDef",
     "TotalAggregationOptionTypeDef",
     "WaterfallChartColorConfigurationTypeDef",
+    "CascadingControlConfigurationOutputTypeDef",
     "CascadingControlConfigurationTypeDef",
+    "DateTimeDefaultValuesOutputTypeDef",
     "DateTimeDefaultValuesTypeDef",
+    "DecimalDefaultValuesOutputTypeDef",
     "DecimalDefaultValuesTypeDef",
+    "IntegerDefaultValuesOutputTypeDef",
     "IntegerDefaultValuesTypeDef",
+    "StringDefaultValuesOutputTypeDef",
     "StringDefaultValuesTypeDef",
+    "DrillDownFilterOutputTypeDef",
     "AnalysisTypeDef",
     "DashboardVersionTypeDef",
     "AnalysisSourceEntityTypeDef",
     "DashboardSourceEntityTypeDef",
     "TemplateSourceEntityTypeDef",
     "AnonymousUserEmbeddingExperienceConfigurationTypeDef",
     "DescribeAssetBundleExportJobResponseTypeDef",
+    "AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef",
     "StartAssetBundleExportJobRequestRequestTypeDef",
+    "AssetBundleImportJobDashboardOverridePermissionsOutputTypeDef",
     "AssetBundleImportJobDashboardOverridePermissionsTypeDef",
+    "AssetBundleImportJobOverrideTagsOutputTypeDef",
     "AssetBundleImportJobOverrideTagsTypeDef",
-    "NumericAxisOptionsTypeDef",
-    "ClusterMarkerConfigurationTypeDef",
-    "TopicCategoryFilterTypeDef",
-    "TagColumnOperationTypeDef",
-    "DataSetConfigurationTypeDef",
-    "ConditionalFormattingIconTypeDef",
-    "DescribeDashboardPermissionsResponseTypeDef",
-    "UpdateDashboardPermissionsResponseTypeDef",
-    "ListDataSetsResponseTypeDef",
-    "SearchDataSetsResponseTypeDef",
     "CustomValuesConfigurationTypeDef",
     "DateTimeDatasetParameterTypeDef",
     "ParametersTypeDef",
     "OverrideDatasetParameterOperationTypeDef",
     "DrillDownFilterTypeDef",
     "CreateTopicRefreshScheduleRequestRequestTypeDef",
-    "DescribeTopicRefreshScheduleResponseTypeDef",
-    "TopicRefreshScheduleSummaryTypeDef",
+    "TopicRefreshScheduleUnionTypeDef",
     "UpdateTopicRefreshScheduleRequestRequestTypeDef",
     "ForecastScenarioTypeDef",
+    "NumericAxisOptionsOutputTypeDef",
+    "NumericAxisOptionsTypeDef",
+    "ClusterMarkerConfigurationTypeDef",
+    "TopicCategoryFilterOutputTypeDef",
+    "TopicCategoryFilterTypeDef",
+    "TagColumnOperationOutputTypeDef",
+    "TagColumnOperationTypeDef",
+    "ColumnGroupUnionTypeDef",
+    "DataSetConfigurationOutputTypeDef",
+    "DataSetConfigurationTypeDef",
+    "ConditionalFormattingIconTypeDef",
+    "ListDataSetsResponseTypeDef",
+    "SearchDataSetsResponseTypeDef",
+    "DestinationParameterValueConfigurationOutputTypeDef",
     "CustomContentConfigurationTypeDef",
     "DashboardPublishOptionsTypeDef",
     "DataPathColorTypeDef",
+    "DataPathSortOutputTypeDef",
     "DataPathSortTypeDef",
+    "PivotTableDataPathOptionOutputTypeDef",
     "PivotTableDataPathOptionTypeDef",
+    "PivotTableFieldCollapseStateTargetOutputTypeDef",
     "PivotTableFieldCollapseStateTargetTypeDef",
+    "DescribeDashboardPermissionsResponseTypeDef",
+    "UpdateDashboardPermissionsResponseTypeDef",
+    "ListTopicRefreshSchedulesResponseTypeDef",
     "DefaultFormattingTypeDef",
+    "CustomActionFilterOperationOutputTypeDef",
     "CustomActionFilterOperationTypeDef",
     "AxisLabelOptionsTypeDef",
+    "DataLabelOptionsOutputTypeDef",
     "DataLabelOptionsTypeDef",
     "FunnelChartDataLabelOptionsTypeDef",
     "LabelOptionsTypeDef",
     "PanelTitleOptionsTypeDef",
     "TableFieldCustomTextContentTypeDef",
+    "ForecastConfigurationOutputTypeDef",
     "DefaultFreeFormLayoutConfigurationTypeDef",
     "SnapshotUserConfigurationTypeDef",
+    "GeospatialHeatmapConfigurationOutputTypeDef",
     "GeospatialHeatmapConfigurationTypeDef",
     "GlobalTableBorderOptionsTypeDef",
+    "ConditionalFormattingGradientColorOutputTypeDef",
     "ConditionalFormattingGradientColorTypeDef",
     "DefaultGridLayoutConfigurationTypeDef",
+    "GridLayoutConfigurationOutputTypeDef",
     "GridLayoutConfigurationTypeDef",
     "RefreshConfigurationTypeDef",
     "DescribeIngestionResponseTypeDef",
     "ListIngestionsResponseTypeDef",
     "LogicalTableSourceTypeDef",
     "DataFieldSeriesItemTypeDef",
     "FieldSeriesItemTypeDef",
+    "LinkSharingConfigurationUnionTypeDef",
+    "CreateFolderRequestRequestTypeDef",
+    "UpdateAnalysisPermissionsRequestRequestTypeDef",
+    "UpdateDashboardPermissionsRequestRequestTypeDef",
+    "UpdateDataSetPermissionsRequestRequestTypeDef",
+    "UpdateDataSourcePermissionsRequestRequestTypeDef",
+    "UpdateFolderPermissionsRequestRequestTypeDef",
+    "UpdateTemplatePermissionsRequestRequestTypeDef",
+    "UpdateThemePermissionsRequestRequestTypeDef",
+    "UpdateTopicPermissionsRequestRequestTypeDef",
     "SheetStyleTypeDef",
+    "TopicNamedEntityOutputTypeDef",
     "TopicNamedEntityTypeDef",
     "DescribeNamespaceResponseTypeDef",
     "ListNamespacesResponseTypeDef",
     "ListVPCConnectionsResponseTypeDef",
     "DescribeVPCConnectionResponseTypeDef",
     "CurrencyDisplayFormatConfigurationTypeDef",
     "NumberDisplayFormatConfigurationTypeDef",
     "PercentageDisplayFormatConfigurationTypeDef",
     "AggregationFunctionTypeDef",
     "ScrollBarOptionsTypeDef",
     "TopicDateRangeFilterTypeDef",
     "TopicNumericRangeFilterTypeDef",
-    "DataSourceParametersPaginatorTypeDef",
+    "DataSourceParametersExtraOutputTypeDef",
+    "DataSourceParametersOutputTypeDef",
     "DataSourceParametersTypeDef",
+    "RefreshScheduleOutputTypeDef",
     "RefreshScheduleTypeDef",
     "RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef",
     "RegisteredUserDashboardEmbeddingConfigurationTypeDef",
+    "RowLevelPermissionTagConfigurationUnionTypeDef",
+    "SnapshotDestinationConfigurationOutputTypeDef",
     "SnapshotDestinationConfigurationTypeDef",
     "SnapshotJobS3ResultTypeDef",
+    "PhysicalTableOutputTypeDef",
     "PhysicalTableTypeDef",
     "SectionBasedLayoutCanvasSizeOptionsTypeDef",
+    "FilterScopeConfigurationOutputTypeDef",
     "FilterScopeConfigurationTypeDef",
+    "FreeFormLayoutElementOutputTypeDef",
     "FreeFormLayoutElementTypeDef",
+    "SnapshotFileGroupOutputTypeDef",
     "SnapshotFileGroupTypeDef",
+    "DatasetParameterOutputTypeDef",
+    "FilterCrossSheetControlOutputTypeDef",
     "FilterCrossSheetControlTypeDef",
+    "DateTimeParameterDeclarationOutputTypeDef",
     "DateTimeParameterDeclarationTypeDef",
+    "DecimalParameterDeclarationOutputTypeDef",
     "DecimalParameterDeclarationTypeDef",
+    "IntegerParameterDeclarationOutputTypeDef",
     "IntegerParameterDeclarationTypeDef",
+    "StringParameterDeclarationOutputTypeDef",
     "StringParameterDeclarationTypeDef",
+    "DateTimeHierarchyOutputTypeDef",
+    "ExplicitHierarchyOutputTypeDef",
+    "PredefinedHierarchyOutputTypeDef",
     "DescribeAnalysisResponseTypeDef",
     "DashboardTypeDef",
     "GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
+    "AssetBundleImportJobOverridePermissionsOutputTypeDef",
     "AssetBundleImportJobOverridePermissionsTypeDef",
-    "AxisDataOptionsTypeDef",
-    "TemplateVersionTypeDef",
+    "AssetBundleImportJobOverrideTagsUnionTypeDef",
     "DestinationParameterValueConfigurationTypeDef",
     "DatasetParameterTypeDef",
-    "TransformOperationTypeDef",
+    "ParametersUnionTypeDef",
     "DateTimeHierarchyTypeDef",
     "ExplicitHierarchyTypeDef",
     "PredefinedHierarchyTypeDef",
-    "ListTopicRefreshSchedulesResponseTypeDef",
     "ForecastConfigurationTypeDef",
+    "AxisDataOptionsOutputTypeDef",
+    "AxisDataOptionsTypeDef",
+    "TransformOperationOutputTypeDef",
+    "TransformOperationTypeDef",
+    "TemplateVersionTypeDef",
+    "SetParameterValueConfigurationOutputTypeDef",
+    "VisualPaletteOutputTypeDef",
     "VisualPaletteTypeDef",
+    "PivotTableFieldCollapseStateOptionOutputTypeDef",
     "PivotTableFieldCollapseStateOptionTypeDef",
+    "TopicCalculatedFieldOutputTypeDef",
     "TopicCalculatedFieldTypeDef",
+    "TopicColumnOutputTypeDef",
     "TopicColumnTypeDef",
+    "ChartAxisLabelOptionsOutputTypeDef",
     "ChartAxisLabelOptionsTypeDef",
     "AxisTickLabelOptionsTypeDef",
     "DateTimePickerControlDisplayOptionsTypeDef",
     "DropDownControlDisplayOptionsTypeDef",
     "LegendOptionsTypeDef",
     "ListControlDisplayOptionsTypeDef",
     "RelativeDateTimeControlDisplayOptionsTypeDef",
     "SliderControlDisplayOptionsTypeDef",
     "TextAreaControlDisplayOptionsTypeDef",
     "TextFieldControlDisplayOptionsTypeDef",
     "PanelConfigurationTypeDef",
     "TableFieldLinkContentConfigurationTypeDef",
+    "GeospatialPointStyleOptionsOutputTypeDef",
     "GeospatialPointStyleOptionsTypeDef",
     "TableCellStyleTypeDef",
+    "ConditionalFormattingColorOutputTypeDef",
     "ConditionalFormattingColorTypeDef",
     "DefaultInteractiveLayoutConfigurationTypeDef",
+    "SheetControlLayoutConfigurationOutputTypeDef",
     "SheetControlLayoutConfigurationTypeDef",
     "DataSetRefreshPropertiesTypeDef",
     "SeriesItemTypeDef",
+    "ThemeConfigurationOutputTypeDef",
     "ThemeConfigurationTypeDef",
     "ComparisonFormatConfigurationTypeDef",
     "NumericFormatConfigurationTypeDef",
     "AggregationSortConfigurationTypeDef",
     "ColumnSortTypeDef",
     "ColumnTooltipItemTypeDef",
     "ReferenceLineDynamicDataConfigurationTypeDef",
+    "TopicFilterOutputTypeDef",
     "TopicFilterTypeDef",
-    "DataSourcePaginatorTypeDef",
+    "AssetBundleImportJobDataSourceOverrideParametersOutputTypeDef",
+    "DataSourceTypeDef",
     "AssetBundleImportJobDataSourceOverrideParametersTypeDef",
     "CredentialPairTypeDef",
-    "DataSourceTypeDef",
-    "CreateRefreshScheduleRequestRequestTypeDef",
+    "DataSourceParametersUnionTypeDef",
     "DescribeRefreshScheduleResponseTypeDef",
     "ListRefreshSchedulesResponseTypeDef",
+    "CreateRefreshScheduleRequestRequestTypeDef",
+    "RefreshScheduleUnionTypeDef",
     "UpdateRefreshScheduleRequestRequestTypeDef",
     "RegisteredUserEmbeddingExperienceConfigurationTypeDef",
     "SnapshotJobResultFileGroupTypeDef",
+    "PhysicalTableUnionTypeDef",
     "DefaultSectionBasedLayoutConfigurationTypeDef",
+    "FreeFormLayoutConfigurationOutputTypeDef",
+    "FreeFormSectionLayoutConfigurationOutputTypeDef",
     "FreeFormLayoutConfigurationTypeDef",
     "FreeFormSectionLayoutConfigurationTypeDef",
+    "SnapshotConfigurationOutputTypeDef",
     "SnapshotConfigurationTypeDef",
+    "ParameterDeclarationOutputTypeDef",
     "ParameterDeclarationTypeDef",
+    "ColumnHierarchyOutputTypeDef",
     "DescribeDashboardResponseTypeDef",
-    "TemplateTypeDef",
+    "AssetBundleImportJobOverridePermissionsUnionTypeDef",
     "SetParameterValueConfigurationTypeDef",
-    "LogicalTableTypeDef",
+    "DatasetParameterUnionTypeDef",
     "ColumnHierarchyTypeDef",
+    "LogicalTableOutputTypeDef",
+    "LogicalTableTypeDef",
+    "TemplateTypeDef",
+    "CustomActionSetParametersOperationOutputTypeDef",
+    "PivotTableFieldOptionsOutputTypeDef",
     "PivotTableFieldOptionsTypeDef",
+    "AxisDisplayOptionsOutputTypeDef",
     "AxisDisplayOptionsTypeDef",
     "DefaultDateTimePickerControlOptionsTypeDef",
     "FilterDateTimePickerControlTypeDef",
     "ParameterDateTimePickerControlTypeDef",
+    "DefaultFilterDropDownControlOptionsOutputTypeDef",
     "DefaultFilterDropDownControlOptionsTypeDef",
+    "FilterDropDownControlOutputTypeDef",
     "FilterDropDownControlTypeDef",
+    "ParameterDropDownControlOutputTypeDef",
     "ParameterDropDownControlTypeDef",
+    "DefaultFilterListControlOptionsOutputTypeDef",
     "DefaultFilterListControlOptionsTypeDef",
+    "FilterListControlOutputTypeDef",
     "FilterListControlTypeDef",
+    "ParameterListControlOutputTypeDef",
     "ParameterListControlTypeDef",
     "DefaultRelativeDateTimeControlOptionsTypeDef",
     "FilterRelativeDateTimeControlTypeDef",
     "DefaultSliderControlOptionsTypeDef",
     "FilterSliderControlTypeDef",
     "ParameterSliderControlTypeDef",
     "DefaultTextAreaControlOptionsTypeDef",
     "FilterTextAreaControlTypeDef",
     "ParameterTextAreaControlTypeDef",
     "DefaultTextFieldControlOptionsTypeDef",
     "FilterTextFieldControlTypeDef",
     "ParameterTextFieldControlTypeDef",
     "SmallMultiplesOptionsTypeDef",
     "TableFieldLinkConfigurationTypeDef",
+    "PivotTableOptionsOutputTypeDef",
     "PivotTableOptionsTypeDef",
+    "PivotTotalOptionsOutputTypeDef",
     "PivotTotalOptionsTypeDef",
+    "SubtotalOptionsOutputTypeDef",
     "SubtotalOptionsTypeDef",
+    "TableOptionsOutputTypeDef",
     "TableOptionsTypeDef",
+    "TotalOptionsOutputTypeDef",
     "TotalOptionsTypeDef",
+    "GaugeChartArcConditionalFormattingOutputTypeDef",
+    "GaugeChartPrimaryValueConditionalFormattingOutputTypeDef",
+    "KPIActualValueConditionalFormattingOutputTypeDef",
+    "KPIComparisonValueConditionalFormattingOutputTypeDef",
+    "KPIPrimaryValueConditionalFormattingOutputTypeDef",
+    "KPIProgressBarConditionalFormattingOutputTypeDef",
+    "ShapeConditionalFormatOutputTypeDef",
+    "TableRowConditionalFormattingOutputTypeDef",
+    "TextConditionalFormatOutputTypeDef",
     "GaugeChartArcConditionalFormattingTypeDef",
     "GaugeChartPrimaryValueConditionalFormattingTypeDef",
     "KPIActualValueConditionalFormattingTypeDef",
     "KPIComparisonValueConditionalFormattingTypeDef",
     "KPIPrimaryValueConditionalFormattingTypeDef",
     "KPIProgressBarConditionalFormattingTypeDef",
     "ShapeConditionalFormatTypeDef",
     "TableRowConditionalFormattingTypeDef",
     "TextConditionalFormatTypeDef",
+    "SheetControlLayoutOutputTypeDef",
     "SheetControlLayoutTypeDef",
     "DescribeDataSetRefreshPropertiesResponseTypeDef",
     "PutDataSetRefreshPropertiesRequestRequestTypeDef",
-    "CreateThemeRequestRequestTypeDef",
     "ThemeVersionTypeDef",
+    "CreateThemeRequestRequestTypeDef",
+    "ThemeConfigurationUnionTypeDef",
     "UpdateThemeRequestRequestTypeDef",
     "ComparisonConfigurationTypeDef",
     "DateTimeFormatConfigurationTypeDef",
     "NumberFormatConfigurationTypeDef",
     "ReferenceLineValueLabelConfigurationTypeDef",
     "StringFormatConfigurationTypeDef",
     "FieldSortOptionsTypeDef",
+    "PivotTableSortByOutputTypeDef",
     "PivotTableSortByTypeDef",
     "TooltipItemTypeDef",
     "ReferenceLineDataConfigurationTypeDef",
+    "DatasetMetadataOutputTypeDef",
     "DatasetMetadataTypeDef",
-    "ListDataSourcesResponsePaginatorTypeDef",
-    "AssetBundleImportJobOverrideParametersTypeDef",
-    "DataSourceCredentialsTypeDef",
+    "AssetBundleImportJobOverrideParametersOutputTypeDef",
     "DescribeDataSourceResponseTypeDef",
     "ListDataSourcesResponseTypeDef",
+    "AssetBundleImportJobOverrideParametersTypeDef",
+    "DataSourceCredentialsTypeDef",
     "GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
     "AnonymousUserSnapshotJobResultTypeDef",
     "DefaultPaginatedLayoutConfigurationTypeDef",
+    "SectionLayoutConfigurationOutputTypeDef",
     "SectionLayoutConfigurationTypeDef",
     "DescribeDashboardSnapshotJobResponseTypeDef",
+    "SnapshotConfigurationUnionTypeDef",
     "StartDashboardSnapshotJobRequestRequestTypeDef",
-    "DescribeTemplateResponseTypeDef",
     "CustomActionSetParametersOperationTypeDef",
-    "CreateDataSetRequestRequestTypeDef",
     "DataSetTypeDef",
-    "UpdateDataSetRequestRequestTypeDef",
+    "LogicalTableUnionTypeDef",
+    "DescribeTemplateResponseTypeDef",
+    "VisualCustomActionOperationOutputTypeDef",
+    "LineSeriesAxisDisplayOptionsOutputTypeDef",
     "LineSeriesAxisDisplayOptionsTypeDef",
+    "DefaultFilterControlOptionsOutputTypeDef",
     "DefaultFilterControlOptionsTypeDef",
+    "FilterControlOutputTypeDef",
     "FilterControlTypeDef",
+    "ParameterControlOutputTypeDef",
     "ParameterControlTypeDef",
     "TableFieldURLConfigurationTypeDef",
+    "PivotTableTotalOptionsOutputTypeDef",
     "PivotTableTotalOptionsTypeDef",
+    "GaugeChartConditionalFormattingOptionOutputTypeDef",
+    "KPIConditionalFormattingOptionOutputTypeDef",
+    "FilledMapShapeConditionalFormattingOutputTypeDef",
+    "PivotTableCellConditionalFormattingOutputTypeDef",
+    "TableCellConditionalFormattingOutputTypeDef",
     "GaugeChartConditionalFormattingOptionTypeDef",
     "KPIConditionalFormattingOptionTypeDef",
     "FilledMapShapeConditionalFormattingTypeDef",
     "PivotTableCellConditionalFormattingTypeDef",
     "TableCellConditionalFormattingTypeDef",
     "ThemeTypeDef",
     "GaugeChartOptionsTypeDef",
@@ -1197,188 +1408,331 @@
     "DateMeasureFieldTypeDef",
     "NumericalDimensionFieldTypeDef",
     "NumericalMeasureFieldTypeDef",
     "ReferenceLineLabelConfigurationTypeDef",
     "CategoricalDimensionFieldTypeDef",
     "CategoricalMeasureFieldTypeDef",
     "FormatConfigurationTypeDef",
+    "BarChartSortConfigurationOutputTypeDef",
     "BarChartSortConfigurationTypeDef",
+    "BoxPlotSortConfigurationOutputTypeDef",
     "BoxPlotSortConfigurationTypeDef",
+    "ComboChartSortConfigurationOutputTypeDef",
     "ComboChartSortConfigurationTypeDef",
+    "FilledMapSortConfigurationOutputTypeDef",
     "FilledMapSortConfigurationTypeDef",
+    "FunnelChartSortConfigurationOutputTypeDef",
     "FunnelChartSortConfigurationTypeDef",
+    "HeatMapSortConfigurationOutputTypeDef",
     "HeatMapSortConfigurationTypeDef",
+    "KPISortConfigurationOutputTypeDef",
     "KPISortConfigurationTypeDef",
+    "LineChartSortConfigurationOutputTypeDef",
     "LineChartSortConfigurationTypeDef",
+    "PieChartSortConfigurationOutputTypeDef",
     "PieChartSortConfigurationTypeDef",
+    "RadarChartSortConfigurationOutputTypeDef",
     "RadarChartSortConfigurationTypeDef",
+    "SankeyDiagramSortConfigurationOutputTypeDef",
     "SankeyDiagramSortConfigurationTypeDef",
+    "TableSortConfigurationOutputTypeDef",
     "TableSortConfigurationTypeDef",
+    "TreeMapSortConfigurationOutputTypeDef",
     "TreeMapSortConfigurationTypeDef",
+    "WaterfallChartSortConfigurationOutputTypeDef",
     "WaterfallChartSortConfigurationTypeDef",
+    "WordCloudSortConfigurationOutputTypeDef",
     "WordCloudSortConfigurationTypeDef",
+    "PivotFieldSortOptionsOutputTypeDef",
     "PivotFieldSortOptionsTypeDef",
+    "FieldBasedTooltipOutputTypeDef",
     "FieldBasedTooltipTypeDef",
+    "TopicDetailsOutputTypeDef",
     "TopicDetailsTypeDef",
     "DescribeAssetBundleImportJobResponseTypeDef",
+    "AssetBundleImportJobOverrideParametersUnionTypeDef",
     "StartAssetBundleImportJobRequestRequestTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
     "SnapshotJobResultTypeDef",
     "DefaultNewSheetConfigurationTypeDef",
+    "BodySectionContentOutputTypeDef",
+    "HeaderFooterSectionConfigurationOutputTypeDef",
     "BodySectionContentTypeDef",
     "HeaderFooterSectionConfigurationTypeDef",
     "VisualCustomActionOperationTypeDef",
     "DescribeDataSetResponseTypeDef",
+    "CreateDataSetRequestRequestTypeDef",
+    "UpdateDataSetRequestRequestTypeDef",
+    "VisualCustomActionOutputTypeDef",
+    "DefaultFilterControlConfigurationOutputTypeDef",
     "DefaultFilterControlConfigurationTypeDef",
     "TableFieldOptionTypeDef",
+    "GaugeChartConditionalFormattingOutputTypeDef",
+    "KPIConditionalFormattingOutputTypeDef",
+    "FilledMapConditionalFormattingOptionOutputTypeDef",
+    "PivotTableConditionalFormattingOptionOutputTypeDef",
+    "TableConditionalFormattingOptionOutputTypeDef",
     "GaugeChartConditionalFormattingTypeDef",
     "KPIConditionalFormattingTypeDef",
     "FilledMapConditionalFormattingOptionTypeDef",
     "PivotTableConditionalFormattingOptionTypeDef",
     "TableConditionalFormattingOptionTypeDef",
     "DescribeThemeResponseTypeDef",
     "ReferenceLineTypeDef",
     "DimensionFieldTypeDef",
     "MeasureFieldTypeDef",
+    "ColumnConfigurationOutputTypeDef",
     "ColumnConfigurationTypeDef",
     "UnaggregatedFieldTypeDef",
+    "PivotTableSortConfigurationOutputTypeDef",
     "PivotTableSortConfigurationTypeDef",
+    "TooltipOptionsOutputTypeDef",
     "TooltipOptionsTypeDef",
-    "CreateTopicRequestRequestTypeDef",
     "DescribeTopicResponseTypeDef",
+    "CreateTopicRequestRequestTypeDef",
+    "TopicDetailsUnionTypeDef",
     "UpdateTopicRequestRequestTypeDef",
     "DescribeDashboardSnapshotJobResultResponseTypeDef",
     "AnalysisDefaultsTypeDef",
+    "BodySectionConfigurationOutputTypeDef",
     "BodySectionConfigurationTypeDef",
     "VisualCustomActionTypeDef",
+    "CustomContentVisualOutputTypeDef",
+    "EmptyVisualOutputTypeDef",
+    "CategoryFilterOutputTypeDef",
+    "NumericEqualityFilterOutputTypeDef",
+    "NumericRangeFilterOutputTypeDef",
+    "RelativeDatesFilterOutputTypeDef",
+    "TimeEqualityFilterOutputTypeDef",
+    "TimeRangeFilterOutputTypeDef",
+    "TopBottomFilterOutputTypeDef",
     "CategoryFilterTypeDef",
     "NumericEqualityFilterTypeDef",
     "NumericRangeFilterTypeDef",
     "RelativeDatesFilterTypeDef",
     "TimeEqualityFilterTypeDef",
     "TimeRangeFilterTypeDef",
     "TopBottomFilterTypeDef",
+    "TableFieldOptionsOutputTypeDef",
     "TableFieldOptionsTypeDef",
+    "FilledMapConditionalFormattingOutputTypeDef",
+    "PivotTableConditionalFormattingOutputTypeDef",
+    "TableConditionalFormattingOutputTypeDef",
     "FilledMapConditionalFormattingTypeDef",
     "PivotTableConditionalFormattingTypeDef",
     "TableConditionalFormattingTypeDef",
     "UniqueValuesComputationTypeDef",
+    "BarChartAggregatedFieldWellsOutputTypeDef",
     "BarChartAggregatedFieldWellsTypeDef",
+    "BoxPlotAggregatedFieldWellsOutputTypeDef",
     "BoxPlotAggregatedFieldWellsTypeDef",
+    "ComboChartAggregatedFieldWellsOutputTypeDef",
     "ComboChartAggregatedFieldWellsTypeDef",
+    "FilledMapAggregatedFieldWellsOutputTypeDef",
     "FilledMapAggregatedFieldWellsTypeDef",
     "ForecastComputationTypeDef",
+    "FunnelChartAggregatedFieldWellsOutputTypeDef",
     "FunnelChartAggregatedFieldWellsTypeDef",
+    "GaugeChartFieldWellsOutputTypeDef",
     "GaugeChartFieldWellsTypeDef",
+    "GeospatialMapAggregatedFieldWellsOutputTypeDef",
     "GeospatialMapAggregatedFieldWellsTypeDef",
     "GrowthRateComputationTypeDef",
+    "HeatMapAggregatedFieldWellsOutputTypeDef",
     "HeatMapAggregatedFieldWellsTypeDef",
+    "HistogramAggregatedFieldWellsOutputTypeDef",
     "HistogramAggregatedFieldWellsTypeDef",
+    "KPIFieldWellsOutputTypeDef",
     "KPIFieldWellsTypeDef",
+    "LineChartAggregatedFieldWellsOutputTypeDef",
     "LineChartAggregatedFieldWellsTypeDef",
     "MaximumMinimumComputationTypeDef",
     "MetricComparisonComputationTypeDef",
     "PeriodOverPeriodComputationTypeDef",
     "PeriodToDateComputationTypeDef",
+    "PieChartAggregatedFieldWellsOutputTypeDef",
     "PieChartAggregatedFieldWellsTypeDef",
+    "PivotTableAggregatedFieldWellsOutputTypeDef",
     "PivotTableAggregatedFieldWellsTypeDef",
+    "RadarChartAggregatedFieldWellsOutputTypeDef",
     "RadarChartAggregatedFieldWellsTypeDef",
+    "SankeyDiagramAggregatedFieldWellsOutputTypeDef",
     "SankeyDiagramAggregatedFieldWellsTypeDef",
+    "ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef",
     "ScatterPlotCategoricallyAggregatedFieldWellsTypeDef",
+    "ScatterPlotUnaggregatedFieldWellsOutputTypeDef",
     "ScatterPlotUnaggregatedFieldWellsTypeDef",
+    "TableAggregatedFieldWellsOutputTypeDef",
     "TableAggregatedFieldWellsTypeDef",
     "TopBottomMoversComputationTypeDef",
     "TopBottomRankedComputationTypeDef",
     "TotalAggregationComputationTypeDef",
+    "TreeMapAggregatedFieldWellsOutputTypeDef",
     "TreeMapAggregatedFieldWellsTypeDef",
+    "WaterfallChartAggregatedFieldWellsOutputTypeDef",
     "WaterfallChartAggregatedFieldWellsTypeDef",
+    "WordCloudAggregatedFieldWellsOutputTypeDef",
     "WordCloudAggregatedFieldWellsTypeDef",
+    "TableUnaggregatedFieldWellsOutputTypeDef",
     "TableUnaggregatedFieldWellsTypeDef",
+    "SectionBasedLayoutConfigurationOutputTypeDef",
     "SectionBasedLayoutConfigurationTypeDef",
     "CustomContentVisualTypeDef",
     "EmptyVisualTypeDef",
+    "FilterOutputTypeDef",
     "FilterTypeDef",
+    "BarChartFieldWellsOutputTypeDef",
     "BarChartFieldWellsTypeDef",
+    "BoxPlotFieldWellsOutputTypeDef",
     "BoxPlotFieldWellsTypeDef",
+    "ComboChartFieldWellsOutputTypeDef",
     "ComboChartFieldWellsTypeDef",
+    "FilledMapFieldWellsOutputTypeDef",
     "FilledMapFieldWellsTypeDef",
+    "FunnelChartFieldWellsOutputTypeDef",
     "FunnelChartFieldWellsTypeDef",
+    "GaugeChartConfigurationOutputTypeDef",
     "GaugeChartConfigurationTypeDef",
+    "GeospatialMapFieldWellsOutputTypeDef",
     "GeospatialMapFieldWellsTypeDef",
+    "HeatMapFieldWellsOutputTypeDef",
     "HeatMapFieldWellsTypeDef",
+    "HistogramFieldWellsOutputTypeDef",
     "HistogramFieldWellsTypeDef",
+    "KPIConfigurationOutputTypeDef",
     "KPIConfigurationTypeDef",
+    "LineChartFieldWellsOutputTypeDef",
     "LineChartFieldWellsTypeDef",
+    "PieChartFieldWellsOutputTypeDef",
     "PieChartFieldWellsTypeDef",
+    "PivotTableFieldWellsOutputTypeDef",
     "PivotTableFieldWellsTypeDef",
+    "RadarChartFieldWellsOutputTypeDef",
     "RadarChartFieldWellsTypeDef",
+    "SankeyDiagramFieldWellsOutputTypeDef",
     "SankeyDiagramFieldWellsTypeDef",
+    "ScatterPlotFieldWellsOutputTypeDef",
     "ScatterPlotFieldWellsTypeDef",
     "ComputationTypeDef",
+    "TreeMapFieldWellsOutputTypeDef",
     "TreeMapFieldWellsTypeDef",
+    "WaterfallChartFieldWellsOutputTypeDef",
     "WaterfallChartFieldWellsTypeDef",
+    "WordCloudFieldWellsOutputTypeDef",
     "WordCloudFieldWellsTypeDef",
+    "TableFieldWellsOutputTypeDef",
     "TableFieldWellsTypeDef",
+    "LayoutConfigurationOutputTypeDef",
     "LayoutConfigurationTypeDef",
+    "FilterGroupOutputTypeDef",
     "FilterGroupTypeDef",
+    "BarChartConfigurationOutputTypeDef",
     "BarChartConfigurationTypeDef",
+    "BoxPlotChartConfigurationOutputTypeDef",
     "BoxPlotChartConfigurationTypeDef",
+    "ComboChartConfigurationOutputTypeDef",
     "ComboChartConfigurationTypeDef",
+    "FilledMapConfigurationOutputTypeDef",
     "FilledMapConfigurationTypeDef",
+    "FunnelChartConfigurationOutputTypeDef",
     "FunnelChartConfigurationTypeDef",
+    "GaugeChartVisualOutputTypeDef",
     "GaugeChartVisualTypeDef",
+    "GeospatialMapConfigurationOutputTypeDef",
     "GeospatialMapConfigurationTypeDef",
+    "HeatMapConfigurationOutputTypeDef",
     "HeatMapConfigurationTypeDef",
+    "HistogramConfigurationOutputTypeDef",
     "HistogramConfigurationTypeDef",
+    "KPIVisualOutputTypeDef",
     "KPIVisualTypeDef",
+    "LineChartConfigurationOutputTypeDef",
     "LineChartConfigurationTypeDef",
+    "PieChartConfigurationOutputTypeDef",
     "PieChartConfigurationTypeDef",
+    "PivotTableConfigurationOutputTypeDef",
     "PivotTableConfigurationTypeDef",
+    "RadarChartConfigurationOutputTypeDef",
     "RadarChartConfigurationTypeDef",
+    "SankeyDiagramChartConfigurationOutputTypeDef",
     "SankeyDiagramChartConfigurationTypeDef",
+    "ScatterPlotConfigurationOutputTypeDef",
     "ScatterPlotConfigurationTypeDef",
+    "InsightConfigurationOutputTypeDef",
     "InsightConfigurationTypeDef",
+    "TreeMapConfigurationOutputTypeDef",
     "TreeMapConfigurationTypeDef",
+    "WaterfallChartConfigurationOutputTypeDef",
     "WaterfallChartConfigurationTypeDef",
+    "WordCloudChartConfigurationOutputTypeDef",
     "WordCloudChartConfigurationTypeDef",
+    "TableConfigurationOutputTypeDef",
     "TableConfigurationTypeDef",
+    "LayoutOutputTypeDef",
     "LayoutTypeDef",
+    "BarChartVisualOutputTypeDef",
     "BarChartVisualTypeDef",
+    "BoxPlotVisualOutputTypeDef",
     "BoxPlotVisualTypeDef",
+    "ComboChartVisualOutputTypeDef",
     "ComboChartVisualTypeDef",
+    "FilledMapVisualOutputTypeDef",
     "FilledMapVisualTypeDef",
+    "FunnelChartVisualOutputTypeDef",
     "FunnelChartVisualTypeDef",
+    "GeospatialMapVisualOutputTypeDef",
     "GeospatialMapVisualTypeDef",
+    "HeatMapVisualOutputTypeDef",
     "HeatMapVisualTypeDef",
+    "HistogramVisualOutputTypeDef",
     "HistogramVisualTypeDef",
+    "LineChartVisualOutputTypeDef",
     "LineChartVisualTypeDef",
+    "PieChartVisualOutputTypeDef",
     "PieChartVisualTypeDef",
+    "PivotTableVisualOutputTypeDef",
     "PivotTableVisualTypeDef",
+    "RadarChartVisualOutputTypeDef",
     "RadarChartVisualTypeDef",
+    "SankeyDiagramVisualOutputTypeDef",
     "SankeyDiagramVisualTypeDef",
+    "ScatterPlotVisualOutputTypeDef",
     "ScatterPlotVisualTypeDef",
+    "InsightVisualOutputTypeDef",
     "InsightVisualTypeDef",
+    "TreeMapVisualOutputTypeDef",
     "TreeMapVisualTypeDef",
+    "WaterfallVisualOutputTypeDef",
     "WaterfallVisualTypeDef",
+    "WordCloudVisualOutputTypeDef",
     "WordCloudVisualTypeDef",
+    "TableVisualOutputTypeDef",
     "TableVisualTypeDef",
+    "VisualOutputTypeDef",
     "VisualTypeDef",
+    "SheetDefinitionOutputTypeDef",
     "SheetDefinitionTypeDef",
+    "AnalysisDefinitionOutputTypeDef",
+    "DashboardVersionDefinitionOutputTypeDef",
+    "TemplateVersionDefinitionOutputTypeDef",
     "AnalysisDefinitionTypeDef",
     "DashboardVersionDefinitionTypeDef",
     "TemplateVersionDefinitionTypeDef",
-    "CreateAnalysisRequestRequestTypeDef",
     "DescribeAnalysisDefinitionResponseTypeDef",
+    "DescribeDashboardDefinitionResponseTypeDef",
+    "DescribeTemplateDefinitionResponseTypeDef",
+    "AnalysisDefinitionUnionTypeDef",
+    "CreateAnalysisRequestRequestTypeDef",
     "UpdateAnalysisRequestRequestTypeDef",
     "CreateDashboardRequestRequestTypeDef",
-    "DescribeDashboardDefinitionResponseTypeDef",
+    "DashboardVersionDefinitionUnionTypeDef",
     "UpdateDashboardRequestRequestTypeDef",
     "CreateTemplateRequestRequestTypeDef",
-    "DescribeTemplateDefinitionResponseTypeDef",
+    "TemplateVersionDefinitionUnionTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
 )
 
 AccountCustomizationTypeDef = TypedDict(
     "AccountCustomizationTypeDef",
     {
         "DefaultTheme": NotRequired[str],
@@ -1524,14 +1878,20 @@
     "DashboardVisualIdTypeDef",
     {
         "DashboardId": str,
         "SheetId": str,
         "VisualId": str,
     },
 )
+AnonymousUserGenerativeQnAEmbeddingConfigurationTypeDef = TypedDict(
+    "AnonymousUserGenerativeQnAEmbeddingConfigurationTypeDef",
+    {
+        "InitialTopicId": str,
+    },
+)
 AnonymousUserQSearchBarEmbeddingConfigurationTypeDef = TypedDict(
     "AnonymousUserQSearchBarEmbeddingConfigurationTypeDef",
     {
         "InitialTopicId": str,
     },
 )
 ArcAxisDisplayRangeTypeDef = TypedDict(
@@ -1550,67 +1910,116 @@
 )
 ArcOptionsTypeDef = TypedDict(
     "ArcOptionsTypeDef",
     {
         "ArcThickness": NotRequired[ArcThicknessType],
     },
 )
-AssetBundleExportJobAnalysisOverridePropertiesTypeDef = TypedDict(
-    "AssetBundleExportJobAnalysisOverridePropertiesTypeDef",
+AssetBundleExportJobAnalysisOverridePropertiesOutputTypeDef = TypedDict(
+    "AssetBundleExportJobAnalysisOverridePropertiesOutputTypeDef",
     {
         "Arn": str,
         "Properties": List[Literal["Name"]],
     },
 )
-AssetBundleExportJobDashboardOverridePropertiesTypeDef = TypedDict(
-    "AssetBundleExportJobDashboardOverridePropertiesTypeDef",
+AssetBundleExportJobDashboardOverridePropertiesOutputTypeDef = TypedDict(
+    "AssetBundleExportJobDashboardOverridePropertiesOutputTypeDef",
     {
         "Arn": str,
         "Properties": List[Literal["Name"]],
     },
 )
-AssetBundleExportJobDataSetOverridePropertiesTypeDef = TypedDict(
-    "AssetBundleExportJobDataSetOverridePropertiesTypeDef",
+AssetBundleExportJobDataSetOverridePropertiesOutputTypeDef = TypedDict(
+    "AssetBundleExportJobDataSetOverridePropertiesOutputTypeDef",
     {
         "Arn": str,
         "Properties": List[Literal["Name"]],
     },
 )
-AssetBundleExportJobDataSourceOverridePropertiesTypeDef = TypedDict(
-    "AssetBundleExportJobDataSourceOverridePropertiesTypeDef",
+AssetBundleExportJobDataSourceOverridePropertiesOutputTypeDef = TypedDict(
+    "AssetBundleExportJobDataSourceOverridePropertiesOutputTypeDef",
     {
         "Arn": str,
         "Properties": List[AssetBundleExportJobDataSourcePropertyToOverrideType],
     },
 )
-AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef = TypedDict(
-    "AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef",
+AssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef = TypedDict(
+    "AssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef",
     {
         "Arn": str,
         "Properties": List[Literal["StartAfterDateTime"]],
     },
 )
 AssetBundleExportJobResourceIdOverrideConfigurationTypeDef = TypedDict(
     "AssetBundleExportJobResourceIdOverrideConfigurationTypeDef",
     {
         "PrefixForAllResources": NotRequired[bool],
     },
 )
+AssetBundleExportJobThemeOverridePropertiesOutputTypeDef = TypedDict(
+    "AssetBundleExportJobThemeOverridePropertiesOutputTypeDef",
+    {
+        "Arn": str,
+        "Properties": List[Literal["Name"]],
+    },
+)
+AssetBundleExportJobVPCConnectionOverridePropertiesOutputTypeDef = TypedDict(
+    "AssetBundleExportJobVPCConnectionOverridePropertiesOutputTypeDef",
+    {
+        "Arn": str,
+        "Properties": List[AssetBundleExportJobVPCConnectionPropertyToOverrideType],
+    },
+)
+AssetBundleExportJobAnalysisOverridePropertiesTypeDef = TypedDict(
+    "AssetBundleExportJobAnalysisOverridePropertiesTypeDef",
+    {
+        "Arn": str,
+        "Properties": Sequence[Literal["Name"]],
+    },
+)
+AssetBundleExportJobDashboardOverridePropertiesTypeDef = TypedDict(
+    "AssetBundleExportJobDashboardOverridePropertiesTypeDef",
+    {
+        "Arn": str,
+        "Properties": Sequence[Literal["Name"]],
+    },
+)
+AssetBundleExportJobDataSetOverridePropertiesTypeDef = TypedDict(
+    "AssetBundleExportJobDataSetOverridePropertiesTypeDef",
+    {
+        "Arn": str,
+        "Properties": Sequence[Literal["Name"]],
+    },
+)
+AssetBundleExportJobDataSourceOverridePropertiesTypeDef = TypedDict(
+    "AssetBundleExportJobDataSourceOverridePropertiesTypeDef",
+    {
+        "Arn": str,
+        "Properties": Sequence[AssetBundleExportJobDataSourcePropertyToOverrideType],
+    },
+)
+AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef = TypedDict(
+    "AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef",
+    {
+        "Arn": str,
+        "Properties": Sequence[Literal["StartAfterDateTime"]],
+    },
+)
 AssetBundleExportJobThemeOverridePropertiesTypeDef = TypedDict(
     "AssetBundleExportJobThemeOverridePropertiesTypeDef",
     {
         "Arn": str,
-        "Properties": List[Literal["Name"]],
+        "Properties": Sequence[Literal["Name"]],
     },
 )
 AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef = TypedDict(
     "AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef",
     {
         "Arn": str,
-        "Properties": List[AssetBundleExportJobVPCConnectionPropertyToOverrideType],
+        "Properties": Sequence[AssetBundleExportJobVPCConnectionPropertyToOverrideType],
     },
 )
 AssetBundleExportJobErrorTypeDef = TypedDict(
     "AssetBundleExportJobErrorTypeDef",
     {
         "Arn": NotRequired[str],
         "Type": NotRequired[str],
@@ -1646,21 +2055,28 @@
 AssetBundleImportJobAnalysisOverrideParametersTypeDef = TypedDict(
     "AssetBundleImportJobAnalysisOverrideParametersTypeDef",
     {
         "AnalysisId": str,
         "Name": NotRequired[str],
     },
 )
-AssetBundleResourcePermissionsTypeDef = TypedDict(
-    "AssetBundleResourcePermissionsTypeDef",
+AssetBundleResourcePermissionsOutputTypeDef = TypedDict(
+    "AssetBundleResourcePermissionsOutputTypeDef",
     {
         "Principals": List[str],
         "Actions": List[str],
     },
 )
+AssetBundleResourcePermissionsTypeDef = TypedDict(
+    "AssetBundleResourcePermissionsTypeDef",
+    {
+        "Principals": Sequence[str],
+        "Actions": Sequence[str],
+    },
+)
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -1701,16 +2117,16 @@
     "AssetBundleImportJobErrorTypeDef",
     {
         "Arn": NotRequired[str],
         "Type": NotRequired[str],
         "Message": NotRequired[str],
     },
 )
-AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef = TypedDict(
-    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
+AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef = TypedDict(
+    "AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef",
     {
         "DataSetId": str,
         "ScheduleId": str,
         "StartAfterDateTime": NotRequired[datetime],
     },
 )
 AssetBundleImportJobResourceIdOverrideConfigurationTypeDef = TypedDict(
@@ -1722,31 +2138,43 @@
 AssetBundleImportJobThemeOverrideParametersTypeDef = TypedDict(
     "AssetBundleImportJobThemeOverrideParametersTypeDef",
     {
         "ThemeId": str,
         "Name": NotRequired[str],
     },
 )
-AssetBundleImportJobVPCConnectionOverrideParametersTypeDef = TypedDict(
-    "AssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
+AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef = TypedDict(
+    "AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef",
     {
         "VPCConnectionId": str,
         "Name": NotRequired[str],
         "SubnetIds": NotRequired[List[str]],
         "SecurityGroupIds": NotRequired[List[str]],
         "DnsResolvers": NotRequired[List[str]],
         "RoleArn": NotRequired[str],
     },
 )
+AssetBundleImportJobVPCConnectionOverrideParametersTypeDef = TypedDict(
+    "AssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
+    {
+        "VPCConnectionId": str,
+        "Name": NotRequired[str],
+        "SubnetIds": NotRequired[Sequence[str]],
+        "SecurityGroupIds": NotRequired[Sequence[str]],
+        "DnsResolvers": NotRequired[Sequence[str]],
+        "RoleArn": NotRequired[str],
+    },
+)
 AssetBundleImportJobOverrideValidationStrategyTypeDef = TypedDict(
     "AssetBundleImportJobOverrideValidationStrategyTypeDef",
     {
         "StrictModeForAllResources": NotRequired[bool],
     },
 )
+TimestampTypeDef = Union[datetime, str]
 AssetBundleImportJobSummaryTypeDef = TypedDict(
     "AssetBundleImportJobSummaryTypeDef",
     {
         "JobStatus": NotRequired[AssetBundleImportJobStatusType],
         "Arn": NotRequired[str],
         "CreatedTime": NotRequired[datetime],
         "AssetBundleImportJobId": NotRequired[str],
@@ -1930,14 +2358,32 @@
         "MatchOperator": CategoryFilterMatchOperatorType,
         "NullOption": FilterNullOptionType,
         "CategoryValue": NotRequired[str],
         "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
         "ParameterName": NotRequired[str],
     },
 )
+CustomFilterListConfigurationOutputTypeDef = TypedDict(
+    "CustomFilterListConfigurationOutputTypeDef",
+    {
+        "MatchOperator": CategoryFilterMatchOperatorType,
+        "NullOption": FilterNullOptionType,
+        "CategoryValues": NotRequired[List[str]],
+        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
+    },
+)
+FilterListConfigurationOutputTypeDef = TypedDict(
+    "FilterListConfigurationOutputTypeDef",
+    {
+        "MatchOperator": CategoryFilterMatchOperatorType,
+        "CategoryValues": NotRequired[List[str]],
+        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
+        "NullOption": NotRequired[FilterNullOptionType],
+    },
+)
 CustomFilterListConfigurationTypeDef = TypedDict(
     "CustomFilterListConfigurationTypeDef",
     {
         "MatchOperator": CategoryFilterMatchOperatorType,
         "NullOption": FilterNullOptionType,
         "CategoryValues": NotRequired[Sequence[str]],
         "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
@@ -1948,27 +2394,40 @@
     {
         "MatchOperator": CategoryFilterMatchOperatorType,
         "CategoryValues": NotRequired[Sequence[str]],
         "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
         "NullOption": NotRequired[FilterNullOptionType],
     },
 )
+CellValueSynonymOutputTypeDef = TypedDict(
+    "CellValueSynonymOutputTypeDef",
+    {
+        "CellValue": NotRequired[str],
+        "Synonyms": NotRequired[List[str]],
+    },
+)
 CellValueSynonymTypeDef = TypedDict(
     "CellValueSynonymTypeDef",
     {
         "CellValue": NotRequired[str],
         "Synonyms": NotRequired[Sequence[str]],
     },
 )
 SimpleClusterMarkerTypeDef = TypedDict(
     "SimpleClusterMarkerTypeDef",
     {
         "Color": NotRequired[str],
     },
 )
+CollectiveConstantOutputTypeDef = TypedDict(
+    "CollectiveConstantOutputTypeDef",
+    {
+        "ValueList": NotRequired[List[str]],
+    },
+)
 CollectiveConstantTypeDef = TypedDict(
     "CollectiveConstantTypeDef",
     {
         "ValueList": NotRequired[Sequence[str]],
     },
 )
 DataColorTypeDef = TypedDict(
@@ -1994,22 +2453,37 @@
 )
 ColumnGroupColumnSchemaTypeDef = TypedDict(
     "ColumnGroupColumnSchemaTypeDef",
     {
         "Name": NotRequired[str],
     },
 )
+GeoSpatialColumnGroupOutputTypeDef = TypedDict(
+    "GeoSpatialColumnGroupOutputTypeDef",
+    {
+        "Name": str,
+        "Columns": List[str],
+        "CountryCode": NotRequired[Literal["US"]],
+    },
+)
 GeoSpatialColumnGroupTypeDef = TypedDict(
     "GeoSpatialColumnGroupTypeDef",
     {
         "Name": str,
         "Columns": Sequence[str],
         "CountryCode": NotRequired[Literal["US"]],
     },
 )
+ColumnLevelPermissionRuleOutputTypeDef = TypedDict(
+    "ColumnLevelPermissionRuleOutputTypeDef",
+    {
+        "Principals": NotRequired[List[str]],
+        "ColumnNames": NotRequired[List[str]],
+    },
+)
 ColumnLevelPermissionRuleTypeDef = TypedDict(
     "ColumnLevelPermissionRuleTypeDef",
     {
         "Principals": NotRequired[Sequence[str]],
         "ColumnNames": NotRequired[Sequence[str]],
     },
 )
@@ -2017,14 +2491,22 @@
     "ColumnSchemaTypeDef",
     {
         "Name": NotRequired[str],
         "DataType": NotRequired[str],
         "GeographicRole": NotRequired[str],
     },
 )
+ComparativeOrderOutputTypeDef = TypedDict(
+    "ComparativeOrderOutputTypeDef",
+    {
+        "UseOrdering": NotRequired[ColumnOrderingTypeType],
+        "SpecifedOrder": NotRequired[List[str]],
+        "TreatUndefinedSpecifiedValues": NotRequired[UndefinedSpecifiedValueTypeType],
+    },
+)
 ComparativeOrderTypeDef = TypedDict(
     "ComparativeOrderTypeDef",
     {
         "UseOrdering": NotRequired[ColumnOrderingTypeType],
         "SpecifedOrder": NotRequired[Sequence[str]],
         "TreatUndefinedSpecifiedValues": NotRequired[UndefinedSpecifiedValueTypeType],
     },
@@ -2061,25 +2543,28 @@
     {
         "AvailabilityStatus": NotRequired[DashboardBehaviorType],
     },
 )
 CreateAccountSubscriptionRequestRequestTypeDef = TypedDict(
     "CreateAccountSubscriptionRequestRequestTypeDef",
     {
-        "Edition": EditionType,
         "AuthenticationMethod": AuthenticationMethodOptionType,
         "AwsAccountId": str,
         "AccountName": str,
         "NotificationEmail": str,
+        "Edition": NotRequired[EditionType],
         "ActiveDirectoryName": NotRequired[str],
         "Realm": NotRequired[str],
         "DirectoryId": NotRequired[str],
         "AdminGroup": NotRequired[Sequence[str]],
         "AuthorGroup": NotRequired[Sequence[str]],
         "ReaderGroup": NotRequired[Sequence[str]],
+        "AdminProGroup": NotRequired[Sequence[str]],
+        "AuthorProGroup": NotRequired[Sequence[str]],
+        "ReaderProGroup": NotRequired[Sequence[str]],
         "FirstName": NotRequired[str],
         "LastName": NotRequired[str],
         "EmailAddress": NotRequired[str],
         "ContactNumber": NotRequired[str],
         "IAMIdentityCenterInstanceArn": NotRequired[str],
     },
 )
@@ -2088,41 +2573,27 @@
     {
         "IAMUser": NotRequired[bool],
         "userLoginName": NotRequired[str],
         "accountName": NotRequired[str],
         "directoryType": NotRequired[str],
     },
 )
-ResourcePermissionTypeDef = TypedDict(
-    "ResourcePermissionTypeDef",
-    {
-        "Principal": str,
-        "Actions": Sequence[str],
-    },
-)
 ValidationStrategyTypeDef = TypedDict(
     "ValidationStrategyTypeDef",
     {
         "Mode": ValidationStrategyModeType,
     },
 )
 DataSetUsageConfigurationTypeDef = TypedDict(
     "DataSetUsageConfigurationTypeDef",
     {
         "DisableUseAsDirectQuerySource": NotRequired[bool],
         "DisableUseAsImportedSource": NotRequired[bool],
     },
 )
-FieldFolderTypeDef = TypedDict(
-    "FieldFolderTypeDef",
-    {
-        "description": NotRequired[str],
-        "columns": NotRequired[Sequence[str]],
-    },
-)
 RowLevelPermissionDataSetTypeDef = TypedDict(
     "RowLevelPermissionDataSetTypeDef",
     {
         "Arn": str,
         "PermissionPolicy": RowLevelPermissionPolicyType,
         "Namespace": NotRequired[str],
         "FormatVersion": NotRequired[RowLevelPermissionFormatVersionType],
@@ -2275,15 +2746,23 @@
 )
 CustomNarrativeOptionsTypeDef = TypedDict(
     "CustomNarrativeOptionsTypeDef",
     {
         "Narrative": str,
     },
 )
-TimestampTypeDef = Union[datetime, str]
+CustomParameterValuesOutputTypeDef = TypedDict(
+    "CustomParameterValuesOutputTypeDef",
+    {
+        "StringValues": NotRequired[List[str]],
+        "IntegerValues": NotRequired[List[int]],
+        "DecimalValues": NotRequired[List[float]],
+        "DateTimeValues": NotRequired[List[datetime]],
+    },
+)
 InputColumnTypeDef = TypedDict(
     "InputColumnTypeDef",
     {
         "Name": str,
         "Type": InputColumnDataTypeType,
         "SubType": NotRequired[ColumnDataSubTypeType],
     },
@@ -2390,14 +2869,22 @@
     "DataBarsOptionsTypeDef",
     {
         "FieldId": str,
         "PositiveColor": NotRequired[str],
         "NegativeColor": NotRequired[str],
     },
 )
+DataColorPaletteOutputTypeDef = TypedDict(
+    "DataColorPaletteOutputTypeDef",
+    {
+        "Colors": NotRequired[List[str]],
+        "MinMaxGradient": NotRequired[List[str]],
+        "EmptyFillColor": NotRequired[str],
+    },
+)
 DataColorPaletteTypeDef = TypedDict(
     "DataColorPaletteTypeDef",
     {
         "Colors": NotRequired[Sequence[str]],
         "MinMaxGradient": NotRequired[Sequence[str]],
         "EmptyFillColor": NotRequired[str],
     },
@@ -2445,14 +2932,21 @@
     "DataSetSearchFilterTypeDef",
     {
         "Operator": FilterOperatorType,
         "Name": DataSetFilterAttributeType,
         "Value": str,
     },
 )
+FieldFolderOutputTypeDef = TypedDict(
+    "FieldFolderOutputTypeDef",
+    {
+        "description": NotRequired[str],
+        "columns": NotRequired[List[str]],
+    },
+)
 OutputColumnTypeDef = TypedDict(
     "OutputColumnTypeDef",
     {
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "Type": NotRequired[ColumnDataTypeType],
         "SubType": NotRequired[ColumnDataSubTypeType],
@@ -2609,55 +3103,94 @@
         "DataSourceId": NotRequired[str],
         "Name": NotRequired[str],
         "Type": NotRequired[DataSourceTypeType],
         "CreatedTime": NotRequired[datetime],
         "LastUpdatedTime": NotRequired[datetime],
     },
 )
+DateTimeDatasetParameterDefaultValuesOutputTypeDef = TypedDict(
+    "DateTimeDatasetParameterDefaultValuesOutputTypeDef",
+    {
+        "StaticValues": NotRequired[List[datetime]],
+    },
+)
 RollingDateConfigurationTypeDef = TypedDict(
     "RollingDateConfigurationTypeDef",
     {
         "Expression": str,
         "DataSetIdentifier": NotRequired[str],
     },
 )
+DateTimeValueWhenUnsetConfigurationOutputTypeDef = TypedDict(
+    "DateTimeValueWhenUnsetConfigurationOutputTypeDef",
+    {
+        "ValueWhenUnsetOption": NotRequired[ValueWhenUnsetOptionType],
+        "CustomValue": NotRequired[datetime],
+    },
+)
 MappedDataSetParameterTypeDef = TypedDict(
     "MappedDataSetParameterTypeDef",
     {
         "DataSetIdentifier": str,
         "DataSetParameterName": str,
     },
 )
+DateTimeParameterOutputTypeDef = TypedDict(
+    "DateTimeParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Values": List[datetime],
+    },
+)
 SheetControlInfoIconLabelOptionsTypeDef = TypedDict(
     "SheetControlInfoIconLabelOptionsTypeDef",
     {
         "Visibility": NotRequired[VisibilityType],
         "InfoIconText": NotRequired[str],
     },
 )
+DecimalDatasetParameterDefaultValuesOutputTypeDef = TypedDict(
+    "DecimalDatasetParameterDefaultValuesOutputTypeDef",
+    {
+        "StaticValues": NotRequired[List[float]],
+    },
+)
 DecimalDatasetParameterDefaultValuesTypeDef = TypedDict(
     "DecimalDatasetParameterDefaultValuesTypeDef",
     {
         "StaticValues": NotRequired[Sequence[float]],
     },
 )
 DecimalValueWhenUnsetConfigurationTypeDef = TypedDict(
     "DecimalValueWhenUnsetConfigurationTypeDef",
     {
         "ValueWhenUnsetOption": NotRequired[ValueWhenUnsetOptionType],
         "CustomValue": NotRequired[float],
     },
 )
+DecimalParameterOutputTypeDef = TypedDict(
+    "DecimalParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Values": List[float],
+    },
+)
 DecimalParameterTypeDef = TypedDict(
     "DecimalParameterTypeDef",
     {
         "Name": str,
         "Values": Sequence[float],
     },
 )
+FilterSelectableValuesOutputTypeDef = TypedDict(
+    "FilterSelectableValuesOutputTypeDef",
+    {
+        "Values": NotRequired[List[str]],
+    },
+)
 FilterSelectableValuesTypeDef = TypedDict(
     "FilterSelectableValuesTypeDef",
     {
         "Values": NotRequired[Sequence[str]],
     },
 )
 DeleteAccountCustomizationRequestRequestTypeDef = TypedDict(
@@ -2891,14 +3424,21 @@
 DescribeAnalysisPermissionsRequestRequestTypeDef = TypedDict(
     "DescribeAnalysisPermissionsRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
+ResourcePermissionOutputTypeDef = TypedDict(
+    "ResourcePermissionOutputTypeDef",
+    {
+        "Principal": str,
+        "Actions": List[str],
+    },
+)
 DescribeAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
@@ -3013,16 +3553,16 @@
         "AwsAccountId": str,
         "FolderId": str,
         "Namespace": NotRequired[str],
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
-ResourcePermissionPaginatorTypeDef = TypedDict(
-    "ResourcePermissionPaginatorTypeDef",
+ResourcePermissionExtraOutputTypeDef = TypedDict(
+    "ResourcePermissionExtraOutputTypeDef",
     {
         "Principal": str,
         "Actions": List[str],
     },
 )
 DescribeFolderRequestRequestTypeDef = TypedDict(
     "DescribeFolderRequestRequestTypeDef",
@@ -3211,14 +3751,25 @@
     "DescribeTopicRefreshScheduleRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TopicId": str,
         "DatasetId": str,
     },
 )
+TopicRefreshScheduleOutputTypeDef = TypedDict(
+    "TopicRefreshScheduleOutputTypeDef",
+    {
+        "IsEnabled": bool,
+        "BasedOnSpiceSchedule": bool,
+        "StartingAt": NotRequired[datetime],
+        "Timezone": NotRequired[str],
+        "RepeatAt": NotRequired[str],
+        "TopicScheduleType": NotRequired[TopicScheduleTypeType],
+    },
+)
 DescribeTopicRequestRequestTypeDef = TypedDict(
     "DescribeTopicRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TopicId": str,
     },
 )
@@ -3283,14 +3834,21 @@
     "ExcludePeriodConfigurationTypeDef",
     {
         "Amount": int,
         "Granularity": TimeGranularityType,
         "Status": NotRequired[WidgetStatusType],
     },
 )
+FieldFolderTypeDef = TypedDict(
+    "FieldFolderTypeDef",
+    {
+        "description": NotRequired[str],
+        "columns": NotRequired[Sequence[str]],
+    },
+)
 FieldSortTypeDef = TypedDict(
     "FieldSortTypeDef",
     {
         "FieldId": str,
         "Direction": SortDirectionType,
     },
 )
@@ -3305,14 +3863,21 @@
 )
 GeospatialMapStyleOptionsTypeDef = TypedDict(
     "GeospatialMapStyleOptionsTypeDef",
     {
         "BaseMapStyle": NotRequired[BaseMapStyleTypeType],
     },
 )
+SameSheetTargetVisualConfigurationOutputTypeDef = TypedDict(
+    "SameSheetTargetVisualConfigurationOutputTypeDef",
+    {
+        "TargetVisuals": NotRequired[List[str]],
+        "TargetVisualOptions": NotRequired[Literal["ALL_VISUALS"]],
+    },
+)
 SameSheetTargetVisualConfigurationTypeDef = TypedDict(
     "SameSheetTargetVisualConfigurationTypeDef",
     {
         "TargetVisuals": NotRequired[Sequence[str]],
         "TargetVisualOptions": NotRequired[Literal["ALL_VISUALS"]],
     },
 )
@@ -3367,14 +3932,29 @@
         "PeriodsBackward": NotRequired[int],
         "UpperBoundary": NotRequired[float],
         "LowerBoundary": NotRequired[float],
         "PredictionInterval": NotRequired[int],
         "Seasonality": NotRequired[int],
     },
 )
+WhatIfPointScenarioOutputTypeDef = TypedDict(
+    "WhatIfPointScenarioOutputTypeDef",
+    {
+        "Date": datetime,
+        "Value": float,
+    },
+)
+WhatIfRangeScenarioOutputTypeDef = TypedDict(
+    "WhatIfRangeScenarioOutputTypeDef",
+    {
+        "StartDate": datetime,
+        "EndDate": datetime,
+        "Value": float,
+    },
+)
 FreeFormLayoutScreenCanvasSizeOptionsTypeDef = TypedDict(
     "FreeFormLayoutScreenCanvasSizeOptionsTypeDef",
     {
         "OptimizedViewPortWidth": str,
     },
 )
 FreeFormLayoutElementBackgroundStyleTypeDef = TypedDict(
@@ -3393,14 +3973,21 @@
 )
 LoadingAnimationTypeDef = TypedDict(
     "LoadingAnimationTypeDef",
     {
         "Visibility": NotRequired[VisibilityType],
     },
 )
+GaugeChartColorConfigurationTypeDef = TypedDict(
+    "GaugeChartColorConfigurationTypeDef",
+    {
+        "ForegroundColor": NotRequired[str],
+        "BackgroundColor": NotRequired[str],
+    },
+)
 SessionTagTypeDef = TypedDict(
     "SessionTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -3523,27 +4110,40 @@
     "RowInfoTypeDef",
     {
         "RowsIngested": NotRequired[int],
         "RowsDropped": NotRequired[int],
         "TotalRowsInDataset": NotRequired[int],
     },
 )
+IntegerDatasetParameterDefaultValuesOutputTypeDef = TypedDict(
+    "IntegerDatasetParameterDefaultValuesOutputTypeDef",
+    {
+        "StaticValues": NotRequired[List[int]],
+    },
+)
 IntegerDatasetParameterDefaultValuesTypeDef = TypedDict(
     "IntegerDatasetParameterDefaultValuesTypeDef",
     {
         "StaticValues": NotRequired[Sequence[int]],
     },
 )
 IntegerValueWhenUnsetConfigurationTypeDef = TypedDict(
     "IntegerValueWhenUnsetConfigurationTypeDef",
     {
         "ValueWhenUnsetOption": NotRequired[ValueWhenUnsetOptionType],
         "CustomValue": NotRequired[int],
     },
 )
+IntegerParameterOutputTypeDef = TypedDict(
+    "IntegerParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Values": List[int],
+    },
+)
 IntegerParameterTypeDef = TypedDict(
     "IntegerParameterTypeDef",
     {
         "Name": str,
         "Values": Sequence[int],
     },
 )
@@ -3606,14 +4206,21 @@
 )
 MissingDataConfigurationTypeDef = TypedDict(
     "MissingDataConfigurationTypeDef",
     {
         "TreatmentOption": NotRequired[MissingDataTreatmentOptionType],
     },
 )
+ResourcePermissionTypeDef = TypedDict(
+    "ResourcePermissionTypeDef",
+    {
+        "Principal": str,
+        "Actions": Sequence[str],
+    },
+)
 ListAnalysesRequestRequestTypeDef = TypedDict(
     "ListAnalysesRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
     },
@@ -3896,14 +4503,15 @@
 )
 TopicSummaryTypeDef = TypedDict(
     "TopicSummaryTypeDef",
     {
         "Arn": NotRequired[str],
         "TopicId": NotRequired[str],
         "Name": NotRequired[str],
+        "UserExperienceVersion": NotRequired[TopicUserExperienceVersionType],
     },
 )
 ListUserGroupsRequestRequestTypeDef = TypedDict(
     "ListUserGroupsRequestRequestTypeDef",
     {
         "UserName": str,
         "AwsAccountId": str,
@@ -3945,14 +4553,21 @@
 )
 MarginStyleTypeDef = TypedDict(
     "MarginStyleTypeDef",
     {
         "Show": NotRequired[bool],
     },
 )
+NamedEntityDefinitionMetricOutputTypeDef = TypedDict(
+    "NamedEntityDefinitionMetricOutputTypeDef",
+    {
+        "Aggregation": NotRequired[NamedEntityAggTypeType],
+        "AggregationFunctionParameters": NotRequired[Dict[str, str]],
+    },
+)
 NamedEntityDefinitionMetricTypeDef = TypedDict(
     "NamedEntityDefinitionMetricTypeDef",
     {
         "Aggregation": NotRequired[NamedEntityAggTypeType],
         "AggregationFunctionParameters": NotRequired[Mapping[str, str]],
     },
 )
@@ -3969,14 +4584,23 @@
         "SubnetId": NotRequired[str],
         "AvailabilityZone": NotRequired[str],
         "ErrorMessage": NotRequired[str],
         "Status": NotRequired[NetworkInterfaceStatusType],
         "NetworkInterfaceId": NotRequired[str],
     },
 )
+NewDefaultValuesOutputTypeDef = TypedDict(
+    "NewDefaultValuesOutputTypeDef",
+    {
+        "StringStaticValues": NotRequired[List[str]],
+        "DecimalStaticValues": NotRequired[List[float]],
+        "DateTimeStaticValues": NotRequired[List[datetime]],
+        "IntegerStaticValues": NotRequired[List[int]],
+    },
+)
 NumericRangeFilterValueTypeDef = TypedDict(
     "NumericRangeFilterValueTypeDef",
     {
         "StaticValue": NotRequired[float],
         "Parameter": NotRequired[str],
     },
 )
@@ -3989,14 +4613,21 @@
 )
 PercentileAggregationTypeDef = TypedDict(
     "PercentileAggregationTypeDef",
     {
         "PercentileValue": NotRequired[float],
     },
 )
+StringParameterOutputTypeDef = TypedDict(
+    "StringParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Values": List[str],
+    },
+)
 StringParameterTypeDef = TypedDict(
     "StringParameterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
@@ -4037,22 +4668,36 @@
 PivotTableRowsLabelOptionsTypeDef = TypedDict(
     "PivotTableRowsLabelOptionsTypeDef",
     {
         "Visibility": NotRequired[VisibilityType],
         "CustomLabel": NotRequired[str],
     },
 )
+RowAlternateColorOptionsOutputTypeDef = TypedDict(
+    "RowAlternateColorOptionsOutputTypeDef",
+    {
+        "Status": NotRequired[WidgetStatusType],
+        "RowAlternateColors": NotRequired[List[str]],
+        "UsePrimaryBackgroundColor": NotRequired[WidgetStatusType],
+    },
+)
 RowAlternateColorOptionsTypeDef = TypedDict(
     "RowAlternateColorOptionsTypeDef",
     {
         "Status": NotRequired[WidgetStatusType],
         "RowAlternateColors": NotRequired[Sequence[str]],
         "UsePrimaryBackgroundColor": NotRequired[WidgetStatusType],
     },
 )
+ProjectOperationOutputTypeDef = TypedDict(
+    "ProjectOperationOutputTypeDef",
+    {
+        "ProjectedColumns": List[str],
+    },
+)
 ProjectOperationTypeDef = TypedDict(
     "ProjectOperationTypeDef",
     {
         "ProjectedColumns": Sequence[str],
     },
 )
 RadarChartAreaStyleSettingsTypeDef = TypedDict(
@@ -4064,16 +4709,25 @@
 RangeConstantTypeDef = TypedDict(
     "RangeConstantTypeDef",
     {
         "Minimum": NotRequired[str],
         "Maximum": NotRequired[str],
     },
 )
-RedshiftIAMParametersPaginatorTypeDef = TypedDict(
-    "RedshiftIAMParametersPaginatorTypeDef",
+RedshiftIAMParametersExtraOutputTypeDef = TypedDict(
+    "RedshiftIAMParametersExtraOutputTypeDef",
+    {
+        "RoleArn": str,
+        "DatabaseUser": str,
+        "DatabaseGroups": NotRequired[List[str]],
+        "AutoCreateDatabaseUser": NotRequired[bool],
+    },
+)
+RedshiftIAMParametersOutputTypeDef = TypedDict(
+    "RedshiftIAMParametersOutputTypeDef",
     {
         "RoleArn": str,
         "DatabaseUser": str,
         "DatabaseGroups": NotRequired[List[str]],
         "AutoCreateDatabaseUser": NotRequired[bool],
     },
 )
@@ -4114,14 +4768,20 @@
 )
 StatePersistenceConfigurationsTypeDef = TypedDict(
     "StatePersistenceConfigurationsTypeDef",
     {
         "Enabled": bool,
     },
 )
+RegisteredUserGenerativeQnAEmbeddingConfigurationTypeDef = TypedDict(
+    "RegisteredUserGenerativeQnAEmbeddingConfigurationTypeDef",
+    {
+        "InitialTopicId": NotRequired[str],
+    },
+)
 RegisteredUserQSearchBarEmbeddingConfigurationTypeDef = TypedDict(
     "RegisteredUserQSearchBarEmbeddingConfigurationTypeDef",
     {
         "InitialTopicId": NotRequired[str],
     },
 )
 RenameColumnOperationTypeDef = TypedDict(
@@ -4176,30 +4836,58 @@
     {
         "Top": NotRequired[str],
         "Bottom": NotRequired[str],
         "Left": NotRequired[str],
         "Right": NotRequired[str],
     },
 )
+SheetVisualScopingConfigurationOutputTypeDef = TypedDict(
+    "SheetVisualScopingConfigurationOutputTypeDef",
+    {
+        "SheetId": str,
+        "Scope": FilterVisualScopeType,
+        "VisualIds": NotRequired[List[str]],
+    },
+)
 SheetVisualScopingConfigurationTypeDef = TypedDict(
     "SheetVisualScopingConfigurationTypeDef",
     {
         "SheetId": str,
         "Scope": FilterVisualScopeType,
         "VisualIds": NotRequired[Sequence[str]],
     },
 )
+SemanticEntityTypeOutputTypeDef = TypedDict(
+    "SemanticEntityTypeOutputTypeDef",
+    {
+        "TypeName": NotRequired[str],
+        "SubTypeName": NotRequired[str],
+        "TypeParameters": NotRequired[Dict[str, str]],
+    },
+)
 SemanticEntityTypeTypeDef = TypedDict(
     "SemanticEntityTypeTypeDef",
     {
         "TypeName": NotRequired[str],
         "SubTypeName": NotRequired[str],
         "TypeParameters": NotRequired[Mapping[str, str]],
     },
 )
+SemanticTypeOutputTypeDef = TypedDict(
+    "SemanticTypeOutputTypeDef",
+    {
+        "TypeName": NotRequired[str],
+        "SubTypeName": NotRequired[str],
+        "TypeParameters": NotRequired[Dict[str, str]],
+        "TruthyCellValue": NotRequired[str],
+        "TruthyCellValueSynonyms": NotRequired[List[str]],
+        "FalseyCellValue": NotRequired[str],
+        "FalseyCellValueSynonyms": NotRequired[List[str]],
+    },
+)
 SemanticTypeTypeDef = TypedDict(
     "SemanticTypeTypeDef",
     {
         "TypeName": NotRequired[str],
         "SubTypeName": NotRequired[str],
         "TypeParameters": NotRequired[Mapping[str, str]],
         "TruthyCellValue": NotRequired[str],
@@ -4243,29 +4931,43 @@
 )
 SnapshotAnonymousUserRedactedTypeDef = TypedDict(
     "SnapshotAnonymousUserRedactedTypeDef",
     {
         "RowLevelPermissionTagKeys": NotRequired[List[str]],
     },
 )
+SnapshotFileSheetSelectionOutputTypeDef = TypedDict(
+    "SnapshotFileSheetSelectionOutputTypeDef",
+    {
+        "SheetId": str,
+        "SelectionScope": SnapshotFileSheetSelectionScopeType,
+        "VisualIds": NotRequired[List[str]],
+    },
+)
 SnapshotFileSheetSelectionTypeDef = TypedDict(
     "SnapshotFileSheetSelectionTypeDef",
     {
         "SheetId": str,
         "SelectionScope": SnapshotFileSheetSelectionScopeType,
-        "VisualIds": NotRequired[List[str]],
+        "VisualIds": NotRequired[Sequence[str]],
     },
 )
 SnapshotJobResultErrorInfoTypeDef = TypedDict(
     "SnapshotJobResultErrorInfoTypeDef",
     {
         "ErrorMessage": NotRequired[str],
         "ErrorType": NotRequired[str],
     },
 )
+StringDatasetParameterDefaultValuesOutputTypeDef = TypedDict(
+    "StringDatasetParameterDefaultValuesOutputTypeDef",
+    {
+        "StaticValues": NotRequired[List[str]],
+    },
+)
 StringDatasetParameterDefaultValuesTypeDef = TypedDict(
     "StringDatasetParameterDefaultValuesTypeDef",
     {
         "StaticValues": NotRequired[Sequence[str]],
     },
 )
 StringValueWhenUnsetConfigurationTypeDef = TypedDict(
@@ -4296,14 +4998,20 @@
 )
 TableFieldCustomIconContentTypeDef = TypedDict(
     "TableFieldCustomIconContentTypeDef",
     {
         "Icon": NotRequired[Literal["LINK"]],
     },
 )
+TablePinnedFieldOptionsOutputTypeDef = TypedDict(
+    "TablePinnedFieldOptionsOutputTypeDef",
+    {
+        "PinnedLeftFields": NotRequired[List[str]],
+    },
+)
 TablePinnedFieldOptionsTypeDef = TypedDict(
     "TablePinnedFieldOptionsTypeDef",
     {
         "PinnedLeftFields": NotRequired[Sequence[str]],
     },
 )
 TemplateSourceTemplateTypeDef = TypedDict(
@@ -4355,14 +5063,21 @@
 )
 TotalAggregationFunctionTypeDef = TypedDict(
     "TotalAggregationFunctionTypeDef",
     {
         "SimpleTotalAggregationFunction": NotRequired[SimpleTotalAggregationFunctionType],
     },
 )
+UntagColumnOperationOutputTypeDef = TypedDict(
+    "UntagColumnOperationOutputTypeDef",
+    {
+        "ColumnName": str,
+        "TagNames": List[ColumnTagNameType],
+    },
+)
 UntagColumnOperationTypeDef = TypedDict(
     "UntagColumnOperationTypeDef",
     {
         "ColumnName": str,
         "TagNames": Sequence[ColumnTagNameType],
     },
 )
@@ -4456,14 +5171,21 @@
     {
         "CustomPermissionsName": str,
         "Role": RoleType,
         "AwsAccountId": str,
         "Namespace": str,
     },
 )
+UpdateSPICECapacityConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateSPICECapacityConfigurationRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "PurchaseMode": PurchaseModeType,
+    },
+)
 UpdateTemplateAliasRequestRequestTypeDef = TypedDict(
     "UpdateTemplateAliasRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TemplateId": str,
         "AliasName": str,
         "TemplateVersionNumber": int,
@@ -4548,21 +5270,35 @@
 CascadingControlSourceTypeDef = TypedDict(
     "CascadingControlSourceTypeDef",
     {
         "SourceSheetControlId": NotRequired[str],
         "ColumnToMatch": NotRequired[ColumnIdentifierTypeDef],
     },
 )
+CategoryDrillDownFilterOutputTypeDef = TypedDict(
+    "CategoryDrillDownFilterOutputTypeDef",
+    {
+        "Column": ColumnIdentifierTypeDef,
+        "CategoryValues": List[str],
+    },
+)
 CategoryDrillDownFilterTypeDef = TypedDict(
     "CategoryDrillDownFilterTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "CategoryValues": Sequence[str],
     },
 )
+ContributionAnalysisDefaultOutputTypeDef = TypedDict(
+    "ContributionAnalysisDefaultOutputTypeDef",
+    {
+        "MeasureFieldId": str,
+        "ContributorDimensions": List[ColumnIdentifierTypeDef],
+    },
+)
 ContributionAnalysisDefaultTypeDef = TypedDict(
     "ContributionAnalysisDefaultTypeDef",
     {
         "MeasureFieldId": str,
         "ContributorDimensions": Sequence[ColumnIdentifierTypeDef],
     },
 )
@@ -4570,14 +5306,22 @@
     "DynamicDefaultValueTypeDef",
     {
         "DefaultValueColumn": ColumnIdentifierTypeDef,
         "UserNameColumn": NotRequired[ColumnIdentifierTypeDef],
         "GroupNameColumn": NotRequired[ColumnIdentifierTypeDef],
     },
 )
+FilterOperationSelectedFieldsConfigurationOutputTypeDef = TypedDict(
+    "FilterOperationSelectedFieldsConfigurationOutputTypeDef",
+    {
+        "SelectedFields": NotRequired[List[str]],
+        "SelectedFieldOptions": NotRequired[Literal["ALL_FIELDS"]],
+        "SelectedColumns": NotRequired[List[ColumnIdentifierTypeDef]],
+    },
+)
 FilterOperationSelectedFieldsConfigurationTypeDef = TypedDict(
     "FilterOperationSelectedFieldsConfigurationTypeDef",
     {
         "SelectedFields": NotRequired[Sequence[str]],
         "SelectedFieldOptions": NotRequired[Literal["ALL_FIELDS"]],
         "SelectedColumns": NotRequired[Sequence[ColumnIdentifierTypeDef]],
     },
@@ -4585,21 +5329,37 @@
 NumericEqualityDrillDownFilterTypeDef = TypedDict(
     "NumericEqualityDrillDownFilterTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "Value": float,
     },
 )
+ParameterSelectableValuesOutputTypeDef = TypedDict(
+    "ParameterSelectableValuesOutputTypeDef",
+    {
+        "Values": NotRequired[List[str]],
+        "LinkToDataSetColumn": NotRequired[ColumnIdentifierTypeDef],
+    },
+)
 ParameterSelectableValuesTypeDef = TypedDict(
     "ParameterSelectableValuesTypeDef",
     {
         "Values": NotRequired[Sequence[str]],
         "LinkToDataSetColumn": NotRequired[ColumnIdentifierTypeDef],
     },
 )
+TimeRangeDrillDownFilterOutputTypeDef = TypedDict(
+    "TimeRangeDrillDownFilterOutputTypeDef",
+    {
+        "Column": ColumnIdentifierTypeDef,
+        "RangeMinimum": datetime,
+        "RangeMaximum": datetime,
+        "TimeGranularity": TimeGranularityType,
+    },
+)
 AnalysisErrorTypeDef = TypedDict(
     "AnalysisErrorTypeDef",
     {
         "Type": NotRequired[AnalysisErrorTypeType],
         "Message": NotRequired[str],
         "ViolatedEntities": NotRequired[List[EntityTypeDef]],
     },
@@ -4665,107 +5425,208 @@
 ArcAxisConfigurationTypeDef = TypedDict(
     "ArcAxisConfigurationTypeDef",
     {
         "Range": NotRequired[ArcAxisDisplayRangeTypeDef],
         "ReserveRange": NotRequired[int],
     },
 )
+AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef = TypedDict(
+    "AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef",
+    {
+        "ResourceIdOverrideConfiguration": NotRequired[
+            AssetBundleExportJobResourceIdOverrideConfigurationTypeDef
+        ],
+        "VPCConnections": NotRequired[
+            List[AssetBundleExportJobVPCConnectionOverridePropertiesOutputTypeDef]
+        ],
+        "RefreshSchedules": NotRequired[
+            List[AssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef]
+        ],
+        "DataSources": NotRequired[
+            List[AssetBundleExportJobDataSourceOverridePropertiesOutputTypeDef]
+        ],
+        "DataSets": NotRequired[List[AssetBundleExportJobDataSetOverridePropertiesOutputTypeDef]],
+        "Themes": NotRequired[List[AssetBundleExportJobThemeOverridePropertiesOutputTypeDef]],
+        "Analyses": NotRequired[List[AssetBundleExportJobAnalysisOverridePropertiesOutputTypeDef]],
+        "Dashboards": NotRequired[
+            List[AssetBundleExportJobDashboardOverridePropertiesOutputTypeDef]
+        ],
+    },
+)
 AssetBundleCloudFormationOverridePropertyConfigurationTypeDef = TypedDict(
     "AssetBundleCloudFormationOverridePropertyConfigurationTypeDef",
     {
         "ResourceIdOverrideConfiguration": NotRequired[
             AssetBundleExportJobResourceIdOverrideConfigurationTypeDef
         ],
         "VPCConnections": NotRequired[
-            List[AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef]
+            Sequence[AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef]
         ],
         "RefreshSchedules": NotRequired[
-            List[AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef]
+            Sequence[AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef]
+        ],
+        "DataSources": NotRequired[
+            Sequence[AssetBundleExportJobDataSourceOverridePropertiesTypeDef]
         ],
-        "DataSources": NotRequired[List[AssetBundleExportJobDataSourceOverridePropertiesTypeDef]],
-        "DataSets": NotRequired[List[AssetBundleExportJobDataSetOverridePropertiesTypeDef]],
-        "Themes": NotRequired[List[AssetBundleExportJobThemeOverridePropertiesTypeDef]],
-        "Analyses": NotRequired[List[AssetBundleExportJobAnalysisOverridePropertiesTypeDef]],
-        "Dashboards": NotRequired[List[AssetBundleExportJobDashboardOverridePropertiesTypeDef]],
+        "DataSets": NotRequired[Sequence[AssetBundleExportJobDataSetOverridePropertiesTypeDef]],
+        "Themes": NotRequired[Sequence[AssetBundleExportJobThemeOverridePropertiesTypeDef]],
+        "Analyses": NotRequired[Sequence[AssetBundleExportJobAnalysisOverridePropertiesTypeDef]],
+        "Dashboards": NotRequired[Sequence[AssetBundleExportJobDashboardOverridePropertiesTypeDef]],
+    },
+)
+AssetBundleImportJobAnalysisOverridePermissionsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobAnalysisOverridePermissionsOutputTypeDef",
+    {
+        "AnalysisIds": List[str],
+        "Permissions": AssetBundleResourcePermissionsOutputTypeDef,
+    },
+)
+AssetBundleImportJobDataSetOverridePermissionsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobDataSetOverridePermissionsOutputTypeDef",
+    {
+        "DataSetIds": List[str],
+        "Permissions": AssetBundleResourcePermissionsOutputTypeDef,
+    },
+)
+AssetBundleImportJobDataSourceOverridePermissionsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobDataSourceOverridePermissionsOutputTypeDef",
+    {
+        "DataSourceIds": List[str],
+        "Permissions": AssetBundleResourcePermissionsOutputTypeDef,
+    },
+)
+AssetBundleImportJobThemeOverridePermissionsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobThemeOverridePermissionsOutputTypeDef",
+    {
+        "ThemeIds": List[str],
+        "Permissions": AssetBundleResourcePermissionsOutputTypeDef,
+    },
+)
+AssetBundleResourceLinkSharingConfigurationOutputTypeDef = TypedDict(
+    "AssetBundleResourceLinkSharingConfigurationOutputTypeDef",
+    {
+        "Permissions": NotRequired[AssetBundleResourcePermissionsOutputTypeDef],
     },
 )
 AssetBundleImportJobAnalysisOverridePermissionsTypeDef = TypedDict(
     "AssetBundleImportJobAnalysisOverridePermissionsTypeDef",
     {
-        "AnalysisIds": List[str],
+        "AnalysisIds": Sequence[str],
         "Permissions": AssetBundleResourcePermissionsTypeDef,
     },
 )
 AssetBundleImportJobDataSetOverridePermissionsTypeDef = TypedDict(
     "AssetBundleImportJobDataSetOverridePermissionsTypeDef",
     {
-        "DataSetIds": List[str],
+        "DataSetIds": Sequence[str],
         "Permissions": AssetBundleResourcePermissionsTypeDef,
     },
 )
 AssetBundleImportJobDataSourceOverridePermissionsTypeDef = TypedDict(
     "AssetBundleImportJobDataSourceOverridePermissionsTypeDef",
     {
-        "DataSourceIds": List[str],
+        "DataSourceIds": Sequence[str],
         "Permissions": AssetBundleResourcePermissionsTypeDef,
     },
 )
 AssetBundleImportJobThemeOverridePermissionsTypeDef = TypedDict(
     "AssetBundleImportJobThemeOverridePermissionsTypeDef",
     {
-        "ThemeIds": List[str],
+        "ThemeIds": Sequence[str],
         "Permissions": AssetBundleResourcePermissionsTypeDef,
     },
 )
 AssetBundleResourceLinkSharingConfigurationTypeDef = TypedDict(
     "AssetBundleResourceLinkSharingConfigurationTypeDef",
     {
         "Permissions": NotRequired[AssetBundleResourcePermissionsTypeDef],
     },
 )
+AssetBundleImportJobAnalysisOverrideTagsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobAnalysisOverrideTagsOutputTypeDef",
+    {
+        "AnalysisIds": List[str],
+        "Tags": List[TagTypeDef],
+    },
+)
 AssetBundleImportJobAnalysisOverrideTagsTypeDef = TypedDict(
     "AssetBundleImportJobAnalysisOverrideTagsTypeDef",
     {
-        "AnalysisIds": List[str],
+        "AnalysisIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+AssetBundleImportJobDashboardOverrideTagsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobDashboardOverrideTagsOutputTypeDef",
+    {
+        "DashboardIds": List[str],
         "Tags": List[TagTypeDef],
     },
 )
 AssetBundleImportJobDashboardOverrideTagsTypeDef = TypedDict(
     "AssetBundleImportJobDashboardOverrideTagsTypeDef",
     {
-        "DashboardIds": List[str],
+        "DashboardIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+AssetBundleImportJobDataSetOverrideTagsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobDataSetOverrideTagsOutputTypeDef",
+    {
+        "DataSetIds": List[str],
         "Tags": List[TagTypeDef],
     },
 )
 AssetBundleImportJobDataSetOverrideTagsTypeDef = TypedDict(
     "AssetBundleImportJobDataSetOverrideTagsTypeDef",
     {
-        "DataSetIds": List[str],
+        "DataSetIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+AssetBundleImportJobDataSourceOverrideTagsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobDataSourceOverrideTagsOutputTypeDef",
+    {
+        "DataSourceIds": List[str],
         "Tags": List[TagTypeDef],
     },
 )
 AssetBundleImportJobDataSourceOverrideTagsTypeDef = TypedDict(
     "AssetBundleImportJobDataSourceOverrideTagsTypeDef",
     {
-        "DataSourceIds": List[str],
+        "DataSourceIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+AssetBundleImportJobThemeOverrideTagsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobThemeOverrideTagsOutputTypeDef",
+    {
+        "ThemeIds": List[str],
         "Tags": List[TagTypeDef],
     },
 )
 AssetBundleImportJobThemeOverrideTagsTypeDef = TypedDict(
     "AssetBundleImportJobThemeOverrideTagsTypeDef",
     {
-        "ThemeIds": List[str],
+        "ThemeIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+AssetBundleImportJobVPCConnectionOverrideTagsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobVPCConnectionOverrideTagsOutputTypeDef",
+    {
+        "VPCConnectionIds": List[str],
         "Tags": List[TagTypeDef],
     },
 )
 AssetBundleImportJobVPCConnectionOverrideTagsTypeDef = TypedDict(
     "AssetBundleImportJobVPCConnectionOverrideTagsTypeDef",
     {
-        "VPCConnectionIds": List[str],
-        "Tags": List[TagTypeDef],
+        "VPCConnectionIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
     },
 )
 CreateAccountCustomizationRequestRequestTypeDef = TypedDict(
     "CreateAccountCustomizationRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AccountCustomization": AccountCustomizationTypeDef,
@@ -4823,21 +5684,109 @@
 AssetBundleImportJobDataSourceCredentialsTypeDef = TypedDict(
     "AssetBundleImportJobDataSourceCredentialsTypeDef",
     {
         "CredentialPair": NotRequired[AssetBundleImportJobDataSourceCredentialPairTypeDef],
         "SecretArn": NotRequired[str],
     },
 )
+AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef = TypedDict(
+    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
+    {
+        "DataSetId": str,
+        "ScheduleId": str,
+        "StartAfterDateTime": NotRequired[TimestampTypeDef],
+    },
+)
+CustomParameterValuesTypeDef = TypedDict(
+    "CustomParameterValuesTypeDef",
+    {
+        "StringValues": NotRequired[Sequence[str]],
+        "IntegerValues": NotRequired[Sequence[int]],
+        "DecimalValues": NotRequired[Sequence[float]],
+        "DateTimeValues": NotRequired[Sequence[TimestampTypeDef]],
+    },
+)
+DateTimeDatasetParameterDefaultValuesTypeDef = TypedDict(
+    "DateTimeDatasetParameterDefaultValuesTypeDef",
+    {
+        "StaticValues": NotRequired[Sequence[TimestampTypeDef]],
+    },
+)
+DateTimeParameterTypeDef = TypedDict(
+    "DateTimeParameterTypeDef",
+    {
+        "Name": str,
+        "Values": Sequence[TimestampTypeDef],
+    },
+)
+DateTimeValueWhenUnsetConfigurationTypeDef = TypedDict(
+    "DateTimeValueWhenUnsetConfigurationTypeDef",
+    {
+        "ValueWhenUnsetOption": NotRequired[ValueWhenUnsetOptionType],
+        "CustomValue": NotRequired[TimestampTypeDef],
+    },
+)
+NewDefaultValuesTypeDef = TypedDict(
+    "NewDefaultValuesTypeDef",
+    {
+        "StringStaticValues": NotRequired[Sequence[str]],
+        "DecimalStaticValues": NotRequired[Sequence[float]],
+        "DateTimeStaticValues": NotRequired[Sequence[TimestampTypeDef]],
+        "IntegerStaticValues": NotRequired[Sequence[int]],
+    },
+)
+TimeRangeDrillDownFilterTypeDef = TypedDict(
+    "TimeRangeDrillDownFilterTypeDef",
+    {
+        "Column": ColumnIdentifierTypeDef,
+        "RangeMinimum": TimestampTypeDef,
+        "RangeMaximum": TimestampTypeDef,
+        "TimeGranularity": TimeGranularityType,
+    },
+)
+TopicRefreshScheduleTypeDef = TypedDict(
+    "TopicRefreshScheduleTypeDef",
+    {
+        "IsEnabled": bool,
+        "BasedOnSpiceSchedule": bool,
+        "StartingAt": NotRequired[TimestampTypeDef],
+        "Timezone": NotRequired[str],
+        "RepeatAt": NotRequired[str],
+        "TopicScheduleType": NotRequired[TopicScheduleTypeType],
+    },
+)
+WhatIfPointScenarioTypeDef = TypedDict(
+    "WhatIfPointScenarioTypeDef",
+    {
+        "Date": TimestampTypeDef,
+        "Value": float,
+    },
+)
+WhatIfRangeScenarioTypeDef = TypedDict(
+    "WhatIfRangeScenarioTypeDef",
+    {
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "Value": float,
+    },
+)
 AssetBundleImportSourceTypeDef = TypedDict(
     "AssetBundleImportSourceTypeDef",
     {
         "Body": NotRequired[BlobTypeDef],
         "S3Uri": NotRequired[str],
     },
 )
+AxisDisplayRangeOutputTypeDef = TypedDict(
+    "AxisDisplayRangeOutputTypeDef",
+    {
+        "MinMax": NotRequired[AxisDisplayMinMaxRangeTypeDef],
+        "DataDriven": NotRequired[Dict[str, Any]],
+    },
+)
 AxisDisplayRangeTypeDef = TypedDict(
     "AxisDisplayRangeTypeDef",
     {
         "MinMax": NotRequired[AxisDisplayMinMaxRangeTypeDef],
         "DataDriven": NotRequired[Mapping[str, Any]],
     },
 )
@@ -4873,14 +5822,20 @@
     "BoxPlotOptionsTypeDef",
     {
         "StyleOptions": NotRequired[BoxPlotStyleOptionsTypeDef],
         "OutlierVisibility": NotRequired[VisibilityType],
         "AllDataPointsVisibility": NotRequired[VisibilityType],
     },
 )
+CreateColumnsOperationOutputTypeDef = TypedDict(
+    "CreateColumnsOperationOutputTypeDef",
+    {
+        "Columns": List[CalculatedColumnTypeDef],
+    },
+)
 CreateColumnsOperationTypeDef = TypedDict(
     "CreateColumnsOperationTypeDef",
     {
         "Columns": Sequence[CalculatedColumnTypeDef],
     },
 )
 CancelIngestionResponseTypeDef = TypedDict(
@@ -5404,68 +6359,68 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAnalysesResponseTypeDef = TypedDict(
     "ListAnalysesResponseTypeDef",
     {
         "AnalysisSummaryList": List[AnalysisSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListAssetBundleExportJobsResponseTypeDef = TypedDict(
     "ListAssetBundleExportJobsResponseTypeDef",
     {
         "AssetBundleExportJobSummaryList": List[AssetBundleExportJobSummaryTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListAssetBundleImportJobsResponseTypeDef = TypedDict(
     "ListAssetBundleImportJobsResponseTypeDef",
     {
         "AssetBundleImportJobSummaryList": List[AssetBundleImportJobSummaryTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListIAMPolicyAssignmentsForUserResponseTypeDef = TypedDict(
     "ListIAMPolicyAssignmentsForUserResponseTypeDef",
     {
         "ActiveAssignments": List[ActiveIAMPolicyAssignmentTypeDef],
         "RequestId": str,
-        "NextToken": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListIdentityPropagationConfigsResponseTypeDef = TypedDict(
     "ListIdentityPropagationConfigsResponseTypeDef",
     {
         "Services": List[AuthorizedTargetsByServiceTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListRoleMembershipsResponseTypeDef = TypedDict(
     "ListRoleMembershipsResponseTypeDef",
     {
         "MembersList": List[str],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "RequestId": str,
@@ -5491,18 +6446,18 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchAnalysesResponseTypeDef = TypedDict(
     "SearchAnalysesResponseTypeDef",
     {
         "AnalysisSummaryList": List[AnalysisSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 StartAssetBundleExportJobResponseTypeDef = TypedDict(
     "StartAssetBundleExportJobResponseTypeDef",
     {
         "Arn": str,
         "AssetBundleExportJobId": str,
@@ -5715,14 +6670,22 @@
     "UpdateRoleCustomPermissionResponseTypeDef",
     {
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateSPICECapacityConfigurationResponseTypeDef = TypedDict(
+    "UpdateSPICECapacityConfigurationResponseTypeDef",
+    {
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 UpdateTemplateResponseTypeDef = TypedDict(
     "UpdateTemplateResponseTypeDef",
     {
         "TemplateId": str,
         "Arn": str,
         "VersionArn": str,
         "CreationStatus": ResourceStatusType,
@@ -5773,70 +6736,122 @@
         "UpdateStatus": VPCConnectionResourceStatusType,
         "AvailabilityStatus": VPCConnectionAvailabilityStatusType,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CategoryFilterConfigurationOutputTypeDef = TypedDict(
+    "CategoryFilterConfigurationOutputTypeDef",
+    {
+        "FilterListConfiguration": NotRequired[FilterListConfigurationOutputTypeDef],
+        "CustomFilterListConfiguration": NotRequired[CustomFilterListConfigurationOutputTypeDef],
+        "CustomFilterConfiguration": NotRequired[CustomFilterConfigurationTypeDef],
+    },
+)
 CategoryFilterConfigurationTypeDef = TypedDict(
     "CategoryFilterConfigurationTypeDef",
     {
         "FilterListConfiguration": NotRequired[FilterListConfigurationTypeDef],
         "CustomFilterListConfiguration": NotRequired[CustomFilterListConfigurationTypeDef],
         "CustomFilterConfiguration": NotRequired[CustomFilterConfigurationTypeDef],
     },
 )
 ClusterMarkerTypeDef = TypedDict(
     "ClusterMarkerTypeDef",
     {
         "SimpleClusterMarker": NotRequired[SimpleClusterMarkerTypeDef],
     },
 )
+TopicCategoryFilterConstantOutputTypeDef = TypedDict(
+    "TopicCategoryFilterConstantOutputTypeDef",
+    {
+        "ConstantType": NotRequired[ConstantTypeType],
+        "SingularConstant": NotRequired[str],
+        "CollectiveConstant": NotRequired[CollectiveConstantOutputTypeDef],
+    },
+)
 TopicCategoryFilterConstantTypeDef = TypedDict(
     "TopicCategoryFilterConstantTypeDef",
     {
         "ConstantType": NotRequired[ConstantTypeType],
         "SingularConstant": NotRequired[str],
         "CollectiveConstant": NotRequired[CollectiveConstantTypeDef],
     },
 )
+ColorScaleOutputTypeDef = TypedDict(
+    "ColorScaleOutputTypeDef",
+    {
+        "Colors": List[DataColorTypeDef],
+        "ColorFillType": ColorFillTypeType,
+        "NullValueColor": NotRequired[DataColorTypeDef],
+    },
+)
 ColorScaleTypeDef = TypedDict(
     "ColorScaleTypeDef",
     {
         "Colors": Sequence[DataColorTypeDef],
         "ColorFillType": ColorFillTypeType,
         "NullValueColor": NotRequired[DataColorTypeDef],
     },
 )
+ColorsConfigurationOutputTypeDef = TypedDict(
+    "ColorsConfigurationOutputTypeDef",
+    {
+        "CustomColors": NotRequired[List[CustomColorTypeDef]],
+    },
+)
 ColorsConfigurationTypeDef = TypedDict(
     "ColorsConfigurationTypeDef",
     {
         "CustomColors": NotRequired[Sequence[CustomColorTypeDef]],
     },
 )
 ColumnTagTypeDef = TypedDict(
     "ColumnTagTypeDef",
     {
         "ColumnGeographicRole": NotRequired[GeoSpatialDataRoleType],
         "ColumnDescription": NotRequired[ColumnDescriptionTypeDef],
     },
 )
+ColumnGroupSchemaOutputTypeDef = TypedDict(
+    "ColumnGroupSchemaOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "ColumnGroupColumnSchemaList": NotRequired[List[ColumnGroupColumnSchemaTypeDef]],
+    },
+)
 ColumnGroupSchemaTypeDef = TypedDict(
     "ColumnGroupSchemaTypeDef",
     {
         "Name": NotRequired[str],
         "ColumnGroupColumnSchemaList": NotRequired[Sequence[ColumnGroupColumnSchemaTypeDef]],
     },
 )
+ColumnGroupOutputTypeDef = TypedDict(
+    "ColumnGroupOutputTypeDef",
+    {
+        "GeoSpatialColumnGroup": NotRequired[GeoSpatialColumnGroupOutputTypeDef],
+    },
+)
 ColumnGroupTypeDef = TypedDict(
     "ColumnGroupTypeDef",
     {
         "GeoSpatialColumnGroup": NotRequired[GeoSpatialColumnGroupTypeDef],
     },
 )
+ColumnLevelPermissionRuleUnionTypeDef = Union[
+    ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef
+]
+DataSetSchemaOutputTypeDef = TypedDict(
+    "DataSetSchemaOutputTypeDef",
+    {
+        "ColumnSchemaList": NotRequired[List[ColumnSchemaTypeDef]],
+    },
+)
 DataSetSchemaTypeDef = TypedDict(
     "DataSetSchemaTypeDef",
     {
         "ColumnSchemaList": NotRequired[Sequence[ColumnSchemaTypeDef]],
     },
 )
 ConditionalFormattingCustomIconConditionTypeDef = TypedDict(
@@ -5853,252 +6868,14 @@
     {
         "SignupResponse": SignupResponseTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateFolderRequestRequestTypeDef = TypedDict(
-    "CreateFolderRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "FolderId": str,
-        "Name": NotRequired[str],
-        "FolderType": NotRequired[FolderTypeType],
-        "ParentFolderArn": NotRequired[str],
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "SharingModel": NotRequired[SharingModelType],
-    },
-)
-DescribeAnalysisPermissionsResponseTypeDef = TypedDict(
-    "DescribeAnalysisPermissionsResponseTypeDef",
-    {
-        "AnalysisId": str,
-        "AnalysisArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeDataSetPermissionsResponseTypeDef = TypedDict(
-    "DescribeDataSetPermissionsResponseTypeDef",
-    {
-        "DataSetArn": str,
-        "DataSetId": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeDataSourcePermissionsResponseTypeDef = TypedDict(
-    "DescribeDataSourcePermissionsResponseTypeDef",
-    {
-        "DataSourceArn": str,
-        "DataSourceId": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeFolderPermissionsResponseTypeDef = TypedDict(
-    "DescribeFolderPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "FolderId": str,
-        "Arn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeFolderResolvedPermissionsResponseTypeDef = TypedDict(
-    "DescribeFolderResolvedPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "FolderId": str,
-        "Arn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeTemplatePermissionsResponseTypeDef = TypedDict(
-    "DescribeTemplatePermissionsResponseTypeDef",
-    {
-        "TemplateId": str,
-        "TemplateArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeThemePermissionsResponseTypeDef = TypedDict(
-    "DescribeThemePermissionsResponseTypeDef",
-    {
-        "ThemeId": str,
-        "ThemeArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeTopicPermissionsResponseTypeDef = TypedDict(
-    "DescribeTopicPermissionsResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-LinkSharingConfigurationTypeDef = TypedDict(
-    "LinkSharingConfigurationTypeDef",
-    {
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateAnalysisPermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateAnalysisPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "AnalysisId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateAnalysisPermissionsResponseTypeDef = TypedDict(
-    "UpdateAnalysisPermissionsResponseTypeDef",
-    {
-        "AnalysisArn": str,
-        "AnalysisId": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateDashboardPermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateDashboardPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DashboardId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "GrantLinkPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokeLinkPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateDataSetPermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateDataSetPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DataSetId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateDataSourcePermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateDataSourcePermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DataSourceId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateFolderPermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateFolderPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "FolderId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateFolderPermissionsResponseTypeDef = TypedDict(
-    "UpdateFolderPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "Arn": str,
-        "FolderId": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateTemplatePermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateTemplatePermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "TemplateId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateTemplatePermissionsResponseTypeDef = TypedDict(
-    "UpdateTemplatePermissionsResponseTypeDef",
-    {
-        "TemplateId": str,
-        "TemplateArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateThemePermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateThemePermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "ThemeId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateThemePermissionsResponseTypeDef = TypedDict(
-    "UpdateThemePermissionsResponseTypeDef",
-    {
-        "ThemeId": str,
-        "ThemeArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateTopicPermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateTopicPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "TopicId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateTopicPermissionsResponseTypeDef = TypedDict(
-    "UpdateTopicPermissionsResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DataSetSummaryTypeDef = TypedDict(
     "DataSetSummaryTypeDef",
     {
         "Arn": NotRequired[str],
         "DataSetId": NotRequired[str],
         "Name": NotRequired[str],
         "CreatedTime": NotRequired[datetime],
@@ -6136,18 +6913,18 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListGroupMembershipsResponseTypeDef = TypedDict(
     "ListGroupMembershipsResponseTypeDef",
     {
         "GroupMemberList": List[GroupMemberTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
         "RequestId": str,
@@ -6164,38 +6941,38 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "GroupList": List[GroupTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListUserGroupsResponseTypeDef = TypedDict(
     "ListUserGroupsResponseTypeDef",
     {
         "GroupList": List[GroupTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SearchGroupsResponseTypeDef = TypedDict(
     "SearchGroupsResponseTypeDef",
     {
         "GroupList": List[GroupTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateGroupResponseTypeDef = TypedDict(
     "UpdateGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
         "RequestId": str,
@@ -6223,16 +7000,16 @@
 )
 ListTemplateAliasesResponseTypeDef = TypedDict(
     "ListTemplateAliasesResponseTypeDef",
     {
         "TemplateAliasList": List[TemplateAliasTypeDef],
         "Status": int,
         "RequestId": str,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateTemplateAliasResponseTypeDef = TypedDict(
     "UpdateTemplateAliasResponseTypeDef",
     {
         "TemplateAlias": TemplateAliasTypeDef,
         "Status": int,
@@ -6260,16 +7037,16 @@
 )
 ListThemeAliasesResponseTypeDef = TypedDict(
     "ListThemeAliasesResponseTypeDef",
     {
         "ThemeAliasList": List[ThemeAliasTypeDef],
         "Status": int,
         "RequestId": str,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateThemeAliasResponseTypeDef = TypedDict(
     "UpdateThemeAliasResponseTypeDef",
     {
         "ThemeAlias": ThemeAliasTypeDef,
         "Status": int,
@@ -6279,96 +7056,49 @@
 )
 CustomActionNavigationOperationTypeDef = TypedDict(
     "CustomActionNavigationOperationTypeDef",
     {
         "LocalNavigationConfiguration": NotRequired[LocalNavigationConfigurationTypeDef],
     },
 )
-CustomParameterValuesTypeDef = TypedDict(
-    "CustomParameterValuesTypeDef",
+CustomValuesConfigurationOutputTypeDef = TypedDict(
+    "CustomValuesConfigurationOutputTypeDef",
     {
-        "StringValues": NotRequired[Sequence[str]],
-        "IntegerValues": NotRequired[Sequence[int]],
-        "DecimalValues": NotRequired[Sequence[float]],
-        "DateTimeValues": NotRequired[Sequence[TimestampTypeDef]],
+        "CustomValues": CustomParameterValuesOutputTypeDef,
+        "IncludeNullValue": NotRequired[bool],
     },
 )
-DateTimeDatasetParameterDefaultValuesTypeDef = TypedDict(
-    "DateTimeDatasetParameterDefaultValuesTypeDef",
-    {
-        "StaticValues": NotRequired[Sequence[TimestampTypeDef]],
-    },
-)
-DateTimeParameterTypeDef = TypedDict(
-    "DateTimeParameterTypeDef",
+CustomSqlOutputTypeDef = TypedDict(
+    "CustomSqlOutputTypeDef",
     {
+        "DataSourceArn": str,
         "Name": str,
-        "Values": Sequence[TimestampTypeDef],
-    },
-)
-DateTimeValueWhenUnsetConfigurationTypeDef = TypedDict(
-    "DateTimeValueWhenUnsetConfigurationTypeDef",
-    {
-        "ValueWhenUnsetOption": NotRequired[ValueWhenUnsetOptionType],
-        "CustomValue": NotRequired[TimestampTypeDef],
-    },
-)
-NewDefaultValuesTypeDef = TypedDict(
-    "NewDefaultValuesTypeDef",
-    {
-        "StringStaticValues": NotRequired[Sequence[str]],
-        "DecimalStaticValues": NotRequired[Sequence[float]],
-        "DateTimeStaticValues": NotRequired[Sequence[TimestampTypeDef]],
-        "IntegerStaticValues": NotRequired[Sequence[int]],
-    },
-)
-TimeRangeDrillDownFilterTypeDef = TypedDict(
-    "TimeRangeDrillDownFilterTypeDef",
-    {
-        "Column": ColumnIdentifierTypeDef,
-        "RangeMinimum": TimestampTypeDef,
-        "RangeMaximum": TimestampTypeDef,
-        "TimeGranularity": TimeGranularityType,
-    },
-)
-TopicRefreshScheduleTypeDef = TypedDict(
-    "TopicRefreshScheduleTypeDef",
-    {
-        "IsEnabled": bool,
-        "BasedOnSpiceSchedule": bool,
-        "StartingAt": NotRequired[TimestampTypeDef],
-        "Timezone": NotRequired[str],
-        "RepeatAt": NotRequired[str],
-        "TopicScheduleType": NotRequired[TopicScheduleTypeType],
-    },
-)
-WhatIfPointScenarioTypeDef = TypedDict(
-    "WhatIfPointScenarioTypeDef",
-    {
-        "Date": TimestampTypeDef,
-        "Value": float,
-    },
-)
-WhatIfRangeScenarioTypeDef = TypedDict(
-    "WhatIfRangeScenarioTypeDef",
-    {
-        "StartDate": TimestampTypeDef,
-        "EndDate": TimestampTypeDef,
-        "Value": float,
+        "SqlQuery": str,
+        "Columns": NotRequired[List[InputColumnTypeDef]],
     },
 )
 CustomSqlTypeDef = TypedDict(
     "CustomSqlTypeDef",
     {
         "DataSourceArn": str,
         "Name": str,
         "SqlQuery": str,
         "Columns": NotRequired[Sequence[InputColumnTypeDef]],
     },
 )
+RelationalTableOutputTypeDef = TypedDict(
+    "RelationalTableOutputTypeDef",
+    {
+        "DataSourceArn": str,
+        "Name": str,
+        "InputColumns": List[InputColumnTypeDef],
+        "Catalog": NotRequired[str],
+        "Schema": NotRequired[str],
+    },
+)
 RelationalTableTypeDef = TypedDict(
     "RelationalTableTypeDef",
     {
         "DataSourceArn": str,
         "Name": str,
         "InputColumns": Sequence[InputColumnTypeDef],
         "Catalog": NotRequired[str],
@@ -6391,38 +7121,38 @@
         "MaxResults": NotRequired[int],
     },
 )
 ListDashboardsResponseTypeDef = TypedDict(
     "ListDashboardsResponseTypeDef",
     {
         "DashboardSummaryList": List[DashboardSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SearchDashboardsResponseTypeDef = TypedDict(
     "SearchDashboardsResponseTypeDef",
     {
         "DashboardSummaryList": List[DashboardSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListDashboardVersionsResponseTypeDef = TypedDict(
     "ListDashboardVersionsResponseTypeDef",
     {
         "DashboardVersionSummaryList": List[DashboardVersionSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DashboardVisualPublishOptionsTypeDef = TypedDict(
     "DashboardVisualPublishOptionsTypeDef",
     {
         "ExportHiddenFieldsOption": NotRequired[ExportHiddenFieldsOptionTypeDef],
     },
@@ -6469,37 +7199,203 @@
         "MaxResults": NotRequired[int],
     },
 )
 SearchDataSourcesResponseTypeDef = TypedDict(
     "SearchDataSourcesResponseTypeDef",
     {
         "DataSourceSummaries": List[DataSourceSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+DateTimeDatasetParameterOutputTypeDef = TypedDict(
+    "DateTimeDatasetParameterOutputTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "ValueType": DatasetParameterValueTypeType,
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "DefaultValues": NotRequired[DateTimeDatasetParameterDefaultValuesOutputTypeDef],
+    },
+)
+TimeRangeFilterValueOutputTypeDef = TypedDict(
+    "TimeRangeFilterValueOutputTypeDef",
+    {
+        "StaticValue": NotRequired[datetime],
+        "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
+        "Parameter": NotRequired[str],
     },
 )
 TimeRangeFilterValueTypeDef = TypedDict(
     "TimeRangeFilterValueTypeDef",
     {
         "StaticValue": NotRequired[TimestampTypeDef],
         "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
         "Parameter": NotRequired[str],
     },
 )
+DecimalDatasetParameterOutputTypeDef = TypedDict(
+    "DecimalDatasetParameterOutputTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "ValueType": DatasetParameterValueTypeType,
+        "DefaultValues": NotRequired[DecimalDatasetParameterDefaultValuesOutputTypeDef],
+    },
+)
 DecimalDatasetParameterTypeDef = TypedDict(
     "DecimalDatasetParameterTypeDef",
     {
         "Id": str,
         "Name": str,
         "ValueType": DatasetParameterValueTypeType,
         "DefaultValues": NotRequired[DecimalDatasetParameterDefaultValuesTypeDef],
     },
 )
+DescribeAnalysisPermissionsResponseTypeDef = TypedDict(
+    "DescribeAnalysisPermissionsResponseTypeDef",
+    {
+        "AnalysisId": str,
+        "AnalysisArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeDataSetPermissionsResponseTypeDef = TypedDict(
+    "DescribeDataSetPermissionsResponseTypeDef",
+    {
+        "DataSetArn": str,
+        "DataSetId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeDataSourcePermissionsResponseTypeDef = TypedDict(
+    "DescribeDataSourcePermissionsResponseTypeDef",
+    {
+        "DataSourceArn": str,
+        "DataSourceId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeFolderResolvedPermissionsResponseTypeDef = TypedDict(
+    "DescribeFolderResolvedPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "FolderId": str,
+        "Arn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+DescribeTemplatePermissionsResponseTypeDef = TypedDict(
+    "DescribeTemplatePermissionsResponseTypeDef",
+    {
+        "TemplateId": str,
+        "TemplateArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeThemePermissionsResponseTypeDef = TypedDict(
+    "DescribeThemePermissionsResponseTypeDef",
+    {
+        "ThemeId": str,
+        "ThemeArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeTopicPermissionsResponseTypeDef = TypedDict(
+    "DescribeTopicPermissionsResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+LinkSharingConfigurationOutputTypeDef = TypedDict(
+    "LinkSharingConfigurationOutputTypeDef",
+    {
+        "Permissions": NotRequired[List[ResourcePermissionOutputTypeDef]],
+    },
+)
+UpdateAnalysisPermissionsResponseTypeDef = TypedDict(
+    "UpdateAnalysisPermissionsResponseTypeDef",
+    {
+        "AnalysisArn": str,
+        "AnalysisId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateFolderPermissionsResponseTypeDef = TypedDict(
+    "UpdateFolderPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "Arn": str,
+        "FolderId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateTemplatePermissionsResponseTypeDef = TypedDict(
+    "UpdateTemplatePermissionsResponseTypeDef",
+    {
+        "TemplateId": str,
+        "TemplateArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateThemePermissionsResponseTypeDef = TypedDict(
+    "UpdateThemePermissionsResponseTypeDef",
+    {
+        "ThemeId": str,
+        "ThemeArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateTopicPermissionsResponseTypeDef = TypedDict(
+    "UpdateTopicPermissionsResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DescribeFolderPermissionsRequestDescribeFolderPermissionsPaginateTypeDef = TypedDict(
     "DescribeFolderPermissionsRequestDescribeFolderPermissionsPaginateTypeDef",
     {
         "AwsAccountId": str,
         "FolderId": str,
         "Namespace": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -6724,36 +7620,24 @@
     "SearchDataSourcesRequestSearchDataSourcesPaginateTypeDef",
     {
         "AwsAccountId": str,
         "Filters": Sequence[DataSourceSearchFilterTypeDef],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-DescribeFolderPermissionsResponsePaginatorTypeDef = TypedDict(
-    "DescribeFolderPermissionsResponsePaginatorTypeDef",
-    {
-        "Status": int,
-        "FolderId": str,
-        "Arn": str,
-        "Permissions": List[ResourcePermissionPaginatorTypeDef],
-        "RequestId": str,
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeFolderResolvedPermissionsResponsePaginatorTypeDef = TypedDict(
-    "DescribeFolderResolvedPermissionsResponsePaginatorTypeDef",
+DescribeFolderPermissionsResponseTypeDef = TypedDict(
+    "DescribeFolderPermissionsResponseTypeDef",
     {
         "Status": int,
         "FolderId": str,
         "Arn": str,
-        "Permissions": List[ResourcePermissionPaginatorTypeDef],
+        "Permissions": List[ResourcePermissionExtraOutputTypeDef],
         "RequestId": str,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeFolderResponseTypeDef = TypedDict(
     "DescribeFolderResponseTypeDef",
     {
         "Status": int,
         "Folder": FolderTypeDef,
@@ -6775,31 +7659,52 @@
     {
         "RefreshDetails": TopicRefreshDetailsTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeTopicRefreshScheduleResponseTypeDef = TypedDict(
+    "DescribeTopicRefreshScheduleResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "DatasetArn": str,
+        "RefreshSchedule": TopicRefreshScheduleOutputTypeDef,
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+TopicRefreshScheduleSummaryTypeDef = TypedDict(
+    "TopicRefreshScheduleSummaryTypeDef",
+    {
+        "DatasetId": NotRequired[str],
+        "DatasetArn": NotRequired[str],
+        "DatasetName": NotRequired[str],
+        "RefreshSchedule": NotRequired[TopicRefreshScheduleOutputTypeDef],
+    },
+)
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "User": UserTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "UserList": List[UserTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RegisterUserResponseTypeDef = TypedDict(
     "RegisterUserResponseTypeDef",
     {
         "User": UserTypeDef,
         "UserInvitationUrl": str,
@@ -6837,14 +7742,23 @@
 DonutOptionsTypeDef = TypedDict(
     "DonutOptionsTypeDef",
     {
         "ArcOptions": NotRequired[ArcOptionsTypeDef],
         "DonutCenterOptions": NotRequired[DonutCenterOptionsTypeDef],
     },
 )
+FieldFolderUnionTypeDef = Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]
+FilterOperationTargetVisualsConfigurationOutputTypeDef = TypedDict(
+    "FilterOperationTargetVisualsConfigurationOutputTypeDef",
+    {
+        "SameSheetTargetVisualConfiguration": NotRequired[
+            SameSheetTargetVisualConfigurationOutputTypeDef
+        ],
+    },
+)
 FilterOperationTargetVisualsConfigurationTypeDef = TypedDict(
     "FilterOperationTargetVisualsConfigurationTypeDef",
     {
         "SameSheetTargetVisualConfiguration": NotRequired[
             SameSheetTargetVisualConfigurationTypeDef
         ],
     },
@@ -6867,45 +7781,58 @@
     },
 )
 ListFoldersResponseTypeDef = TypedDict(
     "ListFoldersResponseTypeDef",
     {
         "Status": int,
         "FolderSummaryList": List[FolderSummaryTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SearchFoldersResponseTypeDef = TypedDict(
     "SearchFoldersResponseTypeDef",
     {
         "Status": int,
         "FolderSummaryList": List[FolderSummaryTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 FontConfigurationTypeDef = TypedDict(
     "FontConfigurationTypeDef",
     {
         "FontSize": NotRequired[FontSizeTypeDef],
         "FontDecoration": NotRequired[FontDecorationType],
         "FontColor": NotRequired[str],
         "FontWeight": NotRequired[FontWeightTypeDef],
         "FontStyle": NotRequired[FontStyleType],
     },
 )
+TypographyOutputTypeDef = TypedDict(
+    "TypographyOutputTypeDef",
+    {
+        "FontFamilies": NotRequired[List[FontTypeDef]],
+    },
+)
 TypographyTypeDef = TypedDict(
     "TypographyTypeDef",
     {
         "FontFamilies": NotRequired[Sequence[FontTypeDef]],
     },
 )
+ForecastScenarioOutputTypeDef = TypedDict(
+    "ForecastScenarioOutputTypeDef",
+    {
+        "WhatIfPointScenario": NotRequired[WhatIfPointScenarioOutputTypeDef],
+        "WhatIfRangeScenario": NotRequired[WhatIfRangeScenarioOutputTypeDef],
+    },
+)
 FreeFormLayoutCanvasSizeOptionsTypeDef = TypedDict(
     "FreeFormLayoutCanvasSizeOptionsTypeDef",
     {
         "ScreenCanvasSizeOptions": NotRequired[FreeFormLayoutScreenCanvasSizeOptionsTypeDef],
     },
 )
 SnapshotAnonymousUserTypeDef = TypedDict(
@@ -6917,14 +7844,20 @@
 GeospatialWindowOptionsTypeDef = TypedDict(
     "GeospatialWindowOptionsTypeDef",
     {
         "Bounds": NotRequired[GeospatialCoordinateBoundsTypeDef],
         "MapZoomMode": NotRequired[MapZoomModeType],
     },
 )
+GeospatialHeatmapColorScaleOutputTypeDef = TypedDict(
+    "GeospatialHeatmapColorScaleOutputTypeDef",
+    {
+        "Colors": NotRequired[List[GeospatialHeatmapDataColorTypeDef]],
+    },
+)
 GeospatialHeatmapColorScaleTypeDef = TypedDict(
     "GeospatialHeatmapColorScaleTypeDef",
     {
         "Colors": NotRequired[Sequence[GeospatialHeatmapDataColorTypeDef]],
     },
 )
 TableSideBorderOptionsTypeDef = TypedDict(
@@ -6934,14 +7867,20 @@
         "InnerHorizontal": NotRequired[TableBorderOptionsTypeDef],
         "Left": NotRequired[TableBorderOptionsTypeDef],
         "Right": NotRequired[TableBorderOptionsTypeDef],
         "Top": NotRequired[TableBorderOptionsTypeDef],
         "Bottom": NotRequired[TableBorderOptionsTypeDef],
     },
 )
+GradientColorOutputTypeDef = TypedDict(
+    "GradientColorOutputTypeDef",
+    {
+        "Stops": NotRequired[List[GradientStopTypeDef]],
+    },
+)
 GradientColorTypeDef = TypedDict(
     "GradientColorTypeDef",
     {
         "Stops": NotRequired[Sequence[GradientStopTypeDef]],
     },
 )
 GridLayoutCanvasSizeOptionsTypeDef = TypedDict(
@@ -6969,18 +7908,18 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListIAMPolicyAssignmentsResponseTypeDef = TypedDict(
     "ListIAMPolicyAssignmentsResponseTypeDef",
     {
         "IAMPolicyAssignments": List[IAMPolicyAssignmentSummaryTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 IncrementalRefreshTypeDef = TypedDict(
     "IncrementalRefreshTypeDef",
     {
         "LookbackWindow": LookbackWindowTypeDef,
     },
@@ -6997,14 +7936,23 @@
         "QueueInfo": NotRequired[QueueInfoTypeDef],
         "IngestionTimeInSeconds": NotRequired[int],
         "IngestionSizeInBytes": NotRequired[int],
         "RequestSource": NotRequired[IngestionRequestSourceType],
         "RequestType": NotRequired[IngestionRequestTypeType],
     },
 )
+IntegerDatasetParameterOutputTypeDef = TypedDict(
+    "IntegerDatasetParameterOutputTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "ValueType": DatasetParameterValueTypeType,
+        "DefaultValues": NotRequired[IntegerDatasetParameterDefaultValuesOutputTypeDef],
+    },
+)
 IntegerDatasetParameterTypeDef = TypedDict(
     "IntegerDatasetParameterTypeDef",
     {
         "Id": str,
         "Name": str,
         "ValueType": DatasetParameterValueTypeType,
         "DefaultValues": NotRequired[IntegerDatasetParameterDefaultValuesTypeDef],
@@ -7038,72 +7986,81 @@
 LineChartSeriesSettingsTypeDef = TypedDict(
     "LineChartSeriesSettingsTypeDef",
     {
         "LineStyleSettings": NotRequired[LineChartLineStyleSettingsTypeDef],
         "MarkerStyleSettings": NotRequired[LineChartMarkerStyleSettingsTypeDef],
     },
 )
+LinkSharingConfigurationTypeDef = TypedDict(
+    "LinkSharingConfigurationTypeDef",
+    {
+        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
+    },
+)
+ResourcePermissionUnionTypeDef = Union[
+    ResourcePermissionTypeDef, ResourcePermissionExtraOutputTypeDef
+]
 ListFolderMembersResponseTypeDef = TypedDict(
     "ListFolderMembersResponseTypeDef",
     {
         "Status": int,
         "FolderMemberList": List[MemberIdArnPairTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTemplateVersionsResponseTypeDef = TypedDict(
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionSummaryList": List[TemplateVersionSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplateSummaryList": List[TemplateSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListThemeVersionsResponseTypeDef = TypedDict(
     "ListThemeVersionsResponseTypeDef",
     {
         "ThemeVersionSummaryList": List[ThemeVersionSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListThemesResponseTypeDef = TypedDict(
     "ListThemesResponseTypeDef",
     {
         "ThemeSummaryList": List[ThemeSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTopicsResponseTypeDef = TypedDict(
     "ListTopicsResponseTypeDef",
     {
         "TopicsSummaries": List[TopicSummaryTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 VisualSubtitleLabelOptionsTypeDef = TypedDict(
     "VisualSubtitleLabelOptionsTypeDef",
     {
         "Visibility": NotRequired[VisibilityType],
         "FormatText": NotRequired[LongFormatTextTypeDef],
@@ -7119,14 +8076,24 @@
 TileLayoutStyleTypeDef = TypedDict(
     "TileLayoutStyleTypeDef",
     {
         "Gutter": NotRequired[GutterStyleTypeDef],
         "Margin": NotRequired[MarginStyleTypeDef],
     },
 )
+NamedEntityDefinitionOutputTypeDef = TypedDict(
+    "NamedEntityDefinitionOutputTypeDef",
+    {
+        "FieldName": NotRequired[str],
+        "PropertyName": NotRequired[str],
+        "PropertyRole": NotRequired[PropertyRoleType],
+        "PropertyUsage": NotRequired[PropertyUsageType],
+        "Metric": NotRequired[NamedEntityDefinitionMetricOutputTypeDef],
+    },
+)
 NamedEntityDefinitionTypeDef = TypedDict(
     "NamedEntityDefinitionTypeDef",
     {
         "FieldName": NotRequired[str],
         "PropertyName": NotRequired[str],
         "PropertyRole": NotRequired[PropertyRoleType],
         "PropertyUsage": NotRequired[PropertyUsageType],
@@ -7174,28 +8141,45 @@
         "AvailabilityStatus": NotRequired[VPCConnectionAvailabilityStatusType],
         "NetworkInterfaces": NotRequired[List[NetworkInterfaceTypeDef]],
         "RoleArn": NotRequired[str],
         "CreatedTime": NotRequired[datetime],
         "LastUpdatedTime": NotRequired[datetime],
     },
 )
+OverrideDatasetParameterOperationOutputTypeDef = TypedDict(
+    "OverrideDatasetParameterOperationOutputTypeDef",
+    {
+        "ParameterName": str,
+        "NewParameterName": NotRequired[str],
+        "NewDefaultValues": NotRequired[NewDefaultValuesOutputTypeDef],
+    },
+)
 NumericSeparatorConfigurationTypeDef = TypedDict(
     "NumericSeparatorConfigurationTypeDef",
     {
         "DecimalSeparator": NotRequired[NumericSeparatorSymbolType],
         "ThousandsSeparator": NotRequired[ThousandSeparatorOptionsTypeDef],
     },
 )
 NumericalAggregationFunctionTypeDef = TypedDict(
     "NumericalAggregationFunctionTypeDef",
     {
         "SimpleNumericalAggregation": NotRequired[SimpleNumericalAggregationFunctionType],
         "PercentileAggregation": NotRequired[PercentileAggregationTypeDef],
     },
 )
+ParametersOutputTypeDef = TypedDict(
+    "ParametersOutputTypeDef",
+    {
+        "StringParameters": NotRequired[List[StringParameterOutputTypeDef]],
+        "IntegerParameters": NotRequired[List[IntegerParameterOutputTypeDef]],
+        "DecimalParameters": NotRequired[List[DecimalParameterOutputTypeDef]],
+        "DateTimeParameters": NotRequired[List[DateTimeParameterOutputTypeDef]],
+    },
+)
 VisibleRangeOptionsTypeDef = TypedDict(
     "VisibleRangeOptionsTypeDef",
     {
         "PercentRange": NotRequired[PercentVisibleRangeTypeDef],
     },
 )
 RadarChartSeriesSettingsTypeDef = TypedDict(
@@ -7207,22 +8191,33 @@
 TopicRangeFilterConstantTypeDef = TypedDict(
     "TopicRangeFilterConstantTypeDef",
     {
         "ConstantType": NotRequired[ConstantTypeType],
         "RangeConstant": NotRequired[RangeConstantTypeDef],
     },
 )
-RedshiftParametersPaginatorTypeDef = TypedDict(
-    "RedshiftParametersPaginatorTypeDef",
+RedshiftParametersExtraOutputTypeDef = TypedDict(
+    "RedshiftParametersExtraOutputTypeDef",
+    {
+        "Database": str,
+        "Host": NotRequired[str],
+        "Port": NotRequired[int],
+        "ClusterId": NotRequired[str],
+        "IAMParameters": NotRequired[RedshiftIAMParametersExtraOutputTypeDef],
+        "IdentityCenterConfiguration": NotRequired[IdentityCenterConfigurationTypeDef],
+    },
+)
+RedshiftParametersOutputTypeDef = TypedDict(
+    "RedshiftParametersOutputTypeDef",
     {
         "Database": str,
         "Host": NotRequired[str],
         "Port": NotRequired[int],
         "ClusterId": NotRequired[str],
-        "IAMParameters": NotRequired[RedshiftIAMParametersPaginatorTypeDef],
+        "IAMParameters": NotRequired[RedshiftIAMParametersOutputTypeDef],
         "IdentityCenterConfiguration": NotRequired[IdentityCenterConfigurationTypeDef],
     },
 )
 RedshiftParametersTypeDef = TypedDict(
     "RedshiftParametersTypeDef",
     {
         "Database": str,
@@ -7251,28 +8246,44 @@
 RegisteredUserDashboardFeatureConfigurationsTypeDef = TypedDict(
     "RegisteredUserDashboardFeatureConfigurationsTypeDef",
     {
         "StatePersistence": NotRequired[StatePersistenceConfigurationsTypeDef],
         "Bookmarks": NotRequired[BookmarksConfigurationsTypeDef],
     },
 )
+RowLevelPermissionTagConfigurationOutputTypeDef = TypedDict(
+    "RowLevelPermissionTagConfigurationOutputTypeDef",
+    {
+        "TagRules": List[RowLevelPermissionTagRuleTypeDef],
+        "Status": NotRequired[StatusType],
+        "TagRuleConfigurations": NotRequired[List[List[str]]],
+    },
+)
 RowLevelPermissionTagConfigurationTypeDef = TypedDict(
     "RowLevelPermissionTagConfigurationTypeDef",
     {
         "TagRules": Sequence[RowLevelPermissionTagRuleTypeDef],
         "Status": NotRequired[StatusType],
         "TagRuleConfigurations": NotRequired[Sequence[Sequence[str]]],
     },
 )
 SnapshotS3DestinationConfigurationTypeDef = TypedDict(
     "SnapshotS3DestinationConfigurationTypeDef",
     {
         "BucketConfiguration": S3BucketConfigurationTypeDef,
     },
 )
+S3SourceOutputTypeDef = TypedDict(
+    "S3SourceOutputTypeDef",
+    {
+        "DataSourceArn": str,
+        "InputColumns": List[InputColumnTypeDef],
+        "UploadSettings": NotRequired[UploadSettingsTypeDef],
+    },
+)
 S3SourceTypeDef = TypedDict(
     "S3SourceTypeDef",
     {
         "DataSourceArn": str,
         "InputColumns": Sequence[InputColumnTypeDef],
         "UploadSettings": NotRequired[UploadSettingsTypeDef],
     },
@@ -7294,14 +8305,22 @@
 SectionStyleTypeDef = TypedDict(
     "SectionStyleTypeDef",
     {
         "Height": NotRequired[str],
         "Padding": NotRequired[SpacingTypeDef],
     },
 )
+SelectedSheetsFilterScopeConfigurationOutputTypeDef = TypedDict(
+    "SelectedSheetsFilterScopeConfigurationOutputTypeDef",
+    {
+        "SheetVisualScopingConfigurations": NotRequired[
+            List[SheetVisualScopingConfigurationOutputTypeDef]
+        ],
+    },
+)
 SelectedSheetsFilterScopeConfigurationTypeDef = TypedDict(
     "SelectedSheetsFilterScopeConfigurationTypeDef",
     {
         "SheetVisualScopingConfigurations": NotRequired[
             Sequence[SheetVisualScopingConfigurationTypeDef]
         ],
     },
@@ -7328,21 +8347,37 @@
 )
 SnapshotUserConfigurationRedactedTypeDef = TypedDict(
     "SnapshotUserConfigurationRedactedTypeDef",
     {
         "AnonymousUsers": NotRequired[List[SnapshotAnonymousUserRedactedTypeDef]],
     },
 )
+SnapshotFileOutputTypeDef = TypedDict(
+    "SnapshotFileOutputTypeDef",
+    {
+        "SheetSelections": List[SnapshotFileSheetSelectionOutputTypeDef],
+        "FormatType": SnapshotFileFormatTypeType,
+    },
+)
 SnapshotFileTypeDef = TypedDict(
     "SnapshotFileTypeDef",
     {
-        "SheetSelections": List[SnapshotFileSheetSelectionTypeDef],
+        "SheetSelections": Sequence[SnapshotFileSheetSelectionTypeDef],
         "FormatType": SnapshotFileFormatTypeType,
     },
 )
+StringDatasetParameterOutputTypeDef = TypedDict(
+    "StringDatasetParameterOutputTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "ValueType": DatasetParameterValueTypeType,
+        "DefaultValues": NotRequired[StringDatasetParameterDefaultValuesOutputTypeDef],
+    },
+)
 StringDatasetParameterTypeDef = TypedDict(
     "StringDatasetParameterTypeDef",
     {
         "Id": str,
         "Name": str,
         "ValueType": DatasetParameterValueTypeType,
         "DefaultValues": NotRequired[StringDatasetParameterDefaultValuesTypeDef],
@@ -7378,49 +8413,92 @@
 )
 WaterfallChartColorConfigurationTypeDef = TypedDict(
     "WaterfallChartColorConfigurationTypeDef",
     {
         "GroupColorConfiguration": NotRequired[WaterfallChartGroupColorConfigurationTypeDef],
     },
 )
+CascadingControlConfigurationOutputTypeDef = TypedDict(
+    "CascadingControlConfigurationOutputTypeDef",
+    {
+        "SourceControls": NotRequired[List[CascadingControlSourceTypeDef]],
+    },
+)
 CascadingControlConfigurationTypeDef = TypedDict(
     "CascadingControlConfigurationTypeDef",
     {
         "SourceControls": NotRequired[Sequence[CascadingControlSourceTypeDef]],
     },
 )
+DateTimeDefaultValuesOutputTypeDef = TypedDict(
+    "DateTimeDefaultValuesOutputTypeDef",
+    {
+        "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
+        "StaticValues": NotRequired[List[datetime]],
+        "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
+    },
+)
 DateTimeDefaultValuesTypeDef = TypedDict(
     "DateTimeDefaultValuesTypeDef",
     {
         "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
         "StaticValues": NotRequired[Sequence[TimestampTypeDef]],
         "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
     },
 )
+DecimalDefaultValuesOutputTypeDef = TypedDict(
+    "DecimalDefaultValuesOutputTypeDef",
+    {
+        "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
+        "StaticValues": NotRequired[List[float]],
+    },
+)
 DecimalDefaultValuesTypeDef = TypedDict(
     "DecimalDefaultValuesTypeDef",
     {
         "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
         "StaticValues": NotRequired[Sequence[float]],
     },
 )
+IntegerDefaultValuesOutputTypeDef = TypedDict(
+    "IntegerDefaultValuesOutputTypeDef",
+    {
+        "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
+        "StaticValues": NotRequired[List[int]],
+    },
+)
 IntegerDefaultValuesTypeDef = TypedDict(
     "IntegerDefaultValuesTypeDef",
     {
         "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
         "StaticValues": NotRequired[Sequence[int]],
     },
 )
+StringDefaultValuesOutputTypeDef = TypedDict(
+    "StringDefaultValuesOutputTypeDef",
+    {
+        "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
+        "StaticValues": NotRequired[List[str]],
+    },
+)
 StringDefaultValuesTypeDef = TypedDict(
     "StringDefaultValuesTypeDef",
     {
         "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
         "StaticValues": NotRequired[Sequence[str]],
     },
 )
+DrillDownFilterOutputTypeDef = TypedDict(
+    "DrillDownFilterOutputTypeDef",
+    {
+        "NumericEqualityFilter": NotRequired[NumericEqualityDrillDownFilterTypeDef],
+        "CategoryFilter": NotRequired[CategoryDrillDownFilterOutputTypeDef],
+        "TimeRangeFilter": NotRequired[TimeRangeDrillDownFilterOutputTypeDef],
+    },
+)
 AnalysisTypeDef = TypedDict(
     "AnalysisTypeDef",
     {
         "AnalysisId": NotRequired[str],
         "Arn": NotRequired[str],
         "Name": NotRequired[str],
         "Status": NotRequired[ResourceStatusType],
@@ -7468,14 +8546,15 @@
 )
 AnonymousUserEmbeddingExperienceConfigurationTypeDef = TypedDict(
     "AnonymousUserEmbeddingExperienceConfigurationTypeDef",
     {
         "Dashboard": NotRequired[AnonymousUserDashboardEmbeddingConfigurationTypeDef],
         "DashboardVisual": NotRequired[AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef],
         "QSearchBar": NotRequired[AnonymousUserQSearchBarEmbeddingConfigurationTypeDef],
+        "GenerativeQnA": NotRequired[AnonymousUserGenerativeQnAEmbeddingConfigurationTypeDef],
     },
 )
 DescribeAssetBundleExportJobResponseTypeDef = TypedDict(
     "DescribeAssetBundleExportJobResponseTypeDef",
     {
         "JobStatus": AssetBundleExportJobStatusType,
         "DownloadUrl": str,
@@ -7483,24 +8562,28 @@
         "Arn": str,
         "CreatedTime": datetime,
         "AssetBundleExportJobId": str,
         "AwsAccountId": str,
         "ResourceArns": List[str],
         "IncludeAllDependencies": bool,
         "ExportFormat": AssetBundleExportFormatType,
-        "CloudFormationOverridePropertyConfiguration": AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
+        "CloudFormationOverridePropertyConfiguration": AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
         "RequestId": str,
         "Status": int,
         "IncludePermissions": bool,
         "IncludeTags": bool,
         "ValidationStrategy": AssetBundleExportJobValidationStrategyTypeDef,
         "Warnings": List[AssetBundleExportJobWarningTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef = Union[
+    AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
+    AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
+]
 StartAssetBundleExportJobRequestRequestTypeDef = TypedDict(
     "StartAssetBundleExportJobRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AssetBundleExportJobId": str,
         "ResourceArns": Sequence[str],
         "ExportFormat": AssetBundleExportFormatType,
@@ -7509,119 +8592,56 @@
             AssetBundleCloudFormationOverridePropertyConfigurationTypeDef
         ],
         "IncludePermissions": NotRequired[bool],
         "IncludeTags": NotRequired[bool],
         "ValidationStrategy": NotRequired[AssetBundleExportJobValidationStrategyTypeDef],
     },
 )
-AssetBundleImportJobDashboardOverridePermissionsTypeDef = TypedDict(
-    "AssetBundleImportJobDashboardOverridePermissionsTypeDef",
+AssetBundleImportJobDashboardOverridePermissionsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobDashboardOverridePermissionsOutputTypeDef",
     {
         "DashboardIds": List[str],
-        "Permissions": NotRequired[AssetBundleResourcePermissionsTypeDef],
-        "LinkSharingConfiguration": NotRequired[AssetBundleResourceLinkSharingConfigurationTypeDef],
-    },
-)
-AssetBundleImportJobOverrideTagsTypeDef = TypedDict(
-    "AssetBundleImportJobOverrideTagsTypeDef",
-    {
-        "VPCConnections": NotRequired[List[AssetBundleImportJobVPCConnectionOverrideTagsTypeDef]],
-        "DataSources": NotRequired[List[AssetBundleImportJobDataSourceOverrideTagsTypeDef]],
-        "DataSets": NotRequired[List[AssetBundleImportJobDataSetOverrideTagsTypeDef]],
-        "Themes": NotRequired[List[AssetBundleImportJobThemeOverrideTagsTypeDef]],
-        "Analyses": NotRequired[List[AssetBundleImportJobAnalysisOverrideTagsTypeDef]],
-        "Dashboards": NotRequired[List[AssetBundleImportJobDashboardOverrideTagsTypeDef]],
-    },
-)
-NumericAxisOptionsTypeDef = TypedDict(
-    "NumericAxisOptionsTypeDef",
-    {
-        "Scale": NotRequired[AxisScaleTypeDef],
-        "Range": NotRequired[AxisDisplayRangeTypeDef],
-    },
-)
-ClusterMarkerConfigurationTypeDef = TypedDict(
-    "ClusterMarkerConfigurationTypeDef",
-    {
-        "ClusterMarker": NotRequired[ClusterMarkerTypeDef],
-    },
-)
-TopicCategoryFilterTypeDef = TypedDict(
-    "TopicCategoryFilterTypeDef",
-    {
-        "CategoryFilterFunction": NotRequired[CategoryFilterFunctionType],
-        "CategoryFilterType": NotRequired[CategoryFilterTypeType],
-        "Constant": NotRequired[TopicCategoryFilterConstantTypeDef],
-        "Inverse": NotRequired[bool],
-    },
-)
-TagColumnOperationTypeDef = TypedDict(
-    "TagColumnOperationTypeDef",
-    {
-        "ColumnName": str,
-        "Tags": Sequence[ColumnTagTypeDef],
-    },
-)
-DataSetConfigurationTypeDef = TypedDict(
-    "DataSetConfigurationTypeDef",
-    {
-        "Placeholder": NotRequired[str],
-        "DataSetSchema": NotRequired[DataSetSchemaTypeDef],
-        "ColumnGroupSchemaList": NotRequired[Sequence[ColumnGroupSchemaTypeDef]],
-    },
-)
-ConditionalFormattingIconTypeDef = TypedDict(
-    "ConditionalFormattingIconTypeDef",
-    {
-        "IconSet": NotRequired[ConditionalFormattingIconSetTypeDef],
-        "CustomCondition": NotRequired[ConditionalFormattingCustomIconConditionTypeDef],
-    },
-)
-DescribeDashboardPermissionsResponseTypeDef = TypedDict(
-    "DescribeDashboardPermissionsResponseTypeDef",
-    {
-        "DashboardId": str,
-        "DashboardArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Permissions": NotRequired[AssetBundleResourcePermissionsOutputTypeDef],
+        "LinkSharingConfiguration": NotRequired[
+            AssetBundleResourceLinkSharingConfigurationOutputTypeDef
+        ],
     },
 )
-UpdateDashboardPermissionsResponseTypeDef = TypedDict(
-    "UpdateDashboardPermissionsResponseTypeDef",
+AssetBundleImportJobDashboardOverridePermissionsTypeDef = TypedDict(
+    "AssetBundleImportJobDashboardOverridePermissionsTypeDef",
     {
-        "DashboardArn": str,
-        "DashboardId": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DashboardIds": Sequence[str],
+        "Permissions": NotRequired[AssetBundleResourcePermissionsTypeDef],
+        "LinkSharingConfiguration": NotRequired[AssetBundleResourceLinkSharingConfigurationTypeDef],
     },
 )
-ListDataSetsResponseTypeDef = TypedDict(
-    "ListDataSetsResponseTypeDef",
+AssetBundleImportJobOverrideTagsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobOverrideTagsOutputTypeDef",
     {
-        "DataSetSummaries": List[DataSetSummaryTypeDef],
-        "NextToken": str,
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "VPCConnections": NotRequired[
+            List[AssetBundleImportJobVPCConnectionOverrideTagsOutputTypeDef]
+        ],
+        "DataSources": NotRequired[List[AssetBundleImportJobDataSourceOverrideTagsOutputTypeDef]],
+        "DataSets": NotRequired[List[AssetBundleImportJobDataSetOverrideTagsOutputTypeDef]],
+        "Themes": NotRequired[List[AssetBundleImportJobThemeOverrideTagsOutputTypeDef]],
+        "Analyses": NotRequired[List[AssetBundleImportJobAnalysisOverrideTagsOutputTypeDef]],
+        "Dashboards": NotRequired[List[AssetBundleImportJobDashboardOverrideTagsOutputTypeDef]],
     },
 )
-SearchDataSetsResponseTypeDef = TypedDict(
-    "SearchDataSetsResponseTypeDef",
+AssetBundleImportJobOverrideTagsTypeDef = TypedDict(
+    "AssetBundleImportJobOverrideTagsTypeDef",
     {
-        "DataSetSummaries": List[DataSetSummaryTypeDef],
-        "NextToken": str,
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "VPCConnections": NotRequired[
+            Sequence[AssetBundleImportJobVPCConnectionOverrideTagsTypeDef]
+        ],
+        "DataSources": NotRequired[Sequence[AssetBundleImportJobDataSourceOverrideTagsTypeDef]],
+        "DataSets": NotRequired[Sequence[AssetBundleImportJobDataSetOverrideTagsTypeDef]],
+        "Themes": NotRequired[Sequence[AssetBundleImportJobThemeOverrideTagsTypeDef]],
+        "Analyses": NotRequired[Sequence[AssetBundleImportJobAnalysisOverrideTagsTypeDef]],
+        "Dashboards": NotRequired[Sequence[AssetBundleImportJobDashboardOverrideTagsTypeDef]],
     },
 )
 CustomValuesConfigurationTypeDef = TypedDict(
     "CustomValuesConfigurationTypeDef",
     {
         "CustomValues": CustomParameterValuesTypeDef,
         "IncludeNullValue": NotRequired[bool],
@@ -7668,35 +8688,17 @@
         "AwsAccountId": str,
         "TopicId": str,
         "DatasetArn": str,
         "RefreshSchedule": TopicRefreshScheduleTypeDef,
         "DatasetName": NotRequired[str],
     },
 )
-DescribeTopicRefreshScheduleResponseTypeDef = TypedDict(
-    "DescribeTopicRefreshScheduleResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "DatasetArn": str,
-        "RefreshSchedule": TopicRefreshScheduleTypeDef,
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-TopicRefreshScheduleSummaryTypeDef = TypedDict(
-    "TopicRefreshScheduleSummaryTypeDef",
-    {
-        "DatasetId": NotRequired[str],
-        "DatasetArn": NotRequired[str],
-        "DatasetName": NotRequired[str],
-        "RefreshSchedule": NotRequired[TopicRefreshScheduleTypeDef],
-    },
-)
+TopicRefreshScheduleUnionTypeDef = Union[
+    TopicRefreshScheduleTypeDef, TopicRefreshScheduleOutputTypeDef
+]
 UpdateTopicRefreshScheduleRequestRequestTypeDef = TypedDict(
     "UpdateTopicRefreshScheduleRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TopicId": str,
         "DatasetId": str,
         "RefreshSchedule": TopicRefreshScheduleTypeDef,
@@ -7705,14 +8707,120 @@
 ForecastScenarioTypeDef = TypedDict(
     "ForecastScenarioTypeDef",
     {
         "WhatIfPointScenario": NotRequired[WhatIfPointScenarioTypeDef],
         "WhatIfRangeScenario": NotRequired[WhatIfRangeScenarioTypeDef],
     },
 )
+NumericAxisOptionsOutputTypeDef = TypedDict(
+    "NumericAxisOptionsOutputTypeDef",
+    {
+        "Scale": NotRequired[AxisScaleTypeDef],
+        "Range": NotRequired[AxisDisplayRangeOutputTypeDef],
+    },
+)
+NumericAxisOptionsTypeDef = TypedDict(
+    "NumericAxisOptionsTypeDef",
+    {
+        "Scale": NotRequired[AxisScaleTypeDef],
+        "Range": NotRequired[AxisDisplayRangeTypeDef],
+    },
+)
+ClusterMarkerConfigurationTypeDef = TypedDict(
+    "ClusterMarkerConfigurationTypeDef",
+    {
+        "ClusterMarker": NotRequired[ClusterMarkerTypeDef],
+    },
+)
+TopicCategoryFilterOutputTypeDef = TypedDict(
+    "TopicCategoryFilterOutputTypeDef",
+    {
+        "CategoryFilterFunction": NotRequired[CategoryFilterFunctionType],
+        "CategoryFilterType": NotRequired[CategoryFilterTypeType],
+        "Constant": NotRequired[TopicCategoryFilterConstantOutputTypeDef],
+        "Inverse": NotRequired[bool],
+    },
+)
+TopicCategoryFilterTypeDef = TypedDict(
+    "TopicCategoryFilterTypeDef",
+    {
+        "CategoryFilterFunction": NotRequired[CategoryFilterFunctionType],
+        "CategoryFilterType": NotRequired[CategoryFilterTypeType],
+        "Constant": NotRequired[TopicCategoryFilterConstantTypeDef],
+        "Inverse": NotRequired[bool],
+    },
+)
+TagColumnOperationOutputTypeDef = TypedDict(
+    "TagColumnOperationOutputTypeDef",
+    {
+        "ColumnName": str,
+        "Tags": List[ColumnTagTypeDef],
+    },
+)
+TagColumnOperationTypeDef = TypedDict(
+    "TagColumnOperationTypeDef",
+    {
+        "ColumnName": str,
+        "Tags": Sequence[ColumnTagTypeDef],
+    },
+)
+ColumnGroupUnionTypeDef = Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]
+DataSetConfigurationOutputTypeDef = TypedDict(
+    "DataSetConfigurationOutputTypeDef",
+    {
+        "Placeholder": NotRequired[str],
+        "DataSetSchema": NotRequired[DataSetSchemaOutputTypeDef],
+        "ColumnGroupSchemaList": NotRequired[List[ColumnGroupSchemaOutputTypeDef]],
+    },
+)
+DataSetConfigurationTypeDef = TypedDict(
+    "DataSetConfigurationTypeDef",
+    {
+        "Placeholder": NotRequired[str],
+        "DataSetSchema": NotRequired[DataSetSchemaTypeDef],
+        "ColumnGroupSchemaList": NotRequired[Sequence[ColumnGroupSchemaTypeDef]],
+    },
+)
+ConditionalFormattingIconTypeDef = TypedDict(
+    "ConditionalFormattingIconTypeDef",
+    {
+        "IconSet": NotRequired[ConditionalFormattingIconSetTypeDef],
+        "CustomCondition": NotRequired[ConditionalFormattingCustomIconConditionTypeDef],
+    },
+)
+ListDataSetsResponseTypeDef = TypedDict(
+    "ListDataSetsResponseTypeDef",
+    {
+        "DataSetSummaries": List[DataSetSummaryTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+SearchDataSetsResponseTypeDef = TypedDict(
+    "SearchDataSetsResponseTypeDef",
+    {
+        "DataSetSummaries": List[DataSetSummaryTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+DestinationParameterValueConfigurationOutputTypeDef = TypedDict(
+    "DestinationParameterValueConfigurationOutputTypeDef",
+    {
+        "CustomValuesConfiguration": NotRequired[CustomValuesConfigurationOutputTypeDef],
+        "SelectAllValueOptions": NotRequired[Literal["ALL_VALUES"]],
+        "SourceParameterName": NotRequired[str],
+        "SourceField": NotRequired[str],
+        "SourceColumn": NotRequired[ColumnIdentifierTypeDef],
+    },
+)
 CustomContentConfigurationTypeDef = TypedDict(
     "CustomContentConfigurationTypeDef",
     {
         "ContentUrl": NotRequired[str],
         "ContentType": NotRequired[CustomContentTypeType],
         "ImageScaling": NotRequired[CustomContentImageScalingConfigurationType],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
@@ -7740,42 +8848,105 @@
     "DataPathColorTypeDef",
     {
         "Element": DataPathValueTypeDef,
         "Color": str,
         "TimeGranularity": NotRequired[TimeGranularityType],
     },
 )
+DataPathSortOutputTypeDef = TypedDict(
+    "DataPathSortOutputTypeDef",
+    {
+        "Direction": SortDirectionType,
+        "SortPaths": List[DataPathValueTypeDef],
+    },
+)
 DataPathSortTypeDef = TypedDict(
     "DataPathSortTypeDef",
     {
         "Direction": SortDirectionType,
         "SortPaths": Sequence[DataPathValueTypeDef],
     },
 )
+PivotTableDataPathOptionOutputTypeDef = TypedDict(
+    "PivotTableDataPathOptionOutputTypeDef",
+    {
+        "DataPathList": List[DataPathValueTypeDef],
+        "Width": NotRequired[str],
+    },
+)
 PivotTableDataPathOptionTypeDef = TypedDict(
     "PivotTableDataPathOptionTypeDef",
     {
         "DataPathList": Sequence[DataPathValueTypeDef],
         "Width": NotRequired[str],
     },
 )
+PivotTableFieldCollapseStateTargetOutputTypeDef = TypedDict(
+    "PivotTableFieldCollapseStateTargetOutputTypeDef",
+    {
+        "FieldId": NotRequired[str],
+        "FieldDataPathValues": NotRequired[List[DataPathValueTypeDef]],
+    },
+)
 PivotTableFieldCollapseStateTargetTypeDef = TypedDict(
     "PivotTableFieldCollapseStateTargetTypeDef",
     {
         "FieldId": NotRequired[str],
         "FieldDataPathValues": NotRequired[Sequence[DataPathValueTypeDef]],
     },
 )
+DescribeDashboardPermissionsResponseTypeDef = TypedDict(
+    "DescribeDashboardPermissionsResponseTypeDef",
+    {
+        "DashboardId": str,
+        "DashboardArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "LinkSharingConfiguration": LinkSharingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateDashboardPermissionsResponseTypeDef = TypedDict(
+    "UpdateDashboardPermissionsResponseTypeDef",
+    {
+        "DashboardArn": str,
+        "DashboardId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "LinkSharingConfiguration": LinkSharingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListTopicRefreshSchedulesResponseTypeDef = TypedDict(
+    "ListTopicRefreshSchedulesResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "RefreshSchedules": List[TopicRefreshScheduleSummaryTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DefaultFormattingTypeDef = TypedDict(
     "DefaultFormattingTypeDef",
     {
         "DisplayFormat": NotRequired[DisplayFormatType],
         "DisplayFormatOptions": NotRequired[DisplayFormatOptionsTypeDef],
     },
 )
+CustomActionFilterOperationOutputTypeDef = TypedDict(
+    "CustomActionFilterOperationOutputTypeDef",
+    {
+        "SelectedFieldsConfiguration": FilterOperationSelectedFieldsConfigurationOutputTypeDef,
+        "TargetVisualsConfiguration": FilterOperationTargetVisualsConfigurationOutputTypeDef,
+    },
+)
 CustomActionFilterOperationTypeDef = TypedDict(
     "CustomActionFilterOperationTypeDef",
     {
         "SelectedFieldsConfiguration": FilterOperationSelectedFieldsConfigurationTypeDef,
         "TargetVisualsConfiguration": FilterOperationTargetVisualsConfigurationTypeDef,
     },
 )
@@ -7783,14 +8954,29 @@
     "AxisLabelOptionsTypeDef",
     {
         "FontConfiguration": NotRequired[FontConfigurationTypeDef],
         "CustomLabel": NotRequired[str],
         "ApplyTo": NotRequired[AxisLabelReferenceOptionsTypeDef],
     },
 )
+DataLabelOptionsOutputTypeDef = TypedDict(
+    "DataLabelOptionsOutputTypeDef",
+    {
+        "Visibility": NotRequired[VisibilityType],
+        "CategoryLabelVisibility": NotRequired[VisibilityType],
+        "MeasureLabelVisibility": NotRequired[VisibilityType],
+        "DataLabelTypes": NotRequired[List[DataLabelTypeTypeDef]],
+        "Position": NotRequired[DataLabelPositionType],
+        "LabelContent": NotRequired[DataLabelContentType],
+        "LabelFontConfiguration": NotRequired[FontConfigurationTypeDef],
+        "LabelColor": NotRequired[str],
+        "Overlap": NotRequired[DataLabelOverlapType],
+        "TotalsVisibility": NotRequired[VisibilityType],
+    },
+)
 DataLabelOptionsTypeDef = TypedDict(
     "DataLabelOptionsTypeDef",
     {
         "Visibility": NotRequired[VisibilityType],
         "CategoryLabelVisibility": NotRequired[VisibilityType],
         "MeasureLabelVisibility": NotRequired[VisibilityType],
         "DataLabelTypes": NotRequired[Sequence[DataLabelTypeTypeDef]],
@@ -7833,52 +9019,79 @@
 TableFieldCustomTextContentTypeDef = TypedDict(
     "TableFieldCustomTextContentTypeDef",
     {
         "FontConfiguration": FontConfigurationTypeDef,
         "Value": NotRequired[str],
     },
 )
+ForecastConfigurationOutputTypeDef = TypedDict(
+    "ForecastConfigurationOutputTypeDef",
+    {
+        "ForecastProperties": NotRequired[TimeBasedForecastPropertiesTypeDef],
+        "Scenario": NotRequired[ForecastScenarioOutputTypeDef],
+    },
+)
 DefaultFreeFormLayoutConfigurationTypeDef = TypedDict(
     "DefaultFreeFormLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": FreeFormLayoutCanvasSizeOptionsTypeDef,
     },
 )
 SnapshotUserConfigurationTypeDef = TypedDict(
     "SnapshotUserConfigurationTypeDef",
     {
         "AnonymousUsers": NotRequired[Sequence[SnapshotAnonymousUserTypeDef]],
     },
 )
+GeospatialHeatmapConfigurationOutputTypeDef = TypedDict(
+    "GeospatialHeatmapConfigurationOutputTypeDef",
+    {
+        "HeatmapColor": NotRequired[GeospatialHeatmapColorScaleOutputTypeDef],
+    },
+)
 GeospatialHeatmapConfigurationTypeDef = TypedDict(
     "GeospatialHeatmapConfigurationTypeDef",
     {
         "HeatmapColor": NotRequired[GeospatialHeatmapColorScaleTypeDef],
     },
 )
 GlobalTableBorderOptionsTypeDef = TypedDict(
     "GlobalTableBorderOptionsTypeDef",
     {
         "UniformBorder": NotRequired[TableBorderOptionsTypeDef],
         "SideSpecificBorder": NotRequired[TableSideBorderOptionsTypeDef],
     },
 )
+ConditionalFormattingGradientColorOutputTypeDef = TypedDict(
+    "ConditionalFormattingGradientColorOutputTypeDef",
+    {
+        "Expression": str,
+        "Color": GradientColorOutputTypeDef,
+    },
+)
 ConditionalFormattingGradientColorTypeDef = TypedDict(
     "ConditionalFormattingGradientColorTypeDef",
     {
         "Expression": str,
         "Color": GradientColorTypeDef,
     },
 )
 DefaultGridLayoutConfigurationTypeDef = TypedDict(
     "DefaultGridLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": GridLayoutCanvasSizeOptionsTypeDef,
     },
 )
+GridLayoutConfigurationOutputTypeDef = TypedDict(
+    "GridLayoutConfigurationOutputTypeDef",
+    {
+        "Elements": List[GridLayoutElementTypeDef],
+        "CanvasSizeOptions": NotRequired[GridLayoutCanvasSizeOptionsTypeDef],
+    },
+)
 GridLayoutConfigurationTypeDef = TypedDict(
     "GridLayoutConfigurationTypeDef",
     {
         "Elements": Sequence[GridLayoutElementTypeDef],
         "CanvasSizeOptions": NotRequired[GridLayoutCanvasSizeOptionsTypeDef],
     },
 )
@@ -7897,18 +9110,18 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListIngestionsResponseTypeDef = TypedDict(
     "ListIngestionsResponseTypeDef",
     {
         "Ingestions": List[IngestionTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 LogicalTableSourceTypeDef = TypedDict(
     "LogicalTableSourceTypeDef",
     {
         "JoinInstruction": NotRequired[JoinInstructionTypeDef],
         "PhysicalTableId": NotRequired[str],
@@ -7928,21 +9141,121 @@
     "FieldSeriesItemTypeDef",
     {
         "FieldId": str,
         "AxisBinding": AxisBindingType,
         "Settings": NotRequired[LineChartSeriesSettingsTypeDef],
     },
 )
+LinkSharingConfigurationUnionTypeDef = Union[
+    LinkSharingConfigurationTypeDef, LinkSharingConfigurationOutputTypeDef
+]
+CreateFolderRequestRequestTypeDef = TypedDict(
+    "CreateFolderRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "FolderId": str,
+        "Name": NotRequired[str],
+        "FolderType": NotRequired[FolderTypeType],
+        "ParentFolderArn": NotRequired[str],
+        "Permissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "SharingModel": NotRequired[SharingModelType],
+    },
+)
+UpdateAnalysisPermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateAnalysisPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "AnalysisId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
+UpdateDashboardPermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateDashboardPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DashboardId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "GrantLinkPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokeLinkPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
+UpdateDataSetPermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateDataSetPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DataSetId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
+UpdateDataSourcePermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateDataSourcePermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DataSourceId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
+UpdateFolderPermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateFolderPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "FolderId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
+UpdateTemplatePermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateTemplatePermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "TemplateId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
+UpdateThemePermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateThemePermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "ThemeId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
+UpdateTopicPermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateTopicPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "TopicId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
 SheetStyleTypeDef = TypedDict(
     "SheetStyleTypeDef",
     {
         "Tile": NotRequired[TileStyleTypeDef],
         "TileLayout": NotRequired[TileLayoutStyleTypeDef],
     },
 )
+TopicNamedEntityOutputTypeDef = TypedDict(
+    "TopicNamedEntityOutputTypeDef",
+    {
+        "EntityName": str,
+        "EntityDescription": NotRequired[str],
+        "EntitySynonyms": NotRequired[List[str]],
+        "SemanticEntityType": NotRequired[SemanticEntityTypeOutputTypeDef],
+        "Definition": NotRequired[List[NamedEntityDefinitionOutputTypeDef]],
+    },
+)
 TopicNamedEntityTypeDef = TypedDict(
     "TopicNamedEntityTypeDef",
     {
         "EntityName": str,
         "EntityDescription": NotRequired[str],
         "EntitySynonyms": NotRequired[Sequence[str]],
         "SemanticEntityType": NotRequired[SemanticEntityTypeTypeDef],
@@ -7958,28 +9271,28 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "Namespaces": List[NamespaceInfoV2TypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListVPCConnectionsResponseTypeDef = TypedDict(
     "ListVPCConnectionsResponseTypeDef",
     {
         "VPCConnectionSummaries": List[VPCConnectionSummaryTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeVPCConnectionResponseTypeDef = TypedDict(
     "DescribeVPCConnectionResponseTypeDef",
     {
         "VPCConnection": VPCConnectionTypeDef,
         "RequestId": str,
@@ -8050,30 +9363,61 @@
     "TopicNumericRangeFilterTypeDef",
     {
         "Inclusive": NotRequired[bool],
         "Constant": NotRequired[TopicRangeFilterConstantTypeDef],
         "Aggregation": NotRequired[NamedFilterAggTypeType],
     },
 )
-DataSourceParametersPaginatorTypeDef = TypedDict(
-    "DataSourceParametersPaginatorTypeDef",
+DataSourceParametersExtraOutputTypeDef = TypedDict(
+    "DataSourceParametersExtraOutputTypeDef",
+    {
+        "AmazonElasticsearchParameters": NotRequired[AmazonElasticsearchParametersTypeDef],
+        "AthenaParameters": NotRequired[AthenaParametersTypeDef],
+        "AuroraParameters": NotRequired[AuroraParametersTypeDef],
+        "AuroraPostgreSqlParameters": NotRequired[AuroraPostgreSqlParametersTypeDef],
+        "AwsIotAnalyticsParameters": NotRequired[AwsIotAnalyticsParametersTypeDef],
+        "JiraParameters": NotRequired[JiraParametersTypeDef],
+        "MariaDbParameters": NotRequired[MariaDbParametersTypeDef],
+        "MySqlParameters": NotRequired[MySqlParametersTypeDef],
+        "OracleParameters": NotRequired[OracleParametersTypeDef],
+        "PostgreSqlParameters": NotRequired[PostgreSqlParametersTypeDef],
+        "PrestoParameters": NotRequired[PrestoParametersTypeDef],
+        "RdsParameters": NotRequired[RdsParametersTypeDef],
+        "RedshiftParameters": NotRequired[RedshiftParametersExtraOutputTypeDef],
+        "S3Parameters": NotRequired[S3ParametersTypeDef],
+        "ServiceNowParameters": NotRequired[ServiceNowParametersTypeDef],
+        "SnowflakeParameters": NotRequired[SnowflakeParametersTypeDef],
+        "SparkParameters": NotRequired[SparkParametersTypeDef],
+        "SqlServerParameters": NotRequired[SqlServerParametersTypeDef],
+        "TeradataParameters": NotRequired[TeradataParametersTypeDef],
+        "TwitterParameters": NotRequired[TwitterParametersTypeDef],
+        "AmazonOpenSearchParameters": NotRequired[AmazonOpenSearchParametersTypeDef],
+        "ExasolParameters": NotRequired[ExasolParametersTypeDef],
+        "DatabricksParameters": NotRequired[DatabricksParametersTypeDef],
+        "StarburstParameters": NotRequired[StarburstParametersTypeDef],
+        "TrinoParameters": NotRequired[TrinoParametersTypeDef],
+        "BigQueryParameters": NotRequired[BigQueryParametersTypeDef],
+    },
+)
+DataSourceParametersOutputTypeDef = TypedDict(
+    "DataSourceParametersOutputTypeDef",
     {
         "AmazonElasticsearchParameters": NotRequired[AmazonElasticsearchParametersTypeDef],
         "AthenaParameters": NotRequired[AthenaParametersTypeDef],
         "AuroraParameters": NotRequired[AuroraParametersTypeDef],
         "AuroraPostgreSqlParameters": NotRequired[AuroraPostgreSqlParametersTypeDef],
         "AwsIotAnalyticsParameters": NotRequired[AwsIotAnalyticsParametersTypeDef],
         "JiraParameters": NotRequired[JiraParametersTypeDef],
         "MariaDbParameters": NotRequired[MariaDbParametersTypeDef],
         "MySqlParameters": NotRequired[MySqlParametersTypeDef],
         "OracleParameters": NotRequired[OracleParametersTypeDef],
         "PostgreSqlParameters": NotRequired[PostgreSqlParametersTypeDef],
         "PrestoParameters": NotRequired[PrestoParametersTypeDef],
         "RdsParameters": NotRequired[RdsParametersTypeDef],
-        "RedshiftParameters": NotRequired[RedshiftParametersPaginatorTypeDef],
+        "RedshiftParameters": NotRequired[RedshiftParametersOutputTypeDef],
         "S3Parameters": NotRequired[S3ParametersTypeDef],
         "ServiceNowParameters": NotRequired[ServiceNowParametersTypeDef],
         "SnowflakeParameters": NotRequired[SnowflakeParametersTypeDef],
         "SparkParameters": NotRequired[SparkParametersTypeDef],
         "SqlServerParameters": NotRequired[SqlServerParametersTypeDef],
         "TeradataParameters": NotRequired[TeradataParametersTypeDef],
         "TwitterParameters": NotRequired[TwitterParametersTypeDef],
@@ -8112,14 +9456,24 @@
         "ExasolParameters": NotRequired[ExasolParametersTypeDef],
         "DatabricksParameters": NotRequired[DatabricksParametersTypeDef],
         "StarburstParameters": NotRequired[StarburstParametersTypeDef],
         "TrinoParameters": NotRequired[TrinoParametersTypeDef],
         "BigQueryParameters": NotRequired[BigQueryParametersTypeDef],
     },
 )
+RefreshScheduleOutputTypeDef = TypedDict(
+    "RefreshScheduleOutputTypeDef",
+    {
+        "ScheduleId": str,
+        "ScheduleFrequency": RefreshFrequencyTypeDef,
+        "RefreshType": IngestionTypeType,
+        "StartAfterDateTime": NotRequired[datetime],
+        "Arn": NotRequired[str],
+    },
+)
 RefreshScheduleTypeDef = TypedDict(
     "RefreshScheduleTypeDef",
     {
         "ScheduleId": str,
         "ScheduleFrequency": RefreshFrequencyTypeDef,
         "RefreshType": IngestionTypeType,
         "StartAfterDateTime": NotRequired[TimestampTypeDef],
@@ -8136,49 +9490,90 @@
 RegisteredUserDashboardEmbeddingConfigurationTypeDef = TypedDict(
     "RegisteredUserDashboardEmbeddingConfigurationTypeDef",
     {
         "InitialDashboardId": str,
         "FeatureConfigurations": NotRequired[RegisteredUserDashboardFeatureConfigurationsTypeDef],
     },
 )
+RowLevelPermissionTagConfigurationUnionTypeDef = Union[
+    RowLevelPermissionTagConfigurationTypeDef, RowLevelPermissionTagConfigurationOutputTypeDef
+]
+SnapshotDestinationConfigurationOutputTypeDef = TypedDict(
+    "SnapshotDestinationConfigurationOutputTypeDef",
+    {
+        "S3Destinations": NotRequired[List[SnapshotS3DestinationConfigurationTypeDef]],
+    },
+)
 SnapshotDestinationConfigurationTypeDef = TypedDict(
     "SnapshotDestinationConfigurationTypeDef",
     {
-        "S3Destinations": NotRequired[List[SnapshotS3DestinationConfigurationTypeDef]],
+        "S3Destinations": NotRequired[Sequence[SnapshotS3DestinationConfigurationTypeDef]],
     },
 )
 SnapshotJobS3ResultTypeDef = TypedDict(
     "SnapshotJobS3ResultTypeDef",
     {
         "S3DestinationConfiguration": NotRequired[SnapshotS3DestinationConfigurationTypeDef],
         "S3Uri": NotRequired[str],
         "ErrorInfo": NotRequired[List[SnapshotJobResultErrorInfoTypeDef]],
     },
 )
+PhysicalTableOutputTypeDef = TypedDict(
+    "PhysicalTableOutputTypeDef",
+    {
+        "RelationalTable": NotRequired[RelationalTableOutputTypeDef],
+        "CustomSql": NotRequired[CustomSqlOutputTypeDef],
+        "S3Source": NotRequired[S3SourceOutputTypeDef],
+    },
+)
 PhysicalTableTypeDef = TypedDict(
     "PhysicalTableTypeDef",
     {
         "RelationalTable": NotRequired[RelationalTableTypeDef],
         "CustomSql": NotRequired[CustomSqlTypeDef],
         "S3Source": NotRequired[S3SourceTypeDef],
     },
 )
 SectionBasedLayoutCanvasSizeOptionsTypeDef = TypedDict(
     "SectionBasedLayoutCanvasSizeOptionsTypeDef",
     {
         "PaperCanvasSizeOptions": NotRequired[SectionBasedLayoutPaperCanvasSizeOptionsTypeDef],
     },
 )
+FilterScopeConfigurationOutputTypeDef = TypedDict(
+    "FilterScopeConfigurationOutputTypeDef",
+    {
+        "SelectedSheets": NotRequired[SelectedSheetsFilterScopeConfigurationOutputTypeDef],
+        "AllSheets": NotRequired[Dict[str, Any]],
+    },
+)
 FilterScopeConfigurationTypeDef = TypedDict(
     "FilterScopeConfigurationTypeDef",
     {
         "SelectedSheets": NotRequired[SelectedSheetsFilterScopeConfigurationTypeDef],
         "AllSheets": NotRequired[Mapping[str, Any]],
     },
 )
+FreeFormLayoutElementOutputTypeDef = TypedDict(
+    "FreeFormLayoutElementOutputTypeDef",
+    {
+        "ElementId": str,
+        "ElementType": LayoutElementTypeType,
+        "XAxisLocation": str,
+        "YAxisLocation": str,
+        "Width": str,
+        "Height": str,
+        "Visibility": NotRequired[VisibilityType],
+        "RenderingRules": NotRequired[List[SheetElementRenderingRuleTypeDef]],
+        "BorderStyle": NotRequired[FreeFormLayoutElementBorderStyleTypeDef],
+        "SelectedBorderStyle": NotRequired[FreeFormLayoutElementBorderStyleTypeDef],
+        "BackgroundStyle": NotRequired[FreeFormLayoutElementBackgroundStyleTypeDef],
+        "LoadingAnimation": NotRequired[LoadingAnimationTypeDef],
+    },
+)
 FreeFormLayoutElementTypeDef = TypedDict(
     "FreeFormLayoutElementTypeDef",
     {
         "ElementId": str,
         "ElementType": LayoutElementTypeType,
         "XAxisLocation": str,
         "YAxisLocation": str,
@@ -8188,68 +9583,154 @@
         "RenderingRules": NotRequired[Sequence[SheetElementRenderingRuleTypeDef]],
         "BorderStyle": NotRequired[FreeFormLayoutElementBorderStyleTypeDef],
         "SelectedBorderStyle": NotRequired[FreeFormLayoutElementBorderStyleTypeDef],
         "BackgroundStyle": NotRequired[FreeFormLayoutElementBackgroundStyleTypeDef],
         "LoadingAnimation": NotRequired[LoadingAnimationTypeDef],
     },
 )
+SnapshotFileGroupOutputTypeDef = TypedDict(
+    "SnapshotFileGroupOutputTypeDef",
+    {
+        "Files": NotRequired[List[SnapshotFileOutputTypeDef]],
+    },
+)
 SnapshotFileGroupTypeDef = TypedDict(
     "SnapshotFileGroupTypeDef",
     {
-        "Files": NotRequired[List[SnapshotFileTypeDef]],
+        "Files": NotRequired[Sequence[SnapshotFileTypeDef]],
+    },
+)
+DatasetParameterOutputTypeDef = TypedDict(
+    "DatasetParameterOutputTypeDef",
+    {
+        "StringDatasetParameter": NotRequired[StringDatasetParameterOutputTypeDef],
+        "DecimalDatasetParameter": NotRequired[DecimalDatasetParameterOutputTypeDef],
+        "IntegerDatasetParameter": NotRequired[IntegerDatasetParameterOutputTypeDef],
+        "DateTimeDatasetParameter": NotRequired[DateTimeDatasetParameterOutputTypeDef],
+    },
+)
+FilterCrossSheetControlOutputTypeDef = TypedDict(
+    "FilterCrossSheetControlOutputTypeDef",
+    {
+        "FilterControlId": str,
+        "SourceFilterId": str,
+        "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationOutputTypeDef],
     },
 )
 FilterCrossSheetControlTypeDef = TypedDict(
     "FilterCrossSheetControlTypeDef",
     {
         "FilterControlId": str,
         "SourceFilterId": str,
         "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationTypeDef],
     },
 )
+DateTimeParameterDeclarationOutputTypeDef = TypedDict(
+    "DateTimeParameterDeclarationOutputTypeDef",
+    {
+        "Name": str,
+        "DefaultValues": NotRequired[DateTimeDefaultValuesOutputTypeDef],
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "ValueWhenUnset": NotRequired[DateTimeValueWhenUnsetConfigurationOutputTypeDef],
+        "MappedDataSetParameters": NotRequired[List[MappedDataSetParameterTypeDef]],
+    },
+)
 DateTimeParameterDeclarationTypeDef = TypedDict(
     "DateTimeParameterDeclarationTypeDef",
     {
         "Name": str,
         "DefaultValues": NotRequired[DateTimeDefaultValuesTypeDef],
         "TimeGranularity": NotRequired[TimeGranularityType],
         "ValueWhenUnset": NotRequired[DateTimeValueWhenUnsetConfigurationTypeDef],
         "MappedDataSetParameters": NotRequired[Sequence[MappedDataSetParameterTypeDef]],
     },
 )
+DecimalParameterDeclarationOutputTypeDef = TypedDict(
+    "DecimalParameterDeclarationOutputTypeDef",
+    {
+        "ParameterValueType": ParameterValueTypeType,
+        "Name": str,
+        "DefaultValues": NotRequired[DecimalDefaultValuesOutputTypeDef],
+        "ValueWhenUnset": NotRequired[DecimalValueWhenUnsetConfigurationTypeDef],
+        "MappedDataSetParameters": NotRequired[List[MappedDataSetParameterTypeDef]],
+    },
+)
 DecimalParameterDeclarationTypeDef = TypedDict(
     "DecimalParameterDeclarationTypeDef",
     {
         "ParameterValueType": ParameterValueTypeType,
         "Name": str,
         "DefaultValues": NotRequired[DecimalDefaultValuesTypeDef],
         "ValueWhenUnset": NotRequired[DecimalValueWhenUnsetConfigurationTypeDef],
         "MappedDataSetParameters": NotRequired[Sequence[MappedDataSetParameterTypeDef]],
     },
 )
+IntegerParameterDeclarationOutputTypeDef = TypedDict(
+    "IntegerParameterDeclarationOutputTypeDef",
+    {
+        "ParameterValueType": ParameterValueTypeType,
+        "Name": str,
+        "DefaultValues": NotRequired[IntegerDefaultValuesOutputTypeDef],
+        "ValueWhenUnset": NotRequired[IntegerValueWhenUnsetConfigurationTypeDef],
+        "MappedDataSetParameters": NotRequired[List[MappedDataSetParameterTypeDef]],
+    },
+)
 IntegerParameterDeclarationTypeDef = TypedDict(
     "IntegerParameterDeclarationTypeDef",
     {
         "ParameterValueType": ParameterValueTypeType,
         "Name": str,
         "DefaultValues": NotRequired[IntegerDefaultValuesTypeDef],
         "ValueWhenUnset": NotRequired[IntegerValueWhenUnsetConfigurationTypeDef],
         "MappedDataSetParameters": NotRequired[Sequence[MappedDataSetParameterTypeDef]],
     },
 )
+StringParameterDeclarationOutputTypeDef = TypedDict(
+    "StringParameterDeclarationOutputTypeDef",
+    {
+        "ParameterValueType": ParameterValueTypeType,
+        "Name": str,
+        "DefaultValues": NotRequired[StringDefaultValuesOutputTypeDef],
+        "ValueWhenUnset": NotRequired[StringValueWhenUnsetConfigurationTypeDef],
+        "MappedDataSetParameters": NotRequired[List[MappedDataSetParameterTypeDef]],
+    },
+)
 StringParameterDeclarationTypeDef = TypedDict(
     "StringParameterDeclarationTypeDef",
     {
         "ParameterValueType": ParameterValueTypeType,
         "Name": str,
         "DefaultValues": NotRequired[StringDefaultValuesTypeDef],
         "ValueWhenUnset": NotRequired[StringValueWhenUnsetConfigurationTypeDef],
         "MappedDataSetParameters": NotRequired[Sequence[MappedDataSetParameterTypeDef]],
     },
 )
+DateTimeHierarchyOutputTypeDef = TypedDict(
+    "DateTimeHierarchyOutputTypeDef",
+    {
+        "HierarchyId": str,
+        "DrillDownFilters": NotRequired[List[DrillDownFilterOutputTypeDef]],
+    },
+)
+ExplicitHierarchyOutputTypeDef = TypedDict(
+    "ExplicitHierarchyOutputTypeDef",
+    {
+        "HierarchyId": str,
+        "Columns": List[ColumnIdentifierTypeDef],
+        "DrillDownFilters": NotRequired[List[DrillDownFilterOutputTypeDef]],
+    },
+)
+PredefinedHierarchyOutputTypeDef = TypedDict(
+    "PredefinedHierarchyOutputTypeDef",
+    {
+        "HierarchyId": str,
+        "Columns": List[ColumnIdentifierTypeDef],
+        "DrillDownFilters": NotRequired[List[DrillDownFilterOutputTypeDef]],
+    },
+)
 DescribeAnalysisResponseTypeDef = TypedDict(
     "DescribeAnalysisResponseTypeDef",
     {
         "Analysis": AnalysisTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -8276,45 +9757,45 @@
         "AuthorizedResourceArns": Sequence[str],
         "ExperienceConfiguration": AnonymousUserEmbeddingExperienceConfigurationTypeDef,
         "SessionLifetimeInMinutes": NotRequired[int],
         "SessionTags": NotRequired[Sequence[SessionTagTypeDef]],
         "AllowedDomains": NotRequired[Sequence[str]],
     },
 )
-AssetBundleImportJobOverridePermissionsTypeDef = TypedDict(
-    "AssetBundleImportJobOverridePermissionsTypeDef",
+AssetBundleImportJobOverridePermissionsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobOverridePermissionsOutputTypeDef",
     {
-        "DataSources": NotRequired[List[AssetBundleImportJobDataSourceOverridePermissionsTypeDef]],
-        "DataSets": NotRequired[List[AssetBundleImportJobDataSetOverridePermissionsTypeDef]],
-        "Themes": NotRequired[List[AssetBundleImportJobThemeOverridePermissionsTypeDef]],
-        "Analyses": NotRequired[List[AssetBundleImportJobAnalysisOverridePermissionsTypeDef]],
-        "Dashboards": NotRequired[List[AssetBundleImportJobDashboardOverridePermissionsTypeDef]],
-    },
-)
-AxisDataOptionsTypeDef = TypedDict(
-    "AxisDataOptionsTypeDef",
-    {
-        "NumericAxisOptions": NotRequired[NumericAxisOptionsTypeDef],
-        "DateAxisOptions": NotRequired[DateAxisOptionsTypeDef],
+        "DataSources": NotRequired[
+            List[AssetBundleImportJobDataSourceOverridePermissionsOutputTypeDef]
+        ],
+        "DataSets": NotRequired[List[AssetBundleImportJobDataSetOverridePermissionsOutputTypeDef]],
+        "Themes": NotRequired[List[AssetBundleImportJobThemeOverridePermissionsOutputTypeDef]],
+        "Analyses": NotRequired[List[AssetBundleImportJobAnalysisOverridePermissionsOutputTypeDef]],
+        "Dashboards": NotRequired[
+            List[AssetBundleImportJobDashboardOverridePermissionsOutputTypeDef]
+        ],
     },
 )
-TemplateVersionTypeDef = TypedDict(
-    "TemplateVersionTypeDef",
+AssetBundleImportJobOverridePermissionsTypeDef = TypedDict(
+    "AssetBundleImportJobOverridePermissionsTypeDef",
     {
-        "CreatedTime": NotRequired[datetime],
-        "Errors": NotRequired[List[TemplateErrorTypeDef]],
-        "VersionNumber": NotRequired[int],
-        "Status": NotRequired[ResourceStatusType],
-        "DataSetConfigurations": NotRequired[List[DataSetConfigurationTypeDef]],
-        "Description": NotRequired[str],
-        "SourceEntityArn": NotRequired[str],
-        "ThemeArn": NotRequired[str],
-        "Sheets": NotRequired[List[SheetTypeDef]],
+        "DataSources": NotRequired[
+            Sequence[AssetBundleImportJobDataSourceOverridePermissionsTypeDef]
+        ],
+        "DataSets": NotRequired[Sequence[AssetBundleImportJobDataSetOverridePermissionsTypeDef]],
+        "Themes": NotRequired[Sequence[AssetBundleImportJobThemeOverridePermissionsTypeDef]],
+        "Analyses": NotRequired[Sequence[AssetBundleImportJobAnalysisOverridePermissionsTypeDef]],
+        "Dashboards": NotRequired[
+            Sequence[AssetBundleImportJobDashboardOverridePermissionsTypeDef]
+        ],
     },
 )
+AssetBundleImportJobOverrideTagsUnionTypeDef = Union[
+    AssetBundleImportJobOverrideTagsTypeDef, AssetBundleImportJobOverrideTagsOutputTypeDef
+]
 DestinationParameterValueConfigurationTypeDef = TypedDict(
     "DestinationParameterValueConfigurationTypeDef",
     {
         "CustomValuesConfiguration": NotRequired[CustomValuesConfigurationTypeDef],
         "SelectAllValueOptions": NotRequired[Literal["ALL_VALUES"]],
         "SourceParameterName": NotRequired[str],
         "SourceField": NotRequired[str],
@@ -8326,27 +9807,15 @@
     {
         "StringDatasetParameter": NotRequired[StringDatasetParameterTypeDef],
         "DecimalDatasetParameter": NotRequired[DecimalDatasetParameterTypeDef],
         "IntegerDatasetParameter": NotRequired[IntegerDatasetParameterTypeDef],
         "DateTimeDatasetParameter": NotRequired[DateTimeDatasetParameterTypeDef],
     },
 )
-TransformOperationTypeDef = TypedDict(
-    "TransformOperationTypeDef",
-    {
-        "ProjectOperation": NotRequired[ProjectOperationTypeDef],
-        "FilterOperation": NotRequired[FilterOperationTypeDef],
-        "CreateColumnsOperation": NotRequired[CreateColumnsOperationTypeDef],
-        "RenameColumnOperation": NotRequired[RenameColumnOperationTypeDef],
-        "CastColumnTypeOperation": NotRequired[CastColumnTypeOperationTypeDef],
-        "TagColumnOperation": NotRequired[TagColumnOperationTypeDef],
-        "UntagColumnOperation": NotRequired[UntagColumnOperationTypeDef],
-        "OverrideDatasetParameterOperation": NotRequired[OverrideDatasetParameterOperationTypeDef],
-    },
-)
+ParametersUnionTypeDef = Union[ParametersTypeDef, ParametersOutputTypeDef]
 DateTimeHierarchyTypeDef = TypedDict(
     "DateTimeHierarchyTypeDef",
     {
         "HierarchyId": str,
         "DrillDownFilters": NotRequired[Sequence[DrillDownFilterTypeDef]],
     },
 )
@@ -8362,46 +9831,134 @@
     "PredefinedHierarchyTypeDef",
     {
         "HierarchyId": str,
         "Columns": Sequence[ColumnIdentifierTypeDef],
         "DrillDownFilters": NotRequired[Sequence[DrillDownFilterTypeDef]],
     },
 )
-ListTopicRefreshSchedulesResponseTypeDef = TypedDict(
-    "ListTopicRefreshSchedulesResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "RefreshSchedules": List[TopicRefreshScheduleSummaryTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ForecastConfigurationTypeDef = TypedDict(
     "ForecastConfigurationTypeDef",
     {
         "ForecastProperties": NotRequired[TimeBasedForecastPropertiesTypeDef],
         "Scenario": NotRequired[ForecastScenarioTypeDef],
     },
 )
+AxisDataOptionsOutputTypeDef = TypedDict(
+    "AxisDataOptionsOutputTypeDef",
+    {
+        "NumericAxisOptions": NotRequired[NumericAxisOptionsOutputTypeDef],
+        "DateAxisOptions": NotRequired[DateAxisOptionsTypeDef],
+    },
+)
+AxisDataOptionsTypeDef = TypedDict(
+    "AxisDataOptionsTypeDef",
+    {
+        "NumericAxisOptions": NotRequired[NumericAxisOptionsTypeDef],
+        "DateAxisOptions": NotRequired[DateAxisOptionsTypeDef],
+    },
+)
+TransformOperationOutputTypeDef = TypedDict(
+    "TransformOperationOutputTypeDef",
+    {
+        "ProjectOperation": NotRequired[ProjectOperationOutputTypeDef],
+        "FilterOperation": NotRequired[FilterOperationTypeDef],
+        "CreateColumnsOperation": NotRequired[CreateColumnsOperationOutputTypeDef],
+        "RenameColumnOperation": NotRequired[RenameColumnOperationTypeDef],
+        "CastColumnTypeOperation": NotRequired[CastColumnTypeOperationTypeDef],
+        "TagColumnOperation": NotRequired[TagColumnOperationOutputTypeDef],
+        "UntagColumnOperation": NotRequired[UntagColumnOperationOutputTypeDef],
+        "OverrideDatasetParameterOperation": NotRequired[
+            OverrideDatasetParameterOperationOutputTypeDef
+        ],
+    },
+)
+TransformOperationTypeDef = TypedDict(
+    "TransformOperationTypeDef",
+    {
+        "ProjectOperation": NotRequired[ProjectOperationTypeDef],
+        "FilterOperation": NotRequired[FilterOperationTypeDef],
+        "CreateColumnsOperation": NotRequired[CreateColumnsOperationTypeDef],
+        "RenameColumnOperation": NotRequired[RenameColumnOperationTypeDef],
+        "CastColumnTypeOperation": NotRequired[CastColumnTypeOperationTypeDef],
+        "TagColumnOperation": NotRequired[TagColumnOperationTypeDef],
+        "UntagColumnOperation": NotRequired[UntagColumnOperationTypeDef],
+        "OverrideDatasetParameterOperation": NotRequired[OverrideDatasetParameterOperationTypeDef],
+    },
+)
+TemplateVersionTypeDef = TypedDict(
+    "TemplateVersionTypeDef",
+    {
+        "CreatedTime": NotRequired[datetime],
+        "Errors": NotRequired[List[TemplateErrorTypeDef]],
+        "VersionNumber": NotRequired[int],
+        "Status": NotRequired[ResourceStatusType],
+        "DataSetConfigurations": NotRequired[List[DataSetConfigurationOutputTypeDef]],
+        "Description": NotRequired[str],
+        "SourceEntityArn": NotRequired[str],
+        "ThemeArn": NotRequired[str],
+        "Sheets": NotRequired[List[SheetTypeDef]],
+    },
+)
+SetParameterValueConfigurationOutputTypeDef = TypedDict(
+    "SetParameterValueConfigurationOutputTypeDef",
+    {
+        "DestinationParameterName": str,
+        "Value": DestinationParameterValueConfigurationOutputTypeDef,
+    },
+)
+VisualPaletteOutputTypeDef = TypedDict(
+    "VisualPaletteOutputTypeDef",
+    {
+        "ChartColor": NotRequired[str],
+        "ColorMap": NotRequired[List[DataPathColorTypeDef]],
+    },
+)
 VisualPaletteTypeDef = TypedDict(
     "VisualPaletteTypeDef",
     {
         "ChartColor": NotRequired[str],
         "ColorMap": NotRequired[Sequence[DataPathColorTypeDef]],
     },
 )
+PivotTableFieldCollapseStateOptionOutputTypeDef = TypedDict(
+    "PivotTableFieldCollapseStateOptionOutputTypeDef",
+    {
+        "Target": PivotTableFieldCollapseStateTargetOutputTypeDef,
+        "State": NotRequired[PivotTableFieldCollapseStateType],
+    },
+)
 PivotTableFieldCollapseStateOptionTypeDef = TypedDict(
     "PivotTableFieldCollapseStateOptionTypeDef",
     {
         "Target": PivotTableFieldCollapseStateTargetTypeDef,
         "State": NotRequired[PivotTableFieldCollapseStateType],
     },
 )
+TopicCalculatedFieldOutputTypeDef = TypedDict(
+    "TopicCalculatedFieldOutputTypeDef",
+    {
+        "CalculatedFieldName": str,
+        "Expression": str,
+        "CalculatedFieldDescription": NotRequired[str],
+        "CalculatedFieldSynonyms": NotRequired[List[str]],
+        "IsIncludedInTopic": NotRequired[bool],
+        "DisableIndexing": NotRequired[bool],
+        "ColumnDataRole": NotRequired[ColumnDataRoleType],
+        "TimeGranularity": NotRequired[TopicTimeGranularityType],
+        "DefaultFormatting": NotRequired[DefaultFormattingTypeDef],
+        "Aggregation": NotRequired[DefaultAggregationType],
+        "ComparativeOrder": NotRequired[ComparativeOrderOutputTypeDef],
+        "SemanticType": NotRequired[SemanticTypeOutputTypeDef],
+        "AllowedAggregations": NotRequired[List[AuthorSpecifiedAggregationType]],
+        "NotAllowedAggregations": NotRequired[List[AuthorSpecifiedAggregationType]],
+        "NeverAggregateInFilter": NotRequired[bool],
+        "CellValueSynonyms": NotRequired[List[CellValueSynonymOutputTypeDef]],
+        "NonAdditive": NotRequired[bool],
+    },
+)
 TopicCalculatedFieldTypeDef = TypedDict(
     "TopicCalculatedFieldTypeDef",
     {
         "CalculatedFieldName": str,
         "Expression": str,
         "CalculatedFieldDescription": NotRequired[str],
         "CalculatedFieldSynonyms": NotRequired[Sequence[str]],
@@ -8416,14 +9973,36 @@
         "AllowedAggregations": NotRequired[Sequence[AuthorSpecifiedAggregationType]],
         "NotAllowedAggregations": NotRequired[Sequence[AuthorSpecifiedAggregationType]],
         "NeverAggregateInFilter": NotRequired[bool],
         "CellValueSynonyms": NotRequired[Sequence[CellValueSynonymTypeDef]],
         "NonAdditive": NotRequired[bool],
     },
 )
+TopicColumnOutputTypeDef = TypedDict(
+    "TopicColumnOutputTypeDef",
+    {
+        "ColumnName": str,
+        "ColumnFriendlyName": NotRequired[str],
+        "ColumnDescription": NotRequired[str],
+        "ColumnSynonyms": NotRequired[List[str]],
+        "ColumnDataRole": NotRequired[ColumnDataRoleType],
+        "Aggregation": NotRequired[DefaultAggregationType],
+        "IsIncludedInTopic": NotRequired[bool],
+        "DisableIndexing": NotRequired[bool],
+        "ComparativeOrder": NotRequired[ComparativeOrderOutputTypeDef],
+        "SemanticType": NotRequired[SemanticTypeOutputTypeDef],
+        "TimeGranularity": NotRequired[TopicTimeGranularityType],
+        "AllowedAggregations": NotRequired[List[AuthorSpecifiedAggregationType]],
+        "NotAllowedAggregations": NotRequired[List[AuthorSpecifiedAggregationType]],
+        "DefaultFormatting": NotRequired[DefaultFormattingTypeDef],
+        "NeverAggregateInFilter": NotRequired[bool],
+        "CellValueSynonyms": NotRequired[List[CellValueSynonymOutputTypeDef]],
+        "NonAdditive": NotRequired[bool],
+    },
+)
 TopicColumnTypeDef = TypedDict(
     "TopicColumnTypeDef",
     {
         "ColumnName": str,
         "ColumnFriendlyName": NotRequired[str],
         "ColumnDescription": NotRequired[str],
         "ColumnSynonyms": NotRequired[Sequence[str]],
@@ -8438,14 +10017,22 @@
         "NotAllowedAggregations": NotRequired[Sequence[AuthorSpecifiedAggregationType]],
         "DefaultFormatting": NotRequired[DefaultFormattingTypeDef],
         "NeverAggregateInFilter": NotRequired[bool],
         "CellValueSynonyms": NotRequired[Sequence[CellValueSynonymTypeDef]],
         "NonAdditive": NotRequired[bool],
     },
 )
+ChartAxisLabelOptionsOutputTypeDef = TypedDict(
+    "ChartAxisLabelOptionsOutputTypeDef",
+    {
+        "Visibility": NotRequired[VisibilityType],
+        "SortIconVisibility": NotRequired[VisibilityType],
+        "AxisLabelOptions": NotRequired[List[AxisLabelOptionsTypeDef]],
+    },
+)
 ChartAxisLabelOptionsTypeDef = TypedDict(
     "ChartAxisLabelOptionsTypeDef",
     {
         "Visibility": NotRequired[VisibilityType],
         "SortIconVisibility": NotRequired[VisibilityType],
         "AxisLabelOptions": NotRequired[Sequence[AxisLabelOptionsTypeDef]],
     },
@@ -8540,14 +10127,22 @@
 TableFieldLinkContentConfigurationTypeDef = TypedDict(
     "TableFieldLinkContentConfigurationTypeDef",
     {
         "CustomTextContent": NotRequired[TableFieldCustomTextContentTypeDef],
         "CustomIconContent": NotRequired[TableFieldCustomIconContentTypeDef],
     },
 )
+GeospatialPointStyleOptionsOutputTypeDef = TypedDict(
+    "GeospatialPointStyleOptionsOutputTypeDef",
+    {
+        "SelectedPointStyle": NotRequired[GeospatialSelectedPointStyleType],
+        "ClusterMarkerConfiguration": NotRequired[ClusterMarkerConfigurationTypeDef],
+        "HeatmapConfiguration": NotRequired[GeospatialHeatmapConfigurationOutputTypeDef],
+    },
+)
 GeospatialPointStyleOptionsTypeDef = TypedDict(
     "GeospatialPointStyleOptionsTypeDef",
     {
         "SelectedPointStyle": NotRequired[GeospatialSelectedPointStyleType],
         "ClusterMarkerConfiguration": NotRequired[ClusterMarkerConfigurationTypeDef],
         "HeatmapConfiguration": NotRequired[GeospatialHeatmapConfigurationTypeDef],
     },
@@ -8561,28 +10156,41 @@
         "HorizontalTextAlignment": NotRequired[HorizontalTextAlignmentType],
         "VerticalTextAlignment": NotRequired[VerticalTextAlignmentType],
         "BackgroundColor": NotRequired[str],
         "Height": NotRequired[int],
         "Border": NotRequired[GlobalTableBorderOptionsTypeDef],
     },
 )
+ConditionalFormattingColorOutputTypeDef = TypedDict(
+    "ConditionalFormattingColorOutputTypeDef",
+    {
+        "Solid": NotRequired[ConditionalFormattingSolidColorTypeDef],
+        "Gradient": NotRequired[ConditionalFormattingGradientColorOutputTypeDef],
+    },
+)
 ConditionalFormattingColorTypeDef = TypedDict(
     "ConditionalFormattingColorTypeDef",
     {
         "Solid": NotRequired[ConditionalFormattingSolidColorTypeDef],
         "Gradient": NotRequired[ConditionalFormattingGradientColorTypeDef],
     },
 )
 DefaultInteractiveLayoutConfigurationTypeDef = TypedDict(
     "DefaultInteractiveLayoutConfigurationTypeDef",
     {
         "Grid": NotRequired[DefaultGridLayoutConfigurationTypeDef],
         "FreeForm": NotRequired[DefaultFreeFormLayoutConfigurationTypeDef],
     },
 )
+SheetControlLayoutConfigurationOutputTypeDef = TypedDict(
+    "SheetControlLayoutConfigurationOutputTypeDef",
+    {
+        "GridLayout": NotRequired[GridLayoutConfigurationOutputTypeDef],
+    },
+)
 SheetControlLayoutConfigurationTypeDef = TypedDict(
     "SheetControlLayoutConfigurationTypeDef",
     {
         "GridLayout": NotRequired[GridLayoutConfigurationTypeDef],
     },
 )
 DataSetRefreshPropertiesTypeDef = TypedDict(
@@ -8594,14 +10202,23 @@
 SeriesItemTypeDef = TypedDict(
     "SeriesItemTypeDef",
     {
         "FieldSeriesItem": NotRequired[FieldSeriesItemTypeDef],
         "DataFieldSeriesItem": NotRequired[DataFieldSeriesItemTypeDef],
     },
 )
+ThemeConfigurationOutputTypeDef = TypedDict(
+    "ThemeConfigurationOutputTypeDef",
+    {
+        "DataColorPalette": NotRequired[DataColorPaletteOutputTypeDef],
+        "UIColorPalette": NotRequired[UIColorPaletteTypeDef],
+        "Sheet": NotRequired[SheetStyleTypeDef],
+        "Typography": NotRequired[TypographyOutputTypeDef],
+    },
+)
 ThemeConfigurationTypeDef = TypedDict(
     "ThemeConfigurationTypeDef",
     {
         "DataColorPalette": NotRequired[DataColorPaletteTypeDef],
         "UIColorPalette": NotRequired[UIColorPaletteTypeDef],
         "Sheet": NotRequired[SheetStyleTypeDef],
         "Typography": NotRequired[TypographyTypeDef],
@@ -8658,14 +10275,30 @@
     "ReferenceLineDynamicDataConfigurationTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "Calculation": NumericalAggregationFunctionTypeDef,
         "MeasureAggregationFunction": NotRequired[AggregationFunctionTypeDef],
     },
 )
+TopicFilterOutputTypeDef = TypedDict(
+    "TopicFilterOutputTypeDef",
+    {
+        "FilterName": str,
+        "OperandFieldName": str,
+        "FilterDescription": NotRequired[str],
+        "FilterClass": NotRequired[FilterClassType],
+        "FilterSynonyms": NotRequired[List[str]],
+        "FilterType": NotRequired[NamedFilterTypeType],
+        "CategoryFilter": NotRequired[TopicCategoryFilterOutputTypeDef],
+        "NumericEqualityFilter": NotRequired[TopicNumericEqualityFilterTypeDef],
+        "NumericRangeFilter": NotRequired[TopicNumericRangeFilterTypeDef],
+        "DateRangeFilter": NotRequired[TopicDateRangeFilterTypeDef],
+        "RelativeDateFilter": NotRequired[TopicRelativeDateFilterTypeDef],
+    },
+)
 TopicFilterTypeDef = TypedDict(
     "TopicFilterTypeDef",
     {
         "FilterName": str,
         "OperandFieldName": str,
         "FilterDescription": NotRequired[str],
         "FilterClass": NotRequired[FilterClassType],
@@ -8674,26 +10307,37 @@
         "CategoryFilter": NotRequired[TopicCategoryFilterTypeDef],
         "NumericEqualityFilter": NotRequired[TopicNumericEqualityFilterTypeDef],
         "NumericRangeFilter": NotRequired[TopicNumericRangeFilterTypeDef],
         "DateRangeFilter": NotRequired[TopicDateRangeFilterTypeDef],
         "RelativeDateFilter": NotRequired[TopicRelativeDateFilterTypeDef],
     },
 )
-DataSourcePaginatorTypeDef = TypedDict(
-    "DataSourcePaginatorTypeDef",
+AssetBundleImportJobDataSourceOverrideParametersOutputTypeDef = TypedDict(
+    "AssetBundleImportJobDataSourceOverrideParametersOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "Name": NotRequired[str],
+        "DataSourceParameters": NotRequired[DataSourceParametersOutputTypeDef],
+        "VpcConnectionProperties": NotRequired[VpcConnectionPropertiesTypeDef],
+        "SslProperties": NotRequired[SslPropertiesTypeDef],
+        "Credentials": NotRequired[AssetBundleImportJobDataSourceCredentialsTypeDef],
+    },
+)
+DataSourceTypeDef = TypedDict(
+    "DataSourceTypeDef",
     {
         "Arn": NotRequired[str],
         "DataSourceId": NotRequired[str],
         "Name": NotRequired[str],
         "Type": NotRequired[DataSourceTypeType],
         "Status": NotRequired[ResourceStatusType],
         "CreatedTime": NotRequired[datetime],
         "LastUpdatedTime": NotRequired[datetime],
-        "DataSourceParameters": NotRequired[DataSourceParametersPaginatorTypeDef],
-        "AlternateDataSourceParameters": NotRequired[List[DataSourceParametersPaginatorTypeDef]],
+        "DataSourceParameters": NotRequired[DataSourceParametersOutputTypeDef],
+        "AlternateDataSourceParameters": NotRequired[List[DataSourceParametersOutputTypeDef]],
         "VpcConnectionProperties": NotRequired[VpcConnectionPropertiesTypeDef],
         "SslProperties": NotRequired[SslPropertiesTypeDef],
         "ErrorInfo": NotRequired[DataSourceErrorInfoTypeDef],
         "SecretArn": NotRequired[str],
     },
 )
 AssetBundleImportJobDataSourceOverrideParametersTypeDef = TypedDict(
@@ -8711,59 +10355,45 @@
     "CredentialPairTypeDef",
     {
         "Username": str,
         "Password": str,
         "AlternateDataSourceParameters": NotRequired[Sequence[DataSourceParametersTypeDef]],
     },
 )
-DataSourceTypeDef = TypedDict(
-    "DataSourceTypeDef",
-    {
-        "Arn": NotRequired[str],
-        "DataSourceId": NotRequired[str],
-        "Name": NotRequired[str],
-        "Type": NotRequired[DataSourceTypeType],
-        "Status": NotRequired[ResourceStatusType],
-        "CreatedTime": NotRequired[datetime],
-        "LastUpdatedTime": NotRequired[datetime],
-        "DataSourceParameters": NotRequired[DataSourceParametersTypeDef],
-        "AlternateDataSourceParameters": NotRequired[List[DataSourceParametersTypeDef]],
-        "VpcConnectionProperties": NotRequired[VpcConnectionPropertiesTypeDef],
-        "SslProperties": NotRequired[SslPropertiesTypeDef],
-        "ErrorInfo": NotRequired[DataSourceErrorInfoTypeDef],
-        "SecretArn": NotRequired[str],
-    },
-)
-CreateRefreshScheduleRequestRequestTypeDef = TypedDict(
-    "CreateRefreshScheduleRequestRequestTypeDef",
-    {
-        "DataSetId": str,
-        "AwsAccountId": str,
-        "Schedule": RefreshScheduleTypeDef,
-    },
-)
+DataSourceParametersUnionTypeDef = Union[
+    DataSourceParametersTypeDef, DataSourceParametersExtraOutputTypeDef
+]
 DescribeRefreshScheduleResponseTypeDef = TypedDict(
     "DescribeRefreshScheduleResponseTypeDef",
     {
-        "RefreshSchedule": RefreshScheduleTypeDef,
+        "RefreshSchedule": RefreshScheduleOutputTypeDef,
         "Status": int,
         "RequestId": str,
         "Arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListRefreshSchedulesResponseTypeDef = TypedDict(
     "ListRefreshSchedulesResponseTypeDef",
     {
-        "RefreshSchedules": List[RefreshScheduleTypeDef],
+        "RefreshSchedules": List[RefreshScheduleOutputTypeDef],
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateRefreshScheduleRequestRequestTypeDef = TypedDict(
+    "CreateRefreshScheduleRequestRequestTypeDef",
+    {
+        "DataSetId": str,
+        "AwsAccountId": str,
+        "Schedule": RefreshScheduleTypeDef,
+    },
+)
+RefreshScheduleUnionTypeDef = Union[RefreshScheduleTypeDef, RefreshScheduleOutputTypeDef]
 UpdateRefreshScheduleRequestRequestTypeDef = TypedDict(
     "UpdateRefreshScheduleRequestRequestTypeDef",
     {
         "DataSetId": str,
         "AwsAccountId": str,
         "Schedule": RefreshScheduleTypeDef,
     },
@@ -8773,110 +10403,188 @@
     {
         "Dashboard": NotRequired[RegisteredUserDashboardEmbeddingConfigurationTypeDef],
         "QuickSightConsole": NotRequired[
             RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef
         ],
         "QSearchBar": NotRequired[RegisteredUserQSearchBarEmbeddingConfigurationTypeDef],
         "DashboardVisual": NotRequired[RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef],
+        "GenerativeQnA": NotRequired[RegisteredUserGenerativeQnAEmbeddingConfigurationTypeDef],
     },
 )
 SnapshotJobResultFileGroupTypeDef = TypedDict(
     "SnapshotJobResultFileGroupTypeDef",
     {
-        "Files": NotRequired[List[SnapshotFileTypeDef]],
+        "Files": NotRequired[List[SnapshotFileOutputTypeDef]],
         "S3Results": NotRequired[List[SnapshotJobS3ResultTypeDef]],
     },
 )
+PhysicalTableUnionTypeDef = Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]
 DefaultSectionBasedLayoutConfigurationTypeDef = TypedDict(
     "DefaultSectionBasedLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
     },
 )
+FreeFormLayoutConfigurationOutputTypeDef = TypedDict(
+    "FreeFormLayoutConfigurationOutputTypeDef",
+    {
+        "Elements": List[FreeFormLayoutElementOutputTypeDef],
+        "CanvasSizeOptions": NotRequired[FreeFormLayoutCanvasSizeOptionsTypeDef],
+    },
+)
+FreeFormSectionLayoutConfigurationOutputTypeDef = TypedDict(
+    "FreeFormSectionLayoutConfigurationOutputTypeDef",
+    {
+        "Elements": List[FreeFormLayoutElementOutputTypeDef],
+    },
+)
 FreeFormLayoutConfigurationTypeDef = TypedDict(
     "FreeFormLayoutConfigurationTypeDef",
     {
         "Elements": Sequence[FreeFormLayoutElementTypeDef],
         "CanvasSizeOptions": NotRequired[FreeFormLayoutCanvasSizeOptionsTypeDef],
     },
 )
 FreeFormSectionLayoutConfigurationTypeDef = TypedDict(
     "FreeFormSectionLayoutConfigurationTypeDef",
     {
         "Elements": Sequence[FreeFormLayoutElementTypeDef],
     },
 )
+SnapshotConfigurationOutputTypeDef = TypedDict(
+    "SnapshotConfigurationOutputTypeDef",
+    {
+        "FileGroups": List[SnapshotFileGroupOutputTypeDef],
+        "DestinationConfiguration": NotRequired[SnapshotDestinationConfigurationOutputTypeDef],
+        "Parameters": NotRequired[ParametersOutputTypeDef],
+    },
+)
 SnapshotConfigurationTypeDef = TypedDict(
     "SnapshotConfigurationTypeDef",
     {
-        "FileGroups": List[SnapshotFileGroupTypeDef],
+        "FileGroups": Sequence[SnapshotFileGroupTypeDef],
         "DestinationConfiguration": NotRequired[SnapshotDestinationConfigurationTypeDef],
         "Parameters": NotRequired[ParametersTypeDef],
     },
 )
+ParameterDeclarationOutputTypeDef = TypedDict(
+    "ParameterDeclarationOutputTypeDef",
+    {
+        "StringParameterDeclaration": NotRequired[StringParameterDeclarationOutputTypeDef],
+        "DecimalParameterDeclaration": NotRequired[DecimalParameterDeclarationOutputTypeDef],
+        "IntegerParameterDeclaration": NotRequired[IntegerParameterDeclarationOutputTypeDef],
+        "DateTimeParameterDeclaration": NotRequired[DateTimeParameterDeclarationOutputTypeDef],
+    },
+)
 ParameterDeclarationTypeDef = TypedDict(
     "ParameterDeclarationTypeDef",
     {
         "StringParameterDeclaration": NotRequired[StringParameterDeclarationTypeDef],
         "DecimalParameterDeclaration": NotRequired[DecimalParameterDeclarationTypeDef],
         "IntegerParameterDeclaration": NotRequired[IntegerParameterDeclarationTypeDef],
         "DateTimeParameterDeclaration": NotRequired[DateTimeParameterDeclarationTypeDef],
     },
 )
+ColumnHierarchyOutputTypeDef = TypedDict(
+    "ColumnHierarchyOutputTypeDef",
+    {
+        "ExplicitHierarchy": NotRequired[ExplicitHierarchyOutputTypeDef],
+        "DateTimeHierarchy": NotRequired[DateTimeHierarchyOutputTypeDef],
+        "PredefinedHierarchy": NotRequired[PredefinedHierarchyOutputTypeDef],
+    },
+)
 DescribeDashboardResponseTypeDef = TypedDict(
     "DescribeDashboardResponseTypeDef",
     {
         "Dashboard": DashboardTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-TemplateTypeDef = TypedDict(
-    "TemplateTypeDef",
-    {
-        "Arn": NotRequired[str],
-        "Name": NotRequired[str],
-        "Version": NotRequired[TemplateVersionTypeDef],
-        "TemplateId": NotRequired[str],
-        "LastUpdatedTime": NotRequired[datetime],
-        "CreatedTime": NotRequired[datetime],
-    },
-)
+AssetBundleImportJobOverridePermissionsUnionTypeDef = Union[
+    AssetBundleImportJobOverridePermissionsTypeDef,
+    AssetBundleImportJobOverridePermissionsOutputTypeDef,
+]
 SetParameterValueConfigurationTypeDef = TypedDict(
     "SetParameterValueConfigurationTypeDef",
     {
         "DestinationParameterName": str,
         "Value": DestinationParameterValueConfigurationTypeDef,
     },
 )
+DatasetParameterUnionTypeDef = Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
+ColumnHierarchyTypeDef = TypedDict(
+    "ColumnHierarchyTypeDef",
+    {
+        "ExplicitHierarchy": NotRequired[ExplicitHierarchyTypeDef],
+        "DateTimeHierarchy": NotRequired[DateTimeHierarchyTypeDef],
+        "PredefinedHierarchy": NotRequired[PredefinedHierarchyTypeDef],
+    },
+)
+LogicalTableOutputTypeDef = TypedDict(
+    "LogicalTableOutputTypeDef",
+    {
+        "Alias": str,
+        "Source": LogicalTableSourceTypeDef,
+        "DataTransforms": NotRequired[List[TransformOperationOutputTypeDef]],
+    },
+)
 LogicalTableTypeDef = TypedDict(
     "LogicalTableTypeDef",
     {
         "Alias": str,
         "Source": LogicalTableSourceTypeDef,
         "DataTransforms": NotRequired[Sequence[TransformOperationTypeDef]],
     },
 )
-ColumnHierarchyTypeDef = TypedDict(
-    "ColumnHierarchyTypeDef",
+TemplateTypeDef = TypedDict(
+    "TemplateTypeDef",
     {
-        "ExplicitHierarchy": NotRequired[ExplicitHierarchyTypeDef],
-        "DateTimeHierarchy": NotRequired[DateTimeHierarchyTypeDef],
-        "PredefinedHierarchy": NotRequired[PredefinedHierarchyTypeDef],
+        "Arn": NotRequired[str],
+        "Name": NotRequired[str],
+        "Version": NotRequired[TemplateVersionTypeDef],
+        "TemplateId": NotRequired[str],
+        "LastUpdatedTime": NotRequired[datetime],
+        "CreatedTime": NotRequired[datetime],
+    },
+)
+CustomActionSetParametersOperationOutputTypeDef = TypedDict(
+    "CustomActionSetParametersOperationOutputTypeDef",
+    {
+        "ParameterValueConfigurations": List[SetParameterValueConfigurationOutputTypeDef],
+    },
+)
+PivotTableFieldOptionsOutputTypeDef = TypedDict(
+    "PivotTableFieldOptionsOutputTypeDef",
+    {
+        "SelectedFieldOptions": NotRequired[List[PivotTableFieldOptionTypeDef]],
+        "DataPathOptions": NotRequired[List[PivotTableDataPathOptionOutputTypeDef]],
+        "CollapseStateOptions": NotRequired[List[PivotTableFieldCollapseStateOptionOutputTypeDef]],
     },
 )
 PivotTableFieldOptionsTypeDef = TypedDict(
     "PivotTableFieldOptionsTypeDef",
     {
         "SelectedFieldOptions": NotRequired[Sequence[PivotTableFieldOptionTypeDef]],
         "DataPathOptions": NotRequired[Sequence[PivotTableDataPathOptionTypeDef]],
         "CollapseStateOptions": NotRequired[Sequence[PivotTableFieldCollapseStateOptionTypeDef]],
     },
 )
+AxisDisplayOptionsOutputTypeDef = TypedDict(
+    "AxisDisplayOptionsOutputTypeDef",
+    {
+        "TickLabelOptions": NotRequired[AxisTickLabelOptionsTypeDef],
+        "AxisLineVisibility": NotRequired[VisibilityType],
+        "GridLineVisibility": NotRequired[VisibilityType],
+        "DataOptions": NotRequired[AxisDataOptionsOutputTypeDef],
+        "ScrollbarOptions": NotRequired[ScrollBarOptionsTypeDef],
+        "AxisOffset": NotRequired[str],
+    },
+)
 AxisDisplayOptionsTypeDef = TypedDict(
     "AxisDisplayOptionsTypeDef",
     {
         "TickLabelOptions": NotRequired[AxisTickLabelOptionsTypeDef],
         "AxisLineVisibility": NotRequired[VisibilityType],
         "GridLineVisibility": NotRequired[VisibilityType],
         "DataOptions": NotRequired[AxisDataOptionsTypeDef],
@@ -8906,66 +10614,130 @@
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
         "DisplayOptions": NotRequired[DateTimePickerControlDisplayOptionsTypeDef],
     },
 )
+DefaultFilterDropDownControlOptionsOutputTypeDef = TypedDict(
+    "DefaultFilterDropDownControlOptionsOutputTypeDef",
+    {
+        "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[FilterSelectableValuesOutputTypeDef],
+    },
+)
 DefaultFilterDropDownControlOptionsTypeDef = TypedDict(
     "DefaultFilterDropDownControlOptionsTypeDef",
     {
         "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
         "Type": NotRequired[SheetControlListTypeType],
         "SelectableValues": NotRequired[FilterSelectableValuesTypeDef],
     },
 )
+FilterDropDownControlOutputTypeDef = TypedDict(
+    "FilterDropDownControlOutputTypeDef",
+    {
+        "FilterControlId": str,
+        "Title": str,
+        "SourceFilterId": str,
+        "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[FilterSelectableValuesOutputTypeDef],
+        "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationOutputTypeDef],
+    },
+)
 FilterDropDownControlTypeDef = TypedDict(
     "FilterDropDownControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
         "Type": NotRequired[SheetControlListTypeType],
         "SelectableValues": NotRequired[FilterSelectableValuesTypeDef],
         "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationTypeDef],
     },
 )
+ParameterDropDownControlOutputTypeDef = TypedDict(
+    "ParameterDropDownControlOutputTypeDef",
+    {
+        "ParameterControlId": str,
+        "Title": str,
+        "SourceParameterName": str,
+        "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[ParameterSelectableValuesOutputTypeDef],
+        "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationOutputTypeDef],
+    },
+)
 ParameterDropDownControlTypeDef = TypedDict(
     "ParameterDropDownControlTypeDef",
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
         "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
         "Type": NotRequired[SheetControlListTypeType],
         "SelectableValues": NotRequired[ParameterSelectableValuesTypeDef],
         "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationTypeDef],
     },
 )
+DefaultFilterListControlOptionsOutputTypeDef = TypedDict(
+    "DefaultFilterListControlOptionsOutputTypeDef",
+    {
+        "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[FilterSelectableValuesOutputTypeDef],
+    },
+)
 DefaultFilterListControlOptionsTypeDef = TypedDict(
     "DefaultFilterListControlOptionsTypeDef",
     {
         "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
         "Type": NotRequired[SheetControlListTypeType],
         "SelectableValues": NotRequired[FilterSelectableValuesTypeDef],
     },
 )
+FilterListControlOutputTypeDef = TypedDict(
+    "FilterListControlOutputTypeDef",
+    {
+        "FilterControlId": str,
+        "Title": str,
+        "SourceFilterId": str,
+        "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[FilterSelectableValuesOutputTypeDef],
+        "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationOutputTypeDef],
+    },
+)
 FilterListControlTypeDef = TypedDict(
     "FilterListControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
         "Type": NotRequired[SheetControlListTypeType],
         "SelectableValues": NotRequired[FilterSelectableValuesTypeDef],
         "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationTypeDef],
     },
 )
+ParameterListControlOutputTypeDef = TypedDict(
+    "ParameterListControlOutputTypeDef",
+    {
+        "ParameterControlId": str,
+        "Title": str,
+        "SourceParameterName": str,
+        "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[ParameterSelectableValuesOutputTypeDef],
+        "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationOutputTypeDef],
+    },
+)
 ParameterListControlTypeDef = TypedDict(
     "ParameterListControlTypeDef",
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
         "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
@@ -9088,14 +10860,32 @@
 TableFieldLinkConfigurationTypeDef = TypedDict(
     "TableFieldLinkConfigurationTypeDef",
     {
         "Target": URLTargetConfigurationType,
         "Content": TableFieldLinkContentConfigurationTypeDef,
     },
 )
+PivotTableOptionsOutputTypeDef = TypedDict(
+    "PivotTableOptionsOutputTypeDef",
+    {
+        "MetricPlacement": NotRequired[PivotTableMetricPlacementType],
+        "SingleMetricVisibility": NotRequired[VisibilityType],
+        "ColumnNamesVisibility": NotRequired[VisibilityType],
+        "ToggleButtonsVisibility": NotRequired[VisibilityType],
+        "ColumnHeaderStyle": NotRequired[TableCellStyleTypeDef],
+        "RowHeaderStyle": NotRequired[TableCellStyleTypeDef],
+        "CellStyle": NotRequired[TableCellStyleTypeDef],
+        "RowFieldNamesStyle": NotRequired[TableCellStyleTypeDef],
+        "RowAlternateColorOptions": NotRequired[RowAlternateColorOptionsOutputTypeDef],
+        "CollapsedRowDimensionsVisibility": NotRequired[VisibilityType],
+        "RowsLayout": NotRequired[PivotTableRowsLayoutType],
+        "RowsLabelOptions": NotRequired[PivotTableRowsLabelOptionsTypeDef],
+        "DefaultCellWidth": NotRequired[str],
+    },
+)
 PivotTableOptionsTypeDef = TypedDict(
     "PivotTableOptionsTypeDef",
     {
         "MetricPlacement": NotRequired[PivotTableMetricPlacementType],
         "SingleMetricVisibility": NotRequired[VisibilityType],
         "ColumnNamesVisibility": NotRequired[VisibilityType],
         "ToggleButtonsVisibility": NotRequired[VisibilityType],
@@ -9106,60 +10896,167 @@
         "RowAlternateColorOptions": NotRequired[RowAlternateColorOptionsTypeDef],
         "CollapsedRowDimensionsVisibility": NotRequired[VisibilityType],
         "RowsLayout": NotRequired[PivotTableRowsLayoutType],
         "RowsLabelOptions": NotRequired[PivotTableRowsLabelOptionsTypeDef],
         "DefaultCellWidth": NotRequired[str],
     },
 )
+PivotTotalOptionsOutputTypeDef = TypedDict(
+    "PivotTotalOptionsOutputTypeDef",
+    {
+        "TotalsVisibility": NotRequired[VisibilityType],
+        "Placement": NotRequired[TableTotalsPlacementType],
+        "ScrollStatus": NotRequired[TableTotalsScrollStatusType],
+        "CustomLabel": NotRequired[str],
+        "TotalCellStyle": NotRequired[TableCellStyleTypeDef],
+        "ValueCellStyle": NotRequired[TableCellStyleTypeDef],
+        "MetricHeaderCellStyle": NotRequired[TableCellStyleTypeDef],
+        "TotalAggregationOptions": NotRequired[List[TotalAggregationOptionTypeDef]],
+    },
+)
 PivotTotalOptionsTypeDef = TypedDict(
     "PivotTotalOptionsTypeDef",
     {
         "TotalsVisibility": NotRequired[VisibilityType],
         "Placement": NotRequired[TableTotalsPlacementType],
         "ScrollStatus": NotRequired[TableTotalsScrollStatusType],
         "CustomLabel": NotRequired[str],
         "TotalCellStyle": NotRequired[TableCellStyleTypeDef],
         "ValueCellStyle": NotRequired[TableCellStyleTypeDef],
         "MetricHeaderCellStyle": NotRequired[TableCellStyleTypeDef],
         "TotalAggregationOptions": NotRequired[Sequence[TotalAggregationOptionTypeDef]],
     },
 )
+SubtotalOptionsOutputTypeDef = TypedDict(
+    "SubtotalOptionsOutputTypeDef",
+    {
+        "TotalsVisibility": NotRequired[VisibilityType],
+        "CustomLabel": NotRequired[str],
+        "FieldLevel": NotRequired[PivotTableSubtotalLevelType],
+        "FieldLevelOptions": NotRequired[List[PivotTableFieldSubtotalOptionsTypeDef]],
+        "TotalCellStyle": NotRequired[TableCellStyleTypeDef],
+        "ValueCellStyle": NotRequired[TableCellStyleTypeDef],
+        "MetricHeaderCellStyle": NotRequired[TableCellStyleTypeDef],
+        "StyleTargets": NotRequired[List[TableStyleTargetTypeDef]],
+    },
+)
 SubtotalOptionsTypeDef = TypedDict(
     "SubtotalOptionsTypeDef",
     {
         "TotalsVisibility": NotRequired[VisibilityType],
         "CustomLabel": NotRequired[str],
         "FieldLevel": NotRequired[PivotTableSubtotalLevelType],
         "FieldLevelOptions": NotRequired[Sequence[PivotTableFieldSubtotalOptionsTypeDef]],
         "TotalCellStyle": NotRequired[TableCellStyleTypeDef],
         "ValueCellStyle": NotRequired[TableCellStyleTypeDef],
         "MetricHeaderCellStyle": NotRequired[TableCellStyleTypeDef],
         "StyleTargets": NotRequired[Sequence[TableStyleTargetTypeDef]],
     },
 )
+TableOptionsOutputTypeDef = TypedDict(
+    "TableOptionsOutputTypeDef",
+    {
+        "Orientation": NotRequired[TableOrientationType],
+        "HeaderStyle": NotRequired[TableCellStyleTypeDef],
+        "CellStyle": NotRequired[TableCellStyleTypeDef],
+        "RowAlternateColorOptions": NotRequired[RowAlternateColorOptionsOutputTypeDef],
+    },
+)
 TableOptionsTypeDef = TypedDict(
     "TableOptionsTypeDef",
     {
         "Orientation": NotRequired[TableOrientationType],
         "HeaderStyle": NotRequired[TableCellStyleTypeDef],
         "CellStyle": NotRequired[TableCellStyleTypeDef],
         "RowAlternateColorOptions": NotRequired[RowAlternateColorOptionsTypeDef],
     },
 )
+TotalOptionsOutputTypeDef = TypedDict(
+    "TotalOptionsOutputTypeDef",
+    {
+        "TotalsVisibility": NotRequired[VisibilityType],
+        "Placement": NotRequired[TableTotalsPlacementType],
+        "ScrollStatus": NotRequired[TableTotalsScrollStatusType],
+        "CustomLabel": NotRequired[str],
+        "TotalCellStyle": NotRequired[TableCellStyleTypeDef],
+        "TotalAggregationOptions": NotRequired[List[TotalAggregationOptionTypeDef]],
+    },
+)
 TotalOptionsTypeDef = TypedDict(
     "TotalOptionsTypeDef",
     {
         "TotalsVisibility": NotRequired[VisibilityType],
         "Placement": NotRequired[TableTotalsPlacementType],
         "ScrollStatus": NotRequired[TableTotalsScrollStatusType],
         "CustomLabel": NotRequired[str],
         "TotalCellStyle": NotRequired[TableCellStyleTypeDef],
         "TotalAggregationOptions": NotRequired[Sequence[TotalAggregationOptionTypeDef]],
     },
 )
+GaugeChartArcConditionalFormattingOutputTypeDef = TypedDict(
+    "GaugeChartArcConditionalFormattingOutputTypeDef",
+    {
+        "ForegroundColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+    },
+)
+GaugeChartPrimaryValueConditionalFormattingOutputTypeDef = TypedDict(
+    "GaugeChartPrimaryValueConditionalFormattingOutputTypeDef",
+    {
+        "TextColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+        "Icon": NotRequired[ConditionalFormattingIconTypeDef],
+    },
+)
+KPIActualValueConditionalFormattingOutputTypeDef = TypedDict(
+    "KPIActualValueConditionalFormattingOutputTypeDef",
+    {
+        "TextColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+        "Icon": NotRequired[ConditionalFormattingIconTypeDef],
+    },
+)
+KPIComparisonValueConditionalFormattingOutputTypeDef = TypedDict(
+    "KPIComparisonValueConditionalFormattingOutputTypeDef",
+    {
+        "TextColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+        "Icon": NotRequired[ConditionalFormattingIconTypeDef],
+    },
+)
+KPIPrimaryValueConditionalFormattingOutputTypeDef = TypedDict(
+    "KPIPrimaryValueConditionalFormattingOutputTypeDef",
+    {
+        "TextColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+        "Icon": NotRequired[ConditionalFormattingIconTypeDef],
+    },
+)
+KPIProgressBarConditionalFormattingOutputTypeDef = TypedDict(
+    "KPIProgressBarConditionalFormattingOutputTypeDef",
+    {
+        "ForegroundColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+    },
+)
+ShapeConditionalFormatOutputTypeDef = TypedDict(
+    "ShapeConditionalFormatOutputTypeDef",
+    {
+        "BackgroundColor": ConditionalFormattingColorOutputTypeDef,
+    },
+)
+TableRowConditionalFormattingOutputTypeDef = TypedDict(
+    "TableRowConditionalFormattingOutputTypeDef",
+    {
+        "BackgroundColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+        "TextColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+    },
+)
+TextConditionalFormatOutputTypeDef = TypedDict(
+    "TextConditionalFormatOutputTypeDef",
+    {
+        "BackgroundColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+        "TextColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+        "Icon": NotRequired[ConditionalFormattingIconTypeDef],
+    },
+)
 GaugeChartArcConditionalFormattingTypeDef = TypedDict(
     "GaugeChartArcConditionalFormattingTypeDef",
     {
         "ForegroundColor": NotRequired[ConditionalFormattingColorTypeDef],
     },
 )
 GaugeChartPrimaryValueConditionalFormattingTypeDef = TypedDict(
@@ -9213,14 +11110,20 @@
     "TextConditionalFormatTypeDef",
     {
         "BackgroundColor": NotRequired[ConditionalFormattingColorTypeDef],
         "TextColor": NotRequired[ConditionalFormattingColorTypeDef],
         "Icon": NotRequired[ConditionalFormattingIconTypeDef],
     },
 )
+SheetControlLayoutOutputTypeDef = TypedDict(
+    "SheetControlLayoutOutputTypeDef",
+    {
+        "Configuration": SheetControlLayoutConfigurationOutputTypeDef,
+    },
+)
 SheetControlLayoutTypeDef = TypedDict(
     "SheetControlLayoutTypeDef",
     {
         "Configuration": SheetControlLayoutConfigurationTypeDef,
     },
 )
 DescribeDataSetRefreshPropertiesResponseTypeDef = TypedDict(
@@ -9236,40 +11139,41 @@
     "PutDataSetRefreshPropertiesRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DataSetId": str,
         "DataSetRefreshProperties": DataSetRefreshPropertiesTypeDef,
     },
 )
-CreateThemeRequestRequestTypeDef = TypedDict(
-    "CreateThemeRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "ThemeId": str,
-        "Name": str,
-        "BaseThemeId": str,
-        "Configuration": ThemeConfigurationTypeDef,
-        "VersionDescription": NotRequired[str],
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 ThemeVersionTypeDef = TypedDict(
     "ThemeVersionTypeDef",
     {
         "VersionNumber": NotRequired[int],
         "Arn": NotRequired[str],
         "Description": NotRequired[str],
         "BaseThemeId": NotRequired[str],
         "CreatedTime": NotRequired[datetime],
-        "Configuration": NotRequired[ThemeConfigurationTypeDef],
+        "Configuration": NotRequired[ThemeConfigurationOutputTypeDef],
         "Errors": NotRequired[List[ThemeErrorTypeDef]],
         "Status": NotRequired[ResourceStatusType],
     },
 )
+CreateThemeRequestRequestTypeDef = TypedDict(
+    "CreateThemeRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "ThemeId": str,
+        "Name": str,
+        "BaseThemeId": str,
+        "Configuration": ThemeConfigurationTypeDef,
+        "VersionDescription": NotRequired[str],
+        "Permissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+ThemeConfigurationUnionTypeDef = Union[ThemeConfigurationTypeDef, ThemeConfigurationOutputTypeDef]
 UpdateThemeRequestRequestTypeDef = TypedDict(
     "UpdateThemeRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "ThemeId": str,
         "BaseThemeId": str,
         "Name": NotRequired[str],
@@ -9315,14 +11219,22 @@
 FieldSortOptionsTypeDef = TypedDict(
     "FieldSortOptionsTypeDef",
     {
         "FieldSort": NotRequired[FieldSortTypeDef],
         "ColumnSort": NotRequired[ColumnSortTypeDef],
     },
 )
+PivotTableSortByOutputTypeDef = TypedDict(
+    "PivotTableSortByOutputTypeDef",
+    {
+        "Field": NotRequired[FieldSortTypeDef],
+        "Column": NotRequired[ColumnSortTypeDef],
+        "DataPath": NotRequired[DataPathSortOutputTypeDef],
+    },
+)
 PivotTableSortByTypeDef = TypedDict(
     "PivotTableSortByTypeDef",
     {
         "Field": NotRequired[FieldSortTypeDef],
         "Column": NotRequired[ColumnSortTypeDef],
         "DataPath": NotRequired[DataPathSortTypeDef],
     },
@@ -9339,81 +11251,107 @@
     {
         "StaticConfiguration": NotRequired[ReferenceLineStaticDataConfigurationTypeDef],
         "DynamicConfiguration": NotRequired[ReferenceLineDynamicDataConfigurationTypeDef],
         "AxisBinding": NotRequired[AxisBindingType],
         "SeriesType": NotRequired[ReferenceLineSeriesTypeType],
     },
 )
+DatasetMetadataOutputTypeDef = TypedDict(
+    "DatasetMetadataOutputTypeDef",
+    {
+        "DatasetArn": str,
+        "DatasetName": NotRequired[str],
+        "DatasetDescription": NotRequired[str],
+        "DataAggregation": NotRequired[DataAggregationTypeDef],
+        "Filters": NotRequired[List[TopicFilterOutputTypeDef]],
+        "Columns": NotRequired[List[TopicColumnOutputTypeDef]],
+        "CalculatedFields": NotRequired[List[TopicCalculatedFieldOutputTypeDef]],
+        "NamedEntities": NotRequired[List[TopicNamedEntityOutputTypeDef]],
+    },
+)
 DatasetMetadataTypeDef = TypedDict(
     "DatasetMetadataTypeDef",
     {
         "DatasetArn": str,
         "DatasetName": NotRequired[str],
         "DatasetDescription": NotRequired[str],
         "DataAggregation": NotRequired[DataAggregationTypeDef],
         "Filters": NotRequired[Sequence[TopicFilterTypeDef]],
         "Columns": NotRequired[Sequence[TopicColumnTypeDef]],
         "CalculatedFields": NotRequired[Sequence[TopicCalculatedFieldTypeDef]],
         "NamedEntities": NotRequired[Sequence[TopicNamedEntityTypeDef]],
     },
 )
-ListDataSourcesResponsePaginatorTypeDef = TypedDict(
-    "ListDataSourcesResponsePaginatorTypeDef",
-    {
-        "DataSources": List[DataSourcePaginatorTypeDef],
-        "NextToken": str,
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-AssetBundleImportJobOverrideParametersTypeDef = TypedDict(
-    "AssetBundleImportJobOverrideParametersTypeDef",
+AssetBundleImportJobOverrideParametersOutputTypeDef = TypedDict(
+    "AssetBundleImportJobOverrideParametersOutputTypeDef",
     {
         "ResourceIdOverrideConfiguration": NotRequired[
             AssetBundleImportJobResourceIdOverrideConfigurationTypeDef
         ],
         "VPCConnections": NotRequired[
-            List[AssetBundleImportJobVPCConnectionOverrideParametersTypeDef]
+            List[AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef]
         ],
         "RefreshSchedules": NotRequired[
-            List[AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef]
+            List[AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef]
+        ],
+        "DataSources": NotRequired[
+            List[AssetBundleImportJobDataSourceOverrideParametersOutputTypeDef]
         ],
-        "DataSources": NotRequired[List[AssetBundleImportJobDataSourceOverrideParametersTypeDef]],
         "DataSets": NotRequired[List[AssetBundleImportJobDataSetOverrideParametersTypeDef]],
         "Themes": NotRequired[List[AssetBundleImportJobThemeOverrideParametersTypeDef]],
         "Analyses": NotRequired[List[AssetBundleImportJobAnalysisOverrideParametersTypeDef]],
         "Dashboards": NotRequired[List[AssetBundleImportJobDashboardOverrideParametersTypeDef]],
     },
 )
-DataSourceCredentialsTypeDef = TypedDict(
-    "DataSourceCredentialsTypeDef",
-    {
-        "CredentialPair": NotRequired[CredentialPairTypeDef],
-        "CopySourceArn": NotRequired[str],
-        "SecretArn": NotRequired[str],
-    },
-)
 DescribeDataSourceResponseTypeDef = TypedDict(
     "DescribeDataSourceResponseTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListDataSourcesResponseTypeDef = TypedDict(
     "ListDataSourcesResponseTypeDef",
     {
         "DataSources": List[DataSourceTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+AssetBundleImportJobOverrideParametersTypeDef = TypedDict(
+    "AssetBundleImportJobOverrideParametersTypeDef",
+    {
+        "ResourceIdOverrideConfiguration": NotRequired[
+            AssetBundleImportJobResourceIdOverrideConfigurationTypeDef
+        ],
+        "VPCConnections": NotRequired[
+            Sequence[AssetBundleImportJobVPCConnectionOverrideParametersTypeDef]
+        ],
+        "RefreshSchedules": NotRequired[
+            Sequence[AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef]
+        ],
+        "DataSources": NotRequired[
+            Sequence[AssetBundleImportJobDataSourceOverrideParametersTypeDef]
+        ],
+        "DataSets": NotRequired[Sequence[AssetBundleImportJobDataSetOverrideParametersTypeDef]],
+        "Themes": NotRequired[Sequence[AssetBundleImportJobThemeOverrideParametersTypeDef]],
+        "Analyses": NotRequired[Sequence[AssetBundleImportJobAnalysisOverrideParametersTypeDef]],
+        "Dashboards": NotRequired[Sequence[AssetBundleImportJobDashboardOverrideParametersTypeDef]],
+    },
+)
+DataSourceCredentialsTypeDef = TypedDict(
+    "DataSourceCredentialsTypeDef",
+    {
+        "CredentialPair": NotRequired[CredentialPairTypeDef],
+        "CopySourceArn": NotRequired[str],
+        "SecretArn": NotRequired[str],
     },
 )
 GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef = TypedDict(
     "GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "UserArn": str,
@@ -9430,161 +11368,180 @@
 )
 DefaultPaginatedLayoutConfigurationTypeDef = TypedDict(
     "DefaultPaginatedLayoutConfigurationTypeDef",
     {
         "SectionBased": NotRequired[DefaultSectionBasedLayoutConfigurationTypeDef],
     },
 )
+SectionLayoutConfigurationOutputTypeDef = TypedDict(
+    "SectionLayoutConfigurationOutputTypeDef",
+    {
+        "FreeFormLayout": FreeFormSectionLayoutConfigurationOutputTypeDef,
+    },
+)
 SectionLayoutConfigurationTypeDef = TypedDict(
     "SectionLayoutConfigurationTypeDef",
     {
         "FreeFormLayout": FreeFormSectionLayoutConfigurationTypeDef,
     },
 )
 DescribeDashboardSnapshotJobResponseTypeDef = TypedDict(
     "DescribeDashboardSnapshotJobResponseTypeDef",
     {
         "AwsAccountId": str,
         "DashboardId": str,
         "SnapshotJobId": str,
         "UserConfiguration": SnapshotUserConfigurationRedactedTypeDef,
-        "SnapshotConfiguration": SnapshotConfigurationTypeDef,
+        "SnapshotConfiguration": SnapshotConfigurationOutputTypeDef,
         "Arn": str,
         "JobStatus": SnapshotJobStatusType,
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SnapshotConfigurationUnionTypeDef = Union[
+    SnapshotConfigurationTypeDef, SnapshotConfigurationOutputTypeDef
+]
 StartDashboardSnapshotJobRequestRequestTypeDef = TypedDict(
     "StartDashboardSnapshotJobRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DashboardId": str,
         "SnapshotJobId": str,
         "UserConfiguration": SnapshotUserConfigurationTypeDef,
         "SnapshotConfiguration": SnapshotConfigurationTypeDef,
     },
 )
-DescribeTemplateResponseTypeDef = TypedDict(
-    "DescribeTemplateResponseTypeDef",
-    {
-        "Template": TemplateTypeDef,
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CustomActionSetParametersOperationTypeDef = TypedDict(
     "CustomActionSetParametersOperationTypeDef",
     {
         "ParameterValueConfigurations": Sequence[SetParameterValueConfigurationTypeDef],
     },
 )
-CreateDataSetRequestRequestTypeDef = TypedDict(
-    "CreateDataSetRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DataSetId": str,
-        "Name": str,
-        "PhysicalTableMap": Mapping[str, PhysicalTableTypeDef],
-        "ImportMode": DataSetImportModeType,
-        "LogicalTableMap": NotRequired[Mapping[str, LogicalTableTypeDef]],
-        "ColumnGroups": NotRequired[Sequence[ColumnGroupTypeDef]],
-        "FieldFolders": NotRequired[Mapping[str, FieldFolderTypeDef]],
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RowLevelPermissionDataSet": NotRequired[RowLevelPermissionDataSetTypeDef],
-        "RowLevelPermissionTagConfiguration": NotRequired[
-            RowLevelPermissionTagConfigurationTypeDef
-        ],
-        "ColumnLevelPermissionRules": NotRequired[Sequence[ColumnLevelPermissionRuleTypeDef]],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "DataSetUsageConfiguration": NotRequired[DataSetUsageConfigurationTypeDef],
-        "DatasetParameters": NotRequired[Sequence[DatasetParameterTypeDef]],
-        "FolderArns": NotRequired[Sequence[str]],
-    },
-)
 DataSetTypeDef = TypedDict(
     "DataSetTypeDef",
     {
         "Arn": NotRequired[str],
         "DataSetId": NotRequired[str],
         "Name": NotRequired[str],
         "CreatedTime": NotRequired[datetime],
         "LastUpdatedTime": NotRequired[datetime],
-        "PhysicalTableMap": NotRequired[Dict[str, PhysicalTableTypeDef]],
-        "LogicalTableMap": NotRequired[Dict[str, LogicalTableTypeDef]],
+        "PhysicalTableMap": NotRequired[Dict[str, PhysicalTableOutputTypeDef]],
+        "LogicalTableMap": NotRequired[Dict[str, LogicalTableOutputTypeDef]],
         "OutputColumns": NotRequired[List[OutputColumnTypeDef]],
         "ImportMode": NotRequired[DataSetImportModeType],
         "ConsumedSpiceCapacityInBytes": NotRequired[int],
-        "ColumnGroups": NotRequired[List[ColumnGroupTypeDef]],
-        "FieldFolders": NotRequired[Dict[str, FieldFolderTypeDef]],
+        "ColumnGroups": NotRequired[List[ColumnGroupOutputTypeDef]],
+        "FieldFolders": NotRequired[Dict[str, FieldFolderOutputTypeDef]],
         "RowLevelPermissionDataSet": NotRequired[RowLevelPermissionDataSetTypeDef],
         "RowLevelPermissionTagConfiguration": NotRequired[
-            RowLevelPermissionTagConfigurationTypeDef
+            RowLevelPermissionTagConfigurationOutputTypeDef
         ],
-        "ColumnLevelPermissionRules": NotRequired[List[ColumnLevelPermissionRuleTypeDef]],
+        "ColumnLevelPermissionRules": NotRequired[List[ColumnLevelPermissionRuleOutputTypeDef]],
         "DataSetUsageConfiguration": NotRequired[DataSetUsageConfigurationTypeDef],
-        "DatasetParameters": NotRequired[List[DatasetParameterTypeDef]],
+        "DatasetParameters": NotRequired[List[DatasetParameterOutputTypeDef]],
     },
 )
-UpdateDataSetRequestRequestTypeDef = TypedDict(
-    "UpdateDataSetRequestRequestTypeDef",
+LogicalTableUnionTypeDef = Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]
+DescribeTemplateResponseTypeDef = TypedDict(
+    "DescribeTemplateResponseTypeDef",
     {
-        "AwsAccountId": str,
-        "DataSetId": str,
-        "Name": str,
-        "PhysicalTableMap": Mapping[str, PhysicalTableTypeDef],
-        "ImportMode": DataSetImportModeType,
-        "LogicalTableMap": NotRequired[Mapping[str, LogicalTableTypeDef]],
-        "ColumnGroups": NotRequired[Sequence[ColumnGroupTypeDef]],
-        "FieldFolders": NotRequired[Mapping[str, FieldFolderTypeDef]],
-        "RowLevelPermissionDataSet": NotRequired[RowLevelPermissionDataSetTypeDef],
-        "RowLevelPermissionTagConfiguration": NotRequired[
-            RowLevelPermissionTagConfigurationTypeDef
-        ],
-        "ColumnLevelPermissionRules": NotRequired[Sequence[ColumnLevelPermissionRuleTypeDef]],
-        "DataSetUsageConfiguration": NotRequired[DataSetUsageConfigurationTypeDef],
-        "DatasetParameters": NotRequired[Sequence[DatasetParameterTypeDef]],
+        "Template": TemplateTypeDef,
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+VisualCustomActionOperationOutputTypeDef = TypedDict(
+    "VisualCustomActionOperationOutputTypeDef",
+    {
+        "FilterOperation": NotRequired[CustomActionFilterOperationOutputTypeDef],
+        "NavigationOperation": NotRequired[CustomActionNavigationOperationTypeDef],
+        "URLOperation": NotRequired[CustomActionURLOperationTypeDef],
+        "SetParametersOperation": NotRequired[CustomActionSetParametersOperationOutputTypeDef],
+    },
+)
+LineSeriesAxisDisplayOptionsOutputTypeDef = TypedDict(
+    "LineSeriesAxisDisplayOptionsOutputTypeDef",
+    {
+        "AxisOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "MissingDataConfigurations": NotRequired[List[MissingDataConfigurationTypeDef]],
     },
 )
 LineSeriesAxisDisplayOptionsTypeDef = TypedDict(
     "LineSeriesAxisDisplayOptionsTypeDef",
     {
         "AxisOptions": NotRequired[AxisDisplayOptionsTypeDef],
         "MissingDataConfigurations": NotRequired[Sequence[MissingDataConfigurationTypeDef]],
     },
 )
+DefaultFilterControlOptionsOutputTypeDef = TypedDict(
+    "DefaultFilterControlOptionsOutputTypeDef",
+    {
+        "DefaultDateTimePickerOptions": NotRequired[DefaultDateTimePickerControlOptionsTypeDef],
+        "DefaultListOptions": NotRequired[DefaultFilterListControlOptionsOutputTypeDef],
+        "DefaultDropdownOptions": NotRequired[DefaultFilterDropDownControlOptionsOutputTypeDef],
+        "DefaultTextFieldOptions": NotRequired[DefaultTextFieldControlOptionsTypeDef],
+        "DefaultTextAreaOptions": NotRequired[DefaultTextAreaControlOptionsTypeDef],
+        "DefaultSliderOptions": NotRequired[DefaultSliderControlOptionsTypeDef],
+        "DefaultRelativeDateTimeOptions": NotRequired[DefaultRelativeDateTimeControlOptionsTypeDef],
+    },
+)
 DefaultFilterControlOptionsTypeDef = TypedDict(
     "DefaultFilterControlOptionsTypeDef",
     {
         "DefaultDateTimePickerOptions": NotRequired[DefaultDateTimePickerControlOptionsTypeDef],
         "DefaultListOptions": NotRequired[DefaultFilterListControlOptionsTypeDef],
         "DefaultDropdownOptions": NotRequired[DefaultFilterDropDownControlOptionsTypeDef],
         "DefaultTextFieldOptions": NotRequired[DefaultTextFieldControlOptionsTypeDef],
         "DefaultTextAreaOptions": NotRequired[DefaultTextAreaControlOptionsTypeDef],
         "DefaultSliderOptions": NotRequired[DefaultSliderControlOptionsTypeDef],
         "DefaultRelativeDateTimeOptions": NotRequired[DefaultRelativeDateTimeControlOptionsTypeDef],
     },
 )
+FilterControlOutputTypeDef = TypedDict(
+    "FilterControlOutputTypeDef",
+    {
+        "DateTimePicker": NotRequired[FilterDateTimePickerControlTypeDef],
+        "List": NotRequired[FilterListControlOutputTypeDef],
+        "Dropdown": NotRequired[FilterDropDownControlOutputTypeDef],
+        "TextField": NotRequired[FilterTextFieldControlTypeDef],
+        "TextArea": NotRequired[FilterTextAreaControlTypeDef],
+        "Slider": NotRequired[FilterSliderControlTypeDef],
+        "RelativeDateTime": NotRequired[FilterRelativeDateTimeControlTypeDef],
+        "CrossSheet": NotRequired[FilterCrossSheetControlOutputTypeDef],
+    },
+)
 FilterControlTypeDef = TypedDict(
     "FilterControlTypeDef",
     {
         "DateTimePicker": NotRequired[FilterDateTimePickerControlTypeDef],
         "List": NotRequired[FilterListControlTypeDef],
         "Dropdown": NotRequired[FilterDropDownControlTypeDef],
         "TextField": NotRequired[FilterTextFieldControlTypeDef],
         "TextArea": NotRequired[FilterTextAreaControlTypeDef],
         "Slider": NotRequired[FilterSliderControlTypeDef],
         "RelativeDateTime": NotRequired[FilterRelativeDateTimeControlTypeDef],
         "CrossSheet": NotRequired[FilterCrossSheetControlTypeDef],
     },
 )
+ParameterControlOutputTypeDef = TypedDict(
+    "ParameterControlOutputTypeDef",
+    {
+        "DateTimePicker": NotRequired[ParameterDateTimePickerControlTypeDef],
+        "List": NotRequired[ParameterListControlOutputTypeDef],
+        "Dropdown": NotRequired[ParameterDropDownControlOutputTypeDef],
+        "TextField": NotRequired[ParameterTextFieldControlTypeDef],
+        "TextArea": NotRequired[ParameterTextAreaControlTypeDef],
+        "Slider": NotRequired[ParameterSliderControlTypeDef],
+    },
+)
 ParameterControlTypeDef = TypedDict(
     "ParameterControlTypeDef",
     {
         "DateTimePicker": NotRequired[ParameterDateTimePickerControlTypeDef],
         "List": NotRequired[ParameterListControlTypeDef],
         "Dropdown": NotRequired[ParameterDropDownControlTypeDef],
         "TextField": NotRequired[ParameterTextFieldControlTypeDef],
@@ -9595,23 +11552,71 @@
 TableFieldURLConfigurationTypeDef = TypedDict(
     "TableFieldURLConfigurationTypeDef",
     {
         "LinkConfiguration": NotRequired[TableFieldLinkConfigurationTypeDef],
         "ImageConfiguration": NotRequired[TableFieldImageConfigurationTypeDef],
     },
 )
+PivotTableTotalOptionsOutputTypeDef = TypedDict(
+    "PivotTableTotalOptionsOutputTypeDef",
+    {
+        "RowSubtotalOptions": NotRequired[SubtotalOptionsOutputTypeDef],
+        "ColumnSubtotalOptions": NotRequired[SubtotalOptionsOutputTypeDef],
+        "RowTotalOptions": NotRequired[PivotTotalOptionsOutputTypeDef],
+        "ColumnTotalOptions": NotRequired[PivotTotalOptionsOutputTypeDef],
+    },
+)
 PivotTableTotalOptionsTypeDef = TypedDict(
     "PivotTableTotalOptionsTypeDef",
     {
         "RowSubtotalOptions": NotRequired[SubtotalOptionsTypeDef],
         "ColumnSubtotalOptions": NotRequired[SubtotalOptionsTypeDef],
         "RowTotalOptions": NotRequired[PivotTotalOptionsTypeDef],
         "ColumnTotalOptions": NotRequired[PivotTotalOptionsTypeDef],
     },
 )
+GaugeChartConditionalFormattingOptionOutputTypeDef = TypedDict(
+    "GaugeChartConditionalFormattingOptionOutputTypeDef",
+    {
+        "PrimaryValue": NotRequired[GaugeChartPrimaryValueConditionalFormattingOutputTypeDef],
+        "Arc": NotRequired[GaugeChartArcConditionalFormattingOutputTypeDef],
+    },
+)
+KPIConditionalFormattingOptionOutputTypeDef = TypedDict(
+    "KPIConditionalFormattingOptionOutputTypeDef",
+    {
+        "PrimaryValue": NotRequired[KPIPrimaryValueConditionalFormattingOutputTypeDef],
+        "ProgressBar": NotRequired[KPIProgressBarConditionalFormattingOutputTypeDef],
+        "ActualValue": NotRequired[KPIActualValueConditionalFormattingOutputTypeDef],
+        "ComparisonValue": NotRequired[KPIComparisonValueConditionalFormattingOutputTypeDef],
+    },
+)
+FilledMapShapeConditionalFormattingOutputTypeDef = TypedDict(
+    "FilledMapShapeConditionalFormattingOutputTypeDef",
+    {
+        "FieldId": str,
+        "Format": NotRequired[ShapeConditionalFormatOutputTypeDef],
+    },
+)
+PivotTableCellConditionalFormattingOutputTypeDef = TypedDict(
+    "PivotTableCellConditionalFormattingOutputTypeDef",
+    {
+        "FieldId": str,
+        "TextFormat": NotRequired[TextConditionalFormatOutputTypeDef],
+        "Scope": NotRequired[PivotTableConditionalFormattingScopeTypeDef],
+        "Scopes": NotRequired[List[PivotTableConditionalFormattingScopeTypeDef]],
+    },
+)
+TableCellConditionalFormattingOutputTypeDef = TypedDict(
+    "TableCellConditionalFormattingOutputTypeDef",
+    {
+        "FieldId": str,
+        "TextFormat": NotRequired[TextConditionalFormatOutputTypeDef],
+    },
+)
 GaugeChartConditionalFormattingOptionTypeDef = TypedDict(
     "GaugeChartConditionalFormattingOptionTypeDef",
     {
         "PrimaryValue": NotRequired[GaugeChartPrimaryValueConditionalFormattingTypeDef],
         "Arc": NotRequired[GaugeChartArcConditionalFormattingTypeDef],
     },
 )
@@ -9753,148 +11758,291 @@
     "FormatConfigurationTypeDef",
     {
         "StringFormatConfiguration": NotRequired[StringFormatConfigurationTypeDef],
         "NumberFormatConfiguration": NotRequired[NumberFormatConfigurationTypeDef],
         "DateTimeFormatConfiguration": NotRequired[DateTimeFormatConfigurationTypeDef],
     },
 )
+BarChartSortConfigurationOutputTypeDef = TypedDict(
+    "BarChartSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+        "ColorSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "ColorItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+        "SmallMultiplesSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "SmallMultiplesLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 BarChartSortConfigurationTypeDef = TypedDict(
     "BarChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "ColorSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "ColorItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "SmallMultiplesSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "SmallMultiplesLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+BoxPlotSortConfigurationOutputTypeDef = TypedDict(
+    "BoxPlotSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "PaginationConfiguration": NotRequired[PaginationConfigurationTypeDef],
+    },
+)
 BoxPlotSortConfigurationTypeDef = TypedDict(
     "BoxPlotSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "PaginationConfiguration": NotRequired[PaginationConfigurationTypeDef],
     },
 )
+ComboChartSortConfigurationOutputTypeDef = TypedDict(
+    "ComboChartSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+        "ColorSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "ColorItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 ComboChartSortConfigurationTypeDef = TypedDict(
     "ComboChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "ColorSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "ColorItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+FilledMapSortConfigurationOutputTypeDef = TypedDict(
+    "FilledMapSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+    },
+)
 FilledMapSortConfigurationTypeDef = TypedDict(
     "FilledMapSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
     },
 )
+FunnelChartSortConfigurationOutputTypeDef = TypedDict(
+    "FunnelChartSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 FunnelChartSortConfigurationTypeDef = TypedDict(
     "FunnelChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+HeatMapSortConfigurationOutputTypeDef = TypedDict(
+    "HeatMapSortConfigurationOutputTypeDef",
+    {
+        "HeatMapRowSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "HeatMapColumnSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "HeatMapRowItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+        "HeatMapColumnItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 HeatMapSortConfigurationTypeDef = TypedDict(
     "HeatMapSortConfigurationTypeDef",
     {
         "HeatMapRowSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "HeatMapColumnSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "HeatMapRowItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
         "HeatMapColumnItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+KPISortConfigurationOutputTypeDef = TypedDict(
+    "KPISortConfigurationOutputTypeDef",
+    {
+        "TrendGroupSort": NotRequired[List[FieldSortOptionsTypeDef]],
+    },
+)
 KPISortConfigurationTypeDef = TypedDict(
     "KPISortConfigurationTypeDef",
     {
         "TrendGroupSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
     },
 )
+LineChartSortConfigurationOutputTypeDef = TypedDict(
+    "LineChartSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "CategoryItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+        "ColorItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+        "SmallMultiplesSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "SmallMultiplesLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 LineChartSortConfigurationTypeDef = TypedDict(
     "LineChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "CategoryItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
         "ColorItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
         "SmallMultiplesSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "SmallMultiplesLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+PieChartSortConfigurationOutputTypeDef = TypedDict(
+    "PieChartSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+        "SmallMultiplesSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "SmallMultiplesLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 PieChartSortConfigurationTypeDef = TypedDict(
     "PieChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "SmallMultiplesSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "SmallMultiplesLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+RadarChartSortConfigurationOutputTypeDef = TypedDict(
+    "RadarChartSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+        "ColorSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "ColorItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 RadarChartSortConfigurationTypeDef = TypedDict(
     "RadarChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "ColorSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "ColorItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+SankeyDiagramSortConfigurationOutputTypeDef = TypedDict(
+    "SankeyDiagramSortConfigurationOutputTypeDef",
+    {
+        "WeightSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "SourceItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+        "DestinationItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 SankeyDiagramSortConfigurationTypeDef = TypedDict(
     "SankeyDiagramSortConfigurationTypeDef",
     {
         "WeightSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "SourceItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "DestinationItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+TableSortConfigurationOutputTypeDef = TypedDict(
+    "TableSortConfigurationOutputTypeDef",
+    {
+        "RowSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "PaginationConfiguration": NotRequired[PaginationConfigurationTypeDef],
+    },
+)
 TableSortConfigurationTypeDef = TypedDict(
     "TableSortConfigurationTypeDef",
     {
         "RowSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "PaginationConfiguration": NotRequired[PaginationConfigurationTypeDef],
     },
 )
+TreeMapSortConfigurationOutputTypeDef = TypedDict(
+    "TreeMapSortConfigurationOutputTypeDef",
+    {
+        "TreeMapSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "TreeMapGroupItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 TreeMapSortConfigurationTypeDef = TypedDict(
     "TreeMapSortConfigurationTypeDef",
     {
         "TreeMapSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "TreeMapGroupItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+WaterfallChartSortConfigurationOutputTypeDef = TypedDict(
+    "WaterfallChartSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "BreakdownItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 WaterfallChartSortConfigurationTypeDef = TypedDict(
     "WaterfallChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "BreakdownItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+WordCloudSortConfigurationOutputTypeDef = TypedDict(
+    "WordCloudSortConfigurationOutputTypeDef",
+    {
+        "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+    },
+)
 WordCloudSortConfigurationTypeDef = TypedDict(
     "WordCloudSortConfigurationTypeDef",
     {
         "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
     },
 )
+PivotFieldSortOptionsOutputTypeDef = TypedDict(
+    "PivotFieldSortOptionsOutputTypeDef",
+    {
+        "FieldId": str,
+        "SortBy": PivotTableSortByOutputTypeDef,
+    },
+)
 PivotFieldSortOptionsTypeDef = TypedDict(
     "PivotFieldSortOptionsTypeDef",
     {
         "FieldId": str,
         "SortBy": PivotTableSortByTypeDef,
     },
 )
+FieldBasedTooltipOutputTypeDef = TypedDict(
+    "FieldBasedTooltipOutputTypeDef",
+    {
+        "AggregationVisibility": NotRequired[VisibilityType],
+        "TooltipTitleType": NotRequired[TooltipTitleTypeType],
+        "TooltipFields": NotRequired[List[TooltipItemTypeDef]],
+    },
+)
 FieldBasedTooltipTypeDef = TypedDict(
     "FieldBasedTooltipTypeDef",
     {
         "AggregationVisibility": NotRequired[VisibilityType],
         "TooltipTitleType": NotRequired[TooltipTitleTypeType],
         "TooltipFields": NotRequired[Sequence[TooltipItemTypeDef]],
     },
 )
+TopicDetailsOutputTypeDef = TypedDict(
+    "TopicDetailsOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "Description": NotRequired[str],
+        "UserExperienceVersion": NotRequired[TopicUserExperienceVersionType],
+        "DataSets": NotRequired[List[DatasetMetadataOutputTypeDef]],
+    },
+)
 TopicDetailsTypeDef = TypedDict(
     "TopicDetailsTypeDef",
     {
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "UserExperienceVersion": NotRequired[TopicUserExperienceVersionType],
         "DataSets": NotRequired[Sequence[DatasetMetadataTypeDef]],
@@ -9907,25 +12055,29 @@
         "Errors": List[AssetBundleImportJobErrorTypeDef],
         "RollbackErrors": List[AssetBundleImportJobErrorTypeDef],
         "Arn": str,
         "CreatedTime": datetime,
         "AssetBundleImportJobId": str,
         "AwsAccountId": str,
         "AssetBundleImportSource": AssetBundleImportSourceDescriptionTypeDef,
-        "OverrideParameters": AssetBundleImportJobOverrideParametersTypeDef,
+        "OverrideParameters": AssetBundleImportJobOverrideParametersOutputTypeDef,
         "FailureAction": AssetBundleImportFailureActionType,
         "RequestId": str,
         "Status": int,
-        "OverridePermissions": AssetBundleImportJobOverridePermissionsTypeDef,
-        "OverrideTags": AssetBundleImportJobOverrideTagsTypeDef,
+        "OverridePermissions": AssetBundleImportJobOverridePermissionsOutputTypeDef,
+        "OverrideTags": AssetBundleImportJobOverrideTagsOutputTypeDef,
         "OverrideValidationStrategy": AssetBundleImportJobOverrideValidationStrategyTypeDef,
         "Warnings": List[AssetBundleImportJobWarningTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AssetBundleImportJobOverrideParametersUnionTypeDef = Union[
+    AssetBundleImportJobOverrideParametersTypeDef,
+    AssetBundleImportJobOverrideParametersOutputTypeDef,
+]
 StartAssetBundleImportJobRequestRequestTypeDef = TypedDict(
     "StartAssetBundleImportJobRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AssetBundleImportJobId": str,
         "AssetBundleImportSource": AssetBundleImportSourceTypeDef,
         "OverrideParameters": NotRequired[AssetBundleImportJobOverrideParametersTypeDef],
@@ -9942,15 +12094,15 @@
     {
         "AwsAccountId": str,
         "DataSourceId": str,
         "Name": str,
         "Type": DataSourceTypeType,
         "DataSourceParameters": NotRequired[DataSourceParametersTypeDef],
         "Credentials": NotRequired[DataSourceCredentialsTypeDef],
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
+        "Permissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
         "VpcConnectionProperties": NotRequired[VpcConnectionPropertiesTypeDef],
         "SslProperties": NotRequired[SslPropertiesTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "FolderArns": NotRequired[Sequence[str]],
     },
 )
 UpdateDataSourceRequestRequestTypeDef = TypedDict(
@@ -9975,14 +12127,28 @@
     "DefaultNewSheetConfigurationTypeDef",
     {
         "InteractiveLayoutConfiguration": NotRequired[DefaultInteractiveLayoutConfigurationTypeDef],
         "PaginatedLayoutConfiguration": NotRequired[DefaultPaginatedLayoutConfigurationTypeDef],
         "SheetContentType": NotRequired[SheetContentTypeType],
     },
 )
+BodySectionContentOutputTypeDef = TypedDict(
+    "BodySectionContentOutputTypeDef",
+    {
+        "Layout": NotRequired[SectionLayoutConfigurationOutputTypeDef],
+    },
+)
+HeaderFooterSectionConfigurationOutputTypeDef = TypedDict(
+    "HeaderFooterSectionConfigurationOutputTypeDef",
+    {
+        "SectionId": str,
+        "Layout": SectionLayoutConfigurationOutputTypeDef,
+        "Style": NotRequired[SectionStyleTypeDef],
+    },
+)
 BodySectionContentTypeDef = TypedDict(
     "BodySectionContentTypeDef",
     {
         "Layout": NotRequired[SectionLayoutConfigurationTypeDef],
     },
 )
 HeaderFooterSectionConfigurationTypeDef = TypedDict(
@@ -10007,14 +12173,74 @@
     {
         "DataSet": DataSetTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateDataSetRequestRequestTypeDef = TypedDict(
+    "CreateDataSetRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DataSetId": str,
+        "Name": str,
+        "PhysicalTableMap": Mapping[str, PhysicalTableUnionTypeDef],
+        "ImportMode": DataSetImportModeType,
+        "LogicalTableMap": NotRequired[Mapping[str, LogicalTableUnionTypeDef]],
+        "ColumnGroups": NotRequired[Sequence[ColumnGroupUnionTypeDef]],
+        "FieldFolders": NotRequired[Mapping[str, FieldFolderUnionTypeDef]],
+        "Permissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RowLevelPermissionDataSet": NotRequired[RowLevelPermissionDataSetTypeDef],
+        "RowLevelPermissionTagConfiguration": NotRequired[
+            RowLevelPermissionTagConfigurationTypeDef
+        ],
+        "ColumnLevelPermissionRules": NotRequired[Sequence[ColumnLevelPermissionRuleUnionTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "DataSetUsageConfiguration": NotRequired[DataSetUsageConfigurationTypeDef],
+        "DatasetParameters": NotRequired[Sequence[DatasetParameterUnionTypeDef]],
+        "FolderArns": NotRequired[Sequence[str]],
+    },
+)
+UpdateDataSetRequestRequestTypeDef = TypedDict(
+    "UpdateDataSetRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DataSetId": str,
+        "Name": str,
+        "PhysicalTableMap": Mapping[str, PhysicalTableUnionTypeDef],
+        "ImportMode": DataSetImportModeType,
+        "LogicalTableMap": NotRequired[Mapping[str, LogicalTableUnionTypeDef]],
+        "ColumnGroups": NotRequired[Sequence[ColumnGroupUnionTypeDef]],
+        "FieldFolders": NotRequired[Mapping[str, FieldFolderUnionTypeDef]],
+        "RowLevelPermissionDataSet": NotRequired[RowLevelPermissionDataSetTypeDef],
+        "RowLevelPermissionTagConfiguration": NotRequired[
+            RowLevelPermissionTagConfigurationTypeDef
+        ],
+        "ColumnLevelPermissionRules": NotRequired[Sequence[ColumnLevelPermissionRuleUnionTypeDef]],
+        "DataSetUsageConfiguration": NotRequired[DataSetUsageConfigurationTypeDef],
+        "DatasetParameters": NotRequired[Sequence[DatasetParameterUnionTypeDef]],
+    },
+)
+VisualCustomActionOutputTypeDef = TypedDict(
+    "VisualCustomActionOutputTypeDef",
+    {
+        "CustomActionId": str,
+        "Name": str,
+        "Trigger": VisualCustomActionTriggerType,
+        "ActionOperations": List[VisualCustomActionOperationOutputTypeDef],
+        "Status": NotRequired[WidgetStatusType],
+    },
+)
+DefaultFilterControlConfigurationOutputTypeDef = TypedDict(
+    "DefaultFilterControlConfigurationOutputTypeDef",
+    {
+        "Title": str,
+        "ControlOptions": DefaultFilterControlOptionsOutputTypeDef,
+    },
+)
 DefaultFilterControlConfigurationTypeDef = TypedDict(
     "DefaultFilterControlConfigurationTypeDef",
     {
         "Title": str,
         "ControlOptions": DefaultFilterControlOptionsTypeDef,
     },
 )
@@ -10024,14 +12250,49 @@
         "FieldId": str,
         "Width": NotRequired[str],
         "CustomLabel": NotRequired[str],
         "Visibility": NotRequired[VisibilityType],
         "URLStyling": NotRequired[TableFieldURLConfigurationTypeDef],
     },
 )
+GaugeChartConditionalFormattingOutputTypeDef = TypedDict(
+    "GaugeChartConditionalFormattingOutputTypeDef",
+    {
+        "ConditionalFormattingOptions": NotRequired[
+            List[GaugeChartConditionalFormattingOptionOutputTypeDef]
+        ],
+    },
+)
+KPIConditionalFormattingOutputTypeDef = TypedDict(
+    "KPIConditionalFormattingOutputTypeDef",
+    {
+        "ConditionalFormattingOptions": NotRequired[
+            List[KPIConditionalFormattingOptionOutputTypeDef]
+        ],
+    },
+)
+FilledMapConditionalFormattingOptionOutputTypeDef = TypedDict(
+    "FilledMapConditionalFormattingOptionOutputTypeDef",
+    {
+        "Shape": FilledMapShapeConditionalFormattingOutputTypeDef,
+    },
+)
+PivotTableConditionalFormattingOptionOutputTypeDef = TypedDict(
+    "PivotTableConditionalFormattingOptionOutputTypeDef",
+    {
+        "Cell": NotRequired[PivotTableCellConditionalFormattingOutputTypeDef],
+    },
+)
+TableConditionalFormattingOptionOutputTypeDef = TypedDict(
+    "TableConditionalFormattingOptionOutputTypeDef",
+    {
+        "Cell": NotRequired[TableCellConditionalFormattingOutputTypeDef],
+        "Row": NotRequired[TableRowConditionalFormattingOutputTypeDef],
+    },
+)
 GaugeChartConditionalFormattingTypeDef = TypedDict(
     "GaugeChartConditionalFormattingTypeDef",
     {
         "ConditionalFormattingOptions": NotRequired[
             Sequence[GaugeChartConditionalFormattingOptionTypeDef]
         ],
     },
@@ -10094,14 +12355,23 @@
     {
         "NumericalMeasureField": NotRequired[NumericalMeasureFieldTypeDef],
         "CategoricalMeasureField": NotRequired[CategoricalMeasureFieldTypeDef],
         "DateMeasureField": NotRequired[DateMeasureFieldTypeDef],
         "CalculatedMeasureField": NotRequired[CalculatedMeasureFieldTypeDef],
     },
 )
+ColumnConfigurationOutputTypeDef = TypedDict(
+    "ColumnConfigurationOutputTypeDef",
+    {
+        "Column": ColumnIdentifierTypeDef,
+        "FormatConfiguration": NotRequired[FormatConfigurationTypeDef],
+        "Role": NotRequired[ColumnRoleType],
+        "ColorsConfiguration": NotRequired[ColorsConfigurationOutputTypeDef],
+    },
+)
 ColumnConfigurationTypeDef = TypedDict(
     "ColumnConfigurationTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "FormatConfiguration": NotRequired[FormatConfigurationTypeDef],
         "Role": NotRequired[ColumnRoleType],
         "ColorsConfiguration": NotRequired[ColorsConfigurationTypeDef],
@@ -10111,48 +12381,63 @@
     "UnaggregatedFieldTypeDef",
     {
         "FieldId": str,
         "Column": ColumnIdentifierTypeDef,
         "FormatConfiguration": NotRequired[FormatConfigurationTypeDef],
     },
 )
+PivotTableSortConfigurationOutputTypeDef = TypedDict(
+    "PivotTableSortConfigurationOutputTypeDef",
+    {
+        "FieldSortOptions": NotRequired[List[PivotFieldSortOptionsOutputTypeDef]],
+    },
+)
 PivotTableSortConfigurationTypeDef = TypedDict(
     "PivotTableSortConfigurationTypeDef",
     {
         "FieldSortOptions": NotRequired[Sequence[PivotFieldSortOptionsTypeDef]],
     },
 )
-TooltipOptionsTypeDef = TypedDict(
-    "TooltipOptionsTypeDef",
+TooltipOptionsOutputTypeDef = TypedDict(
+    "TooltipOptionsOutputTypeDef",
     {
         "TooltipVisibility": NotRequired[VisibilityType],
         "SelectedTooltipType": NotRequired[SelectedTooltipTypeType],
-        "FieldBasedTooltip": NotRequired[FieldBasedTooltipTypeDef],
+        "FieldBasedTooltip": NotRequired[FieldBasedTooltipOutputTypeDef],
     },
 )
-CreateTopicRequestRequestTypeDef = TypedDict(
-    "CreateTopicRequestRequestTypeDef",
+TooltipOptionsTypeDef = TypedDict(
+    "TooltipOptionsTypeDef",
     {
-        "AwsAccountId": str,
-        "TopicId": str,
-        "Topic": TopicDetailsTypeDef,
-        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "TooltipVisibility": NotRequired[VisibilityType],
+        "SelectedTooltipType": NotRequired[SelectedTooltipTypeType],
+        "FieldBasedTooltip": NotRequired[FieldBasedTooltipTypeDef],
     },
 )
 DescribeTopicResponseTypeDef = TypedDict(
     "DescribeTopicResponseTypeDef",
     {
         "Arn": str,
         "TopicId": str,
-        "Topic": TopicDetailsTypeDef,
+        "Topic": TopicDetailsOutputTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateTopicRequestRequestTypeDef = TypedDict(
+    "CreateTopicRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "TopicId": str,
+        "Topic": TopicDetailsTypeDef,
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+TopicDetailsUnionTypeDef = Union[TopicDetailsTypeDef, TopicDetailsOutputTypeDef]
 UpdateTopicRequestRequestTypeDef = TypedDict(
     "UpdateTopicRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TopicId": str,
         "Topic": TopicDetailsTypeDef,
     },
@@ -10173,14 +12458,23 @@
 )
 AnalysisDefaultsTypeDef = TypedDict(
     "AnalysisDefaultsTypeDef",
     {
         "DefaultNewSheetConfiguration": DefaultNewSheetConfigurationTypeDef,
     },
 )
+BodySectionConfigurationOutputTypeDef = TypedDict(
+    "BodySectionConfigurationOutputTypeDef",
+    {
+        "SectionId": str,
+        "Content": BodySectionContentOutputTypeDef,
+        "Style": NotRequired[SectionStyleTypeDef],
+        "PageBreakConfiguration": NotRequired[SectionPageBreakConfigurationTypeDef],
+    },
+)
 BodySectionConfigurationTypeDef = TypedDict(
     "BodySectionConfigurationTypeDef",
     {
         "SectionId": str,
         "Content": BodySectionContentTypeDef,
         "Style": NotRequired[SectionStyleTypeDef],
         "PageBreakConfiguration": NotRequired[SectionPageBreakConfigurationTypeDef],
@@ -10192,14 +12486,140 @@
         "CustomActionId": str,
         "Name": str,
         "Trigger": VisualCustomActionTriggerType,
         "ActionOperations": Sequence[VisualCustomActionOperationTypeDef],
         "Status": NotRequired[WidgetStatusType],
     },
 )
+CustomContentVisualOutputTypeDef = TypedDict(
+    "CustomContentVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "DataSetIdentifier": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[CustomContentConfigurationTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
+EmptyVisualOutputTypeDef = TypedDict(
+    "EmptyVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "DataSetIdentifier": str,
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
+CategoryFilterOutputTypeDef = TypedDict(
+    "CategoryFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "Configuration": CategoryFilterConfigurationOutputTypeDef,
+        "DefaultFilterControlConfiguration": NotRequired[
+            DefaultFilterControlConfigurationOutputTypeDef
+        ],
+    },
+)
+NumericEqualityFilterOutputTypeDef = TypedDict(
+    "NumericEqualityFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "MatchOperator": NumericEqualityMatchOperatorType,
+        "NullOption": FilterNullOptionType,
+        "Value": NotRequired[float],
+        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
+        "AggregationFunction": NotRequired[AggregationFunctionTypeDef],
+        "ParameterName": NotRequired[str],
+        "DefaultFilterControlConfiguration": NotRequired[
+            DefaultFilterControlConfigurationOutputTypeDef
+        ],
+    },
+)
+NumericRangeFilterOutputTypeDef = TypedDict(
+    "NumericRangeFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "NullOption": FilterNullOptionType,
+        "IncludeMinimum": NotRequired[bool],
+        "IncludeMaximum": NotRequired[bool],
+        "RangeMinimum": NotRequired[NumericRangeFilterValueTypeDef],
+        "RangeMaximum": NotRequired[NumericRangeFilterValueTypeDef],
+        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
+        "AggregationFunction": NotRequired[AggregationFunctionTypeDef],
+        "DefaultFilterControlConfiguration": NotRequired[
+            DefaultFilterControlConfigurationOutputTypeDef
+        ],
+    },
+)
+RelativeDatesFilterOutputTypeDef = TypedDict(
+    "RelativeDatesFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "AnchorDateConfiguration": AnchorDateConfigurationTypeDef,
+        "TimeGranularity": TimeGranularityType,
+        "RelativeDateType": RelativeDateTypeType,
+        "NullOption": FilterNullOptionType,
+        "MinimumGranularity": NotRequired[TimeGranularityType],
+        "RelativeDateValue": NotRequired[int],
+        "ParameterName": NotRequired[str],
+        "ExcludePeriodConfiguration": NotRequired[ExcludePeriodConfigurationTypeDef],
+        "DefaultFilterControlConfiguration": NotRequired[
+            DefaultFilterControlConfigurationOutputTypeDef
+        ],
+    },
+)
+TimeEqualityFilterOutputTypeDef = TypedDict(
+    "TimeEqualityFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "Value": NotRequired[datetime],
+        "ParameterName": NotRequired[str],
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
+        "DefaultFilterControlConfiguration": NotRequired[
+            DefaultFilterControlConfigurationOutputTypeDef
+        ],
+    },
+)
+TimeRangeFilterOutputTypeDef = TypedDict(
+    "TimeRangeFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "NullOption": FilterNullOptionType,
+        "IncludeMinimum": NotRequired[bool],
+        "IncludeMaximum": NotRequired[bool],
+        "RangeMinimumValue": NotRequired[TimeRangeFilterValueOutputTypeDef],
+        "RangeMaximumValue": NotRequired[TimeRangeFilterValueOutputTypeDef],
+        "ExcludePeriodConfiguration": NotRequired[ExcludePeriodConfigurationTypeDef],
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "DefaultFilterControlConfiguration": NotRequired[
+            DefaultFilterControlConfigurationOutputTypeDef
+        ],
+    },
+)
+TopBottomFilterOutputTypeDef = TypedDict(
+    "TopBottomFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "AggregationSortConfigurations": List[AggregationSortConfigurationTypeDef],
+        "Limit": NotRequired[int],
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "ParameterName": NotRequired[str],
+        "DefaultFilterControlConfiguration": NotRequired[
+            DefaultFilterControlConfigurationOutputTypeDef
+        ],
+    },
+)
 CategoryFilterTypeDef = TypedDict(
     "CategoryFilterTypeDef",
     {
         "FilterId": str,
         "Column": ColumnIdentifierTypeDef,
         "Configuration": CategoryFilterConfigurationTypeDef,
         "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
@@ -10285,22 +12705,52 @@
         "AggregationSortConfigurations": Sequence[AggregationSortConfigurationTypeDef],
         "Limit": NotRequired[int],
         "TimeGranularity": NotRequired[TimeGranularityType],
         "ParameterName": NotRequired[str],
         "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
     },
 )
+TableFieldOptionsOutputTypeDef = TypedDict(
+    "TableFieldOptionsOutputTypeDef",
+    {
+        "SelectedFieldOptions": NotRequired[List[TableFieldOptionTypeDef]],
+        "Order": NotRequired[List[str]],
+        "PinnedFieldOptions": NotRequired[TablePinnedFieldOptionsOutputTypeDef],
+    },
+)
 TableFieldOptionsTypeDef = TypedDict(
     "TableFieldOptionsTypeDef",
     {
         "SelectedFieldOptions": NotRequired[Sequence[TableFieldOptionTypeDef]],
         "Order": NotRequired[Sequence[str]],
         "PinnedFieldOptions": NotRequired[TablePinnedFieldOptionsTypeDef],
     },
 )
+FilledMapConditionalFormattingOutputTypeDef = TypedDict(
+    "FilledMapConditionalFormattingOutputTypeDef",
+    {
+        "ConditionalFormattingOptions": List[FilledMapConditionalFormattingOptionOutputTypeDef],
+    },
+)
+PivotTableConditionalFormattingOutputTypeDef = TypedDict(
+    "PivotTableConditionalFormattingOutputTypeDef",
+    {
+        "ConditionalFormattingOptions": NotRequired[
+            List[PivotTableConditionalFormattingOptionOutputTypeDef]
+        ],
+    },
+)
+TableConditionalFormattingOutputTypeDef = TypedDict(
+    "TableConditionalFormattingOutputTypeDef",
+    {
+        "ConditionalFormattingOptions": NotRequired[
+            List[TableConditionalFormattingOptionOutputTypeDef]
+        ],
+    },
+)
 FilledMapConditionalFormattingTypeDef = TypedDict(
     "FilledMapConditionalFormattingTypeDef",
     {
         "ConditionalFormattingOptions": Sequence[FilledMapConditionalFormattingOptionTypeDef],
     },
 )
 PivotTableConditionalFormattingTypeDef = TypedDict(
@@ -10323,39 +12773,71 @@
     "UniqueValuesComputationTypeDef",
     {
         "ComputationId": str,
         "Name": NotRequired[str],
         "Category": NotRequired[DimensionFieldTypeDef],
     },
 )
+BarChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "BarChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+        "Colors": NotRequired[List[DimensionFieldTypeDef]],
+        "SmallMultiples": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 BarChartAggregatedFieldWellsTypeDef = TypedDict(
     "BarChartAggregatedFieldWellsTypeDef",
     {
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Colors": NotRequired[Sequence[DimensionFieldTypeDef]],
         "SmallMultiples": NotRequired[Sequence[DimensionFieldTypeDef]],
     },
 )
+BoxPlotAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "BoxPlotAggregatedFieldWellsOutputTypeDef",
+    {
+        "GroupBy": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 BoxPlotAggregatedFieldWellsTypeDef = TypedDict(
     "BoxPlotAggregatedFieldWellsTypeDef",
     {
         "GroupBy": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+ComboChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "ComboChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "BarValues": NotRequired[List[MeasureFieldTypeDef]],
+        "Colors": NotRequired[List[DimensionFieldTypeDef]],
+        "LineValues": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 ComboChartAggregatedFieldWellsTypeDef = TypedDict(
     "ComboChartAggregatedFieldWellsTypeDef",
     {
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "BarValues": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Colors": NotRequired[Sequence[DimensionFieldTypeDef]],
         "LineValues": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+FilledMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "FilledMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Geospatial": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 FilledMapAggregatedFieldWellsTypeDef = TypedDict(
     "FilledMapAggregatedFieldWellsTypeDef",
     {
         "Geospatial": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
@@ -10371,28 +12853,50 @@
         "UpperBoundary": NotRequired[float],
         "LowerBoundary": NotRequired[float],
         "PredictionInterval": NotRequired[int],
         "Seasonality": NotRequired[ForecastComputationSeasonalityType],
         "CustomSeasonalityValue": NotRequired[int],
     },
 )
+FunnelChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "FunnelChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 FunnelChartAggregatedFieldWellsTypeDef = TypedDict(
     "FunnelChartAggregatedFieldWellsTypeDef",
     {
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+GaugeChartFieldWellsOutputTypeDef = TypedDict(
+    "GaugeChartFieldWellsOutputTypeDef",
+    {
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+        "TargetValues": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 GaugeChartFieldWellsTypeDef = TypedDict(
     "GaugeChartFieldWellsTypeDef",
     {
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
         "TargetValues": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+GeospatialMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "GeospatialMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Geospatial": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+        "Colors": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 GeospatialMapAggregatedFieldWellsTypeDef = TypedDict(
     "GeospatialMapAggregatedFieldWellsTypeDef",
     {
         "Geospatial": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Colors": NotRequired[Sequence[DimensionFieldTypeDef]],
     },
@@ -10403,36 +12907,67 @@
         "ComputationId": str,
         "Name": NotRequired[str],
         "Time": NotRequired[DimensionFieldTypeDef],
         "Value": NotRequired[MeasureFieldTypeDef],
         "PeriodSize": NotRequired[int],
     },
 )
+HeatMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "HeatMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Rows": NotRequired[List[DimensionFieldTypeDef]],
+        "Columns": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 HeatMapAggregatedFieldWellsTypeDef = TypedDict(
     "HeatMapAggregatedFieldWellsTypeDef",
     {
         "Rows": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Columns": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+HistogramAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "HistogramAggregatedFieldWellsOutputTypeDef",
+    {
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 HistogramAggregatedFieldWellsTypeDef = TypedDict(
     "HistogramAggregatedFieldWellsTypeDef",
     {
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+KPIFieldWellsOutputTypeDef = TypedDict(
+    "KPIFieldWellsOutputTypeDef",
+    {
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+        "TargetValues": NotRequired[List[MeasureFieldTypeDef]],
+        "TrendGroups": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 KPIFieldWellsTypeDef = TypedDict(
     "KPIFieldWellsTypeDef",
     {
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
         "TargetValues": NotRequired[Sequence[MeasureFieldTypeDef]],
         "TrendGroups": NotRequired[Sequence[DimensionFieldTypeDef]],
     },
 )
+LineChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "LineChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+        "Colors": NotRequired[List[DimensionFieldTypeDef]],
+        "SmallMultiples": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 LineChartAggregatedFieldWellsTypeDef = TypedDict(
     "LineChartAggregatedFieldWellsTypeDef",
     {
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Colors": NotRequired[Sequence[DimensionFieldTypeDef]],
         "SmallMultiples": NotRequired[Sequence[DimensionFieldTypeDef]],
@@ -10473,66 +13008,125 @@
         "ComputationId": str,
         "Name": NotRequired[str],
         "Time": NotRequired[DimensionFieldTypeDef],
         "Value": NotRequired[MeasureFieldTypeDef],
         "PeriodTimeGranularity": NotRequired[TimeGranularityType],
     },
 )
+PieChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "PieChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+        "SmallMultiples": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 PieChartAggregatedFieldWellsTypeDef = TypedDict(
     "PieChartAggregatedFieldWellsTypeDef",
     {
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
         "SmallMultiples": NotRequired[Sequence[DimensionFieldTypeDef]],
     },
 )
+PivotTableAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "PivotTableAggregatedFieldWellsOutputTypeDef",
+    {
+        "Rows": NotRequired[List[DimensionFieldTypeDef]],
+        "Columns": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 PivotTableAggregatedFieldWellsTypeDef = TypedDict(
     "PivotTableAggregatedFieldWellsTypeDef",
     {
         "Rows": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Columns": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+RadarChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "RadarChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "Color": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 RadarChartAggregatedFieldWellsTypeDef = TypedDict(
     "RadarChartAggregatedFieldWellsTypeDef",
     {
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Color": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+SankeyDiagramAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "SankeyDiagramAggregatedFieldWellsOutputTypeDef",
+    {
+        "Source": NotRequired[List[DimensionFieldTypeDef]],
+        "Destination": NotRequired[List[DimensionFieldTypeDef]],
+        "Weight": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 SankeyDiagramAggregatedFieldWellsTypeDef = TypedDict(
     "SankeyDiagramAggregatedFieldWellsTypeDef",
     {
         "Source": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Destination": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Weight": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef",
+    {
+        "XAxis": NotRequired[List[MeasureFieldTypeDef]],
+        "YAxis": NotRequired[List[MeasureFieldTypeDef]],
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "Size": NotRequired[List[MeasureFieldTypeDef]],
+        "Label": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 ScatterPlotCategoricallyAggregatedFieldWellsTypeDef = TypedDict(
     "ScatterPlotCategoricallyAggregatedFieldWellsTypeDef",
     {
         "XAxis": NotRequired[Sequence[MeasureFieldTypeDef]],
         "YAxis": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Size": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Label": NotRequired[Sequence[DimensionFieldTypeDef]],
     },
 )
+ScatterPlotUnaggregatedFieldWellsOutputTypeDef = TypedDict(
+    "ScatterPlotUnaggregatedFieldWellsOutputTypeDef",
+    {
+        "XAxis": NotRequired[List[DimensionFieldTypeDef]],
+        "YAxis": NotRequired[List[DimensionFieldTypeDef]],
+        "Size": NotRequired[List[MeasureFieldTypeDef]],
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "Label": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 ScatterPlotUnaggregatedFieldWellsTypeDef = TypedDict(
     "ScatterPlotUnaggregatedFieldWellsTypeDef",
     {
         "XAxis": NotRequired[Sequence[DimensionFieldTypeDef]],
         "YAxis": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Size": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Label": NotRequired[Sequence[DimensionFieldTypeDef]],
     },
 )
+TableAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "TableAggregatedFieldWellsOutputTypeDef",
+    {
+        "GroupBy": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 TableAggregatedFieldWellsTypeDef = TypedDict(
     "TableAggregatedFieldWellsTypeDef",
     {
         "GroupBy": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
@@ -10564,43 +13158,81 @@
     "TotalAggregationComputationTypeDef",
     {
         "ComputationId": str,
         "Name": NotRequired[str],
         "Value": NotRequired[MeasureFieldTypeDef],
     },
 )
+TreeMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "TreeMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Groups": NotRequired[List[DimensionFieldTypeDef]],
+        "Sizes": NotRequired[List[MeasureFieldTypeDef]],
+        "Colors": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 TreeMapAggregatedFieldWellsTypeDef = TypedDict(
     "TreeMapAggregatedFieldWellsTypeDef",
     {
         "Groups": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Sizes": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Colors": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+WaterfallChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "WaterfallChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Categories": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+        "Breakdowns": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 WaterfallChartAggregatedFieldWellsTypeDef = TypedDict(
     "WaterfallChartAggregatedFieldWellsTypeDef",
     {
         "Categories": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Breakdowns": NotRequired[Sequence[DimensionFieldTypeDef]],
     },
 )
+WordCloudAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "WordCloudAggregatedFieldWellsOutputTypeDef",
+    {
+        "GroupBy": NotRequired[List[DimensionFieldTypeDef]],
+        "Size": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 WordCloudAggregatedFieldWellsTypeDef = TypedDict(
     "WordCloudAggregatedFieldWellsTypeDef",
     {
         "GroupBy": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Size": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+TableUnaggregatedFieldWellsOutputTypeDef = TypedDict(
+    "TableUnaggregatedFieldWellsOutputTypeDef",
+    {
+        "Values": NotRequired[List[UnaggregatedFieldTypeDef]],
+    },
+)
 TableUnaggregatedFieldWellsTypeDef = TypedDict(
     "TableUnaggregatedFieldWellsTypeDef",
     {
         "Values": NotRequired[Sequence[UnaggregatedFieldTypeDef]],
     },
 )
+SectionBasedLayoutConfigurationOutputTypeDef = TypedDict(
+    "SectionBasedLayoutConfigurationOutputTypeDef",
+    {
+        "HeaderSections": List[HeaderFooterSectionConfigurationOutputTypeDef],
+        "BodySections": List[BodySectionConfigurationOutputTypeDef],
+        "FooterSections": List[HeaderFooterSectionConfigurationOutputTypeDef],
+        "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
+    },
+)
 SectionBasedLayoutConfigurationTypeDef = TypedDict(
     "SectionBasedLayoutConfigurationTypeDef",
     {
         "HeaderSections": Sequence[HeaderFooterSectionConfigurationTypeDef],
         "BodySections": Sequence[BodySectionConfigurationTypeDef],
         "FooterSections": Sequence[HeaderFooterSectionConfigurationTypeDef],
         "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
@@ -10621,124 +13253,253 @@
     "EmptyVisualTypeDef",
     {
         "VisualId": str,
         "DataSetIdentifier": str,
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+FilterOutputTypeDef = TypedDict(
+    "FilterOutputTypeDef",
+    {
+        "CategoryFilter": NotRequired[CategoryFilterOutputTypeDef],
+        "NumericRangeFilter": NotRequired[NumericRangeFilterOutputTypeDef],
+        "NumericEqualityFilter": NotRequired[NumericEqualityFilterOutputTypeDef],
+        "TimeEqualityFilter": NotRequired[TimeEqualityFilterOutputTypeDef],
+        "TimeRangeFilter": NotRequired[TimeRangeFilterOutputTypeDef],
+        "RelativeDatesFilter": NotRequired[RelativeDatesFilterOutputTypeDef],
+        "TopBottomFilter": NotRequired[TopBottomFilterOutputTypeDef],
+    },
+)
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "CategoryFilter": NotRequired[CategoryFilterTypeDef],
         "NumericRangeFilter": NotRequired[NumericRangeFilterTypeDef],
         "NumericEqualityFilter": NotRequired[NumericEqualityFilterTypeDef],
         "TimeEqualityFilter": NotRequired[TimeEqualityFilterTypeDef],
         "TimeRangeFilter": NotRequired[TimeRangeFilterTypeDef],
         "RelativeDatesFilter": NotRequired[RelativeDatesFilterTypeDef],
         "TopBottomFilter": NotRequired[TopBottomFilterTypeDef],
     },
 )
+BarChartFieldWellsOutputTypeDef = TypedDict(
+    "BarChartFieldWellsOutputTypeDef",
+    {
+        "BarChartAggregatedFieldWells": NotRequired[BarChartAggregatedFieldWellsOutputTypeDef],
+    },
+)
 BarChartFieldWellsTypeDef = TypedDict(
     "BarChartFieldWellsTypeDef",
     {
         "BarChartAggregatedFieldWells": NotRequired[BarChartAggregatedFieldWellsTypeDef],
     },
 )
+BoxPlotFieldWellsOutputTypeDef = TypedDict(
+    "BoxPlotFieldWellsOutputTypeDef",
+    {
+        "BoxPlotAggregatedFieldWells": NotRequired[BoxPlotAggregatedFieldWellsOutputTypeDef],
+    },
+)
 BoxPlotFieldWellsTypeDef = TypedDict(
     "BoxPlotFieldWellsTypeDef",
     {
         "BoxPlotAggregatedFieldWells": NotRequired[BoxPlotAggregatedFieldWellsTypeDef],
     },
 )
+ComboChartFieldWellsOutputTypeDef = TypedDict(
+    "ComboChartFieldWellsOutputTypeDef",
+    {
+        "ComboChartAggregatedFieldWells": NotRequired[ComboChartAggregatedFieldWellsOutputTypeDef],
+    },
+)
 ComboChartFieldWellsTypeDef = TypedDict(
     "ComboChartFieldWellsTypeDef",
     {
         "ComboChartAggregatedFieldWells": NotRequired[ComboChartAggregatedFieldWellsTypeDef],
     },
 )
+FilledMapFieldWellsOutputTypeDef = TypedDict(
+    "FilledMapFieldWellsOutputTypeDef",
+    {
+        "FilledMapAggregatedFieldWells": NotRequired[FilledMapAggregatedFieldWellsOutputTypeDef],
+    },
+)
 FilledMapFieldWellsTypeDef = TypedDict(
     "FilledMapFieldWellsTypeDef",
     {
         "FilledMapAggregatedFieldWells": NotRequired[FilledMapAggregatedFieldWellsTypeDef],
     },
 )
+FunnelChartFieldWellsOutputTypeDef = TypedDict(
+    "FunnelChartFieldWellsOutputTypeDef",
+    {
+        "FunnelChartAggregatedFieldWells": NotRequired[
+            FunnelChartAggregatedFieldWellsOutputTypeDef
+        ],
+    },
+)
 FunnelChartFieldWellsTypeDef = TypedDict(
     "FunnelChartFieldWellsTypeDef",
     {
         "FunnelChartAggregatedFieldWells": NotRequired[FunnelChartAggregatedFieldWellsTypeDef],
     },
 )
+GaugeChartConfigurationOutputTypeDef = TypedDict(
+    "GaugeChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[GaugeChartFieldWellsOutputTypeDef],
+        "GaugeChartOptions": NotRequired[GaugeChartOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "TooltipOptions": NotRequired[TooltipOptionsOutputTypeDef],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "ColorConfiguration": NotRequired[GaugeChartColorConfigurationTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 GaugeChartConfigurationTypeDef = TypedDict(
     "GaugeChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[GaugeChartFieldWellsTypeDef],
         "GaugeChartOptions": NotRequired[GaugeChartOptionsTypeDef],
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "TooltipOptions": NotRequired[TooltipOptionsTypeDef],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
+        "ColorConfiguration": NotRequired[GaugeChartColorConfigurationTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+GeospatialMapFieldWellsOutputTypeDef = TypedDict(
+    "GeospatialMapFieldWellsOutputTypeDef",
+    {
+        "GeospatialMapAggregatedFieldWells": NotRequired[
+            GeospatialMapAggregatedFieldWellsOutputTypeDef
+        ],
+    },
+)
 GeospatialMapFieldWellsTypeDef = TypedDict(
     "GeospatialMapFieldWellsTypeDef",
     {
         "GeospatialMapAggregatedFieldWells": NotRequired[GeospatialMapAggregatedFieldWellsTypeDef],
     },
 )
+HeatMapFieldWellsOutputTypeDef = TypedDict(
+    "HeatMapFieldWellsOutputTypeDef",
+    {
+        "HeatMapAggregatedFieldWells": NotRequired[HeatMapAggregatedFieldWellsOutputTypeDef],
+    },
+)
 HeatMapFieldWellsTypeDef = TypedDict(
     "HeatMapFieldWellsTypeDef",
     {
         "HeatMapAggregatedFieldWells": NotRequired[HeatMapAggregatedFieldWellsTypeDef],
     },
 )
+HistogramFieldWellsOutputTypeDef = TypedDict(
+    "HistogramFieldWellsOutputTypeDef",
+    {
+        "HistogramAggregatedFieldWells": NotRequired[HistogramAggregatedFieldWellsOutputTypeDef],
+    },
+)
 HistogramFieldWellsTypeDef = TypedDict(
     "HistogramFieldWellsTypeDef",
     {
         "HistogramAggregatedFieldWells": NotRequired[HistogramAggregatedFieldWellsTypeDef],
     },
 )
+KPIConfigurationOutputTypeDef = TypedDict(
+    "KPIConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[KPIFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[KPISortConfigurationOutputTypeDef],
+        "KPIOptions": NotRequired[KPIOptionsTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 KPIConfigurationTypeDef = TypedDict(
     "KPIConfigurationTypeDef",
     {
         "FieldWells": NotRequired[KPIFieldWellsTypeDef],
         "SortConfiguration": NotRequired[KPISortConfigurationTypeDef],
         "KPIOptions": NotRequired[KPIOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+LineChartFieldWellsOutputTypeDef = TypedDict(
+    "LineChartFieldWellsOutputTypeDef",
+    {
+        "LineChartAggregatedFieldWells": NotRequired[LineChartAggregatedFieldWellsOutputTypeDef],
+    },
+)
 LineChartFieldWellsTypeDef = TypedDict(
     "LineChartFieldWellsTypeDef",
     {
         "LineChartAggregatedFieldWells": NotRequired[LineChartAggregatedFieldWellsTypeDef],
     },
 )
+PieChartFieldWellsOutputTypeDef = TypedDict(
+    "PieChartFieldWellsOutputTypeDef",
+    {
+        "PieChartAggregatedFieldWells": NotRequired[PieChartAggregatedFieldWellsOutputTypeDef],
+    },
+)
 PieChartFieldWellsTypeDef = TypedDict(
     "PieChartFieldWellsTypeDef",
     {
         "PieChartAggregatedFieldWells": NotRequired[PieChartAggregatedFieldWellsTypeDef],
     },
 )
+PivotTableFieldWellsOutputTypeDef = TypedDict(
+    "PivotTableFieldWellsOutputTypeDef",
+    {
+        "PivotTableAggregatedFieldWells": NotRequired[PivotTableAggregatedFieldWellsOutputTypeDef],
+    },
+)
 PivotTableFieldWellsTypeDef = TypedDict(
     "PivotTableFieldWellsTypeDef",
     {
         "PivotTableAggregatedFieldWells": NotRequired[PivotTableAggregatedFieldWellsTypeDef],
     },
 )
+RadarChartFieldWellsOutputTypeDef = TypedDict(
+    "RadarChartFieldWellsOutputTypeDef",
+    {
+        "RadarChartAggregatedFieldWells": NotRequired[RadarChartAggregatedFieldWellsOutputTypeDef],
+    },
+)
 RadarChartFieldWellsTypeDef = TypedDict(
     "RadarChartFieldWellsTypeDef",
     {
         "RadarChartAggregatedFieldWells": NotRequired[RadarChartAggregatedFieldWellsTypeDef],
     },
 )
+SankeyDiagramFieldWellsOutputTypeDef = TypedDict(
+    "SankeyDiagramFieldWellsOutputTypeDef",
+    {
+        "SankeyDiagramAggregatedFieldWells": NotRequired[
+            SankeyDiagramAggregatedFieldWellsOutputTypeDef
+        ],
+    },
+)
 SankeyDiagramFieldWellsTypeDef = TypedDict(
     "SankeyDiagramFieldWellsTypeDef",
     {
         "SankeyDiagramAggregatedFieldWells": NotRequired[SankeyDiagramAggregatedFieldWellsTypeDef],
     },
 )
+ScatterPlotFieldWellsOutputTypeDef = TypedDict(
+    "ScatterPlotFieldWellsOutputTypeDef",
+    {
+        "ScatterPlotCategoricallyAggregatedFieldWells": NotRequired[
+            ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef
+        ],
+        "ScatterPlotUnaggregatedFieldWells": NotRequired[
+            ScatterPlotUnaggregatedFieldWellsOutputTypeDef
+        ],
+    },
+)
 ScatterPlotFieldWellsTypeDef = TypedDict(
     "ScatterPlotFieldWellsTypeDef",
     {
         "ScatterPlotCategoricallyAggregatedFieldWells": NotRequired[
             ScatterPlotCategoricallyAggregatedFieldWellsTypeDef
         ],
         "ScatterPlotUnaggregatedFieldWells": NotRequired[ScatterPlotUnaggregatedFieldWellsTypeDef],
@@ -10755,59 +13516,126 @@
         "PeriodOverPeriod": NotRequired[PeriodOverPeriodComputationTypeDef],
         "PeriodToDate": NotRequired[PeriodToDateComputationTypeDef],
         "GrowthRate": NotRequired[GrowthRateComputationTypeDef],
         "UniqueValues": NotRequired[UniqueValuesComputationTypeDef],
         "Forecast": NotRequired[ForecastComputationTypeDef],
     },
 )
+TreeMapFieldWellsOutputTypeDef = TypedDict(
+    "TreeMapFieldWellsOutputTypeDef",
+    {
+        "TreeMapAggregatedFieldWells": NotRequired[TreeMapAggregatedFieldWellsOutputTypeDef],
+    },
+)
 TreeMapFieldWellsTypeDef = TypedDict(
     "TreeMapFieldWellsTypeDef",
     {
         "TreeMapAggregatedFieldWells": NotRequired[TreeMapAggregatedFieldWellsTypeDef],
     },
 )
+WaterfallChartFieldWellsOutputTypeDef = TypedDict(
+    "WaterfallChartFieldWellsOutputTypeDef",
+    {
+        "WaterfallChartAggregatedFieldWells": NotRequired[
+            WaterfallChartAggregatedFieldWellsOutputTypeDef
+        ],
+    },
+)
 WaterfallChartFieldWellsTypeDef = TypedDict(
     "WaterfallChartFieldWellsTypeDef",
     {
         "WaterfallChartAggregatedFieldWells": NotRequired[
             WaterfallChartAggregatedFieldWellsTypeDef
         ],
     },
 )
+WordCloudFieldWellsOutputTypeDef = TypedDict(
+    "WordCloudFieldWellsOutputTypeDef",
+    {
+        "WordCloudAggregatedFieldWells": NotRequired[WordCloudAggregatedFieldWellsOutputTypeDef],
+    },
+)
 WordCloudFieldWellsTypeDef = TypedDict(
     "WordCloudFieldWellsTypeDef",
     {
         "WordCloudAggregatedFieldWells": NotRequired[WordCloudAggregatedFieldWellsTypeDef],
     },
 )
+TableFieldWellsOutputTypeDef = TypedDict(
+    "TableFieldWellsOutputTypeDef",
+    {
+        "TableAggregatedFieldWells": NotRequired[TableAggregatedFieldWellsOutputTypeDef],
+        "TableUnaggregatedFieldWells": NotRequired[TableUnaggregatedFieldWellsOutputTypeDef],
+    },
+)
 TableFieldWellsTypeDef = TypedDict(
     "TableFieldWellsTypeDef",
     {
         "TableAggregatedFieldWells": NotRequired[TableAggregatedFieldWellsTypeDef],
         "TableUnaggregatedFieldWells": NotRequired[TableUnaggregatedFieldWellsTypeDef],
     },
 )
+LayoutConfigurationOutputTypeDef = TypedDict(
+    "LayoutConfigurationOutputTypeDef",
+    {
+        "GridLayout": NotRequired[GridLayoutConfigurationOutputTypeDef],
+        "FreeFormLayout": NotRequired[FreeFormLayoutConfigurationOutputTypeDef],
+        "SectionBasedLayout": NotRequired[SectionBasedLayoutConfigurationOutputTypeDef],
+    },
+)
 LayoutConfigurationTypeDef = TypedDict(
     "LayoutConfigurationTypeDef",
     {
         "GridLayout": NotRequired[GridLayoutConfigurationTypeDef],
         "FreeFormLayout": NotRequired[FreeFormLayoutConfigurationTypeDef],
         "SectionBasedLayout": NotRequired[SectionBasedLayoutConfigurationTypeDef],
     },
 )
+FilterGroupOutputTypeDef = TypedDict(
+    "FilterGroupOutputTypeDef",
+    {
+        "FilterGroupId": str,
+        "Filters": List[FilterOutputTypeDef],
+        "ScopeConfiguration": FilterScopeConfigurationOutputTypeDef,
+        "CrossDataset": CrossDatasetTypesType,
+        "Status": NotRequired[WidgetStatusType],
+    },
+)
 FilterGroupTypeDef = TypedDict(
     "FilterGroupTypeDef",
     {
         "FilterGroupId": str,
         "Filters": Sequence[FilterTypeDef],
         "ScopeConfiguration": FilterScopeConfigurationTypeDef,
         "CrossDataset": CrossDatasetTypesType,
         "Status": NotRequired[WidgetStatusType],
     },
 )
+BarChartConfigurationOutputTypeDef = TypedDict(
+    "BarChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[BarChartFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[BarChartSortConfigurationOutputTypeDef],
+        "Orientation": NotRequired[BarChartOrientationType],
+        "BarsArrangement": NotRequired[BarsArrangementType],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "SmallMultiplesOptions": NotRequired[SmallMultiplesOptionsTypeDef],
+        "CategoryAxis": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ValueAxis": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "ValueLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ColorLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "ReferenceLines": NotRequired[List[ReferenceLineTypeDef]],
+        "ContributionAnalysisDefaults": NotRequired[List[ContributionAnalysisDefaultOutputTypeDef]],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 BarChartConfigurationTypeDef = TypedDict(
     "BarChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[BarChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[BarChartSortConfigurationTypeDef],
         "Orientation": NotRequired[BarChartOrientationType],
         "BarsArrangement": NotRequired[BarsArrangementType],
@@ -10822,14 +13650,31 @@
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "ReferenceLines": NotRequired[Sequence[ReferenceLineTypeDef]],
         "ContributionAnalysisDefaults": NotRequired[Sequence[ContributionAnalysisDefaultTypeDef]],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+BoxPlotChartConfigurationOutputTypeDef = TypedDict(
+    "BoxPlotChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[BoxPlotFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[BoxPlotSortConfigurationOutputTypeDef],
+        "BoxPlotOptions": NotRequired[BoxPlotOptionsTypeDef],
+        "CategoryAxis": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "PrimaryYAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "PrimaryYAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "ReferenceLines": NotRequired[List[ReferenceLineTypeDef]],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 BoxPlotChartConfigurationTypeDef = TypedDict(
     "BoxPlotChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[BoxPlotFieldWellsTypeDef],
         "SortConfiguration": NotRequired[BoxPlotSortConfigurationTypeDef],
         "BoxPlotOptions": NotRequired[BoxPlotOptionsTypeDef],
         "CategoryAxis": NotRequired[AxisDisplayOptionsTypeDef],
@@ -10839,14 +13684,37 @@
         "Legend": NotRequired[LegendOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "ReferenceLines": NotRequired[Sequence[ReferenceLineTypeDef]],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+ComboChartConfigurationOutputTypeDef = TypedDict(
+    "ComboChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[ComboChartFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[ComboChartSortConfigurationOutputTypeDef],
+        "BarsArrangement": NotRequired[BarsArrangementType],
+        "CategoryAxis": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "PrimaryYAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "PrimaryYAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "SecondaryYAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "SecondaryYAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "SingleAxisOptions": NotRequired[SingleAxisOptionsTypeDef],
+        "ColorLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "BarDataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "LineDataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "ReferenceLines": NotRequired[List[ReferenceLineTypeDef]],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 ComboChartConfigurationTypeDef = TypedDict(
     "ComboChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[ComboChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[ComboChartSortConfigurationTypeDef],
         "BarsArrangement": NotRequired[BarsArrangementType],
         "CategoryAxis": NotRequired[AxisDisplayOptionsTypeDef],
@@ -10862,103 +13730,218 @@
         "LineDataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "ReferenceLines": NotRequired[Sequence[ReferenceLineTypeDef]],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+FilledMapConfigurationOutputTypeDef = TypedDict(
+    "FilledMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[FilledMapFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[FilledMapSortConfigurationOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "WindowOptions": NotRequired[GeospatialWindowOptionsTypeDef],
+        "MapStyleOptions": NotRequired[GeospatialMapStyleOptionsTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 FilledMapConfigurationTypeDef = TypedDict(
     "FilledMapConfigurationTypeDef",
     {
         "FieldWells": NotRequired[FilledMapFieldWellsTypeDef],
         "SortConfiguration": NotRequired[FilledMapSortConfigurationTypeDef],
         "Legend": NotRequired[LegendOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "WindowOptions": NotRequired[GeospatialWindowOptionsTypeDef],
         "MapStyleOptions": NotRequired[GeospatialMapStyleOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+FunnelChartConfigurationOutputTypeDef = TypedDict(
+    "FunnelChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[FunnelChartFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[FunnelChartSortConfigurationOutputTypeDef],
+        "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ValueLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "DataLabelOptions": NotRequired[FunnelChartDataLabelOptionsTypeDef],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 FunnelChartConfigurationTypeDef = TypedDict(
     "FunnelChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[FunnelChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[FunnelChartSortConfigurationTypeDef],
         "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "ValueLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "DataLabelOptions": NotRequired[FunnelChartDataLabelOptionsTypeDef],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+GaugeChartVisualOutputTypeDef = TypedDict(
+    "GaugeChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[GaugeChartConfigurationOutputTypeDef],
+        "ConditionalFormatting": NotRequired[GaugeChartConditionalFormattingOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 GaugeChartVisualTypeDef = TypedDict(
     "GaugeChartVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[GaugeChartConfigurationTypeDef],
         "ConditionalFormatting": NotRequired[GaugeChartConditionalFormattingTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+GeospatialMapConfigurationOutputTypeDef = TypedDict(
+    "GeospatialMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[GeospatialMapFieldWellsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "WindowOptions": NotRequired[GeospatialWindowOptionsTypeDef],
+        "MapStyleOptions": NotRequired[GeospatialMapStyleOptionsTypeDef],
+        "PointStyleOptions": NotRequired[GeospatialPointStyleOptionsOutputTypeDef],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 GeospatialMapConfigurationTypeDef = TypedDict(
     "GeospatialMapConfigurationTypeDef",
     {
         "FieldWells": NotRequired[GeospatialMapFieldWellsTypeDef],
         "Legend": NotRequired[LegendOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "WindowOptions": NotRequired[GeospatialWindowOptionsTypeDef],
         "MapStyleOptions": NotRequired[GeospatialMapStyleOptionsTypeDef],
         "PointStyleOptions": NotRequired[GeospatialPointStyleOptionsTypeDef],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+HeatMapConfigurationOutputTypeDef = TypedDict(
+    "HeatMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[HeatMapFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[HeatMapSortConfigurationOutputTypeDef],
+        "RowLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ColumnLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ColorScale": NotRequired[ColorScaleOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 HeatMapConfigurationTypeDef = TypedDict(
     "HeatMapConfigurationTypeDef",
     {
         "FieldWells": NotRequired[HeatMapFieldWellsTypeDef],
         "SortConfiguration": NotRequired[HeatMapSortConfigurationTypeDef],
         "RowLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "ColumnLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "ColorScale": NotRequired[ColorScaleTypeDef],
         "Legend": NotRequired[LegendOptionsTypeDef],
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+HistogramConfigurationOutputTypeDef = TypedDict(
+    "HistogramConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[HistogramFieldWellsOutputTypeDef],
+        "XAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "XAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "YAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "BinOptions": NotRequired[HistogramBinOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 HistogramConfigurationTypeDef = TypedDict(
     "HistogramConfigurationTypeDef",
     {
         "FieldWells": NotRequired[HistogramFieldWellsTypeDef],
         "XAxisDisplayOptions": NotRequired[AxisDisplayOptionsTypeDef],
         "XAxisLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "YAxisDisplayOptions": NotRequired[AxisDisplayOptionsTypeDef],
         "BinOptions": NotRequired[HistogramBinOptionsTypeDef],
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+KPIVisualOutputTypeDef = TypedDict(
+    "KPIVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[KPIConfigurationOutputTypeDef],
+        "ConditionalFormatting": NotRequired[KPIConditionalFormattingOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 KPIVisualTypeDef = TypedDict(
     "KPIVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[KPIConfigurationTypeDef],
         "ConditionalFormatting": NotRequired[KPIConditionalFormattingTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+LineChartConfigurationOutputTypeDef = TypedDict(
+    "LineChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[LineChartFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[LineChartSortConfigurationOutputTypeDef],
+        "ForecastConfigurations": NotRequired[List[ForecastConfigurationOutputTypeDef]],
+        "Type": NotRequired[LineChartTypeType],
+        "SmallMultiplesOptions": NotRequired[SmallMultiplesOptionsTypeDef],
+        "XAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "XAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "PrimaryYAxisDisplayOptions": NotRequired[LineSeriesAxisDisplayOptionsOutputTypeDef],
+        "PrimaryYAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "SecondaryYAxisDisplayOptions": NotRequired[LineSeriesAxisDisplayOptionsOutputTypeDef],
+        "SecondaryYAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "SingleAxisOptions": NotRequired[SingleAxisOptionsTypeDef],
+        "DefaultSeriesSettings": NotRequired[LineChartDefaultSeriesSettingsTypeDef],
+        "Series": NotRequired[List[SeriesItemTypeDef]],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "ReferenceLines": NotRequired[List[ReferenceLineTypeDef]],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "ContributionAnalysisDefaults": NotRequired[List[ContributionAnalysisDefaultOutputTypeDef]],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 LineChartConfigurationTypeDef = TypedDict(
     "LineChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[LineChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[LineChartSortConfigurationTypeDef],
         "ForecastConfigurations": NotRequired[Sequence[ForecastConfigurationTypeDef]],
         "Type": NotRequired[LineChartTypeType],
@@ -10977,14 +13960,31 @@
         "ReferenceLines": NotRequired[Sequence[ReferenceLineTypeDef]],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "ContributionAnalysisDefaults": NotRequired[Sequence[ContributionAnalysisDefaultTypeDef]],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+PieChartConfigurationOutputTypeDef = TypedDict(
+    "PieChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[PieChartFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[PieChartSortConfigurationOutputTypeDef],
+        "DonutOptions": NotRequired[DonutOptionsTypeDef],
+        "SmallMultiplesOptions": NotRequired[SmallMultiplesOptionsTypeDef],
+        "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ValueLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "ContributionAnalysisDefaults": NotRequired[List[ContributionAnalysisDefaultOutputTypeDef]],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 PieChartConfigurationTypeDef = TypedDict(
     "PieChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[PieChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[PieChartSortConfigurationTypeDef],
         "DonutOptions": NotRequired[DonutOptionsTypeDef],
         "SmallMultiplesOptions": NotRequired[SmallMultiplesOptionsTypeDef],
@@ -10994,26 +13994,59 @@
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "ContributionAnalysisDefaults": NotRequired[Sequence[ContributionAnalysisDefaultTypeDef]],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+PivotTableConfigurationOutputTypeDef = TypedDict(
+    "PivotTableConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[PivotTableFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[PivotTableSortConfigurationOutputTypeDef],
+        "TableOptions": NotRequired[PivotTableOptionsOutputTypeDef],
+        "TotalOptions": NotRequired[PivotTableTotalOptionsOutputTypeDef],
+        "FieldOptions": NotRequired[PivotTableFieldOptionsOutputTypeDef],
+        "PaginatedReportOptions": NotRequired[PivotTablePaginatedReportOptionsTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 PivotTableConfigurationTypeDef = TypedDict(
     "PivotTableConfigurationTypeDef",
     {
         "FieldWells": NotRequired[PivotTableFieldWellsTypeDef],
         "SortConfiguration": NotRequired[PivotTableSortConfigurationTypeDef],
         "TableOptions": NotRequired[PivotTableOptionsTypeDef],
         "TotalOptions": NotRequired[PivotTableTotalOptionsTypeDef],
         "FieldOptions": NotRequired[PivotTableFieldOptionsTypeDef],
         "PaginatedReportOptions": NotRequired[PivotTablePaginatedReportOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+RadarChartConfigurationOutputTypeDef = TypedDict(
+    "RadarChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[RadarChartFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[RadarChartSortConfigurationOutputTypeDef],
+        "Shape": NotRequired[RadarChartShapeType],
+        "BaseSeriesSettings": NotRequired[RadarChartSeriesSettingsTypeDef],
+        "StartAngle": NotRequired[float],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "AlternateBandColorsVisibility": NotRequired[VisibilityType],
+        "AlternateBandEvenColor": NotRequired[str],
+        "AlternateBandOddColor": NotRequired[str],
+        "CategoryAxis": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ColorAxis": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "ColorLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "AxesRangeScale": NotRequired[RadarChartAxesRangeScaleType],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 RadarChartConfigurationTypeDef = TypedDict(
     "RadarChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[RadarChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[RadarChartSortConfigurationTypeDef],
         "Shape": NotRequired[RadarChartShapeType],
         "BaseSeriesSettings": NotRequired[RadarChartSeriesSettingsTypeDef],
@@ -11027,23 +14060,48 @@
         "ColorAxis": NotRequired[AxisDisplayOptionsTypeDef],
         "ColorLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "Legend": NotRequired[LegendOptionsTypeDef],
         "AxesRangeScale": NotRequired[RadarChartAxesRangeScaleType],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+SankeyDiagramChartConfigurationOutputTypeDef = TypedDict(
+    "SankeyDiagramChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[SankeyDiagramFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[SankeyDiagramSortConfigurationOutputTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 SankeyDiagramChartConfigurationTypeDef = TypedDict(
     "SankeyDiagramChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[SankeyDiagramFieldWellsTypeDef],
         "SortConfiguration": NotRequired[SankeyDiagramSortConfigurationTypeDef],
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+ScatterPlotConfigurationOutputTypeDef = TypedDict(
+    "ScatterPlotConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[ScatterPlotFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[ScatterPlotSortConfigurationTypeDef],
+        "XAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "XAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "YAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "YAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 ScatterPlotConfigurationTypeDef = TypedDict(
     "ScatterPlotConfigurationTypeDef",
     {
         "FieldWells": NotRequired[ScatterPlotFieldWellsTypeDef],
         "SortConfiguration": NotRequired[ScatterPlotSortConfigurationTypeDef],
         "XAxisLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "XAxisDisplayOptions": NotRequired[AxisDisplayOptionsTypeDef],
@@ -11052,22 +14110,45 @@
         "Legend": NotRequired[LegendOptionsTypeDef],
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+InsightConfigurationOutputTypeDef = TypedDict(
+    "InsightConfigurationOutputTypeDef",
+    {
+        "Computations": NotRequired[List[ComputationTypeDef]],
+        "CustomNarrative": NotRequired[CustomNarrativeOptionsTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 InsightConfigurationTypeDef = TypedDict(
     "InsightConfigurationTypeDef",
     {
         "Computations": NotRequired[Sequence[ComputationTypeDef]],
         "CustomNarrative": NotRequired[CustomNarrativeOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+TreeMapConfigurationOutputTypeDef = TypedDict(
+    "TreeMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[TreeMapFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[TreeMapSortConfigurationOutputTypeDef],
+        "GroupLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "SizeLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ColorLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ColorScale": NotRequired[ColorScaleOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 TreeMapConfigurationTypeDef = TypedDict(
     "TreeMapConfigurationTypeDef",
     {
         "FieldWells": NotRequired[TreeMapFieldWellsTypeDef],
         "SortConfiguration": NotRequired[TreeMapSortConfigurationTypeDef],
         "GroupLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "SizeLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
@@ -11075,14 +14156,31 @@
         "ColorScale": NotRequired[ColorScaleTypeDef],
         "Legend": NotRequired[LegendOptionsTypeDef],
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+WaterfallChartConfigurationOutputTypeDef = TypedDict(
+    "WaterfallChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[WaterfallChartFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[WaterfallChartSortConfigurationOutputTypeDef],
+        "WaterfallChartOptions": NotRequired[WaterfallChartOptionsTypeDef],
+        "CategoryAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "CategoryAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "PrimaryYAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "PrimaryYAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "ColorConfiguration": NotRequired[WaterfallChartColorConfigurationTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 WaterfallChartConfigurationTypeDef = TypedDict(
     "WaterfallChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[WaterfallChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[WaterfallChartSortConfigurationTypeDef],
         "WaterfallChartOptions": NotRequired[WaterfallChartOptionsTypeDef],
         "CategoryAxisLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
@@ -11092,251 +14190,516 @@
         "Legend": NotRequired[LegendOptionsTypeDef],
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "ColorConfiguration": NotRequired[WaterfallChartColorConfigurationTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+WordCloudChartConfigurationOutputTypeDef = TypedDict(
+    "WordCloudChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[WordCloudFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[WordCloudSortConfigurationOutputTypeDef],
+        "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "WordCloudOptions": NotRequired[WordCloudOptionsTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 WordCloudChartConfigurationTypeDef = TypedDict(
     "WordCloudChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[WordCloudFieldWellsTypeDef],
         "SortConfiguration": NotRequired[WordCloudSortConfigurationTypeDef],
         "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "WordCloudOptions": NotRequired[WordCloudOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+TableConfigurationOutputTypeDef = TypedDict(
+    "TableConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[TableFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[TableSortConfigurationOutputTypeDef],
+        "TableOptions": NotRequired[TableOptionsOutputTypeDef],
+        "TotalOptions": NotRequired[TotalOptionsOutputTypeDef],
+        "FieldOptions": NotRequired[TableFieldOptionsOutputTypeDef],
+        "PaginatedReportOptions": NotRequired[TablePaginatedReportOptionsTypeDef],
+        "TableInlineVisualizations": NotRequired[List[TableInlineVisualizationTypeDef]],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 TableConfigurationTypeDef = TypedDict(
     "TableConfigurationTypeDef",
     {
         "FieldWells": NotRequired[TableFieldWellsTypeDef],
         "SortConfiguration": NotRequired[TableSortConfigurationTypeDef],
         "TableOptions": NotRequired[TableOptionsTypeDef],
         "TotalOptions": NotRequired[TotalOptionsTypeDef],
         "FieldOptions": NotRequired[TableFieldOptionsTypeDef],
         "PaginatedReportOptions": NotRequired[TablePaginatedReportOptionsTypeDef],
         "TableInlineVisualizations": NotRequired[Sequence[TableInlineVisualizationTypeDef]],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+LayoutOutputTypeDef = TypedDict(
+    "LayoutOutputTypeDef",
+    {
+        "Configuration": LayoutConfigurationOutputTypeDef,
+    },
+)
 LayoutTypeDef = TypedDict(
     "LayoutTypeDef",
     {
         "Configuration": LayoutConfigurationTypeDef,
     },
 )
+BarChartVisualOutputTypeDef = TypedDict(
+    "BarChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[BarChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 BarChartVisualTypeDef = TypedDict(
     "BarChartVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[BarChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+BoxPlotVisualOutputTypeDef = TypedDict(
+    "BoxPlotVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[BoxPlotChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 BoxPlotVisualTypeDef = TypedDict(
     "BoxPlotVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[BoxPlotChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+ComboChartVisualOutputTypeDef = TypedDict(
+    "ComboChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[ComboChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 ComboChartVisualTypeDef = TypedDict(
     "ComboChartVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[ComboChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+FilledMapVisualOutputTypeDef = TypedDict(
+    "FilledMapVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[FilledMapConfigurationOutputTypeDef],
+        "ConditionalFormatting": NotRequired[FilledMapConditionalFormattingOutputTypeDef],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 FilledMapVisualTypeDef = TypedDict(
     "FilledMapVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[FilledMapConfigurationTypeDef],
         "ConditionalFormatting": NotRequired[FilledMapConditionalFormattingTypeDef],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+FunnelChartVisualOutputTypeDef = TypedDict(
+    "FunnelChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[FunnelChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 FunnelChartVisualTypeDef = TypedDict(
     "FunnelChartVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[FunnelChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+GeospatialMapVisualOutputTypeDef = TypedDict(
+    "GeospatialMapVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[GeospatialMapConfigurationOutputTypeDef],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 GeospatialMapVisualTypeDef = TypedDict(
     "GeospatialMapVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[GeospatialMapConfigurationTypeDef],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+HeatMapVisualOutputTypeDef = TypedDict(
+    "HeatMapVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[HeatMapConfigurationOutputTypeDef],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 HeatMapVisualTypeDef = TypedDict(
     "HeatMapVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[HeatMapConfigurationTypeDef],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+HistogramVisualOutputTypeDef = TypedDict(
+    "HistogramVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[HistogramConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 HistogramVisualTypeDef = TypedDict(
     "HistogramVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[HistogramConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+LineChartVisualOutputTypeDef = TypedDict(
+    "LineChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[LineChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 LineChartVisualTypeDef = TypedDict(
     "LineChartVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[LineChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+PieChartVisualOutputTypeDef = TypedDict(
+    "PieChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[PieChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 PieChartVisualTypeDef = TypedDict(
     "PieChartVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[PieChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+PivotTableVisualOutputTypeDef = TypedDict(
+    "PivotTableVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[PivotTableConfigurationOutputTypeDef],
+        "ConditionalFormatting": NotRequired[PivotTableConditionalFormattingOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 PivotTableVisualTypeDef = TypedDict(
     "PivotTableVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[PivotTableConfigurationTypeDef],
         "ConditionalFormatting": NotRequired[PivotTableConditionalFormattingTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+RadarChartVisualOutputTypeDef = TypedDict(
+    "RadarChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[RadarChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 RadarChartVisualTypeDef = TypedDict(
     "RadarChartVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[RadarChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+SankeyDiagramVisualOutputTypeDef = TypedDict(
+    "SankeyDiagramVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[SankeyDiagramChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 SankeyDiagramVisualTypeDef = TypedDict(
     "SankeyDiagramVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[SankeyDiagramChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+ScatterPlotVisualOutputTypeDef = TypedDict(
+    "ScatterPlotVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[ScatterPlotConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 ScatterPlotVisualTypeDef = TypedDict(
     "ScatterPlotVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[ScatterPlotConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+InsightVisualOutputTypeDef = TypedDict(
+    "InsightVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "DataSetIdentifier": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "InsightConfiguration": NotRequired[InsightConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 InsightVisualTypeDef = TypedDict(
     "InsightVisualTypeDef",
     {
         "VisualId": str,
         "DataSetIdentifier": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "InsightConfiguration": NotRequired[InsightConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+TreeMapVisualOutputTypeDef = TypedDict(
+    "TreeMapVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[TreeMapConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 TreeMapVisualTypeDef = TypedDict(
     "TreeMapVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[TreeMapConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+WaterfallVisualOutputTypeDef = TypedDict(
+    "WaterfallVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[WaterfallChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 WaterfallVisualTypeDef = TypedDict(
     "WaterfallVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[WaterfallChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+WordCloudVisualOutputTypeDef = TypedDict(
+    "WordCloudVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[WordCloudChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 WordCloudVisualTypeDef = TypedDict(
     "WordCloudVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[WordCloudChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+TableVisualOutputTypeDef = TypedDict(
+    "TableVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[TableConfigurationOutputTypeDef],
+        "ConditionalFormatting": NotRequired[TableConditionalFormattingOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 TableVisualTypeDef = TypedDict(
     "TableVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[TableConfigurationTypeDef],
         "ConditionalFormatting": NotRequired[TableConditionalFormattingTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+VisualOutputTypeDef = TypedDict(
+    "VisualOutputTypeDef",
+    {
+        "TableVisual": NotRequired[TableVisualOutputTypeDef],
+        "PivotTableVisual": NotRequired[PivotTableVisualOutputTypeDef],
+        "BarChartVisual": NotRequired[BarChartVisualOutputTypeDef],
+        "KPIVisual": NotRequired[KPIVisualOutputTypeDef],
+        "PieChartVisual": NotRequired[PieChartVisualOutputTypeDef],
+        "GaugeChartVisual": NotRequired[GaugeChartVisualOutputTypeDef],
+        "LineChartVisual": NotRequired[LineChartVisualOutputTypeDef],
+        "HeatMapVisual": NotRequired[HeatMapVisualOutputTypeDef],
+        "TreeMapVisual": NotRequired[TreeMapVisualOutputTypeDef],
+        "GeospatialMapVisual": NotRequired[GeospatialMapVisualOutputTypeDef],
+        "FilledMapVisual": NotRequired[FilledMapVisualOutputTypeDef],
+        "FunnelChartVisual": NotRequired[FunnelChartVisualOutputTypeDef],
+        "ScatterPlotVisual": NotRequired[ScatterPlotVisualOutputTypeDef],
+        "ComboChartVisual": NotRequired[ComboChartVisualOutputTypeDef],
+        "BoxPlotVisual": NotRequired[BoxPlotVisualOutputTypeDef],
+        "WaterfallVisual": NotRequired[WaterfallVisualOutputTypeDef],
+        "HistogramVisual": NotRequired[HistogramVisualOutputTypeDef],
+        "WordCloudVisual": NotRequired[WordCloudVisualOutputTypeDef],
+        "InsightVisual": NotRequired[InsightVisualOutputTypeDef],
+        "SankeyDiagramVisual": NotRequired[SankeyDiagramVisualOutputTypeDef],
+        "CustomContentVisual": NotRequired[CustomContentVisualOutputTypeDef],
+        "EmptyVisual": NotRequired[EmptyVisualOutputTypeDef],
+        "RadarChartVisual": NotRequired[RadarChartVisualOutputTypeDef],
+    },
+)
 VisualTypeDef = TypedDict(
     "VisualTypeDef",
     {
         "TableVisual": NotRequired[TableVisualTypeDef],
         "PivotTableVisual": NotRequired[PivotTableVisualTypeDef],
         "BarChartVisual": NotRequired[BarChartVisualTypeDef],
         "KPIVisual": NotRequired[KPIVisualTypeDef],
@@ -11357,14 +14720,30 @@
         "InsightVisual": NotRequired[InsightVisualTypeDef],
         "SankeyDiagramVisual": NotRequired[SankeyDiagramVisualTypeDef],
         "CustomContentVisual": NotRequired[CustomContentVisualTypeDef],
         "EmptyVisual": NotRequired[EmptyVisualTypeDef],
         "RadarChartVisual": NotRequired[RadarChartVisualTypeDef],
     },
 )
+SheetDefinitionOutputTypeDef = TypedDict(
+    "SheetDefinitionOutputTypeDef",
+    {
+        "SheetId": str,
+        "Title": NotRequired[str],
+        "Description": NotRequired[str],
+        "Name": NotRequired[str],
+        "ParameterControls": NotRequired[List[ParameterControlOutputTypeDef]],
+        "FilterControls": NotRequired[List[FilterControlOutputTypeDef]],
+        "Visuals": NotRequired[List[VisualOutputTypeDef]],
+        "TextBoxes": NotRequired[List[SheetTextBoxTypeDef]],
+        "Layouts": NotRequired[List[LayoutOutputTypeDef]],
+        "SheetControlLayouts": NotRequired[List[SheetControlLayoutOutputTypeDef]],
+        "ContentType": NotRequired[SheetContentTypeType],
+    },
+)
 SheetDefinitionTypeDef = TypedDict(
     "SheetDefinitionTypeDef",
     {
         "SheetId": str,
         "Title": NotRequired[str],
         "Description": NotRequired[str],
         "Name": NotRequired[str],
@@ -11373,14 +14752,53 @@
         "Visuals": NotRequired[Sequence[VisualTypeDef]],
         "TextBoxes": NotRequired[Sequence[SheetTextBoxTypeDef]],
         "Layouts": NotRequired[Sequence[LayoutTypeDef]],
         "SheetControlLayouts": NotRequired[Sequence[SheetControlLayoutTypeDef]],
         "ContentType": NotRequired[SheetContentTypeType],
     },
 )
+AnalysisDefinitionOutputTypeDef = TypedDict(
+    "AnalysisDefinitionOutputTypeDef",
+    {
+        "DataSetIdentifierDeclarations": List[DataSetIdentifierDeclarationTypeDef],
+        "Sheets": NotRequired[List[SheetDefinitionOutputTypeDef]],
+        "CalculatedFields": NotRequired[List[CalculatedFieldTypeDef]],
+        "ParameterDeclarations": NotRequired[List[ParameterDeclarationOutputTypeDef]],
+        "FilterGroups": NotRequired[List[FilterGroupOutputTypeDef]],
+        "ColumnConfigurations": NotRequired[List[ColumnConfigurationOutputTypeDef]],
+        "AnalysisDefaults": NotRequired[AnalysisDefaultsTypeDef],
+        "Options": NotRequired[AssetOptionsTypeDef],
+    },
+)
+DashboardVersionDefinitionOutputTypeDef = TypedDict(
+    "DashboardVersionDefinitionOutputTypeDef",
+    {
+        "DataSetIdentifierDeclarations": List[DataSetIdentifierDeclarationTypeDef],
+        "Sheets": NotRequired[List[SheetDefinitionOutputTypeDef]],
+        "CalculatedFields": NotRequired[List[CalculatedFieldTypeDef]],
+        "ParameterDeclarations": NotRequired[List[ParameterDeclarationOutputTypeDef]],
+        "FilterGroups": NotRequired[List[FilterGroupOutputTypeDef]],
+        "ColumnConfigurations": NotRequired[List[ColumnConfigurationOutputTypeDef]],
+        "AnalysisDefaults": NotRequired[AnalysisDefaultsTypeDef],
+        "Options": NotRequired[AssetOptionsTypeDef],
+    },
+)
+TemplateVersionDefinitionOutputTypeDef = TypedDict(
+    "TemplateVersionDefinitionOutputTypeDef",
+    {
+        "DataSetConfigurations": List[DataSetConfigurationOutputTypeDef],
+        "Sheets": NotRequired[List[SheetDefinitionOutputTypeDef]],
+        "CalculatedFields": NotRequired[List[CalculatedFieldTypeDef]],
+        "ParameterDeclarations": NotRequired[List[ParameterDeclarationOutputTypeDef]],
+        "FilterGroups": NotRequired[List[FilterGroupOutputTypeDef]],
+        "ColumnConfigurations": NotRequired[List[ColumnConfigurationOutputTypeDef]],
+        "AnalysisDefaults": NotRequired[AnalysisDefaultsTypeDef],
+        "Options": NotRequired[AssetOptionsTypeDef],
+    },
+)
 AnalysisDefinitionTypeDef = TypedDict(
     "AnalysisDefinitionTypeDef",
     {
         "DataSetIdentifierDeclarations": Sequence[DataSetIdentifierDeclarationTypeDef],
         "Sheets": NotRequired[Sequence[SheetDefinitionTypeDef]],
         "CalculatedFields": NotRequired[Sequence[CalculatedFieldTypeDef]],
         "ParameterDeclarations": NotRequired[Sequence[ParameterDeclarationTypeDef]],
@@ -11412,44 +14830,74 @@
         "ParameterDeclarations": NotRequired[Sequence[ParameterDeclarationTypeDef]],
         "FilterGroups": NotRequired[Sequence[FilterGroupTypeDef]],
         "ColumnConfigurations": NotRequired[Sequence[ColumnConfigurationTypeDef]],
         "AnalysisDefaults": NotRequired[AnalysisDefaultsTypeDef],
         "Options": NotRequired[AssetOptionsTypeDef],
     },
 )
+DescribeAnalysisDefinitionResponseTypeDef = TypedDict(
+    "DescribeAnalysisDefinitionResponseTypeDef",
+    {
+        "AnalysisId": str,
+        "Name": str,
+        "Errors": List[AnalysisErrorTypeDef],
+        "ResourceStatus": ResourceStatusType,
+        "ThemeArn": str,
+        "Definition": AnalysisDefinitionOutputTypeDef,
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeDashboardDefinitionResponseTypeDef = TypedDict(
+    "DescribeDashboardDefinitionResponseTypeDef",
+    {
+        "DashboardId": str,
+        "Errors": List[DashboardErrorTypeDef],
+        "Name": str,
+        "ResourceStatus": ResourceStatusType,
+        "ThemeArn": str,
+        "Definition": DashboardVersionDefinitionOutputTypeDef,
+        "Status": int,
+        "RequestId": str,
+        "DashboardPublishOptions": DashboardPublishOptionsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeTemplateDefinitionResponseTypeDef = TypedDict(
+    "DescribeTemplateDefinitionResponseTypeDef",
+    {
+        "Name": str,
+        "TemplateId": str,
+        "Errors": List[TemplateErrorTypeDef],
+        "ResourceStatus": ResourceStatusType,
+        "ThemeArn": str,
+        "Definition": TemplateVersionDefinitionOutputTypeDef,
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+AnalysisDefinitionUnionTypeDef = Union[AnalysisDefinitionTypeDef, AnalysisDefinitionOutputTypeDef]
 CreateAnalysisRequestRequestTypeDef = TypedDict(
     "CreateAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
         "Name": str,
         "Parameters": NotRequired[ParametersTypeDef],
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
+        "Permissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
         "SourceEntity": NotRequired[AnalysisSourceEntityTypeDef],
         "ThemeArn": NotRequired[str],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "Definition": NotRequired[AnalysisDefinitionTypeDef],
         "ValidationStrategy": NotRequired[ValidationStrategyTypeDef],
         "FolderArns": NotRequired[Sequence[str]],
     },
 )
-DescribeAnalysisDefinitionResponseTypeDef = TypedDict(
-    "DescribeAnalysisDefinitionResponseTypeDef",
-    {
-        "AnalysisId": str,
-        "Name": str,
-        "Errors": List[AnalysisErrorTypeDef],
-        "ResourceStatus": ResourceStatusType,
-        "ThemeArn": str,
-        "Definition": AnalysisDefinitionTypeDef,
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 UpdateAnalysisRequestRequestTypeDef = TypedDict(
     "UpdateAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
         "Name": str,
         "Parameters": NotRequired[ParametersTypeDef],
@@ -11462,42 +14910,30 @@
 CreateDashboardRequestRequestTypeDef = TypedDict(
     "CreateDashboardRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DashboardId": str,
         "Name": str,
         "Parameters": NotRequired[ParametersTypeDef],
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
+        "Permissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
         "SourceEntity": NotRequired[DashboardSourceEntityTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "VersionDescription": NotRequired[str],
         "DashboardPublishOptions": NotRequired[DashboardPublishOptionsTypeDef],
         "ThemeArn": NotRequired[str],
         "Definition": NotRequired[DashboardVersionDefinitionTypeDef],
         "ValidationStrategy": NotRequired[ValidationStrategyTypeDef],
         "FolderArns": NotRequired[Sequence[str]],
         "LinkSharingConfiguration": NotRequired[LinkSharingConfigurationTypeDef],
         "LinkEntities": NotRequired[Sequence[str]],
     },
 )
-DescribeDashboardDefinitionResponseTypeDef = TypedDict(
-    "DescribeDashboardDefinitionResponseTypeDef",
-    {
-        "DashboardId": str,
-        "Errors": List[DashboardErrorTypeDef],
-        "Name": str,
-        "ResourceStatus": ResourceStatusType,
-        "ThemeArn": str,
-        "Definition": DashboardVersionDefinitionTypeDef,
-        "Status": int,
-        "RequestId": str,
-        "DashboardPublishOptions": DashboardPublishOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+DashboardVersionDefinitionUnionTypeDef = Union[
+    DashboardVersionDefinitionTypeDef, DashboardVersionDefinitionOutputTypeDef
+]
 UpdateDashboardRequestRequestTypeDef = TypedDict(
     "UpdateDashboardRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DashboardId": str,
         "Name": str,
         "SourceEntity": NotRequired[DashboardSourceEntityTypeDef],
@@ -11511,36 +14947,25 @@
 )
 CreateTemplateRequestRequestTypeDef = TypedDict(
     "CreateTemplateRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TemplateId": str,
         "Name": NotRequired[str],
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
+        "Permissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
         "SourceEntity": NotRequired[TemplateSourceEntityTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "VersionDescription": NotRequired[str],
         "Definition": NotRequired[TemplateVersionDefinitionTypeDef],
         "ValidationStrategy": NotRequired[ValidationStrategyTypeDef],
     },
 )
-DescribeTemplateDefinitionResponseTypeDef = TypedDict(
-    "DescribeTemplateDefinitionResponseTypeDef",
-    {
-        "Name": str,
-        "TemplateId": str,
-        "Errors": List[TemplateErrorTypeDef],
-        "ResourceStatus": ResourceStatusType,
-        "ThemeArn": str,
-        "Definition": TemplateVersionDefinitionTypeDef,
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+TemplateVersionDefinitionUnionTypeDef = Union[
+    TemplateVersionDefinitionTypeDef, TemplateVersionDefinitionOutputTypeDef
+]
 UpdateTemplateRequestRequestTypeDef = TypedDict(
     "UpdateTemplateRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TemplateId": str,
         "SourceEntity": NotRequired[TemplateSourceEntityTypeDef],
         "VersionDescription": NotRequired[str],
```

### Comparing `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight/type_defs.pyi` & `mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight/type_defs.pyi`

 * *Files 17% similar despite different names*

```diff
@@ -132,14 +132,15 @@
     PivotTableFieldCollapseStateType,
     PivotTableMetricPlacementType,
     PivotTableRowsLayoutType,
     PivotTableSubtotalLevelType,
     PrimaryValueDisplayTypeType,
     PropertyRoleType,
     PropertyUsageType,
+    PurchaseModeType,
     RadarChartAxesRangeScaleType,
     RadarChartShapeType,
     ReferenceLineLabelHorizontalPositionType,
     ReferenceLineLabelVerticalPositionType,
     ReferenceLinePatternTypeType,
     ReferenceLineSeriesTypeType,
     ReferenceLineValueLabelRelativePositionType,
@@ -238,44 +239,55 @@
     "AnalysisSearchFilterTypeDef",
     "DataSetReferenceTypeDef",
     "AnalysisSummaryTypeDef",
     "SheetTypeDef",
     "AnchorDateConfigurationTypeDef",
     "AnonymousUserDashboardEmbeddingConfigurationTypeDef",
     "DashboardVisualIdTypeDef",
+    "AnonymousUserGenerativeQnAEmbeddingConfigurationTypeDef",
     "AnonymousUserQSearchBarEmbeddingConfigurationTypeDef",
     "ArcAxisDisplayRangeTypeDef",
     "ArcConfigurationTypeDef",
     "ArcOptionsTypeDef",
+    "AssetBundleExportJobAnalysisOverridePropertiesOutputTypeDef",
+    "AssetBundleExportJobDashboardOverridePropertiesOutputTypeDef",
+    "AssetBundleExportJobDataSetOverridePropertiesOutputTypeDef",
+    "AssetBundleExportJobDataSourceOverridePropertiesOutputTypeDef",
+    "AssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef",
+    "AssetBundleExportJobResourceIdOverrideConfigurationTypeDef",
+    "AssetBundleExportJobThemeOverridePropertiesOutputTypeDef",
+    "AssetBundleExportJobVPCConnectionOverridePropertiesOutputTypeDef",
     "AssetBundleExportJobAnalysisOverridePropertiesTypeDef",
     "AssetBundleExportJobDashboardOverridePropertiesTypeDef",
     "AssetBundleExportJobDataSetOverridePropertiesTypeDef",
     "AssetBundleExportJobDataSourceOverridePropertiesTypeDef",
     "AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef",
-    "AssetBundleExportJobResourceIdOverrideConfigurationTypeDef",
     "AssetBundleExportJobThemeOverridePropertiesTypeDef",
     "AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef",
     "AssetBundleExportJobErrorTypeDef",
     "AssetBundleExportJobSummaryTypeDef",
     "AssetBundleExportJobValidationStrategyTypeDef",
     "AssetBundleExportJobWarningTypeDef",
     "AssetBundleImportJobAnalysisOverrideParametersTypeDef",
+    "AssetBundleResourcePermissionsOutputTypeDef",
     "AssetBundleResourcePermissionsTypeDef",
     "TagTypeDef",
     "AssetBundleImportJobDashboardOverrideParametersTypeDef",
     "AssetBundleImportJobDataSetOverrideParametersTypeDef",
     "AssetBundleImportJobDataSourceCredentialPairTypeDef",
     "SslPropertiesTypeDef",
     "VpcConnectionPropertiesTypeDef",
     "AssetBundleImportJobErrorTypeDef",
-    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
+    "AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef",
     "AssetBundleImportJobResourceIdOverrideConfigurationTypeDef",
     "AssetBundleImportJobThemeOverrideParametersTypeDef",
+    "AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef",
     "AssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
     "AssetBundleImportJobOverrideValidationStrategyTypeDef",
+    "TimestampTypeDef",
     "AssetBundleImportJobSummaryTypeDef",
     "AssetBundleImportJobWarningTypeDef",
     "AssetBundleImportSourceDescriptionTypeDef",
     "BlobTypeDef",
     "AthenaParametersTypeDef",
     "AuroraParametersTypeDef",
     "AuroraPostgreSqlParametersTypeDef",
@@ -295,38 +307,43 @@
     "PaginationConfigurationTypeDef",
     "CalculatedColumnTypeDef",
     "CalculatedMeasureFieldTypeDef",
     "CancelIngestionRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "CastColumnTypeOperationTypeDef",
     "CustomFilterConfigurationTypeDef",
+    "CustomFilterListConfigurationOutputTypeDef",
+    "FilterListConfigurationOutputTypeDef",
     "CustomFilterListConfigurationTypeDef",
     "FilterListConfigurationTypeDef",
+    "CellValueSynonymOutputTypeDef",
     "CellValueSynonymTypeDef",
     "SimpleClusterMarkerTypeDef",
+    "CollectiveConstantOutputTypeDef",
     "CollectiveConstantTypeDef",
     "DataColorTypeDef",
     "CustomColorTypeDef",
     "ColumnDescriptionTypeDef",
     "ColumnGroupColumnSchemaTypeDef",
+    "GeoSpatialColumnGroupOutputTypeDef",
     "GeoSpatialColumnGroupTypeDef",
+    "ColumnLevelPermissionRuleOutputTypeDef",
     "ColumnLevelPermissionRuleTypeDef",
     "ColumnSchemaTypeDef",
+    "ComparativeOrderOutputTypeDef",
     "ComparativeOrderTypeDef",
     "ConditionalFormattingSolidColorTypeDef",
     "ConditionalFormattingCustomIconOptionsTypeDef",
     "ConditionalFormattingIconDisplayConfigurationTypeDef",
     "ConditionalFormattingIconSetTypeDef",
     "ContextMenuOptionTypeDef",
     "CreateAccountSubscriptionRequestRequestTypeDef",
     "SignupResponseTypeDef",
-    "ResourcePermissionTypeDef",
     "ValidationStrategyTypeDef",
     "DataSetUsageConfigurationTypeDef",
-    "FieldFolderTypeDef",
     "RowLevelPermissionDataSetTypeDef",
     "CreateFolderMembershipRequestRequestTypeDef",
     "FolderMemberTypeDef",
     "CreateGroupMembershipRequestRequestTypeDef",
     "GroupMemberTypeDef",
     "CreateGroupRequestRequestTypeDef",
     "GroupTypeDef",
@@ -339,15 +356,15 @@
     "ThemeAliasTypeDef",
     "DecimalPlacesConfigurationTypeDef",
     "NegativeValueConfigurationTypeDef",
     "NullValueFormatConfigurationTypeDef",
     "LocalNavigationConfigurationTypeDef",
     "CustomActionURLOperationTypeDef",
     "CustomNarrativeOptionsTypeDef",
-    "TimestampTypeDef",
+    "CustomParameterValuesOutputTypeDef",
     "InputColumnTypeDef",
     "DataPointDrillUpDownOptionTypeDef",
     "DataPointMenuLabelOptionTypeDef",
     "DataPointTooltipOptionTypeDef",
     "ExportToCSVOptionTypeDef",
     "ExportWithHiddenFieldsOptionTypeDef",
     "SheetControlsOptionTypeDef",
@@ -356,22 +373,24 @@
     "VisualMenuOptionTypeDef",
     "DashboardSearchFilterTypeDef",
     "DashboardSummaryTypeDef",
     "DashboardVersionSummaryTypeDef",
     "ExportHiddenFieldsOptionTypeDef",
     "DataAggregationTypeDef",
     "DataBarsOptionsTypeDef",
+    "DataColorPaletteOutputTypeDef",
     "DataColorPaletteTypeDef",
     "DataPathLabelTypeTypeDef",
     "FieldLabelTypeTypeDef",
     "MaximumLabelTypeTypeDef",
     "MinimumLabelTypeTypeDef",
     "RangeEndsLabelTypeTypeDef",
     "DataPathTypeTypeDef",
     "DataSetSearchFilterTypeDef",
+    "FieldFolderOutputTypeDef",
     "OutputColumnTypeDef",
     "DataSourceErrorInfoTypeDef",
     "DatabricksParametersTypeDef",
     "ExasolParametersTypeDef",
     "JiraParametersTypeDef",
     "MariaDbParametersTypeDef",
     "MySqlParametersTypeDef",
@@ -385,20 +404,26 @@
     "SqlServerParametersTypeDef",
     "StarburstParametersTypeDef",
     "TeradataParametersTypeDef",
     "TrinoParametersTypeDef",
     "TwitterParametersTypeDef",
     "DataSourceSearchFilterTypeDef",
     "DataSourceSummaryTypeDef",
+    "DateTimeDatasetParameterDefaultValuesOutputTypeDef",
     "RollingDateConfigurationTypeDef",
+    "DateTimeValueWhenUnsetConfigurationOutputTypeDef",
     "MappedDataSetParameterTypeDef",
+    "DateTimeParameterOutputTypeDef",
     "SheetControlInfoIconLabelOptionsTypeDef",
+    "DecimalDatasetParameterDefaultValuesOutputTypeDef",
     "DecimalDatasetParameterDefaultValuesTypeDef",
     "DecimalValueWhenUnsetConfigurationTypeDef",
+    "DecimalParameterOutputTypeDef",
     "DecimalParameterTypeDef",
+    "FilterSelectableValuesOutputTypeDef",
     "FilterSelectableValuesTypeDef",
     "DeleteAccountCustomizationRequestRequestTypeDef",
     "DeleteAccountSubscriptionRequestRequestTypeDef",
     "DeleteAnalysisRequestRequestTypeDef",
     "DeleteDashboardRequestRequestTypeDef",
     "DeleteDataSetRefreshPropertiesRequestRequestTypeDef",
     "DeleteDataSetRequestRequestTypeDef",
@@ -423,14 +448,15 @@
     "DeleteUserRequestRequestTypeDef",
     "DeleteVPCConnectionRequestRequestTypeDef",
     "DescribeAccountCustomizationRequestRequestTypeDef",
     "DescribeAccountSettingsRequestRequestTypeDef",
     "DescribeAccountSubscriptionRequestRequestTypeDef",
     "DescribeAnalysisDefinitionRequestRequestTypeDef",
     "DescribeAnalysisPermissionsRequestRequestTypeDef",
+    "ResourcePermissionOutputTypeDef",
     "DescribeAnalysisRequestRequestTypeDef",
     "DescribeAssetBundleExportJobRequestRequestTypeDef",
     "DescribeAssetBundleImportJobRequestRequestTypeDef",
     "DescribeDashboardDefinitionRequestRequestTypeDef",
     "DescribeDashboardPermissionsRequestRequestTypeDef",
     "DescribeDashboardRequestRequestTypeDef",
     "DescribeDashboardSnapshotJobRequestRequestTypeDef",
@@ -439,15 +465,15 @@
     "DescribeDataSetPermissionsRequestRequestTypeDef",
     "DescribeDataSetRefreshPropertiesRequestRequestTypeDef",
     "DescribeDataSetRequestRequestTypeDef",
     "DescribeDataSourcePermissionsRequestRequestTypeDef",
     "DescribeDataSourceRequestRequestTypeDef",
     "PaginatorConfigTypeDef",
     "DescribeFolderPermissionsRequestRequestTypeDef",
-    "ResourcePermissionPaginatorTypeDef",
+    "ResourcePermissionExtraOutputTypeDef",
     "DescribeFolderRequestRequestTypeDef",
     "DescribeFolderResolvedPermissionsRequestRequestTypeDef",
     "FolderTypeDef",
     "DescribeGroupMembershipRequestRequestTypeDef",
     "DescribeGroupRequestRequestTypeDef",
     "DescribeIAMPolicyAssignmentRequestRequestTypeDef",
     "IAMPolicyAssignmentTypeDef",
@@ -463,38 +489,44 @@
     "DescribeThemeAliasRequestRequestTypeDef",
     "DescribeThemePermissionsRequestRequestTypeDef",
     "DescribeThemeRequestRequestTypeDef",
     "DescribeTopicPermissionsRequestRequestTypeDef",
     "DescribeTopicRefreshRequestRequestTypeDef",
     "TopicRefreshDetailsTypeDef",
     "DescribeTopicRefreshScheduleRequestRequestTypeDef",
+    "TopicRefreshScheduleOutputTypeDef",
     "DescribeTopicRequestRequestTypeDef",
     "DescribeUserRequestRequestTypeDef",
     "UserTypeDef",
     "DescribeVPCConnectionRequestRequestTypeDef",
     "NegativeFormatTypeDef",
     "DonutCenterOptionsTypeDef",
     "ListControlSelectAllOptionsTypeDef",
     "ErrorInfoTypeDef",
     "ExcludePeriodConfigurationTypeDef",
+    "FieldFolderTypeDef",
     "FieldSortTypeDef",
     "FieldTooltipItemTypeDef",
     "GeospatialMapStyleOptionsTypeDef",
+    "SameSheetTargetVisualConfigurationOutputTypeDef",
     "SameSheetTargetVisualConfigurationTypeDef",
     "FilterOperationTypeDef",
     "FolderSearchFilterTypeDef",
     "FolderSummaryTypeDef",
     "FontSizeTypeDef",
     "FontWeightTypeDef",
     "FontTypeDef",
     "TimeBasedForecastPropertiesTypeDef",
+    "WhatIfPointScenarioOutputTypeDef",
+    "WhatIfRangeScenarioOutputTypeDef",
     "FreeFormLayoutScreenCanvasSizeOptionsTypeDef",
     "FreeFormLayoutElementBackgroundStyleTypeDef",
     "FreeFormLayoutElementBorderStyleTypeDef",
     "LoadingAnimationTypeDef",
+    "GaugeChartColorConfigurationTypeDef",
     "SessionTagTypeDef",
     "GeospatialCoordinateBoundsTypeDef",
     "GeospatialHeatmapDataColorTypeDef",
     "GetDashboardEmbedUrlRequestRequestTypeDef",
     "GetSessionEmbedUrlRequestRequestTypeDef",
     "TableBorderOptionsTypeDef",
     "GradientStopTypeDef",
@@ -503,26 +535,29 @@
     "GroupSearchFilterTypeDef",
     "GutterStyleTypeDef",
     "IAMPolicyAssignmentSummaryTypeDef",
     "IdentityCenterConfigurationTypeDef",
     "LookbackWindowTypeDef",
     "QueueInfoTypeDef",
     "RowInfoTypeDef",
+    "IntegerDatasetParameterDefaultValuesOutputTypeDef",
     "IntegerDatasetParameterDefaultValuesTypeDef",
     "IntegerValueWhenUnsetConfigurationTypeDef",
+    "IntegerParameterOutputTypeDef",
     "IntegerParameterTypeDef",
     "JoinKeyPropertiesTypeDef",
     "KPISparklineOptionsTypeDef",
     "ProgressBarOptionsTypeDef",
     "SecondaryValueOptionsTypeDef",
     "TrendArrowOptionsTypeDef",
     "KPIVisualStandardLayoutTypeDef",
     "LineChartLineStyleSettingsTypeDef",
     "LineChartMarkerStyleSettingsTypeDef",
     "MissingDataConfigurationTypeDef",
+    "ResourcePermissionTypeDef",
     "ListAnalysesRequestRequestTypeDef",
     "ListAssetBundleExportJobsRequestRequestTypeDef",
     "ListAssetBundleImportJobsRequestRequestTypeDef",
     "ListControlSearchOptionsTypeDef",
     "ListDashboardVersionsRequestRequestTypeDef",
     "ListDashboardsRequestRequestTypeDef",
     "ListDataSetsRequestRequestTypeDef",
@@ -555,133 +590,177 @@
     "TopicSummaryTypeDef",
     "ListUserGroupsRequestRequestTypeDef",
     "ListUsersRequestRequestTypeDef",
     "ListVPCConnectionsRequestRequestTypeDef",
     "LongFormatTextTypeDef",
     "ManifestFileLocationTypeDef",
     "MarginStyleTypeDef",
+    "NamedEntityDefinitionMetricOutputTypeDef",
     "NamedEntityDefinitionMetricTypeDef",
     "NamespaceErrorTypeDef",
     "NetworkInterfaceTypeDef",
+    "NewDefaultValuesOutputTypeDef",
     "NumericRangeFilterValueTypeDef",
     "ThousandSeparatorOptionsTypeDef",
     "PercentileAggregationTypeDef",
+    "StringParameterOutputTypeDef",
     "StringParameterTypeDef",
     "PercentVisibleRangeTypeDef",
     "PivotTableConditionalFormattingScopeTypeDef",
     "PivotTablePaginatedReportOptionsTypeDef",
     "PivotTableFieldOptionTypeDef",
     "PivotTableFieldSubtotalOptionsTypeDef",
     "PivotTableRowsLabelOptionsTypeDef",
+    "RowAlternateColorOptionsOutputTypeDef",
     "RowAlternateColorOptionsTypeDef",
+    "ProjectOperationOutputTypeDef",
     "ProjectOperationTypeDef",
     "RadarChartAreaStyleSettingsTypeDef",
     "RangeConstantTypeDef",
-    "RedshiftIAMParametersPaginatorTypeDef",
+    "RedshiftIAMParametersExtraOutputTypeDef",
+    "RedshiftIAMParametersOutputTypeDef",
     "RedshiftIAMParametersTypeDef",
     "ReferenceLineCustomLabelConfigurationTypeDef",
     "ReferenceLineStaticDataConfigurationTypeDef",
     "ReferenceLineStyleConfigurationTypeDef",
     "ScheduleRefreshOnEntityTypeDef",
     "StatePersistenceConfigurationsTypeDef",
+    "RegisteredUserGenerativeQnAEmbeddingConfigurationTypeDef",
     "RegisteredUserQSearchBarEmbeddingConfigurationTypeDef",
     "RenameColumnOperationTypeDef",
     "RestoreAnalysisRequestRequestTypeDef",
     "RowLevelPermissionTagRuleTypeDef",
     "S3BucketConfigurationTypeDef",
     "UploadSettingsTypeDef",
     "SectionAfterPageBreakTypeDef",
     "SpacingTypeDef",
+    "SheetVisualScopingConfigurationOutputTypeDef",
     "SheetVisualScopingConfigurationTypeDef",
+    "SemanticEntityTypeOutputTypeDef",
     "SemanticEntityTypeTypeDef",
+    "SemanticTypeOutputTypeDef",
     "SemanticTypeTypeDef",
     "SheetTextBoxTypeDef",
     "SheetElementConfigurationOverridesTypeDef",
     "ShortFormatTextTypeDef",
     "YAxisOptionsTypeDef",
     "SmallMultiplesAxisPropertiesTypeDef",
     "SnapshotAnonymousUserRedactedTypeDef",
+    "SnapshotFileSheetSelectionOutputTypeDef",
     "SnapshotFileSheetSelectionTypeDef",
     "SnapshotJobResultErrorInfoTypeDef",
+    "StringDatasetParameterDefaultValuesOutputTypeDef",
     "StringDatasetParameterDefaultValuesTypeDef",
     "StringValueWhenUnsetConfigurationTypeDef",
     "TableStyleTargetTypeDef",
     "TableCellImageSizingConfigurationTypeDef",
     "TablePaginatedReportOptionsTypeDef",
     "TableFieldCustomIconContentTypeDef",
+    "TablePinnedFieldOptionsOutputTypeDef",
     "TablePinnedFieldOptionsTypeDef",
     "TemplateSourceTemplateTypeDef",
     "TextControlPlaceholderOptionsTypeDef",
     "UIColorPaletteTypeDef",
     "ThemeErrorTypeDef",
     "TopicSingularFilterConstantTypeDef",
     "TotalAggregationFunctionTypeDef",
+    "UntagColumnOperationOutputTypeDef",
     "UntagColumnOperationTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateAccountSettingsRequestRequestTypeDef",
     "UpdateDashboardLinksRequestRequestTypeDef",
     "UpdateDashboardPublishedVersionRequestRequestTypeDef",
     "UpdateFolderRequestRequestTypeDef",
     "UpdateGroupRequestRequestTypeDef",
     "UpdateIAMPolicyAssignmentRequestRequestTypeDef",
     "UpdateIdentityPropagationConfigRequestRequestTypeDef",
     "UpdateIpRestrictionRequestRequestTypeDef",
     "UpdatePublicSharingSettingsRequestRequestTypeDef",
     "UpdateRoleCustomPermissionRequestRequestTypeDef",
+    "UpdateSPICECapacityConfigurationRequestRequestTypeDef",
     "UpdateTemplateAliasRequestRequestTypeDef",
     "UpdateThemeAliasRequestRequestTypeDef",
     "UpdateUserRequestRequestTypeDef",
     "UpdateVPCConnectionRequestRequestTypeDef",
     "WaterfallChartGroupColorConfigurationTypeDef",
     "WaterfallChartOptionsTypeDef",
     "WordCloudOptionsTypeDef",
     "UpdateAccountCustomizationRequestRequestTypeDef",
     "AxisLabelReferenceOptionsTypeDef",
     "CascadingControlSourceTypeDef",
+    "CategoryDrillDownFilterOutputTypeDef",
     "CategoryDrillDownFilterTypeDef",
+    "ContributionAnalysisDefaultOutputTypeDef",
     "ContributionAnalysisDefaultTypeDef",
     "DynamicDefaultValueTypeDef",
+    "FilterOperationSelectedFieldsConfigurationOutputTypeDef",
     "FilterOperationSelectedFieldsConfigurationTypeDef",
     "NumericEqualityDrillDownFilterTypeDef",
+    "ParameterSelectableValuesOutputTypeDef",
     "ParameterSelectableValuesTypeDef",
+    "TimeRangeDrillDownFilterOutputTypeDef",
     "AnalysisErrorTypeDef",
     "DashboardErrorTypeDef",
     "TemplateErrorTypeDef",
     "SearchAnalysesRequestRequestTypeDef",
     "AnalysisSourceTemplateTypeDef",
     "DashboardSourceTemplateTypeDef",
     "TemplateSourceAnalysisTypeDef",
     "AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef",
     "RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef",
     "ArcAxisConfigurationTypeDef",
+    "AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef",
     "AssetBundleCloudFormationOverridePropertyConfigurationTypeDef",
+    "AssetBundleImportJobAnalysisOverridePermissionsOutputTypeDef",
+    "AssetBundleImportJobDataSetOverridePermissionsOutputTypeDef",
+    "AssetBundleImportJobDataSourceOverridePermissionsOutputTypeDef",
+    "AssetBundleImportJobThemeOverridePermissionsOutputTypeDef",
+    "AssetBundleResourceLinkSharingConfigurationOutputTypeDef",
     "AssetBundleImportJobAnalysisOverridePermissionsTypeDef",
     "AssetBundleImportJobDataSetOverridePermissionsTypeDef",
     "AssetBundleImportJobDataSourceOverridePermissionsTypeDef",
     "AssetBundleImportJobThemeOverridePermissionsTypeDef",
     "AssetBundleResourceLinkSharingConfigurationTypeDef",
+    "AssetBundleImportJobAnalysisOverrideTagsOutputTypeDef",
     "AssetBundleImportJobAnalysisOverrideTagsTypeDef",
+    "AssetBundleImportJobDashboardOverrideTagsOutputTypeDef",
     "AssetBundleImportJobDashboardOverrideTagsTypeDef",
+    "AssetBundleImportJobDataSetOverrideTagsOutputTypeDef",
     "AssetBundleImportJobDataSetOverrideTagsTypeDef",
+    "AssetBundleImportJobDataSourceOverrideTagsOutputTypeDef",
     "AssetBundleImportJobDataSourceOverrideTagsTypeDef",
+    "AssetBundleImportJobThemeOverrideTagsOutputTypeDef",
     "AssetBundleImportJobThemeOverrideTagsTypeDef",
+    "AssetBundleImportJobVPCConnectionOverrideTagsOutputTypeDef",
     "AssetBundleImportJobVPCConnectionOverrideTagsTypeDef",
     "CreateAccountCustomizationRequestRequestTypeDef",
     "CreateNamespaceRequestRequestTypeDef",
     "CreateVPCConnectionRequestRequestTypeDef",
     "RegisterUserRequestRequestTypeDef",
     "TagResourceRequestRequestTypeDef",
     "AssetBundleImportJobDataSourceCredentialsTypeDef",
+    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
+    "CustomParameterValuesTypeDef",
+    "DateTimeDatasetParameterDefaultValuesTypeDef",
+    "DateTimeParameterTypeDef",
+    "DateTimeValueWhenUnsetConfigurationTypeDef",
+    "NewDefaultValuesTypeDef",
+    "TimeRangeDrillDownFilterTypeDef",
+    "TopicRefreshScheduleTypeDef",
+    "WhatIfPointScenarioTypeDef",
+    "WhatIfRangeScenarioTypeDef",
     "AssetBundleImportSourceTypeDef",
+    "AxisDisplayRangeOutputTypeDef",
     "AxisDisplayRangeTypeDef",
     "AxisScaleTypeDef",
     "ScatterPlotSortConfigurationTypeDef",
     "HistogramBinOptionsTypeDef",
     "TileStyleTypeDef",
     "BoxPlotOptionsTypeDef",
+    "CreateColumnsOperationOutputTypeDef",
     "CreateColumnsOperationTypeDef",
     "CancelIngestionResponseTypeDef",
     "CreateAccountCustomizationResponseTypeDef",
     "CreateAnalysisResponseTypeDef",
     "CreateDashboardResponseTypeDef",
     "CreateDataSetResponseTypeDef",
     "CreateDataSourceResponseTypeDef",
@@ -759,53 +838,39 @@
     "UpdateFolderResponseTypeDef",
     "UpdateIAMPolicyAssignmentResponseTypeDef",
     "UpdateIdentityPropagationConfigResponseTypeDef",
     "UpdateIpRestrictionResponseTypeDef",
     "UpdatePublicSharingSettingsResponseTypeDef",
     "UpdateRefreshScheduleResponseTypeDef",
     "UpdateRoleCustomPermissionResponseTypeDef",
+    "UpdateSPICECapacityConfigurationResponseTypeDef",
     "UpdateTemplateResponseTypeDef",
     "UpdateThemeResponseTypeDef",
     "UpdateTopicRefreshScheduleResponseTypeDef",
     "UpdateTopicResponseTypeDef",
     "UpdateVPCConnectionResponseTypeDef",
+    "CategoryFilterConfigurationOutputTypeDef",
     "CategoryFilterConfigurationTypeDef",
     "ClusterMarkerTypeDef",
+    "TopicCategoryFilterConstantOutputTypeDef",
     "TopicCategoryFilterConstantTypeDef",
+    "ColorScaleOutputTypeDef",
     "ColorScaleTypeDef",
+    "ColorsConfigurationOutputTypeDef",
     "ColorsConfigurationTypeDef",
     "ColumnTagTypeDef",
+    "ColumnGroupSchemaOutputTypeDef",
     "ColumnGroupSchemaTypeDef",
+    "ColumnGroupOutputTypeDef",
     "ColumnGroupTypeDef",
+    "ColumnLevelPermissionRuleUnionTypeDef",
+    "DataSetSchemaOutputTypeDef",
     "DataSetSchemaTypeDef",
     "ConditionalFormattingCustomIconConditionTypeDef",
     "CreateAccountSubscriptionResponseTypeDef",
-    "CreateFolderRequestRequestTypeDef",
-    "DescribeAnalysisPermissionsResponseTypeDef",
-    "DescribeDataSetPermissionsResponseTypeDef",
-    "DescribeDataSourcePermissionsResponseTypeDef",
-    "DescribeFolderPermissionsResponseTypeDef",
-    "DescribeFolderResolvedPermissionsResponseTypeDef",
-    "DescribeTemplatePermissionsResponseTypeDef",
-    "DescribeThemePermissionsResponseTypeDef",
-    "DescribeTopicPermissionsResponseTypeDef",
-    "LinkSharingConfigurationTypeDef",
-    "UpdateAnalysisPermissionsRequestRequestTypeDef",
-    "UpdateAnalysisPermissionsResponseTypeDef",
-    "UpdateDashboardPermissionsRequestRequestTypeDef",
-    "UpdateDataSetPermissionsRequestRequestTypeDef",
-    "UpdateDataSourcePermissionsRequestRequestTypeDef",
-    "UpdateFolderPermissionsRequestRequestTypeDef",
-    "UpdateFolderPermissionsResponseTypeDef",
-    "UpdateTemplatePermissionsRequestRequestTypeDef",
-    "UpdateTemplatePermissionsResponseTypeDef",
-    "UpdateThemePermissionsRequestRequestTypeDef",
-    "UpdateThemePermissionsResponseTypeDef",
-    "UpdateTopicPermissionsRequestRequestTypeDef",
-    "UpdateTopicPermissionsResponseTypeDef",
     "DataSetSummaryTypeDef",
     "CreateFolderMembershipResponseTypeDef",
     "CreateGroupMembershipResponseTypeDef",
     "DescribeGroupMembershipResponseTypeDef",
     "ListGroupMembershipsResponseTypeDef",
     "CreateGroupResponseTypeDef",
     "DescribeGroupResponseTypeDef",
@@ -818,39 +883,49 @@
     "ListTemplateAliasesResponseTypeDef",
     "UpdateTemplateAliasResponseTypeDef",
     "CreateThemeAliasResponseTypeDef",
     "DescribeThemeAliasResponseTypeDef",
     "ListThemeAliasesResponseTypeDef",
     "UpdateThemeAliasResponseTypeDef",
     "CustomActionNavigationOperationTypeDef",
-    "CustomParameterValuesTypeDef",
-    "DateTimeDatasetParameterDefaultValuesTypeDef",
-    "DateTimeParameterTypeDef",
-    "DateTimeValueWhenUnsetConfigurationTypeDef",
-    "NewDefaultValuesTypeDef",
-    "TimeRangeDrillDownFilterTypeDef",
-    "TopicRefreshScheduleTypeDef",
-    "WhatIfPointScenarioTypeDef",
-    "WhatIfRangeScenarioTypeDef",
+    "CustomValuesConfigurationOutputTypeDef",
+    "CustomSqlOutputTypeDef",
     "CustomSqlTypeDef",
+    "RelationalTableOutputTypeDef",
     "RelationalTableTypeDef",
     "VisualInteractionOptionsTypeDef",
     "SearchDashboardsRequestRequestTypeDef",
     "ListDashboardsResponseTypeDef",
     "SearchDashboardsResponseTypeDef",
     "ListDashboardVersionsResponseTypeDef",
     "DashboardVisualPublishOptionsTypeDef",
     "TableInlineVisualizationTypeDef",
     "DataLabelTypeTypeDef",
     "DataPathValueTypeDef",
     "SearchDataSetsRequestRequestTypeDef",
     "SearchDataSourcesRequestRequestTypeDef",
     "SearchDataSourcesResponseTypeDef",
+    "DateTimeDatasetParameterOutputTypeDef",
+    "TimeRangeFilterValueOutputTypeDef",
     "TimeRangeFilterValueTypeDef",
+    "DecimalDatasetParameterOutputTypeDef",
     "DecimalDatasetParameterTypeDef",
+    "DescribeAnalysisPermissionsResponseTypeDef",
+    "DescribeDataSetPermissionsResponseTypeDef",
+    "DescribeDataSourcePermissionsResponseTypeDef",
+    "DescribeFolderResolvedPermissionsResponseTypeDef",
+    "DescribeTemplatePermissionsResponseTypeDef",
+    "DescribeThemePermissionsResponseTypeDef",
+    "DescribeTopicPermissionsResponseTypeDef",
+    "LinkSharingConfigurationOutputTypeDef",
+    "UpdateAnalysisPermissionsResponseTypeDef",
+    "UpdateFolderPermissionsResponseTypeDef",
+    "UpdateTemplatePermissionsResponseTypeDef",
+    "UpdateThemePermissionsResponseTypeDef",
+    "UpdateTopicPermissionsResponseTypeDef",
     "DescribeFolderPermissionsRequestDescribeFolderPermissionsPaginateTypeDef",
     "DescribeFolderResolvedPermissionsRequestDescribeFolderResolvedPermissionsPaginateTypeDef",
     "ListAnalysesRequestListAnalysesPaginateTypeDef",
     "ListAssetBundleExportJobsRequestListAssetBundleExportJobsPaginateTypeDef",
     "ListAssetBundleImportJobsRequestListAssetBundleImportJobsPaginateTypeDef",
     "ListDashboardVersionsRequestListDashboardVersionsPaginateTypeDef",
     "ListDashboardsRequestListDashboardsPaginateTypeDef",
@@ -872,323 +947,459 @@
     "ListThemesRequestListThemesPaginateTypeDef",
     "ListUserGroupsRequestListUserGroupsPaginateTypeDef",
     "ListUsersRequestListUsersPaginateTypeDef",
     "SearchAnalysesRequestSearchAnalysesPaginateTypeDef",
     "SearchDashboardsRequestSearchDashboardsPaginateTypeDef",
     "SearchDataSetsRequestSearchDataSetsPaginateTypeDef",
     "SearchDataSourcesRequestSearchDataSourcesPaginateTypeDef",
-    "DescribeFolderPermissionsResponsePaginatorTypeDef",
-    "DescribeFolderResolvedPermissionsResponsePaginatorTypeDef",
+    "DescribeFolderPermissionsResponseTypeDef",
     "DescribeFolderResponseTypeDef",
     "DescribeIAMPolicyAssignmentResponseTypeDef",
     "DescribeTopicRefreshResponseTypeDef",
+    "DescribeTopicRefreshScheduleResponseTypeDef",
+    "TopicRefreshScheduleSummaryTypeDef",
     "DescribeUserResponseTypeDef",
     "ListUsersResponseTypeDef",
     "RegisterUserResponseTypeDef",
     "UpdateUserResponseTypeDef",
     "DisplayFormatOptionsTypeDef",
     "DonutOptionsTypeDef",
+    "FieldFolderUnionTypeDef",
+    "FilterOperationTargetVisualsConfigurationOutputTypeDef",
     "FilterOperationTargetVisualsConfigurationTypeDef",
     "SearchFoldersRequestRequestTypeDef",
     "SearchFoldersRequestSearchFoldersPaginateTypeDef",
     "ListFoldersResponseTypeDef",
     "SearchFoldersResponseTypeDef",
     "FontConfigurationTypeDef",
+    "TypographyOutputTypeDef",
     "TypographyTypeDef",
+    "ForecastScenarioOutputTypeDef",
     "FreeFormLayoutCanvasSizeOptionsTypeDef",
     "SnapshotAnonymousUserTypeDef",
     "GeospatialWindowOptionsTypeDef",
+    "GeospatialHeatmapColorScaleOutputTypeDef",
     "GeospatialHeatmapColorScaleTypeDef",
     "TableSideBorderOptionsTypeDef",
+    "GradientColorOutputTypeDef",
     "GradientColorTypeDef",
     "GridLayoutCanvasSizeOptionsTypeDef",
     "SearchGroupsRequestRequestTypeDef",
     "SearchGroupsRequestSearchGroupsPaginateTypeDef",
     "ListIAMPolicyAssignmentsResponseTypeDef",
     "IncrementalRefreshTypeDef",
     "IngestionTypeDef",
+    "IntegerDatasetParameterOutputTypeDef",
     "IntegerDatasetParameterTypeDef",
     "JoinInstructionTypeDef",
     "KPIVisualLayoutOptionsTypeDef",
     "LineChartDefaultSeriesSettingsTypeDef",
     "LineChartSeriesSettingsTypeDef",
+    "LinkSharingConfigurationTypeDef",
+    "ResourcePermissionUnionTypeDef",
     "ListFolderMembersResponseTypeDef",
     "ListTemplateVersionsResponseTypeDef",
     "ListTemplatesResponseTypeDef",
     "ListThemeVersionsResponseTypeDef",
     "ListThemesResponseTypeDef",
     "ListTopicsResponseTypeDef",
     "VisualSubtitleLabelOptionsTypeDef",
     "S3ParametersTypeDef",
     "TileLayoutStyleTypeDef",
+    "NamedEntityDefinitionOutputTypeDef",
     "NamedEntityDefinitionTypeDef",
     "NamespaceInfoV2TypeDef",
     "VPCConnectionSummaryTypeDef",
     "VPCConnectionTypeDef",
+    "OverrideDatasetParameterOperationOutputTypeDef",
     "NumericSeparatorConfigurationTypeDef",
     "NumericalAggregationFunctionTypeDef",
+    "ParametersOutputTypeDef",
     "VisibleRangeOptionsTypeDef",
     "RadarChartSeriesSettingsTypeDef",
     "TopicRangeFilterConstantTypeDef",
-    "RedshiftParametersPaginatorTypeDef",
+    "RedshiftParametersExtraOutputTypeDef",
+    "RedshiftParametersOutputTypeDef",
     "RedshiftParametersTypeDef",
     "RefreshFrequencyTypeDef",
     "RegisteredUserConsoleFeatureConfigurationsTypeDef",
     "RegisteredUserDashboardFeatureConfigurationsTypeDef",
+    "RowLevelPermissionTagConfigurationOutputTypeDef",
     "RowLevelPermissionTagConfigurationTypeDef",
     "SnapshotS3DestinationConfigurationTypeDef",
+    "S3SourceOutputTypeDef",
     "S3SourceTypeDef",
     "SectionPageBreakConfigurationTypeDef",
     "SectionBasedLayoutPaperCanvasSizeOptionsTypeDef",
     "SectionStyleTypeDef",
+    "SelectedSheetsFilterScopeConfigurationOutputTypeDef",
     "SelectedSheetsFilterScopeConfigurationTypeDef",
     "SheetElementRenderingRuleTypeDef",
     "VisualTitleLabelOptionsTypeDef",
     "SingleAxisOptionsTypeDef",
     "SnapshotUserConfigurationRedactedTypeDef",
+    "SnapshotFileOutputTypeDef",
     "SnapshotFileTypeDef",
+    "StringDatasetParameterOutputTypeDef",
     "StringDatasetParameterTypeDef",
     "TableFieldImageConfigurationTypeDef",
     "TopicNumericEqualityFilterTypeDef",
     "TopicRelativeDateFilterTypeDef",
     "TotalAggregationOptionTypeDef",
     "WaterfallChartColorConfigurationTypeDef",
+    "CascadingControlConfigurationOutputTypeDef",
     "CascadingControlConfigurationTypeDef",
+    "DateTimeDefaultValuesOutputTypeDef",
     "DateTimeDefaultValuesTypeDef",
+    "DecimalDefaultValuesOutputTypeDef",
     "DecimalDefaultValuesTypeDef",
+    "IntegerDefaultValuesOutputTypeDef",
     "IntegerDefaultValuesTypeDef",
+    "StringDefaultValuesOutputTypeDef",
     "StringDefaultValuesTypeDef",
+    "DrillDownFilterOutputTypeDef",
     "AnalysisTypeDef",
     "DashboardVersionTypeDef",
     "AnalysisSourceEntityTypeDef",
     "DashboardSourceEntityTypeDef",
     "TemplateSourceEntityTypeDef",
     "AnonymousUserEmbeddingExperienceConfigurationTypeDef",
     "DescribeAssetBundleExportJobResponseTypeDef",
+    "AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef",
     "StartAssetBundleExportJobRequestRequestTypeDef",
+    "AssetBundleImportJobDashboardOverridePermissionsOutputTypeDef",
     "AssetBundleImportJobDashboardOverridePermissionsTypeDef",
+    "AssetBundleImportJobOverrideTagsOutputTypeDef",
     "AssetBundleImportJobOverrideTagsTypeDef",
-    "NumericAxisOptionsTypeDef",
-    "ClusterMarkerConfigurationTypeDef",
-    "TopicCategoryFilterTypeDef",
-    "TagColumnOperationTypeDef",
-    "DataSetConfigurationTypeDef",
-    "ConditionalFormattingIconTypeDef",
-    "DescribeDashboardPermissionsResponseTypeDef",
-    "UpdateDashboardPermissionsResponseTypeDef",
-    "ListDataSetsResponseTypeDef",
-    "SearchDataSetsResponseTypeDef",
     "CustomValuesConfigurationTypeDef",
     "DateTimeDatasetParameterTypeDef",
     "ParametersTypeDef",
     "OverrideDatasetParameterOperationTypeDef",
     "DrillDownFilterTypeDef",
     "CreateTopicRefreshScheduleRequestRequestTypeDef",
-    "DescribeTopicRefreshScheduleResponseTypeDef",
-    "TopicRefreshScheduleSummaryTypeDef",
+    "TopicRefreshScheduleUnionTypeDef",
     "UpdateTopicRefreshScheduleRequestRequestTypeDef",
     "ForecastScenarioTypeDef",
+    "NumericAxisOptionsOutputTypeDef",
+    "NumericAxisOptionsTypeDef",
+    "ClusterMarkerConfigurationTypeDef",
+    "TopicCategoryFilterOutputTypeDef",
+    "TopicCategoryFilterTypeDef",
+    "TagColumnOperationOutputTypeDef",
+    "TagColumnOperationTypeDef",
+    "ColumnGroupUnionTypeDef",
+    "DataSetConfigurationOutputTypeDef",
+    "DataSetConfigurationTypeDef",
+    "ConditionalFormattingIconTypeDef",
+    "ListDataSetsResponseTypeDef",
+    "SearchDataSetsResponseTypeDef",
+    "DestinationParameterValueConfigurationOutputTypeDef",
     "CustomContentConfigurationTypeDef",
     "DashboardPublishOptionsTypeDef",
     "DataPathColorTypeDef",
+    "DataPathSortOutputTypeDef",
     "DataPathSortTypeDef",
+    "PivotTableDataPathOptionOutputTypeDef",
     "PivotTableDataPathOptionTypeDef",
+    "PivotTableFieldCollapseStateTargetOutputTypeDef",
     "PivotTableFieldCollapseStateTargetTypeDef",
+    "DescribeDashboardPermissionsResponseTypeDef",
+    "UpdateDashboardPermissionsResponseTypeDef",
+    "ListTopicRefreshSchedulesResponseTypeDef",
     "DefaultFormattingTypeDef",
+    "CustomActionFilterOperationOutputTypeDef",
     "CustomActionFilterOperationTypeDef",
     "AxisLabelOptionsTypeDef",
+    "DataLabelOptionsOutputTypeDef",
     "DataLabelOptionsTypeDef",
     "FunnelChartDataLabelOptionsTypeDef",
     "LabelOptionsTypeDef",
     "PanelTitleOptionsTypeDef",
     "TableFieldCustomTextContentTypeDef",
+    "ForecastConfigurationOutputTypeDef",
     "DefaultFreeFormLayoutConfigurationTypeDef",
     "SnapshotUserConfigurationTypeDef",
+    "GeospatialHeatmapConfigurationOutputTypeDef",
     "GeospatialHeatmapConfigurationTypeDef",
     "GlobalTableBorderOptionsTypeDef",
+    "ConditionalFormattingGradientColorOutputTypeDef",
     "ConditionalFormattingGradientColorTypeDef",
     "DefaultGridLayoutConfigurationTypeDef",
+    "GridLayoutConfigurationOutputTypeDef",
     "GridLayoutConfigurationTypeDef",
     "RefreshConfigurationTypeDef",
     "DescribeIngestionResponseTypeDef",
     "ListIngestionsResponseTypeDef",
     "LogicalTableSourceTypeDef",
     "DataFieldSeriesItemTypeDef",
     "FieldSeriesItemTypeDef",
+    "LinkSharingConfigurationUnionTypeDef",
+    "CreateFolderRequestRequestTypeDef",
+    "UpdateAnalysisPermissionsRequestRequestTypeDef",
+    "UpdateDashboardPermissionsRequestRequestTypeDef",
+    "UpdateDataSetPermissionsRequestRequestTypeDef",
+    "UpdateDataSourcePermissionsRequestRequestTypeDef",
+    "UpdateFolderPermissionsRequestRequestTypeDef",
+    "UpdateTemplatePermissionsRequestRequestTypeDef",
+    "UpdateThemePermissionsRequestRequestTypeDef",
+    "UpdateTopicPermissionsRequestRequestTypeDef",
     "SheetStyleTypeDef",
+    "TopicNamedEntityOutputTypeDef",
     "TopicNamedEntityTypeDef",
     "DescribeNamespaceResponseTypeDef",
     "ListNamespacesResponseTypeDef",
     "ListVPCConnectionsResponseTypeDef",
     "DescribeVPCConnectionResponseTypeDef",
     "CurrencyDisplayFormatConfigurationTypeDef",
     "NumberDisplayFormatConfigurationTypeDef",
     "PercentageDisplayFormatConfigurationTypeDef",
     "AggregationFunctionTypeDef",
     "ScrollBarOptionsTypeDef",
     "TopicDateRangeFilterTypeDef",
     "TopicNumericRangeFilterTypeDef",
-    "DataSourceParametersPaginatorTypeDef",
+    "DataSourceParametersExtraOutputTypeDef",
+    "DataSourceParametersOutputTypeDef",
     "DataSourceParametersTypeDef",
+    "RefreshScheduleOutputTypeDef",
     "RefreshScheduleTypeDef",
     "RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef",
     "RegisteredUserDashboardEmbeddingConfigurationTypeDef",
+    "RowLevelPermissionTagConfigurationUnionTypeDef",
+    "SnapshotDestinationConfigurationOutputTypeDef",
     "SnapshotDestinationConfigurationTypeDef",
     "SnapshotJobS3ResultTypeDef",
+    "PhysicalTableOutputTypeDef",
     "PhysicalTableTypeDef",
     "SectionBasedLayoutCanvasSizeOptionsTypeDef",
+    "FilterScopeConfigurationOutputTypeDef",
     "FilterScopeConfigurationTypeDef",
+    "FreeFormLayoutElementOutputTypeDef",
     "FreeFormLayoutElementTypeDef",
+    "SnapshotFileGroupOutputTypeDef",
     "SnapshotFileGroupTypeDef",
+    "DatasetParameterOutputTypeDef",
+    "FilterCrossSheetControlOutputTypeDef",
     "FilterCrossSheetControlTypeDef",
+    "DateTimeParameterDeclarationOutputTypeDef",
     "DateTimeParameterDeclarationTypeDef",
+    "DecimalParameterDeclarationOutputTypeDef",
     "DecimalParameterDeclarationTypeDef",
+    "IntegerParameterDeclarationOutputTypeDef",
     "IntegerParameterDeclarationTypeDef",
+    "StringParameterDeclarationOutputTypeDef",
     "StringParameterDeclarationTypeDef",
+    "DateTimeHierarchyOutputTypeDef",
+    "ExplicitHierarchyOutputTypeDef",
+    "PredefinedHierarchyOutputTypeDef",
     "DescribeAnalysisResponseTypeDef",
     "DashboardTypeDef",
     "GenerateEmbedUrlForAnonymousUserRequestRequestTypeDef",
+    "AssetBundleImportJobOverridePermissionsOutputTypeDef",
     "AssetBundleImportJobOverridePermissionsTypeDef",
-    "AxisDataOptionsTypeDef",
-    "TemplateVersionTypeDef",
+    "AssetBundleImportJobOverrideTagsUnionTypeDef",
     "DestinationParameterValueConfigurationTypeDef",
     "DatasetParameterTypeDef",
-    "TransformOperationTypeDef",
+    "ParametersUnionTypeDef",
     "DateTimeHierarchyTypeDef",
     "ExplicitHierarchyTypeDef",
     "PredefinedHierarchyTypeDef",
-    "ListTopicRefreshSchedulesResponseTypeDef",
     "ForecastConfigurationTypeDef",
+    "AxisDataOptionsOutputTypeDef",
+    "AxisDataOptionsTypeDef",
+    "TransformOperationOutputTypeDef",
+    "TransformOperationTypeDef",
+    "TemplateVersionTypeDef",
+    "SetParameterValueConfigurationOutputTypeDef",
+    "VisualPaletteOutputTypeDef",
     "VisualPaletteTypeDef",
+    "PivotTableFieldCollapseStateOptionOutputTypeDef",
     "PivotTableFieldCollapseStateOptionTypeDef",
+    "TopicCalculatedFieldOutputTypeDef",
     "TopicCalculatedFieldTypeDef",
+    "TopicColumnOutputTypeDef",
     "TopicColumnTypeDef",
+    "ChartAxisLabelOptionsOutputTypeDef",
     "ChartAxisLabelOptionsTypeDef",
     "AxisTickLabelOptionsTypeDef",
     "DateTimePickerControlDisplayOptionsTypeDef",
     "DropDownControlDisplayOptionsTypeDef",
     "LegendOptionsTypeDef",
     "ListControlDisplayOptionsTypeDef",
     "RelativeDateTimeControlDisplayOptionsTypeDef",
     "SliderControlDisplayOptionsTypeDef",
     "TextAreaControlDisplayOptionsTypeDef",
     "TextFieldControlDisplayOptionsTypeDef",
     "PanelConfigurationTypeDef",
     "TableFieldLinkContentConfigurationTypeDef",
+    "GeospatialPointStyleOptionsOutputTypeDef",
     "GeospatialPointStyleOptionsTypeDef",
     "TableCellStyleTypeDef",
+    "ConditionalFormattingColorOutputTypeDef",
     "ConditionalFormattingColorTypeDef",
     "DefaultInteractiveLayoutConfigurationTypeDef",
+    "SheetControlLayoutConfigurationOutputTypeDef",
     "SheetControlLayoutConfigurationTypeDef",
     "DataSetRefreshPropertiesTypeDef",
     "SeriesItemTypeDef",
+    "ThemeConfigurationOutputTypeDef",
     "ThemeConfigurationTypeDef",
     "ComparisonFormatConfigurationTypeDef",
     "NumericFormatConfigurationTypeDef",
     "AggregationSortConfigurationTypeDef",
     "ColumnSortTypeDef",
     "ColumnTooltipItemTypeDef",
     "ReferenceLineDynamicDataConfigurationTypeDef",
+    "TopicFilterOutputTypeDef",
     "TopicFilterTypeDef",
-    "DataSourcePaginatorTypeDef",
+    "AssetBundleImportJobDataSourceOverrideParametersOutputTypeDef",
+    "DataSourceTypeDef",
     "AssetBundleImportJobDataSourceOverrideParametersTypeDef",
     "CredentialPairTypeDef",
-    "DataSourceTypeDef",
-    "CreateRefreshScheduleRequestRequestTypeDef",
+    "DataSourceParametersUnionTypeDef",
     "DescribeRefreshScheduleResponseTypeDef",
     "ListRefreshSchedulesResponseTypeDef",
+    "CreateRefreshScheduleRequestRequestTypeDef",
+    "RefreshScheduleUnionTypeDef",
     "UpdateRefreshScheduleRequestRequestTypeDef",
     "RegisteredUserEmbeddingExperienceConfigurationTypeDef",
     "SnapshotJobResultFileGroupTypeDef",
+    "PhysicalTableUnionTypeDef",
     "DefaultSectionBasedLayoutConfigurationTypeDef",
+    "FreeFormLayoutConfigurationOutputTypeDef",
+    "FreeFormSectionLayoutConfigurationOutputTypeDef",
     "FreeFormLayoutConfigurationTypeDef",
     "FreeFormSectionLayoutConfigurationTypeDef",
+    "SnapshotConfigurationOutputTypeDef",
     "SnapshotConfigurationTypeDef",
+    "ParameterDeclarationOutputTypeDef",
     "ParameterDeclarationTypeDef",
+    "ColumnHierarchyOutputTypeDef",
     "DescribeDashboardResponseTypeDef",
-    "TemplateTypeDef",
+    "AssetBundleImportJobOverridePermissionsUnionTypeDef",
     "SetParameterValueConfigurationTypeDef",
-    "LogicalTableTypeDef",
+    "DatasetParameterUnionTypeDef",
     "ColumnHierarchyTypeDef",
+    "LogicalTableOutputTypeDef",
+    "LogicalTableTypeDef",
+    "TemplateTypeDef",
+    "CustomActionSetParametersOperationOutputTypeDef",
+    "PivotTableFieldOptionsOutputTypeDef",
     "PivotTableFieldOptionsTypeDef",
+    "AxisDisplayOptionsOutputTypeDef",
     "AxisDisplayOptionsTypeDef",
     "DefaultDateTimePickerControlOptionsTypeDef",
     "FilterDateTimePickerControlTypeDef",
     "ParameterDateTimePickerControlTypeDef",
+    "DefaultFilterDropDownControlOptionsOutputTypeDef",
     "DefaultFilterDropDownControlOptionsTypeDef",
+    "FilterDropDownControlOutputTypeDef",
     "FilterDropDownControlTypeDef",
+    "ParameterDropDownControlOutputTypeDef",
     "ParameterDropDownControlTypeDef",
+    "DefaultFilterListControlOptionsOutputTypeDef",
     "DefaultFilterListControlOptionsTypeDef",
+    "FilterListControlOutputTypeDef",
     "FilterListControlTypeDef",
+    "ParameterListControlOutputTypeDef",
     "ParameterListControlTypeDef",
     "DefaultRelativeDateTimeControlOptionsTypeDef",
     "FilterRelativeDateTimeControlTypeDef",
     "DefaultSliderControlOptionsTypeDef",
     "FilterSliderControlTypeDef",
     "ParameterSliderControlTypeDef",
     "DefaultTextAreaControlOptionsTypeDef",
     "FilterTextAreaControlTypeDef",
     "ParameterTextAreaControlTypeDef",
     "DefaultTextFieldControlOptionsTypeDef",
     "FilterTextFieldControlTypeDef",
     "ParameterTextFieldControlTypeDef",
     "SmallMultiplesOptionsTypeDef",
     "TableFieldLinkConfigurationTypeDef",
+    "PivotTableOptionsOutputTypeDef",
     "PivotTableOptionsTypeDef",
+    "PivotTotalOptionsOutputTypeDef",
     "PivotTotalOptionsTypeDef",
+    "SubtotalOptionsOutputTypeDef",
     "SubtotalOptionsTypeDef",
+    "TableOptionsOutputTypeDef",
     "TableOptionsTypeDef",
+    "TotalOptionsOutputTypeDef",
     "TotalOptionsTypeDef",
+    "GaugeChartArcConditionalFormattingOutputTypeDef",
+    "GaugeChartPrimaryValueConditionalFormattingOutputTypeDef",
+    "KPIActualValueConditionalFormattingOutputTypeDef",
+    "KPIComparisonValueConditionalFormattingOutputTypeDef",
+    "KPIPrimaryValueConditionalFormattingOutputTypeDef",
+    "KPIProgressBarConditionalFormattingOutputTypeDef",
+    "ShapeConditionalFormatOutputTypeDef",
+    "TableRowConditionalFormattingOutputTypeDef",
+    "TextConditionalFormatOutputTypeDef",
     "GaugeChartArcConditionalFormattingTypeDef",
     "GaugeChartPrimaryValueConditionalFormattingTypeDef",
     "KPIActualValueConditionalFormattingTypeDef",
     "KPIComparisonValueConditionalFormattingTypeDef",
     "KPIPrimaryValueConditionalFormattingTypeDef",
     "KPIProgressBarConditionalFormattingTypeDef",
     "ShapeConditionalFormatTypeDef",
     "TableRowConditionalFormattingTypeDef",
     "TextConditionalFormatTypeDef",
+    "SheetControlLayoutOutputTypeDef",
     "SheetControlLayoutTypeDef",
     "DescribeDataSetRefreshPropertiesResponseTypeDef",
     "PutDataSetRefreshPropertiesRequestRequestTypeDef",
-    "CreateThemeRequestRequestTypeDef",
     "ThemeVersionTypeDef",
+    "CreateThemeRequestRequestTypeDef",
+    "ThemeConfigurationUnionTypeDef",
     "UpdateThemeRequestRequestTypeDef",
     "ComparisonConfigurationTypeDef",
     "DateTimeFormatConfigurationTypeDef",
     "NumberFormatConfigurationTypeDef",
     "ReferenceLineValueLabelConfigurationTypeDef",
     "StringFormatConfigurationTypeDef",
     "FieldSortOptionsTypeDef",
+    "PivotTableSortByOutputTypeDef",
     "PivotTableSortByTypeDef",
     "TooltipItemTypeDef",
     "ReferenceLineDataConfigurationTypeDef",
+    "DatasetMetadataOutputTypeDef",
     "DatasetMetadataTypeDef",
-    "ListDataSourcesResponsePaginatorTypeDef",
-    "AssetBundleImportJobOverrideParametersTypeDef",
-    "DataSourceCredentialsTypeDef",
+    "AssetBundleImportJobOverrideParametersOutputTypeDef",
     "DescribeDataSourceResponseTypeDef",
     "ListDataSourcesResponseTypeDef",
+    "AssetBundleImportJobOverrideParametersTypeDef",
+    "DataSourceCredentialsTypeDef",
     "GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
     "AnonymousUserSnapshotJobResultTypeDef",
     "DefaultPaginatedLayoutConfigurationTypeDef",
+    "SectionLayoutConfigurationOutputTypeDef",
     "SectionLayoutConfigurationTypeDef",
     "DescribeDashboardSnapshotJobResponseTypeDef",
+    "SnapshotConfigurationUnionTypeDef",
     "StartDashboardSnapshotJobRequestRequestTypeDef",
-    "DescribeTemplateResponseTypeDef",
     "CustomActionSetParametersOperationTypeDef",
-    "CreateDataSetRequestRequestTypeDef",
     "DataSetTypeDef",
-    "UpdateDataSetRequestRequestTypeDef",
+    "LogicalTableUnionTypeDef",
+    "DescribeTemplateResponseTypeDef",
+    "VisualCustomActionOperationOutputTypeDef",
+    "LineSeriesAxisDisplayOptionsOutputTypeDef",
     "LineSeriesAxisDisplayOptionsTypeDef",
+    "DefaultFilterControlOptionsOutputTypeDef",
     "DefaultFilterControlOptionsTypeDef",
+    "FilterControlOutputTypeDef",
     "FilterControlTypeDef",
+    "ParameterControlOutputTypeDef",
     "ParameterControlTypeDef",
     "TableFieldURLConfigurationTypeDef",
+    "PivotTableTotalOptionsOutputTypeDef",
     "PivotTableTotalOptionsTypeDef",
+    "GaugeChartConditionalFormattingOptionOutputTypeDef",
+    "KPIConditionalFormattingOptionOutputTypeDef",
+    "FilledMapShapeConditionalFormattingOutputTypeDef",
+    "PivotTableCellConditionalFormattingOutputTypeDef",
+    "TableCellConditionalFormattingOutputTypeDef",
     "GaugeChartConditionalFormattingOptionTypeDef",
     "KPIConditionalFormattingOptionTypeDef",
     "FilledMapShapeConditionalFormattingTypeDef",
     "PivotTableCellConditionalFormattingTypeDef",
     "TableCellConditionalFormattingTypeDef",
     "ThemeTypeDef",
     "GaugeChartOptionsTypeDef",
@@ -1197,188 +1408,331 @@
     "DateMeasureFieldTypeDef",
     "NumericalDimensionFieldTypeDef",
     "NumericalMeasureFieldTypeDef",
     "ReferenceLineLabelConfigurationTypeDef",
     "CategoricalDimensionFieldTypeDef",
     "CategoricalMeasureFieldTypeDef",
     "FormatConfigurationTypeDef",
+    "BarChartSortConfigurationOutputTypeDef",
     "BarChartSortConfigurationTypeDef",
+    "BoxPlotSortConfigurationOutputTypeDef",
     "BoxPlotSortConfigurationTypeDef",
+    "ComboChartSortConfigurationOutputTypeDef",
     "ComboChartSortConfigurationTypeDef",
+    "FilledMapSortConfigurationOutputTypeDef",
     "FilledMapSortConfigurationTypeDef",
+    "FunnelChartSortConfigurationOutputTypeDef",
     "FunnelChartSortConfigurationTypeDef",
+    "HeatMapSortConfigurationOutputTypeDef",
     "HeatMapSortConfigurationTypeDef",
+    "KPISortConfigurationOutputTypeDef",
     "KPISortConfigurationTypeDef",
+    "LineChartSortConfigurationOutputTypeDef",
     "LineChartSortConfigurationTypeDef",
+    "PieChartSortConfigurationOutputTypeDef",
     "PieChartSortConfigurationTypeDef",
+    "RadarChartSortConfigurationOutputTypeDef",
     "RadarChartSortConfigurationTypeDef",
+    "SankeyDiagramSortConfigurationOutputTypeDef",
     "SankeyDiagramSortConfigurationTypeDef",
+    "TableSortConfigurationOutputTypeDef",
     "TableSortConfigurationTypeDef",
+    "TreeMapSortConfigurationOutputTypeDef",
     "TreeMapSortConfigurationTypeDef",
+    "WaterfallChartSortConfigurationOutputTypeDef",
     "WaterfallChartSortConfigurationTypeDef",
+    "WordCloudSortConfigurationOutputTypeDef",
     "WordCloudSortConfigurationTypeDef",
+    "PivotFieldSortOptionsOutputTypeDef",
     "PivotFieldSortOptionsTypeDef",
+    "FieldBasedTooltipOutputTypeDef",
     "FieldBasedTooltipTypeDef",
+    "TopicDetailsOutputTypeDef",
     "TopicDetailsTypeDef",
     "DescribeAssetBundleImportJobResponseTypeDef",
+    "AssetBundleImportJobOverrideParametersUnionTypeDef",
     "StartAssetBundleImportJobRequestRequestTypeDef",
     "CreateDataSourceRequestRequestTypeDef",
     "UpdateDataSourceRequestRequestTypeDef",
     "SnapshotJobResultTypeDef",
     "DefaultNewSheetConfigurationTypeDef",
+    "BodySectionContentOutputTypeDef",
+    "HeaderFooterSectionConfigurationOutputTypeDef",
     "BodySectionContentTypeDef",
     "HeaderFooterSectionConfigurationTypeDef",
     "VisualCustomActionOperationTypeDef",
     "DescribeDataSetResponseTypeDef",
+    "CreateDataSetRequestRequestTypeDef",
+    "UpdateDataSetRequestRequestTypeDef",
+    "VisualCustomActionOutputTypeDef",
+    "DefaultFilterControlConfigurationOutputTypeDef",
     "DefaultFilterControlConfigurationTypeDef",
     "TableFieldOptionTypeDef",
+    "GaugeChartConditionalFormattingOutputTypeDef",
+    "KPIConditionalFormattingOutputTypeDef",
+    "FilledMapConditionalFormattingOptionOutputTypeDef",
+    "PivotTableConditionalFormattingOptionOutputTypeDef",
+    "TableConditionalFormattingOptionOutputTypeDef",
     "GaugeChartConditionalFormattingTypeDef",
     "KPIConditionalFormattingTypeDef",
     "FilledMapConditionalFormattingOptionTypeDef",
     "PivotTableConditionalFormattingOptionTypeDef",
     "TableConditionalFormattingOptionTypeDef",
     "DescribeThemeResponseTypeDef",
     "ReferenceLineTypeDef",
     "DimensionFieldTypeDef",
     "MeasureFieldTypeDef",
+    "ColumnConfigurationOutputTypeDef",
     "ColumnConfigurationTypeDef",
     "UnaggregatedFieldTypeDef",
+    "PivotTableSortConfigurationOutputTypeDef",
     "PivotTableSortConfigurationTypeDef",
+    "TooltipOptionsOutputTypeDef",
     "TooltipOptionsTypeDef",
-    "CreateTopicRequestRequestTypeDef",
     "DescribeTopicResponseTypeDef",
+    "CreateTopicRequestRequestTypeDef",
+    "TopicDetailsUnionTypeDef",
     "UpdateTopicRequestRequestTypeDef",
     "DescribeDashboardSnapshotJobResultResponseTypeDef",
     "AnalysisDefaultsTypeDef",
+    "BodySectionConfigurationOutputTypeDef",
     "BodySectionConfigurationTypeDef",
     "VisualCustomActionTypeDef",
+    "CustomContentVisualOutputTypeDef",
+    "EmptyVisualOutputTypeDef",
+    "CategoryFilterOutputTypeDef",
+    "NumericEqualityFilterOutputTypeDef",
+    "NumericRangeFilterOutputTypeDef",
+    "RelativeDatesFilterOutputTypeDef",
+    "TimeEqualityFilterOutputTypeDef",
+    "TimeRangeFilterOutputTypeDef",
+    "TopBottomFilterOutputTypeDef",
     "CategoryFilterTypeDef",
     "NumericEqualityFilterTypeDef",
     "NumericRangeFilterTypeDef",
     "RelativeDatesFilterTypeDef",
     "TimeEqualityFilterTypeDef",
     "TimeRangeFilterTypeDef",
     "TopBottomFilterTypeDef",
+    "TableFieldOptionsOutputTypeDef",
     "TableFieldOptionsTypeDef",
+    "FilledMapConditionalFormattingOutputTypeDef",
+    "PivotTableConditionalFormattingOutputTypeDef",
+    "TableConditionalFormattingOutputTypeDef",
     "FilledMapConditionalFormattingTypeDef",
     "PivotTableConditionalFormattingTypeDef",
     "TableConditionalFormattingTypeDef",
     "UniqueValuesComputationTypeDef",
+    "BarChartAggregatedFieldWellsOutputTypeDef",
     "BarChartAggregatedFieldWellsTypeDef",
+    "BoxPlotAggregatedFieldWellsOutputTypeDef",
     "BoxPlotAggregatedFieldWellsTypeDef",
+    "ComboChartAggregatedFieldWellsOutputTypeDef",
     "ComboChartAggregatedFieldWellsTypeDef",
+    "FilledMapAggregatedFieldWellsOutputTypeDef",
     "FilledMapAggregatedFieldWellsTypeDef",
     "ForecastComputationTypeDef",
+    "FunnelChartAggregatedFieldWellsOutputTypeDef",
     "FunnelChartAggregatedFieldWellsTypeDef",
+    "GaugeChartFieldWellsOutputTypeDef",
     "GaugeChartFieldWellsTypeDef",
+    "GeospatialMapAggregatedFieldWellsOutputTypeDef",
     "GeospatialMapAggregatedFieldWellsTypeDef",
     "GrowthRateComputationTypeDef",
+    "HeatMapAggregatedFieldWellsOutputTypeDef",
     "HeatMapAggregatedFieldWellsTypeDef",
+    "HistogramAggregatedFieldWellsOutputTypeDef",
     "HistogramAggregatedFieldWellsTypeDef",
+    "KPIFieldWellsOutputTypeDef",
     "KPIFieldWellsTypeDef",
+    "LineChartAggregatedFieldWellsOutputTypeDef",
     "LineChartAggregatedFieldWellsTypeDef",
     "MaximumMinimumComputationTypeDef",
     "MetricComparisonComputationTypeDef",
     "PeriodOverPeriodComputationTypeDef",
     "PeriodToDateComputationTypeDef",
+    "PieChartAggregatedFieldWellsOutputTypeDef",
     "PieChartAggregatedFieldWellsTypeDef",
+    "PivotTableAggregatedFieldWellsOutputTypeDef",
     "PivotTableAggregatedFieldWellsTypeDef",
+    "RadarChartAggregatedFieldWellsOutputTypeDef",
     "RadarChartAggregatedFieldWellsTypeDef",
+    "SankeyDiagramAggregatedFieldWellsOutputTypeDef",
     "SankeyDiagramAggregatedFieldWellsTypeDef",
+    "ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef",
     "ScatterPlotCategoricallyAggregatedFieldWellsTypeDef",
+    "ScatterPlotUnaggregatedFieldWellsOutputTypeDef",
     "ScatterPlotUnaggregatedFieldWellsTypeDef",
+    "TableAggregatedFieldWellsOutputTypeDef",
     "TableAggregatedFieldWellsTypeDef",
     "TopBottomMoversComputationTypeDef",
     "TopBottomRankedComputationTypeDef",
     "TotalAggregationComputationTypeDef",
+    "TreeMapAggregatedFieldWellsOutputTypeDef",
     "TreeMapAggregatedFieldWellsTypeDef",
+    "WaterfallChartAggregatedFieldWellsOutputTypeDef",
     "WaterfallChartAggregatedFieldWellsTypeDef",
+    "WordCloudAggregatedFieldWellsOutputTypeDef",
     "WordCloudAggregatedFieldWellsTypeDef",
+    "TableUnaggregatedFieldWellsOutputTypeDef",
     "TableUnaggregatedFieldWellsTypeDef",
+    "SectionBasedLayoutConfigurationOutputTypeDef",
     "SectionBasedLayoutConfigurationTypeDef",
     "CustomContentVisualTypeDef",
     "EmptyVisualTypeDef",
+    "FilterOutputTypeDef",
     "FilterTypeDef",
+    "BarChartFieldWellsOutputTypeDef",
     "BarChartFieldWellsTypeDef",
+    "BoxPlotFieldWellsOutputTypeDef",
     "BoxPlotFieldWellsTypeDef",
+    "ComboChartFieldWellsOutputTypeDef",
     "ComboChartFieldWellsTypeDef",
+    "FilledMapFieldWellsOutputTypeDef",
     "FilledMapFieldWellsTypeDef",
+    "FunnelChartFieldWellsOutputTypeDef",
     "FunnelChartFieldWellsTypeDef",
+    "GaugeChartConfigurationOutputTypeDef",
     "GaugeChartConfigurationTypeDef",
+    "GeospatialMapFieldWellsOutputTypeDef",
     "GeospatialMapFieldWellsTypeDef",
+    "HeatMapFieldWellsOutputTypeDef",
     "HeatMapFieldWellsTypeDef",
+    "HistogramFieldWellsOutputTypeDef",
     "HistogramFieldWellsTypeDef",
+    "KPIConfigurationOutputTypeDef",
     "KPIConfigurationTypeDef",
+    "LineChartFieldWellsOutputTypeDef",
     "LineChartFieldWellsTypeDef",
+    "PieChartFieldWellsOutputTypeDef",
     "PieChartFieldWellsTypeDef",
+    "PivotTableFieldWellsOutputTypeDef",
     "PivotTableFieldWellsTypeDef",
+    "RadarChartFieldWellsOutputTypeDef",
     "RadarChartFieldWellsTypeDef",
+    "SankeyDiagramFieldWellsOutputTypeDef",
     "SankeyDiagramFieldWellsTypeDef",
+    "ScatterPlotFieldWellsOutputTypeDef",
     "ScatterPlotFieldWellsTypeDef",
     "ComputationTypeDef",
+    "TreeMapFieldWellsOutputTypeDef",
     "TreeMapFieldWellsTypeDef",
+    "WaterfallChartFieldWellsOutputTypeDef",
     "WaterfallChartFieldWellsTypeDef",
+    "WordCloudFieldWellsOutputTypeDef",
     "WordCloudFieldWellsTypeDef",
+    "TableFieldWellsOutputTypeDef",
     "TableFieldWellsTypeDef",
+    "LayoutConfigurationOutputTypeDef",
     "LayoutConfigurationTypeDef",
+    "FilterGroupOutputTypeDef",
     "FilterGroupTypeDef",
+    "BarChartConfigurationOutputTypeDef",
     "BarChartConfigurationTypeDef",
+    "BoxPlotChartConfigurationOutputTypeDef",
     "BoxPlotChartConfigurationTypeDef",
+    "ComboChartConfigurationOutputTypeDef",
     "ComboChartConfigurationTypeDef",
+    "FilledMapConfigurationOutputTypeDef",
     "FilledMapConfigurationTypeDef",
+    "FunnelChartConfigurationOutputTypeDef",
     "FunnelChartConfigurationTypeDef",
+    "GaugeChartVisualOutputTypeDef",
     "GaugeChartVisualTypeDef",
+    "GeospatialMapConfigurationOutputTypeDef",
     "GeospatialMapConfigurationTypeDef",
+    "HeatMapConfigurationOutputTypeDef",
     "HeatMapConfigurationTypeDef",
+    "HistogramConfigurationOutputTypeDef",
     "HistogramConfigurationTypeDef",
+    "KPIVisualOutputTypeDef",
     "KPIVisualTypeDef",
+    "LineChartConfigurationOutputTypeDef",
     "LineChartConfigurationTypeDef",
+    "PieChartConfigurationOutputTypeDef",
     "PieChartConfigurationTypeDef",
+    "PivotTableConfigurationOutputTypeDef",
     "PivotTableConfigurationTypeDef",
+    "RadarChartConfigurationOutputTypeDef",
     "RadarChartConfigurationTypeDef",
+    "SankeyDiagramChartConfigurationOutputTypeDef",
     "SankeyDiagramChartConfigurationTypeDef",
+    "ScatterPlotConfigurationOutputTypeDef",
     "ScatterPlotConfigurationTypeDef",
+    "InsightConfigurationOutputTypeDef",
     "InsightConfigurationTypeDef",
+    "TreeMapConfigurationOutputTypeDef",
     "TreeMapConfigurationTypeDef",
+    "WaterfallChartConfigurationOutputTypeDef",
     "WaterfallChartConfigurationTypeDef",
+    "WordCloudChartConfigurationOutputTypeDef",
     "WordCloudChartConfigurationTypeDef",
+    "TableConfigurationOutputTypeDef",
     "TableConfigurationTypeDef",
+    "LayoutOutputTypeDef",
     "LayoutTypeDef",
+    "BarChartVisualOutputTypeDef",
     "BarChartVisualTypeDef",
+    "BoxPlotVisualOutputTypeDef",
     "BoxPlotVisualTypeDef",
+    "ComboChartVisualOutputTypeDef",
     "ComboChartVisualTypeDef",
+    "FilledMapVisualOutputTypeDef",
     "FilledMapVisualTypeDef",
+    "FunnelChartVisualOutputTypeDef",
     "FunnelChartVisualTypeDef",
+    "GeospatialMapVisualOutputTypeDef",
     "GeospatialMapVisualTypeDef",
+    "HeatMapVisualOutputTypeDef",
     "HeatMapVisualTypeDef",
+    "HistogramVisualOutputTypeDef",
     "HistogramVisualTypeDef",
+    "LineChartVisualOutputTypeDef",
     "LineChartVisualTypeDef",
+    "PieChartVisualOutputTypeDef",
     "PieChartVisualTypeDef",
+    "PivotTableVisualOutputTypeDef",
     "PivotTableVisualTypeDef",
+    "RadarChartVisualOutputTypeDef",
     "RadarChartVisualTypeDef",
+    "SankeyDiagramVisualOutputTypeDef",
     "SankeyDiagramVisualTypeDef",
+    "ScatterPlotVisualOutputTypeDef",
     "ScatterPlotVisualTypeDef",
+    "InsightVisualOutputTypeDef",
     "InsightVisualTypeDef",
+    "TreeMapVisualOutputTypeDef",
     "TreeMapVisualTypeDef",
+    "WaterfallVisualOutputTypeDef",
     "WaterfallVisualTypeDef",
+    "WordCloudVisualOutputTypeDef",
     "WordCloudVisualTypeDef",
+    "TableVisualOutputTypeDef",
     "TableVisualTypeDef",
+    "VisualOutputTypeDef",
     "VisualTypeDef",
+    "SheetDefinitionOutputTypeDef",
     "SheetDefinitionTypeDef",
+    "AnalysisDefinitionOutputTypeDef",
+    "DashboardVersionDefinitionOutputTypeDef",
+    "TemplateVersionDefinitionOutputTypeDef",
     "AnalysisDefinitionTypeDef",
     "DashboardVersionDefinitionTypeDef",
     "TemplateVersionDefinitionTypeDef",
-    "CreateAnalysisRequestRequestTypeDef",
     "DescribeAnalysisDefinitionResponseTypeDef",
+    "DescribeDashboardDefinitionResponseTypeDef",
+    "DescribeTemplateDefinitionResponseTypeDef",
+    "AnalysisDefinitionUnionTypeDef",
+    "CreateAnalysisRequestRequestTypeDef",
     "UpdateAnalysisRequestRequestTypeDef",
     "CreateDashboardRequestRequestTypeDef",
-    "DescribeDashboardDefinitionResponseTypeDef",
+    "DashboardVersionDefinitionUnionTypeDef",
     "UpdateDashboardRequestRequestTypeDef",
     "CreateTemplateRequestRequestTypeDef",
-    "DescribeTemplateDefinitionResponseTypeDef",
+    "TemplateVersionDefinitionUnionTypeDef",
     "UpdateTemplateRequestRequestTypeDef",
 )
 
 AccountCustomizationTypeDef = TypedDict(
     "AccountCustomizationTypeDef",
     {
         "DefaultTheme": NotRequired[str],
@@ -1524,14 +1878,20 @@
     "DashboardVisualIdTypeDef",
     {
         "DashboardId": str,
         "SheetId": str,
         "VisualId": str,
     },
 )
+AnonymousUserGenerativeQnAEmbeddingConfigurationTypeDef = TypedDict(
+    "AnonymousUserGenerativeQnAEmbeddingConfigurationTypeDef",
+    {
+        "InitialTopicId": str,
+    },
+)
 AnonymousUserQSearchBarEmbeddingConfigurationTypeDef = TypedDict(
     "AnonymousUserQSearchBarEmbeddingConfigurationTypeDef",
     {
         "InitialTopicId": str,
     },
 )
 ArcAxisDisplayRangeTypeDef = TypedDict(
@@ -1550,67 +1910,116 @@
 )
 ArcOptionsTypeDef = TypedDict(
     "ArcOptionsTypeDef",
     {
         "ArcThickness": NotRequired[ArcThicknessType],
     },
 )
-AssetBundleExportJobAnalysisOverridePropertiesTypeDef = TypedDict(
-    "AssetBundleExportJobAnalysisOverridePropertiesTypeDef",
+AssetBundleExportJobAnalysisOverridePropertiesOutputTypeDef = TypedDict(
+    "AssetBundleExportJobAnalysisOverridePropertiesOutputTypeDef",
     {
         "Arn": str,
         "Properties": List[Literal["Name"]],
     },
 )
-AssetBundleExportJobDashboardOverridePropertiesTypeDef = TypedDict(
-    "AssetBundleExportJobDashboardOverridePropertiesTypeDef",
+AssetBundleExportJobDashboardOverridePropertiesOutputTypeDef = TypedDict(
+    "AssetBundleExportJobDashboardOverridePropertiesOutputTypeDef",
     {
         "Arn": str,
         "Properties": List[Literal["Name"]],
     },
 )
-AssetBundleExportJobDataSetOverridePropertiesTypeDef = TypedDict(
-    "AssetBundleExportJobDataSetOverridePropertiesTypeDef",
+AssetBundleExportJobDataSetOverridePropertiesOutputTypeDef = TypedDict(
+    "AssetBundleExportJobDataSetOverridePropertiesOutputTypeDef",
     {
         "Arn": str,
         "Properties": List[Literal["Name"]],
     },
 )
-AssetBundleExportJobDataSourceOverridePropertiesTypeDef = TypedDict(
-    "AssetBundleExportJobDataSourceOverridePropertiesTypeDef",
+AssetBundleExportJobDataSourceOverridePropertiesOutputTypeDef = TypedDict(
+    "AssetBundleExportJobDataSourceOverridePropertiesOutputTypeDef",
     {
         "Arn": str,
         "Properties": List[AssetBundleExportJobDataSourcePropertyToOverrideType],
     },
 )
-AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef = TypedDict(
-    "AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef",
+AssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef = TypedDict(
+    "AssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef",
     {
         "Arn": str,
         "Properties": List[Literal["StartAfterDateTime"]],
     },
 )
 AssetBundleExportJobResourceIdOverrideConfigurationTypeDef = TypedDict(
     "AssetBundleExportJobResourceIdOverrideConfigurationTypeDef",
     {
         "PrefixForAllResources": NotRequired[bool],
     },
 )
+AssetBundleExportJobThemeOverridePropertiesOutputTypeDef = TypedDict(
+    "AssetBundleExportJobThemeOverridePropertiesOutputTypeDef",
+    {
+        "Arn": str,
+        "Properties": List[Literal["Name"]],
+    },
+)
+AssetBundleExportJobVPCConnectionOverridePropertiesOutputTypeDef = TypedDict(
+    "AssetBundleExportJobVPCConnectionOverridePropertiesOutputTypeDef",
+    {
+        "Arn": str,
+        "Properties": List[AssetBundleExportJobVPCConnectionPropertyToOverrideType],
+    },
+)
+AssetBundleExportJobAnalysisOverridePropertiesTypeDef = TypedDict(
+    "AssetBundleExportJobAnalysisOverridePropertiesTypeDef",
+    {
+        "Arn": str,
+        "Properties": Sequence[Literal["Name"]],
+    },
+)
+AssetBundleExportJobDashboardOverridePropertiesTypeDef = TypedDict(
+    "AssetBundleExportJobDashboardOverridePropertiesTypeDef",
+    {
+        "Arn": str,
+        "Properties": Sequence[Literal["Name"]],
+    },
+)
+AssetBundleExportJobDataSetOverridePropertiesTypeDef = TypedDict(
+    "AssetBundleExportJobDataSetOverridePropertiesTypeDef",
+    {
+        "Arn": str,
+        "Properties": Sequence[Literal["Name"]],
+    },
+)
+AssetBundleExportJobDataSourceOverridePropertiesTypeDef = TypedDict(
+    "AssetBundleExportJobDataSourceOverridePropertiesTypeDef",
+    {
+        "Arn": str,
+        "Properties": Sequence[AssetBundleExportJobDataSourcePropertyToOverrideType],
+    },
+)
+AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef = TypedDict(
+    "AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef",
+    {
+        "Arn": str,
+        "Properties": Sequence[Literal["StartAfterDateTime"]],
+    },
+)
 AssetBundleExportJobThemeOverridePropertiesTypeDef = TypedDict(
     "AssetBundleExportJobThemeOverridePropertiesTypeDef",
     {
         "Arn": str,
-        "Properties": List[Literal["Name"]],
+        "Properties": Sequence[Literal["Name"]],
     },
 )
 AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef = TypedDict(
     "AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef",
     {
         "Arn": str,
-        "Properties": List[AssetBundleExportJobVPCConnectionPropertyToOverrideType],
+        "Properties": Sequence[AssetBundleExportJobVPCConnectionPropertyToOverrideType],
     },
 )
 AssetBundleExportJobErrorTypeDef = TypedDict(
     "AssetBundleExportJobErrorTypeDef",
     {
         "Arn": NotRequired[str],
         "Type": NotRequired[str],
@@ -1646,21 +2055,28 @@
 AssetBundleImportJobAnalysisOverrideParametersTypeDef = TypedDict(
     "AssetBundleImportJobAnalysisOverrideParametersTypeDef",
     {
         "AnalysisId": str,
         "Name": NotRequired[str],
     },
 )
-AssetBundleResourcePermissionsTypeDef = TypedDict(
-    "AssetBundleResourcePermissionsTypeDef",
+AssetBundleResourcePermissionsOutputTypeDef = TypedDict(
+    "AssetBundleResourcePermissionsOutputTypeDef",
     {
         "Principals": List[str],
         "Actions": List[str],
     },
 )
+AssetBundleResourcePermissionsTypeDef = TypedDict(
+    "AssetBundleResourcePermissionsTypeDef",
+    {
+        "Principals": Sequence[str],
+        "Actions": Sequence[str],
+    },
+)
 TagTypeDef = TypedDict(
     "TagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -1701,16 +2117,16 @@
     "AssetBundleImportJobErrorTypeDef",
     {
         "Arn": NotRequired[str],
         "Type": NotRequired[str],
         "Message": NotRequired[str],
     },
 )
-AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef = TypedDict(
-    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
+AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef = TypedDict(
+    "AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef",
     {
         "DataSetId": str,
         "ScheduleId": str,
         "StartAfterDateTime": NotRequired[datetime],
     },
 )
 AssetBundleImportJobResourceIdOverrideConfigurationTypeDef = TypedDict(
@@ -1722,31 +2138,43 @@
 AssetBundleImportJobThemeOverrideParametersTypeDef = TypedDict(
     "AssetBundleImportJobThemeOverrideParametersTypeDef",
     {
         "ThemeId": str,
         "Name": NotRequired[str],
     },
 )
-AssetBundleImportJobVPCConnectionOverrideParametersTypeDef = TypedDict(
-    "AssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
+AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef = TypedDict(
+    "AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef",
     {
         "VPCConnectionId": str,
         "Name": NotRequired[str],
         "SubnetIds": NotRequired[List[str]],
         "SecurityGroupIds": NotRequired[List[str]],
         "DnsResolvers": NotRequired[List[str]],
         "RoleArn": NotRequired[str],
     },
 )
+AssetBundleImportJobVPCConnectionOverrideParametersTypeDef = TypedDict(
+    "AssetBundleImportJobVPCConnectionOverrideParametersTypeDef",
+    {
+        "VPCConnectionId": str,
+        "Name": NotRequired[str],
+        "SubnetIds": NotRequired[Sequence[str]],
+        "SecurityGroupIds": NotRequired[Sequence[str]],
+        "DnsResolvers": NotRequired[Sequence[str]],
+        "RoleArn": NotRequired[str],
+    },
+)
 AssetBundleImportJobOverrideValidationStrategyTypeDef = TypedDict(
     "AssetBundleImportJobOverrideValidationStrategyTypeDef",
     {
         "StrictModeForAllResources": NotRequired[bool],
     },
 )
+TimestampTypeDef = Union[datetime, str]
 AssetBundleImportJobSummaryTypeDef = TypedDict(
     "AssetBundleImportJobSummaryTypeDef",
     {
         "JobStatus": NotRequired[AssetBundleImportJobStatusType],
         "Arn": NotRequired[str],
         "CreatedTime": NotRequired[datetime],
         "AssetBundleImportJobId": NotRequired[str],
@@ -1930,14 +2358,32 @@
         "MatchOperator": CategoryFilterMatchOperatorType,
         "NullOption": FilterNullOptionType,
         "CategoryValue": NotRequired[str],
         "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
         "ParameterName": NotRequired[str],
     },
 )
+CustomFilterListConfigurationOutputTypeDef = TypedDict(
+    "CustomFilterListConfigurationOutputTypeDef",
+    {
+        "MatchOperator": CategoryFilterMatchOperatorType,
+        "NullOption": FilterNullOptionType,
+        "CategoryValues": NotRequired[List[str]],
+        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
+    },
+)
+FilterListConfigurationOutputTypeDef = TypedDict(
+    "FilterListConfigurationOutputTypeDef",
+    {
+        "MatchOperator": CategoryFilterMatchOperatorType,
+        "CategoryValues": NotRequired[List[str]],
+        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
+        "NullOption": NotRequired[FilterNullOptionType],
+    },
+)
 CustomFilterListConfigurationTypeDef = TypedDict(
     "CustomFilterListConfigurationTypeDef",
     {
         "MatchOperator": CategoryFilterMatchOperatorType,
         "NullOption": FilterNullOptionType,
         "CategoryValues": NotRequired[Sequence[str]],
         "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
@@ -1948,27 +2394,40 @@
     {
         "MatchOperator": CategoryFilterMatchOperatorType,
         "CategoryValues": NotRequired[Sequence[str]],
         "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
         "NullOption": NotRequired[FilterNullOptionType],
     },
 )
+CellValueSynonymOutputTypeDef = TypedDict(
+    "CellValueSynonymOutputTypeDef",
+    {
+        "CellValue": NotRequired[str],
+        "Synonyms": NotRequired[List[str]],
+    },
+)
 CellValueSynonymTypeDef = TypedDict(
     "CellValueSynonymTypeDef",
     {
         "CellValue": NotRequired[str],
         "Synonyms": NotRequired[Sequence[str]],
     },
 )
 SimpleClusterMarkerTypeDef = TypedDict(
     "SimpleClusterMarkerTypeDef",
     {
         "Color": NotRequired[str],
     },
 )
+CollectiveConstantOutputTypeDef = TypedDict(
+    "CollectiveConstantOutputTypeDef",
+    {
+        "ValueList": NotRequired[List[str]],
+    },
+)
 CollectiveConstantTypeDef = TypedDict(
     "CollectiveConstantTypeDef",
     {
         "ValueList": NotRequired[Sequence[str]],
     },
 )
 DataColorTypeDef = TypedDict(
@@ -1994,22 +2453,37 @@
 )
 ColumnGroupColumnSchemaTypeDef = TypedDict(
     "ColumnGroupColumnSchemaTypeDef",
     {
         "Name": NotRequired[str],
     },
 )
+GeoSpatialColumnGroupOutputTypeDef = TypedDict(
+    "GeoSpatialColumnGroupOutputTypeDef",
+    {
+        "Name": str,
+        "Columns": List[str],
+        "CountryCode": NotRequired[Literal["US"]],
+    },
+)
 GeoSpatialColumnGroupTypeDef = TypedDict(
     "GeoSpatialColumnGroupTypeDef",
     {
         "Name": str,
         "Columns": Sequence[str],
         "CountryCode": NotRequired[Literal["US"]],
     },
 )
+ColumnLevelPermissionRuleOutputTypeDef = TypedDict(
+    "ColumnLevelPermissionRuleOutputTypeDef",
+    {
+        "Principals": NotRequired[List[str]],
+        "ColumnNames": NotRequired[List[str]],
+    },
+)
 ColumnLevelPermissionRuleTypeDef = TypedDict(
     "ColumnLevelPermissionRuleTypeDef",
     {
         "Principals": NotRequired[Sequence[str]],
         "ColumnNames": NotRequired[Sequence[str]],
     },
 )
@@ -2017,14 +2491,22 @@
     "ColumnSchemaTypeDef",
     {
         "Name": NotRequired[str],
         "DataType": NotRequired[str],
         "GeographicRole": NotRequired[str],
     },
 )
+ComparativeOrderOutputTypeDef = TypedDict(
+    "ComparativeOrderOutputTypeDef",
+    {
+        "UseOrdering": NotRequired[ColumnOrderingTypeType],
+        "SpecifedOrder": NotRequired[List[str]],
+        "TreatUndefinedSpecifiedValues": NotRequired[UndefinedSpecifiedValueTypeType],
+    },
+)
 ComparativeOrderTypeDef = TypedDict(
     "ComparativeOrderTypeDef",
     {
         "UseOrdering": NotRequired[ColumnOrderingTypeType],
         "SpecifedOrder": NotRequired[Sequence[str]],
         "TreatUndefinedSpecifiedValues": NotRequired[UndefinedSpecifiedValueTypeType],
     },
@@ -2061,25 +2543,28 @@
     {
         "AvailabilityStatus": NotRequired[DashboardBehaviorType],
     },
 )
 CreateAccountSubscriptionRequestRequestTypeDef = TypedDict(
     "CreateAccountSubscriptionRequestRequestTypeDef",
     {
-        "Edition": EditionType,
         "AuthenticationMethod": AuthenticationMethodOptionType,
         "AwsAccountId": str,
         "AccountName": str,
         "NotificationEmail": str,
+        "Edition": NotRequired[EditionType],
         "ActiveDirectoryName": NotRequired[str],
         "Realm": NotRequired[str],
         "DirectoryId": NotRequired[str],
         "AdminGroup": NotRequired[Sequence[str]],
         "AuthorGroup": NotRequired[Sequence[str]],
         "ReaderGroup": NotRequired[Sequence[str]],
+        "AdminProGroup": NotRequired[Sequence[str]],
+        "AuthorProGroup": NotRequired[Sequence[str]],
+        "ReaderProGroup": NotRequired[Sequence[str]],
         "FirstName": NotRequired[str],
         "LastName": NotRequired[str],
         "EmailAddress": NotRequired[str],
         "ContactNumber": NotRequired[str],
         "IAMIdentityCenterInstanceArn": NotRequired[str],
     },
 )
@@ -2088,41 +2573,27 @@
     {
         "IAMUser": NotRequired[bool],
         "userLoginName": NotRequired[str],
         "accountName": NotRequired[str],
         "directoryType": NotRequired[str],
     },
 )
-ResourcePermissionTypeDef = TypedDict(
-    "ResourcePermissionTypeDef",
-    {
-        "Principal": str,
-        "Actions": Sequence[str],
-    },
-)
 ValidationStrategyTypeDef = TypedDict(
     "ValidationStrategyTypeDef",
     {
         "Mode": ValidationStrategyModeType,
     },
 )
 DataSetUsageConfigurationTypeDef = TypedDict(
     "DataSetUsageConfigurationTypeDef",
     {
         "DisableUseAsDirectQuerySource": NotRequired[bool],
         "DisableUseAsImportedSource": NotRequired[bool],
     },
 )
-FieldFolderTypeDef = TypedDict(
-    "FieldFolderTypeDef",
-    {
-        "description": NotRequired[str],
-        "columns": NotRequired[Sequence[str]],
-    },
-)
 RowLevelPermissionDataSetTypeDef = TypedDict(
     "RowLevelPermissionDataSetTypeDef",
     {
         "Arn": str,
         "PermissionPolicy": RowLevelPermissionPolicyType,
         "Namespace": NotRequired[str],
         "FormatVersion": NotRequired[RowLevelPermissionFormatVersionType],
@@ -2275,15 +2746,23 @@
 )
 CustomNarrativeOptionsTypeDef = TypedDict(
     "CustomNarrativeOptionsTypeDef",
     {
         "Narrative": str,
     },
 )
-TimestampTypeDef = Union[datetime, str]
+CustomParameterValuesOutputTypeDef = TypedDict(
+    "CustomParameterValuesOutputTypeDef",
+    {
+        "StringValues": NotRequired[List[str]],
+        "IntegerValues": NotRequired[List[int]],
+        "DecimalValues": NotRequired[List[float]],
+        "DateTimeValues": NotRequired[List[datetime]],
+    },
+)
 InputColumnTypeDef = TypedDict(
     "InputColumnTypeDef",
     {
         "Name": str,
         "Type": InputColumnDataTypeType,
         "SubType": NotRequired[ColumnDataSubTypeType],
     },
@@ -2390,14 +2869,22 @@
     "DataBarsOptionsTypeDef",
     {
         "FieldId": str,
         "PositiveColor": NotRequired[str],
         "NegativeColor": NotRequired[str],
     },
 )
+DataColorPaletteOutputTypeDef = TypedDict(
+    "DataColorPaletteOutputTypeDef",
+    {
+        "Colors": NotRequired[List[str]],
+        "MinMaxGradient": NotRequired[List[str]],
+        "EmptyFillColor": NotRequired[str],
+    },
+)
 DataColorPaletteTypeDef = TypedDict(
     "DataColorPaletteTypeDef",
     {
         "Colors": NotRequired[Sequence[str]],
         "MinMaxGradient": NotRequired[Sequence[str]],
         "EmptyFillColor": NotRequired[str],
     },
@@ -2445,14 +2932,21 @@
     "DataSetSearchFilterTypeDef",
     {
         "Operator": FilterOperatorType,
         "Name": DataSetFilterAttributeType,
         "Value": str,
     },
 )
+FieldFolderOutputTypeDef = TypedDict(
+    "FieldFolderOutputTypeDef",
+    {
+        "description": NotRequired[str],
+        "columns": NotRequired[List[str]],
+    },
+)
 OutputColumnTypeDef = TypedDict(
     "OutputColumnTypeDef",
     {
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "Type": NotRequired[ColumnDataTypeType],
         "SubType": NotRequired[ColumnDataSubTypeType],
@@ -2609,55 +3103,94 @@
         "DataSourceId": NotRequired[str],
         "Name": NotRequired[str],
         "Type": NotRequired[DataSourceTypeType],
         "CreatedTime": NotRequired[datetime],
         "LastUpdatedTime": NotRequired[datetime],
     },
 )
+DateTimeDatasetParameterDefaultValuesOutputTypeDef = TypedDict(
+    "DateTimeDatasetParameterDefaultValuesOutputTypeDef",
+    {
+        "StaticValues": NotRequired[List[datetime]],
+    },
+)
 RollingDateConfigurationTypeDef = TypedDict(
     "RollingDateConfigurationTypeDef",
     {
         "Expression": str,
         "DataSetIdentifier": NotRequired[str],
     },
 )
+DateTimeValueWhenUnsetConfigurationOutputTypeDef = TypedDict(
+    "DateTimeValueWhenUnsetConfigurationOutputTypeDef",
+    {
+        "ValueWhenUnsetOption": NotRequired[ValueWhenUnsetOptionType],
+        "CustomValue": NotRequired[datetime],
+    },
+)
 MappedDataSetParameterTypeDef = TypedDict(
     "MappedDataSetParameterTypeDef",
     {
         "DataSetIdentifier": str,
         "DataSetParameterName": str,
     },
 )
+DateTimeParameterOutputTypeDef = TypedDict(
+    "DateTimeParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Values": List[datetime],
+    },
+)
 SheetControlInfoIconLabelOptionsTypeDef = TypedDict(
     "SheetControlInfoIconLabelOptionsTypeDef",
     {
         "Visibility": NotRequired[VisibilityType],
         "InfoIconText": NotRequired[str],
     },
 )
+DecimalDatasetParameterDefaultValuesOutputTypeDef = TypedDict(
+    "DecimalDatasetParameterDefaultValuesOutputTypeDef",
+    {
+        "StaticValues": NotRequired[List[float]],
+    },
+)
 DecimalDatasetParameterDefaultValuesTypeDef = TypedDict(
     "DecimalDatasetParameterDefaultValuesTypeDef",
     {
         "StaticValues": NotRequired[Sequence[float]],
     },
 )
 DecimalValueWhenUnsetConfigurationTypeDef = TypedDict(
     "DecimalValueWhenUnsetConfigurationTypeDef",
     {
         "ValueWhenUnsetOption": NotRequired[ValueWhenUnsetOptionType],
         "CustomValue": NotRequired[float],
     },
 )
+DecimalParameterOutputTypeDef = TypedDict(
+    "DecimalParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Values": List[float],
+    },
+)
 DecimalParameterTypeDef = TypedDict(
     "DecimalParameterTypeDef",
     {
         "Name": str,
         "Values": Sequence[float],
     },
 )
+FilterSelectableValuesOutputTypeDef = TypedDict(
+    "FilterSelectableValuesOutputTypeDef",
+    {
+        "Values": NotRequired[List[str]],
+    },
+)
 FilterSelectableValuesTypeDef = TypedDict(
     "FilterSelectableValuesTypeDef",
     {
         "Values": NotRequired[Sequence[str]],
     },
 )
 DeleteAccountCustomizationRequestRequestTypeDef = TypedDict(
@@ -2891,14 +3424,21 @@
 DescribeAnalysisPermissionsRequestRequestTypeDef = TypedDict(
     "DescribeAnalysisPermissionsRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
+ResourcePermissionOutputTypeDef = TypedDict(
+    "ResourcePermissionOutputTypeDef",
+    {
+        "Principal": str,
+        "Actions": List[str],
+    },
+)
 DescribeAnalysisRequestRequestTypeDef = TypedDict(
     "DescribeAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
     },
 )
@@ -3013,16 +3553,16 @@
         "AwsAccountId": str,
         "FolderId": str,
         "Namespace": NotRequired[str],
         "MaxResults": NotRequired[int],
         "NextToken": NotRequired[str],
     },
 )
-ResourcePermissionPaginatorTypeDef = TypedDict(
-    "ResourcePermissionPaginatorTypeDef",
+ResourcePermissionExtraOutputTypeDef = TypedDict(
+    "ResourcePermissionExtraOutputTypeDef",
     {
         "Principal": str,
         "Actions": List[str],
     },
 )
 DescribeFolderRequestRequestTypeDef = TypedDict(
     "DescribeFolderRequestRequestTypeDef",
@@ -3211,14 +3751,25 @@
     "DescribeTopicRefreshScheduleRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TopicId": str,
         "DatasetId": str,
     },
 )
+TopicRefreshScheduleOutputTypeDef = TypedDict(
+    "TopicRefreshScheduleOutputTypeDef",
+    {
+        "IsEnabled": bool,
+        "BasedOnSpiceSchedule": bool,
+        "StartingAt": NotRequired[datetime],
+        "Timezone": NotRequired[str],
+        "RepeatAt": NotRequired[str],
+        "TopicScheduleType": NotRequired[TopicScheduleTypeType],
+    },
+)
 DescribeTopicRequestRequestTypeDef = TypedDict(
     "DescribeTopicRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TopicId": str,
     },
 )
@@ -3283,14 +3834,21 @@
     "ExcludePeriodConfigurationTypeDef",
     {
         "Amount": int,
         "Granularity": TimeGranularityType,
         "Status": NotRequired[WidgetStatusType],
     },
 )
+FieldFolderTypeDef = TypedDict(
+    "FieldFolderTypeDef",
+    {
+        "description": NotRequired[str],
+        "columns": NotRequired[Sequence[str]],
+    },
+)
 FieldSortTypeDef = TypedDict(
     "FieldSortTypeDef",
     {
         "FieldId": str,
         "Direction": SortDirectionType,
     },
 )
@@ -3305,14 +3863,21 @@
 )
 GeospatialMapStyleOptionsTypeDef = TypedDict(
     "GeospatialMapStyleOptionsTypeDef",
     {
         "BaseMapStyle": NotRequired[BaseMapStyleTypeType],
     },
 )
+SameSheetTargetVisualConfigurationOutputTypeDef = TypedDict(
+    "SameSheetTargetVisualConfigurationOutputTypeDef",
+    {
+        "TargetVisuals": NotRequired[List[str]],
+        "TargetVisualOptions": NotRequired[Literal["ALL_VISUALS"]],
+    },
+)
 SameSheetTargetVisualConfigurationTypeDef = TypedDict(
     "SameSheetTargetVisualConfigurationTypeDef",
     {
         "TargetVisuals": NotRequired[Sequence[str]],
         "TargetVisualOptions": NotRequired[Literal["ALL_VISUALS"]],
     },
 )
@@ -3367,14 +3932,29 @@
         "PeriodsBackward": NotRequired[int],
         "UpperBoundary": NotRequired[float],
         "LowerBoundary": NotRequired[float],
         "PredictionInterval": NotRequired[int],
         "Seasonality": NotRequired[int],
     },
 )
+WhatIfPointScenarioOutputTypeDef = TypedDict(
+    "WhatIfPointScenarioOutputTypeDef",
+    {
+        "Date": datetime,
+        "Value": float,
+    },
+)
+WhatIfRangeScenarioOutputTypeDef = TypedDict(
+    "WhatIfRangeScenarioOutputTypeDef",
+    {
+        "StartDate": datetime,
+        "EndDate": datetime,
+        "Value": float,
+    },
+)
 FreeFormLayoutScreenCanvasSizeOptionsTypeDef = TypedDict(
     "FreeFormLayoutScreenCanvasSizeOptionsTypeDef",
     {
         "OptimizedViewPortWidth": str,
     },
 )
 FreeFormLayoutElementBackgroundStyleTypeDef = TypedDict(
@@ -3393,14 +3973,21 @@
 )
 LoadingAnimationTypeDef = TypedDict(
     "LoadingAnimationTypeDef",
     {
         "Visibility": NotRequired[VisibilityType],
     },
 )
+GaugeChartColorConfigurationTypeDef = TypedDict(
+    "GaugeChartColorConfigurationTypeDef",
+    {
+        "ForegroundColor": NotRequired[str],
+        "BackgroundColor": NotRequired[str],
+    },
+)
 SessionTagTypeDef = TypedDict(
     "SessionTagTypeDef",
     {
         "Key": str,
         "Value": str,
     },
 )
@@ -3523,27 +4110,40 @@
     "RowInfoTypeDef",
     {
         "RowsIngested": NotRequired[int],
         "RowsDropped": NotRequired[int],
         "TotalRowsInDataset": NotRequired[int],
     },
 )
+IntegerDatasetParameterDefaultValuesOutputTypeDef = TypedDict(
+    "IntegerDatasetParameterDefaultValuesOutputTypeDef",
+    {
+        "StaticValues": NotRequired[List[int]],
+    },
+)
 IntegerDatasetParameterDefaultValuesTypeDef = TypedDict(
     "IntegerDatasetParameterDefaultValuesTypeDef",
     {
         "StaticValues": NotRequired[Sequence[int]],
     },
 )
 IntegerValueWhenUnsetConfigurationTypeDef = TypedDict(
     "IntegerValueWhenUnsetConfigurationTypeDef",
     {
         "ValueWhenUnsetOption": NotRequired[ValueWhenUnsetOptionType],
         "CustomValue": NotRequired[int],
     },
 )
+IntegerParameterOutputTypeDef = TypedDict(
+    "IntegerParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Values": List[int],
+    },
+)
 IntegerParameterTypeDef = TypedDict(
     "IntegerParameterTypeDef",
     {
         "Name": str,
         "Values": Sequence[int],
     },
 )
@@ -3606,14 +4206,21 @@
 )
 MissingDataConfigurationTypeDef = TypedDict(
     "MissingDataConfigurationTypeDef",
     {
         "TreatmentOption": NotRequired[MissingDataTreatmentOptionType],
     },
 )
+ResourcePermissionTypeDef = TypedDict(
+    "ResourcePermissionTypeDef",
+    {
+        "Principal": str,
+        "Actions": Sequence[str],
+    },
+)
 ListAnalysesRequestRequestTypeDef = TypedDict(
     "ListAnalysesRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "NextToken": NotRequired[str],
         "MaxResults": NotRequired[int],
     },
@@ -3896,14 +4503,15 @@
 )
 TopicSummaryTypeDef = TypedDict(
     "TopicSummaryTypeDef",
     {
         "Arn": NotRequired[str],
         "TopicId": NotRequired[str],
         "Name": NotRequired[str],
+        "UserExperienceVersion": NotRequired[TopicUserExperienceVersionType],
     },
 )
 ListUserGroupsRequestRequestTypeDef = TypedDict(
     "ListUserGroupsRequestRequestTypeDef",
     {
         "UserName": str,
         "AwsAccountId": str,
@@ -3945,14 +4553,21 @@
 )
 MarginStyleTypeDef = TypedDict(
     "MarginStyleTypeDef",
     {
         "Show": NotRequired[bool],
     },
 )
+NamedEntityDefinitionMetricOutputTypeDef = TypedDict(
+    "NamedEntityDefinitionMetricOutputTypeDef",
+    {
+        "Aggregation": NotRequired[NamedEntityAggTypeType],
+        "AggregationFunctionParameters": NotRequired[Dict[str, str]],
+    },
+)
 NamedEntityDefinitionMetricTypeDef = TypedDict(
     "NamedEntityDefinitionMetricTypeDef",
     {
         "Aggregation": NotRequired[NamedEntityAggTypeType],
         "AggregationFunctionParameters": NotRequired[Mapping[str, str]],
     },
 )
@@ -3969,14 +4584,23 @@
         "SubnetId": NotRequired[str],
         "AvailabilityZone": NotRequired[str],
         "ErrorMessage": NotRequired[str],
         "Status": NotRequired[NetworkInterfaceStatusType],
         "NetworkInterfaceId": NotRequired[str],
     },
 )
+NewDefaultValuesOutputTypeDef = TypedDict(
+    "NewDefaultValuesOutputTypeDef",
+    {
+        "StringStaticValues": NotRequired[List[str]],
+        "DecimalStaticValues": NotRequired[List[float]],
+        "DateTimeStaticValues": NotRequired[List[datetime]],
+        "IntegerStaticValues": NotRequired[List[int]],
+    },
+)
 NumericRangeFilterValueTypeDef = TypedDict(
     "NumericRangeFilterValueTypeDef",
     {
         "StaticValue": NotRequired[float],
         "Parameter": NotRequired[str],
     },
 )
@@ -3989,14 +4613,21 @@
 )
 PercentileAggregationTypeDef = TypedDict(
     "PercentileAggregationTypeDef",
     {
         "PercentileValue": NotRequired[float],
     },
 )
+StringParameterOutputTypeDef = TypedDict(
+    "StringParameterOutputTypeDef",
+    {
+        "Name": str,
+        "Values": List[str],
+    },
+)
 StringParameterTypeDef = TypedDict(
     "StringParameterTypeDef",
     {
         "Name": str,
         "Values": Sequence[str],
     },
 )
@@ -4037,22 +4668,36 @@
 PivotTableRowsLabelOptionsTypeDef = TypedDict(
     "PivotTableRowsLabelOptionsTypeDef",
     {
         "Visibility": NotRequired[VisibilityType],
         "CustomLabel": NotRequired[str],
     },
 )
+RowAlternateColorOptionsOutputTypeDef = TypedDict(
+    "RowAlternateColorOptionsOutputTypeDef",
+    {
+        "Status": NotRequired[WidgetStatusType],
+        "RowAlternateColors": NotRequired[List[str]],
+        "UsePrimaryBackgroundColor": NotRequired[WidgetStatusType],
+    },
+)
 RowAlternateColorOptionsTypeDef = TypedDict(
     "RowAlternateColorOptionsTypeDef",
     {
         "Status": NotRequired[WidgetStatusType],
         "RowAlternateColors": NotRequired[Sequence[str]],
         "UsePrimaryBackgroundColor": NotRequired[WidgetStatusType],
     },
 )
+ProjectOperationOutputTypeDef = TypedDict(
+    "ProjectOperationOutputTypeDef",
+    {
+        "ProjectedColumns": List[str],
+    },
+)
 ProjectOperationTypeDef = TypedDict(
     "ProjectOperationTypeDef",
     {
         "ProjectedColumns": Sequence[str],
     },
 )
 RadarChartAreaStyleSettingsTypeDef = TypedDict(
@@ -4064,16 +4709,25 @@
 RangeConstantTypeDef = TypedDict(
     "RangeConstantTypeDef",
     {
         "Minimum": NotRequired[str],
         "Maximum": NotRequired[str],
     },
 )
-RedshiftIAMParametersPaginatorTypeDef = TypedDict(
-    "RedshiftIAMParametersPaginatorTypeDef",
+RedshiftIAMParametersExtraOutputTypeDef = TypedDict(
+    "RedshiftIAMParametersExtraOutputTypeDef",
+    {
+        "RoleArn": str,
+        "DatabaseUser": str,
+        "DatabaseGroups": NotRequired[List[str]],
+        "AutoCreateDatabaseUser": NotRequired[bool],
+    },
+)
+RedshiftIAMParametersOutputTypeDef = TypedDict(
+    "RedshiftIAMParametersOutputTypeDef",
     {
         "RoleArn": str,
         "DatabaseUser": str,
         "DatabaseGroups": NotRequired[List[str]],
         "AutoCreateDatabaseUser": NotRequired[bool],
     },
 )
@@ -4114,14 +4768,20 @@
 )
 StatePersistenceConfigurationsTypeDef = TypedDict(
     "StatePersistenceConfigurationsTypeDef",
     {
         "Enabled": bool,
     },
 )
+RegisteredUserGenerativeQnAEmbeddingConfigurationTypeDef = TypedDict(
+    "RegisteredUserGenerativeQnAEmbeddingConfigurationTypeDef",
+    {
+        "InitialTopicId": NotRequired[str],
+    },
+)
 RegisteredUserQSearchBarEmbeddingConfigurationTypeDef = TypedDict(
     "RegisteredUserQSearchBarEmbeddingConfigurationTypeDef",
     {
         "InitialTopicId": NotRequired[str],
     },
 )
 RenameColumnOperationTypeDef = TypedDict(
@@ -4176,30 +4836,58 @@
     {
         "Top": NotRequired[str],
         "Bottom": NotRequired[str],
         "Left": NotRequired[str],
         "Right": NotRequired[str],
     },
 )
+SheetVisualScopingConfigurationOutputTypeDef = TypedDict(
+    "SheetVisualScopingConfigurationOutputTypeDef",
+    {
+        "SheetId": str,
+        "Scope": FilterVisualScopeType,
+        "VisualIds": NotRequired[List[str]],
+    },
+)
 SheetVisualScopingConfigurationTypeDef = TypedDict(
     "SheetVisualScopingConfigurationTypeDef",
     {
         "SheetId": str,
         "Scope": FilterVisualScopeType,
         "VisualIds": NotRequired[Sequence[str]],
     },
 )
+SemanticEntityTypeOutputTypeDef = TypedDict(
+    "SemanticEntityTypeOutputTypeDef",
+    {
+        "TypeName": NotRequired[str],
+        "SubTypeName": NotRequired[str],
+        "TypeParameters": NotRequired[Dict[str, str]],
+    },
+)
 SemanticEntityTypeTypeDef = TypedDict(
     "SemanticEntityTypeTypeDef",
     {
         "TypeName": NotRequired[str],
         "SubTypeName": NotRequired[str],
         "TypeParameters": NotRequired[Mapping[str, str]],
     },
 )
+SemanticTypeOutputTypeDef = TypedDict(
+    "SemanticTypeOutputTypeDef",
+    {
+        "TypeName": NotRequired[str],
+        "SubTypeName": NotRequired[str],
+        "TypeParameters": NotRequired[Dict[str, str]],
+        "TruthyCellValue": NotRequired[str],
+        "TruthyCellValueSynonyms": NotRequired[List[str]],
+        "FalseyCellValue": NotRequired[str],
+        "FalseyCellValueSynonyms": NotRequired[List[str]],
+    },
+)
 SemanticTypeTypeDef = TypedDict(
     "SemanticTypeTypeDef",
     {
         "TypeName": NotRequired[str],
         "SubTypeName": NotRequired[str],
         "TypeParameters": NotRequired[Mapping[str, str]],
         "TruthyCellValue": NotRequired[str],
@@ -4243,29 +4931,43 @@
 )
 SnapshotAnonymousUserRedactedTypeDef = TypedDict(
     "SnapshotAnonymousUserRedactedTypeDef",
     {
         "RowLevelPermissionTagKeys": NotRequired[List[str]],
     },
 )
+SnapshotFileSheetSelectionOutputTypeDef = TypedDict(
+    "SnapshotFileSheetSelectionOutputTypeDef",
+    {
+        "SheetId": str,
+        "SelectionScope": SnapshotFileSheetSelectionScopeType,
+        "VisualIds": NotRequired[List[str]],
+    },
+)
 SnapshotFileSheetSelectionTypeDef = TypedDict(
     "SnapshotFileSheetSelectionTypeDef",
     {
         "SheetId": str,
         "SelectionScope": SnapshotFileSheetSelectionScopeType,
-        "VisualIds": NotRequired[List[str]],
+        "VisualIds": NotRequired[Sequence[str]],
     },
 )
 SnapshotJobResultErrorInfoTypeDef = TypedDict(
     "SnapshotJobResultErrorInfoTypeDef",
     {
         "ErrorMessage": NotRequired[str],
         "ErrorType": NotRequired[str],
     },
 )
+StringDatasetParameterDefaultValuesOutputTypeDef = TypedDict(
+    "StringDatasetParameterDefaultValuesOutputTypeDef",
+    {
+        "StaticValues": NotRequired[List[str]],
+    },
+)
 StringDatasetParameterDefaultValuesTypeDef = TypedDict(
     "StringDatasetParameterDefaultValuesTypeDef",
     {
         "StaticValues": NotRequired[Sequence[str]],
     },
 )
 StringValueWhenUnsetConfigurationTypeDef = TypedDict(
@@ -4296,14 +4998,20 @@
 )
 TableFieldCustomIconContentTypeDef = TypedDict(
     "TableFieldCustomIconContentTypeDef",
     {
         "Icon": NotRequired[Literal["LINK"]],
     },
 )
+TablePinnedFieldOptionsOutputTypeDef = TypedDict(
+    "TablePinnedFieldOptionsOutputTypeDef",
+    {
+        "PinnedLeftFields": NotRequired[List[str]],
+    },
+)
 TablePinnedFieldOptionsTypeDef = TypedDict(
     "TablePinnedFieldOptionsTypeDef",
     {
         "PinnedLeftFields": NotRequired[Sequence[str]],
     },
 )
 TemplateSourceTemplateTypeDef = TypedDict(
@@ -4355,14 +5063,21 @@
 )
 TotalAggregationFunctionTypeDef = TypedDict(
     "TotalAggregationFunctionTypeDef",
     {
         "SimpleTotalAggregationFunction": NotRequired[SimpleTotalAggregationFunctionType],
     },
 )
+UntagColumnOperationOutputTypeDef = TypedDict(
+    "UntagColumnOperationOutputTypeDef",
+    {
+        "ColumnName": str,
+        "TagNames": List[ColumnTagNameType],
+    },
+)
 UntagColumnOperationTypeDef = TypedDict(
     "UntagColumnOperationTypeDef",
     {
         "ColumnName": str,
         "TagNames": Sequence[ColumnTagNameType],
     },
 )
@@ -4456,14 +5171,21 @@
     {
         "CustomPermissionsName": str,
         "Role": RoleType,
         "AwsAccountId": str,
         "Namespace": str,
     },
 )
+UpdateSPICECapacityConfigurationRequestRequestTypeDef = TypedDict(
+    "UpdateSPICECapacityConfigurationRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "PurchaseMode": PurchaseModeType,
+    },
+)
 UpdateTemplateAliasRequestRequestTypeDef = TypedDict(
     "UpdateTemplateAliasRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TemplateId": str,
         "AliasName": str,
         "TemplateVersionNumber": int,
@@ -4548,21 +5270,35 @@
 CascadingControlSourceTypeDef = TypedDict(
     "CascadingControlSourceTypeDef",
     {
         "SourceSheetControlId": NotRequired[str],
         "ColumnToMatch": NotRequired[ColumnIdentifierTypeDef],
     },
 )
+CategoryDrillDownFilterOutputTypeDef = TypedDict(
+    "CategoryDrillDownFilterOutputTypeDef",
+    {
+        "Column": ColumnIdentifierTypeDef,
+        "CategoryValues": List[str],
+    },
+)
 CategoryDrillDownFilterTypeDef = TypedDict(
     "CategoryDrillDownFilterTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "CategoryValues": Sequence[str],
     },
 )
+ContributionAnalysisDefaultOutputTypeDef = TypedDict(
+    "ContributionAnalysisDefaultOutputTypeDef",
+    {
+        "MeasureFieldId": str,
+        "ContributorDimensions": List[ColumnIdentifierTypeDef],
+    },
+)
 ContributionAnalysisDefaultTypeDef = TypedDict(
     "ContributionAnalysisDefaultTypeDef",
     {
         "MeasureFieldId": str,
         "ContributorDimensions": Sequence[ColumnIdentifierTypeDef],
     },
 )
@@ -4570,14 +5306,22 @@
     "DynamicDefaultValueTypeDef",
     {
         "DefaultValueColumn": ColumnIdentifierTypeDef,
         "UserNameColumn": NotRequired[ColumnIdentifierTypeDef],
         "GroupNameColumn": NotRequired[ColumnIdentifierTypeDef],
     },
 )
+FilterOperationSelectedFieldsConfigurationOutputTypeDef = TypedDict(
+    "FilterOperationSelectedFieldsConfigurationOutputTypeDef",
+    {
+        "SelectedFields": NotRequired[List[str]],
+        "SelectedFieldOptions": NotRequired[Literal["ALL_FIELDS"]],
+        "SelectedColumns": NotRequired[List[ColumnIdentifierTypeDef]],
+    },
+)
 FilterOperationSelectedFieldsConfigurationTypeDef = TypedDict(
     "FilterOperationSelectedFieldsConfigurationTypeDef",
     {
         "SelectedFields": NotRequired[Sequence[str]],
         "SelectedFieldOptions": NotRequired[Literal["ALL_FIELDS"]],
         "SelectedColumns": NotRequired[Sequence[ColumnIdentifierTypeDef]],
     },
@@ -4585,21 +5329,37 @@
 NumericEqualityDrillDownFilterTypeDef = TypedDict(
     "NumericEqualityDrillDownFilterTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "Value": float,
     },
 )
+ParameterSelectableValuesOutputTypeDef = TypedDict(
+    "ParameterSelectableValuesOutputTypeDef",
+    {
+        "Values": NotRequired[List[str]],
+        "LinkToDataSetColumn": NotRequired[ColumnIdentifierTypeDef],
+    },
+)
 ParameterSelectableValuesTypeDef = TypedDict(
     "ParameterSelectableValuesTypeDef",
     {
         "Values": NotRequired[Sequence[str]],
         "LinkToDataSetColumn": NotRequired[ColumnIdentifierTypeDef],
     },
 )
+TimeRangeDrillDownFilterOutputTypeDef = TypedDict(
+    "TimeRangeDrillDownFilterOutputTypeDef",
+    {
+        "Column": ColumnIdentifierTypeDef,
+        "RangeMinimum": datetime,
+        "RangeMaximum": datetime,
+        "TimeGranularity": TimeGranularityType,
+    },
+)
 AnalysisErrorTypeDef = TypedDict(
     "AnalysisErrorTypeDef",
     {
         "Type": NotRequired[AnalysisErrorTypeType],
         "Message": NotRequired[str],
         "ViolatedEntities": NotRequired[List[EntityTypeDef]],
     },
@@ -4665,107 +5425,208 @@
 ArcAxisConfigurationTypeDef = TypedDict(
     "ArcAxisConfigurationTypeDef",
     {
         "Range": NotRequired[ArcAxisDisplayRangeTypeDef],
         "ReserveRange": NotRequired[int],
     },
 )
+AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef = TypedDict(
+    "AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef",
+    {
+        "ResourceIdOverrideConfiguration": NotRequired[
+            AssetBundleExportJobResourceIdOverrideConfigurationTypeDef
+        ],
+        "VPCConnections": NotRequired[
+            List[AssetBundleExportJobVPCConnectionOverridePropertiesOutputTypeDef]
+        ],
+        "RefreshSchedules": NotRequired[
+            List[AssetBundleExportJobRefreshScheduleOverridePropertiesOutputTypeDef]
+        ],
+        "DataSources": NotRequired[
+            List[AssetBundleExportJobDataSourceOverridePropertiesOutputTypeDef]
+        ],
+        "DataSets": NotRequired[List[AssetBundleExportJobDataSetOverridePropertiesOutputTypeDef]],
+        "Themes": NotRequired[List[AssetBundleExportJobThemeOverridePropertiesOutputTypeDef]],
+        "Analyses": NotRequired[List[AssetBundleExportJobAnalysisOverridePropertiesOutputTypeDef]],
+        "Dashboards": NotRequired[
+            List[AssetBundleExportJobDashboardOverridePropertiesOutputTypeDef]
+        ],
+    },
+)
 AssetBundleCloudFormationOverridePropertyConfigurationTypeDef = TypedDict(
     "AssetBundleCloudFormationOverridePropertyConfigurationTypeDef",
     {
         "ResourceIdOverrideConfiguration": NotRequired[
             AssetBundleExportJobResourceIdOverrideConfigurationTypeDef
         ],
         "VPCConnections": NotRequired[
-            List[AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef]
+            Sequence[AssetBundleExportJobVPCConnectionOverridePropertiesTypeDef]
         ],
         "RefreshSchedules": NotRequired[
-            List[AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef]
+            Sequence[AssetBundleExportJobRefreshScheduleOverridePropertiesTypeDef]
+        ],
+        "DataSources": NotRequired[
+            Sequence[AssetBundleExportJobDataSourceOverridePropertiesTypeDef]
         ],
-        "DataSources": NotRequired[List[AssetBundleExportJobDataSourceOverridePropertiesTypeDef]],
-        "DataSets": NotRequired[List[AssetBundleExportJobDataSetOverridePropertiesTypeDef]],
-        "Themes": NotRequired[List[AssetBundleExportJobThemeOverridePropertiesTypeDef]],
-        "Analyses": NotRequired[List[AssetBundleExportJobAnalysisOverridePropertiesTypeDef]],
-        "Dashboards": NotRequired[List[AssetBundleExportJobDashboardOverridePropertiesTypeDef]],
+        "DataSets": NotRequired[Sequence[AssetBundleExportJobDataSetOverridePropertiesTypeDef]],
+        "Themes": NotRequired[Sequence[AssetBundleExportJobThemeOverridePropertiesTypeDef]],
+        "Analyses": NotRequired[Sequence[AssetBundleExportJobAnalysisOverridePropertiesTypeDef]],
+        "Dashboards": NotRequired[Sequence[AssetBundleExportJobDashboardOverridePropertiesTypeDef]],
+    },
+)
+AssetBundleImportJobAnalysisOverridePermissionsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobAnalysisOverridePermissionsOutputTypeDef",
+    {
+        "AnalysisIds": List[str],
+        "Permissions": AssetBundleResourcePermissionsOutputTypeDef,
+    },
+)
+AssetBundleImportJobDataSetOverridePermissionsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobDataSetOverridePermissionsOutputTypeDef",
+    {
+        "DataSetIds": List[str],
+        "Permissions": AssetBundleResourcePermissionsOutputTypeDef,
+    },
+)
+AssetBundleImportJobDataSourceOverridePermissionsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobDataSourceOverridePermissionsOutputTypeDef",
+    {
+        "DataSourceIds": List[str],
+        "Permissions": AssetBundleResourcePermissionsOutputTypeDef,
+    },
+)
+AssetBundleImportJobThemeOverridePermissionsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobThemeOverridePermissionsOutputTypeDef",
+    {
+        "ThemeIds": List[str],
+        "Permissions": AssetBundleResourcePermissionsOutputTypeDef,
+    },
+)
+AssetBundleResourceLinkSharingConfigurationOutputTypeDef = TypedDict(
+    "AssetBundleResourceLinkSharingConfigurationOutputTypeDef",
+    {
+        "Permissions": NotRequired[AssetBundleResourcePermissionsOutputTypeDef],
     },
 )
 AssetBundleImportJobAnalysisOverridePermissionsTypeDef = TypedDict(
     "AssetBundleImportJobAnalysisOverridePermissionsTypeDef",
     {
-        "AnalysisIds": List[str],
+        "AnalysisIds": Sequence[str],
         "Permissions": AssetBundleResourcePermissionsTypeDef,
     },
 )
 AssetBundleImportJobDataSetOverridePermissionsTypeDef = TypedDict(
     "AssetBundleImportJobDataSetOverridePermissionsTypeDef",
     {
-        "DataSetIds": List[str],
+        "DataSetIds": Sequence[str],
         "Permissions": AssetBundleResourcePermissionsTypeDef,
     },
 )
 AssetBundleImportJobDataSourceOverridePermissionsTypeDef = TypedDict(
     "AssetBundleImportJobDataSourceOverridePermissionsTypeDef",
     {
-        "DataSourceIds": List[str],
+        "DataSourceIds": Sequence[str],
         "Permissions": AssetBundleResourcePermissionsTypeDef,
     },
 )
 AssetBundleImportJobThemeOverridePermissionsTypeDef = TypedDict(
     "AssetBundleImportJobThemeOverridePermissionsTypeDef",
     {
-        "ThemeIds": List[str],
+        "ThemeIds": Sequence[str],
         "Permissions": AssetBundleResourcePermissionsTypeDef,
     },
 )
 AssetBundleResourceLinkSharingConfigurationTypeDef = TypedDict(
     "AssetBundleResourceLinkSharingConfigurationTypeDef",
     {
         "Permissions": NotRequired[AssetBundleResourcePermissionsTypeDef],
     },
 )
+AssetBundleImportJobAnalysisOverrideTagsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobAnalysisOverrideTagsOutputTypeDef",
+    {
+        "AnalysisIds": List[str],
+        "Tags": List[TagTypeDef],
+    },
+)
 AssetBundleImportJobAnalysisOverrideTagsTypeDef = TypedDict(
     "AssetBundleImportJobAnalysisOverrideTagsTypeDef",
     {
-        "AnalysisIds": List[str],
+        "AnalysisIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+AssetBundleImportJobDashboardOverrideTagsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobDashboardOverrideTagsOutputTypeDef",
+    {
+        "DashboardIds": List[str],
         "Tags": List[TagTypeDef],
     },
 )
 AssetBundleImportJobDashboardOverrideTagsTypeDef = TypedDict(
     "AssetBundleImportJobDashboardOverrideTagsTypeDef",
     {
-        "DashboardIds": List[str],
+        "DashboardIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+AssetBundleImportJobDataSetOverrideTagsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobDataSetOverrideTagsOutputTypeDef",
+    {
+        "DataSetIds": List[str],
         "Tags": List[TagTypeDef],
     },
 )
 AssetBundleImportJobDataSetOverrideTagsTypeDef = TypedDict(
     "AssetBundleImportJobDataSetOverrideTagsTypeDef",
     {
-        "DataSetIds": List[str],
+        "DataSetIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+AssetBundleImportJobDataSourceOverrideTagsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobDataSourceOverrideTagsOutputTypeDef",
+    {
+        "DataSourceIds": List[str],
         "Tags": List[TagTypeDef],
     },
 )
 AssetBundleImportJobDataSourceOverrideTagsTypeDef = TypedDict(
     "AssetBundleImportJobDataSourceOverrideTagsTypeDef",
     {
-        "DataSourceIds": List[str],
+        "DataSourceIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+AssetBundleImportJobThemeOverrideTagsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobThemeOverrideTagsOutputTypeDef",
+    {
+        "ThemeIds": List[str],
         "Tags": List[TagTypeDef],
     },
 )
 AssetBundleImportJobThemeOverrideTagsTypeDef = TypedDict(
     "AssetBundleImportJobThemeOverrideTagsTypeDef",
     {
-        "ThemeIds": List[str],
+        "ThemeIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
+    },
+)
+AssetBundleImportJobVPCConnectionOverrideTagsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobVPCConnectionOverrideTagsOutputTypeDef",
+    {
+        "VPCConnectionIds": List[str],
         "Tags": List[TagTypeDef],
     },
 )
 AssetBundleImportJobVPCConnectionOverrideTagsTypeDef = TypedDict(
     "AssetBundleImportJobVPCConnectionOverrideTagsTypeDef",
     {
-        "VPCConnectionIds": List[str],
-        "Tags": List[TagTypeDef],
+        "VPCConnectionIds": Sequence[str],
+        "Tags": Sequence[TagTypeDef],
     },
 )
 CreateAccountCustomizationRequestRequestTypeDef = TypedDict(
     "CreateAccountCustomizationRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AccountCustomization": AccountCustomizationTypeDef,
@@ -4823,21 +5684,109 @@
 AssetBundleImportJobDataSourceCredentialsTypeDef = TypedDict(
     "AssetBundleImportJobDataSourceCredentialsTypeDef",
     {
         "CredentialPair": NotRequired[AssetBundleImportJobDataSourceCredentialPairTypeDef],
         "SecretArn": NotRequired[str],
     },
 )
+AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef = TypedDict(
+    "AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef",
+    {
+        "DataSetId": str,
+        "ScheduleId": str,
+        "StartAfterDateTime": NotRequired[TimestampTypeDef],
+    },
+)
+CustomParameterValuesTypeDef = TypedDict(
+    "CustomParameterValuesTypeDef",
+    {
+        "StringValues": NotRequired[Sequence[str]],
+        "IntegerValues": NotRequired[Sequence[int]],
+        "DecimalValues": NotRequired[Sequence[float]],
+        "DateTimeValues": NotRequired[Sequence[TimestampTypeDef]],
+    },
+)
+DateTimeDatasetParameterDefaultValuesTypeDef = TypedDict(
+    "DateTimeDatasetParameterDefaultValuesTypeDef",
+    {
+        "StaticValues": NotRequired[Sequence[TimestampTypeDef]],
+    },
+)
+DateTimeParameterTypeDef = TypedDict(
+    "DateTimeParameterTypeDef",
+    {
+        "Name": str,
+        "Values": Sequence[TimestampTypeDef],
+    },
+)
+DateTimeValueWhenUnsetConfigurationTypeDef = TypedDict(
+    "DateTimeValueWhenUnsetConfigurationTypeDef",
+    {
+        "ValueWhenUnsetOption": NotRequired[ValueWhenUnsetOptionType],
+        "CustomValue": NotRequired[TimestampTypeDef],
+    },
+)
+NewDefaultValuesTypeDef = TypedDict(
+    "NewDefaultValuesTypeDef",
+    {
+        "StringStaticValues": NotRequired[Sequence[str]],
+        "DecimalStaticValues": NotRequired[Sequence[float]],
+        "DateTimeStaticValues": NotRequired[Sequence[TimestampTypeDef]],
+        "IntegerStaticValues": NotRequired[Sequence[int]],
+    },
+)
+TimeRangeDrillDownFilterTypeDef = TypedDict(
+    "TimeRangeDrillDownFilterTypeDef",
+    {
+        "Column": ColumnIdentifierTypeDef,
+        "RangeMinimum": TimestampTypeDef,
+        "RangeMaximum": TimestampTypeDef,
+        "TimeGranularity": TimeGranularityType,
+    },
+)
+TopicRefreshScheduleTypeDef = TypedDict(
+    "TopicRefreshScheduleTypeDef",
+    {
+        "IsEnabled": bool,
+        "BasedOnSpiceSchedule": bool,
+        "StartingAt": NotRequired[TimestampTypeDef],
+        "Timezone": NotRequired[str],
+        "RepeatAt": NotRequired[str],
+        "TopicScheduleType": NotRequired[TopicScheduleTypeType],
+    },
+)
+WhatIfPointScenarioTypeDef = TypedDict(
+    "WhatIfPointScenarioTypeDef",
+    {
+        "Date": TimestampTypeDef,
+        "Value": float,
+    },
+)
+WhatIfRangeScenarioTypeDef = TypedDict(
+    "WhatIfRangeScenarioTypeDef",
+    {
+        "StartDate": TimestampTypeDef,
+        "EndDate": TimestampTypeDef,
+        "Value": float,
+    },
+)
 AssetBundleImportSourceTypeDef = TypedDict(
     "AssetBundleImportSourceTypeDef",
     {
         "Body": NotRequired[BlobTypeDef],
         "S3Uri": NotRequired[str],
     },
 )
+AxisDisplayRangeOutputTypeDef = TypedDict(
+    "AxisDisplayRangeOutputTypeDef",
+    {
+        "MinMax": NotRequired[AxisDisplayMinMaxRangeTypeDef],
+        "DataDriven": NotRequired[Dict[str, Any]],
+    },
+)
 AxisDisplayRangeTypeDef = TypedDict(
     "AxisDisplayRangeTypeDef",
     {
         "MinMax": NotRequired[AxisDisplayMinMaxRangeTypeDef],
         "DataDriven": NotRequired[Mapping[str, Any]],
     },
 )
@@ -4873,14 +5822,20 @@
     "BoxPlotOptionsTypeDef",
     {
         "StyleOptions": NotRequired[BoxPlotStyleOptionsTypeDef],
         "OutlierVisibility": NotRequired[VisibilityType],
         "AllDataPointsVisibility": NotRequired[VisibilityType],
     },
 )
+CreateColumnsOperationOutputTypeDef = TypedDict(
+    "CreateColumnsOperationOutputTypeDef",
+    {
+        "Columns": List[CalculatedColumnTypeDef],
+    },
+)
 CreateColumnsOperationTypeDef = TypedDict(
     "CreateColumnsOperationTypeDef",
     {
         "Columns": Sequence[CalculatedColumnTypeDef],
     },
 )
 CancelIngestionResponseTypeDef = TypedDict(
@@ -5404,68 +6359,68 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListAnalysesResponseTypeDef = TypedDict(
     "ListAnalysesResponseTypeDef",
     {
         "AnalysisSummaryList": List[AnalysisSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListAssetBundleExportJobsResponseTypeDef = TypedDict(
     "ListAssetBundleExportJobsResponseTypeDef",
     {
         "AssetBundleExportJobSummaryList": List[AssetBundleExportJobSummaryTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListAssetBundleImportJobsResponseTypeDef = TypedDict(
     "ListAssetBundleImportJobsResponseTypeDef",
     {
         "AssetBundleImportJobSummaryList": List[AssetBundleImportJobSummaryTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListIAMPolicyAssignmentsForUserResponseTypeDef = TypedDict(
     "ListIAMPolicyAssignmentsForUserResponseTypeDef",
     {
         "ActiveAssignments": List[ActiveIAMPolicyAssignmentTypeDef],
         "RequestId": str,
-        "NextToken": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListIdentityPropagationConfigsResponseTypeDef = TypedDict(
     "ListIdentityPropagationConfigsResponseTypeDef",
     {
         "Services": List[AuthorizedTargetsByServiceTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListRoleMembershipsResponseTypeDef = TypedDict(
     "ListRoleMembershipsResponseTypeDef",
     {
         "MembersList": List[str],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": List[TagTypeDef],
         "RequestId": str,
@@ -5491,18 +6446,18 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 SearchAnalysesResponseTypeDef = TypedDict(
     "SearchAnalysesResponseTypeDef",
     {
         "AnalysisSummaryList": List[AnalysisSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 StartAssetBundleExportJobResponseTypeDef = TypedDict(
     "StartAssetBundleExportJobResponseTypeDef",
     {
         "Arn": str,
         "AssetBundleExportJobId": str,
@@ -5715,14 +6670,22 @@
     "UpdateRoleCustomPermissionResponseTypeDef",
     {
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+UpdateSPICECapacityConfigurationResponseTypeDef = TypedDict(
+    "UpdateSPICECapacityConfigurationResponseTypeDef",
+    {
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 UpdateTemplateResponseTypeDef = TypedDict(
     "UpdateTemplateResponseTypeDef",
     {
         "TemplateId": str,
         "Arn": str,
         "VersionArn": str,
         "CreationStatus": ResourceStatusType,
@@ -5773,70 +6736,122 @@
         "UpdateStatus": VPCConnectionResourceStatusType,
         "AvailabilityStatus": VPCConnectionAvailabilityStatusType,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CategoryFilterConfigurationOutputTypeDef = TypedDict(
+    "CategoryFilterConfigurationOutputTypeDef",
+    {
+        "FilterListConfiguration": NotRequired[FilterListConfigurationOutputTypeDef],
+        "CustomFilterListConfiguration": NotRequired[CustomFilterListConfigurationOutputTypeDef],
+        "CustomFilterConfiguration": NotRequired[CustomFilterConfigurationTypeDef],
+    },
+)
 CategoryFilterConfigurationTypeDef = TypedDict(
     "CategoryFilterConfigurationTypeDef",
     {
         "FilterListConfiguration": NotRequired[FilterListConfigurationTypeDef],
         "CustomFilterListConfiguration": NotRequired[CustomFilterListConfigurationTypeDef],
         "CustomFilterConfiguration": NotRequired[CustomFilterConfigurationTypeDef],
     },
 )
 ClusterMarkerTypeDef = TypedDict(
     "ClusterMarkerTypeDef",
     {
         "SimpleClusterMarker": NotRequired[SimpleClusterMarkerTypeDef],
     },
 )
+TopicCategoryFilterConstantOutputTypeDef = TypedDict(
+    "TopicCategoryFilterConstantOutputTypeDef",
+    {
+        "ConstantType": NotRequired[ConstantTypeType],
+        "SingularConstant": NotRequired[str],
+        "CollectiveConstant": NotRequired[CollectiveConstantOutputTypeDef],
+    },
+)
 TopicCategoryFilterConstantTypeDef = TypedDict(
     "TopicCategoryFilterConstantTypeDef",
     {
         "ConstantType": NotRequired[ConstantTypeType],
         "SingularConstant": NotRequired[str],
         "CollectiveConstant": NotRequired[CollectiveConstantTypeDef],
     },
 )
+ColorScaleOutputTypeDef = TypedDict(
+    "ColorScaleOutputTypeDef",
+    {
+        "Colors": List[DataColorTypeDef],
+        "ColorFillType": ColorFillTypeType,
+        "NullValueColor": NotRequired[DataColorTypeDef],
+    },
+)
 ColorScaleTypeDef = TypedDict(
     "ColorScaleTypeDef",
     {
         "Colors": Sequence[DataColorTypeDef],
         "ColorFillType": ColorFillTypeType,
         "NullValueColor": NotRequired[DataColorTypeDef],
     },
 )
+ColorsConfigurationOutputTypeDef = TypedDict(
+    "ColorsConfigurationOutputTypeDef",
+    {
+        "CustomColors": NotRequired[List[CustomColorTypeDef]],
+    },
+)
 ColorsConfigurationTypeDef = TypedDict(
     "ColorsConfigurationTypeDef",
     {
         "CustomColors": NotRequired[Sequence[CustomColorTypeDef]],
     },
 )
 ColumnTagTypeDef = TypedDict(
     "ColumnTagTypeDef",
     {
         "ColumnGeographicRole": NotRequired[GeoSpatialDataRoleType],
         "ColumnDescription": NotRequired[ColumnDescriptionTypeDef],
     },
 )
+ColumnGroupSchemaOutputTypeDef = TypedDict(
+    "ColumnGroupSchemaOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "ColumnGroupColumnSchemaList": NotRequired[List[ColumnGroupColumnSchemaTypeDef]],
+    },
+)
 ColumnGroupSchemaTypeDef = TypedDict(
     "ColumnGroupSchemaTypeDef",
     {
         "Name": NotRequired[str],
         "ColumnGroupColumnSchemaList": NotRequired[Sequence[ColumnGroupColumnSchemaTypeDef]],
     },
 )
+ColumnGroupOutputTypeDef = TypedDict(
+    "ColumnGroupOutputTypeDef",
+    {
+        "GeoSpatialColumnGroup": NotRequired[GeoSpatialColumnGroupOutputTypeDef],
+    },
+)
 ColumnGroupTypeDef = TypedDict(
     "ColumnGroupTypeDef",
     {
         "GeoSpatialColumnGroup": NotRequired[GeoSpatialColumnGroupTypeDef],
     },
 )
+ColumnLevelPermissionRuleUnionTypeDef = Union[
+    ColumnLevelPermissionRuleTypeDef, ColumnLevelPermissionRuleOutputTypeDef
+]
+DataSetSchemaOutputTypeDef = TypedDict(
+    "DataSetSchemaOutputTypeDef",
+    {
+        "ColumnSchemaList": NotRequired[List[ColumnSchemaTypeDef]],
+    },
+)
 DataSetSchemaTypeDef = TypedDict(
     "DataSetSchemaTypeDef",
     {
         "ColumnSchemaList": NotRequired[Sequence[ColumnSchemaTypeDef]],
     },
 )
 ConditionalFormattingCustomIconConditionTypeDef = TypedDict(
@@ -5853,252 +6868,14 @@
     {
         "SignupResponse": SignupResponseTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-CreateFolderRequestRequestTypeDef = TypedDict(
-    "CreateFolderRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "FolderId": str,
-        "Name": NotRequired[str],
-        "FolderType": NotRequired[FolderTypeType],
-        "ParentFolderArn": NotRequired[str],
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "SharingModel": NotRequired[SharingModelType],
-    },
-)
-DescribeAnalysisPermissionsResponseTypeDef = TypedDict(
-    "DescribeAnalysisPermissionsResponseTypeDef",
-    {
-        "AnalysisId": str,
-        "AnalysisArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeDataSetPermissionsResponseTypeDef = TypedDict(
-    "DescribeDataSetPermissionsResponseTypeDef",
-    {
-        "DataSetArn": str,
-        "DataSetId": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeDataSourcePermissionsResponseTypeDef = TypedDict(
-    "DescribeDataSourcePermissionsResponseTypeDef",
-    {
-        "DataSourceArn": str,
-        "DataSourceId": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeFolderPermissionsResponseTypeDef = TypedDict(
-    "DescribeFolderPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "FolderId": str,
-        "Arn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeFolderResolvedPermissionsResponseTypeDef = TypedDict(
-    "DescribeFolderResolvedPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "FolderId": str,
-        "Arn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeTemplatePermissionsResponseTypeDef = TypedDict(
-    "DescribeTemplatePermissionsResponseTypeDef",
-    {
-        "TemplateId": str,
-        "TemplateArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeThemePermissionsResponseTypeDef = TypedDict(
-    "DescribeThemePermissionsResponseTypeDef",
-    {
-        "ThemeId": str,
-        "ThemeArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeTopicPermissionsResponseTypeDef = TypedDict(
-    "DescribeTopicPermissionsResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-LinkSharingConfigurationTypeDef = TypedDict(
-    "LinkSharingConfigurationTypeDef",
-    {
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateAnalysisPermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateAnalysisPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "AnalysisId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateAnalysisPermissionsResponseTypeDef = TypedDict(
-    "UpdateAnalysisPermissionsResponseTypeDef",
-    {
-        "AnalysisArn": str,
-        "AnalysisId": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateDashboardPermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateDashboardPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DashboardId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "GrantLinkPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokeLinkPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateDataSetPermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateDataSetPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DataSetId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateDataSourcePermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateDataSourcePermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DataSourceId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateFolderPermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateFolderPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "FolderId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateFolderPermissionsResponseTypeDef = TypedDict(
-    "UpdateFolderPermissionsResponseTypeDef",
-    {
-        "Status": int,
-        "Arn": str,
-        "FolderId": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateTemplatePermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateTemplatePermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "TemplateId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateTemplatePermissionsResponseTypeDef = TypedDict(
-    "UpdateTemplatePermissionsResponseTypeDef",
-    {
-        "TemplateId": str,
-        "TemplateArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateThemePermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateThemePermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "ThemeId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateThemePermissionsResponseTypeDef = TypedDict(
-    "UpdateThemePermissionsResponseTypeDef",
-    {
-        "ThemeId": str,
-        "ThemeArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-UpdateTopicPermissionsRequestRequestTypeDef = TypedDict(
-    "UpdateTopicPermissionsRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "TopicId": str,
-        "GrantPermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RevokePermissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-    },
-)
-UpdateTopicPermissionsResponseTypeDef = TypedDict(
-    "UpdateTopicPermissionsResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 DataSetSummaryTypeDef = TypedDict(
     "DataSetSummaryTypeDef",
     {
         "Arn": NotRequired[str],
         "DataSetId": NotRequired[str],
         "Name": NotRequired[str],
         "CreatedTime": NotRequired[datetime],
@@ -6136,18 +6913,18 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListGroupMembershipsResponseTypeDef = TypedDict(
     "ListGroupMembershipsResponseTypeDef",
     {
         "GroupMemberList": List[GroupMemberTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 CreateGroupResponseTypeDef = TypedDict(
     "CreateGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
         "RequestId": str,
@@ -6164,38 +6941,38 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListGroupsResponseTypeDef = TypedDict(
     "ListGroupsResponseTypeDef",
     {
         "GroupList": List[GroupTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListUserGroupsResponseTypeDef = TypedDict(
     "ListUserGroupsResponseTypeDef",
     {
         "GroupList": List[GroupTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SearchGroupsResponseTypeDef = TypedDict(
     "SearchGroupsResponseTypeDef",
     {
         "GroupList": List[GroupTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateGroupResponseTypeDef = TypedDict(
     "UpdateGroupResponseTypeDef",
     {
         "Group": GroupTypeDef,
         "RequestId": str,
@@ -6223,16 +7000,16 @@
 )
 ListTemplateAliasesResponseTypeDef = TypedDict(
     "ListTemplateAliasesResponseTypeDef",
     {
         "TemplateAliasList": List[TemplateAliasTypeDef],
         "Status": int,
         "RequestId": str,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateTemplateAliasResponseTypeDef = TypedDict(
     "UpdateTemplateAliasResponseTypeDef",
     {
         "TemplateAlias": TemplateAliasTypeDef,
         "Status": int,
@@ -6260,16 +7037,16 @@
 )
 ListThemeAliasesResponseTypeDef = TypedDict(
     "ListThemeAliasesResponseTypeDef",
     {
         "ThemeAliasList": List[ThemeAliasTypeDef],
         "Status": int,
         "RequestId": str,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 UpdateThemeAliasResponseTypeDef = TypedDict(
     "UpdateThemeAliasResponseTypeDef",
     {
         "ThemeAlias": ThemeAliasTypeDef,
         "Status": int,
@@ -6279,96 +7056,49 @@
 )
 CustomActionNavigationOperationTypeDef = TypedDict(
     "CustomActionNavigationOperationTypeDef",
     {
         "LocalNavigationConfiguration": NotRequired[LocalNavigationConfigurationTypeDef],
     },
 )
-CustomParameterValuesTypeDef = TypedDict(
-    "CustomParameterValuesTypeDef",
+CustomValuesConfigurationOutputTypeDef = TypedDict(
+    "CustomValuesConfigurationOutputTypeDef",
     {
-        "StringValues": NotRequired[Sequence[str]],
-        "IntegerValues": NotRequired[Sequence[int]],
-        "DecimalValues": NotRequired[Sequence[float]],
-        "DateTimeValues": NotRequired[Sequence[TimestampTypeDef]],
+        "CustomValues": CustomParameterValuesOutputTypeDef,
+        "IncludeNullValue": NotRequired[bool],
     },
 )
-DateTimeDatasetParameterDefaultValuesTypeDef = TypedDict(
-    "DateTimeDatasetParameterDefaultValuesTypeDef",
-    {
-        "StaticValues": NotRequired[Sequence[TimestampTypeDef]],
-    },
-)
-DateTimeParameterTypeDef = TypedDict(
-    "DateTimeParameterTypeDef",
+CustomSqlOutputTypeDef = TypedDict(
+    "CustomSqlOutputTypeDef",
     {
+        "DataSourceArn": str,
         "Name": str,
-        "Values": Sequence[TimestampTypeDef],
-    },
-)
-DateTimeValueWhenUnsetConfigurationTypeDef = TypedDict(
-    "DateTimeValueWhenUnsetConfigurationTypeDef",
-    {
-        "ValueWhenUnsetOption": NotRequired[ValueWhenUnsetOptionType],
-        "CustomValue": NotRequired[TimestampTypeDef],
-    },
-)
-NewDefaultValuesTypeDef = TypedDict(
-    "NewDefaultValuesTypeDef",
-    {
-        "StringStaticValues": NotRequired[Sequence[str]],
-        "DecimalStaticValues": NotRequired[Sequence[float]],
-        "DateTimeStaticValues": NotRequired[Sequence[TimestampTypeDef]],
-        "IntegerStaticValues": NotRequired[Sequence[int]],
-    },
-)
-TimeRangeDrillDownFilterTypeDef = TypedDict(
-    "TimeRangeDrillDownFilterTypeDef",
-    {
-        "Column": ColumnIdentifierTypeDef,
-        "RangeMinimum": TimestampTypeDef,
-        "RangeMaximum": TimestampTypeDef,
-        "TimeGranularity": TimeGranularityType,
-    },
-)
-TopicRefreshScheduleTypeDef = TypedDict(
-    "TopicRefreshScheduleTypeDef",
-    {
-        "IsEnabled": bool,
-        "BasedOnSpiceSchedule": bool,
-        "StartingAt": NotRequired[TimestampTypeDef],
-        "Timezone": NotRequired[str],
-        "RepeatAt": NotRequired[str],
-        "TopicScheduleType": NotRequired[TopicScheduleTypeType],
-    },
-)
-WhatIfPointScenarioTypeDef = TypedDict(
-    "WhatIfPointScenarioTypeDef",
-    {
-        "Date": TimestampTypeDef,
-        "Value": float,
-    },
-)
-WhatIfRangeScenarioTypeDef = TypedDict(
-    "WhatIfRangeScenarioTypeDef",
-    {
-        "StartDate": TimestampTypeDef,
-        "EndDate": TimestampTypeDef,
-        "Value": float,
+        "SqlQuery": str,
+        "Columns": NotRequired[List[InputColumnTypeDef]],
     },
 )
 CustomSqlTypeDef = TypedDict(
     "CustomSqlTypeDef",
     {
         "DataSourceArn": str,
         "Name": str,
         "SqlQuery": str,
         "Columns": NotRequired[Sequence[InputColumnTypeDef]],
     },
 )
+RelationalTableOutputTypeDef = TypedDict(
+    "RelationalTableOutputTypeDef",
+    {
+        "DataSourceArn": str,
+        "Name": str,
+        "InputColumns": List[InputColumnTypeDef],
+        "Catalog": NotRequired[str],
+        "Schema": NotRequired[str],
+    },
+)
 RelationalTableTypeDef = TypedDict(
     "RelationalTableTypeDef",
     {
         "DataSourceArn": str,
         "Name": str,
         "InputColumns": Sequence[InputColumnTypeDef],
         "Catalog": NotRequired[str],
@@ -6391,38 +7121,38 @@
         "MaxResults": NotRequired[int],
     },
 )
 ListDashboardsResponseTypeDef = TypedDict(
     "ListDashboardsResponseTypeDef",
     {
         "DashboardSummaryList": List[DashboardSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SearchDashboardsResponseTypeDef = TypedDict(
     "SearchDashboardsResponseTypeDef",
     {
         "DashboardSummaryList": List[DashboardSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListDashboardVersionsResponseTypeDef = TypedDict(
     "ListDashboardVersionsResponseTypeDef",
     {
         "DashboardVersionSummaryList": List[DashboardVersionSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DashboardVisualPublishOptionsTypeDef = TypedDict(
     "DashboardVisualPublishOptionsTypeDef",
     {
         "ExportHiddenFieldsOption": NotRequired[ExportHiddenFieldsOptionTypeDef],
     },
@@ -6469,37 +7199,203 @@
         "MaxResults": NotRequired[int],
     },
 )
 SearchDataSourcesResponseTypeDef = TypedDict(
     "SearchDataSourcesResponseTypeDef",
     {
         "DataSourceSummaries": List[DataSourceSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+DateTimeDatasetParameterOutputTypeDef = TypedDict(
+    "DateTimeDatasetParameterOutputTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "ValueType": DatasetParameterValueTypeType,
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "DefaultValues": NotRequired[DateTimeDatasetParameterDefaultValuesOutputTypeDef],
+    },
+)
+TimeRangeFilterValueOutputTypeDef = TypedDict(
+    "TimeRangeFilterValueOutputTypeDef",
+    {
+        "StaticValue": NotRequired[datetime],
+        "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
+        "Parameter": NotRequired[str],
     },
 )
 TimeRangeFilterValueTypeDef = TypedDict(
     "TimeRangeFilterValueTypeDef",
     {
         "StaticValue": NotRequired[TimestampTypeDef],
         "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
         "Parameter": NotRequired[str],
     },
 )
+DecimalDatasetParameterOutputTypeDef = TypedDict(
+    "DecimalDatasetParameterOutputTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "ValueType": DatasetParameterValueTypeType,
+        "DefaultValues": NotRequired[DecimalDatasetParameterDefaultValuesOutputTypeDef],
+    },
+)
 DecimalDatasetParameterTypeDef = TypedDict(
     "DecimalDatasetParameterTypeDef",
     {
         "Id": str,
         "Name": str,
         "ValueType": DatasetParameterValueTypeType,
         "DefaultValues": NotRequired[DecimalDatasetParameterDefaultValuesTypeDef],
     },
 )
+DescribeAnalysisPermissionsResponseTypeDef = TypedDict(
+    "DescribeAnalysisPermissionsResponseTypeDef",
+    {
+        "AnalysisId": str,
+        "AnalysisArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeDataSetPermissionsResponseTypeDef = TypedDict(
+    "DescribeDataSetPermissionsResponseTypeDef",
+    {
+        "DataSetArn": str,
+        "DataSetId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeDataSourcePermissionsResponseTypeDef = TypedDict(
+    "DescribeDataSourcePermissionsResponseTypeDef",
+    {
+        "DataSourceArn": str,
+        "DataSourceId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeFolderResolvedPermissionsResponseTypeDef = TypedDict(
+    "DescribeFolderResolvedPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "FolderId": str,
+        "Arn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+DescribeTemplatePermissionsResponseTypeDef = TypedDict(
+    "DescribeTemplatePermissionsResponseTypeDef",
+    {
+        "TemplateId": str,
+        "TemplateArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeThemePermissionsResponseTypeDef = TypedDict(
+    "DescribeThemePermissionsResponseTypeDef",
+    {
+        "ThemeId": str,
+        "ThemeArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeTopicPermissionsResponseTypeDef = TypedDict(
+    "DescribeTopicPermissionsResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+LinkSharingConfigurationOutputTypeDef = TypedDict(
+    "LinkSharingConfigurationOutputTypeDef",
+    {
+        "Permissions": NotRequired[List[ResourcePermissionOutputTypeDef]],
+    },
+)
+UpdateAnalysisPermissionsResponseTypeDef = TypedDict(
+    "UpdateAnalysisPermissionsResponseTypeDef",
+    {
+        "AnalysisArn": str,
+        "AnalysisId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateFolderPermissionsResponseTypeDef = TypedDict(
+    "UpdateFolderPermissionsResponseTypeDef",
+    {
+        "Status": int,
+        "Arn": str,
+        "FolderId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateTemplatePermissionsResponseTypeDef = TypedDict(
+    "UpdateTemplatePermissionsResponseTypeDef",
+    {
+        "TemplateId": str,
+        "TemplateArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateThemePermissionsResponseTypeDef = TypedDict(
+    "UpdateThemePermissionsResponseTypeDef",
+    {
+        "ThemeId": str,
+        "ThemeArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateTopicPermissionsResponseTypeDef = TypedDict(
+    "UpdateTopicPermissionsResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DescribeFolderPermissionsRequestDescribeFolderPermissionsPaginateTypeDef = TypedDict(
     "DescribeFolderPermissionsRequestDescribeFolderPermissionsPaginateTypeDef",
     {
         "AwsAccountId": str,
         "FolderId": str,
         "Namespace": NotRequired[str],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -6724,36 +7620,24 @@
     "SearchDataSourcesRequestSearchDataSourcesPaginateTypeDef",
     {
         "AwsAccountId": str,
         "Filters": Sequence[DataSourceSearchFilterTypeDef],
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
-DescribeFolderPermissionsResponsePaginatorTypeDef = TypedDict(
-    "DescribeFolderPermissionsResponsePaginatorTypeDef",
-    {
-        "Status": int,
-        "FolderId": str,
-        "Arn": str,
-        "Permissions": List[ResourcePermissionPaginatorTypeDef],
-        "RequestId": str,
-        "NextToken": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-DescribeFolderResolvedPermissionsResponsePaginatorTypeDef = TypedDict(
-    "DescribeFolderResolvedPermissionsResponsePaginatorTypeDef",
+DescribeFolderPermissionsResponseTypeDef = TypedDict(
+    "DescribeFolderPermissionsResponseTypeDef",
     {
         "Status": int,
         "FolderId": str,
         "Arn": str,
-        "Permissions": List[ResourcePermissionPaginatorTypeDef],
+        "Permissions": List[ResourcePermissionExtraOutputTypeDef],
         "RequestId": str,
-        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeFolderResponseTypeDef = TypedDict(
     "DescribeFolderResponseTypeDef",
     {
         "Status": int,
         "Folder": FolderTypeDef,
@@ -6775,31 +7659,52 @@
     {
         "RefreshDetails": TopicRefreshDetailsTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+DescribeTopicRefreshScheduleResponseTypeDef = TypedDict(
+    "DescribeTopicRefreshScheduleResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "DatasetArn": str,
+        "RefreshSchedule": TopicRefreshScheduleOutputTypeDef,
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+TopicRefreshScheduleSummaryTypeDef = TypedDict(
+    "TopicRefreshScheduleSummaryTypeDef",
+    {
+        "DatasetId": NotRequired[str],
+        "DatasetArn": NotRequired[str],
+        "DatasetName": NotRequired[str],
+        "RefreshSchedule": NotRequired[TopicRefreshScheduleOutputTypeDef],
+    },
+)
 DescribeUserResponseTypeDef = TypedDict(
     "DescribeUserResponseTypeDef",
     {
         "User": UserTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListUsersResponseTypeDef = TypedDict(
     "ListUsersResponseTypeDef",
     {
         "UserList": List[UserTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 RegisterUserResponseTypeDef = TypedDict(
     "RegisterUserResponseTypeDef",
     {
         "User": UserTypeDef,
         "UserInvitationUrl": str,
@@ -6837,14 +7742,23 @@
 DonutOptionsTypeDef = TypedDict(
     "DonutOptionsTypeDef",
     {
         "ArcOptions": NotRequired[ArcOptionsTypeDef],
         "DonutCenterOptions": NotRequired[DonutCenterOptionsTypeDef],
     },
 )
+FieldFolderUnionTypeDef = Union[FieldFolderTypeDef, FieldFolderOutputTypeDef]
+FilterOperationTargetVisualsConfigurationOutputTypeDef = TypedDict(
+    "FilterOperationTargetVisualsConfigurationOutputTypeDef",
+    {
+        "SameSheetTargetVisualConfiguration": NotRequired[
+            SameSheetTargetVisualConfigurationOutputTypeDef
+        ],
+    },
+)
 FilterOperationTargetVisualsConfigurationTypeDef = TypedDict(
     "FilterOperationTargetVisualsConfigurationTypeDef",
     {
         "SameSheetTargetVisualConfiguration": NotRequired[
             SameSheetTargetVisualConfigurationTypeDef
         ],
     },
@@ -6867,45 +7781,58 @@
     },
 )
 ListFoldersResponseTypeDef = TypedDict(
     "ListFoldersResponseTypeDef",
     {
         "Status": int,
         "FolderSummaryList": List[FolderSummaryTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 SearchFoldersResponseTypeDef = TypedDict(
     "SearchFoldersResponseTypeDef",
     {
         "Status": int,
         "FolderSummaryList": List[FolderSummaryTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 FontConfigurationTypeDef = TypedDict(
     "FontConfigurationTypeDef",
     {
         "FontSize": NotRequired[FontSizeTypeDef],
         "FontDecoration": NotRequired[FontDecorationType],
         "FontColor": NotRequired[str],
         "FontWeight": NotRequired[FontWeightTypeDef],
         "FontStyle": NotRequired[FontStyleType],
     },
 )
+TypographyOutputTypeDef = TypedDict(
+    "TypographyOutputTypeDef",
+    {
+        "FontFamilies": NotRequired[List[FontTypeDef]],
+    },
+)
 TypographyTypeDef = TypedDict(
     "TypographyTypeDef",
     {
         "FontFamilies": NotRequired[Sequence[FontTypeDef]],
     },
 )
+ForecastScenarioOutputTypeDef = TypedDict(
+    "ForecastScenarioOutputTypeDef",
+    {
+        "WhatIfPointScenario": NotRequired[WhatIfPointScenarioOutputTypeDef],
+        "WhatIfRangeScenario": NotRequired[WhatIfRangeScenarioOutputTypeDef],
+    },
+)
 FreeFormLayoutCanvasSizeOptionsTypeDef = TypedDict(
     "FreeFormLayoutCanvasSizeOptionsTypeDef",
     {
         "ScreenCanvasSizeOptions": NotRequired[FreeFormLayoutScreenCanvasSizeOptionsTypeDef],
     },
 )
 SnapshotAnonymousUserTypeDef = TypedDict(
@@ -6917,14 +7844,20 @@
 GeospatialWindowOptionsTypeDef = TypedDict(
     "GeospatialWindowOptionsTypeDef",
     {
         "Bounds": NotRequired[GeospatialCoordinateBoundsTypeDef],
         "MapZoomMode": NotRequired[MapZoomModeType],
     },
 )
+GeospatialHeatmapColorScaleOutputTypeDef = TypedDict(
+    "GeospatialHeatmapColorScaleOutputTypeDef",
+    {
+        "Colors": NotRequired[List[GeospatialHeatmapDataColorTypeDef]],
+    },
+)
 GeospatialHeatmapColorScaleTypeDef = TypedDict(
     "GeospatialHeatmapColorScaleTypeDef",
     {
         "Colors": NotRequired[Sequence[GeospatialHeatmapDataColorTypeDef]],
     },
 )
 TableSideBorderOptionsTypeDef = TypedDict(
@@ -6934,14 +7867,20 @@
         "InnerHorizontal": NotRequired[TableBorderOptionsTypeDef],
         "Left": NotRequired[TableBorderOptionsTypeDef],
         "Right": NotRequired[TableBorderOptionsTypeDef],
         "Top": NotRequired[TableBorderOptionsTypeDef],
         "Bottom": NotRequired[TableBorderOptionsTypeDef],
     },
 )
+GradientColorOutputTypeDef = TypedDict(
+    "GradientColorOutputTypeDef",
+    {
+        "Stops": NotRequired[List[GradientStopTypeDef]],
+    },
+)
 GradientColorTypeDef = TypedDict(
     "GradientColorTypeDef",
     {
         "Stops": NotRequired[Sequence[GradientStopTypeDef]],
     },
 )
 GridLayoutCanvasSizeOptionsTypeDef = TypedDict(
@@ -6969,18 +7908,18 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListIAMPolicyAssignmentsResponseTypeDef = TypedDict(
     "ListIAMPolicyAssignmentsResponseTypeDef",
     {
         "IAMPolicyAssignments": List[IAMPolicyAssignmentSummaryTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 IncrementalRefreshTypeDef = TypedDict(
     "IncrementalRefreshTypeDef",
     {
         "LookbackWindow": LookbackWindowTypeDef,
     },
@@ -6997,14 +7936,23 @@
         "QueueInfo": NotRequired[QueueInfoTypeDef],
         "IngestionTimeInSeconds": NotRequired[int],
         "IngestionSizeInBytes": NotRequired[int],
         "RequestSource": NotRequired[IngestionRequestSourceType],
         "RequestType": NotRequired[IngestionRequestTypeType],
     },
 )
+IntegerDatasetParameterOutputTypeDef = TypedDict(
+    "IntegerDatasetParameterOutputTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "ValueType": DatasetParameterValueTypeType,
+        "DefaultValues": NotRequired[IntegerDatasetParameterDefaultValuesOutputTypeDef],
+    },
+)
 IntegerDatasetParameterTypeDef = TypedDict(
     "IntegerDatasetParameterTypeDef",
     {
         "Id": str,
         "Name": str,
         "ValueType": DatasetParameterValueTypeType,
         "DefaultValues": NotRequired[IntegerDatasetParameterDefaultValuesTypeDef],
@@ -7038,72 +7986,81 @@
 LineChartSeriesSettingsTypeDef = TypedDict(
     "LineChartSeriesSettingsTypeDef",
     {
         "LineStyleSettings": NotRequired[LineChartLineStyleSettingsTypeDef],
         "MarkerStyleSettings": NotRequired[LineChartMarkerStyleSettingsTypeDef],
     },
 )
+LinkSharingConfigurationTypeDef = TypedDict(
+    "LinkSharingConfigurationTypeDef",
+    {
+        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
+    },
+)
+ResourcePermissionUnionTypeDef = Union[
+    ResourcePermissionTypeDef, ResourcePermissionExtraOutputTypeDef
+]
 ListFolderMembersResponseTypeDef = TypedDict(
     "ListFolderMembersResponseTypeDef",
     {
         "Status": int,
         "FolderMemberList": List[MemberIdArnPairTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTemplateVersionsResponseTypeDef = TypedDict(
     "ListTemplateVersionsResponseTypeDef",
     {
         "TemplateVersionSummaryList": List[TemplateVersionSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTemplatesResponseTypeDef = TypedDict(
     "ListTemplatesResponseTypeDef",
     {
         "TemplateSummaryList": List[TemplateSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListThemeVersionsResponseTypeDef = TypedDict(
     "ListThemeVersionsResponseTypeDef",
     {
         "ThemeVersionSummaryList": List[ThemeVersionSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListThemesResponseTypeDef = TypedDict(
     "ListThemesResponseTypeDef",
     {
         "ThemeSummaryList": List[ThemeSummaryTypeDef],
-        "NextToken": str,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListTopicsResponseTypeDef = TypedDict(
     "ListTopicsResponseTypeDef",
     {
         "TopicsSummaries": List[TopicSummaryTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 VisualSubtitleLabelOptionsTypeDef = TypedDict(
     "VisualSubtitleLabelOptionsTypeDef",
     {
         "Visibility": NotRequired[VisibilityType],
         "FormatText": NotRequired[LongFormatTextTypeDef],
@@ -7119,14 +8076,24 @@
 TileLayoutStyleTypeDef = TypedDict(
     "TileLayoutStyleTypeDef",
     {
         "Gutter": NotRequired[GutterStyleTypeDef],
         "Margin": NotRequired[MarginStyleTypeDef],
     },
 )
+NamedEntityDefinitionOutputTypeDef = TypedDict(
+    "NamedEntityDefinitionOutputTypeDef",
+    {
+        "FieldName": NotRequired[str],
+        "PropertyName": NotRequired[str],
+        "PropertyRole": NotRequired[PropertyRoleType],
+        "PropertyUsage": NotRequired[PropertyUsageType],
+        "Metric": NotRequired[NamedEntityDefinitionMetricOutputTypeDef],
+    },
+)
 NamedEntityDefinitionTypeDef = TypedDict(
     "NamedEntityDefinitionTypeDef",
     {
         "FieldName": NotRequired[str],
         "PropertyName": NotRequired[str],
         "PropertyRole": NotRequired[PropertyRoleType],
         "PropertyUsage": NotRequired[PropertyUsageType],
@@ -7174,28 +8141,45 @@
         "AvailabilityStatus": NotRequired[VPCConnectionAvailabilityStatusType],
         "NetworkInterfaces": NotRequired[List[NetworkInterfaceTypeDef]],
         "RoleArn": NotRequired[str],
         "CreatedTime": NotRequired[datetime],
         "LastUpdatedTime": NotRequired[datetime],
     },
 )
+OverrideDatasetParameterOperationOutputTypeDef = TypedDict(
+    "OverrideDatasetParameterOperationOutputTypeDef",
+    {
+        "ParameterName": str,
+        "NewParameterName": NotRequired[str],
+        "NewDefaultValues": NotRequired[NewDefaultValuesOutputTypeDef],
+    },
+)
 NumericSeparatorConfigurationTypeDef = TypedDict(
     "NumericSeparatorConfigurationTypeDef",
     {
         "DecimalSeparator": NotRequired[NumericSeparatorSymbolType],
         "ThousandsSeparator": NotRequired[ThousandSeparatorOptionsTypeDef],
     },
 )
 NumericalAggregationFunctionTypeDef = TypedDict(
     "NumericalAggregationFunctionTypeDef",
     {
         "SimpleNumericalAggregation": NotRequired[SimpleNumericalAggregationFunctionType],
         "PercentileAggregation": NotRequired[PercentileAggregationTypeDef],
     },
 )
+ParametersOutputTypeDef = TypedDict(
+    "ParametersOutputTypeDef",
+    {
+        "StringParameters": NotRequired[List[StringParameterOutputTypeDef]],
+        "IntegerParameters": NotRequired[List[IntegerParameterOutputTypeDef]],
+        "DecimalParameters": NotRequired[List[DecimalParameterOutputTypeDef]],
+        "DateTimeParameters": NotRequired[List[DateTimeParameterOutputTypeDef]],
+    },
+)
 VisibleRangeOptionsTypeDef = TypedDict(
     "VisibleRangeOptionsTypeDef",
     {
         "PercentRange": NotRequired[PercentVisibleRangeTypeDef],
     },
 )
 RadarChartSeriesSettingsTypeDef = TypedDict(
@@ -7207,22 +8191,33 @@
 TopicRangeFilterConstantTypeDef = TypedDict(
     "TopicRangeFilterConstantTypeDef",
     {
         "ConstantType": NotRequired[ConstantTypeType],
         "RangeConstant": NotRequired[RangeConstantTypeDef],
     },
 )
-RedshiftParametersPaginatorTypeDef = TypedDict(
-    "RedshiftParametersPaginatorTypeDef",
+RedshiftParametersExtraOutputTypeDef = TypedDict(
+    "RedshiftParametersExtraOutputTypeDef",
+    {
+        "Database": str,
+        "Host": NotRequired[str],
+        "Port": NotRequired[int],
+        "ClusterId": NotRequired[str],
+        "IAMParameters": NotRequired[RedshiftIAMParametersExtraOutputTypeDef],
+        "IdentityCenterConfiguration": NotRequired[IdentityCenterConfigurationTypeDef],
+    },
+)
+RedshiftParametersOutputTypeDef = TypedDict(
+    "RedshiftParametersOutputTypeDef",
     {
         "Database": str,
         "Host": NotRequired[str],
         "Port": NotRequired[int],
         "ClusterId": NotRequired[str],
-        "IAMParameters": NotRequired[RedshiftIAMParametersPaginatorTypeDef],
+        "IAMParameters": NotRequired[RedshiftIAMParametersOutputTypeDef],
         "IdentityCenterConfiguration": NotRequired[IdentityCenterConfigurationTypeDef],
     },
 )
 RedshiftParametersTypeDef = TypedDict(
     "RedshiftParametersTypeDef",
     {
         "Database": str,
@@ -7251,28 +8246,44 @@
 RegisteredUserDashboardFeatureConfigurationsTypeDef = TypedDict(
     "RegisteredUserDashboardFeatureConfigurationsTypeDef",
     {
         "StatePersistence": NotRequired[StatePersistenceConfigurationsTypeDef],
         "Bookmarks": NotRequired[BookmarksConfigurationsTypeDef],
     },
 )
+RowLevelPermissionTagConfigurationOutputTypeDef = TypedDict(
+    "RowLevelPermissionTagConfigurationOutputTypeDef",
+    {
+        "TagRules": List[RowLevelPermissionTagRuleTypeDef],
+        "Status": NotRequired[StatusType],
+        "TagRuleConfigurations": NotRequired[List[List[str]]],
+    },
+)
 RowLevelPermissionTagConfigurationTypeDef = TypedDict(
     "RowLevelPermissionTagConfigurationTypeDef",
     {
         "TagRules": Sequence[RowLevelPermissionTagRuleTypeDef],
         "Status": NotRequired[StatusType],
         "TagRuleConfigurations": NotRequired[Sequence[Sequence[str]]],
     },
 )
 SnapshotS3DestinationConfigurationTypeDef = TypedDict(
     "SnapshotS3DestinationConfigurationTypeDef",
     {
         "BucketConfiguration": S3BucketConfigurationTypeDef,
     },
 )
+S3SourceOutputTypeDef = TypedDict(
+    "S3SourceOutputTypeDef",
+    {
+        "DataSourceArn": str,
+        "InputColumns": List[InputColumnTypeDef],
+        "UploadSettings": NotRequired[UploadSettingsTypeDef],
+    },
+)
 S3SourceTypeDef = TypedDict(
     "S3SourceTypeDef",
     {
         "DataSourceArn": str,
         "InputColumns": Sequence[InputColumnTypeDef],
         "UploadSettings": NotRequired[UploadSettingsTypeDef],
     },
@@ -7294,14 +8305,22 @@
 SectionStyleTypeDef = TypedDict(
     "SectionStyleTypeDef",
     {
         "Height": NotRequired[str],
         "Padding": NotRequired[SpacingTypeDef],
     },
 )
+SelectedSheetsFilterScopeConfigurationOutputTypeDef = TypedDict(
+    "SelectedSheetsFilterScopeConfigurationOutputTypeDef",
+    {
+        "SheetVisualScopingConfigurations": NotRequired[
+            List[SheetVisualScopingConfigurationOutputTypeDef]
+        ],
+    },
+)
 SelectedSheetsFilterScopeConfigurationTypeDef = TypedDict(
     "SelectedSheetsFilterScopeConfigurationTypeDef",
     {
         "SheetVisualScopingConfigurations": NotRequired[
             Sequence[SheetVisualScopingConfigurationTypeDef]
         ],
     },
@@ -7328,21 +8347,37 @@
 )
 SnapshotUserConfigurationRedactedTypeDef = TypedDict(
     "SnapshotUserConfigurationRedactedTypeDef",
     {
         "AnonymousUsers": NotRequired[List[SnapshotAnonymousUserRedactedTypeDef]],
     },
 )
+SnapshotFileOutputTypeDef = TypedDict(
+    "SnapshotFileOutputTypeDef",
+    {
+        "SheetSelections": List[SnapshotFileSheetSelectionOutputTypeDef],
+        "FormatType": SnapshotFileFormatTypeType,
+    },
+)
 SnapshotFileTypeDef = TypedDict(
     "SnapshotFileTypeDef",
     {
-        "SheetSelections": List[SnapshotFileSheetSelectionTypeDef],
+        "SheetSelections": Sequence[SnapshotFileSheetSelectionTypeDef],
         "FormatType": SnapshotFileFormatTypeType,
     },
 )
+StringDatasetParameterOutputTypeDef = TypedDict(
+    "StringDatasetParameterOutputTypeDef",
+    {
+        "Id": str,
+        "Name": str,
+        "ValueType": DatasetParameterValueTypeType,
+        "DefaultValues": NotRequired[StringDatasetParameterDefaultValuesOutputTypeDef],
+    },
+)
 StringDatasetParameterTypeDef = TypedDict(
     "StringDatasetParameterTypeDef",
     {
         "Id": str,
         "Name": str,
         "ValueType": DatasetParameterValueTypeType,
         "DefaultValues": NotRequired[StringDatasetParameterDefaultValuesTypeDef],
@@ -7378,49 +8413,92 @@
 )
 WaterfallChartColorConfigurationTypeDef = TypedDict(
     "WaterfallChartColorConfigurationTypeDef",
     {
         "GroupColorConfiguration": NotRequired[WaterfallChartGroupColorConfigurationTypeDef],
     },
 )
+CascadingControlConfigurationOutputTypeDef = TypedDict(
+    "CascadingControlConfigurationOutputTypeDef",
+    {
+        "SourceControls": NotRequired[List[CascadingControlSourceTypeDef]],
+    },
+)
 CascadingControlConfigurationTypeDef = TypedDict(
     "CascadingControlConfigurationTypeDef",
     {
         "SourceControls": NotRequired[Sequence[CascadingControlSourceTypeDef]],
     },
 )
+DateTimeDefaultValuesOutputTypeDef = TypedDict(
+    "DateTimeDefaultValuesOutputTypeDef",
+    {
+        "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
+        "StaticValues": NotRequired[List[datetime]],
+        "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
+    },
+)
 DateTimeDefaultValuesTypeDef = TypedDict(
     "DateTimeDefaultValuesTypeDef",
     {
         "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
         "StaticValues": NotRequired[Sequence[TimestampTypeDef]],
         "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
     },
 )
+DecimalDefaultValuesOutputTypeDef = TypedDict(
+    "DecimalDefaultValuesOutputTypeDef",
+    {
+        "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
+        "StaticValues": NotRequired[List[float]],
+    },
+)
 DecimalDefaultValuesTypeDef = TypedDict(
     "DecimalDefaultValuesTypeDef",
     {
         "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
         "StaticValues": NotRequired[Sequence[float]],
     },
 )
+IntegerDefaultValuesOutputTypeDef = TypedDict(
+    "IntegerDefaultValuesOutputTypeDef",
+    {
+        "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
+        "StaticValues": NotRequired[List[int]],
+    },
+)
 IntegerDefaultValuesTypeDef = TypedDict(
     "IntegerDefaultValuesTypeDef",
     {
         "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
         "StaticValues": NotRequired[Sequence[int]],
     },
 )
+StringDefaultValuesOutputTypeDef = TypedDict(
+    "StringDefaultValuesOutputTypeDef",
+    {
+        "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
+        "StaticValues": NotRequired[List[str]],
+    },
+)
 StringDefaultValuesTypeDef = TypedDict(
     "StringDefaultValuesTypeDef",
     {
         "DynamicValue": NotRequired[DynamicDefaultValueTypeDef],
         "StaticValues": NotRequired[Sequence[str]],
     },
 )
+DrillDownFilterOutputTypeDef = TypedDict(
+    "DrillDownFilterOutputTypeDef",
+    {
+        "NumericEqualityFilter": NotRequired[NumericEqualityDrillDownFilterTypeDef],
+        "CategoryFilter": NotRequired[CategoryDrillDownFilterOutputTypeDef],
+        "TimeRangeFilter": NotRequired[TimeRangeDrillDownFilterOutputTypeDef],
+    },
+)
 AnalysisTypeDef = TypedDict(
     "AnalysisTypeDef",
     {
         "AnalysisId": NotRequired[str],
         "Arn": NotRequired[str],
         "Name": NotRequired[str],
         "Status": NotRequired[ResourceStatusType],
@@ -7468,14 +8546,15 @@
 )
 AnonymousUserEmbeddingExperienceConfigurationTypeDef = TypedDict(
     "AnonymousUserEmbeddingExperienceConfigurationTypeDef",
     {
         "Dashboard": NotRequired[AnonymousUserDashboardEmbeddingConfigurationTypeDef],
         "DashboardVisual": NotRequired[AnonymousUserDashboardVisualEmbeddingConfigurationTypeDef],
         "QSearchBar": NotRequired[AnonymousUserQSearchBarEmbeddingConfigurationTypeDef],
+        "GenerativeQnA": NotRequired[AnonymousUserGenerativeQnAEmbeddingConfigurationTypeDef],
     },
 )
 DescribeAssetBundleExportJobResponseTypeDef = TypedDict(
     "DescribeAssetBundleExportJobResponseTypeDef",
     {
         "JobStatus": AssetBundleExportJobStatusType,
         "DownloadUrl": str,
@@ -7483,24 +8562,28 @@
         "Arn": str,
         "CreatedTime": datetime,
         "AssetBundleExportJobId": str,
         "AwsAccountId": str,
         "ResourceArns": List[str],
         "IncludeAllDependencies": bool,
         "ExportFormat": AssetBundleExportFormatType,
-        "CloudFormationOverridePropertyConfiguration": AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
+        "CloudFormationOverridePropertyConfiguration": AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
         "RequestId": str,
         "Status": int,
         "IncludePermissions": bool,
         "IncludeTags": bool,
         "ValidationStrategy": AssetBundleExportJobValidationStrategyTypeDef,
         "Warnings": List[AssetBundleExportJobWarningTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AssetBundleCloudFormationOverridePropertyConfigurationUnionTypeDef = Union[
+    AssetBundleCloudFormationOverridePropertyConfigurationTypeDef,
+    AssetBundleCloudFormationOverridePropertyConfigurationOutputTypeDef,
+]
 StartAssetBundleExportJobRequestRequestTypeDef = TypedDict(
     "StartAssetBundleExportJobRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AssetBundleExportJobId": str,
         "ResourceArns": Sequence[str],
         "ExportFormat": AssetBundleExportFormatType,
@@ -7509,119 +8592,56 @@
             AssetBundleCloudFormationOverridePropertyConfigurationTypeDef
         ],
         "IncludePermissions": NotRequired[bool],
         "IncludeTags": NotRequired[bool],
         "ValidationStrategy": NotRequired[AssetBundleExportJobValidationStrategyTypeDef],
     },
 )
-AssetBundleImportJobDashboardOverridePermissionsTypeDef = TypedDict(
-    "AssetBundleImportJobDashboardOverridePermissionsTypeDef",
+AssetBundleImportJobDashboardOverridePermissionsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobDashboardOverridePermissionsOutputTypeDef",
     {
         "DashboardIds": List[str],
-        "Permissions": NotRequired[AssetBundleResourcePermissionsTypeDef],
-        "LinkSharingConfiguration": NotRequired[AssetBundleResourceLinkSharingConfigurationTypeDef],
-    },
-)
-AssetBundleImportJobOverrideTagsTypeDef = TypedDict(
-    "AssetBundleImportJobOverrideTagsTypeDef",
-    {
-        "VPCConnections": NotRequired[List[AssetBundleImportJobVPCConnectionOverrideTagsTypeDef]],
-        "DataSources": NotRequired[List[AssetBundleImportJobDataSourceOverrideTagsTypeDef]],
-        "DataSets": NotRequired[List[AssetBundleImportJobDataSetOverrideTagsTypeDef]],
-        "Themes": NotRequired[List[AssetBundleImportJobThemeOverrideTagsTypeDef]],
-        "Analyses": NotRequired[List[AssetBundleImportJobAnalysisOverrideTagsTypeDef]],
-        "Dashboards": NotRequired[List[AssetBundleImportJobDashboardOverrideTagsTypeDef]],
-    },
-)
-NumericAxisOptionsTypeDef = TypedDict(
-    "NumericAxisOptionsTypeDef",
-    {
-        "Scale": NotRequired[AxisScaleTypeDef],
-        "Range": NotRequired[AxisDisplayRangeTypeDef],
-    },
-)
-ClusterMarkerConfigurationTypeDef = TypedDict(
-    "ClusterMarkerConfigurationTypeDef",
-    {
-        "ClusterMarker": NotRequired[ClusterMarkerTypeDef],
-    },
-)
-TopicCategoryFilterTypeDef = TypedDict(
-    "TopicCategoryFilterTypeDef",
-    {
-        "CategoryFilterFunction": NotRequired[CategoryFilterFunctionType],
-        "CategoryFilterType": NotRequired[CategoryFilterTypeType],
-        "Constant": NotRequired[TopicCategoryFilterConstantTypeDef],
-        "Inverse": NotRequired[bool],
-    },
-)
-TagColumnOperationTypeDef = TypedDict(
-    "TagColumnOperationTypeDef",
-    {
-        "ColumnName": str,
-        "Tags": Sequence[ColumnTagTypeDef],
-    },
-)
-DataSetConfigurationTypeDef = TypedDict(
-    "DataSetConfigurationTypeDef",
-    {
-        "Placeholder": NotRequired[str],
-        "DataSetSchema": NotRequired[DataSetSchemaTypeDef],
-        "ColumnGroupSchemaList": NotRequired[Sequence[ColumnGroupSchemaTypeDef]],
-    },
-)
-ConditionalFormattingIconTypeDef = TypedDict(
-    "ConditionalFormattingIconTypeDef",
-    {
-        "IconSet": NotRequired[ConditionalFormattingIconSetTypeDef],
-        "CustomCondition": NotRequired[ConditionalFormattingCustomIconConditionTypeDef],
-    },
-)
-DescribeDashboardPermissionsResponseTypeDef = TypedDict(
-    "DescribeDashboardPermissionsResponseTypeDef",
-    {
-        "DashboardId": str,
-        "DashboardArn": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "Permissions": NotRequired[AssetBundleResourcePermissionsOutputTypeDef],
+        "LinkSharingConfiguration": NotRequired[
+            AssetBundleResourceLinkSharingConfigurationOutputTypeDef
+        ],
     },
 )
-UpdateDashboardPermissionsResponseTypeDef = TypedDict(
-    "UpdateDashboardPermissionsResponseTypeDef",
+AssetBundleImportJobDashboardOverridePermissionsTypeDef = TypedDict(
+    "AssetBundleImportJobDashboardOverridePermissionsTypeDef",
     {
-        "DashboardArn": str,
-        "DashboardId": str,
-        "Permissions": List[ResourcePermissionTypeDef],
-        "RequestId": str,
-        "Status": int,
-        "LinkSharingConfiguration": LinkSharingConfigurationTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "DashboardIds": Sequence[str],
+        "Permissions": NotRequired[AssetBundleResourcePermissionsTypeDef],
+        "LinkSharingConfiguration": NotRequired[AssetBundleResourceLinkSharingConfigurationTypeDef],
     },
 )
-ListDataSetsResponseTypeDef = TypedDict(
-    "ListDataSetsResponseTypeDef",
+AssetBundleImportJobOverrideTagsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobOverrideTagsOutputTypeDef",
     {
-        "DataSetSummaries": List[DataSetSummaryTypeDef],
-        "NextToken": str,
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "VPCConnections": NotRequired[
+            List[AssetBundleImportJobVPCConnectionOverrideTagsOutputTypeDef]
+        ],
+        "DataSources": NotRequired[List[AssetBundleImportJobDataSourceOverrideTagsOutputTypeDef]],
+        "DataSets": NotRequired[List[AssetBundleImportJobDataSetOverrideTagsOutputTypeDef]],
+        "Themes": NotRequired[List[AssetBundleImportJobThemeOverrideTagsOutputTypeDef]],
+        "Analyses": NotRequired[List[AssetBundleImportJobAnalysisOverrideTagsOutputTypeDef]],
+        "Dashboards": NotRequired[List[AssetBundleImportJobDashboardOverrideTagsOutputTypeDef]],
     },
 )
-SearchDataSetsResponseTypeDef = TypedDict(
-    "SearchDataSetsResponseTypeDef",
+AssetBundleImportJobOverrideTagsTypeDef = TypedDict(
+    "AssetBundleImportJobOverrideTagsTypeDef",
     {
-        "DataSetSummaries": List[DataSetSummaryTypeDef],
-        "NextToken": str,
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
+        "VPCConnections": NotRequired[
+            Sequence[AssetBundleImportJobVPCConnectionOverrideTagsTypeDef]
+        ],
+        "DataSources": NotRequired[Sequence[AssetBundleImportJobDataSourceOverrideTagsTypeDef]],
+        "DataSets": NotRequired[Sequence[AssetBundleImportJobDataSetOverrideTagsTypeDef]],
+        "Themes": NotRequired[Sequence[AssetBundleImportJobThemeOverrideTagsTypeDef]],
+        "Analyses": NotRequired[Sequence[AssetBundleImportJobAnalysisOverrideTagsTypeDef]],
+        "Dashboards": NotRequired[Sequence[AssetBundleImportJobDashboardOverrideTagsTypeDef]],
     },
 )
 CustomValuesConfigurationTypeDef = TypedDict(
     "CustomValuesConfigurationTypeDef",
     {
         "CustomValues": CustomParameterValuesTypeDef,
         "IncludeNullValue": NotRequired[bool],
@@ -7668,35 +8688,17 @@
         "AwsAccountId": str,
         "TopicId": str,
         "DatasetArn": str,
         "RefreshSchedule": TopicRefreshScheduleTypeDef,
         "DatasetName": NotRequired[str],
     },
 )
-DescribeTopicRefreshScheduleResponseTypeDef = TypedDict(
-    "DescribeTopicRefreshScheduleResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "DatasetArn": str,
-        "RefreshSchedule": TopicRefreshScheduleTypeDef,
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-TopicRefreshScheduleSummaryTypeDef = TypedDict(
-    "TopicRefreshScheduleSummaryTypeDef",
-    {
-        "DatasetId": NotRequired[str],
-        "DatasetArn": NotRequired[str],
-        "DatasetName": NotRequired[str],
-        "RefreshSchedule": NotRequired[TopicRefreshScheduleTypeDef],
-    },
-)
+TopicRefreshScheduleUnionTypeDef = Union[
+    TopicRefreshScheduleTypeDef, TopicRefreshScheduleOutputTypeDef
+]
 UpdateTopicRefreshScheduleRequestRequestTypeDef = TypedDict(
     "UpdateTopicRefreshScheduleRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TopicId": str,
         "DatasetId": str,
         "RefreshSchedule": TopicRefreshScheduleTypeDef,
@@ -7705,14 +8707,120 @@
 ForecastScenarioTypeDef = TypedDict(
     "ForecastScenarioTypeDef",
     {
         "WhatIfPointScenario": NotRequired[WhatIfPointScenarioTypeDef],
         "WhatIfRangeScenario": NotRequired[WhatIfRangeScenarioTypeDef],
     },
 )
+NumericAxisOptionsOutputTypeDef = TypedDict(
+    "NumericAxisOptionsOutputTypeDef",
+    {
+        "Scale": NotRequired[AxisScaleTypeDef],
+        "Range": NotRequired[AxisDisplayRangeOutputTypeDef],
+    },
+)
+NumericAxisOptionsTypeDef = TypedDict(
+    "NumericAxisOptionsTypeDef",
+    {
+        "Scale": NotRequired[AxisScaleTypeDef],
+        "Range": NotRequired[AxisDisplayRangeTypeDef],
+    },
+)
+ClusterMarkerConfigurationTypeDef = TypedDict(
+    "ClusterMarkerConfigurationTypeDef",
+    {
+        "ClusterMarker": NotRequired[ClusterMarkerTypeDef],
+    },
+)
+TopicCategoryFilterOutputTypeDef = TypedDict(
+    "TopicCategoryFilterOutputTypeDef",
+    {
+        "CategoryFilterFunction": NotRequired[CategoryFilterFunctionType],
+        "CategoryFilterType": NotRequired[CategoryFilterTypeType],
+        "Constant": NotRequired[TopicCategoryFilterConstantOutputTypeDef],
+        "Inverse": NotRequired[bool],
+    },
+)
+TopicCategoryFilterTypeDef = TypedDict(
+    "TopicCategoryFilterTypeDef",
+    {
+        "CategoryFilterFunction": NotRequired[CategoryFilterFunctionType],
+        "CategoryFilterType": NotRequired[CategoryFilterTypeType],
+        "Constant": NotRequired[TopicCategoryFilterConstantTypeDef],
+        "Inverse": NotRequired[bool],
+    },
+)
+TagColumnOperationOutputTypeDef = TypedDict(
+    "TagColumnOperationOutputTypeDef",
+    {
+        "ColumnName": str,
+        "Tags": List[ColumnTagTypeDef],
+    },
+)
+TagColumnOperationTypeDef = TypedDict(
+    "TagColumnOperationTypeDef",
+    {
+        "ColumnName": str,
+        "Tags": Sequence[ColumnTagTypeDef],
+    },
+)
+ColumnGroupUnionTypeDef = Union[ColumnGroupTypeDef, ColumnGroupOutputTypeDef]
+DataSetConfigurationOutputTypeDef = TypedDict(
+    "DataSetConfigurationOutputTypeDef",
+    {
+        "Placeholder": NotRequired[str],
+        "DataSetSchema": NotRequired[DataSetSchemaOutputTypeDef],
+        "ColumnGroupSchemaList": NotRequired[List[ColumnGroupSchemaOutputTypeDef]],
+    },
+)
+DataSetConfigurationTypeDef = TypedDict(
+    "DataSetConfigurationTypeDef",
+    {
+        "Placeholder": NotRequired[str],
+        "DataSetSchema": NotRequired[DataSetSchemaTypeDef],
+        "ColumnGroupSchemaList": NotRequired[Sequence[ColumnGroupSchemaTypeDef]],
+    },
+)
+ConditionalFormattingIconTypeDef = TypedDict(
+    "ConditionalFormattingIconTypeDef",
+    {
+        "IconSet": NotRequired[ConditionalFormattingIconSetTypeDef],
+        "CustomCondition": NotRequired[ConditionalFormattingCustomIconConditionTypeDef],
+    },
+)
+ListDataSetsResponseTypeDef = TypedDict(
+    "ListDataSetsResponseTypeDef",
+    {
+        "DataSetSummaries": List[DataSetSummaryTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+SearchDataSetsResponseTypeDef = TypedDict(
+    "SearchDataSetsResponseTypeDef",
+    {
+        "DataSetSummaries": List[DataSetSummaryTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+DestinationParameterValueConfigurationOutputTypeDef = TypedDict(
+    "DestinationParameterValueConfigurationOutputTypeDef",
+    {
+        "CustomValuesConfiguration": NotRequired[CustomValuesConfigurationOutputTypeDef],
+        "SelectAllValueOptions": NotRequired[Literal["ALL_VALUES"]],
+        "SourceParameterName": NotRequired[str],
+        "SourceField": NotRequired[str],
+        "SourceColumn": NotRequired[ColumnIdentifierTypeDef],
+    },
+)
 CustomContentConfigurationTypeDef = TypedDict(
     "CustomContentConfigurationTypeDef",
     {
         "ContentUrl": NotRequired[str],
         "ContentType": NotRequired[CustomContentTypeType],
         "ImageScaling": NotRequired[CustomContentImageScalingConfigurationType],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
@@ -7740,42 +8848,105 @@
     "DataPathColorTypeDef",
     {
         "Element": DataPathValueTypeDef,
         "Color": str,
         "TimeGranularity": NotRequired[TimeGranularityType],
     },
 )
+DataPathSortOutputTypeDef = TypedDict(
+    "DataPathSortOutputTypeDef",
+    {
+        "Direction": SortDirectionType,
+        "SortPaths": List[DataPathValueTypeDef],
+    },
+)
 DataPathSortTypeDef = TypedDict(
     "DataPathSortTypeDef",
     {
         "Direction": SortDirectionType,
         "SortPaths": Sequence[DataPathValueTypeDef],
     },
 )
+PivotTableDataPathOptionOutputTypeDef = TypedDict(
+    "PivotTableDataPathOptionOutputTypeDef",
+    {
+        "DataPathList": List[DataPathValueTypeDef],
+        "Width": NotRequired[str],
+    },
+)
 PivotTableDataPathOptionTypeDef = TypedDict(
     "PivotTableDataPathOptionTypeDef",
     {
         "DataPathList": Sequence[DataPathValueTypeDef],
         "Width": NotRequired[str],
     },
 )
+PivotTableFieldCollapseStateTargetOutputTypeDef = TypedDict(
+    "PivotTableFieldCollapseStateTargetOutputTypeDef",
+    {
+        "FieldId": NotRequired[str],
+        "FieldDataPathValues": NotRequired[List[DataPathValueTypeDef]],
+    },
+)
 PivotTableFieldCollapseStateTargetTypeDef = TypedDict(
     "PivotTableFieldCollapseStateTargetTypeDef",
     {
         "FieldId": NotRequired[str],
         "FieldDataPathValues": NotRequired[Sequence[DataPathValueTypeDef]],
     },
 )
+DescribeDashboardPermissionsResponseTypeDef = TypedDict(
+    "DescribeDashboardPermissionsResponseTypeDef",
+    {
+        "DashboardId": str,
+        "DashboardArn": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "LinkSharingConfiguration": LinkSharingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+UpdateDashboardPermissionsResponseTypeDef = TypedDict(
+    "UpdateDashboardPermissionsResponseTypeDef",
+    {
+        "DashboardArn": str,
+        "DashboardId": str,
+        "Permissions": List[ResourcePermissionOutputTypeDef],
+        "RequestId": str,
+        "Status": int,
+        "LinkSharingConfiguration": LinkSharingConfigurationOutputTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ListTopicRefreshSchedulesResponseTypeDef = TypedDict(
+    "ListTopicRefreshSchedulesResponseTypeDef",
+    {
+        "TopicId": str,
+        "TopicArn": str,
+        "RefreshSchedules": List[TopicRefreshScheduleSummaryTypeDef],
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DefaultFormattingTypeDef = TypedDict(
     "DefaultFormattingTypeDef",
     {
         "DisplayFormat": NotRequired[DisplayFormatType],
         "DisplayFormatOptions": NotRequired[DisplayFormatOptionsTypeDef],
     },
 )
+CustomActionFilterOperationOutputTypeDef = TypedDict(
+    "CustomActionFilterOperationOutputTypeDef",
+    {
+        "SelectedFieldsConfiguration": FilterOperationSelectedFieldsConfigurationOutputTypeDef,
+        "TargetVisualsConfiguration": FilterOperationTargetVisualsConfigurationOutputTypeDef,
+    },
+)
 CustomActionFilterOperationTypeDef = TypedDict(
     "CustomActionFilterOperationTypeDef",
     {
         "SelectedFieldsConfiguration": FilterOperationSelectedFieldsConfigurationTypeDef,
         "TargetVisualsConfiguration": FilterOperationTargetVisualsConfigurationTypeDef,
     },
 )
@@ -7783,14 +8954,29 @@
     "AxisLabelOptionsTypeDef",
     {
         "FontConfiguration": NotRequired[FontConfigurationTypeDef],
         "CustomLabel": NotRequired[str],
         "ApplyTo": NotRequired[AxisLabelReferenceOptionsTypeDef],
     },
 )
+DataLabelOptionsOutputTypeDef = TypedDict(
+    "DataLabelOptionsOutputTypeDef",
+    {
+        "Visibility": NotRequired[VisibilityType],
+        "CategoryLabelVisibility": NotRequired[VisibilityType],
+        "MeasureLabelVisibility": NotRequired[VisibilityType],
+        "DataLabelTypes": NotRequired[List[DataLabelTypeTypeDef]],
+        "Position": NotRequired[DataLabelPositionType],
+        "LabelContent": NotRequired[DataLabelContentType],
+        "LabelFontConfiguration": NotRequired[FontConfigurationTypeDef],
+        "LabelColor": NotRequired[str],
+        "Overlap": NotRequired[DataLabelOverlapType],
+        "TotalsVisibility": NotRequired[VisibilityType],
+    },
+)
 DataLabelOptionsTypeDef = TypedDict(
     "DataLabelOptionsTypeDef",
     {
         "Visibility": NotRequired[VisibilityType],
         "CategoryLabelVisibility": NotRequired[VisibilityType],
         "MeasureLabelVisibility": NotRequired[VisibilityType],
         "DataLabelTypes": NotRequired[Sequence[DataLabelTypeTypeDef]],
@@ -7833,52 +9019,79 @@
 TableFieldCustomTextContentTypeDef = TypedDict(
     "TableFieldCustomTextContentTypeDef",
     {
         "FontConfiguration": FontConfigurationTypeDef,
         "Value": NotRequired[str],
     },
 )
+ForecastConfigurationOutputTypeDef = TypedDict(
+    "ForecastConfigurationOutputTypeDef",
+    {
+        "ForecastProperties": NotRequired[TimeBasedForecastPropertiesTypeDef],
+        "Scenario": NotRequired[ForecastScenarioOutputTypeDef],
+    },
+)
 DefaultFreeFormLayoutConfigurationTypeDef = TypedDict(
     "DefaultFreeFormLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": FreeFormLayoutCanvasSizeOptionsTypeDef,
     },
 )
 SnapshotUserConfigurationTypeDef = TypedDict(
     "SnapshotUserConfigurationTypeDef",
     {
         "AnonymousUsers": NotRequired[Sequence[SnapshotAnonymousUserTypeDef]],
     },
 )
+GeospatialHeatmapConfigurationOutputTypeDef = TypedDict(
+    "GeospatialHeatmapConfigurationOutputTypeDef",
+    {
+        "HeatmapColor": NotRequired[GeospatialHeatmapColorScaleOutputTypeDef],
+    },
+)
 GeospatialHeatmapConfigurationTypeDef = TypedDict(
     "GeospatialHeatmapConfigurationTypeDef",
     {
         "HeatmapColor": NotRequired[GeospatialHeatmapColorScaleTypeDef],
     },
 )
 GlobalTableBorderOptionsTypeDef = TypedDict(
     "GlobalTableBorderOptionsTypeDef",
     {
         "UniformBorder": NotRequired[TableBorderOptionsTypeDef],
         "SideSpecificBorder": NotRequired[TableSideBorderOptionsTypeDef],
     },
 )
+ConditionalFormattingGradientColorOutputTypeDef = TypedDict(
+    "ConditionalFormattingGradientColorOutputTypeDef",
+    {
+        "Expression": str,
+        "Color": GradientColorOutputTypeDef,
+    },
+)
 ConditionalFormattingGradientColorTypeDef = TypedDict(
     "ConditionalFormattingGradientColorTypeDef",
     {
         "Expression": str,
         "Color": GradientColorTypeDef,
     },
 )
 DefaultGridLayoutConfigurationTypeDef = TypedDict(
     "DefaultGridLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": GridLayoutCanvasSizeOptionsTypeDef,
     },
 )
+GridLayoutConfigurationOutputTypeDef = TypedDict(
+    "GridLayoutConfigurationOutputTypeDef",
+    {
+        "Elements": List[GridLayoutElementTypeDef],
+        "CanvasSizeOptions": NotRequired[GridLayoutCanvasSizeOptionsTypeDef],
+    },
+)
 GridLayoutConfigurationTypeDef = TypedDict(
     "GridLayoutConfigurationTypeDef",
     {
         "Elements": Sequence[GridLayoutElementTypeDef],
         "CanvasSizeOptions": NotRequired[GridLayoutCanvasSizeOptionsTypeDef],
     },
 )
@@ -7897,18 +9110,18 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListIngestionsResponseTypeDef = TypedDict(
     "ListIngestionsResponseTypeDef",
     {
         "Ingestions": List[IngestionTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 LogicalTableSourceTypeDef = TypedDict(
     "LogicalTableSourceTypeDef",
     {
         "JoinInstruction": NotRequired[JoinInstructionTypeDef],
         "PhysicalTableId": NotRequired[str],
@@ -7928,21 +9141,121 @@
     "FieldSeriesItemTypeDef",
     {
         "FieldId": str,
         "AxisBinding": AxisBindingType,
         "Settings": NotRequired[LineChartSeriesSettingsTypeDef],
     },
 )
+LinkSharingConfigurationUnionTypeDef = Union[
+    LinkSharingConfigurationTypeDef, LinkSharingConfigurationOutputTypeDef
+]
+CreateFolderRequestRequestTypeDef = TypedDict(
+    "CreateFolderRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "FolderId": str,
+        "Name": NotRequired[str],
+        "FolderType": NotRequired[FolderTypeType],
+        "ParentFolderArn": NotRequired[str],
+        "Permissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "SharingModel": NotRequired[SharingModelType],
+    },
+)
+UpdateAnalysisPermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateAnalysisPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "AnalysisId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
+UpdateDashboardPermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateDashboardPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DashboardId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "GrantLinkPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokeLinkPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
+UpdateDataSetPermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateDataSetPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DataSetId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
+UpdateDataSourcePermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateDataSourcePermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DataSourceId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
+UpdateFolderPermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateFolderPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "FolderId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
+UpdateTemplatePermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateTemplatePermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "TemplateId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
+UpdateThemePermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateThemePermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "ThemeId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
+UpdateTopicPermissionsRequestRequestTypeDef = TypedDict(
+    "UpdateTopicPermissionsRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "TopicId": str,
+        "GrantPermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RevokePermissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+    },
+)
 SheetStyleTypeDef = TypedDict(
     "SheetStyleTypeDef",
     {
         "Tile": NotRequired[TileStyleTypeDef],
         "TileLayout": NotRequired[TileLayoutStyleTypeDef],
     },
 )
+TopicNamedEntityOutputTypeDef = TypedDict(
+    "TopicNamedEntityOutputTypeDef",
+    {
+        "EntityName": str,
+        "EntityDescription": NotRequired[str],
+        "EntitySynonyms": NotRequired[List[str]],
+        "SemanticEntityType": NotRequired[SemanticEntityTypeOutputTypeDef],
+        "Definition": NotRequired[List[NamedEntityDefinitionOutputTypeDef]],
+    },
+)
 TopicNamedEntityTypeDef = TypedDict(
     "TopicNamedEntityTypeDef",
     {
         "EntityName": str,
         "EntityDescription": NotRequired[str],
         "EntitySynonyms": NotRequired[Sequence[str]],
         "SemanticEntityType": NotRequired[SemanticEntityTypeTypeDef],
@@ -7958,28 +9271,28 @@
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListNamespacesResponseTypeDef = TypedDict(
     "ListNamespacesResponseTypeDef",
     {
         "Namespaces": List[NamespaceInfoV2TypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 ListVPCConnectionsResponseTypeDef = TypedDict(
     "ListVPCConnectionsResponseTypeDef",
     {
         "VPCConnectionSummaries": List[VPCConnectionSummaryTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
     },
 )
 DescribeVPCConnectionResponseTypeDef = TypedDict(
     "DescribeVPCConnectionResponseTypeDef",
     {
         "VPCConnection": VPCConnectionTypeDef,
         "RequestId": str,
@@ -8050,30 +9363,61 @@
     "TopicNumericRangeFilterTypeDef",
     {
         "Inclusive": NotRequired[bool],
         "Constant": NotRequired[TopicRangeFilterConstantTypeDef],
         "Aggregation": NotRequired[NamedFilterAggTypeType],
     },
 )
-DataSourceParametersPaginatorTypeDef = TypedDict(
-    "DataSourceParametersPaginatorTypeDef",
+DataSourceParametersExtraOutputTypeDef = TypedDict(
+    "DataSourceParametersExtraOutputTypeDef",
+    {
+        "AmazonElasticsearchParameters": NotRequired[AmazonElasticsearchParametersTypeDef],
+        "AthenaParameters": NotRequired[AthenaParametersTypeDef],
+        "AuroraParameters": NotRequired[AuroraParametersTypeDef],
+        "AuroraPostgreSqlParameters": NotRequired[AuroraPostgreSqlParametersTypeDef],
+        "AwsIotAnalyticsParameters": NotRequired[AwsIotAnalyticsParametersTypeDef],
+        "JiraParameters": NotRequired[JiraParametersTypeDef],
+        "MariaDbParameters": NotRequired[MariaDbParametersTypeDef],
+        "MySqlParameters": NotRequired[MySqlParametersTypeDef],
+        "OracleParameters": NotRequired[OracleParametersTypeDef],
+        "PostgreSqlParameters": NotRequired[PostgreSqlParametersTypeDef],
+        "PrestoParameters": NotRequired[PrestoParametersTypeDef],
+        "RdsParameters": NotRequired[RdsParametersTypeDef],
+        "RedshiftParameters": NotRequired[RedshiftParametersExtraOutputTypeDef],
+        "S3Parameters": NotRequired[S3ParametersTypeDef],
+        "ServiceNowParameters": NotRequired[ServiceNowParametersTypeDef],
+        "SnowflakeParameters": NotRequired[SnowflakeParametersTypeDef],
+        "SparkParameters": NotRequired[SparkParametersTypeDef],
+        "SqlServerParameters": NotRequired[SqlServerParametersTypeDef],
+        "TeradataParameters": NotRequired[TeradataParametersTypeDef],
+        "TwitterParameters": NotRequired[TwitterParametersTypeDef],
+        "AmazonOpenSearchParameters": NotRequired[AmazonOpenSearchParametersTypeDef],
+        "ExasolParameters": NotRequired[ExasolParametersTypeDef],
+        "DatabricksParameters": NotRequired[DatabricksParametersTypeDef],
+        "StarburstParameters": NotRequired[StarburstParametersTypeDef],
+        "TrinoParameters": NotRequired[TrinoParametersTypeDef],
+        "BigQueryParameters": NotRequired[BigQueryParametersTypeDef],
+    },
+)
+DataSourceParametersOutputTypeDef = TypedDict(
+    "DataSourceParametersOutputTypeDef",
     {
         "AmazonElasticsearchParameters": NotRequired[AmazonElasticsearchParametersTypeDef],
         "AthenaParameters": NotRequired[AthenaParametersTypeDef],
         "AuroraParameters": NotRequired[AuroraParametersTypeDef],
         "AuroraPostgreSqlParameters": NotRequired[AuroraPostgreSqlParametersTypeDef],
         "AwsIotAnalyticsParameters": NotRequired[AwsIotAnalyticsParametersTypeDef],
         "JiraParameters": NotRequired[JiraParametersTypeDef],
         "MariaDbParameters": NotRequired[MariaDbParametersTypeDef],
         "MySqlParameters": NotRequired[MySqlParametersTypeDef],
         "OracleParameters": NotRequired[OracleParametersTypeDef],
         "PostgreSqlParameters": NotRequired[PostgreSqlParametersTypeDef],
         "PrestoParameters": NotRequired[PrestoParametersTypeDef],
         "RdsParameters": NotRequired[RdsParametersTypeDef],
-        "RedshiftParameters": NotRequired[RedshiftParametersPaginatorTypeDef],
+        "RedshiftParameters": NotRequired[RedshiftParametersOutputTypeDef],
         "S3Parameters": NotRequired[S3ParametersTypeDef],
         "ServiceNowParameters": NotRequired[ServiceNowParametersTypeDef],
         "SnowflakeParameters": NotRequired[SnowflakeParametersTypeDef],
         "SparkParameters": NotRequired[SparkParametersTypeDef],
         "SqlServerParameters": NotRequired[SqlServerParametersTypeDef],
         "TeradataParameters": NotRequired[TeradataParametersTypeDef],
         "TwitterParameters": NotRequired[TwitterParametersTypeDef],
@@ -8112,14 +9456,24 @@
         "ExasolParameters": NotRequired[ExasolParametersTypeDef],
         "DatabricksParameters": NotRequired[DatabricksParametersTypeDef],
         "StarburstParameters": NotRequired[StarburstParametersTypeDef],
         "TrinoParameters": NotRequired[TrinoParametersTypeDef],
         "BigQueryParameters": NotRequired[BigQueryParametersTypeDef],
     },
 )
+RefreshScheduleOutputTypeDef = TypedDict(
+    "RefreshScheduleOutputTypeDef",
+    {
+        "ScheduleId": str,
+        "ScheduleFrequency": RefreshFrequencyTypeDef,
+        "RefreshType": IngestionTypeType,
+        "StartAfterDateTime": NotRequired[datetime],
+        "Arn": NotRequired[str],
+    },
+)
 RefreshScheduleTypeDef = TypedDict(
     "RefreshScheduleTypeDef",
     {
         "ScheduleId": str,
         "ScheduleFrequency": RefreshFrequencyTypeDef,
         "RefreshType": IngestionTypeType,
         "StartAfterDateTime": NotRequired[TimestampTypeDef],
@@ -8136,49 +9490,90 @@
 RegisteredUserDashboardEmbeddingConfigurationTypeDef = TypedDict(
     "RegisteredUserDashboardEmbeddingConfigurationTypeDef",
     {
         "InitialDashboardId": str,
         "FeatureConfigurations": NotRequired[RegisteredUserDashboardFeatureConfigurationsTypeDef],
     },
 )
+RowLevelPermissionTagConfigurationUnionTypeDef = Union[
+    RowLevelPermissionTagConfigurationTypeDef, RowLevelPermissionTagConfigurationOutputTypeDef
+]
+SnapshotDestinationConfigurationOutputTypeDef = TypedDict(
+    "SnapshotDestinationConfigurationOutputTypeDef",
+    {
+        "S3Destinations": NotRequired[List[SnapshotS3DestinationConfigurationTypeDef]],
+    },
+)
 SnapshotDestinationConfigurationTypeDef = TypedDict(
     "SnapshotDestinationConfigurationTypeDef",
     {
-        "S3Destinations": NotRequired[List[SnapshotS3DestinationConfigurationTypeDef]],
+        "S3Destinations": NotRequired[Sequence[SnapshotS3DestinationConfigurationTypeDef]],
     },
 )
 SnapshotJobS3ResultTypeDef = TypedDict(
     "SnapshotJobS3ResultTypeDef",
     {
         "S3DestinationConfiguration": NotRequired[SnapshotS3DestinationConfigurationTypeDef],
         "S3Uri": NotRequired[str],
         "ErrorInfo": NotRequired[List[SnapshotJobResultErrorInfoTypeDef]],
     },
 )
+PhysicalTableOutputTypeDef = TypedDict(
+    "PhysicalTableOutputTypeDef",
+    {
+        "RelationalTable": NotRequired[RelationalTableOutputTypeDef],
+        "CustomSql": NotRequired[CustomSqlOutputTypeDef],
+        "S3Source": NotRequired[S3SourceOutputTypeDef],
+    },
+)
 PhysicalTableTypeDef = TypedDict(
     "PhysicalTableTypeDef",
     {
         "RelationalTable": NotRequired[RelationalTableTypeDef],
         "CustomSql": NotRequired[CustomSqlTypeDef],
         "S3Source": NotRequired[S3SourceTypeDef],
     },
 )
 SectionBasedLayoutCanvasSizeOptionsTypeDef = TypedDict(
     "SectionBasedLayoutCanvasSizeOptionsTypeDef",
     {
         "PaperCanvasSizeOptions": NotRequired[SectionBasedLayoutPaperCanvasSizeOptionsTypeDef],
     },
 )
+FilterScopeConfigurationOutputTypeDef = TypedDict(
+    "FilterScopeConfigurationOutputTypeDef",
+    {
+        "SelectedSheets": NotRequired[SelectedSheetsFilterScopeConfigurationOutputTypeDef],
+        "AllSheets": NotRequired[Dict[str, Any]],
+    },
+)
 FilterScopeConfigurationTypeDef = TypedDict(
     "FilterScopeConfigurationTypeDef",
     {
         "SelectedSheets": NotRequired[SelectedSheetsFilterScopeConfigurationTypeDef],
         "AllSheets": NotRequired[Mapping[str, Any]],
     },
 )
+FreeFormLayoutElementOutputTypeDef = TypedDict(
+    "FreeFormLayoutElementOutputTypeDef",
+    {
+        "ElementId": str,
+        "ElementType": LayoutElementTypeType,
+        "XAxisLocation": str,
+        "YAxisLocation": str,
+        "Width": str,
+        "Height": str,
+        "Visibility": NotRequired[VisibilityType],
+        "RenderingRules": NotRequired[List[SheetElementRenderingRuleTypeDef]],
+        "BorderStyle": NotRequired[FreeFormLayoutElementBorderStyleTypeDef],
+        "SelectedBorderStyle": NotRequired[FreeFormLayoutElementBorderStyleTypeDef],
+        "BackgroundStyle": NotRequired[FreeFormLayoutElementBackgroundStyleTypeDef],
+        "LoadingAnimation": NotRequired[LoadingAnimationTypeDef],
+    },
+)
 FreeFormLayoutElementTypeDef = TypedDict(
     "FreeFormLayoutElementTypeDef",
     {
         "ElementId": str,
         "ElementType": LayoutElementTypeType,
         "XAxisLocation": str,
         "YAxisLocation": str,
@@ -8188,68 +9583,154 @@
         "RenderingRules": NotRequired[Sequence[SheetElementRenderingRuleTypeDef]],
         "BorderStyle": NotRequired[FreeFormLayoutElementBorderStyleTypeDef],
         "SelectedBorderStyle": NotRequired[FreeFormLayoutElementBorderStyleTypeDef],
         "BackgroundStyle": NotRequired[FreeFormLayoutElementBackgroundStyleTypeDef],
         "LoadingAnimation": NotRequired[LoadingAnimationTypeDef],
     },
 )
+SnapshotFileGroupOutputTypeDef = TypedDict(
+    "SnapshotFileGroupOutputTypeDef",
+    {
+        "Files": NotRequired[List[SnapshotFileOutputTypeDef]],
+    },
+)
 SnapshotFileGroupTypeDef = TypedDict(
     "SnapshotFileGroupTypeDef",
     {
-        "Files": NotRequired[List[SnapshotFileTypeDef]],
+        "Files": NotRequired[Sequence[SnapshotFileTypeDef]],
+    },
+)
+DatasetParameterOutputTypeDef = TypedDict(
+    "DatasetParameterOutputTypeDef",
+    {
+        "StringDatasetParameter": NotRequired[StringDatasetParameterOutputTypeDef],
+        "DecimalDatasetParameter": NotRequired[DecimalDatasetParameterOutputTypeDef],
+        "IntegerDatasetParameter": NotRequired[IntegerDatasetParameterOutputTypeDef],
+        "DateTimeDatasetParameter": NotRequired[DateTimeDatasetParameterOutputTypeDef],
+    },
+)
+FilterCrossSheetControlOutputTypeDef = TypedDict(
+    "FilterCrossSheetControlOutputTypeDef",
+    {
+        "FilterControlId": str,
+        "SourceFilterId": str,
+        "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationOutputTypeDef],
     },
 )
 FilterCrossSheetControlTypeDef = TypedDict(
     "FilterCrossSheetControlTypeDef",
     {
         "FilterControlId": str,
         "SourceFilterId": str,
         "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationTypeDef],
     },
 )
+DateTimeParameterDeclarationOutputTypeDef = TypedDict(
+    "DateTimeParameterDeclarationOutputTypeDef",
+    {
+        "Name": str,
+        "DefaultValues": NotRequired[DateTimeDefaultValuesOutputTypeDef],
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "ValueWhenUnset": NotRequired[DateTimeValueWhenUnsetConfigurationOutputTypeDef],
+        "MappedDataSetParameters": NotRequired[List[MappedDataSetParameterTypeDef]],
+    },
+)
 DateTimeParameterDeclarationTypeDef = TypedDict(
     "DateTimeParameterDeclarationTypeDef",
     {
         "Name": str,
         "DefaultValues": NotRequired[DateTimeDefaultValuesTypeDef],
         "TimeGranularity": NotRequired[TimeGranularityType],
         "ValueWhenUnset": NotRequired[DateTimeValueWhenUnsetConfigurationTypeDef],
         "MappedDataSetParameters": NotRequired[Sequence[MappedDataSetParameterTypeDef]],
     },
 )
+DecimalParameterDeclarationOutputTypeDef = TypedDict(
+    "DecimalParameterDeclarationOutputTypeDef",
+    {
+        "ParameterValueType": ParameterValueTypeType,
+        "Name": str,
+        "DefaultValues": NotRequired[DecimalDefaultValuesOutputTypeDef],
+        "ValueWhenUnset": NotRequired[DecimalValueWhenUnsetConfigurationTypeDef],
+        "MappedDataSetParameters": NotRequired[List[MappedDataSetParameterTypeDef]],
+    },
+)
 DecimalParameterDeclarationTypeDef = TypedDict(
     "DecimalParameterDeclarationTypeDef",
     {
         "ParameterValueType": ParameterValueTypeType,
         "Name": str,
         "DefaultValues": NotRequired[DecimalDefaultValuesTypeDef],
         "ValueWhenUnset": NotRequired[DecimalValueWhenUnsetConfigurationTypeDef],
         "MappedDataSetParameters": NotRequired[Sequence[MappedDataSetParameterTypeDef]],
     },
 )
+IntegerParameterDeclarationOutputTypeDef = TypedDict(
+    "IntegerParameterDeclarationOutputTypeDef",
+    {
+        "ParameterValueType": ParameterValueTypeType,
+        "Name": str,
+        "DefaultValues": NotRequired[IntegerDefaultValuesOutputTypeDef],
+        "ValueWhenUnset": NotRequired[IntegerValueWhenUnsetConfigurationTypeDef],
+        "MappedDataSetParameters": NotRequired[List[MappedDataSetParameterTypeDef]],
+    },
+)
 IntegerParameterDeclarationTypeDef = TypedDict(
     "IntegerParameterDeclarationTypeDef",
     {
         "ParameterValueType": ParameterValueTypeType,
         "Name": str,
         "DefaultValues": NotRequired[IntegerDefaultValuesTypeDef],
         "ValueWhenUnset": NotRequired[IntegerValueWhenUnsetConfigurationTypeDef],
         "MappedDataSetParameters": NotRequired[Sequence[MappedDataSetParameterTypeDef]],
     },
 )
+StringParameterDeclarationOutputTypeDef = TypedDict(
+    "StringParameterDeclarationOutputTypeDef",
+    {
+        "ParameterValueType": ParameterValueTypeType,
+        "Name": str,
+        "DefaultValues": NotRequired[StringDefaultValuesOutputTypeDef],
+        "ValueWhenUnset": NotRequired[StringValueWhenUnsetConfigurationTypeDef],
+        "MappedDataSetParameters": NotRequired[List[MappedDataSetParameterTypeDef]],
+    },
+)
 StringParameterDeclarationTypeDef = TypedDict(
     "StringParameterDeclarationTypeDef",
     {
         "ParameterValueType": ParameterValueTypeType,
         "Name": str,
         "DefaultValues": NotRequired[StringDefaultValuesTypeDef],
         "ValueWhenUnset": NotRequired[StringValueWhenUnsetConfigurationTypeDef],
         "MappedDataSetParameters": NotRequired[Sequence[MappedDataSetParameterTypeDef]],
     },
 )
+DateTimeHierarchyOutputTypeDef = TypedDict(
+    "DateTimeHierarchyOutputTypeDef",
+    {
+        "HierarchyId": str,
+        "DrillDownFilters": NotRequired[List[DrillDownFilterOutputTypeDef]],
+    },
+)
+ExplicitHierarchyOutputTypeDef = TypedDict(
+    "ExplicitHierarchyOutputTypeDef",
+    {
+        "HierarchyId": str,
+        "Columns": List[ColumnIdentifierTypeDef],
+        "DrillDownFilters": NotRequired[List[DrillDownFilterOutputTypeDef]],
+    },
+)
+PredefinedHierarchyOutputTypeDef = TypedDict(
+    "PredefinedHierarchyOutputTypeDef",
+    {
+        "HierarchyId": str,
+        "Columns": List[ColumnIdentifierTypeDef],
+        "DrillDownFilters": NotRequired[List[DrillDownFilterOutputTypeDef]],
+    },
+)
 DescribeAnalysisResponseTypeDef = TypedDict(
     "DescribeAnalysisResponseTypeDef",
     {
         "Analysis": AnalysisTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -8276,45 +9757,45 @@
         "AuthorizedResourceArns": Sequence[str],
         "ExperienceConfiguration": AnonymousUserEmbeddingExperienceConfigurationTypeDef,
         "SessionLifetimeInMinutes": NotRequired[int],
         "SessionTags": NotRequired[Sequence[SessionTagTypeDef]],
         "AllowedDomains": NotRequired[Sequence[str]],
     },
 )
-AssetBundleImportJobOverridePermissionsTypeDef = TypedDict(
-    "AssetBundleImportJobOverridePermissionsTypeDef",
+AssetBundleImportJobOverridePermissionsOutputTypeDef = TypedDict(
+    "AssetBundleImportJobOverridePermissionsOutputTypeDef",
     {
-        "DataSources": NotRequired[List[AssetBundleImportJobDataSourceOverridePermissionsTypeDef]],
-        "DataSets": NotRequired[List[AssetBundleImportJobDataSetOverridePermissionsTypeDef]],
-        "Themes": NotRequired[List[AssetBundleImportJobThemeOverridePermissionsTypeDef]],
-        "Analyses": NotRequired[List[AssetBundleImportJobAnalysisOverridePermissionsTypeDef]],
-        "Dashboards": NotRequired[List[AssetBundleImportJobDashboardOverridePermissionsTypeDef]],
-    },
-)
-AxisDataOptionsTypeDef = TypedDict(
-    "AxisDataOptionsTypeDef",
-    {
-        "NumericAxisOptions": NotRequired[NumericAxisOptionsTypeDef],
-        "DateAxisOptions": NotRequired[DateAxisOptionsTypeDef],
+        "DataSources": NotRequired[
+            List[AssetBundleImportJobDataSourceOverridePermissionsOutputTypeDef]
+        ],
+        "DataSets": NotRequired[List[AssetBundleImportJobDataSetOverridePermissionsOutputTypeDef]],
+        "Themes": NotRequired[List[AssetBundleImportJobThemeOverridePermissionsOutputTypeDef]],
+        "Analyses": NotRequired[List[AssetBundleImportJobAnalysisOverridePermissionsOutputTypeDef]],
+        "Dashboards": NotRequired[
+            List[AssetBundleImportJobDashboardOverridePermissionsOutputTypeDef]
+        ],
     },
 )
-TemplateVersionTypeDef = TypedDict(
-    "TemplateVersionTypeDef",
+AssetBundleImportJobOverridePermissionsTypeDef = TypedDict(
+    "AssetBundleImportJobOverridePermissionsTypeDef",
     {
-        "CreatedTime": NotRequired[datetime],
-        "Errors": NotRequired[List[TemplateErrorTypeDef]],
-        "VersionNumber": NotRequired[int],
-        "Status": NotRequired[ResourceStatusType],
-        "DataSetConfigurations": NotRequired[List[DataSetConfigurationTypeDef]],
-        "Description": NotRequired[str],
-        "SourceEntityArn": NotRequired[str],
-        "ThemeArn": NotRequired[str],
-        "Sheets": NotRequired[List[SheetTypeDef]],
+        "DataSources": NotRequired[
+            Sequence[AssetBundleImportJobDataSourceOverridePermissionsTypeDef]
+        ],
+        "DataSets": NotRequired[Sequence[AssetBundleImportJobDataSetOverridePermissionsTypeDef]],
+        "Themes": NotRequired[Sequence[AssetBundleImportJobThemeOverridePermissionsTypeDef]],
+        "Analyses": NotRequired[Sequence[AssetBundleImportJobAnalysisOverridePermissionsTypeDef]],
+        "Dashboards": NotRequired[
+            Sequence[AssetBundleImportJobDashboardOverridePermissionsTypeDef]
+        ],
     },
 )
+AssetBundleImportJobOverrideTagsUnionTypeDef = Union[
+    AssetBundleImportJobOverrideTagsTypeDef, AssetBundleImportJobOverrideTagsOutputTypeDef
+]
 DestinationParameterValueConfigurationTypeDef = TypedDict(
     "DestinationParameterValueConfigurationTypeDef",
     {
         "CustomValuesConfiguration": NotRequired[CustomValuesConfigurationTypeDef],
         "SelectAllValueOptions": NotRequired[Literal["ALL_VALUES"]],
         "SourceParameterName": NotRequired[str],
         "SourceField": NotRequired[str],
@@ -8326,27 +9807,15 @@
     {
         "StringDatasetParameter": NotRequired[StringDatasetParameterTypeDef],
         "DecimalDatasetParameter": NotRequired[DecimalDatasetParameterTypeDef],
         "IntegerDatasetParameter": NotRequired[IntegerDatasetParameterTypeDef],
         "DateTimeDatasetParameter": NotRequired[DateTimeDatasetParameterTypeDef],
     },
 )
-TransformOperationTypeDef = TypedDict(
-    "TransformOperationTypeDef",
-    {
-        "ProjectOperation": NotRequired[ProjectOperationTypeDef],
-        "FilterOperation": NotRequired[FilterOperationTypeDef],
-        "CreateColumnsOperation": NotRequired[CreateColumnsOperationTypeDef],
-        "RenameColumnOperation": NotRequired[RenameColumnOperationTypeDef],
-        "CastColumnTypeOperation": NotRequired[CastColumnTypeOperationTypeDef],
-        "TagColumnOperation": NotRequired[TagColumnOperationTypeDef],
-        "UntagColumnOperation": NotRequired[UntagColumnOperationTypeDef],
-        "OverrideDatasetParameterOperation": NotRequired[OverrideDatasetParameterOperationTypeDef],
-    },
-)
+ParametersUnionTypeDef = Union[ParametersTypeDef, ParametersOutputTypeDef]
 DateTimeHierarchyTypeDef = TypedDict(
     "DateTimeHierarchyTypeDef",
     {
         "HierarchyId": str,
         "DrillDownFilters": NotRequired[Sequence[DrillDownFilterTypeDef]],
     },
 )
@@ -8362,46 +9831,134 @@
     "PredefinedHierarchyTypeDef",
     {
         "HierarchyId": str,
         "Columns": Sequence[ColumnIdentifierTypeDef],
         "DrillDownFilters": NotRequired[Sequence[DrillDownFilterTypeDef]],
     },
 )
-ListTopicRefreshSchedulesResponseTypeDef = TypedDict(
-    "ListTopicRefreshSchedulesResponseTypeDef",
-    {
-        "TopicId": str,
-        "TopicArn": str,
-        "RefreshSchedules": List[TopicRefreshScheduleSummaryTypeDef],
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 ForecastConfigurationTypeDef = TypedDict(
     "ForecastConfigurationTypeDef",
     {
         "ForecastProperties": NotRequired[TimeBasedForecastPropertiesTypeDef],
         "Scenario": NotRequired[ForecastScenarioTypeDef],
     },
 )
+AxisDataOptionsOutputTypeDef = TypedDict(
+    "AxisDataOptionsOutputTypeDef",
+    {
+        "NumericAxisOptions": NotRequired[NumericAxisOptionsOutputTypeDef],
+        "DateAxisOptions": NotRequired[DateAxisOptionsTypeDef],
+    },
+)
+AxisDataOptionsTypeDef = TypedDict(
+    "AxisDataOptionsTypeDef",
+    {
+        "NumericAxisOptions": NotRequired[NumericAxisOptionsTypeDef],
+        "DateAxisOptions": NotRequired[DateAxisOptionsTypeDef],
+    },
+)
+TransformOperationOutputTypeDef = TypedDict(
+    "TransformOperationOutputTypeDef",
+    {
+        "ProjectOperation": NotRequired[ProjectOperationOutputTypeDef],
+        "FilterOperation": NotRequired[FilterOperationTypeDef],
+        "CreateColumnsOperation": NotRequired[CreateColumnsOperationOutputTypeDef],
+        "RenameColumnOperation": NotRequired[RenameColumnOperationTypeDef],
+        "CastColumnTypeOperation": NotRequired[CastColumnTypeOperationTypeDef],
+        "TagColumnOperation": NotRequired[TagColumnOperationOutputTypeDef],
+        "UntagColumnOperation": NotRequired[UntagColumnOperationOutputTypeDef],
+        "OverrideDatasetParameterOperation": NotRequired[
+            OverrideDatasetParameterOperationOutputTypeDef
+        ],
+    },
+)
+TransformOperationTypeDef = TypedDict(
+    "TransformOperationTypeDef",
+    {
+        "ProjectOperation": NotRequired[ProjectOperationTypeDef],
+        "FilterOperation": NotRequired[FilterOperationTypeDef],
+        "CreateColumnsOperation": NotRequired[CreateColumnsOperationTypeDef],
+        "RenameColumnOperation": NotRequired[RenameColumnOperationTypeDef],
+        "CastColumnTypeOperation": NotRequired[CastColumnTypeOperationTypeDef],
+        "TagColumnOperation": NotRequired[TagColumnOperationTypeDef],
+        "UntagColumnOperation": NotRequired[UntagColumnOperationTypeDef],
+        "OverrideDatasetParameterOperation": NotRequired[OverrideDatasetParameterOperationTypeDef],
+    },
+)
+TemplateVersionTypeDef = TypedDict(
+    "TemplateVersionTypeDef",
+    {
+        "CreatedTime": NotRequired[datetime],
+        "Errors": NotRequired[List[TemplateErrorTypeDef]],
+        "VersionNumber": NotRequired[int],
+        "Status": NotRequired[ResourceStatusType],
+        "DataSetConfigurations": NotRequired[List[DataSetConfigurationOutputTypeDef]],
+        "Description": NotRequired[str],
+        "SourceEntityArn": NotRequired[str],
+        "ThemeArn": NotRequired[str],
+        "Sheets": NotRequired[List[SheetTypeDef]],
+    },
+)
+SetParameterValueConfigurationOutputTypeDef = TypedDict(
+    "SetParameterValueConfigurationOutputTypeDef",
+    {
+        "DestinationParameterName": str,
+        "Value": DestinationParameterValueConfigurationOutputTypeDef,
+    },
+)
+VisualPaletteOutputTypeDef = TypedDict(
+    "VisualPaletteOutputTypeDef",
+    {
+        "ChartColor": NotRequired[str],
+        "ColorMap": NotRequired[List[DataPathColorTypeDef]],
+    },
+)
 VisualPaletteTypeDef = TypedDict(
     "VisualPaletteTypeDef",
     {
         "ChartColor": NotRequired[str],
         "ColorMap": NotRequired[Sequence[DataPathColorTypeDef]],
     },
 )
+PivotTableFieldCollapseStateOptionOutputTypeDef = TypedDict(
+    "PivotTableFieldCollapseStateOptionOutputTypeDef",
+    {
+        "Target": PivotTableFieldCollapseStateTargetOutputTypeDef,
+        "State": NotRequired[PivotTableFieldCollapseStateType],
+    },
+)
 PivotTableFieldCollapseStateOptionTypeDef = TypedDict(
     "PivotTableFieldCollapseStateOptionTypeDef",
     {
         "Target": PivotTableFieldCollapseStateTargetTypeDef,
         "State": NotRequired[PivotTableFieldCollapseStateType],
     },
 )
+TopicCalculatedFieldOutputTypeDef = TypedDict(
+    "TopicCalculatedFieldOutputTypeDef",
+    {
+        "CalculatedFieldName": str,
+        "Expression": str,
+        "CalculatedFieldDescription": NotRequired[str],
+        "CalculatedFieldSynonyms": NotRequired[List[str]],
+        "IsIncludedInTopic": NotRequired[bool],
+        "DisableIndexing": NotRequired[bool],
+        "ColumnDataRole": NotRequired[ColumnDataRoleType],
+        "TimeGranularity": NotRequired[TopicTimeGranularityType],
+        "DefaultFormatting": NotRequired[DefaultFormattingTypeDef],
+        "Aggregation": NotRequired[DefaultAggregationType],
+        "ComparativeOrder": NotRequired[ComparativeOrderOutputTypeDef],
+        "SemanticType": NotRequired[SemanticTypeOutputTypeDef],
+        "AllowedAggregations": NotRequired[List[AuthorSpecifiedAggregationType]],
+        "NotAllowedAggregations": NotRequired[List[AuthorSpecifiedAggregationType]],
+        "NeverAggregateInFilter": NotRequired[bool],
+        "CellValueSynonyms": NotRequired[List[CellValueSynonymOutputTypeDef]],
+        "NonAdditive": NotRequired[bool],
+    },
+)
 TopicCalculatedFieldTypeDef = TypedDict(
     "TopicCalculatedFieldTypeDef",
     {
         "CalculatedFieldName": str,
         "Expression": str,
         "CalculatedFieldDescription": NotRequired[str],
         "CalculatedFieldSynonyms": NotRequired[Sequence[str]],
@@ -8416,14 +9973,36 @@
         "AllowedAggregations": NotRequired[Sequence[AuthorSpecifiedAggregationType]],
         "NotAllowedAggregations": NotRequired[Sequence[AuthorSpecifiedAggregationType]],
         "NeverAggregateInFilter": NotRequired[bool],
         "CellValueSynonyms": NotRequired[Sequence[CellValueSynonymTypeDef]],
         "NonAdditive": NotRequired[bool],
     },
 )
+TopicColumnOutputTypeDef = TypedDict(
+    "TopicColumnOutputTypeDef",
+    {
+        "ColumnName": str,
+        "ColumnFriendlyName": NotRequired[str],
+        "ColumnDescription": NotRequired[str],
+        "ColumnSynonyms": NotRequired[List[str]],
+        "ColumnDataRole": NotRequired[ColumnDataRoleType],
+        "Aggregation": NotRequired[DefaultAggregationType],
+        "IsIncludedInTopic": NotRequired[bool],
+        "DisableIndexing": NotRequired[bool],
+        "ComparativeOrder": NotRequired[ComparativeOrderOutputTypeDef],
+        "SemanticType": NotRequired[SemanticTypeOutputTypeDef],
+        "TimeGranularity": NotRequired[TopicTimeGranularityType],
+        "AllowedAggregations": NotRequired[List[AuthorSpecifiedAggregationType]],
+        "NotAllowedAggregations": NotRequired[List[AuthorSpecifiedAggregationType]],
+        "DefaultFormatting": NotRequired[DefaultFormattingTypeDef],
+        "NeverAggregateInFilter": NotRequired[bool],
+        "CellValueSynonyms": NotRequired[List[CellValueSynonymOutputTypeDef]],
+        "NonAdditive": NotRequired[bool],
+    },
+)
 TopicColumnTypeDef = TypedDict(
     "TopicColumnTypeDef",
     {
         "ColumnName": str,
         "ColumnFriendlyName": NotRequired[str],
         "ColumnDescription": NotRequired[str],
         "ColumnSynonyms": NotRequired[Sequence[str]],
@@ -8438,14 +10017,22 @@
         "NotAllowedAggregations": NotRequired[Sequence[AuthorSpecifiedAggregationType]],
         "DefaultFormatting": NotRequired[DefaultFormattingTypeDef],
         "NeverAggregateInFilter": NotRequired[bool],
         "CellValueSynonyms": NotRequired[Sequence[CellValueSynonymTypeDef]],
         "NonAdditive": NotRequired[bool],
     },
 )
+ChartAxisLabelOptionsOutputTypeDef = TypedDict(
+    "ChartAxisLabelOptionsOutputTypeDef",
+    {
+        "Visibility": NotRequired[VisibilityType],
+        "SortIconVisibility": NotRequired[VisibilityType],
+        "AxisLabelOptions": NotRequired[List[AxisLabelOptionsTypeDef]],
+    },
+)
 ChartAxisLabelOptionsTypeDef = TypedDict(
     "ChartAxisLabelOptionsTypeDef",
     {
         "Visibility": NotRequired[VisibilityType],
         "SortIconVisibility": NotRequired[VisibilityType],
         "AxisLabelOptions": NotRequired[Sequence[AxisLabelOptionsTypeDef]],
     },
@@ -8540,14 +10127,22 @@
 TableFieldLinkContentConfigurationTypeDef = TypedDict(
     "TableFieldLinkContentConfigurationTypeDef",
     {
         "CustomTextContent": NotRequired[TableFieldCustomTextContentTypeDef],
         "CustomIconContent": NotRequired[TableFieldCustomIconContentTypeDef],
     },
 )
+GeospatialPointStyleOptionsOutputTypeDef = TypedDict(
+    "GeospatialPointStyleOptionsOutputTypeDef",
+    {
+        "SelectedPointStyle": NotRequired[GeospatialSelectedPointStyleType],
+        "ClusterMarkerConfiguration": NotRequired[ClusterMarkerConfigurationTypeDef],
+        "HeatmapConfiguration": NotRequired[GeospatialHeatmapConfigurationOutputTypeDef],
+    },
+)
 GeospatialPointStyleOptionsTypeDef = TypedDict(
     "GeospatialPointStyleOptionsTypeDef",
     {
         "SelectedPointStyle": NotRequired[GeospatialSelectedPointStyleType],
         "ClusterMarkerConfiguration": NotRequired[ClusterMarkerConfigurationTypeDef],
         "HeatmapConfiguration": NotRequired[GeospatialHeatmapConfigurationTypeDef],
     },
@@ -8561,28 +10156,41 @@
         "HorizontalTextAlignment": NotRequired[HorizontalTextAlignmentType],
         "VerticalTextAlignment": NotRequired[VerticalTextAlignmentType],
         "BackgroundColor": NotRequired[str],
         "Height": NotRequired[int],
         "Border": NotRequired[GlobalTableBorderOptionsTypeDef],
     },
 )
+ConditionalFormattingColorOutputTypeDef = TypedDict(
+    "ConditionalFormattingColorOutputTypeDef",
+    {
+        "Solid": NotRequired[ConditionalFormattingSolidColorTypeDef],
+        "Gradient": NotRequired[ConditionalFormattingGradientColorOutputTypeDef],
+    },
+)
 ConditionalFormattingColorTypeDef = TypedDict(
     "ConditionalFormattingColorTypeDef",
     {
         "Solid": NotRequired[ConditionalFormattingSolidColorTypeDef],
         "Gradient": NotRequired[ConditionalFormattingGradientColorTypeDef],
     },
 )
 DefaultInteractiveLayoutConfigurationTypeDef = TypedDict(
     "DefaultInteractiveLayoutConfigurationTypeDef",
     {
         "Grid": NotRequired[DefaultGridLayoutConfigurationTypeDef],
         "FreeForm": NotRequired[DefaultFreeFormLayoutConfigurationTypeDef],
     },
 )
+SheetControlLayoutConfigurationOutputTypeDef = TypedDict(
+    "SheetControlLayoutConfigurationOutputTypeDef",
+    {
+        "GridLayout": NotRequired[GridLayoutConfigurationOutputTypeDef],
+    },
+)
 SheetControlLayoutConfigurationTypeDef = TypedDict(
     "SheetControlLayoutConfigurationTypeDef",
     {
         "GridLayout": NotRequired[GridLayoutConfigurationTypeDef],
     },
 )
 DataSetRefreshPropertiesTypeDef = TypedDict(
@@ -8594,14 +10202,23 @@
 SeriesItemTypeDef = TypedDict(
     "SeriesItemTypeDef",
     {
         "FieldSeriesItem": NotRequired[FieldSeriesItemTypeDef],
         "DataFieldSeriesItem": NotRequired[DataFieldSeriesItemTypeDef],
     },
 )
+ThemeConfigurationOutputTypeDef = TypedDict(
+    "ThemeConfigurationOutputTypeDef",
+    {
+        "DataColorPalette": NotRequired[DataColorPaletteOutputTypeDef],
+        "UIColorPalette": NotRequired[UIColorPaletteTypeDef],
+        "Sheet": NotRequired[SheetStyleTypeDef],
+        "Typography": NotRequired[TypographyOutputTypeDef],
+    },
+)
 ThemeConfigurationTypeDef = TypedDict(
     "ThemeConfigurationTypeDef",
     {
         "DataColorPalette": NotRequired[DataColorPaletteTypeDef],
         "UIColorPalette": NotRequired[UIColorPaletteTypeDef],
         "Sheet": NotRequired[SheetStyleTypeDef],
         "Typography": NotRequired[TypographyTypeDef],
@@ -8658,14 +10275,30 @@
     "ReferenceLineDynamicDataConfigurationTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "Calculation": NumericalAggregationFunctionTypeDef,
         "MeasureAggregationFunction": NotRequired[AggregationFunctionTypeDef],
     },
 )
+TopicFilterOutputTypeDef = TypedDict(
+    "TopicFilterOutputTypeDef",
+    {
+        "FilterName": str,
+        "OperandFieldName": str,
+        "FilterDescription": NotRequired[str],
+        "FilterClass": NotRequired[FilterClassType],
+        "FilterSynonyms": NotRequired[List[str]],
+        "FilterType": NotRequired[NamedFilterTypeType],
+        "CategoryFilter": NotRequired[TopicCategoryFilterOutputTypeDef],
+        "NumericEqualityFilter": NotRequired[TopicNumericEqualityFilterTypeDef],
+        "NumericRangeFilter": NotRequired[TopicNumericRangeFilterTypeDef],
+        "DateRangeFilter": NotRequired[TopicDateRangeFilterTypeDef],
+        "RelativeDateFilter": NotRequired[TopicRelativeDateFilterTypeDef],
+    },
+)
 TopicFilterTypeDef = TypedDict(
     "TopicFilterTypeDef",
     {
         "FilterName": str,
         "OperandFieldName": str,
         "FilterDescription": NotRequired[str],
         "FilterClass": NotRequired[FilterClassType],
@@ -8674,26 +10307,37 @@
         "CategoryFilter": NotRequired[TopicCategoryFilterTypeDef],
         "NumericEqualityFilter": NotRequired[TopicNumericEqualityFilterTypeDef],
         "NumericRangeFilter": NotRequired[TopicNumericRangeFilterTypeDef],
         "DateRangeFilter": NotRequired[TopicDateRangeFilterTypeDef],
         "RelativeDateFilter": NotRequired[TopicRelativeDateFilterTypeDef],
     },
 )
-DataSourcePaginatorTypeDef = TypedDict(
-    "DataSourcePaginatorTypeDef",
+AssetBundleImportJobDataSourceOverrideParametersOutputTypeDef = TypedDict(
+    "AssetBundleImportJobDataSourceOverrideParametersOutputTypeDef",
+    {
+        "DataSourceId": str,
+        "Name": NotRequired[str],
+        "DataSourceParameters": NotRequired[DataSourceParametersOutputTypeDef],
+        "VpcConnectionProperties": NotRequired[VpcConnectionPropertiesTypeDef],
+        "SslProperties": NotRequired[SslPropertiesTypeDef],
+        "Credentials": NotRequired[AssetBundleImportJobDataSourceCredentialsTypeDef],
+    },
+)
+DataSourceTypeDef = TypedDict(
+    "DataSourceTypeDef",
     {
         "Arn": NotRequired[str],
         "DataSourceId": NotRequired[str],
         "Name": NotRequired[str],
         "Type": NotRequired[DataSourceTypeType],
         "Status": NotRequired[ResourceStatusType],
         "CreatedTime": NotRequired[datetime],
         "LastUpdatedTime": NotRequired[datetime],
-        "DataSourceParameters": NotRequired[DataSourceParametersPaginatorTypeDef],
-        "AlternateDataSourceParameters": NotRequired[List[DataSourceParametersPaginatorTypeDef]],
+        "DataSourceParameters": NotRequired[DataSourceParametersOutputTypeDef],
+        "AlternateDataSourceParameters": NotRequired[List[DataSourceParametersOutputTypeDef]],
         "VpcConnectionProperties": NotRequired[VpcConnectionPropertiesTypeDef],
         "SslProperties": NotRequired[SslPropertiesTypeDef],
         "ErrorInfo": NotRequired[DataSourceErrorInfoTypeDef],
         "SecretArn": NotRequired[str],
     },
 )
 AssetBundleImportJobDataSourceOverrideParametersTypeDef = TypedDict(
@@ -8711,59 +10355,45 @@
     "CredentialPairTypeDef",
     {
         "Username": str,
         "Password": str,
         "AlternateDataSourceParameters": NotRequired[Sequence[DataSourceParametersTypeDef]],
     },
 )
-DataSourceTypeDef = TypedDict(
-    "DataSourceTypeDef",
-    {
-        "Arn": NotRequired[str],
-        "DataSourceId": NotRequired[str],
-        "Name": NotRequired[str],
-        "Type": NotRequired[DataSourceTypeType],
-        "Status": NotRequired[ResourceStatusType],
-        "CreatedTime": NotRequired[datetime],
-        "LastUpdatedTime": NotRequired[datetime],
-        "DataSourceParameters": NotRequired[DataSourceParametersTypeDef],
-        "AlternateDataSourceParameters": NotRequired[List[DataSourceParametersTypeDef]],
-        "VpcConnectionProperties": NotRequired[VpcConnectionPropertiesTypeDef],
-        "SslProperties": NotRequired[SslPropertiesTypeDef],
-        "ErrorInfo": NotRequired[DataSourceErrorInfoTypeDef],
-        "SecretArn": NotRequired[str],
-    },
-)
-CreateRefreshScheduleRequestRequestTypeDef = TypedDict(
-    "CreateRefreshScheduleRequestRequestTypeDef",
-    {
-        "DataSetId": str,
-        "AwsAccountId": str,
-        "Schedule": RefreshScheduleTypeDef,
-    },
-)
+DataSourceParametersUnionTypeDef = Union[
+    DataSourceParametersTypeDef, DataSourceParametersExtraOutputTypeDef
+]
 DescribeRefreshScheduleResponseTypeDef = TypedDict(
     "DescribeRefreshScheduleResponseTypeDef",
     {
-        "RefreshSchedule": RefreshScheduleTypeDef,
+        "RefreshSchedule": RefreshScheduleOutputTypeDef,
         "Status": int,
         "RequestId": str,
         "Arn": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListRefreshSchedulesResponseTypeDef = TypedDict(
     "ListRefreshSchedulesResponseTypeDef",
     {
-        "RefreshSchedules": List[RefreshScheduleTypeDef],
+        "RefreshSchedules": List[RefreshScheduleOutputTypeDef],
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateRefreshScheduleRequestRequestTypeDef = TypedDict(
+    "CreateRefreshScheduleRequestRequestTypeDef",
+    {
+        "DataSetId": str,
+        "AwsAccountId": str,
+        "Schedule": RefreshScheduleTypeDef,
+    },
+)
+RefreshScheduleUnionTypeDef = Union[RefreshScheduleTypeDef, RefreshScheduleOutputTypeDef]
 UpdateRefreshScheduleRequestRequestTypeDef = TypedDict(
     "UpdateRefreshScheduleRequestRequestTypeDef",
     {
         "DataSetId": str,
         "AwsAccountId": str,
         "Schedule": RefreshScheduleTypeDef,
     },
@@ -8773,110 +10403,188 @@
     {
         "Dashboard": NotRequired[RegisteredUserDashboardEmbeddingConfigurationTypeDef],
         "QuickSightConsole": NotRequired[
             RegisteredUserQuickSightConsoleEmbeddingConfigurationTypeDef
         ],
         "QSearchBar": NotRequired[RegisteredUserQSearchBarEmbeddingConfigurationTypeDef],
         "DashboardVisual": NotRequired[RegisteredUserDashboardVisualEmbeddingConfigurationTypeDef],
+        "GenerativeQnA": NotRequired[RegisteredUserGenerativeQnAEmbeddingConfigurationTypeDef],
     },
 )
 SnapshotJobResultFileGroupTypeDef = TypedDict(
     "SnapshotJobResultFileGroupTypeDef",
     {
-        "Files": NotRequired[List[SnapshotFileTypeDef]],
+        "Files": NotRequired[List[SnapshotFileOutputTypeDef]],
         "S3Results": NotRequired[List[SnapshotJobS3ResultTypeDef]],
     },
 )
+PhysicalTableUnionTypeDef = Union[PhysicalTableTypeDef, PhysicalTableOutputTypeDef]
 DefaultSectionBasedLayoutConfigurationTypeDef = TypedDict(
     "DefaultSectionBasedLayoutConfigurationTypeDef",
     {
         "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
     },
 )
+FreeFormLayoutConfigurationOutputTypeDef = TypedDict(
+    "FreeFormLayoutConfigurationOutputTypeDef",
+    {
+        "Elements": List[FreeFormLayoutElementOutputTypeDef],
+        "CanvasSizeOptions": NotRequired[FreeFormLayoutCanvasSizeOptionsTypeDef],
+    },
+)
+FreeFormSectionLayoutConfigurationOutputTypeDef = TypedDict(
+    "FreeFormSectionLayoutConfigurationOutputTypeDef",
+    {
+        "Elements": List[FreeFormLayoutElementOutputTypeDef],
+    },
+)
 FreeFormLayoutConfigurationTypeDef = TypedDict(
     "FreeFormLayoutConfigurationTypeDef",
     {
         "Elements": Sequence[FreeFormLayoutElementTypeDef],
         "CanvasSizeOptions": NotRequired[FreeFormLayoutCanvasSizeOptionsTypeDef],
     },
 )
 FreeFormSectionLayoutConfigurationTypeDef = TypedDict(
     "FreeFormSectionLayoutConfigurationTypeDef",
     {
         "Elements": Sequence[FreeFormLayoutElementTypeDef],
     },
 )
+SnapshotConfigurationOutputTypeDef = TypedDict(
+    "SnapshotConfigurationOutputTypeDef",
+    {
+        "FileGroups": List[SnapshotFileGroupOutputTypeDef],
+        "DestinationConfiguration": NotRequired[SnapshotDestinationConfigurationOutputTypeDef],
+        "Parameters": NotRequired[ParametersOutputTypeDef],
+    },
+)
 SnapshotConfigurationTypeDef = TypedDict(
     "SnapshotConfigurationTypeDef",
     {
-        "FileGroups": List[SnapshotFileGroupTypeDef],
+        "FileGroups": Sequence[SnapshotFileGroupTypeDef],
         "DestinationConfiguration": NotRequired[SnapshotDestinationConfigurationTypeDef],
         "Parameters": NotRequired[ParametersTypeDef],
     },
 )
+ParameterDeclarationOutputTypeDef = TypedDict(
+    "ParameterDeclarationOutputTypeDef",
+    {
+        "StringParameterDeclaration": NotRequired[StringParameterDeclarationOutputTypeDef],
+        "DecimalParameterDeclaration": NotRequired[DecimalParameterDeclarationOutputTypeDef],
+        "IntegerParameterDeclaration": NotRequired[IntegerParameterDeclarationOutputTypeDef],
+        "DateTimeParameterDeclaration": NotRequired[DateTimeParameterDeclarationOutputTypeDef],
+    },
+)
 ParameterDeclarationTypeDef = TypedDict(
     "ParameterDeclarationTypeDef",
     {
         "StringParameterDeclaration": NotRequired[StringParameterDeclarationTypeDef],
         "DecimalParameterDeclaration": NotRequired[DecimalParameterDeclarationTypeDef],
         "IntegerParameterDeclaration": NotRequired[IntegerParameterDeclarationTypeDef],
         "DateTimeParameterDeclaration": NotRequired[DateTimeParameterDeclarationTypeDef],
     },
 )
+ColumnHierarchyOutputTypeDef = TypedDict(
+    "ColumnHierarchyOutputTypeDef",
+    {
+        "ExplicitHierarchy": NotRequired[ExplicitHierarchyOutputTypeDef],
+        "DateTimeHierarchy": NotRequired[DateTimeHierarchyOutputTypeDef],
+        "PredefinedHierarchy": NotRequired[PredefinedHierarchyOutputTypeDef],
+    },
+)
 DescribeDashboardResponseTypeDef = TypedDict(
     "DescribeDashboardResponseTypeDef",
     {
         "Dashboard": DashboardTypeDef,
         "Status": int,
         "RequestId": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
-TemplateTypeDef = TypedDict(
-    "TemplateTypeDef",
-    {
-        "Arn": NotRequired[str],
-        "Name": NotRequired[str],
-        "Version": NotRequired[TemplateVersionTypeDef],
-        "TemplateId": NotRequired[str],
-        "LastUpdatedTime": NotRequired[datetime],
-        "CreatedTime": NotRequired[datetime],
-    },
-)
+AssetBundleImportJobOverridePermissionsUnionTypeDef = Union[
+    AssetBundleImportJobOverridePermissionsTypeDef,
+    AssetBundleImportJobOverridePermissionsOutputTypeDef,
+]
 SetParameterValueConfigurationTypeDef = TypedDict(
     "SetParameterValueConfigurationTypeDef",
     {
         "DestinationParameterName": str,
         "Value": DestinationParameterValueConfigurationTypeDef,
     },
 )
+DatasetParameterUnionTypeDef = Union[DatasetParameterTypeDef, DatasetParameterOutputTypeDef]
+ColumnHierarchyTypeDef = TypedDict(
+    "ColumnHierarchyTypeDef",
+    {
+        "ExplicitHierarchy": NotRequired[ExplicitHierarchyTypeDef],
+        "DateTimeHierarchy": NotRequired[DateTimeHierarchyTypeDef],
+        "PredefinedHierarchy": NotRequired[PredefinedHierarchyTypeDef],
+    },
+)
+LogicalTableOutputTypeDef = TypedDict(
+    "LogicalTableOutputTypeDef",
+    {
+        "Alias": str,
+        "Source": LogicalTableSourceTypeDef,
+        "DataTransforms": NotRequired[List[TransformOperationOutputTypeDef]],
+    },
+)
 LogicalTableTypeDef = TypedDict(
     "LogicalTableTypeDef",
     {
         "Alias": str,
         "Source": LogicalTableSourceTypeDef,
         "DataTransforms": NotRequired[Sequence[TransformOperationTypeDef]],
     },
 )
-ColumnHierarchyTypeDef = TypedDict(
-    "ColumnHierarchyTypeDef",
+TemplateTypeDef = TypedDict(
+    "TemplateTypeDef",
     {
-        "ExplicitHierarchy": NotRequired[ExplicitHierarchyTypeDef],
-        "DateTimeHierarchy": NotRequired[DateTimeHierarchyTypeDef],
-        "PredefinedHierarchy": NotRequired[PredefinedHierarchyTypeDef],
+        "Arn": NotRequired[str],
+        "Name": NotRequired[str],
+        "Version": NotRequired[TemplateVersionTypeDef],
+        "TemplateId": NotRequired[str],
+        "LastUpdatedTime": NotRequired[datetime],
+        "CreatedTime": NotRequired[datetime],
+    },
+)
+CustomActionSetParametersOperationOutputTypeDef = TypedDict(
+    "CustomActionSetParametersOperationOutputTypeDef",
+    {
+        "ParameterValueConfigurations": List[SetParameterValueConfigurationOutputTypeDef],
+    },
+)
+PivotTableFieldOptionsOutputTypeDef = TypedDict(
+    "PivotTableFieldOptionsOutputTypeDef",
+    {
+        "SelectedFieldOptions": NotRequired[List[PivotTableFieldOptionTypeDef]],
+        "DataPathOptions": NotRequired[List[PivotTableDataPathOptionOutputTypeDef]],
+        "CollapseStateOptions": NotRequired[List[PivotTableFieldCollapseStateOptionOutputTypeDef]],
     },
 )
 PivotTableFieldOptionsTypeDef = TypedDict(
     "PivotTableFieldOptionsTypeDef",
     {
         "SelectedFieldOptions": NotRequired[Sequence[PivotTableFieldOptionTypeDef]],
         "DataPathOptions": NotRequired[Sequence[PivotTableDataPathOptionTypeDef]],
         "CollapseStateOptions": NotRequired[Sequence[PivotTableFieldCollapseStateOptionTypeDef]],
     },
 )
+AxisDisplayOptionsOutputTypeDef = TypedDict(
+    "AxisDisplayOptionsOutputTypeDef",
+    {
+        "TickLabelOptions": NotRequired[AxisTickLabelOptionsTypeDef],
+        "AxisLineVisibility": NotRequired[VisibilityType],
+        "GridLineVisibility": NotRequired[VisibilityType],
+        "DataOptions": NotRequired[AxisDataOptionsOutputTypeDef],
+        "ScrollbarOptions": NotRequired[ScrollBarOptionsTypeDef],
+        "AxisOffset": NotRequired[str],
+    },
+)
 AxisDisplayOptionsTypeDef = TypedDict(
     "AxisDisplayOptionsTypeDef",
     {
         "TickLabelOptions": NotRequired[AxisTickLabelOptionsTypeDef],
         "AxisLineVisibility": NotRequired[VisibilityType],
         "GridLineVisibility": NotRequired[VisibilityType],
         "DataOptions": NotRequired[AxisDataOptionsTypeDef],
@@ -8906,66 +10614,130 @@
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
         "DisplayOptions": NotRequired[DateTimePickerControlDisplayOptionsTypeDef],
     },
 )
+DefaultFilterDropDownControlOptionsOutputTypeDef = TypedDict(
+    "DefaultFilterDropDownControlOptionsOutputTypeDef",
+    {
+        "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[FilterSelectableValuesOutputTypeDef],
+    },
+)
 DefaultFilterDropDownControlOptionsTypeDef = TypedDict(
     "DefaultFilterDropDownControlOptionsTypeDef",
     {
         "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
         "Type": NotRequired[SheetControlListTypeType],
         "SelectableValues": NotRequired[FilterSelectableValuesTypeDef],
     },
 )
+FilterDropDownControlOutputTypeDef = TypedDict(
+    "FilterDropDownControlOutputTypeDef",
+    {
+        "FilterControlId": str,
+        "Title": str,
+        "SourceFilterId": str,
+        "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[FilterSelectableValuesOutputTypeDef],
+        "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationOutputTypeDef],
+    },
+)
 FilterDropDownControlTypeDef = TypedDict(
     "FilterDropDownControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
         "Type": NotRequired[SheetControlListTypeType],
         "SelectableValues": NotRequired[FilterSelectableValuesTypeDef],
         "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationTypeDef],
     },
 )
+ParameterDropDownControlOutputTypeDef = TypedDict(
+    "ParameterDropDownControlOutputTypeDef",
+    {
+        "ParameterControlId": str,
+        "Title": str,
+        "SourceParameterName": str,
+        "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[ParameterSelectableValuesOutputTypeDef],
+        "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationOutputTypeDef],
+    },
+)
 ParameterDropDownControlTypeDef = TypedDict(
     "ParameterDropDownControlTypeDef",
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
         "DisplayOptions": NotRequired[DropDownControlDisplayOptionsTypeDef],
         "Type": NotRequired[SheetControlListTypeType],
         "SelectableValues": NotRequired[ParameterSelectableValuesTypeDef],
         "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationTypeDef],
     },
 )
+DefaultFilterListControlOptionsOutputTypeDef = TypedDict(
+    "DefaultFilterListControlOptionsOutputTypeDef",
+    {
+        "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[FilterSelectableValuesOutputTypeDef],
+    },
+)
 DefaultFilterListControlOptionsTypeDef = TypedDict(
     "DefaultFilterListControlOptionsTypeDef",
     {
         "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
         "Type": NotRequired[SheetControlListTypeType],
         "SelectableValues": NotRequired[FilterSelectableValuesTypeDef],
     },
 )
+FilterListControlOutputTypeDef = TypedDict(
+    "FilterListControlOutputTypeDef",
+    {
+        "FilterControlId": str,
+        "Title": str,
+        "SourceFilterId": str,
+        "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[FilterSelectableValuesOutputTypeDef],
+        "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationOutputTypeDef],
+    },
+)
 FilterListControlTypeDef = TypedDict(
     "FilterListControlTypeDef",
     {
         "FilterControlId": str,
         "Title": str,
         "SourceFilterId": str,
         "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
         "Type": NotRequired[SheetControlListTypeType],
         "SelectableValues": NotRequired[FilterSelectableValuesTypeDef],
         "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationTypeDef],
     },
 )
+ParameterListControlOutputTypeDef = TypedDict(
+    "ParameterListControlOutputTypeDef",
+    {
+        "ParameterControlId": str,
+        "Title": str,
+        "SourceParameterName": str,
+        "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
+        "Type": NotRequired[SheetControlListTypeType],
+        "SelectableValues": NotRequired[ParameterSelectableValuesOutputTypeDef],
+        "CascadingControlConfiguration": NotRequired[CascadingControlConfigurationOutputTypeDef],
+    },
+)
 ParameterListControlTypeDef = TypedDict(
     "ParameterListControlTypeDef",
     {
         "ParameterControlId": str,
         "Title": str,
         "SourceParameterName": str,
         "DisplayOptions": NotRequired[ListControlDisplayOptionsTypeDef],
@@ -9088,14 +10860,32 @@
 TableFieldLinkConfigurationTypeDef = TypedDict(
     "TableFieldLinkConfigurationTypeDef",
     {
         "Target": URLTargetConfigurationType,
         "Content": TableFieldLinkContentConfigurationTypeDef,
     },
 )
+PivotTableOptionsOutputTypeDef = TypedDict(
+    "PivotTableOptionsOutputTypeDef",
+    {
+        "MetricPlacement": NotRequired[PivotTableMetricPlacementType],
+        "SingleMetricVisibility": NotRequired[VisibilityType],
+        "ColumnNamesVisibility": NotRequired[VisibilityType],
+        "ToggleButtonsVisibility": NotRequired[VisibilityType],
+        "ColumnHeaderStyle": NotRequired[TableCellStyleTypeDef],
+        "RowHeaderStyle": NotRequired[TableCellStyleTypeDef],
+        "CellStyle": NotRequired[TableCellStyleTypeDef],
+        "RowFieldNamesStyle": NotRequired[TableCellStyleTypeDef],
+        "RowAlternateColorOptions": NotRequired[RowAlternateColorOptionsOutputTypeDef],
+        "CollapsedRowDimensionsVisibility": NotRequired[VisibilityType],
+        "RowsLayout": NotRequired[PivotTableRowsLayoutType],
+        "RowsLabelOptions": NotRequired[PivotTableRowsLabelOptionsTypeDef],
+        "DefaultCellWidth": NotRequired[str],
+    },
+)
 PivotTableOptionsTypeDef = TypedDict(
     "PivotTableOptionsTypeDef",
     {
         "MetricPlacement": NotRequired[PivotTableMetricPlacementType],
         "SingleMetricVisibility": NotRequired[VisibilityType],
         "ColumnNamesVisibility": NotRequired[VisibilityType],
         "ToggleButtonsVisibility": NotRequired[VisibilityType],
@@ -9106,60 +10896,167 @@
         "RowAlternateColorOptions": NotRequired[RowAlternateColorOptionsTypeDef],
         "CollapsedRowDimensionsVisibility": NotRequired[VisibilityType],
         "RowsLayout": NotRequired[PivotTableRowsLayoutType],
         "RowsLabelOptions": NotRequired[PivotTableRowsLabelOptionsTypeDef],
         "DefaultCellWidth": NotRequired[str],
     },
 )
+PivotTotalOptionsOutputTypeDef = TypedDict(
+    "PivotTotalOptionsOutputTypeDef",
+    {
+        "TotalsVisibility": NotRequired[VisibilityType],
+        "Placement": NotRequired[TableTotalsPlacementType],
+        "ScrollStatus": NotRequired[TableTotalsScrollStatusType],
+        "CustomLabel": NotRequired[str],
+        "TotalCellStyle": NotRequired[TableCellStyleTypeDef],
+        "ValueCellStyle": NotRequired[TableCellStyleTypeDef],
+        "MetricHeaderCellStyle": NotRequired[TableCellStyleTypeDef],
+        "TotalAggregationOptions": NotRequired[List[TotalAggregationOptionTypeDef]],
+    },
+)
 PivotTotalOptionsTypeDef = TypedDict(
     "PivotTotalOptionsTypeDef",
     {
         "TotalsVisibility": NotRequired[VisibilityType],
         "Placement": NotRequired[TableTotalsPlacementType],
         "ScrollStatus": NotRequired[TableTotalsScrollStatusType],
         "CustomLabel": NotRequired[str],
         "TotalCellStyle": NotRequired[TableCellStyleTypeDef],
         "ValueCellStyle": NotRequired[TableCellStyleTypeDef],
         "MetricHeaderCellStyle": NotRequired[TableCellStyleTypeDef],
         "TotalAggregationOptions": NotRequired[Sequence[TotalAggregationOptionTypeDef]],
     },
 )
+SubtotalOptionsOutputTypeDef = TypedDict(
+    "SubtotalOptionsOutputTypeDef",
+    {
+        "TotalsVisibility": NotRequired[VisibilityType],
+        "CustomLabel": NotRequired[str],
+        "FieldLevel": NotRequired[PivotTableSubtotalLevelType],
+        "FieldLevelOptions": NotRequired[List[PivotTableFieldSubtotalOptionsTypeDef]],
+        "TotalCellStyle": NotRequired[TableCellStyleTypeDef],
+        "ValueCellStyle": NotRequired[TableCellStyleTypeDef],
+        "MetricHeaderCellStyle": NotRequired[TableCellStyleTypeDef],
+        "StyleTargets": NotRequired[List[TableStyleTargetTypeDef]],
+    },
+)
 SubtotalOptionsTypeDef = TypedDict(
     "SubtotalOptionsTypeDef",
     {
         "TotalsVisibility": NotRequired[VisibilityType],
         "CustomLabel": NotRequired[str],
         "FieldLevel": NotRequired[PivotTableSubtotalLevelType],
         "FieldLevelOptions": NotRequired[Sequence[PivotTableFieldSubtotalOptionsTypeDef]],
         "TotalCellStyle": NotRequired[TableCellStyleTypeDef],
         "ValueCellStyle": NotRequired[TableCellStyleTypeDef],
         "MetricHeaderCellStyle": NotRequired[TableCellStyleTypeDef],
         "StyleTargets": NotRequired[Sequence[TableStyleTargetTypeDef]],
     },
 )
+TableOptionsOutputTypeDef = TypedDict(
+    "TableOptionsOutputTypeDef",
+    {
+        "Orientation": NotRequired[TableOrientationType],
+        "HeaderStyle": NotRequired[TableCellStyleTypeDef],
+        "CellStyle": NotRequired[TableCellStyleTypeDef],
+        "RowAlternateColorOptions": NotRequired[RowAlternateColorOptionsOutputTypeDef],
+    },
+)
 TableOptionsTypeDef = TypedDict(
     "TableOptionsTypeDef",
     {
         "Orientation": NotRequired[TableOrientationType],
         "HeaderStyle": NotRequired[TableCellStyleTypeDef],
         "CellStyle": NotRequired[TableCellStyleTypeDef],
         "RowAlternateColorOptions": NotRequired[RowAlternateColorOptionsTypeDef],
     },
 )
+TotalOptionsOutputTypeDef = TypedDict(
+    "TotalOptionsOutputTypeDef",
+    {
+        "TotalsVisibility": NotRequired[VisibilityType],
+        "Placement": NotRequired[TableTotalsPlacementType],
+        "ScrollStatus": NotRequired[TableTotalsScrollStatusType],
+        "CustomLabel": NotRequired[str],
+        "TotalCellStyle": NotRequired[TableCellStyleTypeDef],
+        "TotalAggregationOptions": NotRequired[List[TotalAggregationOptionTypeDef]],
+    },
+)
 TotalOptionsTypeDef = TypedDict(
     "TotalOptionsTypeDef",
     {
         "TotalsVisibility": NotRequired[VisibilityType],
         "Placement": NotRequired[TableTotalsPlacementType],
         "ScrollStatus": NotRequired[TableTotalsScrollStatusType],
         "CustomLabel": NotRequired[str],
         "TotalCellStyle": NotRequired[TableCellStyleTypeDef],
         "TotalAggregationOptions": NotRequired[Sequence[TotalAggregationOptionTypeDef]],
     },
 )
+GaugeChartArcConditionalFormattingOutputTypeDef = TypedDict(
+    "GaugeChartArcConditionalFormattingOutputTypeDef",
+    {
+        "ForegroundColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+    },
+)
+GaugeChartPrimaryValueConditionalFormattingOutputTypeDef = TypedDict(
+    "GaugeChartPrimaryValueConditionalFormattingOutputTypeDef",
+    {
+        "TextColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+        "Icon": NotRequired[ConditionalFormattingIconTypeDef],
+    },
+)
+KPIActualValueConditionalFormattingOutputTypeDef = TypedDict(
+    "KPIActualValueConditionalFormattingOutputTypeDef",
+    {
+        "TextColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+        "Icon": NotRequired[ConditionalFormattingIconTypeDef],
+    },
+)
+KPIComparisonValueConditionalFormattingOutputTypeDef = TypedDict(
+    "KPIComparisonValueConditionalFormattingOutputTypeDef",
+    {
+        "TextColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+        "Icon": NotRequired[ConditionalFormattingIconTypeDef],
+    },
+)
+KPIPrimaryValueConditionalFormattingOutputTypeDef = TypedDict(
+    "KPIPrimaryValueConditionalFormattingOutputTypeDef",
+    {
+        "TextColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+        "Icon": NotRequired[ConditionalFormattingIconTypeDef],
+    },
+)
+KPIProgressBarConditionalFormattingOutputTypeDef = TypedDict(
+    "KPIProgressBarConditionalFormattingOutputTypeDef",
+    {
+        "ForegroundColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+    },
+)
+ShapeConditionalFormatOutputTypeDef = TypedDict(
+    "ShapeConditionalFormatOutputTypeDef",
+    {
+        "BackgroundColor": ConditionalFormattingColorOutputTypeDef,
+    },
+)
+TableRowConditionalFormattingOutputTypeDef = TypedDict(
+    "TableRowConditionalFormattingOutputTypeDef",
+    {
+        "BackgroundColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+        "TextColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+    },
+)
+TextConditionalFormatOutputTypeDef = TypedDict(
+    "TextConditionalFormatOutputTypeDef",
+    {
+        "BackgroundColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+        "TextColor": NotRequired[ConditionalFormattingColorOutputTypeDef],
+        "Icon": NotRequired[ConditionalFormattingIconTypeDef],
+    },
+)
 GaugeChartArcConditionalFormattingTypeDef = TypedDict(
     "GaugeChartArcConditionalFormattingTypeDef",
     {
         "ForegroundColor": NotRequired[ConditionalFormattingColorTypeDef],
     },
 )
 GaugeChartPrimaryValueConditionalFormattingTypeDef = TypedDict(
@@ -9213,14 +11110,20 @@
     "TextConditionalFormatTypeDef",
     {
         "BackgroundColor": NotRequired[ConditionalFormattingColorTypeDef],
         "TextColor": NotRequired[ConditionalFormattingColorTypeDef],
         "Icon": NotRequired[ConditionalFormattingIconTypeDef],
     },
 )
+SheetControlLayoutOutputTypeDef = TypedDict(
+    "SheetControlLayoutOutputTypeDef",
+    {
+        "Configuration": SheetControlLayoutConfigurationOutputTypeDef,
+    },
+)
 SheetControlLayoutTypeDef = TypedDict(
     "SheetControlLayoutTypeDef",
     {
         "Configuration": SheetControlLayoutConfigurationTypeDef,
     },
 )
 DescribeDataSetRefreshPropertiesResponseTypeDef = TypedDict(
@@ -9236,40 +11139,41 @@
     "PutDataSetRefreshPropertiesRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DataSetId": str,
         "DataSetRefreshProperties": DataSetRefreshPropertiesTypeDef,
     },
 )
-CreateThemeRequestRequestTypeDef = TypedDict(
-    "CreateThemeRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "ThemeId": str,
-        "Name": str,
-        "BaseThemeId": str,
-        "Configuration": ThemeConfigurationTypeDef,
-        "VersionDescription": NotRequired[str],
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-    },
-)
 ThemeVersionTypeDef = TypedDict(
     "ThemeVersionTypeDef",
     {
         "VersionNumber": NotRequired[int],
         "Arn": NotRequired[str],
         "Description": NotRequired[str],
         "BaseThemeId": NotRequired[str],
         "CreatedTime": NotRequired[datetime],
-        "Configuration": NotRequired[ThemeConfigurationTypeDef],
+        "Configuration": NotRequired[ThemeConfigurationOutputTypeDef],
         "Errors": NotRequired[List[ThemeErrorTypeDef]],
         "Status": NotRequired[ResourceStatusType],
     },
 )
+CreateThemeRequestRequestTypeDef = TypedDict(
+    "CreateThemeRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "ThemeId": str,
+        "Name": str,
+        "BaseThemeId": str,
+        "Configuration": ThemeConfigurationTypeDef,
+        "VersionDescription": NotRequired[str],
+        "Permissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+ThemeConfigurationUnionTypeDef = Union[ThemeConfigurationTypeDef, ThemeConfigurationOutputTypeDef]
 UpdateThemeRequestRequestTypeDef = TypedDict(
     "UpdateThemeRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "ThemeId": str,
         "BaseThemeId": str,
         "Name": NotRequired[str],
@@ -9315,14 +11219,22 @@
 FieldSortOptionsTypeDef = TypedDict(
     "FieldSortOptionsTypeDef",
     {
         "FieldSort": NotRequired[FieldSortTypeDef],
         "ColumnSort": NotRequired[ColumnSortTypeDef],
     },
 )
+PivotTableSortByOutputTypeDef = TypedDict(
+    "PivotTableSortByOutputTypeDef",
+    {
+        "Field": NotRequired[FieldSortTypeDef],
+        "Column": NotRequired[ColumnSortTypeDef],
+        "DataPath": NotRequired[DataPathSortOutputTypeDef],
+    },
+)
 PivotTableSortByTypeDef = TypedDict(
     "PivotTableSortByTypeDef",
     {
         "Field": NotRequired[FieldSortTypeDef],
         "Column": NotRequired[ColumnSortTypeDef],
         "DataPath": NotRequired[DataPathSortTypeDef],
     },
@@ -9339,81 +11251,107 @@
     {
         "StaticConfiguration": NotRequired[ReferenceLineStaticDataConfigurationTypeDef],
         "DynamicConfiguration": NotRequired[ReferenceLineDynamicDataConfigurationTypeDef],
         "AxisBinding": NotRequired[AxisBindingType],
         "SeriesType": NotRequired[ReferenceLineSeriesTypeType],
     },
 )
+DatasetMetadataOutputTypeDef = TypedDict(
+    "DatasetMetadataOutputTypeDef",
+    {
+        "DatasetArn": str,
+        "DatasetName": NotRequired[str],
+        "DatasetDescription": NotRequired[str],
+        "DataAggregation": NotRequired[DataAggregationTypeDef],
+        "Filters": NotRequired[List[TopicFilterOutputTypeDef]],
+        "Columns": NotRequired[List[TopicColumnOutputTypeDef]],
+        "CalculatedFields": NotRequired[List[TopicCalculatedFieldOutputTypeDef]],
+        "NamedEntities": NotRequired[List[TopicNamedEntityOutputTypeDef]],
+    },
+)
 DatasetMetadataTypeDef = TypedDict(
     "DatasetMetadataTypeDef",
     {
         "DatasetArn": str,
         "DatasetName": NotRequired[str],
         "DatasetDescription": NotRequired[str],
         "DataAggregation": NotRequired[DataAggregationTypeDef],
         "Filters": NotRequired[Sequence[TopicFilterTypeDef]],
         "Columns": NotRequired[Sequence[TopicColumnTypeDef]],
         "CalculatedFields": NotRequired[Sequence[TopicCalculatedFieldTypeDef]],
         "NamedEntities": NotRequired[Sequence[TopicNamedEntityTypeDef]],
     },
 )
-ListDataSourcesResponsePaginatorTypeDef = TypedDict(
-    "ListDataSourcesResponsePaginatorTypeDef",
-    {
-        "DataSources": List[DataSourcePaginatorTypeDef],
-        "NextToken": str,
-        "RequestId": str,
-        "Status": int,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
-AssetBundleImportJobOverrideParametersTypeDef = TypedDict(
-    "AssetBundleImportJobOverrideParametersTypeDef",
+AssetBundleImportJobOverrideParametersOutputTypeDef = TypedDict(
+    "AssetBundleImportJobOverrideParametersOutputTypeDef",
     {
         "ResourceIdOverrideConfiguration": NotRequired[
             AssetBundleImportJobResourceIdOverrideConfigurationTypeDef
         ],
         "VPCConnections": NotRequired[
-            List[AssetBundleImportJobVPCConnectionOverrideParametersTypeDef]
+            List[AssetBundleImportJobVPCConnectionOverrideParametersOutputTypeDef]
         ],
         "RefreshSchedules": NotRequired[
-            List[AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef]
+            List[AssetBundleImportJobRefreshScheduleOverrideParametersOutputTypeDef]
+        ],
+        "DataSources": NotRequired[
+            List[AssetBundleImportJobDataSourceOverrideParametersOutputTypeDef]
         ],
-        "DataSources": NotRequired[List[AssetBundleImportJobDataSourceOverrideParametersTypeDef]],
         "DataSets": NotRequired[List[AssetBundleImportJobDataSetOverrideParametersTypeDef]],
         "Themes": NotRequired[List[AssetBundleImportJobThemeOverrideParametersTypeDef]],
         "Analyses": NotRequired[List[AssetBundleImportJobAnalysisOverrideParametersTypeDef]],
         "Dashboards": NotRequired[List[AssetBundleImportJobDashboardOverrideParametersTypeDef]],
     },
 )
-DataSourceCredentialsTypeDef = TypedDict(
-    "DataSourceCredentialsTypeDef",
-    {
-        "CredentialPair": NotRequired[CredentialPairTypeDef],
-        "CopySourceArn": NotRequired[str],
-        "SecretArn": NotRequired[str],
-    },
-)
 DescribeDataSourceResponseTypeDef = TypedDict(
     "DescribeDataSourceResponseTypeDef",
     {
         "DataSource": DataSourceTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListDataSourcesResponseTypeDef = TypedDict(
     "ListDataSourcesResponseTypeDef",
     {
         "DataSources": List[DataSourceTypeDef],
-        "NextToken": str,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
+        "NextToken": NotRequired[str],
+    },
+)
+AssetBundleImportJobOverrideParametersTypeDef = TypedDict(
+    "AssetBundleImportJobOverrideParametersTypeDef",
+    {
+        "ResourceIdOverrideConfiguration": NotRequired[
+            AssetBundleImportJobResourceIdOverrideConfigurationTypeDef
+        ],
+        "VPCConnections": NotRequired[
+            Sequence[AssetBundleImportJobVPCConnectionOverrideParametersTypeDef]
+        ],
+        "RefreshSchedules": NotRequired[
+            Sequence[AssetBundleImportJobRefreshScheduleOverrideParametersTypeDef]
+        ],
+        "DataSources": NotRequired[
+            Sequence[AssetBundleImportJobDataSourceOverrideParametersTypeDef]
+        ],
+        "DataSets": NotRequired[Sequence[AssetBundleImportJobDataSetOverrideParametersTypeDef]],
+        "Themes": NotRequired[Sequence[AssetBundleImportJobThemeOverrideParametersTypeDef]],
+        "Analyses": NotRequired[Sequence[AssetBundleImportJobAnalysisOverrideParametersTypeDef]],
+        "Dashboards": NotRequired[Sequence[AssetBundleImportJobDashboardOverrideParametersTypeDef]],
+    },
+)
+DataSourceCredentialsTypeDef = TypedDict(
+    "DataSourceCredentialsTypeDef",
+    {
+        "CredentialPair": NotRequired[CredentialPairTypeDef],
+        "CopySourceArn": NotRequired[str],
+        "SecretArn": NotRequired[str],
     },
 )
 GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef = TypedDict(
     "GenerateEmbedUrlForRegisteredUserRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "UserArn": str,
@@ -9430,161 +11368,180 @@
 )
 DefaultPaginatedLayoutConfigurationTypeDef = TypedDict(
     "DefaultPaginatedLayoutConfigurationTypeDef",
     {
         "SectionBased": NotRequired[DefaultSectionBasedLayoutConfigurationTypeDef],
     },
 )
+SectionLayoutConfigurationOutputTypeDef = TypedDict(
+    "SectionLayoutConfigurationOutputTypeDef",
+    {
+        "FreeFormLayout": FreeFormSectionLayoutConfigurationOutputTypeDef,
+    },
+)
 SectionLayoutConfigurationTypeDef = TypedDict(
     "SectionLayoutConfigurationTypeDef",
     {
         "FreeFormLayout": FreeFormSectionLayoutConfigurationTypeDef,
     },
 )
 DescribeDashboardSnapshotJobResponseTypeDef = TypedDict(
     "DescribeDashboardSnapshotJobResponseTypeDef",
     {
         "AwsAccountId": str,
         "DashboardId": str,
         "SnapshotJobId": str,
         "UserConfiguration": SnapshotUserConfigurationRedactedTypeDef,
-        "SnapshotConfiguration": SnapshotConfigurationTypeDef,
+        "SnapshotConfiguration": SnapshotConfigurationOutputTypeDef,
         "Arn": str,
         "JobStatus": SnapshotJobStatusType,
         "CreatedTime": datetime,
         "LastUpdatedTime": datetime,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+SnapshotConfigurationUnionTypeDef = Union[
+    SnapshotConfigurationTypeDef, SnapshotConfigurationOutputTypeDef
+]
 StartDashboardSnapshotJobRequestRequestTypeDef = TypedDict(
     "StartDashboardSnapshotJobRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DashboardId": str,
         "SnapshotJobId": str,
         "UserConfiguration": SnapshotUserConfigurationTypeDef,
         "SnapshotConfiguration": SnapshotConfigurationTypeDef,
     },
 )
-DescribeTemplateResponseTypeDef = TypedDict(
-    "DescribeTemplateResponseTypeDef",
-    {
-        "Template": TemplateTypeDef,
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 CustomActionSetParametersOperationTypeDef = TypedDict(
     "CustomActionSetParametersOperationTypeDef",
     {
         "ParameterValueConfigurations": Sequence[SetParameterValueConfigurationTypeDef],
     },
 )
-CreateDataSetRequestRequestTypeDef = TypedDict(
-    "CreateDataSetRequestRequestTypeDef",
-    {
-        "AwsAccountId": str,
-        "DataSetId": str,
-        "Name": str,
-        "PhysicalTableMap": Mapping[str, PhysicalTableTypeDef],
-        "ImportMode": DataSetImportModeType,
-        "LogicalTableMap": NotRequired[Mapping[str, LogicalTableTypeDef]],
-        "ColumnGroups": NotRequired[Sequence[ColumnGroupTypeDef]],
-        "FieldFolders": NotRequired[Mapping[str, FieldFolderTypeDef]],
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
-        "RowLevelPermissionDataSet": NotRequired[RowLevelPermissionDataSetTypeDef],
-        "RowLevelPermissionTagConfiguration": NotRequired[
-            RowLevelPermissionTagConfigurationTypeDef
-        ],
-        "ColumnLevelPermissionRules": NotRequired[Sequence[ColumnLevelPermissionRuleTypeDef]],
-        "Tags": NotRequired[Sequence[TagTypeDef]],
-        "DataSetUsageConfiguration": NotRequired[DataSetUsageConfigurationTypeDef],
-        "DatasetParameters": NotRequired[Sequence[DatasetParameterTypeDef]],
-        "FolderArns": NotRequired[Sequence[str]],
-    },
-)
 DataSetTypeDef = TypedDict(
     "DataSetTypeDef",
     {
         "Arn": NotRequired[str],
         "DataSetId": NotRequired[str],
         "Name": NotRequired[str],
         "CreatedTime": NotRequired[datetime],
         "LastUpdatedTime": NotRequired[datetime],
-        "PhysicalTableMap": NotRequired[Dict[str, PhysicalTableTypeDef]],
-        "LogicalTableMap": NotRequired[Dict[str, LogicalTableTypeDef]],
+        "PhysicalTableMap": NotRequired[Dict[str, PhysicalTableOutputTypeDef]],
+        "LogicalTableMap": NotRequired[Dict[str, LogicalTableOutputTypeDef]],
         "OutputColumns": NotRequired[List[OutputColumnTypeDef]],
         "ImportMode": NotRequired[DataSetImportModeType],
         "ConsumedSpiceCapacityInBytes": NotRequired[int],
-        "ColumnGroups": NotRequired[List[ColumnGroupTypeDef]],
-        "FieldFolders": NotRequired[Dict[str, FieldFolderTypeDef]],
+        "ColumnGroups": NotRequired[List[ColumnGroupOutputTypeDef]],
+        "FieldFolders": NotRequired[Dict[str, FieldFolderOutputTypeDef]],
         "RowLevelPermissionDataSet": NotRequired[RowLevelPermissionDataSetTypeDef],
         "RowLevelPermissionTagConfiguration": NotRequired[
-            RowLevelPermissionTagConfigurationTypeDef
+            RowLevelPermissionTagConfigurationOutputTypeDef
         ],
-        "ColumnLevelPermissionRules": NotRequired[List[ColumnLevelPermissionRuleTypeDef]],
+        "ColumnLevelPermissionRules": NotRequired[List[ColumnLevelPermissionRuleOutputTypeDef]],
         "DataSetUsageConfiguration": NotRequired[DataSetUsageConfigurationTypeDef],
-        "DatasetParameters": NotRequired[List[DatasetParameterTypeDef]],
+        "DatasetParameters": NotRequired[List[DatasetParameterOutputTypeDef]],
     },
 )
-UpdateDataSetRequestRequestTypeDef = TypedDict(
-    "UpdateDataSetRequestRequestTypeDef",
+LogicalTableUnionTypeDef = Union[LogicalTableTypeDef, LogicalTableOutputTypeDef]
+DescribeTemplateResponseTypeDef = TypedDict(
+    "DescribeTemplateResponseTypeDef",
     {
-        "AwsAccountId": str,
-        "DataSetId": str,
-        "Name": str,
-        "PhysicalTableMap": Mapping[str, PhysicalTableTypeDef],
-        "ImportMode": DataSetImportModeType,
-        "LogicalTableMap": NotRequired[Mapping[str, LogicalTableTypeDef]],
-        "ColumnGroups": NotRequired[Sequence[ColumnGroupTypeDef]],
-        "FieldFolders": NotRequired[Mapping[str, FieldFolderTypeDef]],
-        "RowLevelPermissionDataSet": NotRequired[RowLevelPermissionDataSetTypeDef],
-        "RowLevelPermissionTagConfiguration": NotRequired[
-            RowLevelPermissionTagConfigurationTypeDef
-        ],
-        "ColumnLevelPermissionRules": NotRequired[Sequence[ColumnLevelPermissionRuleTypeDef]],
-        "DataSetUsageConfiguration": NotRequired[DataSetUsageConfigurationTypeDef],
-        "DatasetParameters": NotRequired[Sequence[DatasetParameterTypeDef]],
+        "Template": TemplateTypeDef,
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+VisualCustomActionOperationOutputTypeDef = TypedDict(
+    "VisualCustomActionOperationOutputTypeDef",
+    {
+        "FilterOperation": NotRequired[CustomActionFilterOperationOutputTypeDef],
+        "NavigationOperation": NotRequired[CustomActionNavigationOperationTypeDef],
+        "URLOperation": NotRequired[CustomActionURLOperationTypeDef],
+        "SetParametersOperation": NotRequired[CustomActionSetParametersOperationOutputTypeDef],
+    },
+)
+LineSeriesAxisDisplayOptionsOutputTypeDef = TypedDict(
+    "LineSeriesAxisDisplayOptionsOutputTypeDef",
+    {
+        "AxisOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "MissingDataConfigurations": NotRequired[List[MissingDataConfigurationTypeDef]],
     },
 )
 LineSeriesAxisDisplayOptionsTypeDef = TypedDict(
     "LineSeriesAxisDisplayOptionsTypeDef",
     {
         "AxisOptions": NotRequired[AxisDisplayOptionsTypeDef],
         "MissingDataConfigurations": NotRequired[Sequence[MissingDataConfigurationTypeDef]],
     },
 )
+DefaultFilterControlOptionsOutputTypeDef = TypedDict(
+    "DefaultFilterControlOptionsOutputTypeDef",
+    {
+        "DefaultDateTimePickerOptions": NotRequired[DefaultDateTimePickerControlOptionsTypeDef],
+        "DefaultListOptions": NotRequired[DefaultFilterListControlOptionsOutputTypeDef],
+        "DefaultDropdownOptions": NotRequired[DefaultFilterDropDownControlOptionsOutputTypeDef],
+        "DefaultTextFieldOptions": NotRequired[DefaultTextFieldControlOptionsTypeDef],
+        "DefaultTextAreaOptions": NotRequired[DefaultTextAreaControlOptionsTypeDef],
+        "DefaultSliderOptions": NotRequired[DefaultSliderControlOptionsTypeDef],
+        "DefaultRelativeDateTimeOptions": NotRequired[DefaultRelativeDateTimeControlOptionsTypeDef],
+    },
+)
 DefaultFilterControlOptionsTypeDef = TypedDict(
     "DefaultFilterControlOptionsTypeDef",
     {
         "DefaultDateTimePickerOptions": NotRequired[DefaultDateTimePickerControlOptionsTypeDef],
         "DefaultListOptions": NotRequired[DefaultFilterListControlOptionsTypeDef],
         "DefaultDropdownOptions": NotRequired[DefaultFilterDropDownControlOptionsTypeDef],
         "DefaultTextFieldOptions": NotRequired[DefaultTextFieldControlOptionsTypeDef],
         "DefaultTextAreaOptions": NotRequired[DefaultTextAreaControlOptionsTypeDef],
         "DefaultSliderOptions": NotRequired[DefaultSliderControlOptionsTypeDef],
         "DefaultRelativeDateTimeOptions": NotRequired[DefaultRelativeDateTimeControlOptionsTypeDef],
     },
 )
+FilterControlOutputTypeDef = TypedDict(
+    "FilterControlOutputTypeDef",
+    {
+        "DateTimePicker": NotRequired[FilterDateTimePickerControlTypeDef],
+        "List": NotRequired[FilterListControlOutputTypeDef],
+        "Dropdown": NotRequired[FilterDropDownControlOutputTypeDef],
+        "TextField": NotRequired[FilterTextFieldControlTypeDef],
+        "TextArea": NotRequired[FilterTextAreaControlTypeDef],
+        "Slider": NotRequired[FilterSliderControlTypeDef],
+        "RelativeDateTime": NotRequired[FilterRelativeDateTimeControlTypeDef],
+        "CrossSheet": NotRequired[FilterCrossSheetControlOutputTypeDef],
+    },
+)
 FilterControlTypeDef = TypedDict(
     "FilterControlTypeDef",
     {
         "DateTimePicker": NotRequired[FilterDateTimePickerControlTypeDef],
         "List": NotRequired[FilterListControlTypeDef],
         "Dropdown": NotRequired[FilterDropDownControlTypeDef],
         "TextField": NotRequired[FilterTextFieldControlTypeDef],
         "TextArea": NotRequired[FilterTextAreaControlTypeDef],
         "Slider": NotRequired[FilterSliderControlTypeDef],
         "RelativeDateTime": NotRequired[FilterRelativeDateTimeControlTypeDef],
         "CrossSheet": NotRequired[FilterCrossSheetControlTypeDef],
     },
 )
+ParameterControlOutputTypeDef = TypedDict(
+    "ParameterControlOutputTypeDef",
+    {
+        "DateTimePicker": NotRequired[ParameterDateTimePickerControlTypeDef],
+        "List": NotRequired[ParameterListControlOutputTypeDef],
+        "Dropdown": NotRequired[ParameterDropDownControlOutputTypeDef],
+        "TextField": NotRequired[ParameterTextFieldControlTypeDef],
+        "TextArea": NotRequired[ParameterTextAreaControlTypeDef],
+        "Slider": NotRequired[ParameterSliderControlTypeDef],
+    },
+)
 ParameterControlTypeDef = TypedDict(
     "ParameterControlTypeDef",
     {
         "DateTimePicker": NotRequired[ParameterDateTimePickerControlTypeDef],
         "List": NotRequired[ParameterListControlTypeDef],
         "Dropdown": NotRequired[ParameterDropDownControlTypeDef],
         "TextField": NotRequired[ParameterTextFieldControlTypeDef],
@@ -9595,23 +11552,71 @@
 TableFieldURLConfigurationTypeDef = TypedDict(
     "TableFieldURLConfigurationTypeDef",
     {
         "LinkConfiguration": NotRequired[TableFieldLinkConfigurationTypeDef],
         "ImageConfiguration": NotRequired[TableFieldImageConfigurationTypeDef],
     },
 )
+PivotTableTotalOptionsOutputTypeDef = TypedDict(
+    "PivotTableTotalOptionsOutputTypeDef",
+    {
+        "RowSubtotalOptions": NotRequired[SubtotalOptionsOutputTypeDef],
+        "ColumnSubtotalOptions": NotRequired[SubtotalOptionsOutputTypeDef],
+        "RowTotalOptions": NotRequired[PivotTotalOptionsOutputTypeDef],
+        "ColumnTotalOptions": NotRequired[PivotTotalOptionsOutputTypeDef],
+    },
+)
 PivotTableTotalOptionsTypeDef = TypedDict(
     "PivotTableTotalOptionsTypeDef",
     {
         "RowSubtotalOptions": NotRequired[SubtotalOptionsTypeDef],
         "ColumnSubtotalOptions": NotRequired[SubtotalOptionsTypeDef],
         "RowTotalOptions": NotRequired[PivotTotalOptionsTypeDef],
         "ColumnTotalOptions": NotRequired[PivotTotalOptionsTypeDef],
     },
 )
+GaugeChartConditionalFormattingOptionOutputTypeDef = TypedDict(
+    "GaugeChartConditionalFormattingOptionOutputTypeDef",
+    {
+        "PrimaryValue": NotRequired[GaugeChartPrimaryValueConditionalFormattingOutputTypeDef],
+        "Arc": NotRequired[GaugeChartArcConditionalFormattingOutputTypeDef],
+    },
+)
+KPIConditionalFormattingOptionOutputTypeDef = TypedDict(
+    "KPIConditionalFormattingOptionOutputTypeDef",
+    {
+        "PrimaryValue": NotRequired[KPIPrimaryValueConditionalFormattingOutputTypeDef],
+        "ProgressBar": NotRequired[KPIProgressBarConditionalFormattingOutputTypeDef],
+        "ActualValue": NotRequired[KPIActualValueConditionalFormattingOutputTypeDef],
+        "ComparisonValue": NotRequired[KPIComparisonValueConditionalFormattingOutputTypeDef],
+    },
+)
+FilledMapShapeConditionalFormattingOutputTypeDef = TypedDict(
+    "FilledMapShapeConditionalFormattingOutputTypeDef",
+    {
+        "FieldId": str,
+        "Format": NotRequired[ShapeConditionalFormatOutputTypeDef],
+    },
+)
+PivotTableCellConditionalFormattingOutputTypeDef = TypedDict(
+    "PivotTableCellConditionalFormattingOutputTypeDef",
+    {
+        "FieldId": str,
+        "TextFormat": NotRequired[TextConditionalFormatOutputTypeDef],
+        "Scope": NotRequired[PivotTableConditionalFormattingScopeTypeDef],
+        "Scopes": NotRequired[List[PivotTableConditionalFormattingScopeTypeDef]],
+    },
+)
+TableCellConditionalFormattingOutputTypeDef = TypedDict(
+    "TableCellConditionalFormattingOutputTypeDef",
+    {
+        "FieldId": str,
+        "TextFormat": NotRequired[TextConditionalFormatOutputTypeDef],
+    },
+)
 GaugeChartConditionalFormattingOptionTypeDef = TypedDict(
     "GaugeChartConditionalFormattingOptionTypeDef",
     {
         "PrimaryValue": NotRequired[GaugeChartPrimaryValueConditionalFormattingTypeDef],
         "Arc": NotRequired[GaugeChartArcConditionalFormattingTypeDef],
     },
 )
@@ -9753,148 +11758,291 @@
     "FormatConfigurationTypeDef",
     {
         "StringFormatConfiguration": NotRequired[StringFormatConfigurationTypeDef],
         "NumberFormatConfiguration": NotRequired[NumberFormatConfigurationTypeDef],
         "DateTimeFormatConfiguration": NotRequired[DateTimeFormatConfigurationTypeDef],
     },
 )
+BarChartSortConfigurationOutputTypeDef = TypedDict(
+    "BarChartSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+        "ColorSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "ColorItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+        "SmallMultiplesSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "SmallMultiplesLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 BarChartSortConfigurationTypeDef = TypedDict(
     "BarChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "ColorSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "ColorItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "SmallMultiplesSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "SmallMultiplesLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+BoxPlotSortConfigurationOutputTypeDef = TypedDict(
+    "BoxPlotSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "PaginationConfiguration": NotRequired[PaginationConfigurationTypeDef],
+    },
+)
 BoxPlotSortConfigurationTypeDef = TypedDict(
     "BoxPlotSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "PaginationConfiguration": NotRequired[PaginationConfigurationTypeDef],
     },
 )
+ComboChartSortConfigurationOutputTypeDef = TypedDict(
+    "ComboChartSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+        "ColorSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "ColorItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 ComboChartSortConfigurationTypeDef = TypedDict(
     "ComboChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "ColorSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "ColorItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+FilledMapSortConfigurationOutputTypeDef = TypedDict(
+    "FilledMapSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+    },
+)
 FilledMapSortConfigurationTypeDef = TypedDict(
     "FilledMapSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
     },
 )
+FunnelChartSortConfigurationOutputTypeDef = TypedDict(
+    "FunnelChartSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 FunnelChartSortConfigurationTypeDef = TypedDict(
     "FunnelChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+HeatMapSortConfigurationOutputTypeDef = TypedDict(
+    "HeatMapSortConfigurationOutputTypeDef",
+    {
+        "HeatMapRowSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "HeatMapColumnSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "HeatMapRowItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+        "HeatMapColumnItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 HeatMapSortConfigurationTypeDef = TypedDict(
     "HeatMapSortConfigurationTypeDef",
     {
         "HeatMapRowSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "HeatMapColumnSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "HeatMapRowItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
         "HeatMapColumnItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+KPISortConfigurationOutputTypeDef = TypedDict(
+    "KPISortConfigurationOutputTypeDef",
+    {
+        "TrendGroupSort": NotRequired[List[FieldSortOptionsTypeDef]],
+    },
+)
 KPISortConfigurationTypeDef = TypedDict(
     "KPISortConfigurationTypeDef",
     {
         "TrendGroupSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
     },
 )
+LineChartSortConfigurationOutputTypeDef = TypedDict(
+    "LineChartSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "CategoryItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+        "ColorItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+        "SmallMultiplesSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "SmallMultiplesLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 LineChartSortConfigurationTypeDef = TypedDict(
     "LineChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "CategoryItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
         "ColorItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
         "SmallMultiplesSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "SmallMultiplesLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+PieChartSortConfigurationOutputTypeDef = TypedDict(
+    "PieChartSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+        "SmallMultiplesSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "SmallMultiplesLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 PieChartSortConfigurationTypeDef = TypedDict(
     "PieChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "SmallMultiplesSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "SmallMultiplesLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+RadarChartSortConfigurationOutputTypeDef = TypedDict(
+    "RadarChartSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+        "ColorSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "ColorItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 RadarChartSortConfigurationTypeDef = TypedDict(
     "RadarChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "ColorSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "ColorItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+SankeyDiagramSortConfigurationOutputTypeDef = TypedDict(
+    "SankeyDiagramSortConfigurationOutputTypeDef",
+    {
+        "WeightSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "SourceItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+        "DestinationItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 SankeyDiagramSortConfigurationTypeDef = TypedDict(
     "SankeyDiagramSortConfigurationTypeDef",
     {
         "WeightSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "SourceItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "DestinationItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+TableSortConfigurationOutputTypeDef = TypedDict(
+    "TableSortConfigurationOutputTypeDef",
+    {
+        "RowSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "PaginationConfiguration": NotRequired[PaginationConfigurationTypeDef],
+    },
+)
 TableSortConfigurationTypeDef = TypedDict(
     "TableSortConfigurationTypeDef",
     {
         "RowSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "PaginationConfiguration": NotRequired[PaginationConfigurationTypeDef],
     },
 )
+TreeMapSortConfigurationOutputTypeDef = TypedDict(
+    "TreeMapSortConfigurationOutputTypeDef",
+    {
+        "TreeMapSort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "TreeMapGroupItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 TreeMapSortConfigurationTypeDef = TypedDict(
     "TreeMapSortConfigurationTypeDef",
     {
         "TreeMapSort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "TreeMapGroupItemsLimitConfiguration": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+WaterfallChartSortConfigurationOutputTypeDef = TypedDict(
+    "WaterfallChartSortConfigurationOutputTypeDef",
+    {
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+        "BreakdownItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+    },
+)
 WaterfallChartSortConfigurationTypeDef = TypedDict(
     "WaterfallChartSortConfigurationTypeDef",
     {
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
         "BreakdownItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
     },
 )
+WordCloudSortConfigurationOutputTypeDef = TypedDict(
+    "WordCloudSortConfigurationOutputTypeDef",
+    {
+        "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
+        "CategorySort": NotRequired[List[FieldSortOptionsTypeDef]],
+    },
+)
 WordCloudSortConfigurationTypeDef = TypedDict(
     "WordCloudSortConfigurationTypeDef",
     {
         "CategoryItemsLimit": NotRequired[ItemsLimitConfigurationTypeDef],
         "CategorySort": NotRequired[Sequence[FieldSortOptionsTypeDef]],
     },
 )
+PivotFieldSortOptionsOutputTypeDef = TypedDict(
+    "PivotFieldSortOptionsOutputTypeDef",
+    {
+        "FieldId": str,
+        "SortBy": PivotTableSortByOutputTypeDef,
+    },
+)
 PivotFieldSortOptionsTypeDef = TypedDict(
     "PivotFieldSortOptionsTypeDef",
     {
         "FieldId": str,
         "SortBy": PivotTableSortByTypeDef,
     },
 )
+FieldBasedTooltipOutputTypeDef = TypedDict(
+    "FieldBasedTooltipOutputTypeDef",
+    {
+        "AggregationVisibility": NotRequired[VisibilityType],
+        "TooltipTitleType": NotRequired[TooltipTitleTypeType],
+        "TooltipFields": NotRequired[List[TooltipItemTypeDef]],
+    },
+)
 FieldBasedTooltipTypeDef = TypedDict(
     "FieldBasedTooltipTypeDef",
     {
         "AggregationVisibility": NotRequired[VisibilityType],
         "TooltipTitleType": NotRequired[TooltipTitleTypeType],
         "TooltipFields": NotRequired[Sequence[TooltipItemTypeDef]],
     },
 )
+TopicDetailsOutputTypeDef = TypedDict(
+    "TopicDetailsOutputTypeDef",
+    {
+        "Name": NotRequired[str],
+        "Description": NotRequired[str],
+        "UserExperienceVersion": NotRequired[TopicUserExperienceVersionType],
+        "DataSets": NotRequired[List[DatasetMetadataOutputTypeDef]],
+    },
+)
 TopicDetailsTypeDef = TypedDict(
     "TopicDetailsTypeDef",
     {
         "Name": NotRequired[str],
         "Description": NotRequired[str],
         "UserExperienceVersion": NotRequired[TopicUserExperienceVersionType],
         "DataSets": NotRequired[Sequence[DatasetMetadataTypeDef]],
@@ -9907,25 +12055,29 @@
         "Errors": List[AssetBundleImportJobErrorTypeDef],
         "RollbackErrors": List[AssetBundleImportJobErrorTypeDef],
         "Arn": str,
         "CreatedTime": datetime,
         "AssetBundleImportJobId": str,
         "AwsAccountId": str,
         "AssetBundleImportSource": AssetBundleImportSourceDescriptionTypeDef,
-        "OverrideParameters": AssetBundleImportJobOverrideParametersTypeDef,
+        "OverrideParameters": AssetBundleImportJobOverrideParametersOutputTypeDef,
         "FailureAction": AssetBundleImportFailureActionType,
         "RequestId": str,
         "Status": int,
-        "OverridePermissions": AssetBundleImportJobOverridePermissionsTypeDef,
-        "OverrideTags": AssetBundleImportJobOverrideTagsTypeDef,
+        "OverridePermissions": AssetBundleImportJobOverridePermissionsOutputTypeDef,
+        "OverrideTags": AssetBundleImportJobOverrideTagsOutputTypeDef,
         "OverrideValidationStrategy": AssetBundleImportJobOverrideValidationStrategyTypeDef,
         "Warnings": List[AssetBundleImportJobWarningTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+AssetBundleImportJobOverrideParametersUnionTypeDef = Union[
+    AssetBundleImportJobOverrideParametersTypeDef,
+    AssetBundleImportJobOverrideParametersOutputTypeDef,
+]
 StartAssetBundleImportJobRequestRequestTypeDef = TypedDict(
     "StartAssetBundleImportJobRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AssetBundleImportJobId": str,
         "AssetBundleImportSource": AssetBundleImportSourceTypeDef,
         "OverrideParameters": NotRequired[AssetBundleImportJobOverrideParametersTypeDef],
@@ -9942,15 +12094,15 @@
     {
         "AwsAccountId": str,
         "DataSourceId": str,
         "Name": str,
         "Type": DataSourceTypeType,
         "DataSourceParameters": NotRequired[DataSourceParametersTypeDef],
         "Credentials": NotRequired[DataSourceCredentialsTypeDef],
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
+        "Permissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
         "VpcConnectionProperties": NotRequired[VpcConnectionPropertiesTypeDef],
         "SslProperties": NotRequired[SslPropertiesTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "FolderArns": NotRequired[Sequence[str]],
     },
 )
 UpdateDataSourceRequestRequestTypeDef = TypedDict(
@@ -9975,14 +12127,28 @@
     "DefaultNewSheetConfigurationTypeDef",
     {
         "InteractiveLayoutConfiguration": NotRequired[DefaultInteractiveLayoutConfigurationTypeDef],
         "PaginatedLayoutConfiguration": NotRequired[DefaultPaginatedLayoutConfigurationTypeDef],
         "SheetContentType": NotRequired[SheetContentTypeType],
     },
 )
+BodySectionContentOutputTypeDef = TypedDict(
+    "BodySectionContentOutputTypeDef",
+    {
+        "Layout": NotRequired[SectionLayoutConfigurationOutputTypeDef],
+    },
+)
+HeaderFooterSectionConfigurationOutputTypeDef = TypedDict(
+    "HeaderFooterSectionConfigurationOutputTypeDef",
+    {
+        "SectionId": str,
+        "Layout": SectionLayoutConfigurationOutputTypeDef,
+        "Style": NotRequired[SectionStyleTypeDef],
+    },
+)
 BodySectionContentTypeDef = TypedDict(
     "BodySectionContentTypeDef",
     {
         "Layout": NotRequired[SectionLayoutConfigurationTypeDef],
     },
 )
 HeaderFooterSectionConfigurationTypeDef = TypedDict(
@@ -10007,14 +12173,74 @@
     {
         "DataSet": DataSetTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateDataSetRequestRequestTypeDef = TypedDict(
+    "CreateDataSetRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DataSetId": str,
+        "Name": str,
+        "PhysicalTableMap": Mapping[str, PhysicalTableUnionTypeDef],
+        "ImportMode": DataSetImportModeType,
+        "LogicalTableMap": NotRequired[Mapping[str, LogicalTableUnionTypeDef]],
+        "ColumnGroups": NotRequired[Sequence[ColumnGroupUnionTypeDef]],
+        "FieldFolders": NotRequired[Mapping[str, FieldFolderUnionTypeDef]],
+        "Permissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
+        "RowLevelPermissionDataSet": NotRequired[RowLevelPermissionDataSetTypeDef],
+        "RowLevelPermissionTagConfiguration": NotRequired[
+            RowLevelPermissionTagConfigurationTypeDef
+        ],
+        "ColumnLevelPermissionRules": NotRequired[Sequence[ColumnLevelPermissionRuleUnionTypeDef]],
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "DataSetUsageConfiguration": NotRequired[DataSetUsageConfigurationTypeDef],
+        "DatasetParameters": NotRequired[Sequence[DatasetParameterUnionTypeDef]],
+        "FolderArns": NotRequired[Sequence[str]],
+    },
+)
+UpdateDataSetRequestRequestTypeDef = TypedDict(
+    "UpdateDataSetRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "DataSetId": str,
+        "Name": str,
+        "PhysicalTableMap": Mapping[str, PhysicalTableUnionTypeDef],
+        "ImportMode": DataSetImportModeType,
+        "LogicalTableMap": NotRequired[Mapping[str, LogicalTableUnionTypeDef]],
+        "ColumnGroups": NotRequired[Sequence[ColumnGroupUnionTypeDef]],
+        "FieldFolders": NotRequired[Mapping[str, FieldFolderUnionTypeDef]],
+        "RowLevelPermissionDataSet": NotRequired[RowLevelPermissionDataSetTypeDef],
+        "RowLevelPermissionTagConfiguration": NotRequired[
+            RowLevelPermissionTagConfigurationTypeDef
+        ],
+        "ColumnLevelPermissionRules": NotRequired[Sequence[ColumnLevelPermissionRuleUnionTypeDef]],
+        "DataSetUsageConfiguration": NotRequired[DataSetUsageConfigurationTypeDef],
+        "DatasetParameters": NotRequired[Sequence[DatasetParameterUnionTypeDef]],
+    },
+)
+VisualCustomActionOutputTypeDef = TypedDict(
+    "VisualCustomActionOutputTypeDef",
+    {
+        "CustomActionId": str,
+        "Name": str,
+        "Trigger": VisualCustomActionTriggerType,
+        "ActionOperations": List[VisualCustomActionOperationOutputTypeDef],
+        "Status": NotRequired[WidgetStatusType],
+    },
+)
+DefaultFilterControlConfigurationOutputTypeDef = TypedDict(
+    "DefaultFilterControlConfigurationOutputTypeDef",
+    {
+        "Title": str,
+        "ControlOptions": DefaultFilterControlOptionsOutputTypeDef,
+    },
+)
 DefaultFilterControlConfigurationTypeDef = TypedDict(
     "DefaultFilterControlConfigurationTypeDef",
     {
         "Title": str,
         "ControlOptions": DefaultFilterControlOptionsTypeDef,
     },
 )
@@ -10024,14 +12250,49 @@
         "FieldId": str,
         "Width": NotRequired[str],
         "CustomLabel": NotRequired[str],
         "Visibility": NotRequired[VisibilityType],
         "URLStyling": NotRequired[TableFieldURLConfigurationTypeDef],
     },
 )
+GaugeChartConditionalFormattingOutputTypeDef = TypedDict(
+    "GaugeChartConditionalFormattingOutputTypeDef",
+    {
+        "ConditionalFormattingOptions": NotRequired[
+            List[GaugeChartConditionalFormattingOptionOutputTypeDef]
+        ],
+    },
+)
+KPIConditionalFormattingOutputTypeDef = TypedDict(
+    "KPIConditionalFormattingOutputTypeDef",
+    {
+        "ConditionalFormattingOptions": NotRequired[
+            List[KPIConditionalFormattingOptionOutputTypeDef]
+        ],
+    },
+)
+FilledMapConditionalFormattingOptionOutputTypeDef = TypedDict(
+    "FilledMapConditionalFormattingOptionOutputTypeDef",
+    {
+        "Shape": FilledMapShapeConditionalFormattingOutputTypeDef,
+    },
+)
+PivotTableConditionalFormattingOptionOutputTypeDef = TypedDict(
+    "PivotTableConditionalFormattingOptionOutputTypeDef",
+    {
+        "Cell": NotRequired[PivotTableCellConditionalFormattingOutputTypeDef],
+    },
+)
+TableConditionalFormattingOptionOutputTypeDef = TypedDict(
+    "TableConditionalFormattingOptionOutputTypeDef",
+    {
+        "Cell": NotRequired[TableCellConditionalFormattingOutputTypeDef],
+        "Row": NotRequired[TableRowConditionalFormattingOutputTypeDef],
+    },
+)
 GaugeChartConditionalFormattingTypeDef = TypedDict(
     "GaugeChartConditionalFormattingTypeDef",
     {
         "ConditionalFormattingOptions": NotRequired[
             Sequence[GaugeChartConditionalFormattingOptionTypeDef]
         ],
     },
@@ -10094,14 +12355,23 @@
     {
         "NumericalMeasureField": NotRequired[NumericalMeasureFieldTypeDef],
         "CategoricalMeasureField": NotRequired[CategoricalMeasureFieldTypeDef],
         "DateMeasureField": NotRequired[DateMeasureFieldTypeDef],
         "CalculatedMeasureField": NotRequired[CalculatedMeasureFieldTypeDef],
     },
 )
+ColumnConfigurationOutputTypeDef = TypedDict(
+    "ColumnConfigurationOutputTypeDef",
+    {
+        "Column": ColumnIdentifierTypeDef,
+        "FormatConfiguration": NotRequired[FormatConfigurationTypeDef],
+        "Role": NotRequired[ColumnRoleType],
+        "ColorsConfiguration": NotRequired[ColorsConfigurationOutputTypeDef],
+    },
+)
 ColumnConfigurationTypeDef = TypedDict(
     "ColumnConfigurationTypeDef",
     {
         "Column": ColumnIdentifierTypeDef,
         "FormatConfiguration": NotRequired[FormatConfigurationTypeDef],
         "Role": NotRequired[ColumnRoleType],
         "ColorsConfiguration": NotRequired[ColorsConfigurationTypeDef],
@@ -10111,48 +12381,63 @@
     "UnaggregatedFieldTypeDef",
     {
         "FieldId": str,
         "Column": ColumnIdentifierTypeDef,
         "FormatConfiguration": NotRequired[FormatConfigurationTypeDef],
     },
 )
+PivotTableSortConfigurationOutputTypeDef = TypedDict(
+    "PivotTableSortConfigurationOutputTypeDef",
+    {
+        "FieldSortOptions": NotRequired[List[PivotFieldSortOptionsOutputTypeDef]],
+    },
+)
 PivotTableSortConfigurationTypeDef = TypedDict(
     "PivotTableSortConfigurationTypeDef",
     {
         "FieldSortOptions": NotRequired[Sequence[PivotFieldSortOptionsTypeDef]],
     },
 )
-TooltipOptionsTypeDef = TypedDict(
-    "TooltipOptionsTypeDef",
+TooltipOptionsOutputTypeDef = TypedDict(
+    "TooltipOptionsOutputTypeDef",
     {
         "TooltipVisibility": NotRequired[VisibilityType],
         "SelectedTooltipType": NotRequired[SelectedTooltipTypeType],
-        "FieldBasedTooltip": NotRequired[FieldBasedTooltipTypeDef],
+        "FieldBasedTooltip": NotRequired[FieldBasedTooltipOutputTypeDef],
     },
 )
-CreateTopicRequestRequestTypeDef = TypedDict(
-    "CreateTopicRequestRequestTypeDef",
+TooltipOptionsTypeDef = TypedDict(
+    "TooltipOptionsTypeDef",
     {
-        "AwsAccountId": str,
-        "TopicId": str,
-        "Topic": TopicDetailsTypeDef,
-        "Tags": NotRequired[Sequence[TagTypeDef]],
+        "TooltipVisibility": NotRequired[VisibilityType],
+        "SelectedTooltipType": NotRequired[SelectedTooltipTypeType],
+        "FieldBasedTooltip": NotRequired[FieldBasedTooltipTypeDef],
     },
 )
 DescribeTopicResponseTypeDef = TypedDict(
     "DescribeTopicResponseTypeDef",
     {
         "Arn": str,
         "TopicId": str,
-        "Topic": TopicDetailsTypeDef,
+        "Topic": TopicDetailsOutputTypeDef,
         "RequestId": str,
         "Status": int,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
+CreateTopicRequestRequestTypeDef = TypedDict(
+    "CreateTopicRequestRequestTypeDef",
+    {
+        "AwsAccountId": str,
+        "TopicId": str,
+        "Topic": TopicDetailsTypeDef,
+        "Tags": NotRequired[Sequence[TagTypeDef]],
+    },
+)
+TopicDetailsUnionTypeDef = Union[TopicDetailsTypeDef, TopicDetailsOutputTypeDef]
 UpdateTopicRequestRequestTypeDef = TypedDict(
     "UpdateTopicRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TopicId": str,
         "Topic": TopicDetailsTypeDef,
     },
@@ -10173,14 +12458,23 @@
 )
 AnalysisDefaultsTypeDef = TypedDict(
     "AnalysisDefaultsTypeDef",
     {
         "DefaultNewSheetConfiguration": DefaultNewSheetConfigurationTypeDef,
     },
 )
+BodySectionConfigurationOutputTypeDef = TypedDict(
+    "BodySectionConfigurationOutputTypeDef",
+    {
+        "SectionId": str,
+        "Content": BodySectionContentOutputTypeDef,
+        "Style": NotRequired[SectionStyleTypeDef],
+        "PageBreakConfiguration": NotRequired[SectionPageBreakConfigurationTypeDef],
+    },
+)
 BodySectionConfigurationTypeDef = TypedDict(
     "BodySectionConfigurationTypeDef",
     {
         "SectionId": str,
         "Content": BodySectionContentTypeDef,
         "Style": NotRequired[SectionStyleTypeDef],
         "PageBreakConfiguration": NotRequired[SectionPageBreakConfigurationTypeDef],
@@ -10192,14 +12486,140 @@
         "CustomActionId": str,
         "Name": str,
         "Trigger": VisualCustomActionTriggerType,
         "ActionOperations": Sequence[VisualCustomActionOperationTypeDef],
         "Status": NotRequired[WidgetStatusType],
     },
 )
+CustomContentVisualOutputTypeDef = TypedDict(
+    "CustomContentVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "DataSetIdentifier": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[CustomContentConfigurationTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
+EmptyVisualOutputTypeDef = TypedDict(
+    "EmptyVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "DataSetIdentifier": str,
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
+CategoryFilterOutputTypeDef = TypedDict(
+    "CategoryFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "Configuration": CategoryFilterConfigurationOutputTypeDef,
+        "DefaultFilterControlConfiguration": NotRequired[
+            DefaultFilterControlConfigurationOutputTypeDef
+        ],
+    },
+)
+NumericEqualityFilterOutputTypeDef = TypedDict(
+    "NumericEqualityFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "MatchOperator": NumericEqualityMatchOperatorType,
+        "NullOption": FilterNullOptionType,
+        "Value": NotRequired[float],
+        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
+        "AggregationFunction": NotRequired[AggregationFunctionTypeDef],
+        "ParameterName": NotRequired[str],
+        "DefaultFilterControlConfiguration": NotRequired[
+            DefaultFilterControlConfigurationOutputTypeDef
+        ],
+    },
+)
+NumericRangeFilterOutputTypeDef = TypedDict(
+    "NumericRangeFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "NullOption": FilterNullOptionType,
+        "IncludeMinimum": NotRequired[bool],
+        "IncludeMaximum": NotRequired[bool],
+        "RangeMinimum": NotRequired[NumericRangeFilterValueTypeDef],
+        "RangeMaximum": NotRequired[NumericRangeFilterValueTypeDef],
+        "SelectAllOptions": NotRequired[Literal["FILTER_ALL_VALUES"]],
+        "AggregationFunction": NotRequired[AggregationFunctionTypeDef],
+        "DefaultFilterControlConfiguration": NotRequired[
+            DefaultFilterControlConfigurationOutputTypeDef
+        ],
+    },
+)
+RelativeDatesFilterOutputTypeDef = TypedDict(
+    "RelativeDatesFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "AnchorDateConfiguration": AnchorDateConfigurationTypeDef,
+        "TimeGranularity": TimeGranularityType,
+        "RelativeDateType": RelativeDateTypeType,
+        "NullOption": FilterNullOptionType,
+        "MinimumGranularity": NotRequired[TimeGranularityType],
+        "RelativeDateValue": NotRequired[int],
+        "ParameterName": NotRequired[str],
+        "ExcludePeriodConfiguration": NotRequired[ExcludePeriodConfigurationTypeDef],
+        "DefaultFilterControlConfiguration": NotRequired[
+            DefaultFilterControlConfigurationOutputTypeDef
+        ],
+    },
+)
+TimeEqualityFilterOutputTypeDef = TypedDict(
+    "TimeEqualityFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "Value": NotRequired[datetime],
+        "ParameterName": NotRequired[str],
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "RollingDate": NotRequired[RollingDateConfigurationTypeDef],
+        "DefaultFilterControlConfiguration": NotRequired[
+            DefaultFilterControlConfigurationOutputTypeDef
+        ],
+    },
+)
+TimeRangeFilterOutputTypeDef = TypedDict(
+    "TimeRangeFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "NullOption": FilterNullOptionType,
+        "IncludeMinimum": NotRequired[bool],
+        "IncludeMaximum": NotRequired[bool],
+        "RangeMinimumValue": NotRequired[TimeRangeFilterValueOutputTypeDef],
+        "RangeMaximumValue": NotRequired[TimeRangeFilterValueOutputTypeDef],
+        "ExcludePeriodConfiguration": NotRequired[ExcludePeriodConfigurationTypeDef],
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "DefaultFilterControlConfiguration": NotRequired[
+            DefaultFilterControlConfigurationOutputTypeDef
+        ],
+    },
+)
+TopBottomFilterOutputTypeDef = TypedDict(
+    "TopBottomFilterOutputTypeDef",
+    {
+        "FilterId": str,
+        "Column": ColumnIdentifierTypeDef,
+        "AggregationSortConfigurations": List[AggregationSortConfigurationTypeDef],
+        "Limit": NotRequired[int],
+        "TimeGranularity": NotRequired[TimeGranularityType],
+        "ParameterName": NotRequired[str],
+        "DefaultFilterControlConfiguration": NotRequired[
+            DefaultFilterControlConfigurationOutputTypeDef
+        ],
+    },
+)
 CategoryFilterTypeDef = TypedDict(
     "CategoryFilterTypeDef",
     {
         "FilterId": str,
         "Column": ColumnIdentifierTypeDef,
         "Configuration": CategoryFilterConfigurationTypeDef,
         "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
@@ -10285,22 +12705,52 @@
         "AggregationSortConfigurations": Sequence[AggregationSortConfigurationTypeDef],
         "Limit": NotRequired[int],
         "TimeGranularity": NotRequired[TimeGranularityType],
         "ParameterName": NotRequired[str],
         "DefaultFilterControlConfiguration": NotRequired[DefaultFilterControlConfigurationTypeDef],
     },
 )
+TableFieldOptionsOutputTypeDef = TypedDict(
+    "TableFieldOptionsOutputTypeDef",
+    {
+        "SelectedFieldOptions": NotRequired[List[TableFieldOptionTypeDef]],
+        "Order": NotRequired[List[str]],
+        "PinnedFieldOptions": NotRequired[TablePinnedFieldOptionsOutputTypeDef],
+    },
+)
 TableFieldOptionsTypeDef = TypedDict(
     "TableFieldOptionsTypeDef",
     {
         "SelectedFieldOptions": NotRequired[Sequence[TableFieldOptionTypeDef]],
         "Order": NotRequired[Sequence[str]],
         "PinnedFieldOptions": NotRequired[TablePinnedFieldOptionsTypeDef],
     },
 )
+FilledMapConditionalFormattingOutputTypeDef = TypedDict(
+    "FilledMapConditionalFormattingOutputTypeDef",
+    {
+        "ConditionalFormattingOptions": List[FilledMapConditionalFormattingOptionOutputTypeDef],
+    },
+)
+PivotTableConditionalFormattingOutputTypeDef = TypedDict(
+    "PivotTableConditionalFormattingOutputTypeDef",
+    {
+        "ConditionalFormattingOptions": NotRequired[
+            List[PivotTableConditionalFormattingOptionOutputTypeDef]
+        ],
+    },
+)
+TableConditionalFormattingOutputTypeDef = TypedDict(
+    "TableConditionalFormattingOutputTypeDef",
+    {
+        "ConditionalFormattingOptions": NotRequired[
+            List[TableConditionalFormattingOptionOutputTypeDef]
+        ],
+    },
+)
 FilledMapConditionalFormattingTypeDef = TypedDict(
     "FilledMapConditionalFormattingTypeDef",
     {
         "ConditionalFormattingOptions": Sequence[FilledMapConditionalFormattingOptionTypeDef],
     },
 )
 PivotTableConditionalFormattingTypeDef = TypedDict(
@@ -10323,39 +12773,71 @@
     "UniqueValuesComputationTypeDef",
     {
         "ComputationId": str,
         "Name": NotRequired[str],
         "Category": NotRequired[DimensionFieldTypeDef],
     },
 )
+BarChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "BarChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+        "Colors": NotRequired[List[DimensionFieldTypeDef]],
+        "SmallMultiples": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 BarChartAggregatedFieldWellsTypeDef = TypedDict(
     "BarChartAggregatedFieldWellsTypeDef",
     {
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Colors": NotRequired[Sequence[DimensionFieldTypeDef]],
         "SmallMultiples": NotRequired[Sequence[DimensionFieldTypeDef]],
     },
 )
+BoxPlotAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "BoxPlotAggregatedFieldWellsOutputTypeDef",
+    {
+        "GroupBy": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 BoxPlotAggregatedFieldWellsTypeDef = TypedDict(
     "BoxPlotAggregatedFieldWellsTypeDef",
     {
         "GroupBy": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+ComboChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "ComboChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "BarValues": NotRequired[List[MeasureFieldTypeDef]],
+        "Colors": NotRequired[List[DimensionFieldTypeDef]],
+        "LineValues": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 ComboChartAggregatedFieldWellsTypeDef = TypedDict(
     "ComboChartAggregatedFieldWellsTypeDef",
     {
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "BarValues": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Colors": NotRequired[Sequence[DimensionFieldTypeDef]],
         "LineValues": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+FilledMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "FilledMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Geospatial": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 FilledMapAggregatedFieldWellsTypeDef = TypedDict(
     "FilledMapAggregatedFieldWellsTypeDef",
     {
         "Geospatial": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
@@ -10371,28 +12853,50 @@
         "UpperBoundary": NotRequired[float],
         "LowerBoundary": NotRequired[float],
         "PredictionInterval": NotRequired[int],
         "Seasonality": NotRequired[ForecastComputationSeasonalityType],
         "CustomSeasonalityValue": NotRequired[int],
     },
 )
+FunnelChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "FunnelChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 FunnelChartAggregatedFieldWellsTypeDef = TypedDict(
     "FunnelChartAggregatedFieldWellsTypeDef",
     {
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+GaugeChartFieldWellsOutputTypeDef = TypedDict(
+    "GaugeChartFieldWellsOutputTypeDef",
+    {
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+        "TargetValues": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 GaugeChartFieldWellsTypeDef = TypedDict(
     "GaugeChartFieldWellsTypeDef",
     {
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
         "TargetValues": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+GeospatialMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "GeospatialMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Geospatial": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+        "Colors": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 GeospatialMapAggregatedFieldWellsTypeDef = TypedDict(
     "GeospatialMapAggregatedFieldWellsTypeDef",
     {
         "Geospatial": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Colors": NotRequired[Sequence[DimensionFieldTypeDef]],
     },
@@ -10403,36 +12907,67 @@
         "ComputationId": str,
         "Name": NotRequired[str],
         "Time": NotRequired[DimensionFieldTypeDef],
         "Value": NotRequired[MeasureFieldTypeDef],
         "PeriodSize": NotRequired[int],
     },
 )
+HeatMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "HeatMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Rows": NotRequired[List[DimensionFieldTypeDef]],
+        "Columns": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 HeatMapAggregatedFieldWellsTypeDef = TypedDict(
     "HeatMapAggregatedFieldWellsTypeDef",
     {
         "Rows": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Columns": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+HistogramAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "HistogramAggregatedFieldWellsOutputTypeDef",
+    {
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 HistogramAggregatedFieldWellsTypeDef = TypedDict(
     "HistogramAggregatedFieldWellsTypeDef",
     {
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+KPIFieldWellsOutputTypeDef = TypedDict(
+    "KPIFieldWellsOutputTypeDef",
+    {
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+        "TargetValues": NotRequired[List[MeasureFieldTypeDef]],
+        "TrendGroups": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 KPIFieldWellsTypeDef = TypedDict(
     "KPIFieldWellsTypeDef",
     {
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
         "TargetValues": NotRequired[Sequence[MeasureFieldTypeDef]],
         "TrendGroups": NotRequired[Sequence[DimensionFieldTypeDef]],
     },
 )
+LineChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "LineChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+        "Colors": NotRequired[List[DimensionFieldTypeDef]],
+        "SmallMultiples": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 LineChartAggregatedFieldWellsTypeDef = TypedDict(
     "LineChartAggregatedFieldWellsTypeDef",
     {
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Colors": NotRequired[Sequence[DimensionFieldTypeDef]],
         "SmallMultiples": NotRequired[Sequence[DimensionFieldTypeDef]],
@@ -10473,66 +13008,125 @@
         "ComputationId": str,
         "Name": NotRequired[str],
         "Time": NotRequired[DimensionFieldTypeDef],
         "Value": NotRequired[MeasureFieldTypeDef],
         "PeriodTimeGranularity": NotRequired[TimeGranularityType],
     },
 )
+PieChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "PieChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+        "SmallMultiples": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 PieChartAggregatedFieldWellsTypeDef = TypedDict(
     "PieChartAggregatedFieldWellsTypeDef",
     {
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
         "SmallMultiples": NotRequired[Sequence[DimensionFieldTypeDef]],
     },
 )
+PivotTableAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "PivotTableAggregatedFieldWellsOutputTypeDef",
+    {
+        "Rows": NotRequired[List[DimensionFieldTypeDef]],
+        "Columns": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 PivotTableAggregatedFieldWellsTypeDef = TypedDict(
     "PivotTableAggregatedFieldWellsTypeDef",
     {
         "Rows": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Columns": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+RadarChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "RadarChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "Color": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 RadarChartAggregatedFieldWellsTypeDef = TypedDict(
     "RadarChartAggregatedFieldWellsTypeDef",
     {
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Color": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+SankeyDiagramAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "SankeyDiagramAggregatedFieldWellsOutputTypeDef",
+    {
+        "Source": NotRequired[List[DimensionFieldTypeDef]],
+        "Destination": NotRequired[List[DimensionFieldTypeDef]],
+        "Weight": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 SankeyDiagramAggregatedFieldWellsTypeDef = TypedDict(
     "SankeyDiagramAggregatedFieldWellsTypeDef",
     {
         "Source": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Destination": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Weight": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef",
+    {
+        "XAxis": NotRequired[List[MeasureFieldTypeDef]],
+        "YAxis": NotRequired[List[MeasureFieldTypeDef]],
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "Size": NotRequired[List[MeasureFieldTypeDef]],
+        "Label": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 ScatterPlotCategoricallyAggregatedFieldWellsTypeDef = TypedDict(
     "ScatterPlotCategoricallyAggregatedFieldWellsTypeDef",
     {
         "XAxis": NotRequired[Sequence[MeasureFieldTypeDef]],
         "YAxis": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Size": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Label": NotRequired[Sequence[DimensionFieldTypeDef]],
     },
 )
+ScatterPlotUnaggregatedFieldWellsOutputTypeDef = TypedDict(
+    "ScatterPlotUnaggregatedFieldWellsOutputTypeDef",
+    {
+        "XAxis": NotRequired[List[DimensionFieldTypeDef]],
+        "YAxis": NotRequired[List[DimensionFieldTypeDef]],
+        "Size": NotRequired[List[MeasureFieldTypeDef]],
+        "Category": NotRequired[List[DimensionFieldTypeDef]],
+        "Label": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 ScatterPlotUnaggregatedFieldWellsTypeDef = TypedDict(
     "ScatterPlotUnaggregatedFieldWellsTypeDef",
     {
         "XAxis": NotRequired[Sequence[DimensionFieldTypeDef]],
         "YAxis": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Size": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Category": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Label": NotRequired[Sequence[DimensionFieldTypeDef]],
     },
 )
+TableAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "TableAggregatedFieldWellsOutputTypeDef",
+    {
+        "GroupBy": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 TableAggregatedFieldWellsTypeDef = TypedDict(
     "TableAggregatedFieldWellsTypeDef",
     {
         "GroupBy": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
@@ -10564,43 +13158,81 @@
     "TotalAggregationComputationTypeDef",
     {
         "ComputationId": str,
         "Name": NotRequired[str],
         "Value": NotRequired[MeasureFieldTypeDef],
     },
 )
+TreeMapAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "TreeMapAggregatedFieldWellsOutputTypeDef",
+    {
+        "Groups": NotRequired[List[DimensionFieldTypeDef]],
+        "Sizes": NotRequired[List[MeasureFieldTypeDef]],
+        "Colors": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 TreeMapAggregatedFieldWellsTypeDef = TypedDict(
     "TreeMapAggregatedFieldWellsTypeDef",
     {
         "Groups": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Sizes": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Colors": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+WaterfallChartAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "WaterfallChartAggregatedFieldWellsOutputTypeDef",
+    {
+        "Categories": NotRequired[List[DimensionFieldTypeDef]],
+        "Values": NotRequired[List[MeasureFieldTypeDef]],
+        "Breakdowns": NotRequired[List[DimensionFieldTypeDef]],
+    },
+)
 WaterfallChartAggregatedFieldWellsTypeDef = TypedDict(
     "WaterfallChartAggregatedFieldWellsTypeDef",
     {
         "Categories": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Values": NotRequired[Sequence[MeasureFieldTypeDef]],
         "Breakdowns": NotRequired[Sequence[DimensionFieldTypeDef]],
     },
 )
+WordCloudAggregatedFieldWellsOutputTypeDef = TypedDict(
+    "WordCloudAggregatedFieldWellsOutputTypeDef",
+    {
+        "GroupBy": NotRequired[List[DimensionFieldTypeDef]],
+        "Size": NotRequired[List[MeasureFieldTypeDef]],
+    },
+)
 WordCloudAggregatedFieldWellsTypeDef = TypedDict(
     "WordCloudAggregatedFieldWellsTypeDef",
     {
         "GroupBy": NotRequired[Sequence[DimensionFieldTypeDef]],
         "Size": NotRequired[Sequence[MeasureFieldTypeDef]],
     },
 )
+TableUnaggregatedFieldWellsOutputTypeDef = TypedDict(
+    "TableUnaggregatedFieldWellsOutputTypeDef",
+    {
+        "Values": NotRequired[List[UnaggregatedFieldTypeDef]],
+    },
+)
 TableUnaggregatedFieldWellsTypeDef = TypedDict(
     "TableUnaggregatedFieldWellsTypeDef",
     {
         "Values": NotRequired[Sequence[UnaggregatedFieldTypeDef]],
     },
 )
+SectionBasedLayoutConfigurationOutputTypeDef = TypedDict(
+    "SectionBasedLayoutConfigurationOutputTypeDef",
+    {
+        "HeaderSections": List[HeaderFooterSectionConfigurationOutputTypeDef],
+        "BodySections": List[BodySectionConfigurationOutputTypeDef],
+        "FooterSections": List[HeaderFooterSectionConfigurationOutputTypeDef],
+        "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
+    },
+)
 SectionBasedLayoutConfigurationTypeDef = TypedDict(
     "SectionBasedLayoutConfigurationTypeDef",
     {
         "HeaderSections": Sequence[HeaderFooterSectionConfigurationTypeDef],
         "BodySections": Sequence[BodySectionConfigurationTypeDef],
         "FooterSections": Sequence[HeaderFooterSectionConfigurationTypeDef],
         "CanvasSizeOptions": SectionBasedLayoutCanvasSizeOptionsTypeDef,
@@ -10621,124 +13253,253 @@
     "EmptyVisualTypeDef",
     {
         "VisualId": str,
         "DataSetIdentifier": str,
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+FilterOutputTypeDef = TypedDict(
+    "FilterOutputTypeDef",
+    {
+        "CategoryFilter": NotRequired[CategoryFilterOutputTypeDef],
+        "NumericRangeFilter": NotRequired[NumericRangeFilterOutputTypeDef],
+        "NumericEqualityFilter": NotRequired[NumericEqualityFilterOutputTypeDef],
+        "TimeEqualityFilter": NotRequired[TimeEqualityFilterOutputTypeDef],
+        "TimeRangeFilter": NotRequired[TimeRangeFilterOutputTypeDef],
+        "RelativeDatesFilter": NotRequired[RelativeDatesFilterOutputTypeDef],
+        "TopBottomFilter": NotRequired[TopBottomFilterOutputTypeDef],
+    },
+)
 FilterTypeDef = TypedDict(
     "FilterTypeDef",
     {
         "CategoryFilter": NotRequired[CategoryFilterTypeDef],
         "NumericRangeFilter": NotRequired[NumericRangeFilterTypeDef],
         "NumericEqualityFilter": NotRequired[NumericEqualityFilterTypeDef],
         "TimeEqualityFilter": NotRequired[TimeEqualityFilterTypeDef],
         "TimeRangeFilter": NotRequired[TimeRangeFilterTypeDef],
         "RelativeDatesFilter": NotRequired[RelativeDatesFilterTypeDef],
         "TopBottomFilter": NotRequired[TopBottomFilterTypeDef],
     },
 )
+BarChartFieldWellsOutputTypeDef = TypedDict(
+    "BarChartFieldWellsOutputTypeDef",
+    {
+        "BarChartAggregatedFieldWells": NotRequired[BarChartAggregatedFieldWellsOutputTypeDef],
+    },
+)
 BarChartFieldWellsTypeDef = TypedDict(
     "BarChartFieldWellsTypeDef",
     {
         "BarChartAggregatedFieldWells": NotRequired[BarChartAggregatedFieldWellsTypeDef],
     },
 )
+BoxPlotFieldWellsOutputTypeDef = TypedDict(
+    "BoxPlotFieldWellsOutputTypeDef",
+    {
+        "BoxPlotAggregatedFieldWells": NotRequired[BoxPlotAggregatedFieldWellsOutputTypeDef],
+    },
+)
 BoxPlotFieldWellsTypeDef = TypedDict(
     "BoxPlotFieldWellsTypeDef",
     {
         "BoxPlotAggregatedFieldWells": NotRequired[BoxPlotAggregatedFieldWellsTypeDef],
     },
 )
+ComboChartFieldWellsOutputTypeDef = TypedDict(
+    "ComboChartFieldWellsOutputTypeDef",
+    {
+        "ComboChartAggregatedFieldWells": NotRequired[ComboChartAggregatedFieldWellsOutputTypeDef],
+    },
+)
 ComboChartFieldWellsTypeDef = TypedDict(
     "ComboChartFieldWellsTypeDef",
     {
         "ComboChartAggregatedFieldWells": NotRequired[ComboChartAggregatedFieldWellsTypeDef],
     },
 )
+FilledMapFieldWellsOutputTypeDef = TypedDict(
+    "FilledMapFieldWellsOutputTypeDef",
+    {
+        "FilledMapAggregatedFieldWells": NotRequired[FilledMapAggregatedFieldWellsOutputTypeDef],
+    },
+)
 FilledMapFieldWellsTypeDef = TypedDict(
     "FilledMapFieldWellsTypeDef",
     {
         "FilledMapAggregatedFieldWells": NotRequired[FilledMapAggregatedFieldWellsTypeDef],
     },
 )
+FunnelChartFieldWellsOutputTypeDef = TypedDict(
+    "FunnelChartFieldWellsOutputTypeDef",
+    {
+        "FunnelChartAggregatedFieldWells": NotRequired[
+            FunnelChartAggregatedFieldWellsOutputTypeDef
+        ],
+    },
+)
 FunnelChartFieldWellsTypeDef = TypedDict(
     "FunnelChartFieldWellsTypeDef",
     {
         "FunnelChartAggregatedFieldWells": NotRequired[FunnelChartAggregatedFieldWellsTypeDef],
     },
 )
+GaugeChartConfigurationOutputTypeDef = TypedDict(
+    "GaugeChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[GaugeChartFieldWellsOutputTypeDef],
+        "GaugeChartOptions": NotRequired[GaugeChartOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "TooltipOptions": NotRequired[TooltipOptionsOutputTypeDef],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "ColorConfiguration": NotRequired[GaugeChartColorConfigurationTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 GaugeChartConfigurationTypeDef = TypedDict(
     "GaugeChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[GaugeChartFieldWellsTypeDef],
         "GaugeChartOptions": NotRequired[GaugeChartOptionsTypeDef],
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "TooltipOptions": NotRequired[TooltipOptionsTypeDef],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
+        "ColorConfiguration": NotRequired[GaugeChartColorConfigurationTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+GeospatialMapFieldWellsOutputTypeDef = TypedDict(
+    "GeospatialMapFieldWellsOutputTypeDef",
+    {
+        "GeospatialMapAggregatedFieldWells": NotRequired[
+            GeospatialMapAggregatedFieldWellsOutputTypeDef
+        ],
+    },
+)
 GeospatialMapFieldWellsTypeDef = TypedDict(
     "GeospatialMapFieldWellsTypeDef",
     {
         "GeospatialMapAggregatedFieldWells": NotRequired[GeospatialMapAggregatedFieldWellsTypeDef],
     },
 )
+HeatMapFieldWellsOutputTypeDef = TypedDict(
+    "HeatMapFieldWellsOutputTypeDef",
+    {
+        "HeatMapAggregatedFieldWells": NotRequired[HeatMapAggregatedFieldWellsOutputTypeDef],
+    },
+)
 HeatMapFieldWellsTypeDef = TypedDict(
     "HeatMapFieldWellsTypeDef",
     {
         "HeatMapAggregatedFieldWells": NotRequired[HeatMapAggregatedFieldWellsTypeDef],
     },
 )
+HistogramFieldWellsOutputTypeDef = TypedDict(
+    "HistogramFieldWellsOutputTypeDef",
+    {
+        "HistogramAggregatedFieldWells": NotRequired[HistogramAggregatedFieldWellsOutputTypeDef],
+    },
+)
 HistogramFieldWellsTypeDef = TypedDict(
     "HistogramFieldWellsTypeDef",
     {
         "HistogramAggregatedFieldWells": NotRequired[HistogramAggregatedFieldWellsTypeDef],
     },
 )
+KPIConfigurationOutputTypeDef = TypedDict(
+    "KPIConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[KPIFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[KPISortConfigurationOutputTypeDef],
+        "KPIOptions": NotRequired[KPIOptionsTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 KPIConfigurationTypeDef = TypedDict(
     "KPIConfigurationTypeDef",
     {
         "FieldWells": NotRequired[KPIFieldWellsTypeDef],
         "SortConfiguration": NotRequired[KPISortConfigurationTypeDef],
         "KPIOptions": NotRequired[KPIOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+LineChartFieldWellsOutputTypeDef = TypedDict(
+    "LineChartFieldWellsOutputTypeDef",
+    {
+        "LineChartAggregatedFieldWells": NotRequired[LineChartAggregatedFieldWellsOutputTypeDef],
+    },
+)
 LineChartFieldWellsTypeDef = TypedDict(
     "LineChartFieldWellsTypeDef",
     {
         "LineChartAggregatedFieldWells": NotRequired[LineChartAggregatedFieldWellsTypeDef],
     },
 )
+PieChartFieldWellsOutputTypeDef = TypedDict(
+    "PieChartFieldWellsOutputTypeDef",
+    {
+        "PieChartAggregatedFieldWells": NotRequired[PieChartAggregatedFieldWellsOutputTypeDef],
+    },
+)
 PieChartFieldWellsTypeDef = TypedDict(
     "PieChartFieldWellsTypeDef",
     {
         "PieChartAggregatedFieldWells": NotRequired[PieChartAggregatedFieldWellsTypeDef],
     },
 )
+PivotTableFieldWellsOutputTypeDef = TypedDict(
+    "PivotTableFieldWellsOutputTypeDef",
+    {
+        "PivotTableAggregatedFieldWells": NotRequired[PivotTableAggregatedFieldWellsOutputTypeDef],
+    },
+)
 PivotTableFieldWellsTypeDef = TypedDict(
     "PivotTableFieldWellsTypeDef",
     {
         "PivotTableAggregatedFieldWells": NotRequired[PivotTableAggregatedFieldWellsTypeDef],
     },
 )
+RadarChartFieldWellsOutputTypeDef = TypedDict(
+    "RadarChartFieldWellsOutputTypeDef",
+    {
+        "RadarChartAggregatedFieldWells": NotRequired[RadarChartAggregatedFieldWellsOutputTypeDef],
+    },
+)
 RadarChartFieldWellsTypeDef = TypedDict(
     "RadarChartFieldWellsTypeDef",
     {
         "RadarChartAggregatedFieldWells": NotRequired[RadarChartAggregatedFieldWellsTypeDef],
     },
 )
+SankeyDiagramFieldWellsOutputTypeDef = TypedDict(
+    "SankeyDiagramFieldWellsOutputTypeDef",
+    {
+        "SankeyDiagramAggregatedFieldWells": NotRequired[
+            SankeyDiagramAggregatedFieldWellsOutputTypeDef
+        ],
+    },
+)
 SankeyDiagramFieldWellsTypeDef = TypedDict(
     "SankeyDiagramFieldWellsTypeDef",
     {
         "SankeyDiagramAggregatedFieldWells": NotRequired[SankeyDiagramAggregatedFieldWellsTypeDef],
     },
 )
+ScatterPlotFieldWellsOutputTypeDef = TypedDict(
+    "ScatterPlotFieldWellsOutputTypeDef",
+    {
+        "ScatterPlotCategoricallyAggregatedFieldWells": NotRequired[
+            ScatterPlotCategoricallyAggregatedFieldWellsOutputTypeDef
+        ],
+        "ScatterPlotUnaggregatedFieldWells": NotRequired[
+            ScatterPlotUnaggregatedFieldWellsOutputTypeDef
+        ],
+    },
+)
 ScatterPlotFieldWellsTypeDef = TypedDict(
     "ScatterPlotFieldWellsTypeDef",
     {
         "ScatterPlotCategoricallyAggregatedFieldWells": NotRequired[
             ScatterPlotCategoricallyAggregatedFieldWellsTypeDef
         ],
         "ScatterPlotUnaggregatedFieldWells": NotRequired[ScatterPlotUnaggregatedFieldWellsTypeDef],
@@ -10755,59 +13516,126 @@
         "PeriodOverPeriod": NotRequired[PeriodOverPeriodComputationTypeDef],
         "PeriodToDate": NotRequired[PeriodToDateComputationTypeDef],
         "GrowthRate": NotRequired[GrowthRateComputationTypeDef],
         "UniqueValues": NotRequired[UniqueValuesComputationTypeDef],
         "Forecast": NotRequired[ForecastComputationTypeDef],
     },
 )
+TreeMapFieldWellsOutputTypeDef = TypedDict(
+    "TreeMapFieldWellsOutputTypeDef",
+    {
+        "TreeMapAggregatedFieldWells": NotRequired[TreeMapAggregatedFieldWellsOutputTypeDef],
+    },
+)
 TreeMapFieldWellsTypeDef = TypedDict(
     "TreeMapFieldWellsTypeDef",
     {
         "TreeMapAggregatedFieldWells": NotRequired[TreeMapAggregatedFieldWellsTypeDef],
     },
 )
+WaterfallChartFieldWellsOutputTypeDef = TypedDict(
+    "WaterfallChartFieldWellsOutputTypeDef",
+    {
+        "WaterfallChartAggregatedFieldWells": NotRequired[
+            WaterfallChartAggregatedFieldWellsOutputTypeDef
+        ],
+    },
+)
 WaterfallChartFieldWellsTypeDef = TypedDict(
     "WaterfallChartFieldWellsTypeDef",
     {
         "WaterfallChartAggregatedFieldWells": NotRequired[
             WaterfallChartAggregatedFieldWellsTypeDef
         ],
     },
 )
+WordCloudFieldWellsOutputTypeDef = TypedDict(
+    "WordCloudFieldWellsOutputTypeDef",
+    {
+        "WordCloudAggregatedFieldWells": NotRequired[WordCloudAggregatedFieldWellsOutputTypeDef],
+    },
+)
 WordCloudFieldWellsTypeDef = TypedDict(
     "WordCloudFieldWellsTypeDef",
     {
         "WordCloudAggregatedFieldWells": NotRequired[WordCloudAggregatedFieldWellsTypeDef],
     },
 )
+TableFieldWellsOutputTypeDef = TypedDict(
+    "TableFieldWellsOutputTypeDef",
+    {
+        "TableAggregatedFieldWells": NotRequired[TableAggregatedFieldWellsOutputTypeDef],
+        "TableUnaggregatedFieldWells": NotRequired[TableUnaggregatedFieldWellsOutputTypeDef],
+    },
+)
 TableFieldWellsTypeDef = TypedDict(
     "TableFieldWellsTypeDef",
     {
         "TableAggregatedFieldWells": NotRequired[TableAggregatedFieldWellsTypeDef],
         "TableUnaggregatedFieldWells": NotRequired[TableUnaggregatedFieldWellsTypeDef],
     },
 )
+LayoutConfigurationOutputTypeDef = TypedDict(
+    "LayoutConfigurationOutputTypeDef",
+    {
+        "GridLayout": NotRequired[GridLayoutConfigurationOutputTypeDef],
+        "FreeFormLayout": NotRequired[FreeFormLayoutConfigurationOutputTypeDef],
+        "SectionBasedLayout": NotRequired[SectionBasedLayoutConfigurationOutputTypeDef],
+    },
+)
 LayoutConfigurationTypeDef = TypedDict(
     "LayoutConfigurationTypeDef",
     {
         "GridLayout": NotRequired[GridLayoutConfigurationTypeDef],
         "FreeFormLayout": NotRequired[FreeFormLayoutConfigurationTypeDef],
         "SectionBasedLayout": NotRequired[SectionBasedLayoutConfigurationTypeDef],
     },
 )
+FilterGroupOutputTypeDef = TypedDict(
+    "FilterGroupOutputTypeDef",
+    {
+        "FilterGroupId": str,
+        "Filters": List[FilterOutputTypeDef],
+        "ScopeConfiguration": FilterScopeConfigurationOutputTypeDef,
+        "CrossDataset": CrossDatasetTypesType,
+        "Status": NotRequired[WidgetStatusType],
+    },
+)
 FilterGroupTypeDef = TypedDict(
     "FilterGroupTypeDef",
     {
         "FilterGroupId": str,
         "Filters": Sequence[FilterTypeDef],
         "ScopeConfiguration": FilterScopeConfigurationTypeDef,
         "CrossDataset": CrossDatasetTypesType,
         "Status": NotRequired[WidgetStatusType],
     },
 )
+BarChartConfigurationOutputTypeDef = TypedDict(
+    "BarChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[BarChartFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[BarChartSortConfigurationOutputTypeDef],
+        "Orientation": NotRequired[BarChartOrientationType],
+        "BarsArrangement": NotRequired[BarsArrangementType],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "SmallMultiplesOptions": NotRequired[SmallMultiplesOptionsTypeDef],
+        "CategoryAxis": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ValueAxis": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "ValueLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ColorLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "ReferenceLines": NotRequired[List[ReferenceLineTypeDef]],
+        "ContributionAnalysisDefaults": NotRequired[List[ContributionAnalysisDefaultOutputTypeDef]],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 BarChartConfigurationTypeDef = TypedDict(
     "BarChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[BarChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[BarChartSortConfigurationTypeDef],
         "Orientation": NotRequired[BarChartOrientationType],
         "BarsArrangement": NotRequired[BarsArrangementType],
@@ -10822,14 +13650,31 @@
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "ReferenceLines": NotRequired[Sequence[ReferenceLineTypeDef]],
         "ContributionAnalysisDefaults": NotRequired[Sequence[ContributionAnalysisDefaultTypeDef]],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+BoxPlotChartConfigurationOutputTypeDef = TypedDict(
+    "BoxPlotChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[BoxPlotFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[BoxPlotSortConfigurationOutputTypeDef],
+        "BoxPlotOptions": NotRequired[BoxPlotOptionsTypeDef],
+        "CategoryAxis": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "PrimaryYAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "PrimaryYAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "ReferenceLines": NotRequired[List[ReferenceLineTypeDef]],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 BoxPlotChartConfigurationTypeDef = TypedDict(
     "BoxPlotChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[BoxPlotFieldWellsTypeDef],
         "SortConfiguration": NotRequired[BoxPlotSortConfigurationTypeDef],
         "BoxPlotOptions": NotRequired[BoxPlotOptionsTypeDef],
         "CategoryAxis": NotRequired[AxisDisplayOptionsTypeDef],
@@ -10839,14 +13684,37 @@
         "Legend": NotRequired[LegendOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "ReferenceLines": NotRequired[Sequence[ReferenceLineTypeDef]],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+ComboChartConfigurationOutputTypeDef = TypedDict(
+    "ComboChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[ComboChartFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[ComboChartSortConfigurationOutputTypeDef],
+        "BarsArrangement": NotRequired[BarsArrangementType],
+        "CategoryAxis": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "PrimaryYAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "PrimaryYAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "SecondaryYAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "SecondaryYAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "SingleAxisOptions": NotRequired[SingleAxisOptionsTypeDef],
+        "ColorLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "BarDataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "LineDataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "ReferenceLines": NotRequired[List[ReferenceLineTypeDef]],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 ComboChartConfigurationTypeDef = TypedDict(
     "ComboChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[ComboChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[ComboChartSortConfigurationTypeDef],
         "BarsArrangement": NotRequired[BarsArrangementType],
         "CategoryAxis": NotRequired[AxisDisplayOptionsTypeDef],
@@ -10862,103 +13730,218 @@
         "LineDataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "ReferenceLines": NotRequired[Sequence[ReferenceLineTypeDef]],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+FilledMapConfigurationOutputTypeDef = TypedDict(
+    "FilledMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[FilledMapFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[FilledMapSortConfigurationOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "WindowOptions": NotRequired[GeospatialWindowOptionsTypeDef],
+        "MapStyleOptions": NotRequired[GeospatialMapStyleOptionsTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 FilledMapConfigurationTypeDef = TypedDict(
     "FilledMapConfigurationTypeDef",
     {
         "FieldWells": NotRequired[FilledMapFieldWellsTypeDef],
         "SortConfiguration": NotRequired[FilledMapSortConfigurationTypeDef],
         "Legend": NotRequired[LegendOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "WindowOptions": NotRequired[GeospatialWindowOptionsTypeDef],
         "MapStyleOptions": NotRequired[GeospatialMapStyleOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+FunnelChartConfigurationOutputTypeDef = TypedDict(
+    "FunnelChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[FunnelChartFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[FunnelChartSortConfigurationOutputTypeDef],
+        "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ValueLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "DataLabelOptions": NotRequired[FunnelChartDataLabelOptionsTypeDef],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 FunnelChartConfigurationTypeDef = TypedDict(
     "FunnelChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[FunnelChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[FunnelChartSortConfigurationTypeDef],
         "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "ValueLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "DataLabelOptions": NotRequired[FunnelChartDataLabelOptionsTypeDef],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+GaugeChartVisualOutputTypeDef = TypedDict(
+    "GaugeChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[GaugeChartConfigurationOutputTypeDef],
+        "ConditionalFormatting": NotRequired[GaugeChartConditionalFormattingOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 GaugeChartVisualTypeDef = TypedDict(
     "GaugeChartVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[GaugeChartConfigurationTypeDef],
         "ConditionalFormatting": NotRequired[GaugeChartConditionalFormattingTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+GeospatialMapConfigurationOutputTypeDef = TypedDict(
+    "GeospatialMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[GeospatialMapFieldWellsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "WindowOptions": NotRequired[GeospatialWindowOptionsTypeDef],
+        "MapStyleOptions": NotRequired[GeospatialMapStyleOptionsTypeDef],
+        "PointStyleOptions": NotRequired[GeospatialPointStyleOptionsOutputTypeDef],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 GeospatialMapConfigurationTypeDef = TypedDict(
     "GeospatialMapConfigurationTypeDef",
     {
         "FieldWells": NotRequired[GeospatialMapFieldWellsTypeDef],
         "Legend": NotRequired[LegendOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "WindowOptions": NotRequired[GeospatialWindowOptionsTypeDef],
         "MapStyleOptions": NotRequired[GeospatialMapStyleOptionsTypeDef],
         "PointStyleOptions": NotRequired[GeospatialPointStyleOptionsTypeDef],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+HeatMapConfigurationOutputTypeDef = TypedDict(
+    "HeatMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[HeatMapFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[HeatMapSortConfigurationOutputTypeDef],
+        "RowLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ColumnLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ColorScale": NotRequired[ColorScaleOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 HeatMapConfigurationTypeDef = TypedDict(
     "HeatMapConfigurationTypeDef",
     {
         "FieldWells": NotRequired[HeatMapFieldWellsTypeDef],
         "SortConfiguration": NotRequired[HeatMapSortConfigurationTypeDef],
         "RowLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "ColumnLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "ColorScale": NotRequired[ColorScaleTypeDef],
         "Legend": NotRequired[LegendOptionsTypeDef],
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+HistogramConfigurationOutputTypeDef = TypedDict(
+    "HistogramConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[HistogramFieldWellsOutputTypeDef],
+        "XAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "XAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "YAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "BinOptions": NotRequired[HistogramBinOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 HistogramConfigurationTypeDef = TypedDict(
     "HistogramConfigurationTypeDef",
     {
         "FieldWells": NotRequired[HistogramFieldWellsTypeDef],
         "XAxisDisplayOptions": NotRequired[AxisDisplayOptionsTypeDef],
         "XAxisLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "YAxisDisplayOptions": NotRequired[AxisDisplayOptionsTypeDef],
         "BinOptions": NotRequired[HistogramBinOptionsTypeDef],
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+KPIVisualOutputTypeDef = TypedDict(
+    "KPIVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[KPIConfigurationOutputTypeDef],
+        "ConditionalFormatting": NotRequired[KPIConditionalFormattingOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 KPIVisualTypeDef = TypedDict(
     "KPIVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[KPIConfigurationTypeDef],
         "ConditionalFormatting": NotRequired[KPIConditionalFormattingTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+LineChartConfigurationOutputTypeDef = TypedDict(
+    "LineChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[LineChartFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[LineChartSortConfigurationOutputTypeDef],
+        "ForecastConfigurations": NotRequired[List[ForecastConfigurationOutputTypeDef]],
+        "Type": NotRequired[LineChartTypeType],
+        "SmallMultiplesOptions": NotRequired[SmallMultiplesOptionsTypeDef],
+        "XAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "XAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "PrimaryYAxisDisplayOptions": NotRequired[LineSeriesAxisDisplayOptionsOutputTypeDef],
+        "PrimaryYAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "SecondaryYAxisDisplayOptions": NotRequired[LineSeriesAxisDisplayOptionsOutputTypeDef],
+        "SecondaryYAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "SingleAxisOptions": NotRequired[SingleAxisOptionsTypeDef],
+        "DefaultSeriesSettings": NotRequired[LineChartDefaultSeriesSettingsTypeDef],
+        "Series": NotRequired[List[SeriesItemTypeDef]],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "ReferenceLines": NotRequired[List[ReferenceLineTypeDef]],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "ContributionAnalysisDefaults": NotRequired[List[ContributionAnalysisDefaultOutputTypeDef]],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 LineChartConfigurationTypeDef = TypedDict(
     "LineChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[LineChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[LineChartSortConfigurationTypeDef],
         "ForecastConfigurations": NotRequired[Sequence[ForecastConfigurationTypeDef]],
         "Type": NotRequired[LineChartTypeType],
@@ -10977,14 +13960,31 @@
         "ReferenceLines": NotRequired[Sequence[ReferenceLineTypeDef]],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "ContributionAnalysisDefaults": NotRequired[Sequence[ContributionAnalysisDefaultTypeDef]],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+PieChartConfigurationOutputTypeDef = TypedDict(
+    "PieChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[PieChartFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[PieChartSortConfigurationOutputTypeDef],
+        "DonutOptions": NotRequired[DonutOptionsTypeDef],
+        "SmallMultiplesOptions": NotRequired[SmallMultiplesOptionsTypeDef],
+        "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ValueLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "ContributionAnalysisDefaults": NotRequired[List[ContributionAnalysisDefaultOutputTypeDef]],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 PieChartConfigurationTypeDef = TypedDict(
     "PieChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[PieChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[PieChartSortConfigurationTypeDef],
         "DonutOptions": NotRequired[DonutOptionsTypeDef],
         "SmallMultiplesOptions": NotRequired[SmallMultiplesOptionsTypeDef],
@@ -10994,26 +13994,59 @@
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "ContributionAnalysisDefaults": NotRequired[Sequence[ContributionAnalysisDefaultTypeDef]],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+PivotTableConfigurationOutputTypeDef = TypedDict(
+    "PivotTableConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[PivotTableFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[PivotTableSortConfigurationOutputTypeDef],
+        "TableOptions": NotRequired[PivotTableOptionsOutputTypeDef],
+        "TotalOptions": NotRequired[PivotTableTotalOptionsOutputTypeDef],
+        "FieldOptions": NotRequired[PivotTableFieldOptionsOutputTypeDef],
+        "PaginatedReportOptions": NotRequired[PivotTablePaginatedReportOptionsTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 PivotTableConfigurationTypeDef = TypedDict(
     "PivotTableConfigurationTypeDef",
     {
         "FieldWells": NotRequired[PivotTableFieldWellsTypeDef],
         "SortConfiguration": NotRequired[PivotTableSortConfigurationTypeDef],
         "TableOptions": NotRequired[PivotTableOptionsTypeDef],
         "TotalOptions": NotRequired[PivotTableTotalOptionsTypeDef],
         "FieldOptions": NotRequired[PivotTableFieldOptionsTypeDef],
         "PaginatedReportOptions": NotRequired[PivotTablePaginatedReportOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+RadarChartConfigurationOutputTypeDef = TypedDict(
+    "RadarChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[RadarChartFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[RadarChartSortConfigurationOutputTypeDef],
+        "Shape": NotRequired[RadarChartShapeType],
+        "BaseSeriesSettings": NotRequired[RadarChartSeriesSettingsTypeDef],
+        "StartAngle": NotRequired[float],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "AlternateBandColorsVisibility": NotRequired[VisibilityType],
+        "AlternateBandEvenColor": NotRequired[str],
+        "AlternateBandOddColor": NotRequired[str],
+        "CategoryAxis": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ColorAxis": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "ColorLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "AxesRangeScale": NotRequired[RadarChartAxesRangeScaleType],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 RadarChartConfigurationTypeDef = TypedDict(
     "RadarChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[RadarChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[RadarChartSortConfigurationTypeDef],
         "Shape": NotRequired[RadarChartShapeType],
         "BaseSeriesSettings": NotRequired[RadarChartSeriesSettingsTypeDef],
@@ -11027,23 +14060,48 @@
         "ColorAxis": NotRequired[AxisDisplayOptionsTypeDef],
         "ColorLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "Legend": NotRequired[LegendOptionsTypeDef],
         "AxesRangeScale": NotRequired[RadarChartAxesRangeScaleType],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+SankeyDiagramChartConfigurationOutputTypeDef = TypedDict(
+    "SankeyDiagramChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[SankeyDiagramFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[SankeyDiagramSortConfigurationOutputTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 SankeyDiagramChartConfigurationTypeDef = TypedDict(
     "SankeyDiagramChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[SankeyDiagramFieldWellsTypeDef],
         "SortConfiguration": NotRequired[SankeyDiagramSortConfigurationTypeDef],
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+ScatterPlotConfigurationOutputTypeDef = TypedDict(
+    "ScatterPlotConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[ScatterPlotFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[ScatterPlotSortConfigurationTypeDef],
+        "XAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "XAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "YAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "YAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 ScatterPlotConfigurationTypeDef = TypedDict(
     "ScatterPlotConfigurationTypeDef",
     {
         "FieldWells": NotRequired[ScatterPlotFieldWellsTypeDef],
         "SortConfiguration": NotRequired[ScatterPlotSortConfigurationTypeDef],
         "XAxisLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "XAxisDisplayOptions": NotRequired[AxisDisplayOptionsTypeDef],
@@ -11052,22 +14110,45 @@
         "Legend": NotRequired[LegendOptionsTypeDef],
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+InsightConfigurationOutputTypeDef = TypedDict(
+    "InsightConfigurationOutputTypeDef",
+    {
+        "Computations": NotRequired[List[ComputationTypeDef]],
+        "CustomNarrative": NotRequired[CustomNarrativeOptionsTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 InsightConfigurationTypeDef = TypedDict(
     "InsightConfigurationTypeDef",
     {
         "Computations": NotRequired[Sequence[ComputationTypeDef]],
         "CustomNarrative": NotRequired[CustomNarrativeOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+TreeMapConfigurationOutputTypeDef = TypedDict(
+    "TreeMapConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[TreeMapFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[TreeMapSortConfigurationOutputTypeDef],
+        "GroupLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "SizeLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ColorLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "ColorScale": NotRequired[ColorScaleOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "Tooltip": NotRequired[TooltipOptionsOutputTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 TreeMapConfigurationTypeDef = TypedDict(
     "TreeMapConfigurationTypeDef",
     {
         "FieldWells": NotRequired[TreeMapFieldWellsTypeDef],
         "SortConfiguration": NotRequired[TreeMapSortConfigurationTypeDef],
         "GroupLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "SizeLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
@@ -11075,14 +14156,31 @@
         "ColorScale": NotRequired[ColorScaleTypeDef],
         "Legend": NotRequired[LegendOptionsTypeDef],
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "Tooltip": NotRequired[TooltipOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+WaterfallChartConfigurationOutputTypeDef = TypedDict(
+    "WaterfallChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[WaterfallChartFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[WaterfallChartSortConfigurationOutputTypeDef],
+        "WaterfallChartOptions": NotRequired[WaterfallChartOptionsTypeDef],
+        "CategoryAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "CategoryAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "PrimaryYAxisLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "PrimaryYAxisDisplayOptions": NotRequired[AxisDisplayOptionsOutputTypeDef],
+        "Legend": NotRequired[LegendOptionsTypeDef],
+        "DataLabels": NotRequired[DataLabelOptionsOutputTypeDef],
+        "VisualPalette": NotRequired[VisualPaletteOutputTypeDef],
+        "ColorConfiguration": NotRequired[WaterfallChartColorConfigurationTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 WaterfallChartConfigurationTypeDef = TypedDict(
     "WaterfallChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[WaterfallChartFieldWellsTypeDef],
         "SortConfiguration": NotRequired[WaterfallChartSortConfigurationTypeDef],
         "WaterfallChartOptions": NotRequired[WaterfallChartOptionsTypeDef],
         "CategoryAxisLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
@@ -11092,251 +14190,516 @@
         "Legend": NotRequired[LegendOptionsTypeDef],
         "DataLabels": NotRequired[DataLabelOptionsTypeDef],
         "VisualPalette": NotRequired[VisualPaletteTypeDef],
         "ColorConfiguration": NotRequired[WaterfallChartColorConfigurationTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+WordCloudChartConfigurationOutputTypeDef = TypedDict(
+    "WordCloudChartConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[WordCloudFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[WordCloudSortConfigurationOutputTypeDef],
+        "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsOutputTypeDef],
+        "WordCloudOptions": NotRequired[WordCloudOptionsTypeDef],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 WordCloudChartConfigurationTypeDef = TypedDict(
     "WordCloudChartConfigurationTypeDef",
     {
         "FieldWells": NotRequired[WordCloudFieldWellsTypeDef],
         "SortConfiguration": NotRequired[WordCloudSortConfigurationTypeDef],
         "CategoryLabelOptions": NotRequired[ChartAxisLabelOptionsTypeDef],
         "WordCloudOptions": NotRequired[WordCloudOptionsTypeDef],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+TableConfigurationOutputTypeDef = TypedDict(
+    "TableConfigurationOutputTypeDef",
+    {
+        "FieldWells": NotRequired[TableFieldWellsOutputTypeDef],
+        "SortConfiguration": NotRequired[TableSortConfigurationOutputTypeDef],
+        "TableOptions": NotRequired[TableOptionsOutputTypeDef],
+        "TotalOptions": NotRequired[TotalOptionsOutputTypeDef],
+        "FieldOptions": NotRequired[TableFieldOptionsOutputTypeDef],
+        "PaginatedReportOptions": NotRequired[TablePaginatedReportOptionsTypeDef],
+        "TableInlineVisualizations": NotRequired[List[TableInlineVisualizationTypeDef]],
+        "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
+    },
+)
 TableConfigurationTypeDef = TypedDict(
     "TableConfigurationTypeDef",
     {
         "FieldWells": NotRequired[TableFieldWellsTypeDef],
         "SortConfiguration": NotRequired[TableSortConfigurationTypeDef],
         "TableOptions": NotRequired[TableOptionsTypeDef],
         "TotalOptions": NotRequired[TotalOptionsTypeDef],
         "FieldOptions": NotRequired[TableFieldOptionsTypeDef],
         "PaginatedReportOptions": NotRequired[TablePaginatedReportOptionsTypeDef],
         "TableInlineVisualizations": NotRequired[Sequence[TableInlineVisualizationTypeDef]],
         "Interactions": NotRequired[VisualInteractionOptionsTypeDef],
     },
 )
+LayoutOutputTypeDef = TypedDict(
+    "LayoutOutputTypeDef",
+    {
+        "Configuration": LayoutConfigurationOutputTypeDef,
+    },
+)
 LayoutTypeDef = TypedDict(
     "LayoutTypeDef",
     {
         "Configuration": LayoutConfigurationTypeDef,
     },
 )
+BarChartVisualOutputTypeDef = TypedDict(
+    "BarChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[BarChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 BarChartVisualTypeDef = TypedDict(
     "BarChartVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[BarChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+BoxPlotVisualOutputTypeDef = TypedDict(
+    "BoxPlotVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[BoxPlotChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 BoxPlotVisualTypeDef = TypedDict(
     "BoxPlotVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[BoxPlotChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+ComboChartVisualOutputTypeDef = TypedDict(
+    "ComboChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[ComboChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 ComboChartVisualTypeDef = TypedDict(
     "ComboChartVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[ComboChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+FilledMapVisualOutputTypeDef = TypedDict(
+    "FilledMapVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[FilledMapConfigurationOutputTypeDef],
+        "ConditionalFormatting": NotRequired[FilledMapConditionalFormattingOutputTypeDef],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 FilledMapVisualTypeDef = TypedDict(
     "FilledMapVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[FilledMapConfigurationTypeDef],
         "ConditionalFormatting": NotRequired[FilledMapConditionalFormattingTypeDef],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+FunnelChartVisualOutputTypeDef = TypedDict(
+    "FunnelChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[FunnelChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 FunnelChartVisualTypeDef = TypedDict(
     "FunnelChartVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[FunnelChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+GeospatialMapVisualOutputTypeDef = TypedDict(
+    "GeospatialMapVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[GeospatialMapConfigurationOutputTypeDef],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 GeospatialMapVisualTypeDef = TypedDict(
     "GeospatialMapVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[GeospatialMapConfigurationTypeDef],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+HeatMapVisualOutputTypeDef = TypedDict(
+    "HeatMapVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[HeatMapConfigurationOutputTypeDef],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 HeatMapVisualTypeDef = TypedDict(
     "HeatMapVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[HeatMapConfigurationTypeDef],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+HistogramVisualOutputTypeDef = TypedDict(
+    "HistogramVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[HistogramConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 HistogramVisualTypeDef = TypedDict(
     "HistogramVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[HistogramConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+LineChartVisualOutputTypeDef = TypedDict(
+    "LineChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[LineChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 LineChartVisualTypeDef = TypedDict(
     "LineChartVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[LineChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+PieChartVisualOutputTypeDef = TypedDict(
+    "PieChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[PieChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 PieChartVisualTypeDef = TypedDict(
     "PieChartVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[PieChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+PivotTableVisualOutputTypeDef = TypedDict(
+    "PivotTableVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[PivotTableConfigurationOutputTypeDef],
+        "ConditionalFormatting": NotRequired[PivotTableConditionalFormattingOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 PivotTableVisualTypeDef = TypedDict(
     "PivotTableVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[PivotTableConfigurationTypeDef],
         "ConditionalFormatting": NotRequired[PivotTableConditionalFormattingTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+RadarChartVisualOutputTypeDef = TypedDict(
+    "RadarChartVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[RadarChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 RadarChartVisualTypeDef = TypedDict(
     "RadarChartVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[RadarChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+SankeyDiagramVisualOutputTypeDef = TypedDict(
+    "SankeyDiagramVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[SankeyDiagramChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 SankeyDiagramVisualTypeDef = TypedDict(
     "SankeyDiagramVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[SankeyDiagramChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+ScatterPlotVisualOutputTypeDef = TypedDict(
+    "ScatterPlotVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[ScatterPlotConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 ScatterPlotVisualTypeDef = TypedDict(
     "ScatterPlotVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[ScatterPlotConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+InsightVisualOutputTypeDef = TypedDict(
+    "InsightVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "DataSetIdentifier": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "InsightConfiguration": NotRequired[InsightConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 InsightVisualTypeDef = TypedDict(
     "InsightVisualTypeDef",
     {
         "VisualId": str,
         "DataSetIdentifier": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "InsightConfiguration": NotRequired[InsightConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+TreeMapVisualOutputTypeDef = TypedDict(
+    "TreeMapVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[TreeMapConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 TreeMapVisualTypeDef = TypedDict(
     "TreeMapVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[TreeMapConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+WaterfallVisualOutputTypeDef = TypedDict(
+    "WaterfallVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[WaterfallChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 WaterfallVisualTypeDef = TypedDict(
     "WaterfallVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[WaterfallChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+WordCloudVisualOutputTypeDef = TypedDict(
+    "WordCloudVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[WordCloudChartConfigurationOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+        "ColumnHierarchies": NotRequired[List[ColumnHierarchyOutputTypeDef]],
+    },
+)
 WordCloudVisualTypeDef = TypedDict(
     "WordCloudVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[WordCloudChartConfigurationTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
         "ColumnHierarchies": NotRequired[Sequence[ColumnHierarchyTypeDef]],
     },
 )
+TableVisualOutputTypeDef = TypedDict(
+    "TableVisualOutputTypeDef",
+    {
+        "VisualId": str,
+        "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
+        "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
+        "ChartConfiguration": NotRequired[TableConfigurationOutputTypeDef],
+        "ConditionalFormatting": NotRequired[TableConditionalFormattingOutputTypeDef],
+        "Actions": NotRequired[List[VisualCustomActionOutputTypeDef]],
+    },
+)
 TableVisualTypeDef = TypedDict(
     "TableVisualTypeDef",
     {
         "VisualId": str,
         "Title": NotRequired[VisualTitleLabelOptionsTypeDef],
         "Subtitle": NotRequired[VisualSubtitleLabelOptionsTypeDef],
         "ChartConfiguration": NotRequired[TableConfigurationTypeDef],
         "ConditionalFormatting": NotRequired[TableConditionalFormattingTypeDef],
         "Actions": NotRequired[Sequence[VisualCustomActionTypeDef]],
     },
 )
+VisualOutputTypeDef = TypedDict(
+    "VisualOutputTypeDef",
+    {
+        "TableVisual": NotRequired[TableVisualOutputTypeDef],
+        "PivotTableVisual": NotRequired[PivotTableVisualOutputTypeDef],
+        "BarChartVisual": NotRequired[BarChartVisualOutputTypeDef],
+        "KPIVisual": NotRequired[KPIVisualOutputTypeDef],
+        "PieChartVisual": NotRequired[PieChartVisualOutputTypeDef],
+        "GaugeChartVisual": NotRequired[GaugeChartVisualOutputTypeDef],
+        "LineChartVisual": NotRequired[LineChartVisualOutputTypeDef],
+        "HeatMapVisual": NotRequired[HeatMapVisualOutputTypeDef],
+        "TreeMapVisual": NotRequired[TreeMapVisualOutputTypeDef],
+        "GeospatialMapVisual": NotRequired[GeospatialMapVisualOutputTypeDef],
+        "FilledMapVisual": NotRequired[FilledMapVisualOutputTypeDef],
+        "FunnelChartVisual": NotRequired[FunnelChartVisualOutputTypeDef],
+        "ScatterPlotVisual": NotRequired[ScatterPlotVisualOutputTypeDef],
+        "ComboChartVisual": NotRequired[ComboChartVisualOutputTypeDef],
+        "BoxPlotVisual": NotRequired[BoxPlotVisualOutputTypeDef],
+        "WaterfallVisual": NotRequired[WaterfallVisualOutputTypeDef],
+        "HistogramVisual": NotRequired[HistogramVisualOutputTypeDef],
+        "WordCloudVisual": NotRequired[WordCloudVisualOutputTypeDef],
+        "InsightVisual": NotRequired[InsightVisualOutputTypeDef],
+        "SankeyDiagramVisual": NotRequired[SankeyDiagramVisualOutputTypeDef],
+        "CustomContentVisual": NotRequired[CustomContentVisualOutputTypeDef],
+        "EmptyVisual": NotRequired[EmptyVisualOutputTypeDef],
+        "RadarChartVisual": NotRequired[RadarChartVisualOutputTypeDef],
+    },
+)
 VisualTypeDef = TypedDict(
     "VisualTypeDef",
     {
         "TableVisual": NotRequired[TableVisualTypeDef],
         "PivotTableVisual": NotRequired[PivotTableVisualTypeDef],
         "BarChartVisual": NotRequired[BarChartVisualTypeDef],
         "KPIVisual": NotRequired[KPIVisualTypeDef],
@@ -11357,14 +14720,30 @@
         "InsightVisual": NotRequired[InsightVisualTypeDef],
         "SankeyDiagramVisual": NotRequired[SankeyDiagramVisualTypeDef],
         "CustomContentVisual": NotRequired[CustomContentVisualTypeDef],
         "EmptyVisual": NotRequired[EmptyVisualTypeDef],
         "RadarChartVisual": NotRequired[RadarChartVisualTypeDef],
     },
 )
+SheetDefinitionOutputTypeDef = TypedDict(
+    "SheetDefinitionOutputTypeDef",
+    {
+        "SheetId": str,
+        "Title": NotRequired[str],
+        "Description": NotRequired[str],
+        "Name": NotRequired[str],
+        "ParameterControls": NotRequired[List[ParameterControlOutputTypeDef]],
+        "FilterControls": NotRequired[List[FilterControlOutputTypeDef]],
+        "Visuals": NotRequired[List[VisualOutputTypeDef]],
+        "TextBoxes": NotRequired[List[SheetTextBoxTypeDef]],
+        "Layouts": NotRequired[List[LayoutOutputTypeDef]],
+        "SheetControlLayouts": NotRequired[List[SheetControlLayoutOutputTypeDef]],
+        "ContentType": NotRequired[SheetContentTypeType],
+    },
+)
 SheetDefinitionTypeDef = TypedDict(
     "SheetDefinitionTypeDef",
     {
         "SheetId": str,
         "Title": NotRequired[str],
         "Description": NotRequired[str],
         "Name": NotRequired[str],
@@ -11373,14 +14752,53 @@
         "Visuals": NotRequired[Sequence[VisualTypeDef]],
         "TextBoxes": NotRequired[Sequence[SheetTextBoxTypeDef]],
         "Layouts": NotRequired[Sequence[LayoutTypeDef]],
         "SheetControlLayouts": NotRequired[Sequence[SheetControlLayoutTypeDef]],
         "ContentType": NotRequired[SheetContentTypeType],
     },
 )
+AnalysisDefinitionOutputTypeDef = TypedDict(
+    "AnalysisDefinitionOutputTypeDef",
+    {
+        "DataSetIdentifierDeclarations": List[DataSetIdentifierDeclarationTypeDef],
+        "Sheets": NotRequired[List[SheetDefinitionOutputTypeDef]],
+        "CalculatedFields": NotRequired[List[CalculatedFieldTypeDef]],
+        "ParameterDeclarations": NotRequired[List[ParameterDeclarationOutputTypeDef]],
+        "FilterGroups": NotRequired[List[FilterGroupOutputTypeDef]],
+        "ColumnConfigurations": NotRequired[List[ColumnConfigurationOutputTypeDef]],
+        "AnalysisDefaults": NotRequired[AnalysisDefaultsTypeDef],
+        "Options": NotRequired[AssetOptionsTypeDef],
+    },
+)
+DashboardVersionDefinitionOutputTypeDef = TypedDict(
+    "DashboardVersionDefinitionOutputTypeDef",
+    {
+        "DataSetIdentifierDeclarations": List[DataSetIdentifierDeclarationTypeDef],
+        "Sheets": NotRequired[List[SheetDefinitionOutputTypeDef]],
+        "CalculatedFields": NotRequired[List[CalculatedFieldTypeDef]],
+        "ParameterDeclarations": NotRequired[List[ParameterDeclarationOutputTypeDef]],
+        "FilterGroups": NotRequired[List[FilterGroupOutputTypeDef]],
+        "ColumnConfigurations": NotRequired[List[ColumnConfigurationOutputTypeDef]],
+        "AnalysisDefaults": NotRequired[AnalysisDefaultsTypeDef],
+        "Options": NotRequired[AssetOptionsTypeDef],
+    },
+)
+TemplateVersionDefinitionOutputTypeDef = TypedDict(
+    "TemplateVersionDefinitionOutputTypeDef",
+    {
+        "DataSetConfigurations": List[DataSetConfigurationOutputTypeDef],
+        "Sheets": NotRequired[List[SheetDefinitionOutputTypeDef]],
+        "CalculatedFields": NotRequired[List[CalculatedFieldTypeDef]],
+        "ParameterDeclarations": NotRequired[List[ParameterDeclarationOutputTypeDef]],
+        "FilterGroups": NotRequired[List[FilterGroupOutputTypeDef]],
+        "ColumnConfigurations": NotRequired[List[ColumnConfigurationOutputTypeDef]],
+        "AnalysisDefaults": NotRequired[AnalysisDefaultsTypeDef],
+        "Options": NotRequired[AssetOptionsTypeDef],
+    },
+)
 AnalysisDefinitionTypeDef = TypedDict(
     "AnalysisDefinitionTypeDef",
     {
         "DataSetIdentifierDeclarations": Sequence[DataSetIdentifierDeclarationTypeDef],
         "Sheets": NotRequired[Sequence[SheetDefinitionTypeDef]],
         "CalculatedFields": NotRequired[Sequence[CalculatedFieldTypeDef]],
         "ParameterDeclarations": NotRequired[Sequence[ParameterDeclarationTypeDef]],
@@ -11412,44 +14830,74 @@
         "ParameterDeclarations": NotRequired[Sequence[ParameterDeclarationTypeDef]],
         "FilterGroups": NotRequired[Sequence[FilterGroupTypeDef]],
         "ColumnConfigurations": NotRequired[Sequence[ColumnConfigurationTypeDef]],
         "AnalysisDefaults": NotRequired[AnalysisDefaultsTypeDef],
         "Options": NotRequired[AssetOptionsTypeDef],
     },
 )
+DescribeAnalysisDefinitionResponseTypeDef = TypedDict(
+    "DescribeAnalysisDefinitionResponseTypeDef",
+    {
+        "AnalysisId": str,
+        "Name": str,
+        "Errors": List[AnalysisErrorTypeDef],
+        "ResourceStatus": ResourceStatusType,
+        "ThemeArn": str,
+        "Definition": AnalysisDefinitionOutputTypeDef,
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeDashboardDefinitionResponseTypeDef = TypedDict(
+    "DescribeDashboardDefinitionResponseTypeDef",
+    {
+        "DashboardId": str,
+        "Errors": List[DashboardErrorTypeDef],
+        "Name": str,
+        "ResourceStatus": ResourceStatusType,
+        "ThemeArn": str,
+        "Definition": DashboardVersionDefinitionOutputTypeDef,
+        "Status": int,
+        "RequestId": str,
+        "DashboardPublishOptions": DashboardPublishOptionsTypeDef,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+DescribeTemplateDefinitionResponseTypeDef = TypedDict(
+    "DescribeTemplateDefinitionResponseTypeDef",
+    {
+        "Name": str,
+        "TemplateId": str,
+        "Errors": List[TemplateErrorTypeDef],
+        "ResourceStatus": ResourceStatusType,
+        "ThemeArn": str,
+        "Definition": TemplateVersionDefinitionOutputTypeDef,
+        "Status": int,
+        "RequestId": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+AnalysisDefinitionUnionTypeDef = Union[AnalysisDefinitionTypeDef, AnalysisDefinitionOutputTypeDef]
 CreateAnalysisRequestRequestTypeDef = TypedDict(
     "CreateAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
         "Name": str,
         "Parameters": NotRequired[ParametersTypeDef],
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
+        "Permissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
         "SourceEntity": NotRequired[AnalysisSourceEntityTypeDef],
         "ThemeArn": NotRequired[str],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "Definition": NotRequired[AnalysisDefinitionTypeDef],
         "ValidationStrategy": NotRequired[ValidationStrategyTypeDef],
         "FolderArns": NotRequired[Sequence[str]],
     },
 )
-DescribeAnalysisDefinitionResponseTypeDef = TypedDict(
-    "DescribeAnalysisDefinitionResponseTypeDef",
-    {
-        "AnalysisId": str,
-        "Name": str,
-        "Errors": List[AnalysisErrorTypeDef],
-        "ResourceStatus": ResourceStatusType,
-        "ThemeArn": str,
-        "Definition": AnalysisDefinitionTypeDef,
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
 UpdateAnalysisRequestRequestTypeDef = TypedDict(
     "UpdateAnalysisRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "AnalysisId": str,
         "Name": str,
         "Parameters": NotRequired[ParametersTypeDef],
@@ -11462,42 +14910,30 @@
 CreateDashboardRequestRequestTypeDef = TypedDict(
     "CreateDashboardRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DashboardId": str,
         "Name": str,
         "Parameters": NotRequired[ParametersTypeDef],
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
+        "Permissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
         "SourceEntity": NotRequired[DashboardSourceEntityTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "VersionDescription": NotRequired[str],
         "DashboardPublishOptions": NotRequired[DashboardPublishOptionsTypeDef],
         "ThemeArn": NotRequired[str],
         "Definition": NotRequired[DashboardVersionDefinitionTypeDef],
         "ValidationStrategy": NotRequired[ValidationStrategyTypeDef],
         "FolderArns": NotRequired[Sequence[str]],
         "LinkSharingConfiguration": NotRequired[LinkSharingConfigurationTypeDef],
         "LinkEntities": NotRequired[Sequence[str]],
     },
 )
-DescribeDashboardDefinitionResponseTypeDef = TypedDict(
-    "DescribeDashboardDefinitionResponseTypeDef",
-    {
-        "DashboardId": str,
-        "Errors": List[DashboardErrorTypeDef],
-        "Name": str,
-        "ResourceStatus": ResourceStatusType,
-        "ThemeArn": str,
-        "Definition": DashboardVersionDefinitionTypeDef,
-        "Status": int,
-        "RequestId": str,
-        "DashboardPublishOptions": DashboardPublishOptionsTypeDef,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+DashboardVersionDefinitionUnionTypeDef = Union[
+    DashboardVersionDefinitionTypeDef, DashboardVersionDefinitionOutputTypeDef
+]
 UpdateDashboardRequestRequestTypeDef = TypedDict(
     "UpdateDashboardRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "DashboardId": str,
         "Name": str,
         "SourceEntity": NotRequired[DashboardSourceEntityTypeDef],
@@ -11511,36 +14947,25 @@
 )
 CreateTemplateRequestRequestTypeDef = TypedDict(
     "CreateTemplateRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TemplateId": str,
         "Name": NotRequired[str],
-        "Permissions": NotRequired[Sequence[ResourcePermissionTypeDef]],
+        "Permissions": NotRequired[Sequence[ResourcePermissionUnionTypeDef]],
         "SourceEntity": NotRequired[TemplateSourceEntityTypeDef],
         "Tags": NotRequired[Sequence[TagTypeDef]],
         "VersionDescription": NotRequired[str],
         "Definition": NotRequired[TemplateVersionDefinitionTypeDef],
         "ValidationStrategy": NotRequired[ValidationStrategyTypeDef],
     },
 )
-DescribeTemplateDefinitionResponseTypeDef = TypedDict(
-    "DescribeTemplateDefinitionResponseTypeDef",
-    {
-        "Name": str,
-        "TemplateId": str,
-        "Errors": List[TemplateErrorTypeDef],
-        "ResourceStatus": ResourceStatusType,
-        "ThemeArn": str,
-        "Definition": TemplateVersionDefinitionTypeDef,
-        "Status": int,
-        "RequestId": str,
-        "ResponseMetadata": ResponseMetadataTypeDef,
-    },
-)
+TemplateVersionDefinitionUnionTypeDef = Union[
+    TemplateVersionDefinitionTypeDef, TemplateVersionDefinitionOutputTypeDef
+]
 UpdateTemplateRequestRequestTypeDef = TypedDict(
     "UpdateTemplateRequestRequestTypeDef",
     {
         "AwsAccountId": str,
         "TemplateId": str,
         "SourceEntity": NotRequired[TemplateSourceEntityTypeDef],
         "VersionDescription": NotRequired[str],
```

### Comparing `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/PKG-INFO` & `mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-quicksight
-Version: 1.34.87
-Summary: Type annotations for boto3.QuickSight 1.34.87 service generated with mypy-boto3-builder 7.23.2
+Version: 1.34.95
+Summary: Type annotations for boto3.QuickSight 1.34.95 service generated with mypy-boto3-builder 7.24.0
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-quicksight.svg?color=blue)](https://pypi.org/project/mypy-boto3-quicksight)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-quicksight)](https://pepy.tech/project/mypy-boto3-quicksight)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.QuickSight 1.34.87](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
+[boto3.QuickSight 1.34.95](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/quicksight.html#QuickSight)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-quicksight docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_quicksight/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_quicksight-1.34.87/mypy_boto3_quicksight.egg-info/SOURCES.txt` & `mypy_boto3_quicksight-1.34.95/mypy_boto3_quicksight.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_quicksight-1.34.87/setup.py` & `mypy_boto3_quicksight-1.34.95/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-quicksight",
-    version="1.34.87",
+    version="1.34.95",
     packages=["mypy_boto3_quicksight"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.QuickSight 1.34.87 service generated with mypy-boto3-builder 7.23.2",
+    description="Type annotations for boto3.QuickSight 1.34.95 service generated with mypy-boto3-builder 7.24.0",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

