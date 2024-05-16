# Comparing `tmp/pulumi_awsx-2.8.0.tar.gz` & `tmp/pulumi_awsx-2.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_awsx-2.8.0.tar", last modified: Fri Apr 19 19:21:49 2024, max compression
+gzip compressed data, was "pulumi_awsx-2.9.0.tar", last modified: Wed Apr 24 09:18:41 2024, max compression
```

## Comparing `pulumi_awsx-2.8.0.tar` & `pulumi_awsx-2.9.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.699719 pulumi_awsx-2.8.0/
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-19 19:21:49.699719 pulumi_awsx-2.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.691719 pulumi_awsx-2.8.0/pulumi_awsx/
--rw-------   0 runner    (1001) docker     (127)     2193 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9223 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.691719 pulumi_awsx-2.8.0/pulumi_awsx/awsx/
--rw-------   0 runner    (1001) docker     (127)      223 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/awsx/__init__.py
--rw-------   0 runner    (1001) docker     (127)    57488 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/awsx/_inputs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.691719 pulumi_awsx-2.8.0/pulumi_awsx/cloudtrail/
--rw-------   0 runner    (1001) docker     (127)      265 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/cloudtrail/__init__.py
--rw-------   0 runner    (1001) docker     (127)    23412 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/cloudtrail/trail.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.695719 pulumi_awsx-2.8.0/pulumi_awsx/ec2/
--rw-------   0 runner    (1001) docker     (127)      388 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ec2/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1983 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ec2/_enums.py
--rw-------   0 runner    (1001) docker     (127)    34412 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ec2/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     3839 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ec2/default_vpc.py
--rw-------   0 runner    (1001) docker     (127)     3454 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ec2/get_default_vpc.py
--rw-------   0 runner    (1001) docker     (127)     4520 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ec2/outputs.py
--rw-------   0 runner    (1001) docker     (127)    41221 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ec2/vpc.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.695719 pulumi_awsx-2.8.0/pulumi_awsx/ecr/
--rw-------   0 runner    (1001) docker     (127)      336 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecr/__init__.py
--rw-------   0 runner    (1001) docker     (127)      834 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecr/_enums.py
--rw-------   0 runner    (1001) docker     (127)     7578 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecr/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    15525 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecr/image.py
--rw-------   0 runner    (1001) docker     (127)    14431 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecr/repository.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.695719 pulumi_awsx-2.8.0/pulumi_awsx/ecs/
--rw-------   0 runner    (1001) docker     (127)      421 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecs/__init__.py
--rw-------   0 runner    (1001) docker     (127)      354 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecs/_enums.py
--rw-------   0 runner    (1001) docker     (127)    86174 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecs/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    46322 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecs/ec2_service.py
--rw-------   0 runner    (1001) docker     (127)    31286 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecs/ec2_task_definition.py
--rw-------   0 runner    (1001) docker     (127)    45038 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecs/fargate_service.py
--rw-------   0 runner    (1001) docker     (127)    30189 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/ecs/fargate_task_definition.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.695719 pulumi_awsx-2.8.0/pulumi_awsx/lb/
--rw-------   0 runner    (1001) docker     (127)      384 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/lb/__init__.py
--rw-------   0 runner    (1001) docker     (127)    97738 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/lb/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    43234 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/lb/application_load_balancer.py
--rw-------   0 runner    (1001) docker     (127)    40347 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/lb/network_load_balancer.py
--rw-------   0 runner    (1001) docker     (127)    11113 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/lb/target_group_attachment.py
--rw-------   0 runner    (1001) docker     (127)     2719 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/provider.py
--rw-------   0 runner    (1001) docker     (127)       41 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pulumi_awsx/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-19 19:21:49.699719 pulumi_awsx-2.8.0/pulumi_awsx.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-19 19:21:49.000000 pulumi_awsx-2.8.0/pulumi_awsx.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-19 19:21:49.000000 pulumi_awsx-2.8.0/pulumi_awsx.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-19 19:21:49.000000 pulumi_awsx-2.8.0/pulumi_awsx.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-19 19:21:49.000000 pulumi_awsx-2.8.0/pulumi_awsx.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-19 19:21:49.000000 pulumi_awsx-2.8.0/pulumi_awsx.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      747 2024-04-19 19:21:41.000000 pulumi_awsx-2.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-19 19:21:49.699719 pulumi_awsx-2.8.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:18:41.591648 pulumi_awsx-2.9.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-24 09:18:41.591648 pulumi_awsx-2.9.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5992 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:18:41.583648 pulumi_awsx-2.9.0/pulumi_awsx/
+-rw-------   0 runner    (1001) docker     (127)     2193 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9223 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:18:41.583648 pulumi_awsx-2.9.0/pulumi_awsx/awsx/
+-rw-------   0 runner    (1001) docker     (127)      223 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/awsx/__init__.py
+-rw-------   0 runner    (1001) docker     (127)    58261 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/awsx/_inputs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:18:41.583648 pulumi_awsx-2.9.0/pulumi_awsx/cloudtrail/
+-rw-------   0 runner    (1001) docker     (127)      265 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/cloudtrail/__init__.py
+-rw-------   0 runner    (1001) docker     (127)    23412 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/cloudtrail/trail.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:18:41.587648 pulumi_awsx-2.9.0/pulumi_awsx/ec2/
+-rw-------   0 runner    (1001) docker     (127)      388 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ec2/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1983 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ec2/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    33706 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ec2/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     3839 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ec2/default_vpc.py
+-rw-------   0 runner    (1001) docker     (127)     3454 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ec2/get_default_vpc.py
+-rw-------   0 runner    (1001) docker     (127)     4520 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ec2/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    41221 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ec2/vpc.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:18:41.587648 pulumi_awsx-2.9.0/pulumi_awsx/ecr/
+-rw-------   0 runner    (1001) docker     (127)      336 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ecr/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      834 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ecr/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     7578 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ecr/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    15525 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ecr/image.py
+-rw-------   0 runner    (1001) docker     (127)    14431 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ecr/repository.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:18:41.587648 pulumi_awsx-2.9.0/pulumi_awsx/ecs/
+-rw-------   0 runner    (1001) docker     (127)      421 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ecs/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      354 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ecs/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    87680 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ecs/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    46334 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ecs/ec2_service.py
+-rw-------   0 runner    (1001) docker     (127)    32387 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ecs/ec2_task_definition.py
+-rw-------   0 runner    (1001) docker     (127)    45050 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ecs/fargate_service.py
+-rw-------   0 runner    (1001) docker     (127)    31290 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/ecs/fargate_task_definition.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:18:41.587648 pulumi_awsx-2.9.0/pulumi_awsx/lb/
+-rw-------   0 runner    (1001) docker     (127)      384 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/lb/__init__.py
+-rw-------   0 runner    (1001) docker     (127)   106884 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/lb/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    48027 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/lb/application_load_balancer.py
+-rw-------   0 runner    (1001) docker     (127)    45176 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/lb/network_load_balancer.py
+-rw-------   0 runner    (1001) docker     (127)    11113 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/lb/target_group_attachment.py
+-rw-------   0 runner    (1001) docker     (127)     2719 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/provider.py
+-rw-------   0 runner    (1001) docker     (127)       41 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pulumi_awsx/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-24 09:18:41.591648 pulumi_awsx-2.9.0/pulumi_awsx.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6529 2024-04-24 09:18:41.000000 pulumi_awsx-2.9.0/pulumi_awsx.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1189 2024-04-24 09:18:41.000000 pulumi_awsx-2.9.0/pulumi_awsx.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-24 09:18:41.000000 pulumi_awsx-2.9.0/pulumi_awsx.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-24 09:18:41.000000 pulumi_awsx-2.9.0/pulumi_awsx.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-24 09:18:41.000000 pulumi_awsx-2.9.0/pulumi_awsx.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      747 2024-04-24 09:18:33.000000 pulumi_awsx-2.9.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-24 09:18:41.591648 pulumi_awsx-2.9.0/setup.cfg
```

### Comparing `pulumi_awsx-2.8.0/PKG-INFO` & `pulumi_awsx-2.9.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_awsx
-Version: 2.8.0
+Version: 2.9.0
 Summary: Pulumi Amazon Web Services (AWS) AWSX Components.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-awsx
 Keywords: pulumi,aws,awsx,kind/component,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_awsx-2.8.0/README.md` & `pulumi_awsx-2.9.0/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/__init__.py` & `pulumi_awsx-2.9.0/pulumi_awsx/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/_utilities.py` & `pulumi_awsx-2.9.0/pulumi_awsx/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/awsx/_inputs.py` & `pulumi_awsx-2.9.0/pulumi_awsx/awsx/_inputs.py`

 * *Files 1% similar despite different names*

```diff
@@ -642,34 +642,38 @@
         pulumi.set(self, "region", value)
 
 
 @pulumi.input_type
 class LogGroupArgs:
     def __init__(__self__, *,
                  kms_key_id: Optional[pulumi.Input[str]] = None,
+                 log_group_class: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
                  retention_in_days: Optional[pulumi.Input[int]] = None,
                  skip_destroy: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         The set of arguments for constructing a LogGroup resource.
         :param pulumi.Input[str] kms_key_id: The ARN of the KMS Key to use when encrypting log data. Please note, after the AWS KMS CMK is disassociated from the log group,
                AWS CloudWatch Logs stops encrypting newly ingested data for the log group. All previously ingested data remains encrypted, and AWS CloudWatch Logs requires
                permissions for the CMK whenever the encrypted data is requested.
+        :param pulumi.Input[str] log_group_class: Specified the log class of the log group. Possible values are: `STANDARD` or `INFREQUENT_ACCESS`.
         :param pulumi.Input[str] name: The name of the log group. If omitted, this provider will assign a random, unique name.
         :param pulumi.Input[str] name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `name`.
         :param pulumi.Input[int] retention_in_days: Specifies the number of days
                you want to retain log events in the specified log group.  Possible values are: 1, 3, 5, 7, 14, 30, 60, 90, 120, 150, 180, 365, 400, 545, 731, 1096, 1827, 2192, 2557, 2922, 3288, 3653, and 0.
                If you select 0, the events in the log group are always retained and never expire.
         :param pulumi.Input[bool] skip_destroy: Set to true if you do not wish the log group (and any logs it may contain) to be deleted at destroy time, and instead just remove the log group from the state.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags to assign to the resource. .If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         """
         if kms_key_id is not None:
             pulumi.set(__self__, "kms_key_id", kms_key_id)
+        if log_group_class is not None:
+            pulumi.set(__self__, "log_group_class", log_group_class)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if name_prefix is not None:
             pulumi.set(__self__, "name_prefix", name_prefix)
         if retention_in_days is not None:
             pulumi.set(__self__, "retention_in_days", retention_in_days)
         if skip_destroy is not None:
@@ -688,14 +692,26 @@
         return pulumi.get(self, "kms_key_id")
 
     @kms_key_id.setter
     def kms_key_id(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "kms_key_id", value)
 
     @property
+    @pulumi.getter(name="logGroupClass")
+    def log_group_class(self) -> Optional[pulumi.Input[str]]:
+        """
+        Specified the log class of the log group. Possible values are: `STANDARD` or `INFREQUENT_ACCESS`.
+        """
+        return pulumi.get(self, "log_group_class")
+
+    @log_group_class.setter
+    def log_group_class(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "log_group_class", value)
+
+    @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
         The name of the log group. If omitted, this provider will assign a random, unique name.
         """
         return pulumi.get(self, "name")
```

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/cloudtrail/trail.py` & `pulumi_awsx-2.9.0/pulumi_awsx/cloudtrail/trail.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ec2/_enums.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ec2/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ec2/_inputs.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ec2/_inputs.py`

 * *Files 19% similar despite different names*

```diff
@@ -180,47 +180,47 @@
         Route Tables - (an association between a VPC endpoint and a single `route_table_id`),
         Security Groups - (an association between a VPC endpoint and a single `security_group_id`),
         and Subnets - (an association between a VPC endpoint and a single `subnet_id`) and
         a VPC Endpoint resource with `route_table_ids` and `subnet_ids` attributes.
         Do not use the same resource ID in both a VPC Endpoint resource and a VPC Endpoint Association resource.
         Doing so will cause a conflict of associations and will overwrite the association.
 
-        {{% examples %}}
         ## Example Usage
-        {{% example %}}
+
         ### Basic
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
         const s3 = new aws.ec2.VpcEndpoint("s3", {
-            vpcId: aws_vpc.main.id,
+            vpcId: main.id,
             serviceName: "com.amazonaws.us-west-2.s3",
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
         s3 = aws.ec2.VpcEndpoint("s3",
-            vpc_id=aws_vpc["main"]["id"],
+            vpc_id=main["id"],
             service_name="com.amazonaws.us-west-2.s3")
         ```
         ```csharp
         using System.Collections.Generic;
         using System.Linq;
         using Pulumi;
         using Aws = Pulumi.Aws;
 
         return await Deployment.RunAsync(() => 
         {
             var s3 = new Aws.Ec2.VpcEndpoint("s3", new()
             {
-                VpcId = aws_vpc.Main.Id,
+                VpcId = main.Id,
                 ServiceName = "com.amazonaws.us-west-2.s3",
             });
 
         });
         ```
         ```go
         package main
@@ -229,15 +229,15 @@
         	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/ec2"
         	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
         )
 
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
         		_, err := ec2.NewVpcEndpoint(ctx, "s3", &ec2.VpcEndpointArgs{
-        			VpcId:       pulumi.Any(aws_vpc.Main.Id),
+        			VpcId:       pulumi.Any(main.Id),
         			ServiceName: pulumi.String("com.amazonaws.us-west-2.s3"),
         		})
         		if err != nil {
         			return err
         		}
         		return nil
         	})
@@ -261,51 +261,52 @@
         public class App {
             public static void main(String[] args) {
                 Pulumi.run(App::stack);
             }
 
             public static void stack(Context ctx) {
                 var s3 = new VpcEndpoint("s3", VpcEndpointArgs.builder()        
-                    .vpcId(aws_vpc.main().id())
+                    .vpcId(main.id())
                     .serviceName("com.amazonaws.us-west-2.s3")
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
           s3:
             type: aws:ec2:VpcEndpoint
             properties:
-              vpcId: ${aws_vpc.main.id}
+              vpcId: ${main.id}
               serviceName: com.amazonaws.us-west-2.s3
         ```
-        {{% /example %}}
-        {{% example %}}
+        <!--End PulumiCodeChooser -->
+
         ### Basic w/ Tags
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
         const s3 = new aws.ec2.VpcEndpoint("s3", {
-            vpcId: aws_vpc.main.id,
+            vpcId: main.id,
             serviceName: "com.amazonaws.us-west-2.s3",
             tags: {
                 Environment: "test",
             },
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
         s3 = aws.ec2.VpcEndpoint("s3",
-            vpc_id=aws_vpc["main"]["id"],
+            vpc_id=main["id"],
             service_name="com.amazonaws.us-west-2.s3",
             tags={
                 "Environment": "test",
             })
         ```
         ```csharp
         using System.Collections.Generic;
@@ -313,15 +314,15 @@
         using Pulumi;
         using Aws = Pulumi.Aws;
 
         return await Deployment.RunAsync(() => 
         {
             var s3 = new Aws.Ec2.VpcEndpoint("s3", new()
             {
-                VpcId = aws_vpc.Main.Id,
+                VpcId = main.Id,
                 ServiceName = "com.amazonaws.us-west-2.s3",
                 Tags = 
                 {
                     { "Environment", "test" },
                 },
             });
 
@@ -334,15 +335,15 @@
         	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/ec2"
         	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
         )
 
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
         		_, err := ec2.NewVpcEndpoint(ctx, "s3", &ec2.VpcEndpointArgs{
-        			VpcId:       pulumi.Any(aws_vpc.Main.Id),
+        			VpcId:       pulumi.Any(main.Id),
         			ServiceName: pulumi.String("com.amazonaws.us-west-2.s3"),
         			Tags: pulumi.StringMap{
         				"Environment": pulumi.String("test"),
         			},
         		})
         		if err != nil {
         			return err
@@ -369,75 +370,76 @@
         public class App {
             public static void main(String[] args) {
                 Pulumi.run(App::stack);
             }
 
             public static void stack(Context ctx) {
                 var s3 = new VpcEndpoint("s3", VpcEndpointArgs.builder()        
-                    .vpcId(aws_vpc.main().id())
+                    .vpcId(main.id())
                     .serviceName("com.amazonaws.us-west-2.s3")
                     .tags(Map.of("Environment", "test"))
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
           s3:
             type: aws:ec2:VpcEndpoint
             properties:
-              vpcId: ${aws_vpc.main.id}
+              vpcId: ${main.id}
               serviceName: com.amazonaws.us-west-2.s3
               tags:
                 Environment: test
         ```
-        {{% /example %}}
-        {{% example %}}
+        <!--End PulumiCodeChooser -->
+
         ### Interface Endpoint Type
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
         const ec2 = new aws.ec2.VpcEndpoint("ec2", {
-            vpcId: aws_vpc.main.id,
+            vpcId: main.id,
             serviceName: "com.amazonaws.us-west-2.ec2",
             vpcEndpointType: "Interface",
-            securityGroupIds: [aws_security_group.sg1.id],
+            securityGroupIds: [sg1.id],
             privateDnsEnabled: true,
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
         ec2 = aws.ec2.VpcEndpoint("ec2",
-            vpc_id=aws_vpc["main"]["id"],
+            vpc_id=main["id"],
             service_name="com.amazonaws.us-west-2.ec2",
             vpc_endpoint_type="Interface",
-            security_group_ids=[aws_security_group["sg1"]["id"]],
+            security_group_ids=[sg1["id"]],
             private_dns_enabled=True)
         ```
         ```csharp
         using System.Collections.Generic;
         using System.Linq;
         using Pulumi;
         using Aws = Pulumi.Aws;
 
         return await Deployment.RunAsync(() => 
         {
             var ec2 = new Aws.Ec2.VpcEndpoint("ec2", new()
             {
-                VpcId = aws_vpc.Main.Id,
+                VpcId = main.Id,
                 ServiceName = "com.amazonaws.us-west-2.ec2",
                 VpcEndpointType = "Interface",
                 SecurityGroupIds = new[]
                 {
-                    aws_security_group.Sg1.Id,
+                    sg1.Id,
                 },
                 PrivateDnsEnabled = true,
             });
 
         });
         ```
         ```go
@@ -447,19 +449,19 @@
         	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/ec2"
         	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
         )
 
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
         		_, err := ec2.NewVpcEndpoint(ctx, "ec2", &ec2.VpcEndpointArgs{
-        			VpcId:           pulumi.Any(aws_vpc.Main.Id),
+        			VpcId:           pulumi.Any(main.Id),
         			ServiceName:     pulumi.String("com.amazonaws.us-west-2.ec2"),
         			VpcEndpointType: pulumi.String("Interface"),
         			SecurityGroupIds: pulumi.StringArray{
-        				aws_security_group.Sg1.Id,
+        				sg1.Id,
         			},
         			PrivateDnsEnabled: pulumi.Bool(true),
         		})
         		if err != nil {
         			return err
         		}
         		return nil
@@ -484,104 +486,105 @@
         public class App {
             public static void main(String[] args) {
                 Pulumi.run(App::stack);
             }
 
             public static void stack(Context ctx) {
                 var ec2 = new VpcEndpoint("ec2", VpcEndpointArgs.builder()        
-                    .vpcId(aws_vpc.main().id())
+                    .vpcId(main.id())
                     .serviceName("com.amazonaws.us-west-2.ec2")
                     .vpcEndpointType("Interface")
-                    .securityGroupIds(aws_security_group.sg1().id())
+                    .securityGroupIds(sg1.id())
                     .privateDnsEnabled(true)
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
           ec2:
             type: aws:ec2:VpcEndpoint
             properties:
-              vpcId: ${aws_vpc.main.id}
+              vpcId: ${main.id}
               serviceName: com.amazonaws.us-west-2.ec2
               vpcEndpointType: Interface
               securityGroupIds:
-                - ${aws_security_group.sg1.id}
+                - ${sg1.id}
               privateDnsEnabled: true
         ```
-        {{% /example %}}
-        {{% example %}}
+        <!--End PulumiCodeChooser -->
+
         ### Gateway Load Balancer Endpoint Type
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
         const current = aws.getCallerIdentity({});
-        const exampleVpcEndpointService = new aws.ec2.VpcEndpointService("exampleVpcEndpointService", {
+        const example = new aws.ec2.VpcEndpointService("example", {
             acceptanceRequired: false,
             allowedPrincipals: [current.then(current => current.arn)],
-            gatewayLoadBalancerArns: [aws_lb.example.arn],
+            gatewayLoadBalancerArns: [exampleAwsLb.arn],
         });
-        const exampleVpcEndpoint = new aws.ec2.VpcEndpoint("exampleVpcEndpoint", {
-            serviceName: exampleVpcEndpointService.serviceName,
-            subnetIds: [aws_subnet.example.id],
-            vpcEndpointType: exampleVpcEndpointService.serviceType,
-            vpcId: aws_vpc.example.id,
+        const exampleVpcEndpoint = new aws.ec2.VpcEndpoint("example", {
+            serviceName: example.serviceName,
+            subnetIds: [exampleAwsSubnet.id],
+            vpcEndpointType: example.serviceType,
+            vpcId: exampleAwsVpc.id,
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
         current = aws.get_caller_identity()
-        example_vpc_endpoint_service = aws.ec2.VpcEndpointService("exampleVpcEndpointService",
+        example = aws.ec2.VpcEndpointService("example",
             acceptance_required=False,
             allowed_principals=[current.arn],
-            gateway_load_balancer_arns=[aws_lb["example"]["arn"]])
-        example_vpc_endpoint = aws.ec2.VpcEndpoint("exampleVpcEndpoint",
-            service_name=example_vpc_endpoint_service.service_name,
-            subnet_ids=[aws_subnet["example"]["id"]],
-            vpc_endpoint_type=example_vpc_endpoint_service.service_type,
-            vpc_id=aws_vpc["example"]["id"])
+            gateway_load_balancer_arns=[example_aws_lb["arn"]])
+        example_vpc_endpoint = aws.ec2.VpcEndpoint("example",
+            service_name=example.service_name,
+            subnet_ids=[example_aws_subnet["id"]],
+            vpc_endpoint_type=example.service_type,
+            vpc_id=example_aws_vpc["id"])
         ```
         ```csharp
         using System.Collections.Generic;
         using System.Linq;
         using Pulumi;
         using Aws = Pulumi.Aws;
 
         return await Deployment.RunAsync(() => 
         {
             var current = Aws.GetCallerIdentity.Invoke();
 
-            var exampleVpcEndpointService = new Aws.Ec2.VpcEndpointService("exampleVpcEndpointService", new()
+            var example = new Aws.Ec2.VpcEndpointService("example", new()
             {
                 AcceptanceRequired = false,
                 AllowedPrincipals = new[]
                 {
                     current.Apply(getCallerIdentityResult => getCallerIdentityResult.Arn),
                 },
                 GatewayLoadBalancerArns = new[]
                 {
-                    aws_lb.Example.Arn,
+                    exampleAwsLb.Arn,
                 },
             });
 
-            var exampleVpcEndpoint = new Aws.Ec2.VpcEndpoint("exampleVpcEndpoint", new()
+            var exampleVpcEndpoint = new Aws.Ec2.VpcEndpoint("example", new()
             {
-                ServiceName = exampleVpcEndpointService.ServiceName,
+                ServiceName = example.ServiceName,
                 SubnetIds = new[]
                 {
-                    aws_subnet.Example.Id,
+                    exampleAwsSubnet.Id,
                 },
-                VpcEndpointType = exampleVpcEndpointService.ServiceType,
-                VpcId = aws_vpc.Example.Id,
+                VpcEndpointType = example.ServiceType,
+                VpcId = exampleAwsVpc.Id,
             });
 
         });
         ```
         ```go
         package main
 
@@ -593,33 +596,33 @@
 
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
         		current, err := aws.GetCallerIdentity(ctx, nil, nil)
         		if err != nil {
         			return err
         		}
-        		exampleVpcEndpointService, err := ec2.NewVpcEndpointService(ctx, "exampleVpcEndpointService", &ec2.VpcEndpointServiceArgs{
+        		example, err := ec2.NewVpcEndpointService(ctx, "example", &ec2.VpcEndpointServiceArgs{
         			AcceptanceRequired: pulumi.Bool(false),
         			AllowedPrincipals: pulumi.StringArray{
-        				*pulumi.String(current.Arn),
+        				pulumi.String(current.Arn),
         			},
         			GatewayLoadBalancerArns: pulumi.StringArray{
-        				aws_lb.Example.Arn,
+        				exampleAwsLb.Arn,
         			},
         		})
         		if err != nil {
         			return err
         		}
-        		_, err = ec2.NewVpcEndpoint(ctx, "exampleVpcEndpoint", &ec2.VpcEndpointArgs{
-        			ServiceName: exampleVpcEndpointService.ServiceName,
+        		_, err = ec2.NewVpcEndpoint(ctx, "example", &ec2.VpcEndpointArgs{
+        			ServiceName: example.ServiceName,
         			SubnetIds: pulumi.StringArray{
-        				aws_subnet.Example.Id,
+        				exampleAwsSubnet.Id,
         			},
-        			VpcEndpointType: exampleVpcEndpointService.ServiceType,
-        			VpcId:           pulumi.Any(aws_vpc.Example.Id),
+        			VpcEndpointType: example.ServiceType,
+        			VpcId:           pulumi.Any(exampleAwsVpc.Id),
         		})
         		if err != nil {
         			return err
         		}
         		return nil
         	})
         }
@@ -647,65 +650,65 @@
             public static void main(String[] args) {
                 Pulumi.run(App::stack);
             }
 
             public static void stack(Context ctx) {
                 final var current = AwsFunctions.getCallerIdentity();
 
-                var exampleVpcEndpointService = new VpcEndpointService("exampleVpcEndpointService", VpcEndpointServiceArgs.builder()        
+                var example = new VpcEndpointService("example", VpcEndpointServiceArgs.builder()        
                     .acceptanceRequired(false)
                     .allowedPrincipals(current.applyValue(getCallerIdentityResult -> getCallerIdentityResult.arn()))
-                    .gatewayLoadBalancerArns(aws_lb.example().arn())
+                    .gatewayLoadBalancerArns(exampleAwsLb.arn())
                     .build());
 
                 var exampleVpcEndpoint = new VpcEndpoint("exampleVpcEndpoint", VpcEndpointArgs.builder()        
-                    .serviceName(exampleVpcEndpointService.serviceName())
-                    .subnetIds(aws_subnet.example().id())
-                    .vpcEndpointType(exampleVpcEndpointService.serviceType())
-                    .vpcId(aws_vpc.example().id())
+                    .serviceName(example.serviceName())
+                    .subnetIds(exampleAwsSubnet.id())
+                    .vpcEndpointType(example.serviceType())
+                    .vpcId(exampleAwsVpc.id())
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
-          exampleVpcEndpointService:
+          example:
             type: aws:ec2:VpcEndpointService
             properties:
               acceptanceRequired: false
               allowedPrincipals:
                 - ${current.arn}
               gatewayLoadBalancerArns:
-                - ${aws_lb.example.arn}
+                - ${exampleAwsLb.arn}
           exampleVpcEndpoint:
             type: aws:ec2:VpcEndpoint
+            name: example
             properties:
-              serviceName: ${exampleVpcEndpointService.serviceName}
+              serviceName: ${example.serviceName}
               subnetIds:
-                - ${aws_subnet.example.id}
-              vpcEndpointType: ${exampleVpcEndpointService.serviceType}
-              vpcId: ${aws_vpc.example.id}
+                - ${exampleAwsSubnet.id}
+              vpcEndpointType: ${example.serviceType}
+              vpcId: ${exampleAwsVpc.id}
         variables:
           current:
             fn::invoke:
               Function: aws:getCallerIdentity
               Arguments: {}
         ```
-        {{% /example %}}
-        {{% /examples %}}
+        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Using `pulumi import`, import VPC Endpoints using the VPC endpoint `id`. For example:
 
         ```sh
-         $ pulumi import aws:ec2/vpcEndpoint:VpcEndpoint endpoint1 vpce-3ecf2a57
+        $ pulumi import aws:ec2/vpcEndpoint:VpcEndpoint endpoint1 vpce-3ecf2a57
         ```
-         
+
         :param str service_name: The service name. For AWS services the service name is usually in the form `com.amazonaws.<region>.<service>` (the SageMaker Notebook service is an exception to this rule, the service name is in the form `aws.sagemaker.<region>.notebook`).
         :param bool auto_accept: Accept the VPC endpoint (the VPC endpoint and service need to be in the same AWS account).
         :param pulumi.Input['pulumi_aws.ec2.VpcEndpointDnsOptionsArgs'] dns_options: The DNS options for the endpoint. See dns_options below.
         :param pulumi.Input[str] ip_address_type: The IP address type for the endpoint. Valid values are `ipv4`, `dualstack`, and `ipv6`.
         :param pulumi.Input[str] policy: A policy to attach to the endpoint that controls access to the service. This is a JSON formatted string. Defaults to full access. All `Gateway` and some `Interface` endpoints support policies - see the [relevant AWS documentation](https://docs.aws.amazon.com/vpc/latest/userguide/vpc-endpoints-access.html) for more details.
         :param bool private_dns_enabled: Whether or not to associate a private hosted zone with the specified VPC. Applicable for endpoints of type Interface. Defaults to `false`.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] route_table_ids: One or more route table IDs. Applicable for endpoints of type `Gateway`.
```

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ec2/default_vpc.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ec2/default_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ec2/get_default_vpc.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ec2/get_default_vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ec2/outputs.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ec2/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ec2/vpc.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ec2/vpc.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ecr/_enums.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ecr/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ecr/_inputs.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ecr/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ecr/image.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ecr/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ecr/repository.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ecr/repository.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ecs/_inputs.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ecs/_inputs.py`

 * *Files 0% similar despite different names*

```diff
@@ -54,14 +54,15 @@
                  pid_mode: Optional[pulumi.Input[str]] = None,
                  placement_constraints: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionPlacementConstraintArgs']]]] = None,
                  proxy_configuration: Optional[pulumi.Input['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs']] = None,
                  runtime_platform: Optional[pulumi.Input['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs']] = None,
                  skip_destroy: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  task_role: Optional['_awsx.DefaultRoleWithPolicyArgs'] = None,
+                 track_latest: Optional[pulumi.Input[bool]] = None,
                  volumes: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]] = None):
         """
         Create a TaskDefinition resource with the given unique name, arguments, and options.
         Creates required log-group and task & execution roles.
         Presents required Service load balancers if target group included in port mappings.
         :param 'TaskDefinitionContainerDefinitionArgs' container: Single container to make a TaskDefinition from.  Useful for simple cases where there aren't
                multiple containers, especially when creating a TaskDefinition to call [run] on.
@@ -86,14 +87,15 @@
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionPlacementConstraintArgs']]] placement_constraints: Configuration block for rules that are taken into consideration during task placement. Maximum number of `placement_constraints` is `10`. Detailed below.
         :param pulumi.Input['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs'] proxy_configuration: Configuration block for the App Mesh proxy. Detailed below.
         :param pulumi.Input['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs'] runtime_platform: Configuration block for runtime_platform that containers in your task may use.
         :param pulumi.Input[bool] skip_destroy: Whether to retain the old revision when the resource is destroyed or replacement is necessary. Default is `false`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param '_awsx.DefaultRoleWithPolicyArgs' task_role: IAM role that allows your Amazon ECS container task to make calls to other AWS services.
                Will be created automatically if not defined.
+        :param pulumi.Input[bool] track_latest: Whether should track latest task definition or the one created with the resource. Default is `false`.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]] volumes: Configuration block for volumes that containers in your task may use. Detailed below.
         """
         if container is not None:
             pulumi.set(__self__, "container", container)
         if containers is not None:
             pulumi.set(__self__, "containers", containers)
         if cpu is not None:
@@ -124,14 +126,16 @@
             pulumi.set(__self__, "runtime_platform", runtime_platform)
         if skip_destroy is not None:
             pulumi.set(__self__, "skip_destroy", skip_destroy)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if task_role is not None:
             pulumi.set(__self__, "task_role", task_role)
+        if track_latest is not None:
+            pulumi.set(__self__, "track_latest", track_latest)
         if volumes is not None:
             pulumi.set(__self__, "volumes", volumes)
 
     @property
     @pulumi.getter
     def container(self) -> Optional['TaskDefinitionContainerDefinitionArgs']:
         """
@@ -353,14 +357,26 @@
         return pulumi.get(self, "task_role")
 
     @task_role.setter
     def task_role(self, value: Optional['_awsx.DefaultRoleWithPolicyArgs']):
         pulumi.set(self, "task_role", value)
 
     @property
+    @pulumi.getter(name="trackLatest")
+    def track_latest(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether should track latest task definition or the one created with the resource. Default is `false`.
+        """
+        return pulumi.get(self, "track_latest")
+
+    @track_latest.setter
+    def track_latest(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "track_latest", value)
+
+    @property
     @pulumi.getter
     def volumes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]]:
         """
         Configuration block for volumes that containers in your task may use. Detailed below.
         """
         return pulumi.get(self, "volumes")
 
@@ -385,14 +401,15 @@
                  pid_mode: Optional[pulumi.Input[str]] = None,
                  placement_constraints: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionPlacementConstraintArgs']]]] = None,
                  proxy_configuration: Optional[pulumi.Input['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs']] = None,
                  runtime_platform: Optional[pulumi.Input['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs']] = None,
                  skip_destroy: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  task_role: Optional['_awsx.DefaultRoleWithPolicyArgs'] = None,
+                 track_latest: Optional[pulumi.Input[bool]] = None,
                  volumes: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]] = None):
         """
         Create a TaskDefinition resource with the given unique name, arguments, and options.
         Creates required log-group and task & execution roles.
         Presents required Service load balancers if target group included in port mappings.
         :param 'TaskDefinitionContainerDefinitionArgs' container: Single container to make a TaskDefinition from.  Useful for simple cases where there aren't
                multiple containers, especially when creating a TaskDefinition to call [run] on.
@@ -416,14 +433,15 @@
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionPlacementConstraintArgs']]] placement_constraints: Configuration block for rules that are taken into consideration during task placement. Maximum number of `placement_constraints` is `10`. Detailed below.
         :param pulumi.Input['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs'] proxy_configuration: Configuration block for the App Mesh proxy. Detailed below.
         :param pulumi.Input['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs'] runtime_platform: Configuration block for runtime_platform that containers in your task may use.
         :param pulumi.Input[bool] skip_destroy: Whether to retain the old revision when the resource is destroyed or replacement is necessary. Default is `false`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param '_awsx.DefaultRoleWithPolicyArgs' task_role: IAM role that allows your Amazon ECS container task to make calls to other AWS services.
                Will be created automatically if not defined.
+        :param pulumi.Input[bool] track_latest: Whether should track latest task definition or the one created with the resource. Default is `false`.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]] volumes: Configuration block for volumes that containers in your task may use. Detailed below.
         """
         if container is not None:
             pulumi.set(__self__, "container", container)
         if containers is not None:
             pulumi.set(__self__, "containers", containers)
         if cpu is not None:
@@ -452,14 +470,16 @@
             pulumi.set(__self__, "runtime_platform", runtime_platform)
         if skip_destroy is not None:
             pulumi.set(__self__, "skip_destroy", skip_destroy)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if task_role is not None:
             pulumi.set(__self__, "task_role", task_role)
+        if track_latest is not None:
+            pulumi.set(__self__, "track_latest", track_latest)
         if volumes is not None:
             pulumi.set(__self__, "volumes", volumes)
 
     @property
     @pulumi.getter
     def container(self) -> Optional['TaskDefinitionContainerDefinitionArgs']:
         """
@@ -669,14 +689,26 @@
         return pulumi.get(self, "task_role")
 
     @task_role.setter
     def task_role(self, value: Optional['_awsx.DefaultRoleWithPolicyArgs']):
         pulumi.set(self, "task_role", value)
 
     @property
+    @pulumi.getter(name="trackLatest")
+    def track_latest(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether should track latest task definition or the one created with the resource. Default is `false`.
+        """
+        return pulumi.get(self, "track_latest")
+
+    @track_latest.setter
+    def track_latest(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "track_latest", value)
+
+    @property
     @pulumi.getter
     def volumes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]]:
         """
         Configuration block for volumes that containers in your task may use. Detailed below.
         """
         return pulumi.get(self, "volumes")
```

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ecs/ec2_service.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ecs/ec2_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         :param pulumi.Input[str] propagate_tags: Specifies whether to propagate the tags from the task definition or the service to the tasks. The valid values are `SERVICE` and `TASK_DEFINITION`.
         :param pulumi.Input[str] scheduling_strategy: Scheduling strategy to use for the service. The valid values are `REPLICA` and `DAEMON`. Defaults to `REPLICA`. Note that [*Tasks using the Fargate launch type or the `CODE_DEPLOY` or `EXTERNAL` deployment controller types don't support the `DAEMON` scheduling strategy*](https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_CreateService.html).
         :param pulumi.Input['pulumi_aws.ecs.ServiceServiceConnectConfigurationArgs'] service_connect_configuration: The ECS Service Connect configuration for this service to discover and connect to services, and be discovered by, and connected from, other services within a namespace. See below.
         :param pulumi.Input['pulumi_aws.ecs.ServiceServiceRegistriesArgs'] service_registries: Service discovery registries for the service. The maximum number of `service_registries` blocks is `1`. See below.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param pulumi.Input[str] task_definition: Family and revision (`family:revision`) or full ARN of the task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
         :param 'EC2ServiceTaskDefinitionArgs' task_definition_args: The args of task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] triggers: Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `timestamp()`. See example above.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] triggers: Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `plantimestamp()`. See example above.
         """
         if alarms is not None:
             pulumi.set(__self__, "alarms", alarms)
         if cluster is not None:
             pulumi.set(__self__, "cluster", cluster)
         if continue_before_steady_state is not None:
             pulumi.set(__self__, "continue_before_steady_state", continue_before_steady_state)
@@ -446,15 +446,15 @@
     def task_definition_args(self, value: Optional['EC2ServiceTaskDefinitionArgs']):
         pulumi.set(self, "task_definition_args", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `timestamp()`. See example above.
+        Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `plantimestamp()`. See example above.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "triggers", value)
 
@@ -522,15 +522,15 @@
         :param pulumi.Input[str] propagate_tags: Specifies whether to propagate the tags from the task definition or the service to the tasks. The valid values are `SERVICE` and `TASK_DEFINITION`.
         :param pulumi.Input[str] scheduling_strategy: Scheduling strategy to use for the service. The valid values are `REPLICA` and `DAEMON`. Defaults to `REPLICA`. Note that [*Tasks using the Fargate launch type or the `CODE_DEPLOY` or `EXTERNAL` deployment controller types don't support the `DAEMON` scheduling strategy*](https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_CreateService.html).
         :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceServiceConnectConfigurationArgs']] service_connect_configuration: The ECS Service Connect configuration for this service to discover and connect to services, and be discovered by, and connected from, other services within a namespace. See below.
         :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceServiceRegistriesArgs']] service_registries: Service discovery registries for the service. The maximum number of `service_registries` blocks is `1`. See below.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param pulumi.Input[str] task_definition: Family and revision (`family:revision`) or full ARN of the task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
         :param pulumi.InputType['EC2ServiceTaskDefinitionArgs'] task_definition_args: The args of task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] triggers: Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `timestamp()`. See example above.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] triggers: Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `plantimestamp()`. See example above.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[EC2ServiceArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
```

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ecs/ec2_task_definition.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ecs/ec2_task_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,14 +32,15 @@
                  pid_mode: Optional[pulumi.Input[str]] = None,
                  placement_constraints: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionPlacementConstraintArgs']]]] = None,
                  proxy_configuration: Optional[pulumi.Input['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs']] = None,
                  runtime_platform: Optional[pulumi.Input['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs']] = None,
                  skip_destroy: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  task_role: Optional['_awsx.DefaultRoleWithPolicyArgs'] = None,
+                 track_latest: Optional[pulumi.Input[bool]] = None,
                  volumes: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]] = None):
         """
         The set of arguments for constructing a EC2TaskDefinition resource.
         :param 'TaskDefinitionContainerDefinitionArgs' container: Single container to make a TaskDefinition from.  Useful for simple cases where there aren't
                multiple containers, especially when creating a TaskDefinition to call [run] on.
                
                Either [container] or [containers] must be provided.
@@ -62,14 +63,15 @@
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionPlacementConstraintArgs']]] placement_constraints: Configuration block for rules that are taken into consideration during task placement. Maximum number of `placement_constraints` is `10`. Detailed below.
         :param pulumi.Input['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs'] proxy_configuration: Configuration block for the App Mesh proxy. Detailed below.
         :param pulumi.Input['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs'] runtime_platform: Configuration block for runtime_platform that containers in your task may use.
         :param pulumi.Input[bool] skip_destroy: Whether to retain the old revision when the resource is destroyed or replacement is necessary. Default is `false`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param '_awsx.DefaultRoleWithPolicyArgs' task_role: IAM role that allows your Amazon ECS container task to make calls to other AWS services.
                Will be created automatically if not defined.
+        :param pulumi.Input[bool] track_latest: Whether should track latest task definition or the one created with the resource. Default is `false`.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]] volumes: Configuration block for volumes that containers in your task may use. Detailed below.
         """
         if container is not None:
             pulumi.set(__self__, "container", container)
         if containers is not None:
             pulumi.set(__self__, "containers", containers)
         if cpu is not None:
@@ -100,14 +102,16 @@
             pulumi.set(__self__, "runtime_platform", runtime_platform)
         if skip_destroy is not None:
             pulumi.set(__self__, "skip_destroy", skip_destroy)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if task_role is not None:
             pulumi.set(__self__, "task_role", task_role)
+        if track_latest is not None:
+            pulumi.set(__self__, "track_latest", track_latest)
         if volumes is not None:
             pulumi.set(__self__, "volumes", volumes)
 
     @property
     @pulumi.getter
     def container(self) -> Optional['TaskDefinitionContainerDefinitionArgs']:
         """
@@ -329,14 +333,26 @@
         return pulumi.get(self, "task_role")
 
     @task_role.setter
     def task_role(self, value: Optional['_awsx.DefaultRoleWithPolicyArgs']):
         pulumi.set(self, "task_role", value)
 
     @property
+    @pulumi.getter(name="trackLatest")
+    def track_latest(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether should track latest task definition or the one created with the resource. Default is `false`.
+        """
+        return pulumi.get(self, "track_latest")
+
+    @track_latest.setter
+    def track_latest(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "track_latest", value)
+
+    @property
     @pulumi.getter
     def volumes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]]:
         """
         Configuration block for volumes that containers in your task may use. Detailed below.
         """
         return pulumi.get(self, "volumes")
 
@@ -364,14 +380,15 @@
                  pid_mode: Optional[pulumi.Input[str]] = None,
                  placement_constraints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionPlacementConstraintArgs']]]]] = None,
                  proxy_configuration: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs']]] = None,
                  runtime_platform: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs']]] = None,
                  skip_destroy: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  task_role: Optional[pulumi.InputType['_awsx.DefaultRoleWithPolicyArgs']] = None,
+                 track_latest: Optional[pulumi.Input[bool]] = None,
                  volumes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]]] = None,
                  __props__=None):
         """
         Create a TaskDefinition resource with the given unique name, arguments, and options.
         Creates required log-group and task & execution roles.
         Presents required Service load balancers if target group included in port mappings.
 
@@ -400,14 +417,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionPlacementConstraintArgs']]]] placement_constraints: Configuration block for rules that are taken into consideration during task placement. Maximum number of `placement_constraints` is `10`. Detailed below.
         :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs']] proxy_configuration: Configuration block for the App Mesh proxy. Detailed below.
         :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs']] runtime_platform: Configuration block for runtime_platform that containers in your task may use.
         :param pulumi.Input[bool] skip_destroy: Whether to retain the old revision when the resource is destroyed or replacement is necessary. Default is `false`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param pulumi.InputType['_awsx.DefaultRoleWithPolicyArgs'] task_role: IAM role that allows your Amazon ECS container task to make calls to other AWS services.
                Will be created automatically if not defined.
+        :param pulumi.Input[bool] track_latest: Whether should track latest task definition or the one created with the resource. Default is `false`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]] volumes: Configuration block for volumes that containers in your task may use. Detailed below.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[EC2TaskDefinitionArgs] = None,
@@ -446,14 +464,15 @@
                  pid_mode: Optional[pulumi.Input[str]] = None,
                  placement_constraints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionPlacementConstraintArgs']]]]] = None,
                  proxy_configuration: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs']]] = None,
                  runtime_platform: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs']]] = None,
                  skip_destroy: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  task_role: Optional[pulumi.InputType['_awsx.DefaultRoleWithPolicyArgs']] = None,
+                 track_latest: Optional[pulumi.Input[bool]] = None,
                  volumes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
@@ -476,14 +495,15 @@
             __props__.__dict__["pid_mode"] = pid_mode
             __props__.__dict__["placement_constraints"] = placement_constraints
             __props__.__dict__["proxy_configuration"] = proxy_configuration
             __props__.__dict__["runtime_platform"] = runtime_platform
             __props__.__dict__["skip_destroy"] = skip_destroy
             __props__.__dict__["tags"] = tags
             __props__.__dict__["task_role"] = task_role
+            __props__.__dict__["track_latest"] = track_latest
             __props__.__dict__["volumes"] = volumes
             __props__.__dict__["load_balancers"] = None
             __props__.__dict__["task_definition"] = None
         super(EC2TaskDefinition, __self__).__init__(
             'awsx:ecs:EC2TaskDefinition',
             resource_name,
             __props__,
```

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ecs/fargate_service.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ecs/fargate_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -71,15 +71,15 @@
         :param pulumi.Input[str] propagate_tags: Specifies whether to propagate the tags from the task definition or the service to the tasks. The valid values are `SERVICE` and `TASK_DEFINITION`.
         :param pulumi.Input[str] scheduling_strategy: Scheduling strategy to use for the service. The valid values are `REPLICA` and `DAEMON`. Defaults to `REPLICA`. Note that [*Tasks using the Fargate launch type or the `CODE_DEPLOY` or `EXTERNAL` deployment controller types don't support the `DAEMON` scheduling strategy*](https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_CreateService.html).
         :param pulumi.Input['pulumi_aws.ecs.ServiceServiceConnectConfigurationArgs'] service_connect_configuration: The ECS Service Connect configuration for this service to discover and connect to services, and be discovered by, and connected from, other services within a namespace. See below.
         :param pulumi.Input['pulumi_aws.ecs.ServiceServiceRegistriesArgs'] service_registries: Service discovery registries for the service. The maximum number of `service_registries` blocks is `1`. See below.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param pulumi.Input[str] task_definition: Family and revision (`family:revision`) or full ARN of the task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
         :param 'FargateServiceTaskDefinitionArgs' task_definition_args: The args of task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] triggers: Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `timestamp()`. See example above.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] triggers: Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `plantimestamp()`. See example above.
         """
         if alarms is not None:
             pulumi.set(__self__, "alarms", alarms)
         if assign_public_ip is not None:
             pulumi.set(__self__, "assign_public_ip", assign_public_ip)
         if cluster is not None:
             pulumi.set(__self__, "cluster", cluster)
@@ -446,15 +446,15 @@
     def task_definition_args(self, value: Optional['FargateServiceTaskDefinitionArgs']):
         pulumi.set(self, "task_definition_args", value)
 
     @property
     @pulumi.getter
     def triggers(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `timestamp()`. See example above.
+        Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `plantimestamp()`. See example above.
         """
         return pulumi.get(self, "triggers")
 
     @triggers.setter
     def triggers(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "triggers", value)
 
@@ -522,15 +522,15 @@
         :param pulumi.Input[str] propagate_tags: Specifies whether to propagate the tags from the task definition or the service to the tasks. The valid values are `SERVICE` and `TASK_DEFINITION`.
         :param pulumi.Input[str] scheduling_strategy: Scheduling strategy to use for the service. The valid values are `REPLICA` and `DAEMON`. Defaults to `REPLICA`. Note that [*Tasks using the Fargate launch type or the `CODE_DEPLOY` or `EXTERNAL` deployment controller types don't support the `DAEMON` scheduling strategy*](https://docs.aws.amazon.com/AmazonECS/latest/APIReference/API_CreateService.html).
         :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceServiceConnectConfigurationArgs']] service_connect_configuration: The ECS Service Connect configuration for this service to discover and connect to services, and be discovered by, and connected from, other services within a namespace. See below.
         :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.ServiceServiceRegistriesArgs']] service_registries: Service discovery registries for the service. The maximum number of `service_registries` blocks is `1`. See below.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param pulumi.Input[str] task_definition: Family and revision (`family:revision`) or full ARN of the task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
         :param pulumi.InputType['FargateServiceTaskDefinitionArgs'] task_definition_args: The args of task definition that you want to run in your service. Either [taskDefinition] or [taskDefinitionArgs] must be provided.
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] triggers: Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `timestamp()`. See example above.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] triggers: Map of arbitrary keys and values that, when changed, will trigger an in-place update (redeployment). Useful with `plantimestamp()`. See example above.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[FargateServiceArgs] = None,
                  opts: Optional[pulumi.ResourceOptions] = None):
```

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/ecs/fargate_task_definition.py` & `pulumi_awsx-2.9.0/pulumi_awsx/ecs/fargate_task_definition.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
                  pid_mode: Optional[pulumi.Input[str]] = None,
                  placement_constraints: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionPlacementConstraintArgs']]]] = None,
                  proxy_configuration: Optional[pulumi.Input['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs']] = None,
                  runtime_platform: Optional[pulumi.Input['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs']] = None,
                  skip_destroy: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  task_role: Optional['_awsx.DefaultRoleWithPolicyArgs'] = None,
+                 track_latest: Optional[pulumi.Input[bool]] = None,
                  volumes: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]] = None):
         """
         The set of arguments for constructing a FargateTaskDefinition resource.
         :param 'TaskDefinitionContainerDefinitionArgs' container: Single container to make a TaskDefinition from.  Useful for simple cases where there aren't
                multiple containers, especially when creating a TaskDefinition to call [run] on.
                
                Either [container] or [containers] must be provided.
@@ -60,14 +61,15 @@
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionPlacementConstraintArgs']]] placement_constraints: Configuration block for rules that are taken into consideration during task placement. Maximum number of `placement_constraints` is `10`. Detailed below.
         :param pulumi.Input['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs'] proxy_configuration: Configuration block for the App Mesh proxy. Detailed below.
         :param pulumi.Input['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs'] runtime_platform: Configuration block for runtime_platform that containers in your task may use.
         :param pulumi.Input[bool] skip_destroy: Whether to retain the old revision when the resource is destroyed or replacement is necessary. Default is `false`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param '_awsx.DefaultRoleWithPolicyArgs' task_role: IAM role that allows your Amazon ECS container task to make calls to other AWS services.
                Will be created automatically if not defined.
+        :param pulumi.Input[bool] track_latest: Whether should track latest task definition or the one created with the resource. Default is `false`.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]] volumes: Configuration block for volumes that containers in your task may use. Detailed below.
         """
         if container is not None:
             pulumi.set(__self__, "container", container)
         if containers is not None:
             pulumi.set(__self__, "containers", containers)
         if cpu is not None:
@@ -96,14 +98,16 @@
             pulumi.set(__self__, "runtime_platform", runtime_platform)
         if skip_destroy is not None:
             pulumi.set(__self__, "skip_destroy", skip_destroy)
         if tags is not None:
             pulumi.set(__self__, "tags", tags)
         if task_role is not None:
             pulumi.set(__self__, "task_role", task_role)
+        if track_latest is not None:
+            pulumi.set(__self__, "track_latest", track_latest)
         if volumes is not None:
             pulumi.set(__self__, "volumes", volumes)
 
     @property
     @pulumi.getter
     def container(self) -> Optional['TaskDefinitionContainerDefinitionArgs']:
         """
