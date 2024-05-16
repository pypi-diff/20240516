# Comparing `tmp/mypy_boto3_kafka-1.34.107.tar.gz` & `tmp/mypy-boto3-kafka-1.34.61.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mypy_boto3_kafka-1.34.107.tar", last modified: Thu May 16 19:34:30 2024, max compression
+gzip compressed data, was "mypy-boto3-kafka-1.34.61.tar", last modified: Tue Mar 12 19:21:13 2024, max compression
```

## Comparing `mypy_boto3_kafka-1.34.107.tar` & `mypy-boto3-kafka-1.34.61.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:34:30.253037 mypy_boto3_kafka-1.34.107/
--rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-05-16 19:32:03.000000 mypy_boto3_kafka-1.34.107/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    14160 2024-05-16 19:34:30.253037 mypy_boto3_kafka-1.34.107/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12611 2024-05-16 19:32:03.000000 mypy_boto3_kafka-1.34.107/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:34:30.253037 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-16 19:32:03.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-05-16 19:32:03.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      914 2024-05-16 19:32:03.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    40155 2024-05-16 19:32:03.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/client.py
--rw-r--r--   0 runner    (1001) docker     (127)    40152 2024-05-16 19:32:03.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/client.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    12100 2024-05-16 19:32:04.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/literals.py
--rw-r--r--   0 runner    (1001) docker     (127)    12100 2024-05-16 19:32:04.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/literals.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    13629 2024-05-16 19:32:03.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/paginator.py
--rw-r--r--   0 runner    (1001) docker     (127)    13616 2024-05-16 19:32:03.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/paginator.pyi
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-05-16 19:32:03.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    62926 2024-05-16 19:32:05.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/type_defs.py
--rw-r--r--   0 runner    (1001) docker     (127)    62926 2024-05-16 19:32:04.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/type_defs.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-05-16 19:32:03.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-05-16 19:34:30.253037 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14160 2024-05-16 19:34:30.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-05-16 19:34:30.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:34:30.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-05-16 19:34:30.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       53 2024-05-16 19:34:30.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       17 2024-05-16 19:34:30.000000 mypy_boto3_kafka-1.34.107/mypy_boto3_kafka.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-05-16 19:34:30.253037 mypy_boto3_kafka-1.34.107/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1962 2024-05-16 19:32:03.000000 mypy_boto3_kafka-1.34.107/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:21:13.571051 mypy-boto3-kafka-1.34.61/
+-rw-r--r--   0 runner    (1001) docker     (127)     1070 2024-03-12 19:20:51.000000 mypy-boto3-kafka-1.34.61/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-03-12 19:21:13.571051 mypy-boto3-kafka-1.34.61/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12610 2024-03-12 19:20:51.000000 mypy-boto3-kafka-1.34.61/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:21:13.571051 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-03-12 19:20:51.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2966 2024-03-12 19:20:51.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      911 2024-03-12 19:20:51.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40130 2024-03-12 19:20:51.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)    40127 2024-03-12 19:20:51.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/client.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-03-12 19:20:51.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/literals.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11994 2024-03-12 19:20:51.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/literals.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    13683 2024-03-12 19:20:51.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/paginator.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13670 2024-03-12 19:20:51.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/paginator.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-12 19:20:51.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    65667 2024-03-12 19:20:52.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/type_defs.py
+-rw-r--r--   0 runner    (1001) docker     (127)    65667 2024-03-12 19:20:52.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/type_defs.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-03-12 19:20:51.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-12 19:21:13.571051 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14157 2024-03-12 19:21:13.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-03-12 19:21:13.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 19:21:13.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-12 19:21:13.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       53 2024-03-12 19:21:13.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       17 2024-03-12 19:21:13.000000 mypy-boto3-kafka-1.34.61/mypy_boto3_kafka.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-12 19:21:13.571051 mypy-boto3-kafka-1.34.61/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1960 2024-03-12 19:20:51.000000 mypy-boto3-kafka-1.34.61/setup.py
```

### Comparing `mypy_boto3_kafka-1.34.107/LICENSE` & `mypy-boto3-kafka-1.34.61/LICENSE`

 * *Files identical despite different names*

### Comparing `mypy_boto3_kafka-1.34.107/PKG-INFO` & `mypy-boto3-kafka-1.34.61/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kafka
-Version: 1.34.107
-Summary: Type annotations for boto3.Kafka 1.34.107 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.61
+Summary: Type annotations for boto3.Kafka 1.34.61 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafka)](https://pepy.tech/project/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.34.107](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.34.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_kafka-1.34.107/README.md` & `mypy-boto3-kafka-1.34.61/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -6,24 +6,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafka)](https://pepy.tech/project/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.34.107](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.34.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/__init__.py` & `mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/__init__.py`

 * *Files identical despite different names*

### Comparing `mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/__init__.pyi` & `mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/__init__.pyi`

 * *Files identical despite different names*

### Comparing `mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/__main__.py` & `mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/__main__.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,29 +6,29 @@
 
 
 def print_info() -> None:
     """
     Print package info to stdout.
     """
     print(
-        "Type annotations for boto3.Kafka 1.34.107\n"
-        "Version:         1.34.107\n"
-        "Builder version: 7.24.0\n"
+        "Type annotations for boto3.Kafka 1.34.61\n"
+        "Version:         1.34.61\n"
+        "Builder version: 7.23.2\n"
         "Docs:            https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka//\n"
         "Boto3 docs:      https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka\n"
         "Other services:  https://pypi.org/project/boto3-stubs/\n"
         "Changelog:       https://github.com/youtype/mypy_boto3_builder/releases"
     )
 
 
 def print_version() -> None:
     """
     Print package version to stdout.
     """
-    print("1.34.107")
+    print("1.34.61")
 
 
 def main() -> None:
     """
     Main CLI entrypoint.
     """
     if "--version" in sys.argv:
```

### Comparing `mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/client.py` & `mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/client.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     ListVpcConnectionsPaginator,
 )
 from .type_defs import (
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BlobTypeDef,
     BrokerEBSVolumeInfoTypeDef,
-    BrokerNodeGroupInfoUnionTypeDef,
-    ClientAuthenticationUnionTypeDef,
+    BrokerNodeGroupInfoTypeDef,
+    ClientAuthenticationTypeDef,
     ConfigurationInfoTypeDef,
     ConnectivityInfoTypeDef,
     ConsumerGroupReplicationUpdateTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationResponseTypeDef,
     CreateReplicatorResponseTypeDef,
@@ -182,19 +182,19 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#close)
         """
 
     def create_cluster(
         self,
         *,
-        BrokerNodeGroupInfo: BrokerNodeGroupInfoUnionTypeDef,
+        BrokerNodeGroupInfo: BrokerNodeGroupInfoTypeDef,
         ClusterName: str,
         KafkaVersion: str,
         NumberOfBrokerNodes: int,
-        ClientAuthentication: ClientAuthenticationUnionTypeDef = ...,
+        ClientAuthentication: ClientAuthenticationTypeDef = ...,
         ConfigurationInfo: ConfigurationInfoTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...,
         EnhancedMonitoring: EnhancedMonitoringType = ...,
         OpenMonitoring: OpenMonitoringInfoTypeDef = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         StorageMode: StorageModeType = ...,
@@ -735,15 +735,15 @@
         """
 
     def update_security(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
-        ClientAuthentication: ClientAuthenticationUnionTypeDef = ...,
+        ClientAuthentication: ClientAuthenticationTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...,
     ) -> UpdateSecurityResponseTypeDef:
         """
         Updates the security settings for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_security)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_security)
```

### Comparing `mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/client.pyi` & `mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/client.pyi`

 * *Files 0% similar despite different names*

```diff
@@ -35,16 +35,16 @@
     ListVpcConnectionsPaginator,
 )
 from .type_defs import (
     BatchAssociateScramSecretResponseTypeDef,
     BatchDisassociateScramSecretResponseTypeDef,
     BlobTypeDef,
     BrokerEBSVolumeInfoTypeDef,
-    BrokerNodeGroupInfoUnionTypeDef,
-    ClientAuthenticationUnionTypeDef,
+    BrokerNodeGroupInfoTypeDef,
+    ClientAuthenticationTypeDef,
     ConfigurationInfoTypeDef,
     ConnectivityInfoTypeDef,
     ConsumerGroupReplicationUpdateTypeDef,
     CreateClusterResponseTypeDef,
     CreateClusterV2ResponseTypeDef,
     CreateConfigurationResponseTypeDef,
     CreateReplicatorResponseTypeDef,
@@ -179,19 +179,19 @@
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.close)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#close)
         """
 
     def create_cluster(
         self,
         *,
-        BrokerNodeGroupInfo: BrokerNodeGroupInfoUnionTypeDef,
+        BrokerNodeGroupInfo: BrokerNodeGroupInfoTypeDef,
         ClusterName: str,
         KafkaVersion: str,
         NumberOfBrokerNodes: int,
-        ClientAuthentication: ClientAuthenticationUnionTypeDef = ...,
+        ClientAuthentication: ClientAuthenticationTypeDef = ...,
         ConfigurationInfo: ConfigurationInfoTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...,
         EnhancedMonitoring: EnhancedMonitoringType = ...,
         OpenMonitoring: OpenMonitoringInfoTypeDef = ...,
         LoggingInfo: LoggingInfoTypeDef = ...,
         Tags: Mapping[str, str] = ...,
         StorageMode: StorageModeType = ...,
@@ -732,15 +732,15 @@
         """
 
     def update_security(
         self,
         *,
         ClusterArn: str,
         CurrentVersion: str,
-        ClientAuthentication: ClientAuthenticationUnionTypeDef = ...,
+        ClientAuthentication: ClientAuthenticationTypeDef = ...,
         EncryptionInfo: EncryptionInfoTypeDef = ...,
     ) -> UpdateSecurityResponseTypeDef:
         """
         Updates the security settings for the cluster.
 
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Client.update_security)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/client/#update_security)
```

### Comparing `mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/literals.py` & `mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/literals.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,14 @@
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
@@ -190,26 +189,24 @@
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
@@ -270,14 +267,15 @@
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
@@ -406,15 +404,14 @@
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
@@ -458,15 +455,14 @@
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
@@ -522,15 +518,14 @@
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

### Comparing `mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/literals.pyi` & `mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/literals.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -169,15 +169,14 @@
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
@@ -190,26 +189,24 @@
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
@@ -270,14 +267,15 @@
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
@@ -406,15 +404,14 @@
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
@@ -458,15 +455,14 @@
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
@@ -522,15 +518,14 @@
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

### Comparing `mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/paginator.py` & `mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/paginator.py`

 * *Files 1% similar despite different names*

```diff
@@ -44,18 +44,18 @@
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ListClientVpcConnectionsResponseTypeDef,
-    ListClusterOperationsResponseTypeDef,
+    ListClusterOperationsResponsePaginatorTypeDef,
     ListClusterOperationsV2ResponseTypeDef,
-    ListClustersResponseTypeDef,
-    ListClustersV2ResponseTypeDef,
+    ListClustersResponsePaginatorTypeDef,
+    ListClustersV2ResponsePaginatorTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListReplicatorsResponseTypeDef,
     ListScramSecretsResponseTypeDef,
     ListVpcConnectionsResponseTypeDef,
@@ -106,15 +106,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationspaginator)
     """
 
     def paginate(
         self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListClusterOperationsResponseTypeDef]:
+    ) -> _PageIterator[ListClusterOperationsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationspaginator)
         """
 
 
 class ListClusterOperationsV2Paginator(Paginator):
@@ -136,15 +136,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusterspaginator)
     """
 
     def paginate(
         self, *, ClusterNameFilter: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListClustersResponseTypeDef]:
+    ) -> _PageIterator[ListClustersResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusterspaginator)
         """
 
 
 class ListClustersV2Paginator(Paginator):
@@ -155,15 +155,15 @@
 
     def paginate(
         self,
         *,
         ClusterNameFilter: str = ...,
         ClusterTypeFilter: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListClustersV2ResponseTypeDef]:
+    ) -> _PageIterator[ListClustersV2ResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClustersV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclustersv2paginator)
         """
 
 
 class ListConfigurationRevisionsPaginator(Paginator):
```

### Comparing `mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/paginator.pyi` & `mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/paginator.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -44,18 +44,18 @@
 
 from typing import Generic, Iterator, TypeVar
 
 from botocore.paginate import PageIterator, Paginator
 
 from .type_defs import (
     ListClientVpcConnectionsResponseTypeDef,
-    ListClusterOperationsResponseTypeDef,
+    ListClusterOperationsResponsePaginatorTypeDef,
     ListClusterOperationsV2ResponseTypeDef,
-    ListClustersResponseTypeDef,
-    ListClustersV2ResponseTypeDef,
+    ListClustersResponsePaginatorTypeDef,
+    ListClustersV2ResponsePaginatorTypeDef,
     ListConfigurationRevisionsResponseTypeDef,
     ListConfigurationsResponseTypeDef,
     ListKafkaVersionsResponseTypeDef,
     ListNodesResponseTypeDef,
     ListReplicatorsResponseTypeDef,
     ListScramSecretsResponseTypeDef,
     ListVpcConnectionsResponseTypeDef,
@@ -103,15 +103,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationspaginator)
     """
 
     def paginate(
         self, *, ClusterArn: str, PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListClusterOperationsResponseTypeDef]:
+    ) -> _PageIterator[ListClusterOperationsResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusterOperations.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusteroperationspaginator)
         """
 
 class ListClusterOperationsV2Paginator(Paginator):
     """
@@ -131,15 +131,15 @@
     """
     [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters)
     [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusterspaginator)
     """
 
     def paginate(
         self, *, ClusterNameFilter: str = ..., PaginationConfig: PaginatorConfigTypeDef = ...
-    ) -> _PageIterator[ListClustersResponseTypeDef]:
+    ) -> _PageIterator[ListClustersResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClusters.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclusterspaginator)
         """
 
 class ListClustersV2Paginator(Paginator):
     """
@@ -149,15 +149,15 @@
 
     def paginate(
         self,
         *,
         ClusterNameFilter: str = ...,
         ClusterTypeFilter: str = ...,
         PaginationConfig: PaginatorConfigTypeDef = ...,
-    ) -> _PageIterator[ListClustersV2ResponseTypeDef]:
+    ) -> _PageIterator[ListClustersV2ResponsePaginatorTypeDef]:
         """
         [Show boto3 documentation](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka.Paginator.ListClustersV2.paginate)
         [Show boto3-stubs documentation](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/paginators/#listclustersv2paginator)
         """
 
 class ListConfigurationRevisionsPaginator(Paginator):
     """
```

### Comparing `mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/type_defs.py` & `mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/type_defs.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,34 +50,31 @@
 __all__ = (
     "AmazonMskClusterTypeDef",
     "BatchAssociateScramSecretRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UnprocessedScramSecretTypeDef",
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     "BlobTypeDef",
-    "BrokerCountUpdateInfoTypeDef",
     "ProvisionedThroughputTypeDef",
     "CloudWatchLogsTypeDef",
     "FirehoseTypeDef",
     "S3TypeDef",
     "BrokerSoftwareInfoTypeDef",
-    "TlsExtraOutputTypeDef",
+    "TlsPaginatorTypeDef",
     "UnauthenticatedTypeDef",
-    "TlsOutputTypeDef",
     "TlsTypeDef",
     "ClientVpcConnectionTypeDef",
     "StateInfoTypeDef",
     "ErrorInfoTypeDef",
     "ClusterOperationStepInfoTypeDef",
     "ClusterOperationV2SummaryTypeDef",
     "CompatibleKafkaVersionTypeDef",
     "ConfigurationInfoTypeDef",
     "ConfigurationRevisionTypeDef",
     "PublicAccessTypeDef",
-    "ConsumerGroupReplicationOutputTypeDef",
     "ConsumerGroupReplicationTypeDef",
     "ConsumerGroupReplicationUpdateTypeDef",
     "CreateVpcConnectionRequestRequestTypeDef",
     "DeleteClusterPolicyRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteConfigurationRequestRequestTypeDef",
     "DeleteReplicatorRequestRequestTypeDef",
@@ -95,15 +92,14 @@
     "EncryptionInTransitTypeDef",
     "GetBootstrapBrokersRequestRequestTypeDef",
     "GetClusterPolicyRequestRequestTypeDef",
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
     "IamTypeDef",
     "JmxExporterInfoTypeDef",
     "JmxExporterTypeDef",
-    "KafkaClusterClientVpcConfigOutputTypeDef",
     "KafkaClusterClientVpcConfigTypeDef",
     "KafkaVersionTypeDef",
     "PaginatorConfigTypeDef",
     "ListClientVpcConnectionsRequestRequestTypeDef",
     "ListClusterOperationsRequestRequestTypeDef",
     "ListClusterOperationsV2RequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
@@ -122,16 +118,16 @@
     "ZookeeperNodeInfoTypeDef",
     "PutClusterPolicyRequestRequestTypeDef",
     "RebootBrokerRequestRequestTypeDef",
     "RejectClientVpcConnectionRequestRequestTypeDef",
     "ReplicationInfoSummaryTypeDef",
     "ReplicationStartingPositionTypeDef",
     "ScramTypeDef",
+    "VpcConfigPaginatorTypeDef",
     "VpcConfigTypeDef",
-    "VpcConfigOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TopicReplicationUpdateTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrokerCountRequestRequestTypeDef",
     "UpdateBrokerTypeRequestRequestTypeDef",
     "UserIdentityTypeDef",
     "VpcConnectivityTlsTypeDef",
@@ -201,15 +197,14 @@
     "ListNodesRequestListNodesPaginateTypeDef",
     "ListReplicatorsRequestListReplicatorsPaginateTypeDef",
     "ListScramSecretsRequestListScramSecretsPaginateTypeDef",
     "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
     "ListVpcConnectionsResponseTypeDef",
     "PrometheusInfoTypeDef",
     "PrometheusTypeDef",
-    "TopicReplicationOutputTypeDef",
     "TopicReplicationTypeDef",
     "SaslTypeDef",
     "UpdateReplicationInfoRequestRequestTypeDef",
     "VpcConnectionInfoServerlessTypeDef",
     "VpcConnectionInfoTypeDef",
     "VpcConnectivitySaslTypeDef",
     "ReplicatorSummaryTypeDef",
@@ -219,49 +214,54 @@
     "NodeInfoTypeDef",
     "ListConfigurationsResponseTypeDef",
     "ServerlessClientAuthenticationTypeDef",
     "OpenMonitoringInfoTypeDef",
     "OpenMonitoringTypeDef",
     "ReplicationInfoDescriptionTypeDef",
     "ReplicationInfoTypeDef",
-    "ClientAuthenticationExtraOutputTypeDef",
-    "ClientAuthenticationOutputTypeDef",
+    "ClientAuthenticationPaginatorTypeDef",
     "ClientAuthenticationTypeDef",
     "ClusterOperationV2ServerlessTypeDef",
     "VpcConnectivityClientAuthenticationTypeDef",
     "ListReplicatorsResponseTypeDef",
     "ListNodesResponseTypeDef",
+    "ServerlessPaginatorTypeDef",
     "ServerlessRequestTypeDef",
     "ServerlessTypeDef",
     "UpdateMonitoringRequestRequestTypeDef",
     "DescribeReplicatorResponseTypeDef",
     "CreateReplicatorRequestRequestTypeDef",
-    "ClientAuthenticationUnionTypeDef",
     "UpdateSecurityRequestRequestTypeDef",
     "VpcConnectivityTypeDef",
     "ConnectivityInfoTypeDef",
-    "BrokerNodeGroupInfoExtraOutputTypeDef",
-    "BrokerNodeGroupInfoOutputTypeDef",
+    "BrokerNodeGroupInfoPaginatorTypeDef",
     "BrokerNodeGroupInfoTypeDef",
+    "MutableClusterInfoPaginatorTypeDef",
     "MutableClusterInfoTypeDef",
     "UpdateConnectivityRequestRequestTypeDef",
+    "ClusterInfoPaginatorTypeDef",
+    "ProvisionedPaginatorTypeDef",
     "ClusterInfoTypeDef",
-    "ProvisionedTypeDef",
-    "BrokerNodeGroupInfoUnionTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ProvisionedRequestTypeDef",
+    "ProvisionedTypeDef",
+    "ClusterOperationInfoPaginatorTypeDef",
     "ClusterOperationInfoTypeDef",
     "ClusterOperationV2ProvisionedTypeDef",
+    "ListClustersResponsePaginatorTypeDef",
+    "ClusterPaginatorTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
-    "ClusterTypeDef",
     "CreateClusterV2RequestRequestTypeDef",
+    "ClusterTypeDef",
+    "ListClusterOperationsResponsePaginatorTypeDef",
     "DescribeClusterOperationResponseTypeDef",
     "ListClusterOperationsResponseTypeDef",
     "ClusterOperationV2TypeDef",
+    "ListClustersV2ResponsePaginatorTypeDef",
     "DescribeClusterV2ResponseTypeDef",
     "ListClustersV2ResponseTypeDef",
     "DescribeClusterOperationV2ResponseTypeDef",
 )
 
 AmazonMskClusterTypeDef = TypedDict(
     "AmazonMskClusterTypeDef",
@@ -298,21 +298,14 @@
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "SecretArnList": Sequence[str],
     },
 )
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
-BrokerCountUpdateInfoTypeDef = TypedDict(
-    "BrokerCountUpdateInfoTypeDef",
-    {
-        "CreatedBrokerIds": NotRequired[List[float]],
-        "DeletedBrokerIds": NotRequired[List[float]],
-    },
-)
 ProvisionedThroughputTypeDef = TypedDict(
     "ProvisionedThroughputTypeDef",
     {
         "Enabled": NotRequired[bool],
         "VolumeThroughput": NotRequired[int],
     },
 )
@@ -342,34 +335,27 @@
     "BrokerSoftwareInfoTypeDef",
     {
         "ConfigurationArn": NotRequired[str],
         "ConfigurationRevision": NotRequired[int],
         "KafkaVersion": NotRequired[str],
     },
 )
-TlsExtraOutputTypeDef = TypedDict(
-    "TlsExtraOutputTypeDef",
+TlsPaginatorTypeDef = TypedDict(
+    "TlsPaginatorTypeDef",
     {
         "CertificateAuthorityArnList": NotRequired[List[str]],
         "Enabled": NotRequired[bool],
     },
 )
 UnauthenticatedTypeDef = TypedDict(
     "UnauthenticatedTypeDef",
     {
         "Enabled": NotRequired[bool],
     },
 )
-TlsOutputTypeDef = TypedDict(
-    "TlsOutputTypeDef",
-    {
-        "CertificateAuthorityArnList": NotRequired[List[str]],
-        "Enabled": NotRequired[bool],
-    },
-)
 TlsTypeDef = TypedDict(
     "TlsTypeDef",
     {
         "CertificateAuthorityArnList": NotRequired[Sequence[str]],
         "Enabled": NotRequired[bool],
     },
 )
@@ -439,23 +425,14 @@
 )
 PublicAccessTypeDef = TypedDict(
     "PublicAccessTypeDef",
     {
         "Type": NotRequired[str],
     },
 )
-ConsumerGroupReplicationOutputTypeDef = TypedDict(
-    "ConsumerGroupReplicationOutputTypeDef",
-    {
-        "ConsumerGroupsToReplicate": List[str],
-        "ConsumerGroupsToExclude": NotRequired[List[str]],
-        "DetectAndCopyNewConsumerGroups": NotRequired[bool],
-        "SynchroniseConsumerGroupOffsets": NotRequired[bool],
-    },
-)
 ConsumerGroupReplicationTypeDef = TypedDict(
     "ConsumerGroupReplicationTypeDef",
     {
         "ConsumerGroupsToReplicate": Sequence[str],
         "ConsumerGroupsToExclude": NotRequired[Sequence[str]],
         "DetectAndCopyNewConsumerGroups": NotRequired[bool],
         "SynchroniseConsumerGroupOffsets": NotRequired[bool],
@@ -614,21 +591,14 @@
 )
 JmxExporterTypeDef = TypedDict(
     "JmxExporterTypeDef",
     {
         "EnabledInBroker": bool,
     },
 )
-KafkaClusterClientVpcConfigOutputTypeDef = TypedDict(
-    "KafkaClusterClientVpcConfigOutputTypeDef",
-    {
-        "SubnetIds": List[str],
-        "SecurityGroupIds": NotRequired[List[str]],
-    },
-)
 KafkaClusterClientVpcConfigTypeDef = TypedDict(
     "KafkaClusterClientVpcConfigTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": NotRequired[Sequence[str]],
     },
 )