@@ -313,14 +317,26 @@
         return pulumi.get(self, "task_role")
 
     @task_role.setter
     def task_role(self, value: Optional['_awsx.DefaultRoleWithPolicyArgs']):
         pulumi.set(self, "task_role", value)
 
     @property
+    @pulumi.getter(name="trackLatest")
+    def track_latest(self) -> Optional[pulumi.Input[bool]]:
+        """
+        Whether should track latest task definition or the one created with the resource. Default is `false`.
+        """
+        return pulumi.get(self, "track_latest")
+
+    @track_latest.setter
+    def track_latest(self, value: Optional[pulumi.Input[bool]]):
+        pulumi.set(self, "track_latest", value)
+
+    @property
     @pulumi.getter
     def volumes(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]]:
         """
         Configuration block for volumes that containers in your task may use. Detailed below.
         """
         return pulumi.get(self, "volumes")
 
@@ -347,14 +363,15 @@
                  pid_mode: Optional[pulumi.Input[str]] = None,
                  placement_constraints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionPlacementConstraintArgs']]]]] = None,
                  proxy_configuration: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs']]] = None,
                  runtime_platform: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs']]] = None,
                  skip_destroy: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  task_role: Optional[pulumi.InputType['_awsx.DefaultRoleWithPolicyArgs']] = None,