@@ -817,28 +787,28 @@
 )
 ScramTypeDef = TypedDict(
     "ScramTypeDef",
     {
         "Enabled": NotRequired[bool],
     },
 )
+VpcConfigPaginatorTypeDef = TypedDict(
+    "VpcConfigPaginatorTypeDef",
+    {
+        "SubnetIds": List[str],
+        "SecurityGroupIds": NotRequired[List[str]],
+    },
+)
 VpcConfigTypeDef = TypedDict(
     "VpcConfigTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": NotRequired[Sequence[str]],
     },
 )
-VpcConfigOutputTypeDef = TypedDict(
-    "VpcConfigOutputTypeDef",
-    {
-        "SubnetIds": List[str],
-        "SecurityGroupIds": NotRequired[List[str]],
-    },
-)
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1036,17 +1006,17 @@
         "Policy": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListScramSecretsResponseTypeDef = TypedDict(
     "ListScramSecretsResponseTypeDef",
     {
+        "NextToken": str,
         "SecretArnList": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1224,31 +1194,31 @@
         "Endpoints": NotRequired[List[str]],
     },
 )
 ListClientVpcConnectionsResponseTypeDef = TypedDict(
     "ListClientVpcConnectionsResponseTypeDef",
     {
         "ClientVpcConnections": List[ClientVpcConnectionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ClusterOperationStepTypeDef = TypedDict(
     "ClusterOperationStepTypeDef",
     {
         "StepInfo": NotRequired[ClusterOperationStepInfoTypeDef],
         "StepName": NotRequired[str],
     },
 )
 ListClusterOperationsV2ResponseTypeDef = TypedDict(
     "ListClusterOperationsV2ResponseTypeDef",
     {
         "ClusterOperationInfoList": List[ClusterOperationV2SummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 GetCompatibleKafkaVersionsResponseTypeDef = TypedDict(
     "GetCompatibleKafkaVersionsResponseTypeDef",
     {
         "CompatibleKafkaVersions": List[CompatibleKafkaVersionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1306,17 +1276,17 @@
         "State": ConfigurationStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListConfigurationRevisionsResponseTypeDef = TypedDict(
     "ListConfigurationRevisionsResponseTypeDef",
     {
+        "NextToken": str,
         "Revisions": List[ConfigurationRevisionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 UpdateConfigurationResponseTypeDef = TypedDict(
     "UpdateConfigurationResponseTypeDef",
     {
         "Arn": str,
         "LatestRevision": ConfigurationRevisionTypeDef,
@@ -1337,30 +1307,30 @@
     },
 )
 KafkaClusterDescriptionTypeDef = TypedDict(
     "KafkaClusterDescriptionTypeDef",
     {
         "AmazonMskCluster": NotRequired[AmazonMskClusterTypeDef],
         "KafkaClusterAlias": NotRequired[str],
-        "VpcConfig": NotRequired[KafkaClusterClientVpcConfigOutputTypeDef],
+        "VpcConfig": NotRequired[KafkaClusterClientVpcConfigTypeDef],
     },
 )
 KafkaClusterTypeDef = TypedDict(
     "KafkaClusterTypeDef",
     {
         "AmazonMskCluster": AmazonMskClusterTypeDef,
         "VpcConfig": KafkaClusterClientVpcConfigTypeDef,
     },
 )
 ListKafkaVersionsResponseTypeDef = TypedDict(
     "ListKafkaVersionsResponseTypeDef",
     {
         "KafkaVersions": List[KafkaVersionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
     "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
     {
         "ClusterArn": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -1441,16 +1411,16 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListVpcConnectionsResponseTypeDef = TypedDict(
     "ListVpcConnectionsResponseTypeDef",
     {
         "VpcConnections": List[VpcConnectionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 PrometheusInfoTypeDef = TypedDict(
     "PrometheusInfoTypeDef",
     {
         "JmxExporter": NotRequired[JmxExporterInfoTypeDef],
         "NodeExporter": NotRequired[NodeExporterInfoTypeDef],
@@ -1459,25 +1429,14 @@
 PrometheusTypeDef = TypedDict(
     "PrometheusTypeDef",
     {
         "JmxExporter": NotRequired[JmxExporterTypeDef],
         "NodeExporter": NotRequired[NodeExporterTypeDef],
     },
 )
-TopicReplicationOutputTypeDef = TypedDict(
-    "TopicReplicationOutputTypeDef",
-    {
-        "TopicsToReplicate": List[str],
-        "CopyAccessControlListsForTopics": NotRequired[bool],
-        "CopyTopicConfigurations": NotRequired[bool],
-        "DetectAndCopyNewTopics": NotRequired[bool],
-        "StartingPosition": NotRequired[ReplicationStartingPositionTypeDef],
-        "TopicsToExclude": NotRequired[List[str]],
-    },
-)
 TopicReplicationTypeDef = TypedDict(
     "TopicReplicationTypeDef",
     {
         "TopicsToReplicate": Sequence[str],
         "CopyAccessControlListsForTopics": NotRequired[bool],
         "CopyTopicConfigurations": NotRequired[bool],
         "DetectAndCopyNewTopics": NotRequired[bool],
@@ -1573,16 +1532,16 @@
         "ZookeeperNodeInfo": NotRequired[ZookeeperNodeInfoTypeDef],
     },
 )
 ListConfigurationsResponseTypeDef = TypedDict(
     "ListConfigurationsResponseTypeDef",
     {
         "Configurations": List[ConfigurationTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ServerlessClientAuthenticationTypeDef = TypedDict(
     "ServerlessClientAuthenticationTypeDef",
     {
         "Sasl": NotRequired[ServerlessSaslTypeDef],
     },
@@ -1598,44 +1557,36 @@
     {
         "Prometheus": PrometheusTypeDef,
     },
 )
 ReplicationInfoDescriptionTypeDef = TypedDict(
     "ReplicationInfoDescriptionTypeDef",
     {
-        "ConsumerGroupReplication": NotRequired[ConsumerGroupReplicationOutputTypeDef],
+        "ConsumerGroupReplication": NotRequired[ConsumerGroupReplicationTypeDef],
         "SourceKafkaClusterAlias": NotRequired[str],
         "TargetCompressionType": NotRequired[TargetCompressionTypeType],
         "TargetKafkaClusterAlias": NotRequired[str],
-        "TopicReplication": NotRequired[TopicReplicationOutputTypeDef],
+        "TopicReplication": NotRequired[TopicReplicationTypeDef],
     },
 )
 ReplicationInfoTypeDef = TypedDict(
     "ReplicationInfoTypeDef",
     {
         "ConsumerGroupReplication": ConsumerGroupReplicationTypeDef,
         "SourceKafkaClusterArn": str,
         "TargetCompressionType": TargetCompressionTypeType,
         "TargetKafkaClusterArn": str,
         "TopicReplication": TopicReplicationTypeDef,
     },
 )
-ClientAuthenticationExtraOutputTypeDef = TypedDict(
-    "ClientAuthenticationExtraOutputTypeDef",
-    {
-        "Sasl": NotRequired[SaslTypeDef],
-        "Tls": NotRequired[TlsExtraOutputTypeDef],
-        "Unauthenticated": NotRequired[UnauthenticatedTypeDef],
-    },
-)
-ClientAuthenticationOutputTypeDef = TypedDict(
-    "ClientAuthenticationOutputTypeDef",
+ClientAuthenticationPaginatorTypeDef = TypedDict(
+    "ClientAuthenticationPaginatorTypeDef",
     {
         "Sasl": NotRequired[SaslTypeDef],
-        "Tls": NotRequired[TlsOutputTypeDef],
+        "Tls": NotRequired[TlsPaginatorTypeDef],
         "Unauthenticated": NotRequired[UnauthenticatedTypeDef],
     },
 )
 ClientAuthenticationTypeDef = TypedDict(
     "ClientAuthenticationTypeDef",
     {
         "Sasl": NotRequired[SaslTypeDef],
@@ -1655,38 +1606,45 @@
         "Sasl": NotRequired[VpcConnectivitySaslTypeDef],
         "Tls": NotRequired[VpcConnectivityTlsTypeDef],
     },
 )
 ListReplicatorsResponseTypeDef = TypedDict(
     "ListReplicatorsResponseTypeDef",
     {
+        "NextToken": str,
         "Replicators": List[ReplicatorSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListNodesResponseTypeDef = TypedDict(
     "ListNodesResponseTypeDef",
     {
+        "NextToken": str,
         "NodeInfoList": List[NodeInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
+    },
+)
+ServerlessPaginatorTypeDef = TypedDict(
+    "ServerlessPaginatorTypeDef",
+    {
+        "VpcConfigs": List[VpcConfigPaginatorTypeDef],
+        "ClientAuthentication": NotRequired[ServerlessClientAuthenticationTypeDef],
     },
 )
 ServerlessRequestTypeDef = TypedDict(
     "ServerlessRequestTypeDef",
     {
         "VpcConfigs": Sequence[VpcConfigTypeDef],
         "ClientAuthentication": NotRequired[ServerlessClientAuthenticationTypeDef],
     },
 )
 ServerlessTypeDef = TypedDict(
     "ServerlessTypeDef",
     {
-        "VpcConfigs": List[VpcConfigOutputTypeDef],
+        "VpcConfigs": List[VpcConfigTypeDef],
         "ClientAuthentication": NotRequired[ServerlessClientAuthenticationTypeDef],
     },
 )
 UpdateMonitoringRequestRequestTypeDef = TypedDict(
     "UpdateMonitoringRequestRequestTypeDef",
     {
         "ClusterArn": str,
@@ -1722,17 +1680,14 @@
         "ReplicationInfoList": Sequence[ReplicationInfoTypeDef],
         "ReplicatorName": str,
         "ServiceExecutionRoleArn": str,
         "Description": NotRequired[str],
         "Tags": NotRequired[Mapping[str, str]],
     },
 )
-ClientAuthenticationUnionTypeDef = Union[
-    ClientAuthenticationTypeDef, ClientAuthenticationExtraOutputTypeDef
-]
 UpdateSecurityRequestRequestTypeDef = TypedDict(
     "UpdateSecurityRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
         "ClientAuthentication": NotRequired[ClientAuthenticationTypeDef],
         "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
@@ -1747,28 +1702,16 @@
 ConnectivityInfoTypeDef = TypedDict(
     "ConnectivityInfoTypeDef",
     {
         "PublicAccess": NotRequired[PublicAccessTypeDef],
         "VpcConnectivity": NotRequired[VpcConnectivityTypeDef],
     },
 )
-BrokerNodeGroupInfoExtraOutputTypeDef = TypedDict(
-    "BrokerNodeGroupInfoExtraOutputTypeDef",
-    {
-        "ClientSubnets": List[str],
-        "InstanceType": str,
-        "BrokerAZDistribution": NotRequired[Literal["DEFAULT"]],
-        "SecurityGroups": NotRequired[List[str]],
-        "StorageInfo": NotRequired[StorageInfoTypeDef],
-        "ConnectivityInfo": NotRequired[ConnectivityInfoTypeDef],
-        "ZoneIds": NotRequired[List[str]],
-    },
-)
-BrokerNodeGroupInfoOutputTypeDef = TypedDict(
-    "BrokerNodeGroupInfoOutputTypeDef",
+BrokerNodeGroupInfoPaginatorTypeDef = TypedDict(
+    "BrokerNodeGroupInfoPaginatorTypeDef",
     {
         "ClientSubnets": List[str],
         "InstanceType": str,
         "BrokerAZDistribution": NotRequired[Literal["DEFAULT"]],
         "SecurityGroups": NotRequired[List[str]],
         "StorageInfo": NotRequired[StorageInfoTypeDef],
         "ConnectivityInfo": NotRequired[ConnectivityInfoTypeDef],
@@ -1783,46 +1726,62 @@
         "BrokerAZDistribution": NotRequired[Literal["DEFAULT"]],
         "SecurityGroups": NotRequired[Sequence[str]],
         "StorageInfo": NotRequired[StorageInfoTypeDef],
         "ConnectivityInfo": NotRequired[ConnectivityInfoTypeDef],
         "ZoneIds": NotRequired[Sequence[str]],
     },
 )
+MutableClusterInfoPaginatorTypeDef = TypedDict(
+    "MutableClusterInfoPaginatorTypeDef",
+    {
+        "BrokerEBSVolumeInfo": NotRequired[List[BrokerEBSVolumeInfoTypeDef]],
+        "ConfigurationInfo": NotRequired[ConfigurationInfoTypeDef],
+        "NumberOfBrokerNodes": NotRequired[int],
+        "EnhancedMonitoring": NotRequired[EnhancedMonitoringType],
+        "OpenMonitoring": NotRequired[OpenMonitoringTypeDef],
+        "KafkaVersion": NotRequired[str],
+        "LoggingInfo": NotRequired[LoggingInfoTypeDef],
+        "InstanceType": NotRequired[str],
+        "ClientAuthentication": NotRequired[ClientAuthenticationPaginatorTypeDef],
+        "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
+        "ConnectivityInfo": NotRequired[ConnectivityInfoTypeDef],
+        "StorageMode": NotRequired[StorageModeType],
+    },
+)
 MutableClusterInfoTypeDef = TypedDict(
     "MutableClusterInfoTypeDef",
     {
         "BrokerEBSVolumeInfo": NotRequired[List[BrokerEBSVolumeInfoTypeDef]],
         "ConfigurationInfo": NotRequired[ConfigurationInfoTypeDef],
         "NumberOfBrokerNodes": NotRequired[int],
         "EnhancedMonitoring": NotRequired[EnhancedMonitoringType],
         "OpenMonitoring": NotRequired[OpenMonitoringTypeDef],
         "KafkaVersion": NotRequired[str],
         "LoggingInfo": NotRequired[LoggingInfoTypeDef],
         "InstanceType": NotRequired[str],
-        "ClientAuthentication": NotRequired[ClientAuthenticationOutputTypeDef],
+        "ClientAuthentication": NotRequired[ClientAuthenticationTypeDef],
         "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
         "ConnectivityInfo": NotRequired[ConnectivityInfoTypeDef],
         "StorageMode": NotRequired[StorageModeType],
-        "BrokerCountUpdateInfo": NotRequired[BrokerCountUpdateInfoTypeDef],
     },
 )
 UpdateConnectivityRequestRequestTypeDef = TypedDict(
     "UpdateConnectivityRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "CurrentVersion": str,
     },
 )
-ClusterInfoTypeDef = TypedDict(
-    "ClusterInfoTypeDef",
+ClusterInfoPaginatorTypeDef = TypedDict(
+    "ClusterInfoPaginatorTypeDef",
     {
         "ActiveOperationArn": NotRequired[str],
-        "BrokerNodeGroupInfo": NotRequired[BrokerNodeGroupInfoOutputTypeDef],
-        "ClientAuthentication": NotRequired[ClientAuthenticationOutputTypeDef],
+        "BrokerNodeGroupInfo": NotRequired[BrokerNodeGroupInfoPaginatorTypeDef],
+        "ClientAuthentication": NotRequired[ClientAuthenticationPaginatorTypeDef],
         "ClusterArn": NotRequired[str],
         "ClusterName": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "CurrentBrokerSoftwareInfo": NotRequired[BrokerSoftwareInfoTypeDef],
         "CurrentVersion": NotRequired[str],
         "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
         "EnhancedMonitoring": NotRequired[EnhancedMonitoringType],
@@ -1834,34 +1793,56 @@
         "Tags": NotRequired[Dict[str, str]],
         "ZookeeperConnectString": NotRequired[str],
         "ZookeeperConnectStringTls": NotRequired[str],
         "StorageMode": NotRequired[StorageModeType],
         "CustomerActionStatus": NotRequired[CustomerActionStatusType],
     },
 )
-ProvisionedTypeDef = TypedDict(
-    "ProvisionedTypeDef",
+ProvisionedPaginatorTypeDef = TypedDict(
+    "ProvisionedPaginatorTypeDef",
     {
-        "BrokerNodeGroupInfo": BrokerNodeGroupInfoOutputTypeDef,
+        "BrokerNodeGroupInfo": BrokerNodeGroupInfoPaginatorTypeDef,
         "NumberOfBrokerNodes": int,
         "CurrentBrokerSoftwareInfo": NotRequired[BrokerSoftwareInfoTypeDef],
-        "ClientAuthentication": NotRequired[ClientAuthenticationOutputTypeDef],
+        "ClientAuthentication": NotRequired[ClientAuthenticationPaginatorTypeDef],
         "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
         "EnhancedMonitoring": NotRequired[EnhancedMonitoringType],
         "OpenMonitoring": NotRequired[OpenMonitoringInfoTypeDef],
         "LoggingInfo": NotRequired[LoggingInfoTypeDef],
         "ZookeeperConnectString": NotRequired[str],
         "ZookeeperConnectStringTls": NotRequired[str],
         "StorageMode": NotRequired[StorageModeType],
         "CustomerActionStatus": NotRequired[CustomerActionStatusType],
     },
 )
-BrokerNodeGroupInfoUnionTypeDef = Union[
-    BrokerNodeGroupInfoTypeDef, BrokerNodeGroupInfoExtraOutputTypeDef
-]
+ClusterInfoTypeDef = TypedDict(
+    "ClusterInfoTypeDef",
+    {
+        "ActiveOperationArn": NotRequired[str],
+        "BrokerNodeGroupInfo": NotRequired[BrokerNodeGroupInfoTypeDef],
+        "ClientAuthentication": NotRequired[ClientAuthenticationTypeDef],
+        "ClusterArn": NotRequired[str],
+        "ClusterName": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "CurrentBrokerSoftwareInfo": NotRequired[BrokerSoftwareInfoTypeDef],
+        "CurrentVersion": NotRequired[str],
+        "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
+        "EnhancedMonitoring": NotRequired[EnhancedMonitoringType],
+        "OpenMonitoring": NotRequired[OpenMonitoringTypeDef],
+        "LoggingInfo": NotRequired[LoggingInfoTypeDef],
+        "NumberOfBrokerNodes": NotRequired[int],
+        "State": NotRequired[ClusterStateType],
+        "StateInfo": NotRequired[StateInfoTypeDef],
+        "Tags": NotRequired[Dict[str, str]],
+        "ZookeeperConnectString": NotRequired[str],
+        "ZookeeperConnectStringTls": NotRequired[str],
+        "StorageMode": NotRequired[StorageModeType],
+        "CustomerActionStatus": NotRequired[CustomerActionStatusType],
+    },
+)
 CreateClusterRequestRequestTypeDef = TypedDict(
     "CreateClusterRequestRequestTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "ClusterName": str,
         "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
@@ -1886,14 +1867,48 @@
         "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
         "EnhancedMonitoring": NotRequired[EnhancedMonitoringType],
         "OpenMonitoring": NotRequired[OpenMonitoringInfoTypeDef],
         "LoggingInfo": NotRequired[LoggingInfoTypeDef],
         "StorageMode": NotRequired[StorageModeType],
     },
 )
+ProvisionedTypeDef = TypedDict(
+    "ProvisionedTypeDef",
+    {
+        "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
+        "NumberOfBrokerNodes": int,
+        "CurrentBrokerSoftwareInfo": NotRequired[BrokerSoftwareInfoTypeDef],
+        "ClientAuthentication": NotRequired[ClientAuthenticationTypeDef],
+        "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
+        "EnhancedMonitoring": NotRequired[EnhancedMonitoringType],
+        "OpenMonitoring": NotRequired[OpenMonitoringInfoTypeDef],
+        "LoggingInfo": NotRequired[LoggingInfoTypeDef],
+        "ZookeeperConnectString": NotRequired[str],
+        "ZookeeperConnectStringTls": NotRequired[str],
+        "StorageMode": NotRequired[StorageModeType],
+        "CustomerActionStatus": NotRequired[CustomerActionStatusType],
+    },
+)
+ClusterOperationInfoPaginatorTypeDef = TypedDict(
+    "ClusterOperationInfoPaginatorTypeDef",
+    {
+        "ClientRequestId": NotRequired[str],
+        "ClusterArn": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "EndTime": NotRequired[datetime],
+        "ErrorInfo": NotRequired[ErrorInfoTypeDef],
+        "OperationArn": NotRequired[str],
+        "OperationState": NotRequired[str],
+        "OperationSteps": NotRequired[List[ClusterOperationStepTypeDef]],
+        "OperationType": NotRequired[str],
+        "SourceClusterInfo": NotRequired[MutableClusterInfoPaginatorTypeDef],
+        "TargetClusterInfo": NotRequired[MutableClusterInfoPaginatorTypeDef],
+        "VpcConnectionInfo": NotRequired[VpcConnectionInfoTypeDef],
+    },
+)
 ClusterOperationInfoTypeDef = TypedDict(
     "ClusterOperationInfoTypeDef",
     {
         "ClientRequestId": NotRequired[str],
         "ClusterArn": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "EndTime": NotRequired[datetime],
@@ -1912,27 +1927,60 @@
     {
         "OperationSteps": NotRequired[List[ClusterOperationStepTypeDef]],
         "SourceClusterInfo": NotRequired[MutableClusterInfoTypeDef],
         "TargetClusterInfo": NotRequired[MutableClusterInfoTypeDef],
         "VpcConnectionInfo": NotRequired[VpcConnectionInfoTypeDef],
     },
 )
+ListClustersResponsePaginatorTypeDef = TypedDict(
+    "ListClustersResponsePaginatorTypeDef",
+    {
+        "ClusterInfoList": List[ClusterInfoPaginatorTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ClusterPaginatorTypeDef = TypedDict(
+    "ClusterPaginatorTypeDef",
+    {
+        "ActiveOperationArn": NotRequired[str],
+        "ClusterType": NotRequired[ClusterTypeType],
+        "ClusterArn": NotRequired[str],
+        "ClusterName": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "CurrentVersion": NotRequired[str],
+        "State": NotRequired[ClusterStateType],
+        "StateInfo": NotRequired[StateInfoTypeDef],
+        "Tags": NotRequired[Dict[str, str]],
+        "Provisioned": NotRequired[ProvisionedPaginatorTypeDef],
+        "Serverless": NotRequired[ServerlessPaginatorTypeDef],
+    },
+)
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "ClusterInfo": ClusterInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListClustersResponseTypeDef = TypedDict(
     "ListClustersResponseTypeDef",
     {
         "ClusterInfoList": List[ClusterInfoTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
+    },
+)
+CreateClusterV2RequestRequestTypeDef = TypedDict(
+    "CreateClusterV2RequestRequestTypeDef",
+    {
+        "ClusterName": str,
+        "Tags": NotRequired[Mapping[str, str]],
+        "Provisioned": NotRequired[ProvisionedRequestTypeDef],
+        "Serverless": NotRequired[ServerlessRequestTypeDef],
     },
 )
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "ActiveOperationArn": NotRequired[str],
         "ClusterType": NotRequired[ClusterTypeType],
@@ -1943,36 +1991,35 @@
         "State": NotRequired[ClusterStateType],
         "StateInfo": NotRequired[StateInfoTypeDef],
         "Tags": NotRequired[Dict[str, str]],
         "Provisioned": NotRequired[ProvisionedTypeDef],
         "Serverless": NotRequired[ServerlessTypeDef],
     },
 )
-CreateClusterV2RequestRequestTypeDef = TypedDict(
-    "CreateClusterV2RequestRequestTypeDef",
+ListClusterOperationsResponsePaginatorTypeDef = TypedDict(
+    "ListClusterOperationsResponsePaginatorTypeDef",
     {
-        "ClusterName": str,
-        "Tags": NotRequired[Mapping[str, str]],
-        "Provisioned": NotRequired[ProvisionedRequestTypeDef],
-        "Serverless": NotRequired[ServerlessRequestTypeDef],
+        "ClusterOperationInfoList": List[ClusterOperationInfoPaginatorTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeClusterOperationResponseTypeDef = TypedDict(
     "DescribeClusterOperationResponseTypeDef",
     {
         "ClusterOperationInfo": ClusterOperationInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListClusterOperationsResponseTypeDef = TypedDict(
     "ListClusterOperationsResponseTypeDef",
     {
         "ClusterOperationInfoList": List[ClusterOperationInfoTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ClusterOperationV2TypeDef = TypedDict(
     "ClusterOperationV2TypeDef",
     {
         "ClusterArn": NotRequired[str],
         "ClusterType": NotRequired[ClusterTypeType],
@@ -1982,27 +2029,35 @@
         "OperationArn": NotRequired[str],
         "OperationState": NotRequired[str],
         "OperationType": NotRequired[str],
         "Provisioned": NotRequired[ClusterOperationV2ProvisionedTypeDef],
         "Serverless": NotRequired[ClusterOperationV2ServerlessTypeDef],
     },
 )
+ListClustersV2ResponsePaginatorTypeDef = TypedDict(
+    "ListClustersV2ResponsePaginatorTypeDef",
+    {
+        "ClusterInfoList": List[ClusterPaginatorTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DescribeClusterV2ResponseTypeDef = TypedDict(
     "DescribeClusterV2ResponseTypeDef",
     {
         "ClusterInfo": ClusterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListClustersV2ResponseTypeDef = TypedDict(
     "ListClustersV2ResponseTypeDef",
     {
         "ClusterInfoList": List[ClusterTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 DescribeClusterOperationV2ResponseTypeDef = TypedDict(
     "DescribeClusterOperationV2ResponseTypeDef",
     {
         "ClusterOperationInfo": ClusterOperationV2TypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy_boto3_kafka-1.34.107/mypy_boto3_kafka/type_defs.pyi` & `mypy-boto3-kafka-1.34.61/mypy_boto3_kafka/type_defs.pyi`

 * *Files 7% similar despite different names*

```diff
@@ -50,34 +50,31 @@
 __all__ = (
     "AmazonMskClusterTypeDef",
     "BatchAssociateScramSecretRequestRequestTypeDef",
     "ResponseMetadataTypeDef",
     "UnprocessedScramSecretTypeDef",
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     "BlobTypeDef",
-    "BrokerCountUpdateInfoTypeDef",
     "ProvisionedThroughputTypeDef",
     "CloudWatchLogsTypeDef",
     "FirehoseTypeDef",
     "S3TypeDef",
     "BrokerSoftwareInfoTypeDef",
-    "TlsExtraOutputTypeDef",
+    "TlsPaginatorTypeDef",
     "UnauthenticatedTypeDef",
-    "TlsOutputTypeDef",
     "TlsTypeDef",
     "ClientVpcConnectionTypeDef",
     "StateInfoTypeDef",
     "ErrorInfoTypeDef",
     "ClusterOperationStepInfoTypeDef",
     "ClusterOperationV2SummaryTypeDef",
     "CompatibleKafkaVersionTypeDef",
     "ConfigurationInfoTypeDef",
     "ConfigurationRevisionTypeDef",
     "PublicAccessTypeDef",
-    "ConsumerGroupReplicationOutputTypeDef",
     "ConsumerGroupReplicationTypeDef",
     "ConsumerGroupReplicationUpdateTypeDef",
     "CreateVpcConnectionRequestRequestTypeDef",
     "DeleteClusterPolicyRequestRequestTypeDef",
     "DeleteClusterRequestRequestTypeDef",
     "DeleteConfigurationRequestRequestTypeDef",
     "DeleteReplicatorRequestRequestTypeDef",
@@ -95,15 +92,14 @@
     "EncryptionInTransitTypeDef",
     "GetBootstrapBrokersRequestRequestTypeDef",
     "GetClusterPolicyRequestRequestTypeDef",
     "GetCompatibleKafkaVersionsRequestRequestTypeDef",
     "IamTypeDef",
     "JmxExporterInfoTypeDef",
     "JmxExporterTypeDef",
-    "KafkaClusterClientVpcConfigOutputTypeDef",
     "KafkaClusterClientVpcConfigTypeDef",
     "KafkaVersionTypeDef",
     "PaginatorConfigTypeDef",
     "ListClientVpcConnectionsRequestRequestTypeDef",
     "ListClusterOperationsRequestRequestTypeDef",
     "ListClusterOperationsV2RequestRequestTypeDef",
     "ListClustersRequestRequestTypeDef",
@@ -122,16 +118,16 @@
     "ZookeeperNodeInfoTypeDef",
     "PutClusterPolicyRequestRequestTypeDef",
     "RebootBrokerRequestRequestTypeDef",
     "RejectClientVpcConnectionRequestRequestTypeDef",
     "ReplicationInfoSummaryTypeDef",
     "ReplicationStartingPositionTypeDef",
     "ScramTypeDef",
+    "VpcConfigPaginatorTypeDef",
     "VpcConfigTypeDef",
-    "VpcConfigOutputTypeDef",
     "TagResourceRequestRequestTypeDef",
     "TopicReplicationUpdateTypeDef",
     "UntagResourceRequestRequestTypeDef",
     "UpdateBrokerCountRequestRequestTypeDef",
     "UpdateBrokerTypeRequestRequestTypeDef",
     "UserIdentityTypeDef",
     "VpcConnectivityTlsTypeDef",
@@ -201,15 +197,14 @@
     "ListNodesRequestListNodesPaginateTypeDef",
     "ListReplicatorsRequestListReplicatorsPaginateTypeDef",
     "ListScramSecretsRequestListScramSecretsPaginateTypeDef",
     "ListVpcConnectionsRequestListVpcConnectionsPaginateTypeDef",
     "ListVpcConnectionsResponseTypeDef",
     "PrometheusInfoTypeDef",
     "PrometheusTypeDef",
-    "TopicReplicationOutputTypeDef",
     "TopicReplicationTypeDef",
     "SaslTypeDef",
     "UpdateReplicationInfoRequestRequestTypeDef",
     "VpcConnectionInfoServerlessTypeDef",
     "VpcConnectionInfoTypeDef",
     "VpcConnectivitySaslTypeDef",
     "ReplicatorSummaryTypeDef",
@@ -219,49 +214,54 @@
     "NodeInfoTypeDef",
     "ListConfigurationsResponseTypeDef",
     "ServerlessClientAuthenticationTypeDef",
     "OpenMonitoringInfoTypeDef",
     "OpenMonitoringTypeDef",
     "ReplicationInfoDescriptionTypeDef",
     "ReplicationInfoTypeDef",
-    "ClientAuthenticationExtraOutputTypeDef",
-    "ClientAuthenticationOutputTypeDef",
+    "ClientAuthenticationPaginatorTypeDef",
     "ClientAuthenticationTypeDef",
     "ClusterOperationV2ServerlessTypeDef",
     "VpcConnectivityClientAuthenticationTypeDef",
     "ListReplicatorsResponseTypeDef",
     "ListNodesResponseTypeDef",
+    "ServerlessPaginatorTypeDef",
     "ServerlessRequestTypeDef",
     "ServerlessTypeDef",
     "UpdateMonitoringRequestRequestTypeDef",
     "DescribeReplicatorResponseTypeDef",
     "CreateReplicatorRequestRequestTypeDef",
-    "ClientAuthenticationUnionTypeDef",
     "UpdateSecurityRequestRequestTypeDef",
     "VpcConnectivityTypeDef",
     "ConnectivityInfoTypeDef",
-    "BrokerNodeGroupInfoExtraOutputTypeDef",
-    "BrokerNodeGroupInfoOutputTypeDef",
+    "BrokerNodeGroupInfoPaginatorTypeDef",
     "BrokerNodeGroupInfoTypeDef",
+    "MutableClusterInfoPaginatorTypeDef",
     "MutableClusterInfoTypeDef",
     "UpdateConnectivityRequestRequestTypeDef",
+    "ClusterInfoPaginatorTypeDef",
+    "ProvisionedPaginatorTypeDef",
     "ClusterInfoTypeDef",
-    "ProvisionedTypeDef",
-    "BrokerNodeGroupInfoUnionTypeDef",
     "CreateClusterRequestRequestTypeDef",
     "ProvisionedRequestTypeDef",
+    "ProvisionedTypeDef",
+    "ClusterOperationInfoPaginatorTypeDef",
     "ClusterOperationInfoTypeDef",
     "ClusterOperationV2ProvisionedTypeDef",
+    "ListClustersResponsePaginatorTypeDef",
+    "ClusterPaginatorTypeDef",
     "DescribeClusterResponseTypeDef",
     "ListClustersResponseTypeDef",
-    "ClusterTypeDef",
     "CreateClusterV2RequestRequestTypeDef",
+    "ClusterTypeDef",
+    "ListClusterOperationsResponsePaginatorTypeDef",
     "DescribeClusterOperationResponseTypeDef",
     "ListClusterOperationsResponseTypeDef",
     "ClusterOperationV2TypeDef",
+    "ListClustersV2ResponsePaginatorTypeDef",
     "DescribeClusterV2ResponseTypeDef",
     "ListClustersV2ResponseTypeDef",
     "DescribeClusterOperationV2ResponseTypeDef",
 )
 
 AmazonMskClusterTypeDef = TypedDict(
     "AmazonMskClusterTypeDef",
@@ -298,21 +298,14 @@
     "BatchDisassociateScramSecretRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "SecretArnList": Sequence[str],
     },
 )
 BlobTypeDef = Union[str, bytes, IO[Any], StreamingBody]
-BrokerCountUpdateInfoTypeDef = TypedDict(
-    "BrokerCountUpdateInfoTypeDef",
-    {
-        "CreatedBrokerIds": NotRequired[List[float]],
-        "DeletedBrokerIds": NotRequired[List[float]],
-    },
-)
 ProvisionedThroughputTypeDef = TypedDict(
     "ProvisionedThroughputTypeDef",
     {
         "Enabled": NotRequired[bool],
         "VolumeThroughput": NotRequired[int],
     },
 )
@@ -342,34 +335,27 @@
     "BrokerSoftwareInfoTypeDef",
     {
         "ConfigurationArn": NotRequired[str],
         "ConfigurationRevision": NotRequired[int],
         "KafkaVersion": NotRequired[str],
     },
 )
-TlsExtraOutputTypeDef = TypedDict(
-    "TlsExtraOutputTypeDef",
+TlsPaginatorTypeDef = TypedDict(
+    "TlsPaginatorTypeDef",
     {
         "CertificateAuthorityArnList": NotRequired[List[str]],
         "Enabled": NotRequired[bool],
     },
 )
 UnauthenticatedTypeDef = TypedDict(
     "UnauthenticatedTypeDef",
     {
         "Enabled": NotRequired[bool],
     },
 )
-TlsOutputTypeDef = TypedDict(
-    "TlsOutputTypeDef",
-    {
-        "CertificateAuthorityArnList": NotRequired[List[str]],
-        "Enabled": NotRequired[bool],
-    },
-)
 TlsTypeDef = TypedDict(
     "TlsTypeDef",
     {
         "CertificateAuthorityArnList": NotRequired[Sequence[str]],
         "Enabled": NotRequired[bool],
     },
 )
@@ -439,23 +425,14 @@
 )
 PublicAccessTypeDef = TypedDict(
     "PublicAccessTypeDef",
     {
         "Type": NotRequired[str],
     },
 )
-ConsumerGroupReplicationOutputTypeDef = TypedDict(
-    "ConsumerGroupReplicationOutputTypeDef",
-    {
-        "ConsumerGroupsToReplicate": List[str],
-        "ConsumerGroupsToExclude": NotRequired[List[str]],
-        "DetectAndCopyNewConsumerGroups": NotRequired[bool],
-        "SynchroniseConsumerGroupOffsets": NotRequired[bool],
-    },
-)
 ConsumerGroupReplicationTypeDef = TypedDict(
     "ConsumerGroupReplicationTypeDef",
     {
         "ConsumerGroupsToReplicate": Sequence[str],
         "ConsumerGroupsToExclude": NotRequired[Sequence[str]],
         "DetectAndCopyNewConsumerGroups": NotRequired[bool],
         "SynchroniseConsumerGroupOffsets": NotRequired[bool],
@@ -614,21 +591,14 @@
 )
 JmxExporterTypeDef = TypedDict(
     "JmxExporterTypeDef",
     {
         "EnabledInBroker": bool,
     },
 )
-KafkaClusterClientVpcConfigOutputTypeDef = TypedDict(
-    "KafkaClusterClientVpcConfigOutputTypeDef",
-    {
-        "SubnetIds": List[str],
-        "SecurityGroupIds": NotRequired[List[str]],
-    },
-)
 KafkaClusterClientVpcConfigTypeDef = TypedDict(
     "KafkaClusterClientVpcConfigTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": NotRequired[Sequence[str]],
     },
 )
@@ -817,28 +787,28 @@
 )
 ScramTypeDef = TypedDict(
     "ScramTypeDef",
     {
         "Enabled": NotRequired[bool],
     },
 )
+VpcConfigPaginatorTypeDef = TypedDict(
+    "VpcConfigPaginatorTypeDef",
+    {
+        "SubnetIds": List[str],
+        "SecurityGroupIds": NotRequired[List[str]],
+    },
+)
 VpcConfigTypeDef = TypedDict(
     "VpcConfigTypeDef",
     {
         "SubnetIds": Sequence[str],
         "SecurityGroupIds": NotRequired[Sequence[str]],
     },
 )
-VpcConfigOutputTypeDef = TypedDict(
-    "VpcConfigOutputTypeDef",
-    {
-        "SubnetIds": List[str],
-        "SecurityGroupIds": NotRequired[List[str]],
-    },
-)
 TagResourceRequestRequestTypeDef = TypedDict(
     "TagResourceRequestRequestTypeDef",
     {
         "ResourceArn": str,
         "Tags": Mapping[str, str],
     },
 )
@@ -1036,17 +1006,17 @@
         "Policy": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListScramSecretsResponseTypeDef = TypedDict(
     "ListScramSecretsResponseTypeDef",
     {
+        "NextToken": str,
         "SecretArnList": List[str],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListTagsForResourceResponseTypeDef = TypedDict(
     "ListTagsForResourceResponseTypeDef",
     {
         "Tags": Dict[str, str],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1224,31 +1194,31 @@
         "Endpoints": NotRequired[List[str]],
     },
 )
 ListClientVpcConnectionsResponseTypeDef = TypedDict(
     "ListClientVpcConnectionsResponseTypeDef",
     {
         "ClientVpcConnections": List[ClientVpcConnectionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ClusterOperationStepTypeDef = TypedDict(
     "ClusterOperationStepTypeDef",
     {
         "StepInfo": NotRequired[ClusterOperationStepInfoTypeDef],
         "StepName": NotRequired[str],
     },
 )
 ListClusterOperationsV2ResponseTypeDef = TypedDict(
     "ListClusterOperationsV2ResponseTypeDef",
     {
         "ClusterOperationInfoList": List[ClusterOperationV2SummaryTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 GetCompatibleKafkaVersionsResponseTypeDef = TypedDict(
     "GetCompatibleKafkaVersionsResponseTypeDef",
     {
         "CompatibleKafkaVersions": List[CompatibleKafkaVersionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
@@ -1306,17 +1276,17 @@
         "State": ConfigurationStateType,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListConfigurationRevisionsResponseTypeDef = TypedDict(
     "ListConfigurationRevisionsResponseTypeDef",
     {
+        "NextToken": str,
         "Revisions": List[ConfigurationRevisionTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 UpdateConfigurationResponseTypeDef = TypedDict(
     "UpdateConfigurationResponseTypeDef",
     {
         "Arn": str,
         "LatestRevision": ConfigurationRevisionTypeDef,
@@ -1337,30 +1307,30 @@
     },
 )
 KafkaClusterDescriptionTypeDef = TypedDict(
     "KafkaClusterDescriptionTypeDef",
     {
         "AmazonMskCluster": NotRequired[AmazonMskClusterTypeDef],
         "KafkaClusterAlias": NotRequired[str],
-        "VpcConfig": NotRequired[KafkaClusterClientVpcConfigOutputTypeDef],
+        "VpcConfig": NotRequired[KafkaClusterClientVpcConfigTypeDef],
     },
 )
 KafkaClusterTypeDef = TypedDict(
     "KafkaClusterTypeDef",
     {
         "AmazonMskCluster": AmazonMskClusterTypeDef,
         "VpcConfig": KafkaClusterClientVpcConfigTypeDef,
     },
 )
 ListKafkaVersionsResponseTypeDef = TypedDict(
     "ListKafkaVersionsResponseTypeDef",
     {
         "KafkaVersions": List[KafkaVersionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef = TypedDict(
     "ListClientVpcConnectionsRequestListClientVpcConnectionsPaginateTypeDef",
     {
         "ClusterArn": str,
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
@@ -1441,16 +1411,16 @@
         "PaginationConfig": NotRequired[PaginatorConfigTypeDef],
     },
 )
 ListVpcConnectionsResponseTypeDef = TypedDict(
     "ListVpcConnectionsResponseTypeDef",
     {
         "VpcConnections": List[VpcConnectionTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 PrometheusInfoTypeDef = TypedDict(
     "PrometheusInfoTypeDef",
     {
         "JmxExporter": NotRequired[JmxExporterInfoTypeDef],
         "NodeExporter": NotRequired[NodeExporterInfoTypeDef],
@@ -1459,25 +1429,14 @@
 PrometheusTypeDef = TypedDict(
     "PrometheusTypeDef",
     {
         "JmxExporter": NotRequired[JmxExporterTypeDef],
         "NodeExporter": NotRequired[NodeExporterTypeDef],
     },
 )
-TopicReplicationOutputTypeDef = TypedDict(
-    "TopicReplicationOutputTypeDef",
-    {
-        "TopicsToReplicate": List[str],
-        "CopyAccessControlListsForTopics": NotRequired[bool],
-        "CopyTopicConfigurations": NotRequired[bool],
-        "DetectAndCopyNewTopics": NotRequired[bool],
-        "StartingPosition": NotRequired[ReplicationStartingPositionTypeDef],
-        "TopicsToExclude": NotRequired[List[str]],
-    },
-)
 TopicReplicationTypeDef = TypedDict(
     "TopicReplicationTypeDef",
     {
         "TopicsToReplicate": Sequence[str],
         "CopyAccessControlListsForTopics": NotRequired[bool],
         "CopyTopicConfigurations": NotRequired[bool],
         "DetectAndCopyNewTopics": NotRequired[bool],
@@ -1573,16 +1532,16 @@
         "ZookeeperNodeInfo": NotRequired[ZookeeperNodeInfoTypeDef],
     },
 )
 ListConfigurationsResponseTypeDef = TypedDict(
     "ListConfigurationsResponseTypeDef",
     {
         "Configurations": List[ConfigurationTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ServerlessClientAuthenticationTypeDef = TypedDict(
     "ServerlessClientAuthenticationTypeDef",
     {
         "Sasl": NotRequired[ServerlessSaslTypeDef],
     },
@@ -1598,44 +1557,36 @@
     {
         "Prometheus": PrometheusTypeDef,
     },
 )
 ReplicationInfoDescriptionTypeDef = TypedDict(
     "ReplicationInfoDescriptionTypeDef",
     {
-        "ConsumerGroupReplication": NotRequired[ConsumerGroupReplicationOutputTypeDef],
+        "ConsumerGroupReplication": NotRequired[ConsumerGroupReplicationTypeDef],
         "SourceKafkaClusterAlias": NotRequired[str],
         "TargetCompressionType": NotRequired[TargetCompressionTypeType],
         "TargetKafkaClusterAlias": NotRequired[str],
-        "TopicReplication": NotRequired[TopicReplicationOutputTypeDef],
+        "TopicReplication": NotRequired[TopicReplicationTypeDef],
     },
 )
 ReplicationInfoTypeDef = TypedDict(
     "ReplicationInfoTypeDef",
     {
         "ConsumerGroupReplication": ConsumerGroupReplicationTypeDef,
         "SourceKafkaClusterArn": str,
         "TargetCompressionType": TargetCompressionTypeType,
         "TargetKafkaClusterArn": str,
         "TopicReplication": TopicReplicationTypeDef,
     },
 )
-ClientAuthenticationExtraOutputTypeDef = TypedDict(
-    "ClientAuthenticationExtraOutputTypeDef",
-    {
-        "Sasl": NotRequired[SaslTypeDef],
-        "Tls": NotRequired[TlsExtraOutputTypeDef],
-        "Unauthenticated": NotRequired[UnauthenticatedTypeDef],
-    },
-)
-ClientAuthenticationOutputTypeDef = TypedDict(
-    "ClientAuthenticationOutputTypeDef",
+ClientAuthenticationPaginatorTypeDef = TypedDict(
+    "ClientAuthenticationPaginatorTypeDef",
     {
         "Sasl": NotRequired[SaslTypeDef],
-        "Tls": NotRequired[TlsOutputTypeDef],
+        "Tls": NotRequired[TlsPaginatorTypeDef],
         "Unauthenticated": NotRequired[UnauthenticatedTypeDef],
     },
 )
 ClientAuthenticationTypeDef = TypedDict(
     "ClientAuthenticationTypeDef",
     {
         "Sasl": NotRequired[SaslTypeDef],
@@ -1655,38 +1606,45 @@
         "Sasl": NotRequired[VpcConnectivitySaslTypeDef],
         "Tls": NotRequired[VpcConnectivityTlsTypeDef],
     },
 )
 ListReplicatorsResponseTypeDef = TypedDict(
     "ListReplicatorsResponseTypeDef",
     {
+        "NextToken": str,
         "Replicators": List[ReplicatorSummaryTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ListNodesResponseTypeDef = TypedDict(
     "ListNodesResponseTypeDef",
     {
+        "NextToken": str,
         "NodeInfoList": List[NodeInfoTypeDef],
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
+    },
+)
+ServerlessPaginatorTypeDef = TypedDict(
+    "ServerlessPaginatorTypeDef",
+    {
+        "VpcConfigs": List[VpcConfigPaginatorTypeDef],
+        "ClientAuthentication": NotRequired[ServerlessClientAuthenticationTypeDef],
     },
 )
 ServerlessRequestTypeDef = TypedDict(
     "ServerlessRequestTypeDef",
     {
         "VpcConfigs": Sequence[VpcConfigTypeDef],
         "ClientAuthentication": NotRequired[ServerlessClientAuthenticationTypeDef],
     },
 )
 ServerlessTypeDef = TypedDict(
     "ServerlessTypeDef",
     {
-        "VpcConfigs": List[VpcConfigOutputTypeDef],
+        "VpcConfigs": List[VpcConfigTypeDef],
         "ClientAuthentication": NotRequired[ServerlessClientAuthenticationTypeDef],
     },
 )
 UpdateMonitoringRequestRequestTypeDef = TypedDict(
     "UpdateMonitoringRequestRequestTypeDef",
     {
         "ClusterArn": str,
@@ -1722,17 +1680,14 @@
         "ReplicationInfoList": Sequence[ReplicationInfoTypeDef],
         "ReplicatorName": str,
         "ServiceExecutionRoleArn": str,
         "Description": NotRequired[str],
         "Tags": NotRequired[Mapping[str, str]],
     },
 )
-ClientAuthenticationUnionTypeDef = Union[
-    ClientAuthenticationTypeDef, ClientAuthenticationExtraOutputTypeDef
-]
 UpdateSecurityRequestRequestTypeDef = TypedDict(
     "UpdateSecurityRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "CurrentVersion": str,
         "ClientAuthentication": NotRequired[ClientAuthenticationTypeDef],
         "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
@@ -1747,28 +1702,16 @@
 ConnectivityInfoTypeDef = TypedDict(
     "ConnectivityInfoTypeDef",
     {
         "PublicAccess": NotRequired[PublicAccessTypeDef],
         "VpcConnectivity": NotRequired[VpcConnectivityTypeDef],
     },
 )
-BrokerNodeGroupInfoExtraOutputTypeDef = TypedDict(
-    "BrokerNodeGroupInfoExtraOutputTypeDef",
-    {
-        "ClientSubnets": List[str],
-        "InstanceType": str,
-        "BrokerAZDistribution": NotRequired[Literal["DEFAULT"]],
-        "SecurityGroups": NotRequired[List[str]],
-        "StorageInfo": NotRequired[StorageInfoTypeDef],
-        "ConnectivityInfo": NotRequired[ConnectivityInfoTypeDef],
-        "ZoneIds": NotRequired[List[str]],
-    },
-)
-BrokerNodeGroupInfoOutputTypeDef = TypedDict(
-    "BrokerNodeGroupInfoOutputTypeDef",
+BrokerNodeGroupInfoPaginatorTypeDef = TypedDict(
+    "BrokerNodeGroupInfoPaginatorTypeDef",
     {
         "ClientSubnets": List[str],
         "InstanceType": str,
         "BrokerAZDistribution": NotRequired[Literal["DEFAULT"]],
         "SecurityGroups": NotRequired[List[str]],
         "StorageInfo": NotRequired[StorageInfoTypeDef],
         "ConnectivityInfo": NotRequired[ConnectivityInfoTypeDef],
@@ -1783,46 +1726,62 @@
         "BrokerAZDistribution": NotRequired[Literal["DEFAULT"]],
         "SecurityGroups": NotRequired[Sequence[str]],
         "StorageInfo": NotRequired[StorageInfoTypeDef],
         "ConnectivityInfo": NotRequired[ConnectivityInfoTypeDef],
         "ZoneIds": NotRequired[Sequence[str]],
     },
 )
+MutableClusterInfoPaginatorTypeDef = TypedDict(
+    "MutableClusterInfoPaginatorTypeDef",
+    {
+        "BrokerEBSVolumeInfo": NotRequired[List[BrokerEBSVolumeInfoTypeDef]],
+        "ConfigurationInfo": NotRequired[ConfigurationInfoTypeDef],
+        "NumberOfBrokerNodes": NotRequired[int],
+        "EnhancedMonitoring": NotRequired[EnhancedMonitoringType],
+        "OpenMonitoring": NotRequired[OpenMonitoringTypeDef],
+        "KafkaVersion": NotRequired[str],
+        "LoggingInfo": NotRequired[LoggingInfoTypeDef],
+        "InstanceType": NotRequired[str],
+        "ClientAuthentication": NotRequired[ClientAuthenticationPaginatorTypeDef],
+        "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
+        "ConnectivityInfo": NotRequired[ConnectivityInfoTypeDef],
+        "StorageMode": NotRequired[StorageModeType],
+    },
+)
 MutableClusterInfoTypeDef = TypedDict(
     "MutableClusterInfoTypeDef",
     {
         "BrokerEBSVolumeInfo": NotRequired[List[BrokerEBSVolumeInfoTypeDef]],
         "ConfigurationInfo": NotRequired[ConfigurationInfoTypeDef],
         "NumberOfBrokerNodes": NotRequired[int],
         "EnhancedMonitoring": NotRequired[EnhancedMonitoringType],
         "OpenMonitoring": NotRequired[OpenMonitoringTypeDef],
         "KafkaVersion": NotRequired[str],
         "LoggingInfo": NotRequired[LoggingInfoTypeDef],
         "InstanceType": NotRequired[str],
-        "ClientAuthentication": NotRequired[ClientAuthenticationOutputTypeDef],
+        "ClientAuthentication": NotRequired[ClientAuthenticationTypeDef],
         "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
         "ConnectivityInfo": NotRequired[ConnectivityInfoTypeDef],
         "StorageMode": NotRequired[StorageModeType],
-        "BrokerCountUpdateInfo": NotRequired[BrokerCountUpdateInfoTypeDef],
     },
 )
 UpdateConnectivityRequestRequestTypeDef = TypedDict(
     "UpdateConnectivityRequestRequestTypeDef",
     {
         "ClusterArn": str,
         "ConnectivityInfo": ConnectivityInfoTypeDef,
         "CurrentVersion": str,
     },
 )
-ClusterInfoTypeDef = TypedDict(
-    "ClusterInfoTypeDef",
+ClusterInfoPaginatorTypeDef = TypedDict(
+    "ClusterInfoPaginatorTypeDef",
     {
         "ActiveOperationArn": NotRequired[str],
-        "BrokerNodeGroupInfo": NotRequired[BrokerNodeGroupInfoOutputTypeDef],
-        "ClientAuthentication": NotRequired[ClientAuthenticationOutputTypeDef],
+        "BrokerNodeGroupInfo": NotRequired[BrokerNodeGroupInfoPaginatorTypeDef],
+        "ClientAuthentication": NotRequired[ClientAuthenticationPaginatorTypeDef],
         "ClusterArn": NotRequired[str],
         "ClusterName": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "CurrentBrokerSoftwareInfo": NotRequired[BrokerSoftwareInfoTypeDef],
         "CurrentVersion": NotRequired[str],
         "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
         "EnhancedMonitoring": NotRequired[EnhancedMonitoringType],
@@ -1834,34 +1793,56 @@
         "Tags": NotRequired[Dict[str, str]],
         "ZookeeperConnectString": NotRequired[str],
         "ZookeeperConnectStringTls": NotRequired[str],
         "StorageMode": NotRequired[StorageModeType],
         "CustomerActionStatus": NotRequired[CustomerActionStatusType],
     },
 )
-ProvisionedTypeDef = TypedDict(
-    "ProvisionedTypeDef",
+ProvisionedPaginatorTypeDef = TypedDict(
+    "ProvisionedPaginatorTypeDef",
     {
-        "BrokerNodeGroupInfo": BrokerNodeGroupInfoOutputTypeDef,
+        "BrokerNodeGroupInfo": BrokerNodeGroupInfoPaginatorTypeDef,
         "NumberOfBrokerNodes": int,
         "CurrentBrokerSoftwareInfo": NotRequired[BrokerSoftwareInfoTypeDef],
-        "ClientAuthentication": NotRequired[ClientAuthenticationOutputTypeDef],
+        "ClientAuthentication": NotRequired[ClientAuthenticationPaginatorTypeDef],
         "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
         "EnhancedMonitoring": NotRequired[EnhancedMonitoringType],
         "OpenMonitoring": NotRequired[OpenMonitoringInfoTypeDef],
         "LoggingInfo": NotRequired[LoggingInfoTypeDef],
         "ZookeeperConnectString": NotRequired[str],
         "ZookeeperConnectStringTls": NotRequired[str],
         "StorageMode": NotRequired[StorageModeType],
         "CustomerActionStatus": NotRequired[CustomerActionStatusType],
     },
 )
-BrokerNodeGroupInfoUnionTypeDef = Union[
-    BrokerNodeGroupInfoTypeDef, BrokerNodeGroupInfoExtraOutputTypeDef
-]
+ClusterInfoTypeDef = TypedDict(
+    "ClusterInfoTypeDef",
+    {
+        "ActiveOperationArn": NotRequired[str],
+        "BrokerNodeGroupInfo": NotRequired[BrokerNodeGroupInfoTypeDef],
+        "ClientAuthentication": NotRequired[ClientAuthenticationTypeDef],
+        "ClusterArn": NotRequired[str],
+        "ClusterName": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "CurrentBrokerSoftwareInfo": NotRequired[BrokerSoftwareInfoTypeDef],
+        "CurrentVersion": NotRequired[str],
+        "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
+        "EnhancedMonitoring": NotRequired[EnhancedMonitoringType],
+        "OpenMonitoring": NotRequired[OpenMonitoringTypeDef],
+        "LoggingInfo": NotRequired[LoggingInfoTypeDef],
+        "NumberOfBrokerNodes": NotRequired[int],
+        "State": NotRequired[ClusterStateType],
+        "StateInfo": NotRequired[StateInfoTypeDef],
+        "Tags": NotRequired[Dict[str, str]],
+        "ZookeeperConnectString": NotRequired[str],
+        "ZookeeperConnectStringTls": NotRequired[str],
+        "StorageMode": NotRequired[StorageModeType],
+        "CustomerActionStatus": NotRequired[CustomerActionStatusType],
+    },
+)
 CreateClusterRequestRequestTypeDef = TypedDict(
     "CreateClusterRequestRequestTypeDef",
     {
         "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
         "ClusterName": str,
         "KafkaVersion": str,
         "NumberOfBrokerNodes": int,
@@ -1886,14 +1867,48 @@
         "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
         "EnhancedMonitoring": NotRequired[EnhancedMonitoringType],
         "OpenMonitoring": NotRequired[OpenMonitoringInfoTypeDef],
         "LoggingInfo": NotRequired[LoggingInfoTypeDef],
         "StorageMode": NotRequired[StorageModeType],
     },
 )
+ProvisionedTypeDef = TypedDict(
+    "ProvisionedTypeDef",
+    {
+        "BrokerNodeGroupInfo": BrokerNodeGroupInfoTypeDef,
+        "NumberOfBrokerNodes": int,
+        "CurrentBrokerSoftwareInfo": NotRequired[BrokerSoftwareInfoTypeDef],
+        "ClientAuthentication": NotRequired[ClientAuthenticationTypeDef],
+        "EncryptionInfo": NotRequired[EncryptionInfoTypeDef],
+        "EnhancedMonitoring": NotRequired[EnhancedMonitoringType],
+        "OpenMonitoring": NotRequired[OpenMonitoringInfoTypeDef],
+        "LoggingInfo": NotRequired[LoggingInfoTypeDef],
+        "ZookeeperConnectString": NotRequired[str],
+        "ZookeeperConnectStringTls": NotRequired[str],
+        "StorageMode": NotRequired[StorageModeType],
+        "CustomerActionStatus": NotRequired[CustomerActionStatusType],
+    },
+)
+ClusterOperationInfoPaginatorTypeDef = TypedDict(
+    "ClusterOperationInfoPaginatorTypeDef",
+    {
+        "ClientRequestId": NotRequired[str],
+        "ClusterArn": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "EndTime": NotRequired[datetime],
+        "ErrorInfo": NotRequired[ErrorInfoTypeDef],
+        "OperationArn": NotRequired[str],
+        "OperationState": NotRequired[str],
+        "OperationSteps": NotRequired[List[ClusterOperationStepTypeDef]],
+        "OperationType": NotRequired[str],
+        "SourceClusterInfo": NotRequired[MutableClusterInfoPaginatorTypeDef],
+        "TargetClusterInfo": NotRequired[MutableClusterInfoPaginatorTypeDef],
+        "VpcConnectionInfo": NotRequired[VpcConnectionInfoTypeDef],
+    },
+)
 ClusterOperationInfoTypeDef = TypedDict(
     "ClusterOperationInfoTypeDef",
     {
         "ClientRequestId": NotRequired[str],
         "ClusterArn": NotRequired[str],
         "CreationTime": NotRequired[datetime],
         "EndTime": NotRequired[datetime],
@@ -1912,27 +1927,60 @@
     {
         "OperationSteps": NotRequired[List[ClusterOperationStepTypeDef]],
         "SourceClusterInfo": NotRequired[MutableClusterInfoTypeDef],
         "TargetClusterInfo": NotRequired[MutableClusterInfoTypeDef],
         "VpcConnectionInfo": NotRequired[VpcConnectionInfoTypeDef],
     },
 )
+ListClustersResponsePaginatorTypeDef = TypedDict(
+    "ListClustersResponsePaginatorTypeDef",
+    {
+        "ClusterInfoList": List[ClusterInfoPaginatorTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
+ClusterPaginatorTypeDef = TypedDict(
+    "ClusterPaginatorTypeDef",
+    {
+        "ActiveOperationArn": NotRequired[str],
+        "ClusterType": NotRequired[ClusterTypeType],
+        "ClusterArn": NotRequired[str],
+        "ClusterName": NotRequired[str],
+        "CreationTime": NotRequired[datetime],
+        "CurrentVersion": NotRequired[str],
+        "State": NotRequired[ClusterStateType],
+        "StateInfo": NotRequired[StateInfoTypeDef],
+        "Tags": NotRequired[Dict[str, str]],
+        "Provisioned": NotRequired[ProvisionedPaginatorTypeDef],
+        "Serverless": NotRequired[ServerlessPaginatorTypeDef],
+    },
+)
 DescribeClusterResponseTypeDef = TypedDict(
     "DescribeClusterResponseTypeDef",
     {
         "ClusterInfo": ClusterInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListClustersResponseTypeDef = TypedDict(
     "ListClustersResponseTypeDef",
     {
         "ClusterInfoList": List[ClusterInfoTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
+    },
+)
+CreateClusterV2RequestRequestTypeDef = TypedDict(
+    "CreateClusterV2RequestRequestTypeDef",
+    {
+        "ClusterName": str,
+        "Tags": NotRequired[Mapping[str, str]],
+        "Provisioned": NotRequired[ProvisionedRequestTypeDef],
+        "Serverless": NotRequired[ServerlessRequestTypeDef],
     },
 )
 ClusterTypeDef = TypedDict(
     "ClusterTypeDef",
     {
         "ActiveOperationArn": NotRequired[str],
         "ClusterType": NotRequired[ClusterTypeType],
@@ -1943,36 +1991,35 @@
         "State": NotRequired[ClusterStateType],
         "StateInfo": NotRequired[StateInfoTypeDef],
         "Tags": NotRequired[Dict[str, str]],
         "Provisioned": NotRequired[ProvisionedTypeDef],
         "Serverless": NotRequired[ServerlessTypeDef],
     },
 )
-CreateClusterV2RequestRequestTypeDef = TypedDict(
-    "CreateClusterV2RequestRequestTypeDef",
+ListClusterOperationsResponsePaginatorTypeDef = TypedDict(
+    "ListClusterOperationsResponsePaginatorTypeDef",
     {
-        "ClusterName": str,
-        "Tags": NotRequired[Mapping[str, str]],
-        "Provisioned": NotRequired[ProvisionedRequestTypeDef],
-        "Serverless": NotRequired[ServerlessRequestTypeDef],
+        "ClusterOperationInfoList": List[ClusterOperationInfoPaginatorTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 DescribeClusterOperationResponseTypeDef = TypedDict(
     "DescribeClusterOperationResponseTypeDef",
     {
         "ClusterOperationInfo": ClusterOperationInfoTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListClusterOperationsResponseTypeDef = TypedDict(
     "ListClusterOperationsResponseTypeDef",
     {
         "ClusterOperationInfoList": List[ClusterOperationInfoTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 ClusterOperationV2TypeDef = TypedDict(
     "ClusterOperationV2TypeDef",
     {
         "ClusterArn": NotRequired[str],
         "ClusterType": NotRequired[ClusterTypeType],
@@ -1982,27 +2029,35 @@
         "OperationArn": NotRequired[str],
         "OperationState": NotRequired[str],
         "OperationType": NotRequired[str],
         "Provisioned": NotRequired[ClusterOperationV2ProvisionedTypeDef],
         "Serverless": NotRequired[ClusterOperationV2ServerlessTypeDef],
     },
 )
+ListClustersV2ResponsePaginatorTypeDef = TypedDict(
+    "ListClustersV2ResponsePaginatorTypeDef",
+    {
+        "ClusterInfoList": List[ClusterPaginatorTypeDef],
+        "NextToken": str,
+        "ResponseMetadata": ResponseMetadataTypeDef,
+    },
+)
 DescribeClusterV2ResponseTypeDef = TypedDict(
     "DescribeClusterV2ResponseTypeDef",
     {
         "ClusterInfo": ClusterTypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
     },
 )
 ListClustersV2ResponseTypeDef = TypedDict(
     "ListClustersV2ResponseTypeDef",
     {
         "ClusterInfoList": List[ClusterTypeDef],
+        "NextToken": str,
         "ResponseMetadata": ResponseMetadataTypeDef,
-        "NextToken": NotRequired[str],
     },
 )
 DescribeClusterOperationV2ResponseTypeDef = TypedDict(
     "DescribeClusterOperationV2ResponseTypeDef",
     {
         "ClusterOperationInfo": ClusterOperationV2TypeDef,
         "ResponseMetadata": ResponseMetadataTypeDef,
```

### Comparing `mypy_boto3_kafka-1.34.107/mypy_boto3_kafka.egg-info/PKG-INFO` & `mypy-boto3-kafka-1.34.61/mypy_boto3_kafka.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: mypy-boto3-kafka
-Version: 1.34.107
-Summary: Type annotations for boto3.Kafka 1.34.107 service generated with mypy-boto3-builder 7.24.0
+Version: 1.34.61
+Summary: Type annotations for boto3.Kafka 1.34.61 service generated with mypy-boto3-builder 7.23.2
 Home-page: https://github.com/youtype/mypy_boto3_builder
 Author: Vlad Emelianov
 Author-email: vlad.emelianov.nz@gmail.com
 License: MIT License
 Project-URL: Documentation, https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/
 Project-URL: Source, https://github.com/youtype/mypy_boto3_builder
 Project-URL: Tracker, https://github.com/youtype/mypy_boto3_builder/issues
@@ -39,24 +39,24 @@
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mypy-boto3-kafka.svg?color=blue)](https://pypi.org/project/mypy-boto3-kafka)
 [![Docs](https://img.shields.io/readthedocs/boto3-stubs.svg?color=blue)](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/)
 [![PyPI - Downloads](https://static.pepy.tech/badge/mypy-boto3-kafka)](https://pepy.tech/project/mypy-boto3-kafka)
 
 ![boto3.typed](https://github.com/youtype/mypy_boto3_builder/raw/main/logo.png)
 
 Type annotations for
-[boto3.Kafka 1.34.107](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
+[boto3.Kafka 1.34.61](https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/kafka.html#Kafka)
 service compatible with [VSCode](https://code.visualstudio.com/),
 [PyCharm](https://www.jetbrains.com/pycharm/),
 [Emacs](https://www.gnu.org/software/emacs/),
 [Sublime Text](https://www.sublimetext.com/),
 [mypy](https://github.com/python/mypy),
 [pyright](https://github.com/microsoft/pyright) and other tools.
 
 Generated by
-[mypy-boto3-builder 7.24.0](https://github.com/youtype/mypy_boto3_builder).
+[mypy-boto3-builder 7.23.2](https://github.com/youtype/mypy_boto3_builder).
 
 More information can be found on
 [boto3-stubs](https://pypi.org/project/boto3-stubs/) page and in
 [mypy-boto3-kafka docs](https://youtype.github.io/boto3_stubs_docs/mypy_boto3_kafka/).
 
 See how it helps to find and fix potential bugs:
```

### Comparing `mypy_boto3_kafka-1.34.107/mypy_boto3_kafka.egg-info/SOURCES.txt` & `mypy-boto3-kafka-1.34.61/mypy_boto3_kafka.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mypy_boto3_kafka-1.34.107/setup.py` & `mypy-boto3-kafka-1.34.61/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,21 +7,21 @@
 from setuptools import setup
 
 LONG_DESCRIPTION = (Path(__file__).parent / "README.md").read_text()
 
 
 setup(
     name="mypy-boto3-kafka",
-    version="1.34.107",
+    version="1.34.61",
     packages=["mypy_boto3_kafka"],
     url="https://github.com/youtype/mypy_boto3_builder",
     license="MIT License",
     author="Vlad Emelianov",
     author_email="vlad.emelianov.nz@gmail.com",
-    description="Type annotations for boto3.Kafka 1.34.107 service generated with mypy-boto3-builder 7.24.0",
+    description="Type annotations for boto3.Kafka 1.34.61 service generated with mypy-boto3-builder 7.23.2",
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "Environment :: Console",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: OS Independent",
```