+                 track_latest: Optional[pulumi.Input[bool]] = None,
                  volumes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]]] = None,
                  __props__=None):
         """
         Create a TaskDefinition resource with the given unique name, arguments, and options.
         Creates required log-group and task & execution roles.
         Presents required Service load balancers if target group included in port mappings.
 
@@ -382,14 +399,15 @@
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionPlacementConstraintArgs']]]] placement_constraints: Configuration block for rules that are taken into consideration during task placement. Maximum number of `placement_constraints` is `10`. Detailed below.
         :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs']] proxy_configuration: Configuration block for the App Mesh proxy. Detailed below.
         :param pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs']] runtime_platform: Configuration block for runtime_platform that containers in your task may use.
         :param pulumi.Input[bool] skip_destroy: Whether to retain the old revision when the resource is destroyed or replacement is necessary. Default is `false`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Key-value map of resource tags. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param pulumi.InputType['_awsx.DefaultRoleWithPolicyArgs'] task_role: IAM role that allows your Amazon ECS container task to make calls to other AWS services.
                Will be created automatically if not defined.
+        :param pulumi.Input[bool] track_latest: Whether should track latest task definition or the one created with the resource. Default is `false`.
         :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]] volumes: Configuration block for volumes that containers in your task may use. Detailed below.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[FargateTaskDefinitionArgs] = None,
@@ -427,14 +445,15 @@
                  pid_mode: Optional[pulumi.Input[str]] = None,
                  placement_constraints: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionPlacementConstraintArgs']]]]] = None,
                  proxy_configuration: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionProxyConfigurationArgs']]] = None,
                  runtime_platform: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionRuntimePlatformArgs']]] = None,
                  skip_destroy: Optional[pulumi.Input[bool]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  task_role: Optional[pulumi.InputType['_awsx.DefaultRoleWithPolicyArgs']] = None,
+                 track_latest: Optional[pulumi.Input[bool]] = None,
                  volumes: Optional[pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.ecs.TaskDefinitionVolumeArgs']]]]] = None,
                  __props__=None):
         opts = pulumi.ResourceOptions.merge(_utilities.get_resource_opts_defaults(), opts)
         if not isinstance(opts, pulumi.ResourceOptions):
             raise TypeError('Expected resource options to be a ResourceOptions instance')
         if opts.id is not None:
             raise ValueError('ComponentResource classes do not support opts.id')
@@ -456,14 +475,15 @@
             __props__.__dict__["pid_mode"] = pid_mode
             __props__.__dict__["placement_constraints"] = placement_constraints
             __props__.__dict__["proxy_configuration"] = proxy_configuration
             __props__.__dict__["runtime_platform"] = runtime_platform
             __props__.__dict__["skip_destroy"] = skip_destroy
             __props__.__dict__["tags"] = tags
             __props__.__dict__["task_role"] = task_role
+            __props__.__dict__["track_latest"] = track_latest
             __props__.__dict__["volumes"] = volumes
             __props__.__dict__["load_balancers"] = None
             __props__.__dict__["task_definition"] = None
         super(FargateTaskDefinition, __self__).__init__(
             'awsx:ecs:FargateTaskDefinition',
             resource_name,
             __props__,
```

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/lb/_inputs.py` & `pulumi_awsx-2.9.0/pulumi_awsx/lb/_inputs.py`

 * *Files 8% similar despite different names*

```diff
@@ -17,58 +17,55 @@
 
 @pulumi.input_type
 class ListenerArgs:
     def __init__(__self__, *,
                  alpn_policy: Optional[pulumi.Input[str]] = None,
                  certificate_arn: Optional[pulumi.Input[str]] = None,
                  default_actions: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.ListenerDefaultActionArgs']]]] = None,
+                 mutual_authentication: Optional[pulumi.Input['pulumi_aws.lb.ListenerMutualAuthenticationArgs']] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  ssl_policy: Optional[pulumi.Input[str]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None):
         """
         Provides a Load Balancer Listener resource.
 
         > **Note:** `aws.alb.Listener` is known as `aws.lb.Listener`. The functionality is identical.
 
-        {{% examples %}}
         ## Example Usage
-        {{% example %}}
+
         ### Forward Action
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
-        const frontEndLoadBalancer = new aws.lb.LoadBalancer("frontEndLoadBalancer", {});
-        // ...
-        const frontEndTargetGroup = new aws.lb.TargetGroup("frontEndTargetGroup", {});
-        // ...
-        const frontEndListener = new aws.lb.Listener("frontEndListener", {
-            loadBalancerArn: frontEndLoadBalancer.arn,
+        const frontEnd = new aws.lb.LoadBalancer("front_end", {});
+        const frontEndTargetGroup = new aws.lb.TargetGroup("front_end", {});
+        const frontEndListener = new aws.lb.Listener("front_end", {
+            loadBalancerArn: frontEnd.arn,
             port: 443,
             protocol: "HTTPS",
             sslPolicy: "ELBSecurityPolicy-2016-08",
             certificateArn: "arn:aws:iam::187416307283:server-certificate/test_cert_rab3wuqwgja25ct3n4jdj2tzu4",
             defaultActions: [{
                 type: "forward",
                 targetGroupArn: frontEndTargetGroup.arn,
             }],
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
-        front_end_load_balancer = aws.lb.LoadBalancer("frontEndLoadBalancer")
-        # ...
-        front_end_target_group = aws.lb.TargetGroup("frontEndTargetGroup")
-        # ...
-        front_end_listener = aws.lb.Listener("frontEndListener",
-            load_balancer_arn=front_end_load_balancer.arn,
+        front_end = aws.lb.LoadBalancer("front_end")
+        front_end_target_group = aws.lb.TargetGroup("front_end")
+        front_end_listener = aws.lb.Listener("front_end",
+            load_balancer_arn=front_end.arn,
             port=443,
             protocol="HTTPS",
             ssl_policy="ELBSecurityPolicy-2016-08",
             certificate_arn="arn:aws:iam::187416307283:server-certificate/test_cert_rab3wuqwgja25ct3n4jdj2tzu4",
             default_actions=[aws.lb.ListenerDefaultActionArgs(
                 type="forward",
                 target_group_arn=front_end_target_group.arn,
@@ -78,23 +75,21 @@
         using System.Collections.Generic;
         using System.Linq;
         using Pulumi;
         using Aws = Pulumi.Aws;
 
         return await Deployment.RunAsync(() => 
         {
-            var frontEndLoadBalancer = new Aws.LB.LoadBalancer("frontEndLoadBalancer");
+            var frontEnd = new Aws.LB.LoadBalancer("front_end");
 
-            // ...
-            var frontEndTargetGroup = new Aws.LB.TargetGroup("frontEndTargetGroup");
+            var frontEndTargetGroup = new Aws.LB.TargetGroup("front_end");
 
-            // ...
-            var frontEndListener = new Aws.LB.Listener("frontEndListener", new()
+            var frontEndListener = new Aws.LB.Listener("front_end", new()
             {
-                LoadBalancerArn = frontEndLoadBalancer.Arn,
+                LoadBalancerArn = frontEnd.Arn,
                 Port = 443,
                 Protocol = "HTTPS",
                 SslPolicy = "ELBSecurityPolicy-2016-08",
                 CertificateArn = "arn:aws:iam::187416307283:server-certificate/test_cert_rab3wuqwgja25ct3n4jdj2tzu4",
                 DefaultActions = new[]
                 {
                     new Aws.LB.Inputs.ListenerDefaultActionArgs
@@ -113,24 +108,24 @@
         import (
         	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/lb"
         	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
         )
 
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
-        		frontEndLoadBalancer, err := lb.NewLoadBalancer(ctx, "frontEndLoadBalancer", nil)
+        		frontEnd, err := lb.NewLoadBalancer(ctx, "front_end", nil)
         		if err != nil {
         			return err
         		}
-        		frontEndTargetGroup, err := lb.NewTargetGroup(ctx, "frontEndTargetGroup", nil)
+        		frontEndTargetGroup, err := lb.NewTargetGroup(ctx, "front_end", nil)
         		if err != nil {
         			return err
         		}
-        		_, err = lb.NewListener(ctx, "frontEndListener", &lb.ListenerArgs{
-        			LoadBalancerArn: frontEndLoadBalancer.Arn,
+        		_, err = lb.NewListener(ctx, "front_end", &lb.ListenerArgs{
+        			LoadBalancerArn: frontEnd.Arn,
         			Port:            pulumi.Int(443),
         			Protocol:        pulumi.String("HTTPS"),
         			SslPolicy:       pulumi.String("ELBSecurityPolicy-2016-08"),
         			CertificateArn:  pulumi.String("arn:aws:iam::187416307283:server-certificate/test_cert_rab3wuqwgja25ct3n4jdj2tzu4"),
         			DefaultActions: lb.ListenerDefaultActionArray{
         				&lb.ListenerDefaultActionArgs{
         					Type:           pulumi.String("forward"),
@@ -165,20 +160,20 @@
 
         public class App {
             public static void main(String[] args) {
                 Pulumi.run(App::stack);
             }
 
             public static void stack(Context ctx) {
-                var frontEndLoadBalancer = new LoadBalancer("frontEndLoadBalancer");
+                var frontEnd = new LoadBalancer("frontEnd");
 
                 var frontEndTargetGroup = new TargetGroup("frontEndTargetGroup");
 
                 var frontEndListener = new Listener("frontEndListener", ListenerArgs.builder()        
-                    .loadBalancerArn(frontEndLoadBalancer.arn())
+                    .loadBalancerArn(frontEnd.arn())
                     .port("443")
                     .protocol("HTTPS")
                     .sslPolicy("ELBSecurityPolicy-2016-08")
                     .certificateArn("arn:aws:iam::187416307283:server-certificate/test_cert_rab3wuqwgja25ct3n4jdj2tzu4")
                     .defaultActions(ListenerDefaultActionArgs.builder()
                         .type("forward")
                         .targetGroupArn(frontEndTargetGroup.arn())
@@ -186,85 +181,90 @@
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
-          frontEndLoadBalancer:
+          frontEnd:
             type: aws:lb:LoadBalancer
+            name: front_end
           frontEndTargetGroup:
             type: aws:lb:TargetGroup
+            name: front_end
           frontEndListener:
             type: aws:lb:Listener
+            name: front_end
             properties:
-              loadBalancerArn: ${frontEndLoadBalancer.arn}
+              loadBalancerArn: ${frontEnd.arn}
               port: '443'
               protocol: HTTPS
               sslPolicy: ELBSecurityPolicy-2016-08
               certificateArn: arn:aws:iam::187416307283:server-certificate/test_cert_rab3wuqwgja25ct3n4jdj2tzu4
               defaultActions:
                 - type: forward
                   targetGroupArn: ${frontEndTargetGroup.arn}
         ```
+        <!--End PulumiCodeChooser -->
 
         To a NLB:
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
-        const frontEnd = new aws.lb.Listener("frontEnd", {
-            loadBalancerArn: aws_lb.front_end.arn,
+        const frontEnd = new aws.lb.Listener("front_end", {
+            loadBalancerArn: frontEndAwsLb.arn,
             port: 443,
             protocol: "TLS",
             certificateArn: "arn:aws:iam::187416307283:server-certificate/test_cert_rab3wuqwgja25ct3n4jdj2tzu4",
             alpnPolicy: "HTTP2Preferred",
             defaultActions: [{
                 type: "forward",
-                targetGroupArn: aws_lb_target_group.front_end.arn,
+                targetGroupArn: frontEndAwsLbTargetGroup.arn,
             }],
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
-        front_end = aws.lb.Listener("frontEnd",
-            load_balancer_arn=aws_lb["front_end"]["arn"],
+        front_end = aws.lb.Listener("front_end",
+            load_balancer_arn=front_end_aws_lb["arn"],
             port=443,
             protocol="TLS",
             certificate_arn="arn:aws:iam::187416307283:server-certificate/test_cert_rab3wuqwgja25ct3n4jdj2tzu4",
             alpn_policy="HTTP2Preferred",
             default_actions=[aws.lb.ListenerDefaultActionArgs(
                 type="forward",
-                target_group_arn=aws_lb_target_group["front_end"]["arn"],
+                target_group_arn=front_end_aws_lb_target_group["arn"],
             )])
         ```
         ```csharp
         using System.Collections.Generic;
         using System.Linq;
         using Pulumi;
         using Aws = Pulumi.Aws;
 
         return await Deployment.RunAsync(() => 
         {
-            var frontEnd = new Aws.LB.Listener("frontEnd", new()
+            var frontEnd = new Aws.LB.Listener("front_end", new()
             {
-                LoadBalancerArn = aws_lb.Front_end.Arn,
+                LoadBalancerArn = frontEndAwsLb.Arn,
                 Port = 443,
                 Protocol = "TLS",
                 CertificateArn = "arn:aws:iam::187416307283:server-certificate/test_cert_rab3wuqwgja25ct3n4jdj2tzu4",
                 AlpnPolicy = "HTTP2Preferred",
                 DefaultActions = new[]
                 {
                     new Aws.LB.Inputs.ListenerDefaultActionArgs
                     {
                         Type = "forward",
-                        TargetGroupArn = aws_lb_target_group.Front_end.Arn,
+                        TargetGroupArn = frontEndAwsLbTargetGroup.Arn,
                     },
                 },
             });
 
         });
         ```
         ```go
@@ -273,24 +273,24 @@
         import (
         	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/lb"
         	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
         )
 
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
-        		_, err := lb.NewListener(ctx, "frontEnd", &lb.ListenerArgs{
-        			LoadBalancerArn: pulumi.Any(aws_lb.Front_end.Arn),
+        		_, err := lb.NewListener(ctx, "front_end", &lb.ListenerArgs{
+        			LoadBalancerArn: pulumi.Any(frontEndAwsLb.Arn),
         			Port:            pulumi.Int(443),
         			Protocol:        pulumi.String("TLS"),
         			CertificateArn:  pulumi.String("arn:aws:iam::187416307283:server-certificate/test_cert_rab3wuqwgja25ct3n4jdj2tzu4"),
         			AlpnPolicy:      pulumi.String("HTTP2Preferred"),
         			DefaultActions: lb.ListenerDefaultActionArray{
         				&lb.ListenerDefaultActionArgs{
         					Type:           pulumi.String("forward"),
-        					TargetGroupArn: pulumi.Any(aws_lb_target_group.Front_end.Arn),
+        					TargetGroupArn: pulumi.Any(frontEndAwsLbTargetGroup.Arn),
         				},
         			},
         		})
         		if err != nil {
         			return err
         		}
         		return nil
@@ -316,54 +316,55 @@
         public class App {
             public static void main(String[] args) {
                 Pulumi.run(App::stack);
             }
 
             public static void stack(Context ctx) {
                 var frontEnd = new Listener("frontEnd", ListenerArgs.builder()        
-                    .loadBalancerArn(aws_lb.front_end().arn())
+                    .loadBalancerArn(frontEndAwsLb.arn())
                     .port("443")
                     .protocol("TLS")
                     .certificateArn("arn:aws:iam::187416307283:server-certificate/test_cert_rab3wuqwgja25ct3n4jdj2tzu4")
                     .alpnPolicy("HTTP2Preferred")
                     .defaultActions(ListenerDefaultActionArgs.builder()
                         .type("forward")
-                        .targetGroupArn(aws_lb_target_group.front_end().arn())
+                        .targetGroupArn(frontEndAwsLbTargetGroup.arn())
                         .build())
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
           frontEnd:
             type: aws:lb:Listener
+            name: front_end
             properties:
-              loadBalancerArn: ${aws_lb.front_end.arn}
+              loadBalancerArn: ${frontEndAwsLb.arn}
               port: '443'
               protocol: TLS
               certificateArn: arn:aws:iam::187416307283:server-certificate/test_cert_rab3wuqwgja25ct3n4jdj2tzu4
               alpnPolicy: HTTP2Preferred
               defaultActions:
                 - type: forward
-                  targetGroupArn: ${aws_lb_target_group.front_end.arn}
+                  targetGroupArn: ${frontEndAwsLbTargetGroup.arn}
         ```
-        {{% /example %}}
-        {{% example %}}
+        <!--End PulumiCodeChooser -->
+
         ### Redirect Action
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
-        const frontEndLoadBalancer = new aws.lb.LoadBalancer("frontEndLoadBalancer", {});
-        // ...
-        const frontEndListener = new aws.lb.Listener("frontEndListener", {
-            loadBalancerArn: frontEndLoadBalancer.arn,
+        const frontEnd = new aws.lb.LoadBalancer("front_end", {});
+        const frontEndListener = new aws.lb.Listener("front_end", {
+            loadBalancerArn: frontEnd.arn,
             port: 80,
             protocol: "HTTP",
             defaultActions: [{
                 type: "redirect",
                 redirect: {
                     port: "443",
                     protocol: "HTTPS",
@@ -372,18 +373,17 @@
             }],
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
-        front_end_load_balancer = aws.lb.LoadBalancer("frontEndLoadBalancer")
-        # ...
-        front_end_listener = aws.lb.Listener("frontEndListener",
-            load_balancer_arn=front_end_load_balancer.arn,
+        front_end = aws.lb.LoadBalancer("front_end")
+        front_end_listener = aws.lb.Listener("front_end",
+            load_balancer_arn=front_end.arn,
             port=80,
             protocol="HTTP",
             default_actions=[aws.lb.ListenerDefaultActionArgs(
                 type="redirect",
                 redirect=aws.lb.ListenerDefaultActionRedirectArgs(
                     port="443",
                     protocol="HTTPS",
@@ -395,20 +395,19 @@
         using System.Collections.Generic;
         using System.Linq;
         using Pulumi;
         using Aws = Pulumi.Aws;
 
         return await Deployment.RunAsync(() => 
         {
-            var frontEndLoadBalancer = new Aws.LB.LoadBalancer("frontEndLoadBalancer");
+            var frontEnd = new Aws.LB.LoadBalancer("front_end");
 
-            // ...
-            var frontEndListener = new Aws.LB.Listener("frontEndListener", new()
+            var frontEndListener = new Aws.LB.Listener("front_end", new()
             {
-                LoadBalancerArn = frontEndLoadBalancer.Arn,
+                LoadBalancerArn = frontEnd.Arn,
                 Port = 80,
                 Protocol = "HTTP",
                 DefaultActions = new[]
                 {
                     new Aws.LB.Inputs.ListenerDefaultActionArgs
                     {
                         Type = "redirect",
@@ -430,20 +429,20 @@
         import (
         	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/lb"
         	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
         )
 
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
-        		frontEndLoadBalancer, err := lb.NewLoadBalancer(ctx, "frontEndLoadBalancer", nil)
+        		frontEnd, err := lb.NewLoadBalancer(ctx, "front_end", nil)
         		if err != nil {
         			return err
         		}
-        		_, err = lb.NewListener(ctx, "frontEndListener", &lb.ListenerArgs{
-        			LoadBalancerArn: frontEndLoadBalancer.Arn,
+        		_, err = lb.NewListener(ctx, "front_end", &lb.ListenerArgs{
+        			LoadBalancerArn: frontEnd.Arn,
         			Port:            pulumi.Int(80),
         			Protocol:        pulumi.String("HTTP"),
         			DefaultActions: lb.ListenerDefaultActionArray{
         				&lb.ListenerDefaultActionArgs{
         					Type: pulumi.String("redirect"),
         					Redirect: &lb.ListenerDefaultActionRedirectArgs{
         						Port:       pulumi.String("443"),
@@ -480,18 +479,18 @@
 
         public class App {
             public static void main(String[] args) {
                 Pulumi.run(App::stack);
             }
 
             public static void stack(Context ctx) {
-                var frontEndLoadBalancer = new LoadBalancer("frontEndLoadBalancer");
+                var frontEnd = new LoadBalancer("frontEnd");
 
                 var frontEndListener = new Listener("frontEndListener", ListenerArgs.builder()        
-                    .loadBalancerArn(frontEndLoadBalancer.arn())
+                    .loadBalancerArn(frontEnd.arn())
                     .port("80")
                     .protocol("HTTP")
                     .defaultActions(ListenerDefaultActionArgs.builder()
                         .type("redirect")
                         .redirect(ListenerDefaultActionRedirectArgs.builder()
                             .port("443")
                             .protocol("HTTPS")
@@ -501,41 +500,43 @@
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
-          frontEndLoadBalancer:
+          frontEnd:
             type: aws:lb:LoadBalancer
+            name: front_end
           frontEndListener:
             type: aws:lb:Listener
+            name: front_end
             properties:
-              loadBalancerArn: ${frontEndLoadBalancer.arn}
+              loadBalancerArn: ${frontEnd.arn}
               port: '80'
               protocol: HTTP
               defaultActions:
                 - type: redirect
                   redirect:
                     port: '443'
                     protocol: HTTPS
                     statusCode: HTTP_301
         ```
-        {{% /example %}}
-        {{% example %}}
+        <!--End PulumiCodeChooser -->
+
         ### Fixed-response Action
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
-        const frontEndLoadBalancer = new aws.lb.LoadBalancer("frontEndLoadBalancer", {});
-        // ...
-        const frontEndListener = new aws.lb.Listener("frontEndListener", {
-            loadBalancerArn: frontEndLoadBalancer.arn,
+        const frontEnd = new aws.lb.LoadBalancer("front_end", {});
+        const frontEndListener = new aws.lb.Listener("front_end", {
+            loadBalancerArn: frontEnd.arn,
             port: 80,
             protocol: "HTTP",
             defaultActions: [{
                 type: "fixed-response",
                 fixedResponse: {
                     contentType: "text/plain",
                     messageBody: "Fixed response content",
@@ -544,18 +545,17 @@
             }],
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
-        front_end_load_balancer = aws.lb.LoadBalancer("frontEndLoadBalancer")
-        # ...
-        front_end_listener = aws.lb.Listener("frontEndListener",
-            load_balancer_arn=front_end_load_balancer.arn,
+        front_end = aws.lb.LoadBalancer("front_end")
+        front_end_listener = aws.lb.Listener("front_end",
+            load_balancer_arn=front_end.arn,
             port=80,
             protocol="HTTP",
             default_actions=[aws.lb.ListenerDefaultActionArgs(
                 type="fixed-response",
                 fixed_response=aws.lb.ListenerDefaultActionFixedResponseArgs(
                     content_type="text/plain",
                     message_body="Fixed response content",
@@ -567,20 +567,19 @@
         using System.Collections.Generic;
         using System.Linq;
         using Pulumi;
         using Aws = Pulumi.Aws;
 
         return await Deployment.RunAsync(() => 
         {
-            var frontEndLoadBalancer = new Aws.LB.LoadBalancer("frontEndLoadBalancer");
+            var frontEnd = new Aws.LB.LoadBalancer("front_end");
 
-            // ...
-            var frontEndListener = new Aws.LB.Listener("frontEndListener", new()
+            var frontEndListener = new Aws.LB.Listener("front_end", new()
             {
-                LoadBalancerArn = frontEndLoadBalancer.Arn,
+                LoadBalancerArn = frontEnd.Arn,
                 Port = 80,
                 Protocol = "HTTP",
                 DefaultActions = new[]
                 {
                     new Aws.LB.Inputs.ListenerDefaultActionArgs
                     {
                         Type = "fixed-response",
@@ -602,20 +601,20 @@
         import (
         	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/lb"
         	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
         )
 
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
-        		frontEndLoadBalancer, err := lb.NewLoadBalancer(ctx, "frontEndLoadBalancer", nil)
+        		frontEnd, err := lb.NewLoadBalancer(ctx, "front_end", nil)
         		if err != nil {
         			return err
         		}
-        		_, err = lb.NewListener(ctx, "frontEndListener", &lb.ListenerArgs{
-        			LoadBalancerArn: frontEndLoadBalancer.Arn,
+        		_, err = lb.NewListener(ctx, "front_end", &lb.ListenerArgs{
+        			LoadBalancerArn: frontEnd.Arn,
         			Port:            pulumi.Int(80),
         			Protocol:        pulumi.String("HTTP"),
         			DefaultActions: lb.ListenerDefaultActionArray{
         				&lb.ListenerDefaultActionArgs{
         					Type: pulumi.String("fixed-response"),
         					FixedResponse: &lb.ListenerDefaultActionFixedResponseArgs{
         						ContentType: pulumi.String("text/plain"),
@@ -652,18 +651,18 @@
 
         public class App {
             public static void main(String[] args) {
                 Pulumi.run(App::stack);
             }
 
             public static void stack(Context ctx) {
-                var frontEndLoadBalancer = new LoadBalancer("frontEndLoadBalancer");
+                var frontEnd = new LoadBalancer("frontEnd");
 
                 var frontEndListener = new Listener("frontEndListener", ListenerArgs.builder()        
-                    .loadBalancerArn(frontEndLoadBalancer.arn())
+                    .loadBalancerArn(frontEnd.arn())
                     .port("80")
                     .protocol("HTTP")
                     .defaultActions(ListenerDefaultActionArgs.builder()
                         .type("fixed-response")
                         .fixedResponse(ListenerDefaultActionFixedResponseArgs.builder()
                             .contentType("text/plain")
                             .messageBody("Fixed response content")
@@ -673,49 +672,47 @@
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
-          frontEndLoadBalancer:
+          frontEnd:
             type: aws:lb:LoadBalancer
+            name: front_end
           frontEndListener:
             type: aws:lb:Listener
+            name: front_end
             properties:
-              loadBalancerArn: ${frontEndLoadBalancer.arn}
+              loadBalancerArn: ${frontEnd.arn}
               port: '80'
               protocol: HTTP
               defaultActions:
                 - type: fixed-response
                   fixedResponse:
                     contentType: text/plain
                     messageBody: Fixed response content
                     statusCode: '200'
         ```
-        {{% /example %}}
-        {{% example %}}
+        <!--End PulumiCodeChooser -->
+
         ### Authenticate-cognito Action
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
-        const frontEndLoadBalancer = new aws.lb.LoadBalancer("frontEndLoadBalancer", {});
-        // ...
-        const frontEndTargetGroup = new aws.lb.TargetGroup("frontEndTargetGroup", {});
-        // ...
+        const frontEnd = new aws.lb.LoadBalancer("front_end", {});
+        const frontEndTargetGroup = new aws.lb.TargetGroup("front_end", {});
         const pool = new aws.cognito.UserPool("pool", {});
-        // ...
         const client = new aws.cognito.UserPoolClient("client", {});
-        // ...
         const domain = new aws.cognito.UserPoolDomain("domain", {});
-        // ...
-        const frontEndListener = new aws.lb.Listener("frontEndListener", {
-            loadBalancerArn: frontEndLoadBalancer.arn,
+        const frontEndListener = new aws.lb.Listener("front_end", {
+            loadBalancerArn: frontEnd.arn,
             port: 80,
             protocol: "HTTP",
             defaultActions: [
                 {
                     type: "authenticate-cognito",
                     authenticateCognito: {
                         userPoolArn: pool.arn,
@@ -730,26 +727,21 @@
             ],
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
-        front_end_load_balancer = aws.lb.LoadBalancer("frontEndLoadBalancer")
-        # ...
-        front_end_target_group = aws.lb.TargetGroup("frontEndTargetGroup")
-        # ...
+        front_end = aws.lb.LoadBalancer("front_end")
+        front_end_target_group = aws.lb.TargetGroup("front_end")
         pool = aws.cognito.UserPool("pool")
-        # ...
         client = aws.cognito.UserPoolClient("client")
-        # ...
         domain = aws.cognito.UserPoolDomain("domain")
-        # ...
-        front_end_listener = aws.lb.Listener("frontEndListener",
-            load_balancer_arn=front_end_load_balancer.arn,
+        front_end_listener = aws.lb.Listener("front_end",
+            load_balancer_arn=front_end.arn,
             port=80,
             protocol="HTTP",
             default_actions=[
                 aws.lb.ListenerDefaultActionArgs(
                     type="authenticate-cognito",
                     authenticate_cognito=aws.lb.ListenerDefaultActionAuthenticateCognitoArgs(
                         user_pool_arn=pool.arn,
@@ -767,32 +759,27 @@
         using System.Collections.Generic;
         using System.Linq;
         using Pulumi;
         using Aws = Pulumi.Aws;
 
         return await Deployment.RunAsync(() => 
         {
-            var frontEndLoadBalancer = new Aws.LB.LoadBalancer("frontEndLoadBalancer");
+            var frontEnd = new Aws.LB.LoadBalancer("front_end");
 
-            // ...
-            var frontEndTargetGroup = new Aws.LB.TargetGroup("frontEndTargetGroup");
+            var frontEndTargetGroup = new Aws.LB.TargetGroup("front_end");
 
-            // ...
             var pool = new Aws.Cognito.UserPool("pool");
 
-            // ...
             var client = new Aws.Cognito.UserPoolClient("client");
 
-            // ...
             var domain = new Aws.Cognito.UserPoolDomain("domain");
 
-            // ...
-            var frontEndListener = new Aws.LB.Listener("frontEndListener", new()
+            var frontEndListener = new Aws.LB.Listener("front_end", new()
             {
-                LoadBalancerArn = frontEndLoadBalancer.Arn,
+                LoadBalancerArn = frontEnd.Arn,
                 Port = 80,
                 Protocol = "HTTP",
                 DefaultActions = new[]
                 {
                     new Aws.LB.Inputs.ListenerDefaultActionArgs
                     {
                         Type = "authenticate-cognito",
@@ -820,19 +807,19 @@
         	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/cognito"
         	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/lb"
         	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
         )
 
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
-        		frontEndLoadBalancer, err := lb.NewLoadBalancer(ctx, "frontEndLoadBalancer", nil)
+        		frontEnd, err := lb.NewLoadBalancer(ctx, "front_end", nil)
         		if err != nil {
         			return err
         		}
-        		frontEndTargetGroup, err := lb.NewTargetGroup(ctx, "frontEndTargetGroup", nil)
+        		frontEndTargetGroup, err := lb.NewTargetGroup(ctx, "front_end", nil)
         		if err != nil {
         			return err
         		}
         		pool, err := cognito.NewUserPool(ctx, "pool", nil)
         		if err != nil {
         			return err
         		}
@@ -840,16 +827,16 @@
         		if err != nil {
         			return err
         		}
         		domain, err := cognito.NewUserPoolDomain(ctx, "domain", nil)
         		if err != nil {
         			return err
         		}
-        		_, err = lb.NewListener(ctx, "frontEndListener", &lb.ListenerArgs{
-        			LoadBalancerArn: frontEndLoadBalancer.Arn,
+        		_, err = lb.NewListener(ctx, "front_end", &lb.ListenerArgs{
+        			LoadBalancerArn: frontEnd.Arn,
         			Port:            pulumi.Int(80),
         			Protocol:        pulumi.String("HTTP"),
         			DefaultActions: lb.ListenerDefaultActionArray{
         				&lb.ListenerDefaultActionArgs{
         					Type: pulumi.String("authenticate-cognito"),
         					AuthenticateCognito: &lb.ListenerDefaultActionAuthenticateCognitoArgs{
         						UserPoolArn:      pool.Arn,
@@ -894,26 +881,26 @@
 
         public class App {
             public static void main(String[] args) {
                 Pulumi.run(App::stack);
             }
 
             public static void stack(Context ctx) {
-                var frontEndLoadBalancer = new LoadBalancer("frontEndLoadBalancer");
+                var frontEnd = new LoadBalancer("frontEnd");
 
                 var frontEndTargetGroup = new TargetGroup("frontEndTargetGroup");
 
                 var pool = new UserPool("pool");
 
                 var client = new UserPoolClient("client");
 
                 var domain = new UserPoolDomain("domain");
 
                 var frontEndListener = new Listener("frontEndListener", ListenerArgs.builder()        
-                    .loadBalancerArn(frontEndLoadBalancer.arn())
+                    .loadBalancerArn(frontEnd.arn())
                     .port("80")
                     .protocol("HTTP")
                     .defaultActions(            
                         ListenerDefaultActionArgs.builder()
                             .type("authenticate-cognito")
                             .authenticateCognito(ListenerDefaultActionAuthenticateCognitoArgs.builder()
                                 .userPoolArn(pool.arn())
@@ -928,53 +915,55 @@
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
-          frontEndLoadBalancer:
+          frontEnd:
             type: aws:lb:LoadBalancer
+            name: front_end
           frontEndTargetGroup:
             type: aws:lb:TargetGroup
+            name: front_end
           pool:
             type: aws:cognito:UserPool
           client:
             type: aws:cognito:UserPoolClient
           domain:
             type: aws:cognito:UserPoolDomain
           frontEndListener:
             type: aws:lb:Listener
+            name: front_end
             properties:
-              loadBalancerArn: ${frontEndLoadBalancer.arn}
+              loadBalancerArn: ${frontEnd.arn}
               port: '80'
               protocol: HTTP
               defaultActions:
                 - type: authenticate-cognito
                   authenticateCognito:
                     userPoolArn: ${pool.arn}
                     userPoolClientId: ${client.id}
                     userPoolDomain: ${domain.domain}
                 - type: forward
                   targetGroupArn: ${frontEndTargetGroup.arn}
         ```
-        {{% /example %}}
-        {{% example %}}
+        <!--End PulumiCodeChooser -->
+
         ### Authenticate-OIDC Action
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
-        const frontEndLoadBalancer = new aws.lb.LoadBalancer("frontEndLoadBalancer", {});
-        // ...
-        const frontEndTargetGroup = new aws.lb.TargetGroup("frontEndTargetGroup", {});
-        // ...
-        const frontEndListener = new aws.lb.Listener("frontEndListener", {
-            loadBalancerArn: frontEndLoadBalancer.arn,
+        const frontEnd = new aws.lb.LoadBalancer("front_end", {});
+        const frontEndTargetGroup = new aws.lb.TargetGroup("front_end", {});
+        const frontEndListener = new aws.lb.Listener("front_end", {
+            loadBalancerArn: frontEnd.arn,
             port: 80,
             protocol: "HTTP",
             defaultActions: [
                 {
                     type: "authenticate-oidc",
                     authenticateOidc: {
                         authorizationEndpoint: "https://example.com/authorization_endpoint",
@@ -992,20 +981,18 @@
             ],
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
-        front_end_load_balancer = aws.lb.LoadBalancer("frontEndLoadBalancer")
-        # ...
-        front_end_target_group = aws.lb.TargetGroup("frontEndTargetGroup")
-        # ...
-        front_end_listener = aws.lb.Listener("frontEndListener",
-            load_balancer_arn=front_end_load_balancer.arn,
+        front_end = aws.lb.LoadBalancer("front_end")
+        front_end_target_group = aws.lb.TargetGroup("front_end")
+        front_end_listener = aws.lb.Listener("front_end",
+            load_balancer_arn=front_end.arn,
             port=80,
             protocol="HTTP",
             default_actions=[
                 aws.lb.ListenerDefaultActionArgs(
                     type="authenticate-oidc",
                     authenticate_oidc=aws.lb.ListenerDefaultActionAuthenticateOidcArgs(
                         authorization_endpoint="https://example.com/authorization_endpoint",
@@ -1026,23 +1013,21 @@
         using System.Collections.Generic;
         using System.Linq;
         using Pulumi;
         using Aws = Pulumi.Aws;
 
         return await Deployment.RunAsync(() => 
         {
-            var frontEndLoadBalancer = new Aws.LB.LoadBalancer("frontEndLoadBalancer");
+            var frontEnd = new Aws.LB.LoadBalancer("front_end");
 
-            // ...
-            var frontEndTargetGroup = new Aws.LB.TargetGroup("frontEndTargetGroup");
+            var frontEndTargetGroup = new Aws.LB.TargetGroup("front_end");
 
-            // ...
-            var frontEndListener = new Aws.LB.Listener("frontEndListener", new()
+            var frontEndListener = new Aws.LB.Listener("front_end", new()
             {
-                LoadBalancerArn = frontEndLoadBalancer.Arn,
+                LoadBalancerArn = frontEnd.Arn,
                 Port = 80,
                 Protocol = "HTTP",
                 DefaultActions = new[]
                 {
                     new Aws.LB.Inputs.ListenerDefaultActionArgs
                     {
                         Type = "authenticate-oidc",
@@ -1072,24 +1057,24 @@
         import (
         	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/lb"
         	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
         )
 
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
-        		frontEndLoadBalancer, err := lb.NewLoadBalancer(ctx, "frontEndLoadBalancer", nil)
+        		frontEnd, err := lb.NewLoadBalancer(ctx, "front_end", nil)
         		if err != nil {
         			return err
         		}
-        		frontEndTargetGroup, err := lb.NewTargetGroup(ctx, "frontEndTargetGroup", nil)
+        		frontEndTargetGroup, err := lb.NewTargetGroup(ctx, "front_end", nil)
         		if err != nil {
         			return err
         		}
-        		_, err = lb.NewListener(ctx, "frontEndListener", &lb.ListenerArgs{
-        			LoadBalancerArn: frontEndLoadBalancer.Arn,
+        		_, err = lb.NewListener(ctx, "front_end", &lb.ListenerArgs{
+        			LoadBalancerArn: frontEnd.Arn,
         			Port:            pulumi.Int(80),
         			Protocol:        pulumi.String("HTTP"),
         			DefaultActions: lb.ListenerDefaultActionArray{
         				&lb.ListenerDefaultActionArgs{
         					Type: pulumi.String("authenticate-oidc"),
         					AuthenticateOidc: &lb.ListenerDefaultActionAuthenticateOidcArgs{
         						AuthorizationEndpoint: pulumi.String("https://example.com/authorization_endpoint"),
@@ -1134,20 +1119,20 @@
 
         public class App {
             public static void main(String[] args) {
                 Pulumi.run(App::stack);
             }
 
             public static void stack(Context ctx) {
-                var frontEndLoadBalancer = new LoadBalancer("frontEndLoadBalancer");
+                var frontEnd = new LoadBalancer("frontEnd");
 
                 var frontEndTargetGroup = new TargetGroup("frontEndTargetGroup");
 
                 var frontEndListener = new Listener("frontEndListener", ListenerArgs.builder()        
-                    .loadBalancerArn(frontEndLoadBalancer.arn())
+                    .loadBalancerArn(frontEnd.arn())
                     .port("80")
                     .protocol("HTTP")
                     .defaultActions(            
                         ListenerDefaultActionArgs.builder()
                             .type("authenticate-oidc")
                             .authenticateOidc(ListenerDefaultActionAuthenticateOidcArgs.builder()
                                 .authorizationEndpoint("https://example.com/authorization_endpoint")
@@ -1165,126 +1150,136 @@
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
-          frontEndLoadBalancer:
+          frontEnd:
             type: aws:lb:LoadBalancer
+            name: front_end
           frontEndTargetGroup:
             type: aws:lb:TargetGroup
+            name: front_end
           frontEndListener:
             type: aws:lb:Listener
+            name: front_end
             properties:
-              loadBalancerArn: ${frontEndLoadBalancer.arn}
+              loadBalancerArn: ${frontEnd.arn}
               port: '80'
               protocol: HTTP
               defaultActions:
                 - type: authenticate-oidc
                   authenticateOidc:
                     authorizationEndpoint: https://example.com/authorization_endpoint
                     clientId: client_id
                     clientSecret: client_secret
                     issuer: https://example.com
                     tokenEndpoint: https://example.com/token_endpoint
                     userInfoEndpoint: https://example.com/user_info_endpoint
                 - type: forward
                   targetGroupArn: ${frontEndTargetGroup.arn}
         ```
-        {{% /example %}}
-        {{% example %}}
+        <!--End PulumiCodeChooser -->
+
         ### Gateway Load Balancer Listener
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
-        const exampleLoadBalancer = new aws.lb.LoadBalancer("exampleLoadBalancer", {
+        const example = new aws.lb.LoadBalancer("example", {
             loadBalancerType: "gateway",
+            name: "example",
             subnetMappings: [{
-                subnetId: aws_subnet.example.id,
+                subnetId: exampleAwsSubnet.id,
             }],
         });
-        const exampleTargetGroup = new aws.lb.TargetGroup("exampleTargetGroup", {
+        const exampleTargetGroup = new aws.lb.TargetGroup("example", {
+            name: "example",
             port: 6081,
             protocol: "GENEVE",
-            vpcId: aws_vpc.example.id,
+            vpcId: exampleAwsVpc.id,
             healthCheck: {
                 port: "80",
                 protocol: "HTTP",
             },
         });
-        const exampleListener = new aws.lb.Listener("exampleListener", {
-            loadBalancerArn: exampleLoadBalancer.id,
+        const exampleListener = new aws.lb.Listener("example", {
+            loadBalancerArn: example.id,
             defaultActions: [{
                 targetGroupArn: exampleTargetGroup.id,
                 type: "forward",
             }],
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
-        example_load_balancer = aws.lb.LoadBalancer("exampleLoadBalancer",
+        example = aws.lb.LoadBalancer("example",
             load_balancer_type="gateway",
+            name="example",
             subnet_mappings=[aws.lb.LoadBalancerSubnetMappingArgs(
-                subnet_id=aws_subnet["example"]["id"],
+                subnet_id=example_aws_subnet["id"],
             )])
-        example_target_group = aws.lb.TargetGroup("exampleTargetGroup",
+        example_target_group = aws.lb.TargetGroup("example",
+            name="example",
             port=6081,
             protocol="GENEVE",
-            vpc_id=aws_vpc["example"]["id"],
+            vpc_id=example_aws_vpc["id"],
             health_check=aws.lb.TargetGroupHealthCheckArgs(
                 port="80",
                 protocol="HTTP",
             ))
-        example_listener = aws.lb.Listener("exampleListener",
-            load_balancer_arn=example_load_balancer.id,
+        example_listener = aws.lb.Listener("example",
+            load_balancer_arn=example.id,
             default_actions=[aws.lb.ListenerDefaultActionArgs(
                 target_group_arn=example_target_group.id,
                 type="forward",
             )])
         ```
         ```csharp
         using System.Collections.Generic;
         using System.Linq;
         using Pulumi;
         using Aws = Pulumi.Aws;
 
         return await Deployment.RunAsync(() => 
         {
-            var exampleLoadBalancer = new Aws.LB.LoadBalancer("exampleLoadBalancer", new()
+            var example = new Aws.LB.LoadBalancer("example", new()
             {
                 LoadBalancerType = "gateway",
+                Name = "example",
                 SubnetMappings = new[]
                 {
                     new Aws.LB.Inputs.LoadBalancerSubnetMappingArgs
                     {
-                        SubnetId = aws_subnet.Example.Id,
+                        SubnetId = exampleAwsSubnet.Id,
                     },
                 },
             });
 
-            var exampleTargetGroup = new Aws.LB.TargetGroup("exampleTargetGroup", new()
+            var exampleTargetGroup = new Aws.LB.TargetGroup("example", new()
             {
+                Name = "example",
                 Port = 6081,
                 Protocol = "GENEVE",
-                VpcId = aws_vpc.Example.Id,
+                VpcId = exampleAwsVpc.Id,
                 HealthCheck = new Aws.LB.Inputs.TargetGroupHealthCheckArgs
                 {
                     Port = "80",
                     Protocol = "HTTP",
                 },
             });
 
-            var exampleListener = new Aws.LB.Listener("exampleListener", new()
+            var exampleListener = new Aws.LB.Listener("example", new()
             {
-                LoadBalancerArn = exampleLoadBalancer.Id,
+                LoadBalancerArn = example.Id,
                 DefaultActions = new[]
                 {
                     new Aws.LB.Inputs.ListenerDefaultActionArgs
                     {
                         TargetGroupArn = exampleTargetGroup.Id,
                         Type = "forward",
                     },
@@ -1299,39 +1294,41 @@
         import (
         	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/lb"
         	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
         )
 
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
-        		exampleLoadBalancer, err := lb.NewLoadBalancer(ctx, "exampleLoadBalancer", &lb.LoadBalancerArgs{
+        		example, err := lb.NewLoadBalancer(ctx, "example", &lb.LoadBalancerArgs{
         			LoadBalancerType: pulumi.String("gateway"),
+        			Name:             pulumi.String("example"),
         			SubnetMappings: lb.LoadBalancerSubnetMappingArray{
         				&lb.LoadBalancerSubnetMappingArgs{
-        					SubnetId: pulumi.Any(aws_subnet.Example.Id),
+        					SubnetId: pulumi.Any(exampleAwsSubnet.Id),
         				},
         			},
         		})
         		if err != nil {
         			return err
         		}
-        		exampleTargetGroup, err := lb.NewTargetGroup(ctx, "exampleTargetGroup", &lb.TargetGroupArgs{
+        		exampleTargetGroup, err := lb.NewTargetGroup(ctx, "example", &lb.TargetGroupArgs{
+        			Name:     pulumi.String("example"),
         			Port:     pulumi.Int(6081),
         			Protocol: pulumi.String("GENEVE"),
-        			VpcId:    pulumi.Any(aws_vpc.Example.Id),
+        			VpcId:    pulumi.Any(exampleAwsVpc.Id),
         			HealthCheck: &lb.TargetGroupHealthCheckArgs{
         				Port:     pulumi.String("80"),
         				Protocol: pulumi.String("HTTP"),
         			},
         		})
         		if err != nil {
         			return err
         		}
-        		_, err = lb.NewListener(ctx, "exampleListener", &lb.ListenerArgs{
-        			LoadBalancerArn: exampleLoadBalancer.ID(),
+        		_, err = lb.NewListener(ctx, "example", &lb.ListenerArgs{
+        			LoadBalancerArn: example.ID(),
         			DefaultActions: lb.ListenerDefaultActionArray{
         				&lb.ListenerDefaultActionArgs{
         					TargetGroupArn: exampleTargetGroup.ID(),
         					Type:           pulumi.String("forward"),
         				},
         			},
         		})
@@ -1366,94 +1363,285 @@
 
         public class App {
             public static void main(String[] args) {
                 Pulumi.run(App::stack);
             }
 
             public static void stack(Context ctx) {
-                var exampleLoadBalancer = new LoadBalancer("exampleLoadBalancer", LoadBalancerArgs.builder()        
+                var example = new LoadBalancer("example", LoadBalancerArgs.builder()        
                     .loadBalancerType("gateway")
+                    .name("example")
                     .subnetMappings(LoadBalancerSubnetMappingArgs.builder()
-                        .subnetId(aws_subnet.example().id())
+                        .subnetId(exampleAwsSubnet.id())
                         .build())
                     .build());
 
                 var exampleTargetGroup = new TargetGroup("exampleTargetGroup", TargetGroupArgs.builder()        
+                    .name("example")
                     .port(6081)
                     .protocol("GENEVE")
-                    .vpcId(aws_vpc.example().id())
+                    .vpcId(exampleAwsVpc.id())
                     .healthCheck(TargetGroupHealthCheckArgs.builder()
                         .port(80)
                         .protocol("HTTP")
                         .build())
                     .build());
 
                 var exampleListener = new Listener("exampleListener", ListenerArgs.builder()        
-                    .loadBalancerArn(exampleLoadBalancer.id())
+                    .loadBalancerArn(example.id())
                     .defaultActions(ListenerDefaultActionArgs.builder()
                         .targetGroupArn(exampleTargetGroup.id())
                         .type("forward")
                         .build())
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
-          exampleLoadBalancer:
+          example:
             type: aws:lb:LoadBalancer
             properties:
               loadBalancerType: gateway
+              name: example
               subnetMappings:
-                - subnetId: ${aws_subnet.example.id}
+                - subnetId: ${exampleAwsSubnet.id}
           exampleTargetGroup:
             type: aws:lb:TargetGroup
+            name: example
             properties:
+              name: example
               port: 6081
               protocol: GENEVE
-              vpcId: ${aws_vpc.example.id}
+              vpcId: ${exampleAwsVpc.id}
               healthCheck:
                 port: 80
                 protocol: HTTP
           exampleListener:
             type: aws:lb:Listener
+            name: example
+            properties:
+              loadBalancerArn: ${example.id}
+              defaultActions:
+                - targetGroupArn: ${exampleTargetGroup.id}
+                  type: forward
+        ```
+        <!--End PulumiCodeChooser -->
+
+        ### Mutual TLS Authentication
+
+        <!--Start PulumiCodeChooser -->
+        ```typescript
+        import * as pulumi from "@pulumi/pulumi";
+        import * as aws from "@pulumi/aws";
+
+        const example = new aws.lb.LoadBalancer("example", {loadBalancerType: "application"});
+        const exampleTargetGroup = new aws.lb.TargetGroup("example", {});
+        const exampleListener = new aws.lb.Listener("example", {
+            loadBalancerArn: example.id,
+            defaultActions: [{
+                targetGroupArn: exampleTargetGroup.id,
+                type: "forward",
+            }],
+            mutualAuthentication: {
+                mode: "verify",
+                trustStoreArn: "...",
+            },
+        });
+        ```
+        ```python
+        import pulumi
+        import pulumi_aws as aws
+
+        example = aws.lb.LoadBalancer("example", load_balancer_type="application")
+        example_target_group = aws.lb.TargetGroup("example")
+        example_listener = aws.lb.Listener("example",
+            load_balancer_arn=example.id,
+            default_actions=[aws.lb.ListenerDefaultActionArgs(
+                target_group_arn=example_target_group.id,
+                type="forward",
+            )],
+            mutual_authentication=aws.lb.ListenerMutualAuthenticationArgs(
+                mode="verify",
+                trust_store_arn="...",
+            ))
+        ```
+        ```csharp
+        using System.Collections.Generic;
+        using System.Linq;
+        using Pulumi;
+        using Aws = Pulumi.Aws;
+
+        return await Deployment.RunAsync(() => 
+        {
+            var example = new Aws.LB.LoadBalancer("example", new()
+            {
+                LoadBalancerType = "application",
+            });
+
+            var exampleTargetGroup = new Aws.LB.TargetGroup("example");
+
+            var exampleListener = new Aws.LB.Listener("example", new()
+            {
+                LoadBalancerArn = example.Id,
+                DefaultActions = new[]
+                {
+                    new Aws.LB.Inputs.ListenerDefaultActionArgs
+                    {
+                        TargetGroupArn = exampleTargetGroup.Id,
+                        Type = "forward",
+                    },
+                },
+                MutualAuthentication = new Aws.LB.Inputs.ListenerMutualAuthenticationArgs
+                {
+                    Mode = "verify",
+                    TrustStoreArn = "...",
+                },
+            });
+
+        });
+        ```
+        ```go
+        package main
+
+        import (
+        	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/lb"
+        	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
+        )
+
+        func main() {
+        	pulumi.Run(func(ctx *pulumi.Context) error {
+        		example, err := lb.NewLoadBalancer(ctx, "example", &lb.LoadBalancerArgs{
+        			LoadBalancerType: pulumi.String("application"),
+        		})
+        		if err != nil {
+        			return err
+        		}
+        		exampleTargetGroup, err := lb.NewTargetGroup(ctx, "example", nil)
+        		if err != nil {
+        			return err
+        		}
+        		_, err = lb.NewListener(ctx, "example", &lb.ListenerArgs{
+        			LoadBalancerArn: example.ID(),
+        			DefaultActions: lb.ListenerDefaultActionArray{
+        				&lb.ListenerDefaultActionArgs{
+        					TargetGroupArn: exampleTargetGroup.ID(),
+        					Type:           pulumi.String("forward"),
+        				},
+        			},
+        			MutualAuthentication: &lb.ListenerMutualAuthenticationArgs{
+        				Mode:          pulumi.String("verify"),
+        				TrustStoreArn: pulumi.String("..."),
+        			},
+        		})
+        		if err != nil {
+        			return err
+        		}
+        		return nil
+        	})
+        }
+        ```
+        ```java
+        package generated_program;
+
+        import com.pulumi.Context;
+        import com.pulumi.Pulumi;
+        import com.pulumi.core.Output;
+        import com.pulumi.aws.lb.LoadBalancer;
+        import com.pulumi.aws.lb.LoadBalancerArgs;
+        import com.pulumi.aws.lb.TargetGroup;
+        import com.pulumi.aws.lb.Listener;
+        import com.pulumi.aws.lb.ListenerArgs;
+        import com.pulumi.aws.lb.inputs.ListenerDefaultActionArgs;
+        import com.pulumi.aws.lb.inputs.ListenerMutualAuthenticationArgs;
+        import java.util.List;
+        import java.util.ArrayList;
+        import java.util.Map;
+        import java.io.File;
+        import java.nio.file.Files;
+        import java.nio.file.Paths;
+
+        public class App {
+            public static void main(String[] args) {
+                Pulumi.run(App::stack);
+            }
+
+            public static void stack(Context ctx) {
+                var example = new LoadBalancer("example", LoadBalancerArgs.builder()        
+                    .loadBalancerType("application")
+                    .build());
+
+                var exampleTargetGroup = new TargetGroup("exampleTargetGroup");
+
+                var exampleListener = new Listener("exampleListener", ListenerArgs.builder()        
+                    .loadBalancerArn(example.id())
+                    .defaultActions(ListenerDefaultActionArgs.builder()
+                        .targetGroupArn(exampleTargetGroup.id())
+                        .type("forward")
+                        .build())
+                    .mutualAuthentication(ListenerMutualAuthenticationArgs.builder()
+                        .mode("verify")
+                        .trustStoreArn("...")
+                        .build())
+                    .build());
+
+            }
+        }
+        ```
+        ```yaml
+        resources:
+          example:
+            type: aws:lb:LoadBalancer
+            properties:
+              loadBalancerType: application
+          exampleTargetGroup:
+            type: aws:lb:TargetGroup
+            name: example
+          exampleListener:
+            type: aws:lb:Listener
+            name: example
             properties:
-              loadBalancerArn: ${exampleLoadBalancer.id}
+              loadBalancerArn: ${example.id}
               defaultActions:
                 - targetGroupArn: ${exampleTargetGroup.id}
                   type: forward
+              mutualAuthentication:
+                mode: verify
+                trustStoreArn: '...'
         ```
-        {{% /example %}}
-        {{% /examples %}}
+        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Using `pulumi import`, import listeners using their ARN. For example:
 
         ```sh
-         $ pulumi import aws:lb/listener:Listener front_end arn:aws:elasticloadbalancing:us-west-2:187416307283:listener/app/front-end-alb/8e4497da625e2d8a/9ab28ade35828f96
+        $ pulumi import aws:lb/listener:Listener front_end arn:aws:elasticloadbalancing:us-west-2:187416307283:listener/app/front-end-alb/8e4497da625e2d8a/9ab28ade35828f96
         ```
-         
+
         :param pulumi.Input[str] alpn_policy: Name of the Application-Layer Protocol Negotiation (ALPN) policy. Can be set if `protocol` is `TLS`. Valid values are `HTTP1Only`, `HTTP2Only`, `HTTP2Optional`, `HTTP2Preferred`, and `None`.
         :param pulumi.Input[str] certificate_arn: ARN of the default SSL server certificate. Exactly one certificate is required if the protocol is HTTPS. For adding additional SSL certificates, see the `aws.lb.ListenerCertificate` resource.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.ListenerDefaultActionArgs']]] default_actions: Configuration block for default actions. Detailed below.
+        :param pulumi.Input['pulumi_aws.lb.ListenerMutualAuthenticationArgs'] mutual_authentication: The mutual authentication configuration information. Detailed below.
         :param pulumi.Input[int] port: Port on which the load balancer is listening. Not valid for Gateway Load Balancers.
         :param pulumi.Input[str] protocol: Protocol for connections from clients to the load balancer. For Application Load Balancers, valid values are `HTTP` and `HTTPS`, with a default of `HTTP`. For Network Load Balancers, valid values are `TCP`, `TLS`, `UDP`, and `TCP_UDP`. Not valid to use `UDP` or `TCP_UDP` if dual-stack mode is enabled. Not valid for Gateway Load Balancers.
         :param pulumi.Input[str] ssl_policy: Name of the SSL Policy for the listener. Required if `protocol` is `HTTPS` or `TLS`.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags to assign to the resource. .If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
                
                > **NOTE::** Please note that listeners that are attached to Application Load Balancers must use either `HTTP` or `HTTPS` protocols while listeners that are attached to Network Load Balancers must use the `TCP` protocol.
         """
         if alpn_policy is not None:
             pulumi.set(__self__, "alpn_policy", alpn_policy)
         if certificate_arn is not None:
             pulumi.set(__self__, "certificate_arn", certificate_arn)
         if default_actions is not None:
             pulumi.set(__self__, "default_actions", default_actions)
+        if mutual_authentication is not None:
+            pulumi.set(__self__, "mutual_authentication", mutual_authentication)
         if port is not None:
             pulumi.set(__self__, "port", port)
         if protocol is not None:
             pulumi.set(__self__, "protocol", protocol)
         if ssl_policy is not None:
             pulumi.set(__self__, "ssl_policy", ssl_policy)
         if tags is not None:
@@ -1492,14 +1680,26 @@
         return pulumi.get(self, "default_actions")
 
     @default_actions.setter
     def default_actions(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.ListenerDefaultActionArgs']]]]):
         pulumi.set(self, "default_actions", value)
 
     @property
+    @pulumi.getter(name="mutualAuthentication")
+    def mutual_authentication(self) -> Optional[pulumi.Input['pulumi_aws.lb.ListenerMutualAuthenticationArgs']]:
+        """
+        The mutual authentication configuration information. Detailed below.
+        """
+        return pulumi.get(self, "mutual_authentication")
+
+    @mutual_authentication.setter
+    def mutual_authentication(self, value: Optional[pulumi.Input['pulumi_aws.lb.ListenerMutualAuthenticationArgs']]):
+        pulumi.set(self, "mutual_authentication", value)
+
+    @property
     @pulumi.getter
     def port(self) -> Optional[pulumi.Input[int]]:
         """
         Port on which the load balancer is listening. Not valid for Gateway Load Balancers.
         """
         return pulumi.get(self, "port")
 
@@ -1551,14 +1751,15 @@
     def __init__(__self__, *,
                  connection_termination: Optional[pulumi.Input[bool]] = None,
                  deregistration_delay: Optional[pulumi.Input[int]] = None,
                  health_check: Optional[pulumi.Input['pulumi_aws.lb.TargetGroupHealthCheckArgs']] = None,
                  ip_address_type: Optional[pulumi.Input[str]] = None,
                  lambda_multi_value_headers_enabled: Optional[pulumi.Input[bool]] = None,
                  load_balancing_algorithm_type: Optional[pulumi.Input[str]] = None,
+                 load_balancing_anomaly_mitigation: Optional[pulumi.Input[str]] = None,
                  load_balancing_cross_zone_enabled: Optional[pulumi.Input[str]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
                  port: Optional[pulumi.Input[int]] = None,
                  preserve_client_ip: Optional[pulumi.Input[str]] = None,
                  protocol: Optional[pulumi.Input[str]] = None,
                  protocol_version: Optional[pulumi.Input[str]] = None,
@@ -1571,36 +1772,38 @@
                  target_type: Optional[pulumi.Input[str]] = None,
                  vpc_id: Optional[pulumi.Input[str]] = None):
         """
         Provides a Target Group resource for use with Load Balancer resources.
 
         > **Note:** `aws.alb.TargetGroup` is known as `aws.lb.TargetGroup`. The functionality is identical.
 
-        {{% examples %}}
         ## Example Usage
-        {{% example %}}
+
         ### Instance Target Group
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
         const main = new aws.ec2.Vpc("main", {cidrBlock: "10.0.0.0/16"});
         const test = new aws.lb.TargetGroup("test", {
+            name: "tf-example-lb-tg",
             port: 80,
             protocol: "HTTP",
             vpcId: main.id,
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
         main = aws.ec2.Vpc("main", cidr_block="10.0.0.0/16")
         test = aws.lb.TargetGroup("test",
+            name="tf-example-lb-tg",
             port=80,
             protocol="HTTP",
             vpc_id=main.id)
         ```
         ```csharp
         using System.Collections.Generic;
         using System.Linq;
@@ -1612,14 +1815,15 @@
             var main = new Aws.Ec2.Vpc("main", new()
             {
                 CidrBlock = "10.0.0.0/16",
             });
 
             var test = new Aws.LB.TargetGroup("test", new()
             {
+                Name = "tf-example-lb-tg",
                 Port = 80,
                 Protocol = "HTTP",
                 VpcId = main.Id,
             });
 
         });
         ```
@@ -1637,14 +1841,15 @@
         		main, err := ec2.NewVpc(ctx, "main", &ec2.VpcArgs{
         			CidrBlock: pulumi.String("10.0.0.0/16"),
         		})
         		if err != nil {
         			return err
         		}
         		_, err = lb.NewTargetGroup(ctx, "test", &lb.TargetGroupArgs{
+        			Name:     pulumi.String("tf-example-lb-tg"),
         			Port:     pulumi.Int(80),
         			Protocol: pulumi.String("HTTP"),
         			VpcId:    main.ID(),
         		})
         		if err != nil {
         			return err
         		}
@@ -1676,57 +1881,62 @@
 
             public static void stack(Context ctx) {
                 var main = new Vpc("main", VpcArgs.builder()        
                     .cidrBlock("10.0.0.0/16")
                     .build());
 
                 var test = new TargetGroup("test", TargetGroupArgs.builder()        
+                    .name("tf-example-lb-tg")
                     .port(80)
                     .protocol("HTTP")
                     .vpcId(main.id())
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
           test:
             type: aws:lb:TargetGroup
             properties:
+              name: tf-example-lb-tg
               port: 80
               protocol: HTTP
               vpcId: ${main.id}
           main:
             type: aws:ec2:Vpc
             properties:
               cidrBlock: 10.0.0.0/16
         ```
-        {{% /example %}}
-        {{% example %}}
+        <!--End PulumiCodeChooser -->
+
         ### IP Target Group
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
         const main = new aws.ec2.Vpc("main", {cidrBlock: "10.0.0.0/16"});
         const ip_example = new aws.lb.TargetGroup("ip-example", {
+            name: "tf-example-lb-tg",
             port: 80,
             protocol: "HTTP",
             targetType: "ip",
             vpcId: main.id,
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
         main = aws.ec2.Vpc("main", cidr_block="10.0.0.0/16")
         ip_example = aws.lb.TargetGroup("ip-example",
+            name="tf-example-lb-tg",
             port=80,
             protocol="HTTP",
             target_type="ip",
             vpc_id=main.id)
         ```
         ```csharp
         using System.Collections.Generic;
@@ -1739,14 +1949,15 @@
             var main = new Aws.Ec2.Vpc("main", new()
             {
                 CidrBlock = "10.0.0.0/16",
             });
 
             var ip_example = new Aws.LB.TargetGroup("ip-example", new()
             {
+                Name = "tf-example-lb-tg",
                 Port = 80,
                 Protocol = "HTTP",
                 TargetType = "ip",
                 VpcId = main.Id,
             });
 
         });
@@ -1765,14 +1976,15 @@
         		main, err := ec2.NewVpc(ctx, "main", &ec2.VpcArgs{
         			CidrBlock: pulumi.String("10.0.0.0/16"),
         		})
         		if err != nil {
         			return err
         		}
         		_, err = lb.NewTargetGroup(ctx, "ip-example", &lb.TargetGroupArgs{
+        			Name:       pulumi.String("tf-example-lb-tg"),
         			Port:       pulumi.Int(80),
         			Protocol:   pulumi.String("HTTP"),
         			TargetType: pulumi.String("ip"),
         			VpcId:      main.ID(),
         		})
         		if err != nil {
         			return err
@@ -1805,63 +2017,72 @@
 
             public static void stack(Context ctx) {
                 var main = new Vpc("main", VpcArgs.builder()        
                     .cidrBlock("10.0.0.0/16")
                     .build());
 
                 var ip_example = new TargetGroup("ip-example", TargetGroupArgs.builder()        
+                    .name("tf-example-lb-tg")
                     .port(80)
                     .protocol("HTTP")
                     .targetType("ip")
                     .vpcId(main.id())
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
           ip-example:
             type: aws:lb:TargetGroup
             properties:
+              name: tf-example-lb-tg
               port: 80
               protocol: HTTP
               targetType: ip
               vpcId: ${main.id}
           main:
             type: aws:ec2:Vpc
             properties:
               cidrBlock: 10.0.0.0/16
         ```
-        {{% /example %}}
-        {{% example %}}
+        <!--End PulumiCodeChooser -->
+
         ### Lambda Target Group
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
-        const lambda_example = new aws.lb.TargetGroup("lambda-example", {targetType: "lambda"});
+        const lambda_example = new aws.lb.TargetGroup("lambda-example", {
+            name: "tf-example-lb-tg",
+            targetType: "lambda",
+        });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
-        lambda_example = aws.lb.TargetGroup("lambda-example", target_type="lambda")
+        lambda_example = aws.lb.TargetGroup("lambda-example",
+            name="tf-example-lb-tg",
+            target_type="lambda")
         ```
         ```csharp
         using System.Collections.Generic;
         using System.Linq;
         using Pulumi;
         using Aws = Pulumi.Aws;
 
         return await Deployment.RunAsync(() => 
         {
             var lambda_example = new Aws.LB.TargetGroup("lambda-example", new()
             {
+                Name = "tf-example-lb-tg",
                 TargetType = "lambda",
             });
 
         });
         ```
         ```go
         package main
@@ -1870,14 +2091,15 @@
         	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/lb"
         	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
         )
 
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
         		_, err := lb.NewTargetGroup(ctx, "lambda-example", &lb.TargetGroupArgs{
+        			Name:       pulumi.String("tf-example-lb-tg"),
         			TargetType: pulumi.String("lambda"),
         		})
         		if err != nil {
         			return err
         		}
         		return nil
         	})
@@ -1901,66 +2123,72 @@
         public class App {
             public static void main(String[] args) {
                 Pulumi.run(App::stack);
             }
 
             public static void stack(Context ctx) {
                 var lambda_example = new TargetGroup("lambda-example", TargetGroupArgs.builder()        
+                    .name("tf-example-lb-tg")
                     .targetType("lambda")
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
           lambda-example:
             type: aws:lb:TargetGroup
             properties:
+              name: tf-example-lb-tg
               targetType: lambda
         ```
-        {{% /example %}}
-        {{% example %}}
+        <!--End PulumiCodeChooser -->
+
         ### ALB Target Group
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
         const alb_example = new aws.lb.TargetGroup("alb-example", {
+            name: "tf-example-lb-alb-tg",
             targetType: "alb",
             port: 80,
             protocol: "TCP",
-            vpcId: aws_vpc.main.id,
+            vpcId: main.id,
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
         alb_example = aws.lb.TargetGroup("alb-example",
+            name="tf-example-lb-alb-tg",
             target_type="alb",
             port=80,
             protocol="TCP",
-            vpc_id=aws_vpc["main"]["id"])
+            vpc_id=main["id"])
         ```
         ```csharp
         using System.Collections.Generic;
         using System.Linq;
         using Pulumi;
         using Aws = Pulumi.Aws;
 
         return await Deployment.RunAsync(() => 
         {
             var alb_example = new Aws.LB.TargetGroup("alb-example", new()
             {
+                Name = "tf-example-lb-alb-tg",
                 TargetType = "alb",
                 Port = 80,
                 Protocol = "TCP",
-                VpcId = aws_vpc.Main.Id,
+                VpcId = main.Id,
             });
 
         });
         ```
         ```go
         package main
 
@@ -1968,18 +2196,19 @@
         	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/lb"
         	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
         )
 
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
         		_, err := lb.NewTargetGroup(ctx, "alb-example", &lb.TargetGroupArgs{
+        			Name:       pulumi.String("tf-example-lb-alb-tg"),
         			TargetType: pulumi.String("alb"),
         			Port:       pulumi.Int(80),
         			Protocol:   pulumi.String("TCP"),
-        			VpcId:      pulumi.Any(aws_vpc.Main.Id),
+        			VpcId:      pulumi.Any(main.Id),
         		})
         		if err != nil {
         			return err
         		}
         		return nil
         	})
         }
@@ -2002,75 +2231,81 @@
         public class App {
             public static void main(String[] args) {
                 Pulumi.run(App::stack);
             }
 
             public static void stack(Context ctx) {
                 var alb_example = new TargetGroup("alb-example", TargetGroupArgs.builder()        
+                    .name("tf-example-lb-alb-tg")
                     .targetType("alb")
                     .port(80)
                     .protocol("TCP")
-                    .vpcId(aws_vpc.main().id())
+                    .vpcId(main.id())
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
           alb-example:
             type: aws:lb:TargetGroup
             properties:
+              name: tf-example-lb-alb-tg
               targetType: alb
               port: 80
               protocol: TCP
-              vpcId: ${aws_vpc.main.id}
+              vpcId: ${main.id}
         ```
-        {{% /example %}}
-        {{% example %}}
+        <!--End PulumiCodeChooser -->
+
         ### Target group with unhealthy connection termination disabled
 
+        <!--Start PulumiCodeChooser -->
         ```typescript
         import * as pulumi from "@pulumi/pulumi";
         import * as aws from "@pulumi/aws";
 
         const tcp_example = new aws.lb.TargetGroup("tcp-example", {
+            name: "tf-example-lb-nlb-tg",
             port: 25,
             protocol: "TCP",
-            vpcId: aws_vpc.main.id,
+            vpcId: main.id,
             targetHealthStates: [{
                 enableUnhealthyConnectionTermination: false,
             }],
         });
         ```
         ```python
         import pulumi
         import pulumi_aws as aws
 
         tcp_example = aws.lb.TargetGroup("tcp-example",
+            name="tf-example-lb-nlb-tg",
             port=25,
             protocol="TCP",
-            vpc_id=aws_vpc["main"]["id"],
+            vpc_id=main["id"],
             target_health_states=[aws.lb.TargetGroupTargetHealthStateArgs(
                 enable_unhealthy_connection_termination=False,
             )])
         ```
         ```csharp
         using System.Collections.Generic;
         using System.Linq;
         using Pulumi;
         using Aws = Pulumi.Aws;
 
         return await Deployment.RunAsync(() => 
         {
             var tcp_example = new Aws.LB.TargetGroup("tcp-example", new()
             {
+                Name = "tf-example-lb-nlb-tg",
                 Port = 25,
                 Protocol = "TCP",
-                VpcId = aws_vpc.Main.Id,
+                VpcId = main.Id,
                 TargetHealthStates = new[]
                 {
                     new Aws.LB.Inputs.TargetGroupTargetHealthStateArgs
                     {
                         EnableUnhealthyConnectionTermination = false,
                     },
                 },
@@ -2085,17 +2320,18 @@
         	"github.com/pulumi/pulumi-aws/sdk/v6/go/aws/lb"
         	"github.com/pulumi/pulumi/sdk/v3/go/pulumi"
         )
 
         func main() {
         	pulumi.Run(func(ctx *pulumi.Context) error {
         		_, err := lb.NewTargetGroup(ctx, "tcp-example", &lb.TargetGroupArgs{
+        			Name:     pulumi.String("tf-example-lb-nlb-tg"),
         			Port:     pulumi.Int(25),
         			Protocol: pulumi.String("TCP"),
-        			VpcId:    pulumi.Any(aws_vpc.Main.Id),
+        			VpcId:    pulumi.Any(main.Id),
         			TargetHealthStates: lb.TargetGroupTargetHealthStateArray{
         				&lb.TargetGroupTargetHealthStateArgs{
         					EnableUnhealthyConnectionTermination: pulumi.Bool(false),
         				},
         			},
         		})
         		if err != nil {
@@ -2124,67 +2360,74 @@
         public class App {
             public static void main(String[] args) {
                 Pulumi.run(App::stack);
             }
 
             public static void stack(Context ctx) {
                 var tcp_example = new TargetGroup("tcp-example", TargetGroupArgs.builder()        
+                    .name("tf-example-lb-nlb-tg")
                     .port(25)
                     .protocol("TCP")
-                    .vpcId(aws_vpc.main().id())
+                    .vpcId(main.id())
                     .targetHealthStates(TargetGroupTargetHealthStateArgs.builder()
                         .enableUnhealthyConnectionTermination(false)
                         .build())
                     .build());
 
             }
         }
         ```
         ```yaml
         resources:
           tcp-example:
             type: aws:lb:TargetGroup
             properties:
+              name: tf-example-lb-nlb-tg
               port: 25
               protocol: TCP
-              vpcId: ${aws_vpc.main.id}
+              vpcId: ${main.id}
               targetHealthStates:
                 - enableUnhealthyConnectionTermination: false
         ```
-        {{% /example %}}
-        {{% /examples %}}
+        <!--End PulumiCodeChooser -->
 
         ## Import
 
         Using `pulumi import`, import Target Groups using their ARN. For example:
 
         ```sh
-         $ pulumi import aws:lb/targetGroup:TargetGroup app_front_end arn:aws:elasticloadbalancing:us-west-2:187416307283:targetgroup/app-front-end/20cfe21448b66314
+        $ pulumi import aws:lb/targetGroup:TargetGroup app_front_end arn:aws:elasticloadbalancing:us-west-2:187416307283:targetgroup/app-front-end/20cfe21448b66314
         ```
-         
+
         :param pulumi.Input[bool] connection_termination: Whether to terminate connections at the end of the deregistration timeout on Network Load Balancers. See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/load-balancer-target-groups.html#deregistration-delay) for more information. Default is `false`.
         :param pulumi.Input[int] deregistration_delay: Amount time for Elastic Load Balancing to wait before changing the state of a deregistering target from draining to unused. The range is 0-3600 seconds. The default value is 300 seconds.
         :param pulumi.Input['pulumi_aws.lb.TargetGroupHealthCheckArgs'] health_check: Health Check configuration block. Detailed below.
         :param pulumi.Input[str] ip_address_type: The type of IP addresses used by the target group, only supported when target type is set to `ip`. Possible values are `ipv4` or `ipv6`.
         :param pulumi.Input[bool] lambda_multi_value_headers_enabled: Whether the request and response headers exchanged between the load balancer and the Lambda function include arrays of values or strings. Only applies when `target_type` is `lambda`. Default is `false`.
-        :param pulumi.Input[str] load_balancing_algorithm_type: Determines how the load balancer selects targets when routing requests. Only applicable for Application Load Balancer Target Groups. The value is `round_robin` or `least_outstanding_requests`. The default is `round_robin`.
+        :param pulumi.Input[str] load_balancing_algorithm_type: Determines how the load balancer selects targets when routing requests. Only applicable for Application Load Balancer Target Groups. The value is `round_robin`, `least_outstanding_requests`, or `weighted_random`. The default is `round_robin`.
+        :param pulumi.Input[str] load_balancing_anomaly_mitigation: Determines whether to enable target anomaly mitigation.  Target anomaly mitigation is only supported by the `weighted_random` load balancing algorithm type.  See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/load-balancer-target-groups.html#automatic-target-weights) for more information.  The value is `"on"` or `"off"`. The default is `"off"`.
         :param pulumi.Input[str] load_balancing_cross_zone_enabled: Indicates whether cross zone load balancing is enabled. The value is `"true"`, `"false"` or `"use_load_balancer_configuration"`. The default is `"use_load_balancer_configuration"`.
         :param pulumi.Input[str] name: Name of the target group. If omitted, this provider will assign a random, unique name. This name must be unique per region per account, can have a maximum of 32 characters, must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen.
         :param pulumi.Input[str] name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `name`. Cannot be longer than 6 characters.
         :param pulumi.Input[int] port: Port on which targets receive traffic, unless overridden when registering a specific target. Required when `target_type` is `instance`, `ip` or `alb`. Does not apply when `target_type` is `lambda`.
         :param pulumi.Input[str] preserve_client_ip: Whether client IP preservation is enabled. See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/load-balancer-target-groups.html#client-ip-preservation) for more information.
-        :param pulumi.Input[str] protocol: Protocol to use for routing traffic to the targets. Should be one of `GENEVE`, `HTTP`, `HTTPS`, `TCP`, `TCP_UDP`, `TLS`, or `UDP`. Required when `target_type` is `instance`, `ip` or `alb`. Does not apply when `target_type` is `lambda`.
+        :param pulumi.Input[str] protocol: Protocol to use for routing traffic to the targets.
+               Should be one of `GENEVE`, `HTTP`, `HTTPS`, `TCP`, `TCP_UDP`, `TLS`, or `UDP`.
+               Required when `target_type` is `instance`, `ip`, or `alb`.
+               Does not apply when `target_type` is `lambda`.
         :param pulumi.Input[str] protocol_version: Only applicable when `protocol` is `HTTP` or `HTTPS`. The protocol version. Specify `GRPC` to send requests to targets using gRPC. Specify `HTTP2` to send requests to targets using HTTP/2. The default is `HTTP1`, which sends requests to targets using HTTP/1.1
         :param pulumi.Input[bool] proxy_protocol_v2: Whether to enable support for proxy protocol v2 on Network Load Balancers. See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/load-balancer-target-groups.html#proxy-protocol) for more information. Default is `false`.
         :param pulumi.Input[int] slow_start: Amount time for targets to warm up before the load balancer sends them a full share of requests. The range is 30-900 seconds or 0 to disable. The default value is 0 seconds.
         :param pulumi.Input['pulumi_aws.lb.TargetGroupStickinessArgs'] stickiness: Stickiness configuration block. Detailed below.
         :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.TargetGroupTargetFailoverArgs']]] target_failovers: Target failover block. Only applicable for Gateway Load Balancer target groups. See target_failover for more information.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.TargetGroupTargetHealthStateArgs']]] target_health_states: Target health state block. Only applicable for Network Load Balancer target groups when `protocol` is `TCP` or `TLS`. See target_health_state for more information.
-        :param pulumi.Input[str] target_type: Type of target that you must specify when registering targets with this target group. See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_CreateTargetGroup.html) for supported values. The default is `instance`.
+        :param pulumi.Input[str] target_type: Type of target that you must specify when registering targets with this target group.
+               See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_CreateTargetGroup.html) for supported values.
+               The default is `instance`.
                
                Note that you can't specify targets for a target group using both instance IDs and IP addresses.
                
                If the target type is `ip`, specify IP addresses from the subnets of the virtual private cloud (VPC) for the target group, the RFC 1918 range (10.0.0.0/8, 172.16.0.0/12, and 192.168.0.0/16), and the RFC 6598 range (100.64.0.0/10). You can't specify publicly routable IP addresses.
                
                Network Load Balancers do not support the `lambda` target type.
                
@@ -2199,14 +2442,16 @@
             pulumi.set(__self__, "health_check", health_check)
         if ip_address_type is not None:
             pulumi.set(__self__, "ip_address_type", ip_address_type)
         if lambda_multi_value_headers_enabled is not None:
             pulumi.set(__self__, "lambda_multi_value_headers_enabled", lambda_multi_value_headers_enabled)
         if load_balancing_algorithm_type is not None:
             pulumi.set(__self__, "load_balancing_algorithm_type", load_balancing_algorithm_type)
+        if load_balancing_anomaly_mitigation is not None:
+            pulumi.set(__self__, "load_balancing_anomaly_mitigation", load_balancing_anomaly_mitigation)
         if load_balancing_cross_zone_enabled is not None:
             pulumi.set(__self__, "load_balancing_cross_zone_enabled", load_balancing_cross_zone_enabled)
         if name is not None:
             pulumi.set(__self__, "name", name)
         if name_prefix is not None:
             pulumi.set(__self__, "name_prefix", name_prefix)
         if port is not None:
@@ -2294,23 +2539,35 @@
     def lambda_multi_value_headers_enabled(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "lambda_multi_value_headers_enabled", value)
 
     @property
     @pulumi.getter(name="loadBalancingAlgorithmType")
     def load_balancing_algorithm_type(self) -> Optional[pulumi.Input[str]]:
         """
-        Determines how the load balancer selects targets when routing requests. Only applicable for Application Load Balancer Target Groups. The value is `round_robin` or `least_outstanding_requests`. The default is `round_robin`.
+        Determines how the load balancer selects targets when routing requests. Only applicable for Application Load Balancer Target Groups. The value is `round_robin`, `least_outstanding_requests`, or `weighted_random`. The default is `round_robin`.
         """
         return pulumi.get(self, "load_balancing_algorithm_type")
 
     @load_balancing_algorithm_type.setter
     def load_balancing_algorithm_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "load_balancing_algorithm_type", value)
 
     @property
+    @pulumi.getter(name="loadBalancingAnomalyMitigation")
+    def load_balancing_anomaly_mitigation(self) -> Optional[pulumi.Input[str]]:
+        """
+        Determines whether to enable target anomaly mitigation.  Target anomaly mitigation is only supported by the `weighted_random` load balancing algorithm type.  See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/application/load-balancer-target-groups.html#automatic-target-weights) for more information.  The value is `"on"` or `"off"`. The default is `"off"`.
+        """
+        return pulumi.get(self, "load_balancing_anomaly_mitigation")
+
+    @load_balancing_anomaly_mitigation.setter
+    def load_balancing_anomaly_mitigation(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "load_balancing_anomaly_mitigation", value)
+
+    @property
     @pulumi.getter(name="loadBalancingCrossZoneEnabled")
     def load_balancing_cross_zone_enabled(self) -> Optional[pulumi.Input[str]]:
         """
         Indicates whether cross zone load balancing is enabled. The value is `"true"`, `"false"` or `"use_load_balancer_configuration"`. The default is `"use_load_balancer_configuration"`.
         """
         return pulumi.get(self, "load_balancing_cross_zone_enabled")
 
@@ -2366,15 +2623,18 @@
     def preserve_client_ip(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "preserve_client_ip", value)
 
     @property
     @pulumi.getter
     def protocol(self) -> Optional[pulumi.Input[str]]:
         """
-        Protocol to use for routing traffic to the targets. Should be one of `GENEVE`, `HTTP`, `HTTPS`, `TCP`, `TCP_UDP`, `TLS`, or `UDP`. Required when `target_type` is `instance`, `ip` or `alb`. Does not apply when `target_type` is `lambda`.
+        Protocol to use for routing traffic to the targets.
+        Should be one of `GENEVE`, `HTTP`, `HTTPS`, `TCP`, `TCP_UDP`, `TLS`, or `UDP`.
+        Required when `target_type` is `instance`, `ip`, or `alb`.
+        Does not apply when `target_type` is `lambda`.
         """
         return pulumi.get(self, "protocol")
 
     @protocol.setter
     def protocol(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "protocol", value)
 
@@ -2462,15 +2722,17 @@
     def target_health_states(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.TargetGroupTargetHealthStateArgs']]]]):
         pulumi.set(self, "target_health_states", value)
 
     @property
     @pulumi.getter(name="targetType")
     def target_type(self) -> Optional[pulumi.Input[str]]:
         """
-        Type of target that you must specify when registering targets with this target group. See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_CreateTargetGroup.html) for supported values. The default is `instance`.
+        Type of target that you must specify when registering targets with this target group.
+        See [doc](https://docs.aws.amazon.com/elasticloadbalancing/latest/APIReference/API_CreateTargetGroup.html) for supported values.
+        The default is `instance`.
 
         Note that you can't specify targets for a target group using both instance IDs and IP addresses.
 
         If the target type is `ip`, specify IP addresses from the subnets of the virtual private cloud (VPC) for the target group, the RFC 1918 range (10.0.0.0/8, 172.16.0.0/12, and 192.168.0.0/16), and the RFC 6598 range (100.64.0.0/10). You can't specify publicly routable IP addresses.
 
         Network Load Balancers do not support the `lambda` target type.
```

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/lb/application_load_balancer.py` & `pulumi_awsx-2.9.0/pulumi_awsx/lb/application_load_balancer.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,26 +14,29 @@
 
 __all__ = ['ApplicationLoadBalancerArgs', 'ApplicationLoadBalancer']
 
 @pulumi.input_type
 class ApplicationLoadBalancerArgs:
     def __init__(__self__, *,
                  access_logs: Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs']] = None,
+                 client_keep_alive: Optional[pulumi.Input[int]] = None,
+                 connection_logs: Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerConnectionLogsArgs']] = None,
                  customer_owned_ipv4_pool: Optional[pulumi.Input[str]] = None,
                  default_security_group: Optional['_awsx.DefaultSecurityGroupArgs'] = None,
                  default_target_group: Optional['TargetGroupArgs'] = None,
                  default_target_group_port: Optional[pulumi.Input[int]] = None,
                  desync_mitigation_mode: Optional[pulumi.Input[str]] = None,
                  dns_record_client_routing_policy: Optional[pulumi.Input[str]] = None,
                  drop_invalid_header_fields: Optional[pulumi.Input[bool]] = None,
                  enable_deletion_protection: Optional[pulumi.Input[bool]] = None,
                  enable_http2: Optional[pulumi.Input[bool]] = None,
                  enable_tls_version_and_cipher_suite_headers: Optional[pulumi.Input[bool]] = None,
                  enable_waf_fail_open: Optional[pulumi.Input[bool]] = None,
                  enable_xff_client_port: Optional[pulumi.Input[bool]] = None,
+                 enforce_security_group_inbound_rules_on_private_link_traffic: Optional[pulumi.Input[str]] = None,
                  idle_timeout: Optional[pulumi.Input[int]] = None,
                  internal: Optional[pulumi.Input[bool]] = None,
                  ip_address_type: Optional[pulumi.Input[str]] = None,
                  listener: Optional['ListenerArgs'] = None,
                  listeners: Optional[Sequence['ListenerArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
@@ -42,48 +45,51 @@
                  subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  subnet_mappings: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]] = None,
                  subnets: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  xff_header_processing_mode: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a ApplicationLoadBalancer resource.
-        :param pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs'] access_logs: An Access Logs block. Access Logs documented below.
-        :param pulumi.Input[str] customer_owned_ipv4_pool: The ID of the customer owned ipv4 pool to use for this load balancer.
+        :param pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs'] access_logs: Access Logs block. See below.
+        :param pulumi.Input[int] client_keep_alive: Client keep alive value in seconds. The valid range is 60-604800 seconds. The default is 3600 seconds.
+        :param pulumi.Input['pulumi_aws.lb.LoadBalancerConnectionLogsArgs'] connection_logs: Connection Logs block. See below. Only valid for Load Balancers of type `application`.
+        :param pulumi.Input[str] customer_owned_ipv4_pool: ID of the customer owned ipv4 pool to use for this load balancer.
         :param '_awsx.DefaultSecurityGroupArgs' default_security_group: Options for creating a default security group if [securityGroups] not specified.
         :param 'TargetGroupArgs' default_target_group: Options creating a default target group.
         :param pulumi.Input[int] default_target_group_port: Port to use to connect with the target. Valid values are ports 1-65535. Defaults to 80.
-        :param pulumi.Input[str] desync_mitigation_mode: Determines how the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
-        :param pulumi.Input[str] dns_record_client_routing_policy: Indicates how traffic is distributed among the load balancer Availability Zones. Possible values are `any_availability_zone` (default), `availability_zone_affinity`, or `partial_availability_zone_affinity`. See   [Availability Zone DNS affinity](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#zonal-dns-affinity) for additional details. Only valid for `network` type load balancers.
-        :param pulumi.Input[bool] drop_invalid_header_fields: Indicates whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
+        :param pulumi.Input[str] desync_mitigation_mode: How the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
+        :param pulumi.Input[str] dns_record_client_routing_policy: How traffic is distributed among the load balancer Availability Zones. Possible values are `any_availability_zone` (default), `availability_zone_affinity`, or `partial_availability_zone_affinity`. See   [Availability Zone DNS affinity](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#zonal-dns-affinity) for additional details. Only valid for `network` type load balancers.
+        :param pulumi.Input[bool] drop_invalid_header_fields: Whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
         :param pulumi.Input[bool] enable_deletion_protection: If true, deletion of the load balancer will be disabled via the AWS API. This will prevent this provider from deleting the load balancer. Defaults to `false`.
-        :param pulumi.Input[bool] enable_http2: Indicates whether HTTP/2 is enabled in `application` load balancers. Defaults to `true`.
-        :param pulumi.Input[bool] enable_tls_version_and_cipher_suite_headers: Indicates whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
-        :param pulumi.Input[bool] enable_waf_fail_open: Indicates whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
-        :param pulumi.Input[bool] enable_xff_client_port: Indicates whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `false`.
-        :param pulumi.Input[int] idle_timeout: The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
+        :param pulumi.Input[bool] enable_http2: Whether HTTP/2 is enabled in `application` load balancers. Defaults to `true`.
+        :param pulumi.Input[bool] enable_tls_version_and_cipher_suite_headers: Whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
+        :param pulumi.Input[bool] enable_waf_fail_open: Whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
+        :param pulumi.Input[bool] enable_xff_client_port: Whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `false`.
+        :param pulumi.Input[str] enforce_security_group_inbound_rules_on_private_link_traffic: Whether inbound security group rules are enforced for traffic originating from a PrivateLink. Only valid for Load Balancers of type `network`. The possible values are `on` and `off`.
+        :param pulumi.Input[int] idle_timeout: Time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
         :param pulumi.Input[bool] internal: If true, the LB will be internal. Defaults to `false`.
-        :param pulumi.Input[str] ip_address_type: The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
+        :param pulumi.Input[str] ip_address_type: Type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
         :param 'ListenerArgs' listener: A listener to create. Only one of [listener] and [listeners] can be specified.
         :param Sequence['ListenerArgs'] listeners: List of listeners to create. Only one of [listener] and [listeners] can be specified.
-        :param pulumi.Input[str] name: The name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters,
-               must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified,
-               this provider will autogenerate a name beginning with `tf-lb`.
+        :param pulumi.Input[str] name: Name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters, must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified, this provider will autogenerate a name beginning with `tf-lb`.
         :param pulumi.Input[str] name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `name`.
-        :param pulumi.Input[bool] preserve_host_header: Indicates whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: A list of security group IDs to assign to the LB. Only valid for Load Balancers of type `application` or `network`. For load balancers of type `network` security groups cannot be added if none are currently present, and cannot all be removed once added. If either of these conditions are met, this will force a recreation of the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] subnet_ids: A list of subnet IDs to attach to the LB. Subnets
-               cannot be updated for Load Balancers of type `network`. Changing this value
-               for load balancers of type `network` will force a recreation of the resource.
-        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]] subnet_mappings: A subnet mapping block as documented below.
+        :param pulumi.Input[bool] preserve_host_header: Whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: List of security group IDs to assign to the LB. Only valid for Load Balancers of type `application` or `network`. For load balancers of type `network` security groups cannot be added if none are currently present, and cannot all be removed once added. If either of these conditions are met, this will force a recreation of the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] subnet_ids: List of subnet IDs to attach to the LB. For Load Balancers of type `network` subnets can only be added (see [Availability Zones](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#availability-zones)), deleting a subnet for load balancers of type `network` will force a recreation of the resource.
+        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]] subnet_mappings: Subnet mapping block. See below. For Load Balancers of type `network` subnet mappings can only be added.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]] subnets: A list of subnets to attach to the LB. Only one of [subnets], [subnetIds] or [subnetMappings] can be specified
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param pulumi.Input[str] xff_header_processing_mode: Determines how the load balancer modifies the `X-Forwarded-For` header in the HTTP request before sending the request to the target. The possible values are `append`, `preserve`, and `remove`. Only valid for Load Balancers of type `application`. The default is `append`.
         """
         if access_logs is not None:
             pulumi.set(__self__, "access_logs", access_logs)
+        if client_keep_alive is not None:
+            pulumi.set(__self__, "client_keep_alive", client_keep_alive)
+        if connection_logs is not None:
+            pulumi.set(__self__, "connection_logs", connection_logs)
         if customer_owned_ipv4_pool is not None:
             pulumi.set(__self__, "customer_owned_ipv4_pool", customer_owned_ipv4_pool)
         if default_security_group is not None:
             pulumi.set(__self__, "default_security_group", default_security_group)
         if default_target_group is not None:
             pulumi.set(__self__, "default_target_group", default_target_group)
         if default_target_group_port is not None:
@@ -100,14 +106,16 @@
             pulumi.set(__self__, "enable_http2", enable_http2)
         if enable_tls_version_and_cipher_suite_headers is not None:
             pulumi.set(__self__, "enable_tls_version_and_cipher_suite_headers", enable_tls_version_and_cipher_suite_headers)
         if enable_waf_fail_open is not None:
             pulumi.set(__self__, "enable_waf_fail_open", enable_waf_fail_open)
         if enable_xff_client_port is not None:
             pulumi.set(__self__, "enable_xff_client_port", enable_xff_client_port)
+        if enforce_security_group_inbound_rules_on_private_link_traffic is not None:
+            pulumi.set(__self__, "enforce_security_group_inbound_rules_on_private_link_traffic", enforce_security_group_inbound_rules_on_private_link_traffic)
         if idle_timeout is not None:
             pulumi.set(__self__, "idle_timeout", idle_timeout)
         if internal is not None:
             pulumi.set(__self__, "internal", internal)
         if ip_address_type is not None:
             pulumi.set(__self__, "ip_address_type", ip_address_type)
         if listener is not None:
@@ -133,27 +141,51 @@
         if xff_header_processing_mode is not None:
             pulumi.set(__self__, "xff_header_processing_mode", xff_header_processing_mode)
 
     @property
     @pulumi.getter(name="accessLogs")
     def access_logs(self) -> Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs']]:
         """
-        An Access Logs block. Access Logs documented below.
+        Access Logs block. See below.
         """
         return pulumi.get(self, "access_logs")
 
     @access_logs.setter
     def access_logs(self, value: Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs']]):
         pulumi.set(self, "access_logs", value)
 
     @property
+    @pulumi.getter(name="clientKeepAlive")
+    def client_keep_alive(self) -> Optional[pulumi.Input[int]]:
+        """
+        Client keep alive value in seconds. The valid range is 60-604800 seconds. The default is 3600 seconds.
+        """
+        return pulumi.get(self, "client_keep_alive")
+
+    @client_keep_alive.setter
+    def client_keep_alive(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "client_keep_alive", value)
+
+    @property
+    @pulumi.getter(name="connectionLogs")
+    def connection_logs(self) -> Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerConnectionLogsArgs']]:
+        """
+        Connection Logs block. See below. Only valid for Load Balancers of type `application`.
+        """
+        return pulumi.get(self, "connection_logs")
+
+    @connection_logs.setter
+    def connection_logs(self, value: Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerConnectionLogsArgs']]):
+        pulumi.set(self, "connection_logs", value)
+
+    @property
     @pulumi.getter(name="customerOwnedIpv4Pool")
     def customer_owned_ipv4_pool(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of the customer owned ipv4 pool to use for this load balancer.
+        ID of the customer owned ipv4 pool to use for this load balancer.
         """
         return pulumi.get(self, "customer_owned_ipv4_pool")
 
     @customer_owned_ipv4_pool.setter
     def customer_owned_ipv4_pool(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "customer_owned_ipv4_pool", value)
 
@@ -193,39 +225,39 @@
     def default_target_group_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "default_target_group_port", value)
 
     @property
     @pulumi.getter(name="desyncMitigationMode")
     def desync_mitigation_mode(self) -> Optional[pulumi.Input[str]]:
         """
-        Determines how the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
+        How the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
         """
         return pulumi.get(self, "desync_mitigation_mode")
 
     @desync_mitigation_mode.setter
     def desync_mitigation_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "desync_mitigation_mode", value)
 
     @property
     @pulumi.getter(name="dnsRecordClientRoutingPolicy")
     def dns_record_client_routing_policy(self) -> Optional[pulumi.Input[str]]:
         """
-        Indicates how traffic is distributed among the load balancer Availability Zones. Possible values are `any_availability_zone` (default), `availability_zone_affinity`, or `partial_availability_zone_affinity`. See   [Availability Zone DNS affinity](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#zonal-dns-affinity) for additional details. Only valid for `network` type load balancers.
+        How traffic is distributed among the load balancer Availability Zones. Possible values are `any_availability_zone` (default), `availability_zone_affinity`, or `partial_availability_zone_affinity`. See   [Availability Zone DNS affinity](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#zonal-dns-affinity) for additional details. Only valid for `network` type load balancers.
         """
         return pulumi.get(self, "dns_record_client_routing_policy")
 
     @dns_record_client_routing_policy.setter
     def dns_record_client_routing_policy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dns_record_client_routing_policy", value)
 
     @property
     @pulumi.getter(name="dropInvalidHeaderFields")
     def drop_invalid_header_fields(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
+        Whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
         """
         return pulumi.get(self, "drop_invalid_header_fields")
 
     @drop_invalid_header_fields.setter
     def drop_invalid_header_fields(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "drop_invalid_header_fields", value)
 
@@ -241,63 +273,75 @@
     def enable_deletion_protection(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_deletion_protection", value)
 
     @property
     @pulumi.getter(name="enableHttp2")
     def enable_http2(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates whether HTTP/2 is enabled in `application` load balancers. Defaults to `true`.
+        Whether HTTP/2 is enabled in `application` load balancers. Defaults to `true`.
         """
         return pulumi.get(self, "enable_http2")
 
     @enable_http2.setter
     def enable_http2(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_http2", value)
 
     @property
     @pulumi.getter(name="enableTlsVersionAndCipherSuiteHeaders")
     def enable_tls_version_and_cipher_suite_headers(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
+        Whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
         """
         return pulumi.get(self, "enable_tls_version_and_cipher_suite_headers")
 
     @enable_tls_version_and_cipher_suite_headers.setter
     def enable_tls_version_and_cipher_suite_headers(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_tls_version_and_cipher_suite_headers", value)
 
     @property
     @pulumi.getter(name="enableWafFailOpen")
     def enable_waf_fail_open(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
+        Whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
         """
         return pulumi.get(self, "enable_waf_fail_open")
 
     @enable_waf_fail_open.setter
     def enable_waf_fail_open(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_waf_fail_open", value)
 
     @property
     @pulumi.getter(name="enableXffClientPort")
     def enable_xff_client_port(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `false`.
+        Whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `false`.
         """
         return pulumi.get(self, "enable_xff_client_port")
 
     @enable_xff_client_port.setter
     def enable_xff_client_port(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_xff_client_port", value)
 
     @property
+    @pulumi.getter(name="enforceSecurityGroupInboundRulesOnPrivateLinkTraffic")
+    def enforce_security_group_inbound_rules_on_private_link_traffic(self) -> Optional[pulumi.Input[str]]:
+        """
+        Whether inbound security group rules are enforced for traffic originating from a PrivateLink. Only valid for Load Balancers of type `network`. The possible values are `on` and `off`.
+        """
+        return pulumi.get(self, "enforce_security_group_inbound_rules_on_private_link_traffic")
+
+    @enforce_security_group_inbound_rules_on_private_link_traffic.setter
+    def enforce_security_group_inbound_rules_on_private_link_traffic(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "enforce_security_group_inbound_rules_on_private_link_traffic", value)
+
+    @property
     @pulumi.getter(name="idleTimeout")
     def idle_timeout(self) -> Optional[pulumi.Input[int]]:
         """
-        The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
+        Time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
         """
         return pulumi.get(self, "idle_timeout")
 
     @idle_timeout.setter
     def idle_timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "idle_timeout", value)
 
@@ -313,15 +357,15 @@
     def internal(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "internal", value)
 
     @property
     @pulumi.getter(name="ipAddressType")
     def ip_address_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
+        Type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
         """
         return pulumi.get(self, "ip_address_type")
 
     @ip_address_type.setter
     def ip_address_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ip_address_type", value)
 
@@ -349,17 +393,15 @@
     def listeners(self, value: Optional[Sequence['ListenerArgs']]):
         pulumi.set(self, "listeners", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters,
-        must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified,
-        this provider will autogenerate a name beginning with `tf-lb`.
+        Name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters, must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified, this provider will autogenerate a name beginning with `tf-lb`.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -375,53 +417,51 @@
     def name_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name_prefix", value)
 
     @property
     @pulumi.getter(name="preserveHostHeader")
     def preserve_host_header(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
+        Whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
         """
         return pulumi.get(self, "preserve_host_header")
 
     @preserve_host_header.setter
     def preserve_host_header(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "preserve_host_header", value)
 
     @property
     @pulumi.getter(name="securityGroups")
     def security_groups(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of security group IDs to assign to the LB. Only valid for Load Balancers of type `application` or `network`. For load balancers of type `network` security groups cannot be added if none are currently present, and cannot all be removed once added. If either of these conditions are met, this will force a recreation of the resource.
+        List of security group IDs to assign to the LB. Only valid for Load Balancers of type `application` or `network`. For load balancers of type `network` security groups cannot be added if none are currently present, and cannot all be removed once added. If either of these conditions are met, this will force a recreation of the resource.
         """
         return pulumi.get(self, "security_groups")
 
     @security_groups.setter
     def security_groups(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "security_groups", value)
 
     @property
     @pulumi.getter(name="subnetIds")
     def subnet_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of subnet IDs to attach to the LB. Subnets
-        cannot be updated for Load Balancers of type `network`. Changing this value
-        for load balancers of type `network` will force a recreation of the resource.
+        List of subnet IDs to attach to the LB. For Load Balancers of type `network` subnets can only be added (see [Availability Zones](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#availability-zones)), deleting a subnet for load balancers of type `network` will force a recreation of the resource.
         """
         return pulumi.get(self, "subnet_ids")
 
     @subnet_ids.setter
     def subnet_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "subnet_ids", value)
 
     @property
     @pulumi.getter(name="subnetMappings")
     def subnet_mappings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]]:
         """
-        A subnet mapping block as documented below.
+        Subnet mapping block. See below. For Load Balancers of type `network` subnet mappings can only be added.
         """
         return pulumi.get(self, "subnet_mappings")
 
     @subnet_mappings.setter
     def subnet_mappings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]]):
         pulumi.set(self, "subnet_mappings", value)
 
@@ -437,15 +477,15 @@
     def subnets(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]]]):
         pulumi.set(self, "subnets", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        A map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
+        Map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -464,26 +504,29 @@
 
 class ApplicationLoadBalancer(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_logs: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerAccessLogsArgs']]] = None,
+                 client_keep_alive: Optional[pulumi.Input[int]] = None,
+                 connection_logs: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerConnectionLogsArgs']]] = None,
                  customer_owned_ipv4_pool: Optional[pulumi.Input[str]] = None,
                  default_security_group: Optional[pulumi.InputType['_awsx.DefaultSecurityGroupArgs']] = None,
                  default_target_group: Optional[pulumi.InputType['TargetGroupArgs']] = None,
                  default_target_group_port: Optional[pulumi.Input[int]] = None,
                  desync_mitigation_mode: Optional[pulumi.Input[str]] = None,
                  dns_record_client_routing_policy: Optional[pulumi.Input[str]] = None,
                  drop_invalid_header_fields: Optional[pulumi.Input[bool]] = None,
                  enable_deletion_protection: Optional[pulumi.Input[bool]] = None,
                  enable_http2: Optional[pulumi.Input[bool]] = None,
                  enable_tls_version_and_cipher_suite_headers: Optional[pulumi.Input[bool]] = None,
                  enable_waf_fail_open: Optional[pulumi.Input[bool]] = None,
                  enable_xff_client_port: Optional[pulumi.Input[bool]] = None,
+                 enforce_security_group_inbound_rules_on_private_link_traffic: Optional[pulumi.Input[str]] = None,
                  idle_timeout: Optional[pulumi.Input[int]] = None,
                  internal: Optional[pulumi.Input[bool]] = None,
                  ip_address_type: Optional[pulumi.Input[str]] = None,
                  listener: Optional[pulumi.InputType['ListenerArgs']] = None,
                  listeners: Optional[Sequence[pulumi.InputType['ListenerArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
@@ -496,44 +539,43 @@
                  xff_header_processing_mode: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides an Application Load Balancer resource with listeners, default target group and default security group.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerAccessLogsArgs']] access_logs: An Access Logs block. Access Logs documented below.
-        :param pulumi.Input[str] customer_owned_ipv4_pool: The ID of the customer owned ipv4 pool to use for this load balancer.
+        :param pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerAccessLogsArgs']] access_logs: Access Logs block. See below.
+        :param pulumi.Input[int] client_keep_alive: Client keep alive value in seconds. The valid range is 60-604800 seconds. The default is 3600 seconds.
+        :param pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerConnectionLogsArgs']] connection_logs: Connection Logs block. See below. Only valid for Load Balancers of type `application`.
+        :param pulumi.Input[str] customer_owned_ipv4_pool: ID of the customer owned ipv4 pool to use for this load balancer.
         :param pulumi.InputType['_awsx.DefaultSecurityGroupArgs'] default_security_group: Options for creating a default security group if [securityGroups] not specified.
         :param pulumi.InputType['TargetGroupArgs'] default_target_group: Options creating a default target group.
         :param pulumi.Input[int] default_target_group_port: Port to use to connect with the target. Valid values are ports 1-65535. Defaults to 80.
-        :param pulumi.Input[str] desync_mitigation_mode: Determines how the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
-        :param pulumi.Input[str] dns_record_client_routing_policy: Indicates how traffic is distributed among the load balancer Availability Zones. Possible values are `any_availability_zone` (default), `availability_zone_affinity`, or `partial_availability_zone_affinity`. See   [Availability Zone DNS affinity](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#zonal-dns-affinity) for additional details. Only valid for `network` type load balancers.
-        :param pulumi.Input[bool] drop_invalid_header_fields: Indicates whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
+        :param pulumi.Input[str] desync_mitigation_mode: How the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
+        :param pulumi.Input[str] dns_record_client_routing_policy: How traffic is distributed among the load balancer Availability Zones. Possible values are `any_availability_zone` (default), `availability_zone_affinity`, or `partial_availability_zone_affinity`. See   [Availability Zone DNS affinity](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#zonal-dns-affinity) for additional details. Only valid for `network` type load balancers.
+        :param pulumi.Input[bool] drop_invalid_header_fields: Whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
         :param pulumi.Input[bool] enable_deletion_protection: If true, deletion of the load balancer will be disabled via the AWS API. This will prevent this provider from deleting the load balancer. Defaults to `false`.
-        :param pulumi.Input[bool] enable_http2: Indicates whether HTTP/2 is enabled in `application` load balancers. Defaults to `true`.
-        :param pulumi.Input[bool] enable_tls_version_and_cipher_suite_headers: Indicates whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
-        :param pulumi.Input[bool] enable_waf_fail_open: Indicates whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
-        :param pulumi.Input[bool] enable_xff_client_port: Indicates whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `false`.
-        :param pulumi.Input[int] idle_timeout: The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
+        :param pulumi.Input[bool] enable_http2: Whether HTTP/2 is enabled in `application` load balancers. Defaults to `true`.
+        :param pulumi.Input[bool] enable_tls_version_and_cipher_suite_headers: Whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
+        :param pulumi.Input[bool] enable_waf_fail_open: Whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
+        :param pulumi.Input[bool] enable_xff_client_port: Whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `false`.
+        :param pulumi.Input[str] enforce_security_group_inbound_rules_on_private_link_traffic: Whether inbound security group rules are enforced for traffic originating from a PrivateLink. Only valid for Load Balancers of type `network`. The possible values are `on` and `off`.
+        :param pulumi.Input[int] idle_timeout: Time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
         :param pulumi.Input[bool] internal: If true, the LB will be internal. Defaults to `false`.
-        :param pulumi.Input[str] ip_address_type: The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
+        :param pulumi.Input[str] ip_address_type: Type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
         :param pulumi.InputType['ListenerArgs'] listener: A listener to create. Only one of [listener] and [listeners] can be specified.
         :param Sequence[pulumi.InputType['ListenerArgs']] listeners: List of listeners to create. Only one of [listener] and [listeners] can be specified.
-        :param pulumi.Input[str] name: The name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters,
-               must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified,
-               this provider will autogenerate a name beginning with `tf-lb`.
+        :param pulumi.Input[str] name: Name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters, must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified, this provider will autogenerate a name beginning with `tf-lb`.
         :param pulumi.Input[str] name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `name`.
-        :param pulumi.Input[bool] preserve_host_header: Indicates whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: A list of security group IDs to assign to the LB. Only valid for Load Balancers of type `application` or `network`. For load balancers of type `network` security groups cannot be added if none are currently present, and cannot all be removed once added. If either of these conditions are met, this will force a recreation of the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] subnet_ids: A list of subnet IDs to attach to the LB. Subnets
-               cannot be updated for Load Balancers of type `network`. Changing this value
-               for load balancers of type `network` will force a recreation of the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]] subnet_mappings: A subnet mapping block as documented below.
+        :param pulumi.Input[bool] preserve_host_header: Whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] security_groups: List of security group IDs to assign to the LB. Only valid for Load Balancers of type `application` or `network`. For load balancers of type `network` security groups cannot be added if none are currently present, and cannot all be removed once added. If either of these conditions are met, this will force a recreation of the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] subnet_ids: List of subnet IDs to attach to the LB. For Load Balancers of type `network` subnets can only be added (see [Availability Zones](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#availability-zones)), deleting a subnet for load balancers of type `network` will force a recreation of the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]] subnet_mappings: Subnet mapping block. See below. For Load Balancers of type `network` subnet mappings can only be added.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]] subnets: A list of subnets to attach to the LB. Only one of [subnets], [subnetIds] or [subnetMappings] can be specified
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param pulumi.Input[str] xff_header_processing_mode: Determines how the load balancer modifies the `X-Forwarded-For` header in the HTTP request before sending the request to the target. The possible values are `append`, `preserve`, and `remove`. Only valid for Load Balancers of type `application`. The default is `append`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[ApplicationLoadBalancerArgs] = None,
@@ -553,26 +595,29 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_logs: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerAccessLogsArgs']]] = None,
+                 client_keep_alive: Optional[pulumi.Input[int]] = None,
+                 connection_logs: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerConnectionLogsArgs']]] = None,
                  customer_owned_ipv4_pool: Optional[pulumi.Input[str]] = None,
                  default_security_group: Optional[pulumi.InputType['_awsx.DefaultSecurityGroupArgs']] = None,
                  default_target_group: Optional[pulumi.InputType['TargetGroupArgs']] = None,
                  default_target_group_port: Optional[pulumi.Input[int]] = None,
                  desync_mitigation_mode: Optional[pulumi.Input[str]] = None,
                  dns_record_client_routing_policy: Optional[pulumi.Input[str]] = None,
                  drop_invalid_header_fields: Optional[pulumi.Input[bool]] = None,
                  enable_deletion_protection: Optional[pulumi.Input[bool]] = None,
                  enable_http2: Optional[pulumi.Input[bool]] = None,
                  enable_tls_version_and_cipher_suite_headers: Optional[pulumi.Input[bool]] = None,
                  enable_waf_fail_open: Optional[pulumi.Input[bool]] = None,
                  enable_xff_client_port: Optional[pulumi.Input[bool]] = None,
+                 enforce_security_group_inbound_rules_on_private_link_traffic: Optional[pulumi.Input[str]] = None,
                  idle_timeout: Optional[pulumi.Input[int]] = None,
                  internal: Optional[pulumi.Input[bool]] = None,
                  ip_address_type: Optional[pulumi.Input[str]] = None,
                  listener: Optional[pulumi.InputType['ListenerArgs']] = None,
                  listeners: Optional[Sequence[pulumi.InputType['ListenerArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
@@ -591,26 +636,29 @@
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = ApplicationLoadBalancerArgs.__new__(ApplicationLoadBalancerArgs)
 
             __props__.__dict__["access_logs"] = access_logs
+            __props__.__dict__["client_keep_alive"] = client_keep_alive
+            __props__.__dict__["connection_logs"] = connection_logs
             __props__.__dict__["customer_owned_ipv4_pool"] = customer_owned_ipv4_pool
             __props__.__dict__["default_security_group"] = default_security_group
             __props__.__dict__["default_target_group"] = default_target_group
             __props__.__dict__["default_target_group_port"] = default_target_group_port
             __props__.__dict__["desync_mitigation_mode"] = desync_mitigation_mode
             __props__.__dict__["dns_record_client_routing_policy"] = dns_record_client_routing_policy
             __props__.__dict__["drop_invalid_header_fields"] = drop_invalid_header_fields
             __props__.__dict__["enable_deletion_protection"] = enable_deletion_protection
             __props__.__dict__["enable_http2"] = enable_http2
             __props__.__dict__["enable_tls_version_and_cipher_suite_headers"] = enable_tls_version_and_cipher_suite_headers
             __props__.__dict__["enable_waf_fail_open"] = enable_waf_fail_open
             __props__.__dict__["enable_xff_client_port"] = enable_xff_client_port
+            __props__.__dict__["enforce_security_group_inbound_rules_on_private_link_traffic"] = enforce_security_group_inbound_rules_on_private_link_traffic
             __props__.__dict__["idle_timeout"] = idle_timeout
             __props__.__dict__["internal"] = internal
             __props__.__dict__["ip_address_type"] = ip_address_type
             __props__.__dict__["listener"] = listener
             __props__.__dict__["listeners"] = listeners
             __props__.__dict__["name"] = name
             __props__.__dict__["name_prefix"] = name_prefix
```

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/lb/network_load_balancer.py` & `pulumi_awsx-2.9.0/pulumi_awsx/lb/network_load_balancer.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,25 +13,28 @@
 
 __all__ = ['NetworkLoadBalancerArgs', 'NetworkLoadBalancer']
 
 @pulumi.input_type
 class NetworkLoadBalancerArgs:
     def __init__(__self__, *,
                  access_logs: Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs']] = None,
+                 client_keep_alive: Optional[pulumi.Input[int]] = None,
+                 connection_logs: Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerConnectionLogsArgs']] = None,
                  customer_owned_ipv4_pool: Optional[pulumi.Input[str]] = None,
                  default_target_group: Optional['TargetGroupArgs'] = None,
                  default_target_group_port: Optional[pulumi.Input[int]] = None,
                  desync_mitigation_mode: Optional[pulumi.Input[str]] = None,
                  dns_record_client_routing_policy: Optional[pulumi.Input[str]] = None,
                  drop_invalid_header_fields: Optional[pulumi.Input[bool]] = None,
                  enable_cross_zone_load_balancing: Optional[pulumi.Input[bool]] = None,
                  enable_deletion_protection: Optional[pulumi.Input[bool]] = None,
                  enable_tls_version_and_cipher_suite_headers: Optional[pulumi.Input[bool]] = None,
                  enable_waf_fail_open: Optional[pulumi.Input[bool]] = None,
                  enable_xff_client_port: Optional[pulumi.Input[bool]] = None,
+                 enforce_security_group_inbound_rules_on_private_link_traffic: Optional[pulumi.Input[str]] = None,
                  idle_timeout: Optional[pulumi.Input[int]] = None,
                  internal: Optional[pulumi.Input[bool]] = None,
                  ip_address_type: Optional[pulumi.Input[str]] = None,
                  listener: Optional['ListenerArgs'] = None,
                  listeners: Optional[Sequence['ListenerArgs']] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
@@ -39,46 +42,49 @@
                  subnet_ids: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  subnet_mappings: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]] = None,
                  subnets: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]]] = None,
                  tags: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]] = None,
                  xff_header_processing_mode: Optional[pulumi.Input[str]] = None):
         """
         The set of arguments for constructing a NetworkLoadBalancer resource.
-        :param pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs'] access_logs: An Access Logs block. Access Logs documented below.
-        :param pulumi.Input[str] customer_owned_ipv4_pool: The ID of the customer owned ipv4 pool to use for this load balancer.
+        :param pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs'] access_logs: Access Logs block. See below.
+        :param pulumi.Input[int] client_keep_alive: Client keep alive value in seconds. The valid range is 60-604800 seconds. The default is 3600 seconds.
+        :param pulumi.Input['pulumi_aws.lb.LoadBalancerConnectionLogsArgs'] connection_logs: Connection Logs block. See below. Only valid for Load Balancers of type `application`.
+        :param pulumi.Input[str] customer_owned_ipv4_pool: ID of the customer owned ipv4 pool to use for this load balancer.
         :param 'TargetGroupArgs' default_target_group: Options creating a default target group.
         :param pulumi.Input[int] default_target_group_port: Port to use to connect with the target. Valid values are ports 1-65535. Defaults to 80.
-        :param pulumi.Input[str] desync_mitigation_mode: Determines how the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
-        :param pulumi.Input[str] dns_record_client_routing_policy: Indicates how traffic is distributed among the load balancer Availability Zones. Possible values are `any_availability_zone` (default), `availability_zone_affinity`, or `partial_availability_zone_affinity`. See   [Availability Zone DNS affinity](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#zonal-dns-affinity) for additional details. Only valid for `network` type load balancers.
-        :param pulumi.Input[bool] drop_invalid_header_fields: Indicates whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
+        :param pulumi.Input[str] desync_mitigation_mode: How the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
+        :param pulumi.Input[str] dns_record_client_routing_policy: How traffic is distributed among the load balancer Availability Zones. Possible values are `any_availability_zone` (default), `availability_zone_affinity`, or `partial_availability_zone_affinity`. See   [Availability Zone DNS affinity](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#zonal-dns-affinity) for additional details. Only valid for `network` type load balancers.
+        :param pulumi.Input[bool] drop_invalid_header_fields: Whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
         :param pulumi.Input[bool] enable_cross_zone_load_balancing: If true, cross-zone load balancing of the load balancer will be enabled. For `network` and `gateway` type load balancers, this feature is disabled by default (`false`). For `application` load balancer this feature is always enabled (`true`) and cannot be disabled. Defaults to `false`.
         :param pulumi.Input[bool] enable_deletion_protection: If true, deletion of the load balancer will be disabled via the AWS API. This will prevent this provider from deleting the load balancer. Defaults to `false`.
-        :param pulumi.Input[bool] enable_tls_version_and_cipher_suite_headers: Indicates whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
-        :param pulumi.Input[bool] enable_waf_fail_open: Indicates whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
-        :param pulumi.Input[bool] enable_xff_client_port: Indicates whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `false`.
-        :param pulumi.Input[int] idle_timeout: The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
+        :param pulumi.Input[bool] enable_tls_version_and_cipher_suite_headers: Whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
+        :param pulumi.Input[bool] enable_waf_fail_open: Whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
+        :param pulumi.Input[bool] enable_xff_client_port: Whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `false`.
+        :param pulumi.Input[str] enforce_security_group_inbound_rules_on_private_link_traffic: Whether inbound security group rules are enforced for traffic originating from a PrivateLink. Only valid for Load Balancers of type `network`. The possible values are `on` and `off`.
+        :param pulumi.Input[int] idle_timeout: Time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
         :param pulumi.Input[bool] internal: If true, the LB will be internal. Defaults to `false`.
-        :param pulumi.Input[str] ip_address_type: The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
+        :param pulumi.Input[str] ip_address_type: Type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
         :param 'ListenerArgs' listener: A listener to create. Only one of [listener] and [listeners] can be specified.
         :param Sequence['ListenerArgs'] listeners: List of listeners to create. Only one of [listener] and [listeners] can be specified.
-        :param pulumi.Input[str] name: The name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters,
-               must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified,
-               this provider will autogenerate a name beginning with `tf-lb`.
+        :param pulumi.Input[str] name: Name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters, must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified, this provider will autogenerate a name beginning with `tf-lb`.
         :param pulumi.Input[str] name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `name`.
-        :param pulumi.Input[bool] preserve_host_header: Indicates whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] subnet_ids: A list of subnet IDs to attach to the LB. Subnets
-               cannot be updated for Load Balancers of type `network`. Changing this value
-               for load balancers of type `network` will force a recreation of the resource.
-        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]] subnet_mappings: A subnet mapping block as documented below.
+        :param pulumi.Input[bool] preserve_host_header: Whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] subnet_ids: List of subnet IDs to attach to the LB. For Load Balancers of type `network` subnets can only be added (see [Availability Zones](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#availability-zones)), deleting a subnet for load balancers of type `network` will force a recreation of the resource.
+        :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]] subnet_mappings: Subnet mapping block. See below. For Load Balancers of type `network` subnet mappings can only be added.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]] subnets: A list of subnets to attach to the LB. Only one of [subnets], [subnetIds] or [subnetMappings] can be specified
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param pulumi.Input[str] xff_header_processing_mode: Determines how the load balancer modifies the `X-Forwarded-For` header in the HTTP request before sending the request to the target. The possible values are `append`, `preserve`, and `remove`. Only valid for Load Balancers of type `application`. The default is `append`.
         """
         if access_logs is not None:
             pulumi.set(__self__, "access_logs", access_logs)
+        if client_keep_alive is not None:
+            pulumi.set(__self__, "client_keep_alive", client_keep_alive)
+        if connection_logs is not None:
+            pulumi.set(__self__, "connection_logs", connection_logs)
         if customer_owned_ipv4_pool is not None:
             pulumi.set(__self__, "customer_owned_ipv4_pool", customer_owned_ipv4_pool)
         if default_target_group is not None:
             pulumi.set(__self__, "default_target_group", default_target_group)
         if default_target_group_port is not None:
             pulumi.set(__self__, "default_target_group_port", default_target_group_port)
         if desync_mitigation_mode is not None:
@@ -93,14 +99,16 @@
             pulumi.set(__self__, "enable_deletion_protection", enable_deletion_protection)
         if enable_tls_version_and_cipher_suite_headers is not None:
             pulumi.set(__self__, "enable_tls_version_and_cipher_suite_headers", enable_tls_version_and_cipher_suite_headers)
         if enable_waf_fail_open is not None:
             pulumi.set(__self__, "enable_waf_fail_open", enable_waf_fail_open)
         if enable_xff_client_port is not None:
             pulumi.set(__self__, "enable_xff_client_port", enable_xff_client_port)
+        if enforce_security_group_inbound_rules_on_private_link_traffic is not None:
+            pulumi.set(__self__, "enforce_security_group_inbound_rules_on_private_link_traffic", enforce_security_group_inbound_rules_on_private_link_traffic)
         if idle_timeout is not None:
             pulumi.set(__self__, "idle_timeout", idle_timeout)
         if internal is not None:
             pulumi.set(__self__, "internal", internal)
         if ip_address_type is not None:
             pulumi.set(__self__, "ip_address_type", ip_address_type)
         if listener is not None:
@@ -124,27 +132,51 @@
         if xff_header_processing_mode is not None:
             pulumi.set(__self__, "xff_header_processing_mode", xff_header_processing_mode)
 
     @property
     @pulumi.getter(name="accessLogs")
     def access_logs(self) -> Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs']]:
         """
-        An Access Logs block. Access Logs documented below.
+        Access Logs block. See below.
         """
         return pulumi.get(self, "access_logs")
 
     @access_logs.setter
     def access_logs(self, value: Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerAccessLogsArgs']]):
         pulumi.set(self, "access_logs", value)
 
     @property
+    @pulumi.getter(name="clientKeepAlive")
+    def client_keep_alive(self) -> Optional[pulumi.Input[int]]:
+        """
+        Client keep alive value in seconds. The valid range is 60-604800 seconds. The default is 3600 seconds.
+        """
+        return pulumi.get(self, "client_keep_alive")
+
+    @client_keep_alive.setter
+    def client_keep_alive(self, value: Optional[pulumi.Input[int]]):
+        pulumi.set(self, "client_keep_alive", value)
+
+    @property
+    @pulumi.getter(name="connectionLogs")
+    def connection_logs(self) -> Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerConnectionLogsArgs']]:
+        """
+        Connection Logs block. See below. Only valid for Load Balancers of type `application`.
+        """
+        return pulumi.get(self, "connection_logs")
+
+    @connection_logs.setter
+    def connection_logs(self, value: Optional[pulumi.Input['pulumi_aws.lb.LoadBalancerConnectionLogsArgs']]):
+        pulumi.set(self, "connection_logs", value)
+
+    @property
     @pulumi.getter(name="customerOwnedIpv4Pool")
     def customer_owned_ipv4_pool(self) -> Optional[pulumi.Input[str]]:
         """
-        The ID of the customer owned ipv4 pool to use for this load balancer.
+        ID of the customer owned ipv4 pool to use for this load balancer.
         """
         return pulumi.get(self, "customer_owned_ipv4_pool")
 
     @customer_owned_ipv4_pool.setter
     def customer_owned_ipv4_pool(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "customer_owned_ipv4_pool", value)
 
@@ -172,39 +204,39 @@
     def default_target_group_port(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "default_target_group_port", value)
 
     @property
     @pulumi.getter(name="desyncMitigationMode")
     def desync_mitigation_mode(self) -> Optional[pulumi.Input[str]]:
         """
-        Determines how the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
+        How the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
         """
         return pulumi.get(self, "desync_mitigation_mode")
 
     @desync_mitigation_mode.setter
     def desync_mitigation_mode(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "desync_mitigation_mode", value)
 
     @property
     @pulumi.getter(name="dnsRecordClientRoutingPolicy")
     def dns_record_client_routing_policy(self) -> Optional[pulumi.Input[str]]:
         """
-        Indicates how traffic is distributed among the load balancer Availability Zones. Possible values are `any_availability_zone` (default), `availability_zone_affinity`, or `partial_availability_zone_affinity`. See   [Availability Zone DNS affinity](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#zonal-dns-affinity) for additional details. Only valid for `network` type load balancers.
+        How traffic is distributed among the load balancer Availability Zones. Possible values are `any_availability_zone` (default), `availability_zone_affinity`, or `partial_availability_zone_affinity`. See   [Availability Zone DNS affinity](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#zonal-dns-affinity) for additional details. Only valid for `network` type load balancers.
         """
         return pulumi.get(self, "dns_record_client_routing_policy")
 
     @dns_record_client_routing_policy.setter
     def dns_record_client_routing_policy(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "dns_record_client_routing_policy", value)
 
     @property
     @pulumi.getter(name="dropInvalidHeaderFields")
     def drop_invalid_header_fields(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
+        Whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
         """
         return pulumi.get(self, "drop_invalid_header_fields")
 
     @drop_invalid_header_fields.setter
     def drop_invalid_header_fields(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "drop_invalid_header_fields", value)
 
@@ -232,51 +264,63 @@
     def enable_deletion_protection(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_deletion_protection", value)
 
     @property
     @pulumi.getter(name="enableTlsVersionAndCipherSuiteHeaders")
     def enable_tls_version_and_cipher_suite_headers(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
+        Whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
         """
         return pulumi.get(self, "enable_tls_version_and_cipher_suite_headers")
 
     @enable_tls_version_and_cipher_suite_headers.setter
     def enable_tls_version_and_cipher_suite_headers(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_tls_version_and_cipher_suite_headers", value)
 
     @property
     @pulumi.getter(name="enableWafFailOpen")
     def enable_waf_fail_open(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
+        Whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
         """
         return pulumi.get(self, "enable_waf_fail_open")
 
     @enable_waf_fail_open.setter
     def enable_waf_fail_open(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_waf_fail_open", value)
 
     @property
     @pulumi.getter(name="enableXffClientPort")
     def enable_xff_client_port(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `false`.
+        Whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `false`.
         """
         return pulumi.get(self, "enable_xff_client_port")
 
     @enable_xff_client_port.setter
     def enable_xff_client_port(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "enable_xff_client_port", value)
 
     @property
+    @pulumi.getter(name="enforceSecurityGroupInboundRulesOnPrivateLinkTraffic")
+    def enforce_security_group_inbound_rules_on_private_link_traffic(self) -> Optional[pulumi.Input[str]]:
+        """
+        Whether inbound security group rules are enforced for traffic originating from a PrivateLink. Only valid for Load Balancers of type `network`. The possible values are `on` and `off`.
+        """
+        return pulumi.get(self, "enforce_security_group_inbound_rules_on_private_link_traffic")
+
+    @enforce_security_group_inbound_rules_on_private_link_traffic.setter
+    def enforce_security_group_inbound_rules_on_private_link_traffic(self, value: Optional[pulumi.Input[str]]):
+        pulumi.set(self, "enforce_security_group_inbound_rules_on_private_link_traffic", value)
+
+    @property
     @pulumi.getter(name="idleTimeout")
     def idle_timeout(self) -> Optional[pulumi.Input[int]]:
         """
-        The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
+        Time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
         """
         return pulumi.get(self, "idle_timeout")
 
     @idle_timeout.setter
     def idle_timeout(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "idle_timeout", value)
 
@@ -292,15 +336,15 @@
     def internal(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "internal", value)
 
     @property
     @pulumi.getter(name="ipAddressType")
     def ip_address_type(self) -> Optional[pulumi.Input[str]]:
         """
-        The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
+        Type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
         """
         return pulumi.get(self, "ip_address_type")
 
     @ip_address_type.setter
     def ip_address_type(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "ip_address_type", value)
 
@@ -328,17 +372,15 @@
     def listeners(self, value: Optional[Sequence['ListenerArgs']]):
         pulumi.set(self, "listeners", value)
 
     @property
     @pulumi.getter
     def name(self) -> Optional[pulumi.Input[str]]:
         """
-        The name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters,
-        must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified,
-        this provider will autogenerate a name beginning with `tf-lb`.
+        Name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters, must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified, this provider will autogenerate a name beginning with `tf-lb`.
         """
         return pulumi.get(self, "name")
 
     @name.setter
     def name(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name", value)
 
@@ -354,41 +396,39 @@
     def name_prefix(self, value: Optional[pulumi.Input[str]]):
         pulumi.set(self, "name_prefix", value)
 
     @property
     @pulumi.getter(name="preserveHostHeader")
     def preserve_host_header(self) -> Optional[pulumi.Input[bool]]:
         """
-        Indicates whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
+        Whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
         """
         return pulumi.get(self, "preserve_host_header")
 
     @preserve_host_header.setter
     def preserve_host_header(self, value: Optional[pulumi.Input[bool]]):
         pulumi.set(self, "preserve_host_header", value)
 
     @property
     @pulumi.getter(name="subnetIds")
     def subnet_ids(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
-        A list of subnet IDs to attach to the LB. Subnets
-        cannot be updated for Load Balancers of type `network`. Changing this value
-        for load balancers of type `network` will force a recreation of the resource.
+        List of subnet IDs to attach to the LB. For Load Balancers of type `network` subnets can only be added (see [Availability Zones](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#availability-zones)), deleting a subnet for load balancers of type `network` will force a recreation of the resource.
         """
         return pulumi.get(self, "subnet_ids")
 
     @subnet_ids.setter
     def subnet_ids(self, value: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]):
         pulumi.set(self, "subnet_ids", value)
 
     @property
     @pulumi.getter(name="subnetMappings")
     def subnet_mappings(self) -> Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]]:
         """
-        A subnet mapping block as documented below.
+        Subnet mapping block. See below. For Load Balancers of type `network` subnet mappings can only be added.
         """
         return pulumi.get(self, "subnet_mappings")
 
     @subnet_mappings.setter
     def subnet_mappings(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]]):
         pulumi.set(self, "subnet_mappings", value)
 
@@ -404,15 +444,15 @@
     def subnets(self, value: Optional[pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]]]):
         pulumi.set(self, "subnets", value)
 
     @property
     @pulumi.getter
     def tags(self) -> Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]:
         """
-        A map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
+        Map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         """
         return pulumi.get(self, "tags")
 
     @tags.setter
     def tags(self, value: Optional[pulumi.Input[Mapping[str, pulumi.Input[str]]]]):
         pulumi.set(self, "tags", value)
 
@@ -431,25 +471,28 @@
 
 class NetworkLoadBalancer(pulumi.ComponentResource):
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_logs: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerAccessLogsArgs']]] = None,
+                 client_keep_alive: Optional[pulumi.Input[int]] = None,
+                 connection_logs: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerConnectionLogsArgs']]] = None,
                  customer_owned_ipv4_pool: Optional[pulumi.Input[str]] = None,
                  default_target_group: Optional[pulumi.InputType['TargetGroupArgs']] = None,
                  default_target_group_port: Optional[pulumi.Input[int]] = None,
                  desync_mitigation_mode: Optional[pulumi.Input[str]] = None,
                  dns_record_client_routing_policy: Optional[pulumi.Input[str]] = None,
                  drop_invalid_header_fields: Optional[pulumi.Input[bool]] = None,
                  enable_cross_zone_load_balancing: Optional[pulumi.Input[bool]] = None,
                  enable_deletion_protection: Optional[pulumi.Input[bool]] = None,
                  enable_tls_version_and_cipher_suite_headers: Optional[pulumi.Input[bool]] = None,
                  enable_waf_fail_open: Optional[pulumi.Input[bool]] = None,
                  enable_xff_client_port: Optional[pulumi.Input[bool]] = None,
+                 enforce_security_group_inbound_rules_on_private_link_traffic: Optional[pulumi.Input[str]] = None,
                  idle_timeout: Optional[pulumi.Input[int]] = None,
                  internal: Optional[pulumi.Input[bool]] = None,
                  ip_address_type: Optional[pulumi.Input[str]] = None,
                  listener: Optional[pulumi.InputType['ListenerArgs']] = None,
                  listeners: Optional[Sequence[pulumi.InputType['ListenerArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
@@ -461,42 +504,41 @@
                  xff_header_processing_mode: Optional[pulumi.Input[str]] = None,
                  __props__=None):
         """
         Provides a Network Load Balancer resource with listeners and default target group.
 
         :param str resource_name: The name of the resource.
         :param pulumi.ResourceOptions opts: Options for the resource.
-        :param pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerAccessLogsArgs']] access_logs: An Access Logs block. Access Logs documented below.
-        :param pulumi.Input[str] customer_owned_ipv4_pool: The ID of the customer owned ipv4 pool to use for this load balancer.
+        :param pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerAccessLogsArgs']] access_logs: Access Logs block. See below.
+        :param pulumi.Input[int] client_keep_alive: Client keep alive value in seconds. The valid range is 60-604800 seconds. The default is 3600 seconds.
+        :param pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerConnectionLogsArgs']] connection_logs: Connection Logs block. See below. Only valid for Load Balancers of type `application`.
+        :param pulumi.Input[str] customer_owned_ipv4_pool: ID of the customer owned ipv4 pool to use for this load balancer.
         :param pulumi.InputType['TargetGroupArgs'] default_target_group: Options creating a default target group.
         :param pulumi.Input[int] default_target_group_port: Port to use to connect with the target. Valid values are ports 1-65535. Defaults to 80.
-        :param pulumi.Input[str] desync_mitigation_mode: Determines how the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
-        :param pulumi.Input[str] dns_record_client_routing_policy: Indicates how traffic is distributed among the load balancer Availability Zones. Possible values are `any_availability_zone` (default), `availability_zone_affinity`, or `partial_availability_zone_affinity`. See   [Availability Zone DNS affinity](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#zonal-dns-affinity) for additional details. Only valid for `network` type load balancers.
-        :param pulumi.Input[bool] drop_invalid_header_fields: Indicates whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
+        :param pulumi.Input[str] desync_mitigation_mode: How the load balancer handles requests that might pose a security risk to an application due to HTTP desync. Valid values are `monitor`, `defensive` (default), `strictest`.
+        :param pulumi.Input[str] dns_record_client_routing_policy: How traffic is distributed among the load balancer Availability Zones. Possible values are `any_availability_zone` (default), `availability_zone_affinity`, or `partial_availability_zone_affinity`. See   [Availability Zone DNS affinity](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#zonal-dns-affinity) for additional details. Only valid for `network` type load balancers.
+        :param pulumi.Input[bool] drop_invalid_header_fields: Whether HTTP headers with header fields that are not valid are removed by the load balancer (true) or routed to targets (false). The default is false. Elastic Load Balancing requires that message header names contain only alphanumeric characters and hyphens. Only valid for Load Balancers of type `application`.
         :param pulumi.Input[bool] enable_cross_zone_load_balancing: If true, cross-zone load balancing of the load balancer will be enabled. For `network` and `gateway` type load balancers, this feature is disabled by default (`false`). For `application` load balancer this feature is always enabled (`true`) and cannot be disabled. Defaults to `false`.
         :param pulumi.Input[bool] enable_deletion_protection: If true, deletion of the load balancer will be disabled via the AWS API. This will prevent this provider from deleting the load balancer. Defaults to `false`.
-        :param pulumi.Input[bool] enable_tls_version_and_cipher_suite_headers: Indicates whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
-        :param pulumi.Input[bool] enable_waf_fail_open: Indicates whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
-        :param pulumi.Input[bool] enable_xff_client_port: Indicates whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `false`.
-        :param pulumi.Input[int] idle_timeout: The time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
+        :param pulumi.Input[bool] enable_tls_version_and_cipher_suite_headers: Whether the two headers (`x-amzn-tls-version` and `x-amzn-tls-cipher-suite`), which contain information about the negotiated TLS version and cipher suite, are added to the client request before sending it to the target. Only valid for Load Balancers of type `application`. Defaults to `false`
+        :param pulumi.Input[bool] enable_waf_fail_open: Whether to allow a WAF-enabled load balancer to route requests to targets if it is unable to forward the request to AWS WAF. Defaults to `false`.
+        :param pulumi.Input[bool] enable_xff_client_port: Whether the X-Forwarded-For header should preserve the source port that the client used to connect to the load balancer in `application` load balancers. Defaults to `false`.
+        :param pulumi.Input[str] enforce_security_group_inbound_rules_on_private_link_traffic: Whether inbound security group rules are enforced for traffic originating from a PrivateLink. Only valid for Load Balancers of type `network`. The possible values are `on` and `off`.
+        :param pulumi.Input[int] idle_timeout: Time in seconds that the connection is allowed to be idle. Only valid for Load Balancers of type `application`. Default: 60.
         :param pulumi.Input[bool] internal: If true, the LB will be internal. Defaults to `false`.
-        :param pulumi.Input[str] ip_address_type: The type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
+        :param pulumi.Input[str] ip_address_type: Type of IP addresses used by the subnets for your load balancer. The possible values are `ipv4` and `dualstack`.
         :param pulumi.InputType['ListenerArgs'] listener: A listener to create. Only one of [listener] and [listeners] can be specified.
         :param Sequence[pulumi.InputType['ListenerArgs']] listeners: List of listeners to create. Only one of [listener] and [listeners] can be specified.
-        :param pulumi.Input[str] name: The name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters,
-               must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified,
-               this provider will autogenerate a name beginning with `tf-lb`.
+        :param pulumi.Input[str] name: Name of the LB. This name must be unique within your AWS account, can have a maximum of 32 characters, must contain only alphanumeric characters or hyphens, and must not begin or end with a hyphen. If not specified, this provider will autogenerate a name beginning with `tf-lb`.
         :param pulumi.Input[str] name_prefix: Creates a unique name beginning with the specified prefix. Conflicts with `name`.
-        :param pulumi.Input[bool] preserve_host_header: Indicates whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
-        :param pulumi.Input[Sequence[pulumi.Input[str]]] subnet_ids: A list of subnet IDs to attach to the LB. Subnets
-               cannot be updated for Load Balancers of type `network`. Changing this value
-               for load balancers of type `network` will force a recreation of the resource.
-        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]] subnet_mappings: A subnet mapping block as documented below.
+        :param pulumi.Input[bool] preserve_host_header: Whether the Application Load Balancer should preserve the Host header in the HTTP request and send it to the target without any change. Defaults to `false`.
+        :param pulumi.Input[Sequence[pulumi.Input[str]]] subnet_ids: List of subnet IDs to attach to the LB. For Load Balancers of type `network` subnets can only be added (see [Availability Zones](https://docs.aws.amazon.com/elasticloadbalancing/latest/network/network-load-balancers.html#availability-zones)), deleting a subnet for load balancers of type `network` will force a recreation of the resource.
+        :param pulumi.Input[Sequence[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerSubnetMappingArgs']]]] subnet_mappings: Subnet mapping block. See below. For Load Balancers of type `network` subnet mappings can only be added.
         :param pulumi.Input[Sequence[pulumi.Input['pulumi_aws.ec2.Subnet']]] subnets: A list of subnets to attach to the LB. Only one of [subnets], [subnetIds] or [subnetMappings] can be specified
-        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: A map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
+        :param pulumi.Input[Mapping[str, pulumi.Input[str]]] tags: Map of tags to assign to the resource. If configured with a provider `default_tags` configuration block present, tags with matching keys will overwrite those defined at the provider-level.
         :param pulumi.Input[str] xff_header_processing_mode: Determines how the load balancer modifies the `X-Forwarded-For` header in the HTTP request before sending the request to the target. The possible values are `append`, `preserve`, and `remove`. Only valid for Load Balancers of type `application`. The default is `append`.
         """
         ...
     @overload
     def __init__(__self__,
                  resource_name: str,
                  args: Optional[NetworkLoadBalancerArgs] = None,
@@ -516,25 +558,28 @@
         else:
             __self__._internal_init(resource_name, *args, **kwargs)
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  access_logs: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerAccessLogsArgs']]] = None,
+                 client_keep_alive: Optional[pulumi.Input[int]] = None,
+                 connection_logs: Optional[pulumi.Input[pulumi.InputType['pulumi_aws.lb.LoadBalancerConnectionLogsArgs']]] = None,
                  customer_owned_ipv4_pool: Optional[pulumi.Input[str]] = None,
                  default_target_group: Optional[pulumi.InputType['TargetGroupArgs']] = None,
                  default_target_group_port: Optional[pulumi.Input[int]] = None,
                  desync_mitigation_mode: Optional[pulumi.Input[str]] = None,
                  dns_record_client_routing_policy: Optional[pulumi.Input[str]] = None,
                  drop_invalid_header_fields: Optional[pulumi.Input[bool]] = None,
                  enable_cross_zone_load_balancing: Optional[pulumi.Input[bool]] = None,
                  enable_deletion_protection: Optional[pulumi.Input[bool]] = None,
                  enable_tls_version_and_cipher_suite_headers: Optional[pulumi.Input[bool]] = None,
                  enable_waf_fail_open: Optional[pulumi.Input[bool]] = None,
                  enable_xff_client_port: Optional[pulumi.Input[bool]] = None,
+                 enforce_security_group_inbound_rules_on_private_link_traffic: Optional[pulumi.Input[str]] = None,
                  idle_timeout: Optional[pulumi.Input[int]] = None,
                  internal: Optional[pulumi.Input[bool]] = None,
                  ip_address_type: Optional[pulumi.Input[str]] = None,
                  listener: Optional[pulumi.InputType['ListenerArgs']] = None,
                  listeners: Optional[Sequence[pulumi.InputType['ListenerArgs']]] = None,
                  name: Optional[pulumi.Input[str]] = None,
                  name_prefix: Optional[pulumi.Input[str]] = None,
@@ -552,25 +597,28 @@
             raise ValueError('ComponentResource classes do not support opts.id')
         else:
             if __props__ is not None:
                 raise TypeError('__props__ is only valid when passed in combination with a valid opts.id to get an existing resource')
             __props__ = NetworkLoadBalancerArgs.__new__(NetworkLoadBalancerArgs)
 
             __props__.__dict__["access_logs"] = access_logs
+            __props__.__dict__["client_keep_alive"] = client_keep_alive
+            __props__.__dict__["connection_logs"] = connection_logs
             __props__.__dict__["customer_owned_ipv4_pool"] = customer_owned_ipv4_pool
             __props__.__dict__["default_target_group"] = default_target_group
             __props__.__dict__["default_target_group_port"] = default_target_group_port
             __props__.__dict__["desync_mitigation_mode"] = desync_mitigation_mode
             __props__.__dict__["dns_record_client_routing_policy"] = dns_record_client_routing_policy
             __props__.__dict__["drop_invalid_header_fields"] = drop_invalid_header_fields
             __props__.__dict__["enable_cross_zone_load_balancing"] = enable_cross_zone_load_balancing
             __props__.__dict__["enable_deletion_protection"] = enable_deletion_protection
             __props__.__dict__["enable_tls_version_and_cipher_suite_headers"] = enable_tls_version_and_cipher_suite_headers
             __props__.__dict__["enable_waf_fail_open"] = enable_waf_fail_open
             __props__.__dict__["enable_xff_client_port"] = enable_xff_client_port
+            __props__.__dict__["enforce_security_group_inbound_rules_on_private_link_traffic"] = enforce_security_group_inbound_rules_on_private_link_traffic
             __props__.__dict__["idle_timeout"] = idle_timeout
             __props__.__dict__["internal"] = internal
             __props__.__dict__["ip_address_type"] = ip_address_type
             __props__.__dict__["listener"] = listener
             __props__.__dict__["listeners"] = listeners
             __props__.__dict__["name"] = name
             __props__.__dict__["name_prefix"] = name_prefix
```

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/lb/target_group_attachment.py` & `pulumi_awsx-2.9.0/pulumi_awsx/lb/target_group_attachment.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx/provider.py` & `pulumi_awsx-2.9.0/pulumi_awsx/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx.egg-info/PKG-INFO` & `pulumi_awsx-2.9.0/pulumi_awsx.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_awsx
-Version: 2.8.0
+Version: 2.9.0
 Summary: Pulumi Amazon Web Services (AWS) AWSX Components.
 License: Apache-2.0
 Project-URL: Homepage, https://pulumi.com
 Project-URL: Repository, https://github.com/pulumi/pulumi-awsx
 Keywords: pulumi,aws,awsx,kind/component,category/cloud
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_awsx-2.8.0/pulumi_awsx.egg-info/SOURCES.txt` & `pulumi_awsx-2.9.0/pulumi_awsx.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_awsx-2.8.0/pyproject.toml` & `pulumi_awsx-2.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_awsx"
   description = "Pulumi Amazon Web Services (AWS) AWSX Components."
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-aws>=6.0.4,<7.0.0", "pulumi-docker>=4.5.1,<5.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "aws", "awsx", "kind/component", "category/cloud"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "2.8.0"
+  version = "2.9.0"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Homepage = "https://pulumi.com"
     Repository = "https://github.com/pulumi/pulumi-awsx"
 
 [build-system]
```

